# Comparing `tmp/xgrid-0.0.1.tar.gz` & `tmp/xgrid-0.0.2.tar.gz`

## Comparing `xgrid-0.0.1.tar` & `xgrid-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 xgrid-0.0.1/requirements.txt
--rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 xgrid-0.0.1/test.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 xgrid-0.0.1/examples/cavity.py
--rw-r--r--   0        0        0   455424 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/cavity.gif
--rw-r--r--   0        0        0   181643 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/cavity.png
--rw-r--r--   0        0        0   181637 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/cavityref.png
--rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/convection_1d.png
--rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/convection_1d_nonlinear.png
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/convection_2d.png
--rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 xgrid-0.0.1/imgs/diffusion_1d.png
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/__init__.py
--rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/generator.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/operator.py
--rw-r--r--   0        0        0    26900 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/parser.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/ir/__init__.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/ir/expression.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/ir/statement.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/lang/ir/visitor.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/__init__.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/console.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/ffi.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/init.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/logging.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/typing/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/typing/annotation.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/typing/reference.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/util/typing/value.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 xgrid-0.0.1/xgrid/xgrid/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 xgrid-0.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 xgrid-0.0.1/LICENSE
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 xgrid-0.0.1/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 xgrid-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 xgrid-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 xgrid-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     9144 2020-02-02 00:00:00.000000 xgrid-0.0.2/test.py
+-rw-r--r--   0        0        0     8574 2020-02-02 00:00:00.000000 xgrid-0.0.2/examples/cavity.py
+-rw-r--r--   0        0        0   455424 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/cavity.gif
+-rw-r--r--   0        0        0   181643 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/cavity.png
+-rw-r--r--   0        0        0   181637 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/cavityref.png
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/convection_1d.png
+-rw-r--r--   0        0        0    14277 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/convection_1d_nonlinear.png
+-rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/convection_2d.png
+-rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 xgrid-0.0.2/imgs/diffusion_1d.png
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/__init__.py
+-rw-r--r--   0        0        0    18300 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/generator.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/operator.py
+-rw-r--r--   0        0        0    27541 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/parser.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/expression.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/statement.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/lang/ir/visitor.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/__init__.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/console.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/ffi.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/init.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/logging.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/__init__.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/annotation.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/reference.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/util/typing/value.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 xgrid-0.0.2/xgrid/xgrid/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 xgrid-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 xgrid-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 xgrid-0.0.2/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 xgrid-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xgrid-0.0.2/PKG-INFO
```

### Comparing `xgrid-0.0.1/requirements.txt` & `xgrid-0.0.2/requirements.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-autopep8==2.0.2
-blinker==1.4
-cffi==1.15.1
-command-not-found==0.3
-cryptography==3.4.8
-dbus-python==1.2.18
-distro==1.7.0
-distro-info===1.1build1
-httplib2==0.20.2
-importlib-metadata==4.6.4
-jeepney==0.7.1
-keyring==23.5.0
-launchpadlib==1.10.16
-lazr.restfulclient==0.14.4
-lazr.uri==1.0.6
-more-itertools==8.10.0
-netifaces==0.11.0
-numpy==1.24.2
-oauthlib==3.2.0
-pycodestyle==2.10.0
-pycparser==2.21
-Pygments==2.11.2
-PyGObject==3.42.1
-PyJWT==2.3.0
-pyparsing==2.4.7
-python-apt==2.4.0+ubuntu1
-PyYAML==5.4.1
-SecretStorage==3.3.1
-six==1.16.0
-systemd-python==234
-tomli==2.0.1
-tqdm==4.65.0
-ubuntu-advantage-tools==8001
-ufw==0.36.1
-unattended-upgrades==0.1
-wadllib==1.3.6
-zipp==1.0.0
+autopep8==2.0.2
+blinker==1.4
+cffi==1.15.1
+command-not-found==0.3
+cryptography==3.4.8
+dbus-python==1.2.18
+distro==1.7.0
+distro-info===1.1build1
+httplib2==0.20.2
+importlib-metadata==4.6.4
+jeepney==0.7.1
+keyring==23.5.0
+launchpadlib==1.10.16
+lazr.restfulclient==0.14.4
+lazr.uri==1.0.6
+more-itertools==8.10.0
+netifaces==0.11.0
+numpy==1.24.2
+oauthlib==3.2.0
+pycodestyle==2.10.0
+pycparser==2.21
+Pygments==2.11.2
+PyGObject==3.42.1
+PyJWT==2.3.0
+pyparsing==2.4.7
+python-apt==2.4.0+ubuntu1
+PyYAML==5.4.1
+SecretStorage==3.3.1
+six==1.16.0
+systemd-python==234
+tomli==2.0.1
+tqdm==4.65.0
+ubuntu-advantage-tools==8001
+ufw==0.36.1
+unattended-upgrades==0.1
+wadllib==1.3.6
+zipp==1.0.0
```

### Comparing `xgrid-0.0.1/test.py` & `xgrid-0.0.2/test.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,319 +1,319 @@
-from dataclasses import dataclass
-from io import StringIO
-import os
-import random
-import shutil
-import time
-from typing import Callable
-
-import numpy
-import xgrid
-from xgrid.util.console import Console
-from xgrid.util.ffi import Compiler, Library
-from xgrid.util.logging import Logger
-from xgrid.util.typing.value import Floating
-from matplotlib import pyplot, cm
-
-
-class Test:
-    def __init__(self) -> None:
-        self.total = 0
-        self.tests: list[tuple[str, Callable]] = []
-        self.current_test = ""
-
-    def fact(self, name: str):
-        def decorator(func):
-            self.tests.append((name, func))
-        return decorator
-
-    def log(self, msg: str):
-        print("  \033[1minfo\033[0m:", self.current_test, msg)
-
-    def run(self):
-        def tmp_device():
-            return StringIO(), StringIO()
-
-        test_prompt = "\033[1;34mtest\033[0m: "
-
-        total = len(self.tests)
-        passed_cases: list[tuple[str, str, str]] = []
-        failed_cases: list[tuple[str, tuple[Exception, str, str]]] = []
-
-        total_begin_time = time.time()
-        for id, (name, test) in enumerate(self.tests):
-            test_id = f"{test_prompt}({id + 1}/{total}) {name}"
-            print(test_id)
-
-            out, err = tmp_device()
-            Logger.stdouts[0] = Console(out)
-            Logger.stderrs[0] = Console(err)
-
-            self.current_test = name
-
-            exc = None
-            begin_time = time.time()
-            try:
-                test()
-            except Exception as e:
-                exc = e
-            finally:
-                end_time = time.time()
-                print(
-                    f"    \033[1;{'31mfailed' if exc else '32mpassed'}\033[0m in {(end_time - begin_time):.6f}s")
-                out_msg, err_msg = out.read(), err.read()
-                if exc:
-                    raise exc
-                    failed_cases.append((name, (exc, out_msg, err_msg)))
-                else:
-                    passed_cases.append((name, out_msg, err_msg))
-
-        total_end_time = time.time()
-        print(
-            f"{test_prompt}total {total} tests, \033[1;32m{len(passed_cases)} passed\033[0m, \033[1;31m{len(failed_cases)} failed\033[0m in {total_end_time - total_begin_time:.5f} s")
-        if any(failed_cases):
-            print("    " + ", ".join(map(lambda x: x[0], failed_cases)))
-
-
-test = Test()
-
-
-@test.fact("ffi.Compiler")
-def ffi_compiler() -> None:
-    global lib_name
-
-    cacheroot = ".xgridtest"
-
-    if os.path.exists(f"./{cacheroot}"):
-        test.log(f"remove existed cacheroot {cacheroot}")
-        shutil.rmtree(f"./{cacheroot}", ignore_errors=True)
-
-    cc = Compiler(cacheroot=".xgridtest", cc=["gcc", "clang"])
-
-    assert os.path.exists(f"./{cacheroot}")
-    assert cc.cc == "/usr/bin/gcc", "fetched wrong cc, expect /usr/bin/gcc"
-
-    test.log(
-        f"initialized compiler, cacheroot = {cc.cacheroot}, cc = {cc.cc}")
-
-    simple_src = "#include <stdio.h>\n#include <stdbool.h>\n\nfloat universe(float a, float b) { return a + b; }\nvoid branch(bool a) { if(a) printf(\"branch function from c works fine\\n\"); }"
-
-    cc.compile(simple_src)
-    lib_name = cc.compile(simple_src)
-
-    test.log(
-        f"compiled source file without and with cached library to {lib_name}")
-
-    dead_src = "innt main() {}"
-    try:
-        cc.compile(dead_src)
-    except Exception as e:
-        test.log("compiled source file with syntax error")
-
-
-@test.fact("ffi.Library")
-def ffi_library() -> None:
-    global lib_name
-
-    lib = Library(lib_name)
-
-    test.log(f"library {lib_name} is loaded")
-
-    float_add = lib.function(
-        "universe", [Floating(4), Floating(4)], Floating(4))
-    assert float_add(1.2, 2.3) == 3.5
-    test.log(f"fetched and tested dynamic function 'float universe(float, float)'")
-
-
-TEMP = 10
-
-
-@test.fact("lang.Operator.simple")
-def operator_simple() -> None:
-    @xgrid.kernel()
-    def aux(a: int, b: int) -> int:
-        return a + b + TEMP
-
-    a = random.randint(0, 1000)
-    b = random.randint(0, 1000)
-    test.log(
-        f"execute simple kernel operator, should obtain (a := {a}) + (b := {b}) + (TEMP := 10)")
-    assert aux(a, b) == a + b + TEMP
-
-
-@dataclass
-class Vector3i:
-    x: int
-    y: int
-    z: int
-
-    @xgrid.function(method=True)
-    def dot(self, b: "Vector3i") -> int:
-        return self.x * b.x + self.y * b.y + self.z * b.z
-
-
-@test.fact("lang.Operator.structure")
-def operator_structure() -> None:
-    @xgrid.kernel()
-    def aux(a: Vector3i, b: Vector3i) -> int:
-        return a.dot(b)
-
-    a = Vector3i(random.randint(0, 1000), random.randint(
-        0, 1000), random.randint(0, 1000))
-    b = Vector3i(random.randint(0, 1000), random.randint(
-        0, 1000), random.randint(0, 1000))
-    test.log(f"execute structure kernel operator, should obtain {a} dot {b}")
-    assert aux(a, b) == a.dot(b)
-
-
-@test.fact("lang.Operator.grid")
-def operator_grid() -> None:
-    @xgrid.kernel()
-    def aux(a: xgrid.grid[int, 2]) -> None:  # type: ignore
-        a[0, 0] = 4
-
-    grid = xgrid.Grid((10, 10), dtype=int)
-    aux(grid)
-
-    test.log(f"execute grid kernel operator, should give 4 to each elements")
-    for a in grid.now:
-        for element in a:
-            assert element == 4
-
-
-@test.fact("lang.Operator.grid_indexguard")
-def operator_grid_indexguard() -> None:
-    @xgrid.kernel()
-    def aux(a: xgrid.grid[int, 2]) -> None:  # type: ignore
-        a[0, 0] = a[-1, -1][-1]
-
-    grid = xgrid.Grid((10, 10), dtype=int)
-    aux(grid)
-
-    test.log(f"execute grid kernel operator with index out of range, the program should run smoothly without error message")
-
-
-def initial_convection_1d(x: xgrid.Grid, dx):
-    x.now.fill(1)
-    x.now[int(.5 / dx):int(1 / dx + 1)] = 2
-    x.boundary[0] = 1
-
-
-@test.fact("lang.Operator.convection_1d")
-def operator_convection_1d() -> None:
-    float1d = xgrid.grid[float, 1]  # type: ignore
-
-    nx = 41
-    dx = 2 / (nx - 1)
-    nt = 25
-    dt = .025
-    c = 1
-
-    u = xgrid.Grid((nx,), float)
-    initial_convection_1d(u, dx)
-
-    @xgrid.kernel()
-    def convection_1d(u: float1d, c: float, dt: float, dx: float) -> None:
-        u[0] = u[0] - c * dt / dx * (u[0] - u[-1])
-        with xgrid.boundary(u, 1):
-            u[0] = 1.0
-
-    for _ in range(nt):
-        convection_1d(u, c, dt, dx)
-
-    pyplot.plot(numpy.linspace(0, 2, nx), u.now)
-    pyplot.savefig(f"imgs/convection_1d.png")
-    pyplot.close()
-
-
-@test.fact("lang.Operator.convection_1d_nonlinear")
-def operator_convection_1d_nonlinear() -> None:
-    float1d = xgrid.grid[float, 1]  # type: ignore
-
-    nx = 41
-    dx = 2 / (nx - 1)
-    nt = 10
-    dt = .025
-
-    u = xgrid.Grid((nx,), float)
-    initial_convection_1d(u, dx)
-
-    @xgrid.kernel()
-    def convection_1d(u: float1d, dt: float, dx: float) -> None:
-        u[0] = u[0] - u[0] * dt / dx * (u[0] - u[-1])
-        with xgrid.boundary(u, 1):
-            u[0] = 1.0
-
-    for _ in range(nt):
-        convection_1d(u, dt, dx)
-
-    pyplot.plot(numpy.linspace(0, 2, nx), u.now)
-    pyplot.savefig(f"imgs/convection_1d_nonlinear.png")
-    pyplot.close()
-
-
-@test.fact("lang.Operator.diffusion_1d")
-def operator_diffusion() -> None:
-    float1d = xgrid.grid[float, 1]  # type: ignore
-
-    nx = 41
-    dx = 2 / (nx - 1)
-    nt = 20
-    dt = .01
-    nu = 0.01
-
-    u = xgrid.Grid((nx,), float)
-    u.now.fill(1)
-    u.now[int(.5 / dx):int(1 / dx + 1)] = 2
-    u.boundary[0] = u.boundary[-1] = 1
-
-    @xgrid.kernel()
-    def diffusion_1d(u: float1d, nu: float, dt: float, dx: float) -> None:
-        u[0] = u[0] + nu * dt / dx ** 2.0 * (u[1] - 2.0 * u[0] + u[-1])
-        with xgrid.boundary(u, 1):
-            u[0] = 1.0
-
-    for _ in range(nt):
-        diffusion_1d(u, nu, dt, dx)
-
-    pyplot.plot(numpy.linspace(0, 2, nx), u.now)
-    pyplot.savefig(f"imgs/diffusion_1d.png")
-    pyplot.close()
-
-
-@test.fact("lang.Operator.convection_2d")
-def operator_convection_2d() -> None:
-    float2d = xgrid.grid[float, 2]  # type: ignore
-
-    nx = ny = 101
-    dx = 2 / (nx-1)
-    dy = 2 / (ny-1)
-    c = 1
-    sigma = .5  # from the CLF condition
-    dt = sigma * (dx / c)
-    nt = int(.7/dt)
-
-    u = xgrid.Grid((nx, ny), float)
-    u.now.fill(1)
-    u.now[int(0.5/dx):int(1/dx) + 1, int(0.5/dy):int(1/dy) + 1] = 2
-    u.boundary[0, :] = u.boundary[:, 0] = 1
-
-    @xgrid.kernel()
-    def convection_2d(u: float2d, c: float, dt: float, dx: float, dy: float) -> None:
-        cdx = c * dt / dx
-        cdy = c * dt / dy
-        u[0, 0] = u[0, 0] + cdx * \
-            (u[0, 0] - u[-1, 0]) - cdy * (u[0, 0] - u[0, -1])
-        with xgrid.boundary(u, 1):
-            u[0, 0] = 1.0
-
-    for _ in range(nt):
-        convection_2d(u, c, dt, dx, dy)
-
-    pyplot.imshow(u.now)
-    pyplot.savefig("imgs/convection_2d.png")
-    pyplot.close()
-
-
-xgrid.init(comment=True, cacheroot=".xgridtest",
-           opt_level=3, precision="double")
-test.run()
+from dataclasses import dataclass
+from io import StringIO
+import os
+import random
+import shutil
+import time
+from typing import Callable
+
+import numpy
+import xgrid
+from xgrid.util.console import Console
+from xgrid.util.ffi import Compiler, Library
+from xgrid.util.logging import Logger
+from xgrid.util.typing.value import Floating
+from matplotlib import pyplot, cm
+
+
+class Test:
+    def __init__(self) -> None:
+        self.total = 0
+        self.tests: list[tuple[str, Callable]] = []
+        self.current_test = ""
+
+    def fact(self, name: str):
+        def decorator(func):
+            self.tests.append((name, func))
+        return decorator
+
+    def log(self, msg: str):
+        print("  \033[1minfo\033[0m:", self.current_test, msg)
+
+    def run(self):
+        def tmp_device():
+            return StringIO(), StringIO()
+
+        test_prompt = "\033[1;34mtest\033[0m: "
+
+        total = len(self.tests)
+        passed_cases: list[tuple[str, str, str]] = []
+        failed_cases: list[tuple[str, tuple[Exception, str, str]]] = []
+
+        total_begin_time = time.time()
+        for id, (name, test) in enumerate(self.tests):
+            test_id = f"{test_prompt}({id + 1}/{total}) {name}"
+            print(test_id)
+
+            out, err = tmp_device()
+            Logger.stdouts[0] = Console(out)
+            Logger.stderrs[0] = Console(err)
+
+            self.current_test = name
+
+            exc = None
+            begin_time = time.time()
+            try:
+                test()
+            except Exception as e:
+                exc = e
+            finally:
+                end_time = time.time()
+                print(
+                    f"    \033[1;{'31mfailed' if exc else '32mpassed'}\033[0m in {(end_time - begin_time):.6f}s")
+                out_msg, err_msg = out.read(), err.read()
+                if exc:
+                    raise exc
+                    failed_cases.append((name, (exc, out_msg, err_msg)))
+                else:
+                    passed_cases.append((name, out_msg, err_msg))
+
+        total_end_time = time.time()
+        print(
+            f"{test_prompt}total {total} tests, \033[1;32m{len(passed_cases)} passed\033[0m, \033[1;31m{len(failed_cases)} failed\033[0m in {total_end_time - total_begin_time:.5f} s")
+        if any(failed_cases):
+            print("    " + ", ".join(map(lambda x: x[0], failed_cases)))
+
+
+test = Test()
+
+
+@test.fact("ffi.Compiler")
+def ffi_compiler() -> None:
+    global lib_name
+
+    cacheroot = ".xgridtest"
+
+    if os.path.exists(f"./{cacheroot}"):
+        test.log(f"remove existed cacheroot {cacheroot}")
+        shutil.rmtree(f"./{cacheroot}", ignore_errors=True)
+
+    cc = Compiler(cacheroot=".xgridtest", cc=["gcc", "clang"])
+
+    assert os.path.exists(f"./{cacheroot}")
+    assert cc.cc == "/usr/bin/gcc", "fetched wrong cc, expect /usr/bin/gcc"
+
+    test.log(
+        f"initialized compiler, cacheroot = {cc.cacheroot}, cc = {cc.cc}")
+
+    simple_src = "#include <stdio.h>\n#include <stdbool.h>\n\nfloat universe(float a, float b) { return a + b; }\nvoid branch(bool a) { if(a) printf(\"branch function from c works fine\\n\"); }"
+
+    cc.compile(simple_src)
+    lib_name = cc.compile(simple_src)
+
+    test.log(
+        f"compiled source file without and with cached library to {lib_name}")
+
+    dead_src = "innt main() {}"
+    try:
+        cc.compile(dead_src)
+    except Exception as e:
+        test.log("compiled source file with syntax error")
+
+
+@test.fact("ffi.Library")
+def ffi_library() -> None:
+    global lib_name
+
+    lib = Library(lib_name)
+
+    test.log(f"library {lib_name} is loaded")
+
+    float_add = lib.function(
+        "universe", [Floating(4), Floating(4)], Floating(4))
+    assert float_add(1.2, 2.3) == 3.5
+    test.log(f"fetched and tested dynamic function 'float universe(float, float)'")
+
+
+TEMP = 10
+
+
+@test.fact("lang.Operator.simple")
+def operator_simple() -> None:
+    @xgrid.kernel()
+    def aux(a: int, b: int) -> int:
+        return a + b + TEMP
+
+    a = random.randint(0, 1000)
+    b = random.randint(0, 1000)
+    test.log(
+        f"execute simple kernel operator, should obtain (a := {a}) + (b := {b}) + (TEMP := 10)")
+    assert aux(a, b) == a + b + TEMP
+
+
+@dataclass
+class Vector3i:
+    x: int
+    y: int
+    z: int
+
+    @xgrid.function(method=True)
+    def dot(self, b: "Vector3i") -> int:
+        return self.x * b.x + self.y * b.y + self.z * b.z
+
+
+@test.fact("lang.Operator.structure")
+def operator_structure() -> None:
+    @xgrid.kernel()
+    def aux(a: Vector3i, b: Vector3i) -> int:
+        return a.dot(b)
+
+    a = Vector3i(random.randint(0, 1000), random.randint(
+        0, 1000), random.randint(0, 1000))
+    b = Vector3i(random.randint(0, 1000), random.randint(
+        0, 1000), random.randint(0, 1000))
+    test.log(f"execute structure kernel operator, should obtain {a} dot {b}")
+    assert aux(a, b) == a.dot(b)
+
+
+@test.fact("lang.Operator.grid")
+def operator_grid() -> None:
+    @xgrid.kernel()
+    def aux(a: xgrid.grid[int, 2]) -> None:  # type: ignore
+        a[0, 0] = 4
+
+    grid = xgrid.Grid((10, 10), dtype=int)
+    aux(grid)
+
+    test.log(f"execute grid kernel operator, should give 4 to each elements")
+    for a in grid.now:
+        for element in a:
+            assert element == 4
+
+
+@test.fact("lang.Operator.grid_indexguard")
+def operator_grid_indexguard() -> None:
+    @xgrid.kernel()
+    def aux(a: xgrid.grid[int, 2]) -> None:  # type: ignore
+        a[0, 0] = a[-1, -1][-1]
+
+    grid = xgrid.Grid((10, 10), dtype=int)
+    aux(grid)
+
+    test.log(f"execute grid kernel operator with index out of range, the program should run smoothly without error message")
+
+
+def initial_convection_1d(x: xgrid.Grid, dx):
+    x.now.fill(1)
+    x.now[int(.5 / dx):int(1 / dx + 1)] = 2
+    x.boundary[0] = 1
+
+
+@test.fact("lang.Operator.convection_1d")
+def operator_convection_1d() -> None:
+    float1d = xgrid.grid[float, 1]  # type: ignore
+
+    nx = 41
+    dx = 2 / (nx - 1)
+    nt = 25
+    dt = .025
+    c = 1
+
+    u = xgrid.Grid((nx,), float)
+    initial_convection_1d(u, dx)
+
+    @xgrid.kernel()
+    def convection_1d(u: float1d, c: float, dt: float, dx: float) -> None:
+        u[0] = u[0] - c * dt / dx * (u[0] - u[-1])
+        with xgrid.boundary(u, 1):
+            u[0] = 1.0
+
+    for _ in range(nt):
+        convection_1d(u, c, dt, dx)
+
+    pyplot.plot(numpy.linspace(0, 2, nx), u.now)
+    pyplot.savefig(f"imgs/convection_1d.png")
+    pyplot.close()
+
+
+@test.fact("lang.Operator.convection_1d_nonlinear")
+def operator_convection_1d_nonlinear() -> None:
+    float1d = xgrid.grid[float, 1]  # type: ignore
+
+    nx = 41
+    dx = 2 / (nx - 1)
+    nt = 10
+    dt = .025
+
+    u = xgrid.Grid((nx,), float)
+    initial_convection_1d(u, dx)
+
+    @xgrid.kernel()
+    def convection_1d(u: float1d, dt: float, dx: float) -> None:
+        u[0] = u[0] - u[0] * dt / dx * (u[0] - u[-1])
+        with xgrid.boundary(u, 1):
+            u[0] = 1.0
+
+    for _ in range(nt):
+        convection_1d(u, dt, dx)
+
+    pyplot.plot(numpy.linspace(0, 2, nx), u.now)
+    pyplot.savefig(f"imgs/convection_1d_nonlinear.png")
+    pyplot.close()
+
+
+@test.fact("lang.Operator.diffusion_1d")
+def operator_diffusion() -> None:
+    float1d = xgrid.grid[float, 1]  # type: ignore
+
+    nx = 41
+    dx = 2 / (nx - 1)
+    nt = 20
+    dt = .01
+    nu = 0.01
+
+    u = xgrid.Grid((nx,), float)
+    u.now.fill(1)
+    u.now[int(.5 / dx):int(1 / dx + 1)] = 2
+    u.boundary[0] = u.boundary[-1] = 1
+
+    @xgrid.kernel()
+    def diffusion_1d(u: float1d, nu: float, dt: float, dx: float) -> None:
+        u[0] = u[0] + nu * dt / dx ** 2.0 * (u[1] - 2.0 * u[0] + u[-1])
+        with xgrid.boundary(u, 1):
+            u[0] = 1.0
+
+    for _ in range(nt):
+        diffusion_1d(u, nu, dt, dx)
+
+    pyplot.plot(numpy.linspace(0, 2, nx), u.now)
+    pyplot.savefig(f"imgs/diffusion_1d.png")
+    pyplot.close()
+
+
+@test.fact("lang.Operator.convection_2d")
+def operator_convection_2d() -> None:
+    float2d = xgrid.grid[float, 2]  # type: ignore
+
+    nx = ny = 101
+    dx = 2 / (nx-1)
+    dy = 2 / (ny-1)
+    c = 1
+    sigma = .5  # from the CLF condition
+    dt = sigma * (dx / c)
+    nt = int(.7/dt)
+
+    u = xgrid.Grid((nx, ny), float)
+    u.now.fill(1)
+    u.now[int(0.5/dx):int(1/dx) + 1, int(0.5/dy):int(1/dy) + 1] = 2
+    u.boundary[0, :] = u.boundary[:, 0] = 1
+
+    @xgrid.kernel()
+    def convection_2d(u: float2d, c: float, dt: float, dx: float, dy: float) -> None:
+        cdx = c * dt / dx
+        cdy = c * dt / dy
+        u[0, 0] = u[0, 0] + cdx * \
+            (u[0, 0] - u[-1, 0]) - cdy * (u[0, 0] - u[0, -1])
+        with xgrid.boundary(u, 1):
+            u[0, 0] = 1.0
+
+    for _ in range(nt):
+        convection_2d(u, c, dt, dx, dy)
+
+    pyplot.imshow(u.now)
+    pyplot.savefig("imgs/convection_2d.png")
+    pyplot.close()
+
+
+xgrid.init(comment=True, cacheroot=".xgridtest",
+           opt_level=3, precision="double")
+test.run()
```

### Comparing `xgrid-0.0.1/examples/cavity.py` & `xgrid-0.0.2/examples/cavity.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-from dataclasses import dataclass
-
-import tqdm
-import xgrid
-import numpy
-import time
-
-
-class Timer:
-    class TimerGuard:
-        def __init__(self, timer: "Timer") -> None:
-            self.timer = timer
-
-        def __enter__(self):
-            self.timer.start_time = time.time()
-
-        def __exit__(self, a, b, c):
-            self.timer.end_time = time.time()
-
-    def __init__(self) -> None:
-        self.start_time = time.time()
-        self.end_time = time.time()
-
-    @property
-    def elapsed(self):
-        return self.end_time - self.start_time
-
-    def timing(self):
-        return Timer.TimerGuard(self)
-
-
-timer = Timer()
-
-xgrid.init(cacheroot=".xgridtest", parallel=True, precision="double", opt_level=3)
-
-float2d = xgrid.grid[float, 2]  # type: ignore
-
-
-@dataclass
-class Config:
-    rho: float
-    nu: float
-    dt: float
-    dx: float
-    dy: float
-
-
-SIZE_X = SIZE_Y = 101
-
-u = xgrid.Grid((SIZE_X, SIZE_Y), float)
-v = xgrid.Grid((SIZE_X, SIZE_Y), float)
-p = xgrid.Grid((SIZE_X, SIZE_Y), float)
-b = xgrid.Grid((SIZE_X, SIZE_Y), float)
-
-
-u.boundary[0, :] = u.boundary[:, 0] = u.boundary[:, -1] = 1
-u.boundary[-1, :] = 2
-
-v.boundary.fill(1)
-v.boundary[1:-1, 1:-1] = 0
-
-p.boundary[:, -1] = 1
-p.boundary[0, :] = 2
-p.boundary[:, 0] = 3
-p.boundary[-1, :] = 4
-
-b.boundary.fill(1)
-b.boundary[1:-1, 1:-1] = 0
-
-
-config = Config(1.0, 0.1, 0.0001, 2 / (SIZE_X - 1), 2 / (SIZE_Y - 1))
-
-
-@xgrid.kernel()
-def cavity_kernel(b: float2d, p: float2d, u: float2d, v: float2d, cfg: Config) -> None:
-    b[0, 0] = (cfg.rho * (1.0 / cfg.dt *
-                          ((u[0, 1] - u[0, -1]) /
-                           (2.0 * cfg.dx) + (v[1, 0] - v[-1, 0]) / (2.0 * cfg.dy)) -
-                          ((u[0, 1] - u[0, -1]) / (2.0 * cfg.dx))**2.0 -
-                          2.0 * ((u[1, 0] - u[-1, 0]) / (2.0 * cfg.dy) *
-                                 (v[0, 1] - v[0, -1]) / (2.0 * cfg.dx)) -
-                          ((v[1, 0] - v[-1, 0]) / (2.0 * cfg.dy))**2.0))
-
-    p[0, 0] = (((p[0, 1] + p[0, -1]) * cfg.dy**2.0 +
-                (p[1, 0] + p[-1, 0]) * cfg.dx**2.0) /
-               (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) -
-               cfg.dx**2.0 * cfg.dy**2.0 / (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) *
-               b[0, 0][0])
-
-    with xgrid.boundary(1):
-        p[0, 0] = p[0, -1][0]  # dp/dx = 0 at x = 2
-    with xgrid.boundary(2):
-        p[0, 0] = p[1, 0][0]   # dp/dy = 0 at y = 0
-    with xgrid.boundary(3):
-        p[0, 0] = p[0, 1][0]   # dp/dx = 0 at x = 0
-    with xgrid.boundary(4):
-        p[0, 0] = 0.0
-
-    for _ in range(0, 50):
-        p[0, 0] = (((p[0, 1][0] + p[0, -1][0]) * cfg.dy**2.0 +
-                    (p[1, 0][0] + p[-1, 0][0]) * cfg.dx**2.0) /
-                   (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) -
-                   cfg.dx**2.0 * cfg.dy**2.0 / (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) *
-                   b[0, 0][0])
-
-        with xgrid.boundary(1):
-            p[0, 0] = p[0, -1][0]  # dp/dx = 0 at x = 2
-        with xgrid.boundary(2):
-            p[0, 0] = p[1, 0][0]   # dp/dy = 0 at y = 0
-        with xgrid.boundary(3):
-            p[0, 0] = p[0, 1][0]   # dp/dx = 0 at x = 0
-        with xgrid.boundary(4):
-            p[0, 0] = 0.0
-
-    u[0, 0] = (u[0, 0] -
-               u[0, 0] * cfg.dt / cfg.dx *
-               (u[0, 0] - u[0, -1]) -
-               v[0, 0] * cfg.dt / cfg.dy *
-               (u[0, 0] - u[-1, 0]) -
-               cfg.dt / (2.0 * cfg.rho * cfg.dx) * (p[0, 1][0] - p[0, -1][0]) +
-               cfg.nu * (cfg.dt / cfg.dx**2.0 *
-                         (u[0, 1] - 2.0 * u[0, 0] + u[0, -1]) +
-                         cfg.dt / cfg.dy**2.0 *
-                         (u[1, 0] - 2.0 * u[0, 0] + u[-1, 0])))
-
-    v[0, 0] = (v[0, 0] -
-               u[0, 0] * cfg.dt / cfg.dx *
-               (v[0, 0] - v[0, -1]) -
-               v[0, 0] * cfg.dt / cfg.dy *
-               (v[0, 0] - v[-1, 0]) -
-               cfg.dt / (2.0 * cfg.rho * cfg.dy) * (p[1, 0][0] - p[-1, 0][0]) +
-               cfg.nu * (cfg.dt / cfg.dx**2.0 *
-                         (v[0, 1] - 2.0 * v[0, 0] + v[0, -1]) +
-                         cfg.dt / cfg.dy**2.0 *
-                         (v[1, 0] - 2.0 * v[0, 0] + v[-1, 0])))
-
-    with xgrid.boundary(1):
-        u[0, 0] = 0.0
-        v[0, 0] = 0.0
-
-    with xgrid.boundary(2):
-        u[0, 0] = 1.0
-
-
-TIME = 1
-FRAMES = int(TIME / config.dt)
-
-with timer.timing():
-    for i in tqdm.tqdm(range(FRAMES)):
-        cavity_kernel(b, p, u, v, config)
-print(f"kernel executed in {timer.elapsed:6f} seconds")
-
-# reference
-
-nit = 50
-
-
-def build_up_b(b, rho, dt, u, v, dx, dy):
-    b[1:-1, 1:-1] = (rho * (1 / dt *
-                            ((u[1:-1, 2:] - u[1:-1, 0:-2]) /
-                             (2 * dx) + (v[2:, 1:-1] - v[0:-2, 1:-1]) / (2 * dy)) -
-                            ((u[1:-1, 2:] - u[1:-1, 0:-2]) / (2 * dx))**2 -
-                            2 * ((u[2:, 1:-1] - u[0:-2, 1:-1]) / (2 * dy) *
-                                 (v[1:-1, 2:] - v[1:-1, 0:-2]) / (2 * dx)) -
-                            ((v[2:, 1:-1] - v[0:-2, 1:-1]) / (2 * dy))**2))
-
-    return b
-
-
-def pressure_poisson(p, dx, dy, b):
-    pn = numpy.empty_like(p)
-    pn = p.copy()
-    for q in range(nit):
-        pn = p.copy()
-        p[1:-1, 1:-1] = (((pn[1:-1, 2:] + pn[1:-1, 0:-2]) * dy**2 +
-                          (pn[2:, 1:-1] + pn[0:-2, 1:-1]) * dx**2) /
-                         (2 * (dx**2 + dy**2)) -
-                         dx**2 * dy**2 / (2 * (dx**2 + dy**2)) *
-                         b[1:-1, 1:-1])
-        p[:, -1] = p[:, -2]  # dp/dx = 0 at x = 2
-        p[0, :] = p[1, :]   # dp/dy = 0 at y = 0
-        p[:, 0] = p[:, 1]   # dp/dx = 0 at x = 0
-        p[-1, :] = 0        # p = 0 at y = 2
-    return p
-
-
-def cavity_flow(nt, u, v, dt, dx, dy, p, rho, nu):
-    un = numpy.empty_like(u)
-    vn = numpy.empty_like(v)
-    b = numpy.zeros((SIZE_Y, SIZE_X))
-
-    for n in tqdm.tqdm(range(nt)):
-        un = u.copy()
-        vn = v.copy()
-
-        b = build_up_b(b, rho, dt, u, v, dx, dy)
-        p = pressure_poisson(p, dx, dy, b)
-
-        u[1:-1, 1:-1] = (un[1:-1, 1:-1] -
-                         un[1:-1, 1:-1] * dt / dx *
-                         (un[1:-1, 1:-1] - un[1:-1, 0:-2]) -
-                         vn[1:-1, 1:-1] * dt / dy *
-                         (un[1:-1, 1:-1] - un[0:-2, 1:-1]) -
-                         dt / (2 * rho * dx) * (p[1:-1, 2:] - p[1:-1, 0:-2]) +
-                         nu * (dt / dx**2 *
-                               (un[1:-1, 2:] - 2 * un[1:-1, 1:-1] + un[1:-1, 0:-2]) +
-                               dt / dy**2 *
-                               (un[2:, 1:-1] - 2 * un[1:-1, 1:-1] + un[0:-2, 1:-1])))
-
-        v[1:-1, 1:-1] = (vn[1:-1, 1:-1] -
-                         un[1:-1, 1:-1] * dt / dx *
-                         (vn[1:-1, 1:-1] - vn[1:-1, 0:-2]) -
-                         vn[1:-1, 1:-1] * dt / dy *
-                         (vn[1:-1, 1:-1] - vn[0:-2, 1:-1]) -
-                         dt / (2 * rho * dy) * (p[2:, 1:-1] - p[0:-2, 1:-1]) +
-                         nu * (dt / dx**2 *
-                               (vn[1:-1, 2:] - 2 * vn[1:-1, 1:-1] + vn[1:-1, 0:-2]) +
-                               dt / dy**2 *
-                               (vn[2:, 1:-1] - 2 * vn[1:-1, 1:-1] + vn[0:-2, 1:-1])))
-
-        u[0, :] = 0
-        u[:, 0] = 0
-        u[:, -1] = 0
-        u[-1, :] = 1    # set velocity on cavity lid equal to 1
-        v[0, :] = 0
-        v[-1, :] = 0
-        v[:, 0] = 0
-        v[:, -1] = 0
-
-    return u, v, p
-
-
-uref = numpy.zeros((SIZE_Y, SIZE_X))
-vref = numpy.zeros((SIZE_Y, SIZE_X))
-pref = numpy.zeros((SIZE_Y, SIZE_X))
-bref = numpy.zeros((SIZE_Y, SIZE_X))
-with timer.timing():
-    uref, vref, pref = cavity_flow(
-        FRAMES, uref, vref, config.dt, config.dx, config.dy, pref, config.rho, config.nu)
-print(f"reference executed in {timer.elapsed:6f} seconds")
-
-
-def plot(p, u, v, name: str):
-    from matplotlib import pyplot
-
-    x = numpy.linspace(0, 2, SIZE_X)
-    y = numpy.linspace(0, 2, SIZE_Y)
-    X, Y = numpy.meshgrid(x, y)
-    fig = pyplot.figure(figsize=(11, 7), dpi=100)
-    pyplot.contourf(X, Y, p, alpha=0.5)
-    pyplot.colorbar()
-    pyplot.contour(X, Y, p)
-    pyplot.streamplot(X, Y, u, v)
-    pyplot.xlabel('X')
-    pyplot.ylabel('Y')
-    pyplot.savefig(name)
-
-
-plot(p.now, u.now, v.now, "imgs/cavity.png")
-plot(pref, uref, vref, "imgs/cavityref.png")
+from dataclasses import dataclass
+
+import tqdm
+import xgrid
+import numpy
+import time
+
+
+class Timer:
+    class TimerGuard:
+        def __init__(self, timer: "Timer") -> None:
+            self.timer = timer
+
+        def __enter__(self):
+            self.timer.start_time = time.time()
+
+        def __exit__(self, a, b, c):
+            self.timer.end_time = time.time()
+
+    def __init__(self) -> None:
+        self.start_time = time.time()
+        self.end_time = time.time()
+
+    @property
+    def elapsed(self):
+        return self.end_time - self.start_time
+
+    def timing(self):
+        return Timer.TimerGuard(self)
+
+
+timer = Timer()
+
+xgrid.init(cacheroot=".xgridtest", parallel=True, precision="double", opt_level=3)
+
+float2d = xgrid.grid[float, 2]  # type: ignore
+
+
+@dataclass
+class Config:
+    rho: float
+    nu: float
+    dt: float
+    dx: float
+    dy: float
+
+
+SIZE_X = SIZE_Y = 101
+
+u = xgrid.Grid((SIZE_X, SIZE_Y), float)
+v = xgrid.Grid((SIZE_X, SIZE_Y), float)
+p = xgrid.Grid((SIZE_X, SIZE_Y), float)
+b = xgrid.Grid((SIZE_X, SIZE_Y), float)
+
+
+u.boundary[0, :] = u.boundary[:, 0] = u.boundary[:, -1] = 1
+u.boundary[-1, :] = 2
+
+v.boundary.fill(1)
+v.boundary[1:-1, 1:-1] = 0
+
+p.boundary[:, -1] = 1
+p.boundary[0, :] = 2
+p.boundary[:, 0] = 3
+p.boundary[-1, :] = 4
+
+b.boundary.fill(1)
+b.boundary[1:-1, 1:-1] = 0
+
+
+config = Config(1.0, 0.1, 0.0001, 2 / (SIZE_X - 1), 2 / (SIZE_Y - 1))
+
+
+@xgrid.kernel()
+def cavity_kernel(b: float2d, p: float2d, u: float2d, v: float2d, cfg: Config) -> None:
+    b[0, 0] = (cfg.rho * (1.0 / cfg.dt *
+                          ((u[0, 1] - u[0, -1]) /
+                           (2.0 * cfg.dx) + (v[1, 0] - v[-1, 0]) / (2.0 * cfg.dy)) -
+                          ((u[0, 1] - u[0, -1]) / (2.0 * cfg.dx))**2.0 -
+                          2.0 * ((u[1, 0] - u[-1, 0]) / (2.0 * cfg.dy) *
+                                 (v[0, 1] - v[0, -1]) / (2.0 * cfg.dx)) -
+                          ((v[1, 0] - v[-1, 0]) / (2.0 * cfg.dy))**2.0))
+
+    p[0, 0] = (((p[0, 1] + p[0, -1]) * cfg.dy**2.0 +
+                (p[1, 0] + p[-1, 0]) * cfg.dx**2.0) /
+               (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) -
+               cfg.dx**2.0 * cfg.dy**2.0 / (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) *
+               b[0, 0][0])
+
+    with xgrid.boundary(1):
+        p[0, 0] = p[0, -1][0]  # dp/dx = 0 at x = 2
+    with xgrid.boundary(2):
+        p[0, 0] = p[1, 0][0]   # dp/dy = 0 at y = 0
+    with xgrid.boundary(3):
+        p[0, 0] = p[0, 1][0]   # dp/dx = 0 at x = 0
+    with xgrid.boundary(4):
+        p[0, 0] = 0.0
+
+    for _ in range(0, 50):
+        p[0, 0] = (((p[0, 1][0] + p[0, -1][0]) * cfg.dy**2.0 +
+                    (p[1, 0][0] + p[-1, 0][0]) * cfg.dx**2.0) /
+                   (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) -
+                   cfg.dx**2.0 * cfg.dy**2.0 / (2.0 * (cfg.dx**2.0 + cfg.dy**2.0)) *
+                   b[0, 0][0])
+
+        with xgrid.boundary(1):
+            p[0, 0] = p[0, -1][0]  # dp/dx = 0 at x = 2
+        with xgrid.boundary(2):
+            p[0, 0] = p[1, 0][0]   # dp/dy = 0 at y = 0
+        with xgrid.boundary(3):
+            p[0, 0] = p[0, 1][0]   # dp/dx = 0 at x = 0
+        with xgrid.boundary(4):
+            p[0, 0] = 0.0
+
+    u[0, 0] = (u[0, 0] -
+               u[0, 0] * cfg.dt / cfg.dx *
+               (u[0, 0] - u[0, -1]) -
+               v[0, 0] * cfg.dt / cfg.dy *
+               (u[0, 0] - u[-1, 0]) -
+               cfg.dt / (2.0 * cfg.rho * cfg.dx) * (p[0, 1][0] - p[0, -1][0]) +
+               cfg.nu * (cfg.dt / cfg.dx**2.0 *
+                         (u[0, 1] - 2.0 * u[0, 0] + u[0, -1]) +
+                         cfg.dt / cfg.dy**2.0 *
+                         (u[1, 0] - 2.0 * u[0, 0] + u[-1, 0])))
+
+    v[0, 0] = (v[0, 0] -
+               u[0, 0] * cfg.dt / cfg.dx *
+               (v[0, 0] - v[0, -1]) -
+               v[0, 0] * cfg.dt / cfg.dy *
+               (v[0, 0] - v[-1, 0]) -
+               cfg.dt / (2.0 * cfg.rho * cfg.dy) * (p[1, 0][0] - p[-1, 0][0]) +
+               cfg.nu * (cfg.dt / cfg.dx**2.0 *
+                         (v[0, 1] - 2.0 * v[0, 0] + v[0, -1]) +
+                         cfg.dt / cfg.dy**2.0 *
+                         (v[1, 0] - 2.0 * v[0, 0] + v[-1, 0])))
+
+    with xgrid.boundary(1):
+        u[0, 0] = 0.0
+        v[0, 0] = 0.0
+
+    with xgrid.boundary(2):
+        u[0, 0] = 1.0
+
+
+TIME = 1
+FRAMES = int(TIME / config.dt)
+
+with timer.timing():
+    for i in tqdm.tqdm(range(FRAMES)):
+        cavity_kernel(b, p, u, v, config)
+print(f"kernel executed in {timer.elapsed:6f} seconds")
+
+# reference
+
+nit = 50
+
+
+def build_up_b(b, rho, dt, u, v, dx, dy):
+    b[1:-1, 1:-1] = (rho * (1 / dt *
+                            ((u[1:-1, 2:] - u[1:-1, 0:-2]) /
+                             (2 * dx) + (v[2:, 1:-1] - v[0:-2, 1:-1]) / (2 * dy)) -
+                            ((u[1:-1, 2:] - u[1:-1, 0:-2]) / (2 * dx))**2 -
+                            2 * ((u[2:, 1:-1] - u[0:-2, 1:-1]) / (2 * dy) *
+                                 (v[1:-1, 2:] - v[1:-1, 0:-2]) / (2 * dx)) -
+                            ((v[2:, 1:-1] - v[0:-2, 1:-1]) / (2 * dy))**2))
+
+    return b
+
+
+def pressure_poisson(p, dx, dy, b):
+    pn = numpy.empty_like(p)
+    pn = p.copy()
+    for q in range(nit):
+        pn = p.copy()
+        p[1:-1, 1:-1] = (((pn[1:-1, 2:] + pn[1:-1, 0:-2]) * dy**2 +
+                          (pn[2:, 1:-1] + pn[0:-2, 1:-1]) * dx**2) /
+                         (2 * (dx**2 + dy**2)) -
+                         dx**2 * dy**2 / (2 * (dx**2 + dy**2)) *
+                         b[1:-1, 1:-1])
+        p[:, -1] = p[:, -2]  # dp/dx = 0 at x = 2
+        p[0, :] = p[1, :]   # dp/dy = 0 at y = 0
+        p[:, 0] = p[:, 1]   # dp/dx = 0 at x = 0
+        p[-1, :] = 0        # p = 0 at y = 2
+    return p
+
+
+def cavity_flow(nt, u, v, dt, dx, dy, p, rho, nu):
+    un = numpy.empty_like(u)
+    vn = numpy.empty_like(v)
+    b = numpy.zeros((SIZE_Y, SIZE_X))
+
+    for n in tqdm.tqdm(range(nt)):
+        un = u.copy()
+        vn = v.copy()
+
+        b = build_up_b(b, rho, dt, u, v, dx, dy)
+        p = pressure_poisson(p, dx, dy, b)
+
+        u[1:-1, 1:-1] = (un[1:-1, 1:-1] -
+                         un[1:-1, 1:-1] * dt / dx *
+                         (un[1:-1, 1:-1] - un[1:-1, 0:-2]) -
+                         vn[1:-1, 1:-1] * dt / dy *
+                         (un[1:-1, 1:-1] - un[0:-2, 1:-1]) -
+                         dt / (2 * rho * dx) * (p[1:-1, 2:] - p[1:-1, 0:-2]) +
+                         nu * (dt / dx**2 *
+                               (un[1:-1, 2:] - 2 * un[1:-1, 1:-1] + un[1:-1, 0:-2]) +
+                               dt / dy**2 *
+                               (un[2:, 1:-1] - 2 * un[1:-1, 1:-1] + un[0:-2, 1:-1])))
+
+        v[1:-1, 1:-1] = (vn[1:-1, 1:-1] -
+                         un[1:-1, 1:-1] * dt / dx *
+                         (vn[1:-1, 1:-1] - vn[1:-1, 0:-2]) -
+                         vn[1:-1, 1:-1] * dt / dy *
+                         (vn[1:-1, 1:-1] - vn[0:-2, 1:-1]) -
+                         dt / (2 * rho * dy) * (p[2:, 1:-1] - p[0:-2, 1:-1]) +
+                         nu * (dt / dx**2 *
+                               (vn[1:-1, 2:] - 2 * vn[1:-1, 1:-1] + vn[1:-1, 0:-2]) +
+                               dt / dy**2 *
+                               (vn[2:, 1:-1] - 2 * vn[1:-1, 1:-1] + vn[0:-2, 1:-1])))
+
+        u[0, :] = 0
+        u[:, 0] = 0
+        u[:, -1] = 0
+        u[-1, :] = 1    # set velocity on cavity lid equal to 1
+        v[0, :] = 0
+        v[-1, :] = 0
+        v[:, 0] = 0
+        v[:, -1] = 0
+
+    return u, v, p
+
+
+uref = numpy.zeros((SIZE_Y, SIZE_X))
+vref = numpy.zeros((SIZE_Y, SIZE_X))
+pref = numpy.zeros((SIZE_Y, SIZE_X))
+bref = numpy.zeros((SIZE_Y, SIZE_X))
+with timer.timing():
+    uref, vref, pref = cavity_flow(
+        FRAMES, uref, vref, config.dt, config.dx, config.dy, pref, config.rho, config.nu)
+print(f"reference executed in {timer.elapsed:6f} seconds")
+
+
+def plot(p, u, v, name: str):
+    from matplotlib import pyplot
+
+    x = numpy.linspace(0, 2, SIZE_X)
+    y = numpy.linspace(0, 2, SIZE_Y)
+    X, Y = numpy.meshgrid(x, y)
+    fig = pyplot.figure(figsize=(11, 7), dpi=100)
+    pyplot.contourf(X, Y, p, alpha=0.5)
+    pyplot.colorbar()
+    pyplot.contour(X, Y, p)
+    pyplot.streamplot(X, Y, u, v)
+    pyplot.xlabel('X')
+    pyplot.ylabel('Y')
+    pyplot.savefig(name)
+
+
+plot(p.now, u.now, v.now, "imgs/cavity.png")
+plot(pref, uref, vref, "imgs/cavityref.png")
```

### Comparing `xgrid-0.0.1/imgs/cavity.gif` & `xgrid-0.0.2/imgs/cavity.gif`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/imgs/cavity.png` & `xgrid-0.0.2/imgs/cavity.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/imgs/cavityref.png` & `xgrid-0.0.2/imgs/cavityref.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/imgs/convection_1d.png` & `xgrid-0.0.2/imgs/convection_1d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/imgs/convection_1d_nonlinear.png` & `xgrid-0.0.2/imgs/convection_1d_nonlinear.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/imgs/convection_2d.png` & `xgrid-0.0.2/imgs/convection_2d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/imgs/diffusion_1d.png` & `xgrid-0.0.2/imgs/diffusion_1d.png`

 * *Files identical despite different names*

### Comparing `xgrid-0.0.1/xgrid/__init__.py` & `xgrid-0.0.2/xgrid/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import struct
-from typing import Any
-from xgrid.lang import boundary, c
-from xgrid.lang.operator import kernel, function, external
-from xgrid.util.init import init
-from xgrid.util.typing import BaseType, Void
-from xgrid.util.typing.annotation import ptr, grid
-from xgrid.util.typing.value import Integer
-from xgrid.util.typing.reference import Grid as _Grid
-from xgrid.xgrid import Grid
-
-
-def _dimension_typecheck(args: list[BaseType]) -> BaseType:
-    if not isinstance(args[0], _Grid):
-        raise Exception(f"Incompatible dimension to type '{args[0]}'")
-
-    return Integer(struct.calcsize("i"))
-
-
-def _shape_typecheck(args: list[BaseType]) -> BaseType:
-    if not isinstance(args[0], _Grid):
-        raise Exception(f"Incompatible shape to type '{args[0]}'")
-
-    if not isinstance(args[1], Integer):
-        raise Exception(f"Incompatible shape dimension '{args[1]}'")
-
-    return Integer(struct.calcsize("i"))
-
-
-def _tick_typecheck(args: list[BaseType]) -> BaseType:
-    if not isinstance(args[0], _Grid):
-        raise Exception(f"Incompatible tick to type '{args[0]}'")
-
-    return Void()
-
-
-@external(typecheck_override=_dimension_typecheck)
-def dimension(grid: Any) -> int:
-    ...
-
-
-@external(typecheck_override=_shape_typecheck)
-def shape(grid: Any, dimension: int) -> int:
-    ...
-
-
-@external(typecheck_override=_tick_typecheck)
-def tick(grid: Any) -> None:
-    ...
-
-
-__all__ = ["kernel", "function", "init",
-           "ptr", "grid", "boundary", "c", "external", "Grid", "shape", "dimension", "tick"]
+import struct
+from typing import Any
+from xgrid.lang import boundary, c
+from xgrid.lang.operator import kernel, function, external
+from xgrid.util.init import init
+from xgrid.util.typing import BaseType, Void
+from xgrid.util.typing.annotation import ptr, grid
+from xgrid.util.typing.value import Integer
+from xgrid.util.typing.reference import Grid as _Grid
+from xgrid.xgrid import Grid
+
+
+def _dimension_typecheck(args: list[BaseType]) -> BaseType:
+    if not isinstance(args[0], _Grid):
+        raise Exception(f"Incompatible dimension to type '{args[0]}'")
+
+    return Integer(struct.calcsize("i"))
+
+
+def _shape_typecheck(args: list[BaseType]) -> BaseType:
+    if not isinstance(args[0], _Grid):
+        raise Exception(f"Incompatible shape to type '{args[0]}'")
+
+    if not isinstance(args[1], Integer):
+        raise Exception(f"Incompatible shape dimension '{args[1]}'")
+
+    return Integer(struct.calcsize("i"))
+
+
+def _tick_typecheck(args: list[BaseType]) -> BaseType:
+    if not isinstance(args[0], _Grid):
+        raise Exception(f"Incompatible tick to type '{args[0]}'")
+
+    return Void()
+
+
+@external(typecheck_override=_dimension_typecheck)
+def dimension(grid: Any) -> int:
+    ...
+
+
+@external(typecheck_override=_shape_typecheck)
+def shape(grid: Any, dimension: int) -> int:
+    ...
+
+
+@external(typecheck_override=_tick_typecheck)
+def tick(grid: Any) -> None:
+    ...
+
+
+__all__ = ["kernel", "function", "init",
+           "ptr", "grid", "boundary", "c", "external", "Grid", "shape", "dimension", "tick"]
```

### Comparing `xgrid-0.0.1/xgrid/lang/generator.py` & `xgrid-0.0.2/xgrid/lang/generator.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,431 +1,431 @@
-from dataclasses import dataclass
-from io import StringIO
-from typing import Optional, cast
-import xgrid.lang.ir as ir
-import xgrid.lang.ir.statement as stat
-import xgrid.lang.ir.expression as expr
-from xgrid.lang.ir.visitor import IRVisitor
-from xgrid.lang.operator import Operator
-from xgrid.util.console import LineFormat
-from xgrid.util.ffi import Compiler, Library
-from xgrid.util.logging import Logger
-from xgrid.util.init import get_config
-from xgrid.util.typing import BaseType, Void
-from xgrid.util.typing.reference import Grid, Pointer
-from xgrid.util.typing.value import Boolean, Floating, Integer, Structure, Value
-
-
-def repeat_str(element: str, time: int, sep: str):
-    return sep.join(element for _ in range(time))
-
-
-@dataclass
-class StencilFlag:
-    variable: ir.Variable
-    boundary: int
-    implicit: bool = False
-
-    def __post_init__(self):
-        assert isinstance(self.variable.type, Grid)
-        self._type = self.variable.type
-
-    @property
-    def name(self) -> str:
-        return self.variable.name
-
-    @property
-    def element(self) -> Value:
-        return self._type.element
-
-    @property
-    def dimension(self) -> int:
-        return self._type.dimension
-
-    @property
-    def type(self) -> Grid:
-        return self._type
-
-
-class StencilParser(IRVisitor):
-    def __init__(self, logger: Logger) -> None:
-        super().__init__()
-        self.logger = logger
-
-        self.stencil_flag = None
-
-    def visit_Stencil(self, ir: expr.Stencil):
-        if ir.context == "store":
-            assert self.stencil_flag is None
-
-            self.stencil_flag = StencilFlag(ir.variable, ir.boundary_mask)
-        elif ir.context == "load":
-            if self.stencil_flag is None:
-                self.logger.dead(
-                    f"Unable to perform load operation to grid '{ir.variable.name}' without stencil context")
-
-            if ir.time_offset == 0 and self.stencil_flag.variable == ir.variable:
-                self.stencil_flag.implicit = True
-
-    def visit_Assignment(self, ir: stat.Assignment):
-        self.visit(ir.terminal)
-        self.visit(ir.value)
-
-        setattr(ir, "__stencil_flag", self.stencil_flag)
-
-        self.stencil_flag = None
-
-
-class Generator:
-    def __init__(self, operator: Operator) -> None:
-        self.logger = Logger(self)
-
-        self.operator = operator
-        assert self.operator.mode == "kernel"
-
-        self.config = get_config()
-
-        self.definitions = LineFormat()
-        self.logger.info("Insert necessary and predefined headers")
-        headers = ["stdio.h", "stdlib.h", "stdint.h", "stdbool.h", "math.h"]
-        if self.config.parallel:
-            headers.append("omp.h")
-
-        for header in headers:
-            self.definitions.println(f"#include <{header}>")
-
-        for header in operator.includes:
-            self.definitions.println(f"#include \"{header}\"")
-
-        self.op_impls: dict[str, LineFormat] = {}
-        self.t_impls: dict[str, LineFormat] = {}
-        self.depth = 0
-
-        self.define_operator(operator)
-
-    @property
-    def result(self):
-        return self.compile(), self.depth + 1
-
-    @property
-    def source(self):
-        with StringIO() as io:
-            self.definitions.write(io)
-            for impls in self.t_impls.values():
-                impls.write(io)
-
-            for impls in self.op_impls.values():
-                impls.write(io)
-            return io.getvalue()
-
-    def format_type(self, t: BaseType, abbr: bool = False):
-        if isinstance(t, Void):
-            return "void"
-
-        if isinstance(t, Boolean):
-            return "b" if abbr else "bool"
-        elif isinstance(t, Integer):
-            return f"i{t.width_bits}" if abbr else f"int{t.width_bits}_t"
-        elif isinstance(t, Floating):
-            fullname = {32: "float", 64: "double"}[t.width_bits]
-            return fullname[0] if abbr else fullname
-        elif isinstance(t, Structure):
-            self.define_type(t, t.name)
-            return f"st{t.name}" if abbr else f"struct {t.name}"
-
-        # reference type does not have abbr
-        elif isinstance(t, Pointer):
-            return f"{self.format_type(t.element)}*"
-        elif isinstance(t, Grid):
-            name = f"__Grid{t.dimension}d_{self.format_type(t.element, True)}"
-            self.define_type(t, name)
-            return name if abbr else f"struct {name}"
-
-    def define_type(self, t: BaseType, name: str):
-        if name in self.t_impls:
-            return
-
-        self.definitions.println(f"struct {name};")
-        implementation = LineFormat()
-        self.t_impls[name] = implementation
-        implementation.println(f"struct {name} {{")
-
-        if isinstance(t, Structure):
-            with implementation.indent():
-                for name, type in t.elements:
-                    implementation.println(f"{self.format_type(type)} {name};")
-            implementation.println("};")
-        elif isinstance(t, Grid):
-            with implementation.indent():
-                implementation.println("int32_t time;")
-                implementation.println(f"int32_t shape[{t.dimension}];")
-                implementation.println(
-                    f"{self.format_type(t.element)}** data;")
-                implementation.println("int32_t* boundary_mask;")
-            implementation.println("};")
-
-            implementation.println(
-                f"static inline {self.format_type(t.element)}* {name}_at(struct {name} grid, {', '.join(f'int32_t space_offset_{i}' for i in range(t.dimension))}, int32_t time_offset) {{")
-            with implementation.indent():
-                implementation.println("int32_t space_offset = 0;")
-                for i in range(t.dimension):
-                    if self.config.overstep == "wrap":
-                        space_offset_i = f"((space_offset_{t.dimension - 1 - i} + grid.shape[{i}]) % grid.shape[{i}])"
-                    elif self.config.overstep == "limit":
-                        space_offset_i = f"(space_offset_{t.dimension - 1 - i} < 0 ? 0 : space_offset_{t.dimension - 1 - i} >= grid.shape[{i}] ? grid.shape[{i}] - 1 : space_offset_{t.dimension - 1 - i})"
-                    else:
-                        space_offset_i = f"space_offset_{t.dimension - 1 - i}"
-                    implementation.println(
-                        f"space_offset += {space_offset_i} * {'1' if i == 0 else f'grid.shape[{i - 1}]'};")
-                implementation.println(
-                    f"return &grid.data[time_offset][space_offset];")
-            implementation.println("}")
-
-    def define_operator(self, operator: Operator):
-        if operator.name in self.op_impls:
-            return
-
-        opir = operator.ir
-
-        previsitors = [StencilParser(self.logger)]
-        for visitor in previsitors:
-            visitor.visit(opir)
-
-        implementation = LineFormat()
-        self.op_impls[operator.name] = implementation
-
-        arguments = ', '.join(
-            map(lambda x: f"{self.format_type(x[1])} {x[0]}", opir.signature.arguments))
-        definition = f"{self.format_type(opir.signature.return_type)} {operator.name}({arguments})"
-        self.definitions.println(
-            ("extern " if operator.mode == "external" else "") + definition + ";")
-
-        if operator.mode == "external":
-            return
-
-        implementation.println(definition + "{")
-
-        with implementation.indent():
-            # variable definitions
-            for name, var in operator.ir.scope.items():
-                if name not in operator.signature.argnames_map:
-                    implementation.println(
-                        f"{self.format_type(var.type)} {name};")
-
-            self.visits(operator.ir.body, implementation)
-        implementation.println("}")
-
-    def compile(self):
-        self.logger.info(
-            f"Compiling kernel {self.operator.name}' and retrive interface")
-        dynlib = Compiler(cacheroot=self.config.cacheroot, cc=self.config.cc).compile(
-            self.source, self.config.cflags)
-
-        argtypes = [x[1] for x in self.operator.ir.signature.arguments]
-        rettype = self.operator.ir.signature.return_type
-
-        return Library(dynlib).function(self.operator.name, argtypes, rettype)
-
-    def visit(self, node: ir.IR, implementation: LineFormat):
-        node_class = node.__class__.__name__
-        method = getattr(self, "visit_" + node_class)
-        if self.config.comment and isinstance(node, stat.Statement):
-            implementation.println(
-                f"#line {node.location.line} \"{node.location.file}\"", indent=False)
-        return method(node, implementation)
-
-    def visits(self, l: list[stat.Statement], implementation: LineFormat):
-        for item in l:
-            self.visit(item, implementation)
-
-    def visit_Return(self, ir: stat.Return, implementation: LineFormat):
-        if ir.value is None:
-            implementation.println(f"return;")
-        else:
-            implementation.println(
-                f"return {self.visit(ir.value, implementation)};")
-
-    def visit_Break(self, ir: stat.Break, implementation: LineFormat):
-        implementation.println("break;")
-
-    def visit_Continue(self, ir: stat.Continue, implementation: LineFormat):
-        implementation.println("continue;")
-
-    def visit_If(self, ir: stat.If, implementation: LineFormat):
-        implementation.println(
-            f"if ({self.visit(ir.condition, implementation)}) {{")
-        with implementation.indent():
-            self.visits(ir.body, implementation)
-        if any(ir.orelse):
-            implementation.println("} else {")
-            with implementation.indent():
-                self.visits(ir.orelse, implementation)
-        implementation.println("}")
-
-    def visit_While(self, ir: stat.While, implementation: LineFormat):
-        implementation.println(
-            f"while ({self.visit(ir.condition, implementation)}) {{")
-        with implementation.indent():
-            self.visits(ir.body, implementation)
-        implementation.println("}")
-
-    def visit_Evaluation(self, ir: stat.Evaluation, implementation: LineFormat):
-        implementation.println(f"{self.visit(ir.value, implementation)};")
-
-    def visit_Assignment(self, ir: stat.Assignment, implementation: LineFormat):
-        stencil_flag = getattr(ir, "__stencil_flag", None)
-
-        if stencil_flag is not None:
-            def gen_head(s: StencilFlag):
-                for i in range(s.dimension):
-                    implementation.println(
-                        f"for (int32_t $dim{i} = 0; $dim{i} < {s.name}.shape[{i}]; $dim{i}++) {{")
-                    implementation.force_indent()
-
-                id = " + ".join(
-                    f"$dim{s.dimension - i - 1} * {'1' if i == 0 else f'{s.name}.shape[{i - 1}]'}" for i in range(s.dimension))
-                implementation.println(
-                    f"if ({s.name}.boundary_mask[{id}] == {s.boundary}) {{")
-                implementation.force_indent()
-
-            def gen_tail(s: StencilFlag):
-                for i in range(s.dimension + 1):
-                    implementation.force_dedent()
-                    implementation.println("}")
-
-            stencil_flag = cast(StencilFlag, stencil_flag)
-
-            if stencil_flag.implicit and not self.config.parallel:
-                self.logger.dead(
-                    f"Unable to perform implicit operation while parallel is off")
-
-            if stencil_flag.implicit and stencil_flag.boundary == 0:
-                # TODO: handle implicit case
-                implementation.println("{")
-                with implementation.indent():
-                    # create a thread local intermediate value to store
-                    value_type = self.format_type(ir.value.type)
-                    value_size = " * ".join(
-                        f"{stencil_flag.name}.shape[{i}]" for i in range(stencil_flag.dimension))
-                    implementation.println(
-                        f"{value_type}* $value = malloc(sizeof({value_type}) * ({value_size}));")
-
-                    implementation.println(
-                        "#pragma omp parallel", indent=False)
-                    implementation.println("{")
-                    with implementation.indent():
-
-                        value_id = " + ".join(
-                            f"$dim{stencil_flag.dimension - i - 1} * {'1' if i == 0 else f'{stencil_flag.name}.shape[{i - 1}]'}" for i in range(stencil_flag.dimension))
-
-                        # load value to thread local value first
-                        implementation.println(
-                            f"#pragma omp for collapse({stencil_flag.dimension})", indent=False)
-                        gen_head(stencil_flag)
-                        implementation.println(
-                            f"$value[{value_id}] = {self.visit(ir.value, implementation)};")
-                        gen_tail(stencil_flag)
-
-                        # perform barrier operation
-                        implementation.println(
-                            "#pragma omp barrier", indent=False)
-
-                        # load value to grid then
-                        implementation.println(
-                            f"#pragma omp for collapse({stencil_flag.dimension})", indent=False)
-                        gen_head(stencil_flag)
-                        implementation.println(
-                            f"{self.visit(ir.terminal, implementation)} = $value[{value_id}];")
-                        gen_tail(stencil_flag)
-                    implementation.println("}")
-                    implementation.println("free($value);")
-                implementation.println("}")
-            else:
-                if self.config.parallel:
-                    implementation.println(
-                        f"#pragma omp parallel for collapse({stencil_flag.dimension})", indent=False)
-
-                gen_head(stencil_flag)
-                implementation.println(
-                    f"{self.visit(ir.terminal, implementation)} = {self.visit(ir.value, implementation)};")
-                gen_tail(stencil_flag)
-        else:
-            implementation.println(
-                f"{self.visit(ir.terminal, implementation)} = {self.visit(ir.value, implementation)};")
-
-    def visit_Inline(self, ir: stat.Inline, implementation: LineFormat):
-        implementation.println(ir.source)
-
-    def visit_For(self, ir: stat.For, implementation: LineFormat):
-        implementation.println(
-            f"for ({ir.variable.name} = {self.visit(ir.start, implementation)}; {ir.variable.name} < {self.visit(ir.end, implementation)}; {ir.variable.name} += {self.visit(ir.step, implementation)}) {{")
-        with implementation.indent():
-            self.visits(ir.body, implementation)
-        implementation.println("}")
-
-    # ===== expression =====
-    def visit_Binary(self, ir: expr.Binary, implementation: LineFormat):
-        if ir.operator == expr.BinaryOperator.Pow:
-            if isinstance(ir.type, Floating) and ir.type.width_bits == 64:
-                pow_func = "pow"
-            else:
-                pow_func = "powf"
-            return f"{pow_func}({self.visit(ir.left, implementation)}, {self.visit(ir.right, implementation)})"
-        else:
-            return f"({self.visit(ir.left, implementation)} {ir.operator.value} {self.visit(ir.right, implementation)})"
-
-    def visit_Unary(self, ir: expr.Unary, implementation: LineFormat):
-        return f"({ir.operator.value} {self.visit(ir.right, implementation)})"
-
-    def visit_Condition(self, ir: expr.Condition, implementation: LineFormat):
-        return f"({self.visit(ir.condition, implementation)} ? {self.visit(ir.body, implementation)} : {self.visit(ir.orelse, implementation)})"
-
-    def visit_Constant(self, ir: expr.Constant, implementation: LineFormat):
-        return repr(ir.value).lower()
-
-    def visit_Identifier(self, ir: expr.Identifier, implementation: LineFormat):
-        if isinstance(ir.variable.type, Pointer):
-            return f"(*{ir.variable.name})"
-        else:
-            return ir.variable.name
-
-    def visit_Access(self, ir: expr.Access, implementation: LineFormat):
-        return f"({self.visit(ir.value, implementation)}).{ir.attribute}"
-
-    def visit_Call(self, ir: expr.Call, implementation: LineFormat):
-        args = []
-
-        for id, argument in enumerate(ir.arguments):
-            arg_code = self.visit(argument, implementation)
-            arg_type = ir.operator.signature.arguments[id][1]
-            if isinstance(arg_type, Pointer) and argument.type == arg_type.element:
-                arg_code = f"&{arg_code}"
-            args.append(arg_code)
-        args = ', '.join(args)
-        if isinstance(ir.operator, expr.Constructor):
-            return f"(({self.format_type(ir.operator.type)}) {{{args}}})"
-        else:
-            self.define_operator(ir.operator)
-            return f"{ir.operator.name}({args})"
-
-    def visit_Cast(self, ir: expr.Cast, implementation: LineFormat):
-        return f"(({self.format_type(ir.type)})({self.visit(ir.value, implementation)}))"
-
-    def visit_Stencil(self, ir: expr.Stencil, implementation: LineFormat):
-        irvar = ir.variable
-        assert isinstance(irvar.type, Grid)
-
-        self.depth = max(self.depth, abs(ir.time_offset))
-
-        indexes = ', '.join(
-            f"$dim{i} + {ir.space_offset[i]}" for i in range(irvar.type.dimension))
-        return f"(*{self.format_type(irvar.type, True)}_at({ir.variable.name}, {indexes}, {abs(ir.time_offset)}))"
-
-    def visit_GridInfo(self, ir: expr.GridInfo, implementation: LineFormat):
-        assert isinstance(ir.variable.type, Grid)
-
-        if ir.info == "dimension":
-            return str(ir.variable.type.dimension)
-        elif ir.info == "shape":
-            assert ir.dimension is not None
-
-            return f"{ir.variable.name}.shape[{self.visit(ir.dimension, implementation)}]"
+from dataclasses import dataclass
+from io import StringIO
+from typing import Optional, cast
+import xgrid.lang.ir as ir
+import xgrid.lang.ir.statement as stat
+import xgrid.lang.ir.expression as expr
+from xgrid.lang.ir.visitor import IRVisitor
+from xgrid.lang.operator import Operator
+from xgrid.util.console import LineFormat
+from xgrid.util.ffi import Compiler, Library
+from xgrid.util.logging import Logger
+from xgrid.util.init import get_config
+from xgrid.util.typing import BaseType, Void
+from xgrid.util.typing.reference import Grid, Pointer
+from xgrid.util.typing.value import Boolean, Floating, Integer, Structure, Value
+
+
+def repeat_str(element: str, time: int, sep: str):
+    return sep.join(element for _ in range(time))
+
+
+@dataclass
+class StencilFlag:
+    variable: ir.Variable
+    boundary: int
+    implicit: bool = False
+
+    def __post_init__(self):
+        assert isinstance(self.variable.type, Grid)
+        self._type = self.variable.type
+
+    @property
+    def name(self) -> str:
+        return self.variable.name
+
+    @property
+    def element(self) -> Value:
+        return self._type.element
+
+    @property
+    def dimension(self) -> int:
+        return self._type.dimension
+
+    @property
+    def type(self) -> Grid:
+        return self._type
+
+
+class StencilParser(IRVisitor):
+    def __init__(self, logger: Logger) -> None:
+        super().__init__()
+        self.logger = logger
+
+        self.stencil_flag = None
+
+    def visit_Stencil(self, ir: expr.Stencil):
+        if ir.context == "store":
+            assert self.stencil_flag is None
+
+            self.stencil_flag = StencilFlag(ir.variable, ir.boundary_mask)
+        elif ir.context == "load":
+            if self.stencil_flag is None:
+                self.logger.dead(
+                    f"Unable to perform load operation to grid '{ir.variable.name}' without stencil context")
+
+            if ir.time_offset == 0 and self.stencil_flag.variable == ir.variable:
+                self.stencil_flag.implicit = True
+
+    def visit_Assignment(self, ir: stat.Assignment):
+        self.visit(ir.terminal)
+        self.visit(ir.value)
+
+        setattr(ir, "__stencil_flag", self.stencil_flag)
+
+        self.stencil_flag = None
+
+
+class Generator:
+    def __init__(self, operator: Operator) -> None:
+        self.logger = Logger(self)
+
+        self.operator = operator
+        assert self.operator.mode == "kernel"
+
+        self.config = get_config()
+
+        self.definitions = LineFormat()
+        self.logger.info("Insert necessary and predefined headers")
+        headers = ["stdio.h", "stdlib.h", "stdint.h", "stdbool.h", "math.h"]
+        if self.config.parallel:
+            headers.append("omp.h")
+
+        for header in headers:
+            self.definitions.println(f"#include <{header}>")
+
+        for header in operator.includes:
+            self.definitions.println(f"#include \"{header}\"")
+
+        self.op_impls: dict[str, LineFormat] = {}
+        self.t_impls: dict[str, LineFormat] = {}
+        self.depth = 0
+
+        self.define_operator(operator)
+
+    @property
+    def result(self):
+        return self.compile(), self.depth + 1
+
+    @property
+    def source(self):
+        with StringIO() as io:
+            self.definitions.write(io)
+            for impls in self.t_impls.values():
+                impls.write(io)
+
+            for impls in self.op_impls.values():
+                impls.write(io)
+            return io.getvalue()
+
+    def format_type(self, t: BaseType, abbr: bool = False):
+        if isinstance(t, Void):
+            return "void"
+
+        if isinstance(t, Boolean):
+            return "b" if abbr else "bool"
+        elif isinstance(t, Integer):
+            return f"i{t.width_bits}" if abbr else f"int{t.width_bits}_t"
+        elif isinstance(t, Floating):
+            fullname = {32: "float", 64: "double"}[t.width_bits]
+            return fullname[0] if abbr else fullname
+        elif isinstance(t, Structure):
+            self.define_type(t, t.name)
+            return f"st{t.name}" if abbr else f"struct {t.name}"
+
+        # reference type does not have abbr
+        elif isinstance(t, Pointer):
+            return f"{self.format_type(t.element)}*"
+        elif isinstance(t, Grid):
+            name = f"__Grid{t.dimension}d_{self.format_type(t.element, True)}"
+            self.define_type(t, name)
+            return name if abbr else f"struct {name}"
+
+    def define_type(self, t: BaseType, name: str):
+        if name in self.t_impls:
+            return
+
+        self.definitions.println(f"struct {name};")
+        implementation = LineFormat()
+        self.t_impls[name] = implementation
+        implementation.println(f"struct {name} {{")
+
+        if isinstance(t, Structure):
+            with implementation.indent():
+                for name, type in t.elements:
+                    implementation.println(f"{self.format_type(type)} {name};")
+            implementation.println("};")
+        elif isinstance(t, Grid):
+            with implementation.indent():
+                implementation.println("int32_t time;")
+                implementation.println(f"int32_t shape[{t.dimension}];")
+                implementation.println(
+                    f"{self.format_type(t.element)}** data;")
+                implementation.println("int32_t* boundary_mask;")
+            implementation.println("};")
+
+            implementation.println(
+                f"static inline {self.format_type(t.element)}* {name}_at(struct {name} grid, {', '.join(f'int32_t space_offset_{i}' for i in range(t.dimension))}, int32_t time_offset) {{")
+            with implementation.indent():
+                implementation.println("int32_t space_offset = 0;")
+                for i in range(t.dimension):
+                    if self.config.overstep == "wrap":
+                        space_offset_i = f"((space_offset_{t.dimension - 1 - i} + grid.shape[{i}]) % grid.shape[{i}])"
+                    elif self.config.overstep == "limit":
+                        space_offset_i = f"(space_offset_{t.dimension - 1 - i} < 0 ? 0 : space_offset_{t.dimension - 1 - i} >= grid.shape[{i}] ? grid.shape[{i}] - 1 : space_offset_{t.dimension - 1 - i})"
+                    else:
+                        space_offset_i = f"space_offset_{t.dimension - 1 - i}"
+                    implementation.println(
+                        f"space_offset += {space_offset_i} * {'1' if i == 0 else f'grid.shape[{i - 1}]'};")
+                implementation.println(
+                    f"return &grid.data[time_offset][space_offset];")
+            implementation.println("}")
+
+    def define_operator(self, operator: Operator):
+        if operator.name in self.op_impls:
+            return
+
+        opir = operator.ir
+
+        previsitors = [StencilParser(self.logger)]
+        for visitor in previsitors:
+            visitor.visit(opir)
+
+        implementation = LineFormat()
+        self.op_impls[operator.name] = implementation
+
+        arguments = ', '.join(
+            map(lambda x: f"{self.format_type(x[1])} {x[0]}", opir.signature.arguments))
+        definition = f"{self.format_type(opir.signature.return_type)} {operator.name}({arguments})"
+        self.definitions.println(
+            ("extern " if operator.mode == "external" else "") + definition + ";")
+
+        if operator.mode == "external":
+            return
+
+        implementation.println(definition + "{")
+
+        with implementation.indent():
+            # variable definitions
+            for name, var in operator.ir.scope.items():
+                if name not in operator.signature.argnames_map:
+                    implementation.println(
+                        f"{self.format_type(var.type)} {name};")
+
+            self.visits(operator.ir.body, implementation)
+        implementation.println("}")
+
+    def compile(self):
+        self.logger.info(
+            f"Compiling kernel {self.operator.name}' and retrive interface")
+        dynlib = Compiler(cacheroot=self.config.cacheroot, cc=self.config.cc).compile(
+            self.source, self.config.cflags)
+
+        argtypes = [x[1] for x in self.operator.ir.signature.arguments]
+        rettype = self.operator.ir.signature.return_type
+
+        return Library(dynlib).function(self.operator.name, argtypes, rettype)
+
+    def visit(self, node: ir.IR, implementation: LineFormat):
+        node_class = node.__class__.__name__
+        method = getattr(self, "visit_" + node_class)
+        if self.config.comment and isinstance(node, stat.Statement):
+            implementation.println(
+                f"#line {node.location.line} \"{node.location.file}\"", indent=False)
+        return method(node, implementation)
+
+    def visits(self, l: list[stat.Statement], implementation: LineFormat):
+        for item in l:
+            self.visit(item, implementation)
+
+    def visit_Return(self, ir: stat.Return, implementation: LineFormat):
+        if ir.value is None:
+            implementation.println(f"return;")
+        else:
+            implementation.println(
+                f"return {self.visit(ir.value, implementation)};")
+
+    def visit_Break(self, ir: stat.Break, implementation: LineFormat):
+        implementation.println("break;")
+
+    def visit_Continue(self, ir: stat.Continue, implementation: LineFormat):
+        implementation.println("continue;")
+
+    def visit_If(self, ir: stat.If, implementation: LineFormat):
+        implementation.println(
+            f"if ({self.visit(ir.condition, implementation)}) {{")
+        with implementation.indent():
+            self.visits(ir.body, implementation)
+        if any(ir.orelse):
+            implementation.println("} else {")
+            with implementation.indent():
+                self.visits(ir.orelse, implementation)
+        implementation.println("}")
+
+    def visit_While(self, ir: stat.While, implementation: LineFormat):
+        implementation.println(
+            f"while ({self.visit(ir.condition, implementation)}) {{")
+        with implementation.indent():
+            self.visits(ir.body, implementation)
+        implementation.println("}")
+
+    def visit_Evaluation(self, ir: stat.Evaluation, implementation: LineFormat):
+        implementation.println(f"{self.visit(ir.value, implementation)};")
+
+    def visit_Assignment(self, ir: stat.Assignment, implementation: LineFormat):
+        stencil_flag = getattr(ir, "__stencil_flag", None)
+
+        if stencil_flag is not None:
+            def gen_head(s: StencilFlag):
+                for i in range(s.dimension):
+                    implementation.println(
+                        f"for (int32_t $dim{i} = 0; $dim{i} < {s.name}.shape[{i}]; $dim{i}++) {{")
+                    implementation.force_indent()
+
+                id = " + ".join(
+                    f"$dim{s.dimension - i - 1} * {'1' if i == 0 else f'{s.name}.shape[{i - 1}]'}" for i in range(s.dimension))
+                implementation.println(
+                    f"if ({s.name}.boundary_mask[{id}] == {s.boundary}) {{")
+                implementation.force_indent()
+
+            def gen_tail(s: StencilFlag):
+                for i in range(s.dimension + 1):
+                    implementation.force_dedent()
+                    implementation.println("}")
+
+            stencil_flag = cast(StencilFlag, stencil_flag)
+
+            if stencil_flag.implicit and not self.config.parallel:
+                self.logger.dead(
+                    f"Unable to perform implicit operation while parallel is off")
+
+            if stencil_flag.implicit and stencil_flag.boundary == 0:
+                # TODO: handle implicit case
+                implementation.println("{")
+                with implementation.indent():
+                    # create a thread local intermediate value to store
+                    value_type = self.format_type(ir.value.type)
+                    value_size = " * ".join(
+                        f"{stencil_flag.name}.shape[{i}]" for i in range(stencil_flag.dimension))
+                    implementation.println(
+                        f"{value_type}* $value = malloc(sizeof({value_type}) * ({value_size}));")
+
+                    implementation.println(
+                        "#pragma omp parallel", indent=False)
+                    implementation.println("{")
+                    with implementation.indent():
+
+                        value_id = " + ".join(
+                            f"$dim{stencil_flag.dimension - i - 1} * {'1' if i == 0 else f'{stencil_flag.name}.shape[{i - 1}]'}" for i in range(stencil_flag.dimension))
+
+                        # load value to thread local value first
+                        implementation.println(
+                            f"#pragma omp for collapse({stencil_flag.dimension})", indent=False)
+                        gen_head(stencil_flag)
+                        implementation.println(
+                            f"$value[{value_id}] = {self.visit(ir.value, implementation)};")
+                        gen_tail(stencil_flag)
+
+                        # perform barrier operation
+                        implementation.println(
+                            "#pragma omp barrier", indent=False)
+
+                        # load value to grid then
+                        implementation.println(
+                            f"#pragma omp for collapse({stencil_flag.dimension})", indent=False)
+                        gen_head(stencil_flag)
+                        implementation.println(
+                            f"{self.visit(ir.terminal, implementation)} = $value[{value_id}];")
+                        gen_tail(stencil_flag)
+                    implementation.println("}")
+                    implementation.println("free($value);")
+                implementation.println("}")
+            else:
+                if self.config.parallel:
+                    implementation.println(
+                        f"#pragma omp parallel for collapse({stencil_flag.dimension})", indent=False)
+
+                gen_head(stencil_flag)
+                implementation.println(
+                    f"{self.visit(ir.terminal, implementation)} = {self.visit(ir.value, implementation)};")
+                gen_tail(stencil_flag)
+        else:
+            implementation.println(
+                f"{self.visit(ir.terminal, implementation)} = {self.visit(ir.value, implementation)};")
+
+    def visit_Inline(self, ir: stat.Inline, implementation: LineFormat):
+        implementation.println(ir.source)
+
+    def visit_For(self, ir: stat.For, implementation: LineFormat):
+        implementation.println(
+            f"for ({ir.variable.name} = {self.visit(ir.start, implementation)}; {ir.variable.name} < {self.visit(ir.end, implementation)}; {ir.variable.name} += {self.visit(ir.step, implementation)}) {{")
+        with implementation.indent():
+            self.visits(ir.body, implementation)
+        implementation.println("}")
+
+    # ===== expression =====
+    def visit_Binary(self, ir: expr.Binary, implementation: LineFormat):
+        if ir.operator == expr.BinaryOperator.Pow:
+            if isinstance(ir.type, Floating) and ir.type.width_bits == 64:
+                pow_func = "pow"
+            else:
+                pow_func = "powf"
+            return f"{pow_func}({self.visit(ir.left, implementation)}, {self.visit(ir.right, implementation)})"
+        else:
+            return f"({self.visit(ir.left, implementation)} {ir.operator.value} {self.visit(ir.right, implementation)})"
+
+    def visit_Unary(self, ir: expr.Unary, implementation: LineFormat):
+        return f"({ir.operator.value} {self.visit(ir.right, implementation)})"
+
+    def visit_Condition(self, ir: expr.Condition, implementation: LineFormat):
+        return f"({self.visit(ir.condition, implementation)} ? {self.visit(ir.body, implementation)} : {self.visit(ir.orelse, implementation)})"
+
+    def visit_Constant(self, ir: expr.Constant, implementation: LineFormat):
+        return repr(ir.value).lower()
+
+    def visit_Identifier(self, ir: expr.Identifier, implementation: LineFormat):
+        if isinstance(ir.variable.type, Pointer):
+            return f"(*{ir.variable.name})"
+        else:
+            return ir.variable.name
+
+    def visit_Access(self, ir: expr.Access, implementation: LineFormat):
+        return f"({self.visit(ir.value, implementation)}).{ir.attribute}"
+
+    def visit_Call(self, ir: expr.Call, implementation: LineFormat):
+        args = []
+
+        for id, argument in enumerate(ir.arguments):
+            arg_code = self.visit(argument, implementation)
+            arg_type = ir.operator.signature.arguments[id][1]
+            if isinstance(arg_type, Pointer) and argument.type == arg_type.element:
+                arg_code = f"&{arg_code}"
+            args.append(arg_code)
+        args = ', '.join(args)
+        if isinstance(ir.operator, expr.Constructor):
+            return f"(({self.format_type(ir.operator.type)}) {{{args}}})"
+        else:
+            self.define_operator(ir.operator)
+            return f"{ir.operator.name}({args})"
+
+    def visit_Cast(self, ir: expr.Cast, implementation: LineFormat):
+        return f"(({self.format_type(ir.type)})({self.visit(ir.value, implementation)}))"
+
+    def visit_Stencil(self, ir: expr.Stencil, implementation: LineFormat):
+        irvar = ir.variable
+        assert isinstance(irvar.type, Grid)
+
+        self.depth = max(self.depth, abs(ir.time_offset))
+
+        indexes = ', '.join(
+            f"$dim{i} + {ir.space_offset[i]}" for i in range(irvar.type.dimension))
+        return f"(*{self.format_type(irvar.type, True)}_at({ir.variable.name}, {indexes}, {abs(ir.time_offset)}))"
+
+    def visit_GridInfo(self, ir: expr.GridInfo, implementation: LineFormat):
+        assert isinstance(ir.variable.type, Grid)
+
+        if ir.info == "dimension":
+            return str(ir.variable.type.dimension)
+        elif ir.info == "shape":
+            assert ir.dimension is not None
+
+            return f"{ir.variable.name}.shape[{self.visit(ir.dimension, implementation)}]"
```

### Comparing `xgrid-0.0.1/xgrid/lang/operator.py` & `xgrid-0.0.2/xgrid/lang/operator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from typing import Any, Callable
-from xgrid.lang.ir.statement import Definition
-from xgrid.lang.parser import Parser
-
-from xgrid.util.logging import Logger
-from xgrid.util.typing import BaseType
-from xgrid.xgrid import Grid as XGrid
-
-
-CustomTypecheck = Callable[[list[BaseType]], BaseType]
-
-
-class Operator:
-    def __init__(self, func, mode: str, name: str | None = None, includes: list[str] | None = None, self_type: BaseType | None = None, typecheck_override: CustomTypecheck | None = None, tick: bool = True) -> None:
-        self.func = func
-        self.mode = mode
-
-        self.logger = Logger(self)
-
-        self.name = func.__name__ if name is None else name
-        self.includes = [] if includes is None else includes
-
-        self.native = None
-        self.self_type = self_type
-        self.typecheck_override = typecheck_override
-        self.tick = tick
-
-    def __call__(self, *args: Any) -> Any:
-        if self.mode == "kernel":
-            if self.native is None:
-                from xgrid.lang.generator import Generator
-
-                self.native, self.depth = Generator(self).result
-
-            # tick the field and resize the time step if necessary
-            for arg in args:
-                if isinstance(arg, XGrid):
-                    arg._op_invoke(self.depth, self.tick)
-
-            return self.native(*args)
-        elif self.mode == "function":
-            return self.func(*args)
-        else:
-            self.logger.dead(
-                f"Invalid call to non-kernel or non-function ({self.mode}) operator '{self.name}'")
-
-    @property
-    def ir(self) -> Definition:
-        _ir = getattr(self, "_ir", None)
-        if _ir is None:
-            parser = Parser(self.func, self.name, self.mode, self.self_type)
-            self._ir = parser.result
-            self.includes.extend(parser.includes)
-        return self._ir
-    
-    @property
-    def src(self) -> str:
-        from xgrid.lang.generator import Generator
-        return Generator(self).source
-
-    @property
-    def signature(self):
-        return self.ir.signature
-
-
-def kernel(*, name: str | None = None, includes: list[str] | None = None, tick: bool = True):
-    def aux(func):
-        return Operator(func, "kernel", name, includes, tick=tick)
-    return aux
-
-
-def function(*, method: bool = False, name: str | None = None, includes: list[str] | None = None):
-    if method:
-        def aux_method(func):
-            setattr(func, "__xgrid_method", (name, includes))
-            return func
-        return aux_method
-    else:
-        def aux(func):
-            return Operator(func, "function", name, includes)
-        return aux
-
-
-def external(*, name: str | None = None, includes: list[str] | None = None, typecheck_override: CustomTypecheck):
-    def aux(func):
-        return Operator(func, "external", name, includes, typecheck_override=typecheck_override)
-    return aux
+from typing import Any, Callable
+from xgrid.lang.ir.statement import Definition
+from xgrid.lang.parser import Parser
+
+from xgrid.util.logging import Logger
+from xgrid.util.typing import BaseType
+from xgrid.xgrid import Grid as XGrid
+
+
+CustomTypecheck = Callable[[list[BaseType]], BaseType]
+
+
+class Operator:
+    def __init__(self, func, mode: str, name: str | None = None, includes: list[str] | None = None, self_type: BaseType | None = None, typecheck_override: CustomTypecheck | None = None, tick: bool = True) -> None:
+        self.func = func
+        self.mode = mode
+
+        self.logger = Logger(self)
+
+        self.name = func.__name__ if name is None else name
+        self.includes = [] if includes is None else includes
+
+        self.native = None
+        self.self_type = self_type
+        self.typecheck_override = typecheck_override
+        self.tick = tick
+
+    def __call__(self, *args: Any) -> Any:
+        if self.mode == "kernel":
+            if self.native is None:
+                from xgrid.lang.generator import Generator
+
+                self.native, self.depth = Generator(self).result
+
+            # tick the field and resize the time step if necessary
+            for arg in args:
+                if isinstance(arg, XGrid):
+                    arg._op_invoke(self.depth, self.tick)
+
+            return self.native(*args)
+        elif self.mode == "function":
+            return self.func(*args)
+        else:
+            self.logger.dead(
+                f"Invalid call to non-kernel or non-function ({self.mode}) operator '{self.name}'")
+
+    @property
+    def ir(self) -> Definition:
+        _ir = getattr(self, "_ir", None)
+        if _ir is None:
+            parser = Parser(self.func, self.name, self.mode, self.self_type)
+            self._ir = parser.result
+            self.includes.extend(parser.includes)
+        return self._ir
+    
+    @property
+    def src(self) -> str:
+        from xgrid.lang.generator import Generator
+        return Generator(self).source
+
+    @property
+    def signature(self):
+        return self.ir.signature
+
+
+def kernel(*, name: str | None = None, includes: list[str] | None = None, tick: bool = True):
+    def aux(func):
+        return Operator(func, "kernel", name, includes, tick=tick)
+    return aux
+
+
+def function(*, method: bool = False, name: str | None = None, includes: list[str] | None = None):
+    if method:
+        def aux_method(func):
+            setattr(func, "__xgrid_method", (name, includes))
+            return func
+        return aux_method
+    else:
+        def aux(func):
+            return Operator(func, "function", name, includes)
+        return aux
+
+
+def external(*, name: str | None = None, includes: list[str] | None = None, typecheck_override: CustomTypecheck):
+    def aux(func):
+        return Operator(func, "external", name, includes, typecheck_override=typecheck_override)
+    return aux
```

### Comparing `xgrid-0.0.1/xgrid/lang/parser.py` & `xgrid-0.0.2/xgrid/lang/parser.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,641 +1,641 @@
-import ast
-from functools import reduce
-import inspect
-import textwrap
-from typing import Literal, NoReturn, cast
-from struct import calcsize
-
-from xgrid.lang.ir import Location, Variable
-from xgrid.lang.ir.expression import Access, Binary, BinaryOperator, Call, Cast, Condition, Constant, Constructor, Expression, GridInfo, Identifier, Stencil, Terminal, Unary, UnaryOperator
-from xgrid.lang.ir.statement import Assignment, Definition, Break, Continue, Evaluation, For, If, Inline, Return, Signature, While
-from xgrid.util.init import get_config
-
-from xgrid.util.logging import Logger
-from xgrid.util.typing import BaseType, Void
-from xgrid.util.typing.annotation import parse_annotation
-from xgrid.util.typing.reference import Grid, Pointer, Reference
-from xgrid.util.typing.value import Boolean, Floating, Integer, Number, Structure, Value
-
-
-class OperatorMap:
-    unary: dict[type[ast.unaryop], UnaryOperator] = {
-        ast.UAdd: UnaryOperator.Pos,
-        ast.USub: UnaryOperator.Neg,
-        ast.Not: UnaryOperator.Not
-    }
-
-    binary: dict[type[ast.operator | ast.cmpop | ast.boolop], BinaryOperator] = {
-        ast.Add: BinaryOperator.Add,
-        ast.Sub: BinaryOperator.Sub,
-        ast.Mult: BinaryOperator.Mul,
-        ast.Div: BinaryOperator.Div,
-        ast.Pow: BinaryOperator.Pow,
-        ast.Mod: BinaryOperator.Mod,
-
-        ast.Eq: BinaryOperator.Eq,
-        ast.NotEq: BinaryOperator.Neq,
-        ast.Gt: BinaryOperator.Gt,
-        ast.GtE: BinaryOperator.Ge,
-        ast.Lt: BinaryOperator.Lt,
-        ast.LtE: BinaryOperator.Le,
-
-        ast.And: BinaryOperator.And,
-        ast.Or: BinaryOperator.Or
-    }
-
-
-def context(ctx: ast.expr_context):
-    if type(ctx) == ast.Load:
-        return "load"
-    else:
-        return "store"
-
-
-class Parser:
-    def __init__(self, func, name: str, mode: str, self_type: BaseType | None) -> None:
-        self.logger = Logger(self)
-        self.mode = mode
-        self.func = func
-        self.name = name
-
-        self.self_type = self_type
-
-        # extract source related information
-        file = inspect.getsourcefile(func)
-        self.file = "<unknown>" if file is None else file
-
-        # extract source code of function
-        lines, lineno = inspect.getsourcelines(func)
-
-        source = textwrap.dedent(
-            "\n".join(map(lambda x: textwrap.fill(x, tabsize=4, width=9999), lines)))
-
-        ast_definition = ast.parse(source, self.file).body[0]
-        ast.fix_missing_locations(ast_definition)
-        ast.increment_lineno(ast_definition, lineno)
-
-        self.context_stack = [mode]
-
-        self.scope: dict[str, Variable] = {}
-        self.boundary_mask = 0
-        self.args: list[tuple[str, BaseType]] = []
-        self.global_scope = func.__globals__
-        self.global_scope.update({"int": int, "float": float, "bool": bool})
-
-        self.includes = []
-
-        self.ir = self.visit(ast_definition)
-
-    @property
-    def result(self):
-        return self.ir
-
-    @property
-    def context(self):
-        return self.context_stack[-1]
-
-    def syntax_error(self, node: ast.AST, message: str) -> NoReturn:
-        self.logger.dead(
-            f"File {self.file}, line {node.lineno - 1}, in {self.name}",
-            f"  Syntax error: {message}")
-
-    def visit(self, node: ast.AST):
-        node_class = node.__class__.__name__
-        method = getattr(self, "visit_" + node_class, None)
-        if method is None:
-            self.syntax_error(node,
-                              f"Python syntax '{node_class}' is currently unsupported")
-        else:
-            return method(node)
-
-    def visits(self, l: list[ast.stmt]):
-        result = []
-        for item in l:
-            visited = self.visit(item)
-            if isinstance(visited, list):
-                result.extend(visited)
-            else:
-                result.append(visited)
-        return result
-
-    def location(self, node: ast.AST):
-        return Location(self.file, self.name, node.lineno - 1)
-
-    def visit_FunctionDef(self, node: ast.FunctionDef):
-        sig = inspect.signature(self.func)
-        for arg_name, arg_param in sig.parameters.items():
-            assert arg_name == arg_param.name
-
-            if arg_param.kind != inspect.Parameter.POSITIONAL_OR_KEYWORD:
-                self.syntax_error(node,
-                                  f"Argument '{arg_name}' of kind '{arg_param.kind}' is not supported")
-
-            if arg_param.annotation == inspect.Parameter.empty and self.self_type is None:
-                self.syntax_error(node,
-                                  f"Argument '{arg_name}' requires type annotation")
-
-            arg_type = self.self_type if arg_param.annotation == inspect.Parameter.empty else parse_annotation(
-                arg_param.annotation, self.global_scope)
-
-            if arg_type is None or isinstance(arg_type, Void):
-                self.syntax_error(node,
-                                  f"Argument '{arg_name}' requires non-void type annotation ({arg_param.annotation})")
-
-            self.scope[arg_name] = Variable(arg_name, arg_type)  # type: ignore
-            self.args.append((arg_name, arg_type))  # type: ignore
-
-        ret_sig = parse_annotation(sig.return_annotation)
-        if ret_sig is None or isinstance(ret_sig, Reference):
-            self.syntax_error(node, f"Invalid return type '{ret_sig}'")
-        self.return_type = ret_sig
-
-        return Definition(self.location(node),
-                          name=self.name,
-                          mode=self.mode,
-                          signature=Signature(self.args, self.return_type),
-                          scope=self.scope,
-                          body=[] if self.mode == "external" else self.visits(node.body))
-
-    # ===== statements =====
-    def visit_Return(self, node: ast.Return):
-        return_value = None if node.value is None else self.visit(node.value)
-        if return_value is not None:
-            if return_value.type != self.return_type:
-                self.syntax_error(
-                    node, f"Incompatible return type '{return_value.type}' with '{self.return_type}'")
-        return Return(self.location(node), return_value)
-
-    def visit_Pass(self, node: ast.Pass):
-        return []
-
-    def visit_Break(self, node: ast.Break):
-        return Break(self.location(node))
-
-    def visit_Continue(self, node: ast.Continue):
-        return Continue(self.location(node))
-
-    def visit_If(self, node: ast.If):
-        condition = cast(Expression, self.visit(node.test))
-
-        self.context_stack.append("if")
-        body = self.visits(node.body)
-        orelse = self.visits(node.orelse)
-        self.context_stack.pop()
-
-        return If(self.location(node), condition, body, orelse)
-
-    def visit_While(self, node: ast.While):
-        condition = cast(Expression, self.visit(node.test))
-
-        self.context_stack.append("while")
-        body = self.visits(node.body)
-        # orelse = self.visits(node.orelse)
-        if any(node.orelse):
-            self.syntax_error(
-                node, f"While statement does not support else clause")
-        self.context_stack.pop()
-
-        return While(self.location(node), condition, body)  # , orelse)
-
-    def visit_Expr(self, node: ast.Expr):
-        if self.context == "c":
-            if isinstance(node.value, ast.Constant) and isinstance(node.value.value, str):
-                docstring = node.value.value
-                return Inline(self.location(node), docstring)
-        else:
-            return Evaluation(self.location(node), cast(Expression, self.visit(node.value)))
-
-    def visit_With(self, node: ast.With):
-        if len(node.items) != 1:
-            self.syntax_error(node, "Only one pragma switch at once")
-
-        withitem = node.items[0]
-
-        if not isinstance(withitem.context_expr, ast.Call):
-            self.syntax_error(
-                node, f"Invalid pragma switch '{withitem.context_expr}'")
-        global_obj = self.resolve_global(withitem.context_expr.func)
-        import xgrid.lang as lang
-        if global_obj == lang.c:
-            self.context_stack.append("c")
-            body = self.visits(node.body)
-            self.context_stack.pop()
-            return body
-        elif global_obj == lang.boundary:
-            args = withitem.context_expr.args
-            if len(args) != 1 or not isinstance(args[0], ast.Constant) or type(args[0].value) != int:
-                self.syntax_error(node, f"Invalid pragram switch 'boundary")
-
-            boundary_mask = args[0].value
-            self.boundary_mask = boundary_mask
-            body = self.visits(node.body)
-            self.boundary_mask = 0
-            return body
-        else:
-            self.syntax_error(node, f"Unknown pragma switch '{global_obj}'")
-
-    def visit_Assign(self, node: ast.Assign):
-        location = self.location(node)
-        value = cast(Expression, self.visit(node.value))
-        if isinstance(value.type, Grid):
-            self.syntax_error(node, f"Incompatible assignment to grid type")
-
-        if len(node.targets) != 1:
-            self.syntax_error(node, f"Multiple assignment is not supported")
-        target = node.targets[0]
-
-        terminal = self.resolve_local(target)
-
-        # try to define new variable
-        if terminal is None:
-            if isinstance(target, ast.Name):
-                variable = Variable(target.id, value.type)
-                self.scope[target.id] = variable
-                terminal = Identifier(
-                    location, value.type, "load", variable)
-            else:
-                self.syntax_error(node, f"Undefined identifier {terminal}")
-
-        if terminal.type != value.type:
-            self.syntax_error(
-                node, f"Incompatible assignment from type {value.type} to {terminal.type}")
-
-        return Assignment(location, terminal, value)
-
-    def visit_AugAssign(self, node: ast.AugAssign):
-        value = cast(Expression, self.visit(node.value))
-        target = self.resolve_local(node.target)
-        if target is None:
-            self.syntax_error(node, f"Undefined identifier {target}")
-
-        optype = type(node.op)
-        if optype not in OperatorMap.binary:
-            self.syntax_error(
-                node, f"Unsupported binary operator '{optype.__name__}'")
-        binary_op = OperatorMap.binary[optype]
-
-        if not isinstance(target.type, Number) or not isinstance(value.type, Number) or target.type != value.type:
-            self.syntax_error(
-                node, f"Incompatible binary operator '{binary_op.value}' with type '{target.type}' and '{value.type}'")
-
-        if binary_op == BinaryOperator.Pow:
-            return_type = Floating(64) if isinstance(
-                target.type, Floating) and value.type.width_bits == 64 else Floating(32)
-        else:
-            return_type = target.type
-
-        return Assignment(self.location(node), target, Binary(self.location(node), return_type, target, value, binary_op))
-
-    def visit_For(self, node: ast.For):
-        if not isinstance(node.target, ast.Name):
-            self.syntax_error(
-                node, f"For loop variable should be a name")
-
-        # check whether is range or not
-        iter_range = node.iter
-        if not isinstance(iter_range, ast.Call) or not isinstance(iter_range.func, ast.Name) or iter_range.func.id != "range":
-            self.syntax_error(node, f"For loop only supports range")
-
-        args = iter_range.args
-        if len(args) not in (2, 3):
-            self.syntax_error(
-                node, f"For loop requires start:end:step or start:end")
-
-        loop_range: list[Expression] = list(map(self.visit, args))
-        if len(loop_range) == 2:
-            loop_range.append(Constant(self.location(node),
-                              Integer(calcsize("i")), 1))
-
-        # check type of loop range
-        loop_range_type = loop_range[2].type
-        for lr in loop_range:
-            if lr.type != loop_range_type or not isinstance(lr.type, Number):
-                self.syntax_error(
-                    node, f"Incompatible loop range type '{lr.type}'")
-
-        var_id = node.target.id
-        if var_id not in self.scope:
-            self.scope[var_id] = Variable(var_id, loop_range_type)
-
-        loop_var = self.scope[var_id]
-        if loop_var.type != loop_range_type:
-            self.syntax_error(
-                node, f"Incompatible loop variable type '{loop_var.type}' with range type '{loop_range_type}'")
-
-        body = self.visits(node.body)
-        return For(self.location(node), loop_var, loop_range[0], loop_range[1], loop_range[2], body)
-
-    def visit_Import(self, node: ast.Import):
-        for name in node.names:
-            if name.asname is not None:
-                self.syntax_error(
-                    node, f"Using import as include requires no alias for '{name.name}'")
-
-            include_name = name.name.replace('.', '/')
-            self.includes.append(include_name + ".h")
-
-        return []
-
-    # ===== expressions =====
-    def parse_constant(self, node: ast.AST, constant):
-        vtype = {int: Integer(calcsize("i")), float: Floating(get_config().fsize),
-                 bool: Boolean()}
-        if type(constant) not in vtype:
-            self.syntax_error(
-                node, f"Incompatible constant '{constant}' of type '{type(constant)}'")
-        return Constant(self.location(node), vtype[type(constant)], constant)
-
-    def visit_Constant(self, node: ast.Constant):
-        return self.parse_constant(node, node.value)
-
-    def visit_UnaryOp(self, node: ast.UnaryOp):
-        optype = type(node.op)
-        if optype not in OperatorMap.unary:
-            self.syntax_error(
-                node, f"Unsupported unary operator '{optype.__name__}'")
-        unary_op = OperatorMap.unary[optype]
-
-        right = cast(Expression, self.visit(node.operand))
-        if (unary_op == UnaryOperator.Not and not isinstance(right.type, Boolean)) or (unary_op in (UnaryOperator.Pos, UnaryOperator.Neg) and not isinstance(right.type, Number)):
-            self.syntax_error(
-                node, f"Incompatible unary operator '{unary_op.value}' with type '{right.type}'")
-
-        return Unary(self.location(node), right.type, right, unary_op)
-
-    def visit_BinOp(self, node: ast.BinOp):
-        optype = type(node.op)
-        if optype not in OperatorMap.binary:
-            self.syntax_error(
-                node, f"Unsupported binary operator '{optype.__name__}'")
-        binary_op = OperatorMap.binary[optype]
-
-        left = cast(Expression, self.visit(node.left))
-        right = cast(Expression, self.visit(node.right))
-        if not isinstance(left.type, Number) or not isinstance(right.type, Number) or left.type != right.type:
-            self.syntax_error(
-                node, f"Incompatible binary operator '{binary_op.value}' with type '{left.type}' and '{right.type}'")
-
-        if binary_op == BinaryOperator.Pow:
-            return_type = Floating(calcsize("d")) if isinstance(
-                left.type, Floating) and left.type.width_bits == 64 else Floating(get_config().fsize)
-        else:
-            return_type = left.type
-
-        return Binary(self.location(node), return_type, left, right, binary_op)
-
-    def visit_BoolOp(self, node: ast.BoolOp):
-        location = self.location(node)
-        op = OperatorMap.binary[type(node.op)]
-        values = [cast(Expression, self.visit(i)) for i in node.values]
-        for value in values:
-            if not isinstance(value.type, Boolean):
-                self.syntax_error(
-                    node, f"Incompatible boolean operator '{op.value}' with '{value.type}'")
-        return reduce(lambda x, y: Binary(location, Boolean(), x, y, op), values)
-
-    def visit_Compare(self, node: ast.Compare):
-        location = self.location(node)
-        left = cast(Expression, self.visit(node.left))
-        if not isinstance(left.type, Number):
-            self.syntax_error(
-                node, f"Incompatible compare expression with type '{left.type}'")
-
-        comparators = [cast(Expression, self.visit(i))
-                       for i in node.comparators]
-        ops = [OperatorMap.binary[type(i)] for i in node.ops]
-
-        for i, comparator in enumerate(comparators):
-            if comparator.type != left.type:
-                self.syntax_error(
-                    node, f"Incompatible compare operator '{ops[i].value}' with type '{left.type}' and '{comparator.type}'")
-
-        boolean = Boolean()
-        return reduce(lambda x, y: Binary(location, boolean, x, y, BinaryOperator.And),
-                      [Binary(location, boolean, left, comparators[i], ops[i]) for i in range(len(ops))])
-
-    def visit_IfExp(self, node: ast.IfExp):
-        condition = cast(Expression, self.visit(node.test))
-        if not isinstance(condition.type, Boolean):
-            self.syntax_error(
-                node, f"Incompatible condition type '{condition.type}' of if expression")
-        body = cast(Expression, self.visit(node.body))
-        orelse = cast(Expression, self.visit(node.orelse))
-        if body.type != orelse.type or not isinstance(body.type, Value):
-            self.syntax_error(
-                node, f"Incompatible type '{body.type}' and '{orelse.type}' of if expression")
-        return Condition(self.location(node), body.type, condition, body, orelse)
-
-    def resolve_global(self, node: ast.AST):
-        names = []
-        while True:
-            if isinstance(node, ast.Name):
-                names.append(node.id)
-                break
-            elif isinstance(node, ast.Attribute):
-                names.append(node.attr)
-                node = node.value
-            else:
-                self.syntax_error(
-                    node, f"Python syntax '{node.__class__.__name__}' is currently unsupported")
-
-        names.reverse()
-
-        scope = self.global_scope
-        resolved_names = ["globals"]
-        for attr in names:
-            try:
-                scope = scope[attr] if isinstance(
-                    scope, dict) else getattr(scope, attr)
-                resolved_names.append(attr)
-            except KeyError:
-                self.syntax_error(
-                    node, f"Undefined attribute '{attr}' of '{'.'.join(resolved_names)}'")
-
-        return scope
-
-    def resolve_local(self, node: ast.AST) -> Terminal | None:
-        location = self.location(node)
-
-        if isinstance(node, ast.Subscript):
-            def extract_space(grid: ast.Subscript, time_offset: int):
-                # or self.context not in ("kernel", "critical", "boundary", "if"):
-                if not isinstance(grid.value, ast.Name):
-                    self.syntax_error(
-                        grid, f"Incompatible subscript to '{grid.value.__class__.__name__}' under context '{self.context}'")
-
-                if grid.value.id not in self.scope:
-                    self.syntax_error(
-                        grid, f"Undefined identifier '{grid.value.id}'")
-
-                grid_var = self.scope[grid.value.id]
-                if not isinstance(grid_var.type, Grid):
-                    self.syntax_error(
-                        grid, f"Incompatible subscript to type '{grid_var.type}'")
-
-                location = self.location(grid)
-                ctx = context(grid.ctx)
-
-                if isinstance(grid.slice, ast.Tuple):
-                    space_slices = grid.slice.elts
-                else:
-                    space_slices = [grid.slice]
-
-                spaces = []
-                for space_slice in space_slices:
-                    failed = False
-                    value = 0
-                    if isinstance(space_slice, ast.UnaryOp):
-                        if type(space_slice.op) != ast.USub:
-                            failed = True
-                        else:
-                            if not isinstance(space_slice.operand, ast.Constant) or type(space_slice.operand.value) != int:
-                                failed = True
-                            else:
-                                value = -space_slice.operand.value
-                    elif isinstance(space_slice, ast.Constant):
-                        if type(space_slice.value) != int:
-                            failed = True
-                        else:
-                            value = space_slice.value
-
-                    if failed:
-                        self.syntax_error(
-                            grid, f"Incompatible subscript '{space_slice}'")
-                    spaces.append(value)
-
-                if len(spaces) != grid_var.type.dimension:
-                    self.syntax_error(
-                        grid, f"Incompatible subscript length '{len(spaces)}' with dimension {grid_var.type.dimension}")
-
-                return Stencil(location, grid_var.type.element, ctx, grid_var, time_offset, spaces, self.boundary_mask)
-
-            if isinstance(node.value, ast.Subscript):
-                time_slice = node.slice
-                if isinstance(time_slice, ast.Constant) and type(time_slice.value) == int:
-                    time_offset = time_slice.value
-                elif isinstance(time_slice, ast.UnaryOp) and type(time_slice.op) == ast.USub and isinstance(time_slice.operand, ast.Constant) and type(time_slice.operand.value) == int:
-                    time_offset = -time_slice.operand.value
-                else:
-                    self.syntax_error(
-                        node.value, f"Invalid time dimension subscript to '{node.value.__class__.__name__}")
-                node = node.value
-            else:
-                time_offset = 0 if context(node.ctx) == "store" else -1
-
-            return extract_space(node, time_offset)
-
-        elif isinstance(node, ast.Attribute):
-            value = self.resolve_local(node.value)
-
-            if value is None or not isinstance(value.type, Structure) or node.attr not in value.type.elements_map:
-                return None
-            else:
-                return Access(location, value.type.elements_map[node.attr], context(node.ctx), value, node.attr)
-
-        elif isinstance(node, ast.Name):
-            try:
-                variable = self.scope[node.id]
-                t = variable.type.element if isinstance(
-                    variable.type, Pointer) else variable.type
-                return Identifier(self.location(node), t, context(node.ctx), variable)
-            except KeyError:
-                return None
-
-        else:
-            self.syntax_error(
-                node, f"Python syntax '{node.__class__.__name__}' is currently unsupported")
-
-    def visit_Name(self, node: ast.Name):
-        local = self.resolve_local(node)
-        return self.parse_constant(node, self.resolve_global(node)) if local is None else local
-
-    def visit_Attribute(self, node: ast.Attribute):
-        local = self.resolve_local(node)
-        return self.parse_constant(node, self.resolve_global(node)) if local is None else local
-
-    def visit_Subscript(self, node: ast.Subscript):
-        return self.resolve_local(node)
-
-    def visit_Call(self, node: ast.Call):
-        from xgrid.lang.operator import Operator
-
-        func_name = None
-        self_type = None
-
-        if isinstance(node.func, ast.Attribute) and (local_obj := self.resolve_local(node.func.value)) is not None:
-            if isinstance(local_obj.type, Structure):
-                func = getattr(
-                    local_obj.type.dataclass, node.func.attr, None)
-                func_name = f"{local_obj.type.dataclass.__qualname__}.{node.func.attr}"
-                self_type = local_obj.type
-            else:
-                # fixed method call, in the future ?
-                self.syntax_error(
-                    node, f"Invalid method call on type {local_obj.type}")
-
-            args: list[Expression] = [local_obj]
-        else:
-            func = self.resolve_global(node.func)
-            args = []
-
-        # specially handle cast expression
-        if func == cast:
-            if len(node.args) != 2:
-                self.syntax_error(
-                    node, f"Cast requires 2 arguments, got {len(node.args)}")
-            target_type = parse_annotation(self.resolve_global(node.args[0]))
-            if target_type is None:
-                self.syntax_error(node, f"Invalid cast type")
-            return Cast(self.location(node), target_type, self.visit(node.args[1]))
-
-        args.extend(self.visit(i) for i in node.args)
-
-        # specially handle type constructor
-        if isinstance(func, type):
-            internal_type = parse_annotation(func)
-            if internal_type is None or not isinstance(internal_type, Structure):
-                self.syntax_error(
-                    node, f"Invalid type constructor '{func.__name__}'")
-
-            func = Constructor(internal_type, Signature(
-                list(internal_type.elements), internal_type))
-            func_name = f"{internal_type.name}.constructor"
-
-        # type check the function and arguments
-        if not isinstance(func, Operator) and not isinstance(func, Constructor):
-            # check the lazy method flag
-            method_flag = getattr(func, "__xgrid_method", None)
-            if method_flag is not None and self_type is not None:
-                func = Operator(func, "function",
-                                method_flag[0], method_flag[1], self_type)
-            else:
-                self.syntax_error(
-                    node, f"Invalid call to object '{func}', it is not an operator")
-
-        if func_name is None:
-            func_name = func.name  # type: ignore
-
-        if (expected := len(func.signature.arguments)) != len(args):
-            self.syntax_error(
-                node, f"Operator '{func_name}' requires {expected} arguments, but got {len(args)}")
-
-        if isinstance(func, Operator) and func.mode == "external" and func.typecheck_override is not None:
-            try:
-                return_type = func.typecheck_override([i.type for i in args])
-            except Exception as e:
-                self.syntax_error(node, e.args[0])
-
-            if func.name in ("shape", "dimension"):
-                if not isinstance(args[0], Identifier):
-                    self.syntax_error(
-                        node, f"Incompatible '{func.name}' to argument '{args[0]}'")
-
-                return GridInfo(self.location(node), Integer(calcsize("i")), cast(Literal["shape", "dimension"], func.name), args[0].variable, args[1] if func.name == "shape" else None)
-        else:
-            for id, (arg_name, arg_type) in enumerate(func.signature.arguments):
-                if arg_type != args[id].type:
-                    self.syntax_error(
-                        node, f"Incompatible type '{args[id].type}' with '{arg_type}' of argument '{arg_name}, operator '{func_name}'")
-            return_type = func.signature.return_type
-
-        return Call(self.location(node), return_type, func, args)
+import ast
+from functools import reduce
+import inspect
+import textwrap
+from typing import Literal, NoReturn, cast
+from struct import calcsize
+
+from xgrid.lang.ir import Location, Variable
+from xgrid.lang.ir.expression import Access, Binary, BinaryOperator, Call, Cast, Condition, Constant, Constructor, Expression, GridInfo, Identifier, Stencil, Terminal, Unary, UnaryOperator
+from xgrid.lang.ir.statement import Assignment, Definition, Break, Continue, Evaluation, For, If, Inline, Return, Signature, While
+from xgrid.util.init import get_config
+
+from xgrid.util.logging import Logger
+from xgrid.util.typing import BaseType, Void
+from xgrid.util.typing.annotation import parse_annotation
+from xgrid.util.typing.reference import Grid, Pointer, Reference
+from xgrid.util.typing.value import Boolean, Floating, Integer, Number, Structure, Value
+
+
+class OperatorMap:
+    unary: dict[type[ast.unaryop], UnaryOperator] = {
+        ast.UAdd: UnaryOperator.Pos,
+        ast.USub: UnaryOperator.Neg,
+        ast.Not: UnaryOperator.Not
+    }
+
+    binary: dict[type[ast.operator | ast.cmpop | ast.boolop], BinaryOperator] = {
+        ast.Add: BinaryOperator.Add,
+        ast.Sub: BinaryOperator.Sub,
+        ast.Mult: BinaryOperator.Mul,
+        ast.Div: BinaryOperator.Div,
+        ast.Pow: BinaryOperator.Pow,
+        ast.Mod: BinaryOperator.Mod,
+
+        ast.Eq: BinaryOperator.Eq,
+        ast.NotEq: BinaryOperator.Neq,
+        ast.Gt: BinaryOperator.Gt,
+        ast.GtE: BinaryOperator.Ge,
+        ast.Lt: BinaryOperator.Lt,
+        ast.LtE: BinaryOperator.Le,
+
+        ast.And: BinaryOperator.And,
+        ast.Or: BinaryOperator.Or
+    }
+
+
+def context(ctx: ast.expr_context):
+    if type(ctx) == ast.Load:
+        return "load"
+    else:
+        return "store"
+
+
+class Parser:
+    def __init__(self, func, name: str, mode: str, self_type: BaseType | None) -> None:
+        self.logger = Logger(self)
+        self.mode = mode
+        self.func = func
+        self.name = name
+
+        self.self_type = self_type
+
+        # extract source related information
+        file = inspect.getsourcefile(func)
+        self.file = "<unknown>" if file is None else file
+
+        # extract source code of function
+        lines, lineno = inspect.getsourcelines(func)
+
+        source = textwrap.dedent(
+            "\n".join(map(lambda x: textwrap.fill(x, tabsize=4, width=9999), lines)))
+
+        ast_definition = ast.parse(source, self.file).body[0]
+        ast.fix_missing_locations(ast_definition)
+        ast.increment_lineno(ast_definition, lineno)
+
+        self.context_stack = [mode]
+
+        self.scope: dict[str, Variable] = {}
+        self.boundary_mask = 0
+        self.args: list[tuple[str, BaseType]] = []
+        self.global_scope = func.__globals__
+        self.global_scope.update({"int": int, "float": float, "bool": bool})
+
+        self.includes = []
+
+        self.ir = self.visit(ast_definition)
+
+    @property
+    def result(self):
+        return self.ir
+
+    @property
+    def context(self):
+        return self.context_stack[-1]
+
+    def syntax_error(self, node: ast.AST, message: str) -> NoReturn:
+        self.logger.dead(
+            f"File {self.file}, line {node.lineno - 1}, in {self.name}",
+            f"  Syntax error: {message}")
+
+    def visit(self, node: ast.AST):
+        node_class = node.__class__.__name__
+        method = getattr(self, "visit_" + node_class, None)
+        if method is None:
+            self.syntax_error(node,
+                              f"Python syntax '{node_class}' is currently unsupported")
+        else:
+            return method(node)
+
+    def visits(self, l: list[ast.stmt]):
+        result = []
+        for item in l:
+            visited = self.visit(item)
+            if isinstance(visited, list):
+                result.extend(visited)
+            else:
+                result.append(visited)
+        return result
+
+    def location(self, node: ast.AST):
+        return Location(self.file, self.name, node.lineno - 1)
+
+    def visit_FunctionDef(self, node: ast.FunctionDef):
+        sig = inspect.signature(self.func)
+        for arg_name, arg_param in sig.parameters.items():
+            assert arg_name == arg_param.name
+
+            if arg_param.kind != inspect.Parameter.POSITIONAL_OR_KEYWORD:
+                self.syntax_error(node,
+                                  f"Argument '{arg_name}' of kind '{arg_param.kind}' is not supported")
+
+            if arg_param.annotation == inspect.Parameter.empty and self.self_type is None:
+                self.syntax_error(node,
+                                  f"Argument '{arg_name}' requires type annotation")
+
+            arg_type = self.self_type if arg_param.annotation == inspect.Parameter.empty else parse_annotation(
+                arg_param.annotation, self.global_scope)
+
+            if arg_type is None or isinstance(arg_type, Void):
+                self.syntax_error(node,
+                                  f"Argument '{arg_name}' requires non-void type annotation ({arg_param.annotation})")
+
+            self.scope[arg_name] = Variable(arg_name, arg_type)  # type: ignore
+            self.args.append((arg_name, arg_type))  # type: ignore
+
+        ret_sig = parse_annotation(sig.return_annotation)
+        if ret_sig is None or isinstance(ret_sig, Reference):
+            self.syntax_error(node, f"Invalid return type '{ret_sig}'")
+        self.return_type = ret_sig
+
+        return Definition(self.location(node),
+                          name=self.name,
+                          mode=self.mode,
+                          signature=Signature(self.args, self.return_type),
+                          scope=self.scope,
+                          body=[] if self.mode == "external" else self.visits(node.body))
+
+    # ===== statements =====
+    def visit_Return(self, node: ast.Return):
+        return_value = None if node.value is None else self.visit(node.value)
+        if return_value is not None:
+            if return_value.type != self.return_type:
+                self.syntax_error(
+                    node, f"Incompatible return type '{return_value.type}' with '{self.return_type}'")
+        return Return(self.location(node), return_value)
+
+    def visit_Pass(self, node: ast.Pass):
+        return []
+
+    def visit_Break(self, node: ast.Break):
+        return Break(self.location(node))
+
+    def visit_Continue(self, node: ast.Continue):
+        return Continue(self.location(node))
+
+    def visit_If(self, node: ast.If):
+        condition = cast(Expression, self.visit(node.test))
+
+        self.context_stack.append("if")
+        body = self.visits(node.body)
+        orelse = self.visits(node.orelse)
+        self.context_stack.pop()
+
+        return If(self.location(node), condition, body, orelse)
+
+    def visit_While(self, node: ast.While):
+        condition = cast(Expression, self.visit(node.test))
+
+        self.context_stack.append("while")
+        body = self.visits(node.body)
+        # orelse = self.visits(node.orelse)
+        if any(node.orelse):
+            self.syntax_error(
+                node, f"While statement does not support else clause")
+        self.context_stack.pop()
+
+        return While(self.location(node), condition, body)  # , orelse)
+
+    def visit_Expr(self, node: ast.Expr):
+        if self.context == "c":
+            if isinstance(node.value, ast.Constant) and isinstance(node.value.value, str):
+                docstring = node.value.value
+                return Inline(self.location(node), docstring)
+        else:
+            return Evaluation(self.location(node), cast(Expression, self.visit(node.value)))
+
+    def visit_With(self, node: ast.With):
+        if len(node.items) != 1:
+            self.syntax_error(node, "Only one pragma switch at once")
+
+        withitem = node.items[0]
+
+        if not isinstance(withitem.context_expr, ast.Call):
+            self.syntax_error(
+                node, f"Invalid pragma switch '{withitem.context_expr}'")
+        global_obj = self.resolve_global(withitem.context_expr.func)
+        import xgrid.lang as lang
+        if global_obj == lang.c:
+            self.context_stack.append("c")
+            body = self.visits(node.body)
+            self.context_stack.pop()
+            return body
+        elif global_obj == lang.boundary:
+            args = withitem.context_expr.args
+            if len(args) != 1 or not isinstance(args[0], ast.Constant) or type(args[0].value) != int:
+                self.syntax_error(node, f"Invalid pragram switch 'boundary")
+
+            boundary_mask = args[0].value
+            self.boundary_mask = boundary_mask
+            body = self.visits(node.body)
+            self.boundary_mask = 0
+            return body
+        else:
+            self.syntax_error(node, f"Unknown pragma switch '{global_obj}'")
+
+    def visit_Assign(self, node: ast.Assign):
+        location = self.location(node)
+        value = cast(Expression, self.visit(node.value))
+        if isinstance(value.type, Grid):
+            self.syntax_error(node, f"Incompatible assignment to grid type")
+
+        if len(node.targets) != 1:
+            self.syntax_error(node, f"Multiple assignment is not supported")
+        target = node.targets[0]
+
+        terminal = self.resolve_local(target)
+
+        # try to define new variable
+        if terminal is None:
+            if isinstance(target, ast.Name):
+                variable = Variable(target.id, value.type)
+                self.scope[target.id] = variable
+                terminal = Identifier(
+                    location, value.type, "load", variable)
+            else:
+                self.syntax_error(node, f"Undefined identifier {terminal}")
+
+        if terminal.type != value.type:
+            self.syntax_error(
+                node, f"Incompatible assignment from type {value.type} to {terminal.type}")
+
+        return Assignment(location, terminal, value)
+
+    def visit_AugAssign(self, node: ast.AugAssign):
+        value = cast(Expression, self.visit(node.value))
+        target = self.resolve_local(node.target)
+        if target is None:
+            self.syntax_error(node, f"Undefined identifier {target}")
+
+        optype = type(node.op)
+        if optype not in OperatorMap.binary:
+            self.syntax_error(
+                node, f"Unsupported binary operator '{optype.__name__}'")
+        binary_op = OperatorMap.binary[optype]
+
+        if not isinstance(target.type, Number) or not isinstance(value.type, Number) or target.type != value.type:
+            self.syntax_error(
+                node, f"Incompatible binary operator '{binary_op.value}' with type '{target.type}' and '{value.type}'")
+
+        if binary_op == BinaryOperator.Pow:
+            return_type = Floating(64) if isinstance(
+                target.type, Floating) and value.type.width_bits == 64 else Floating(32)
+        else:
+            return_type = target.type
+
+        return Assignment(self.location(node), target, Binary(self.location(node), return_type, target, value, binary_op))
+
+    def visit_For(self, node: ast.For):
+        if not isinstance(node.target, ast.Name):
+            self.syntax_error(
+                node, f"For loop variable should be a name")
+
+        # check whether is range or not
+        iter_range = node.iter
+        if not isinstance(iter_range, ast.Call) or not isinstance(iter_range.func, ast.Name) or iter_range.func.id != "range":
+            self.syntax_error(node, f"For loop only supports range")
+
+        args = iter_range.args
+        if len(args) not in (2, 3):
+            self.syntax_error(
+                node, f"For loop requires start:end:step or start:end")
+
+        loop_range: list[Expression] = list(map(self.visit, args))
+        if len(loop_range) == 2:
+            loop_range.append(Constant(self.location(node),
+                              Integer(calcsize("i")), 1))
+
+        # check type of loop range
+        loop_range_type = loop_range[2].type
+        for lr in loop_range:
+            if lr.type != loop_range_type or not isinstance(lr.type, Number):
+                self.syntax_error(
+                    node, f"Incompatible loop range type '{lr.type}'")
+
+        var_id = node.target.id
+        if var_id not in self.scope:
+            self.scope[var_id] = Variable(var_id, loop_range_type)
+
+        loop_var = self.scope[var_id]
+        if loop_var.type != loop_range_type:
+            self.syntax_error(
+                node, f"Incompatible loop variable type '{loop_var.type}' with range type '{loop_range_type}'")
+
+        body = self.visits(node.body)
+        return For(self.location(node), loop_var, loop_range[0], loop_range[1], loop_range[2], body)
+
+    def visit_Import(self, node: ast.Import):
+        for name in node.names:
+            if name.asname is not None:
+                self.syntax_error(
+                    node, f"Using import as include requires no alias for '{name.name}'")
+
+            include_name = name.name.replace('.', '/')
+            self.includes.append(include_name + ".h")
+
+        return []
+
+    # ===== expressions =====
+    def parse_constant(self, node: ast.AST, constant):
+        vtype = {int: Integer(calcsize("i")), float: Floating(get_config().fsize),
+                 bool: Boolean()}
+        if type(constant) not in vtype:
+            self.syntax_error(
+                node, f"Incompatible constant '{constant}' of type '{type(constant)}'")
+        return Constant(self.location(node), vtype[type(constant)], constant)
+
+    def visit_Constant(self, node: ast.Constant):
+        return self.parse_constant(node, node.value)
+
+    def visit_UnaryOp(self, node: ast.UnaryOp):
+        optype = type(node.op)
+        if optype not in OperatorMap.unary:
+            self.syntax_error(
+                node, f"Unsupported unary operator '{optype.__name__}'")
+        unary_op = OperatorMap.unary[optype]
+
+        right = cast(Expression, self.visit(node.operand))
+        if (unary_op == UnaryOperator.Not and not isinstance(right.type, Boolean)) or (unary_op in (UnaryOperator.Pos, UnaryOperator.Neg) and not isinstance(right.type, Number)):
+            self.syntax_error(
+                node, f"Incompatible unary operator '{unary_op.value}' with type '{right.type}'")
+
+        return Unary(self.location(node), right.type, right, unary_op)
+
+    def visit_BinOp(self, node: ast.BinOp):
+        optype = type(node.op)
+        if optype not in OperatorMap.binary:
+            self.syntax_error(
+                node, f"Unsupported binary operator '{optype.__name__}'")
+        binary_op = OperatorMap.binary[optype]
+
+        left = cast(Expression, self.visit(node.left))
+        right = cast(Expression, self.visit(node.right))
+        if not isinstance(left.type, Number) or not isinstance(right.type, Number) or left.type != right.type:
+            self.syntax_error(
+                node, f"Incompatible binary operator '{binary_op.value}' with type '{left.type}' and '{right.type}'")
+
+        if binary_op == BinaryOperator.Pow:
+            return_type = Floating(calcsize("d")) if isinstance(
+                left.type, Floating) and left.type.width_bits == 64 else Floating(get_config().fsize)
+        else:
+            return_type = left.type
+
+        return Binary(self.location(node), return_type, left, right, binary_op)
+
+    def visit_BoolOp(self, node: ast.BoolOp):
+        location = self.location(node)
+        op = OperatorMap.binary[type(node.op)]
+        values = [cast(Expression, self.visit(i)) for i in node.values]
+        for value in values:
+            if not isinstance(value.type, Boolean):
+                self.syntax_error(
+                    node, f"Incompatible boolean operator '{op.value}' with '{value.type}'")
+        return reduce(lambda x, y: Binary(location, Boolean(), x, y, op), values)
+
+    def visit_Compare(self, node: ast.Compare):
+        location = self.location(node)
+        left = cast(Expression, self.visit(node.left))
+        if not isinstance(left.type, Number):
+            self.syntax_error(
+                node, f"Incompatible compare expression with type '{left.type}'")
+
+        comparators = [cast(Expression, self.visit(i))
+                       for i in node.comparators]
+        ops = [OperatorMap.binary[type(i)] for i in node.ops]
+
+        for i, comparator in enumerate(comparators):
+            if comparator.type != left.type:
+                self.syntax_error(
+                    node, f"Incompatible compare operator '{ops[i].value}' with type '{left.type}' and '{comparator.type}'")
+
+        boolean = Boolean()
+        return reduce(lambda x, y: Binary(location, boolean, x, y, BinaryOperator.And),
+                      [Binary(location, boolean, left, comparators[i], ops[i]) for i in range(len(ops))])
+
+    def visit_IfExp(self, node: ast.IfExp):
+        condition = cast(Expression, self.visit(node.test))
+        if not isinstance(condition.type, Boolean):
+            self.syntax_error(
+                node, f"Incompatible condition type '{condition.type}' of if expression")
+        body = cast(Expression, self.visit(node.body))
+        orelse = cast(Expression, self.visit(node.orelse))
+        if body.type != orelse.type or not isinstance(body.type, Value):
+            self.syntax_error(
+                node, f"Incompatible type '{body.type}' and '{orelse.type}' of if expression")
+        return Condition(self.location(node), body.type, condition, body, orelse)
+
+    def resolve_global(self, node: ast.AST):
+        names = []
+        while True:
+            if isinstance(node, ast.Name):
+                names.append(node.id)
+                break
+            elif isinstance(node, ast.Attribute):
+                names.append(node.attr)
+                node = node.value
+            else:
+                self.syntax_error(
+                    node, f"Python syntax '{node.__class__.__name__}' is currently unsupported")
+
+        names.reverse()
+
+        scope = self.global_scope
+        resolved_names = ["globals"]
+        for attr in names:
+            try:
+                scope = scope[attr] if isinstance(
+                    scope, dict) else getattr(scope, attr)
+                resolved_names.append(attr)
+            except KeyError:
+                self.syntax_error(
+                    node, f"Undefined attribute '{attr}' of '{'.'.join(resolved_names)}'")
+
+        return scope
+
+    def resolve_local(self, node: ast.AST) -> Terminal | None:
+        location = self.location(node)
+
+        if isinstance(node, ast.Subscript):
+            def extract_space(grid: ast.Subscript, time_offset: int):
+                # or self.context not in ("kernel", "critical", "boundary", "if"):
+                if not isinstance(grid.value, ast.Name):
+                    self.syntax_error(
+                        grid, f"Incompatible subscript to '{grid.value.__class__.__name__}' under context '{self.context}'")
+
+                if grid.value.id not in self.scope:
+                    self.syntax_error(
+                        grid, f"Undefined identifier '{grid.value.id}'")
+
+                grid_var = self.scope[grid.value.id]
+                if not isinstance(grid_var.type, Grid):
+                    self.syntax_error(
+                        grid, f"Incompatible subscript to type '{grid_var.type}'")
+
+                location = self.location(grid)
+                ctx = context(grid.ctx)
+
+                if isinstance(grid.slice, ast.Tuple):
+                    space_slices = grid.slice.elts
+                else:
+                    space_slices = [grid.slice]
+
+                spaces = []
+                for space_slice in space_slices:
+                    failed = False
+                    value = 0
+                    if isinstance(space_slice, ast.UnaryOp):
+                        if type(space_slice.op) != ast.USub:
+                            failed = True
+                        else:
+                            if not isinstance(space_slice.operand, ast.Constant) or type(space_slice.operand.value) != int:
+                                failed = True
+                            else:
+                                value = -space_slice.operand.value
+                    elif isinstance(space_slice, ast.Constant):
+                        if type(space_slice.value) != int:
+                            failed = True
+                        else:
+                            value = space_slice.value
+
+                    if failed:
+                        self.syntax_error(
+                            grid, f"Incompatible subscript '{space_slice}'")
+                    spaces.append(value)
+
+                if len(spaces) != grid_var.type.dimension:
+                    self.syntax_error(
+                        grid, f"Incompatible subscript length '{len(spaces)}' with dimension {grid_var.type.dimension}")
+
+                return Stencil(location, grid_var.type.element, ctx, grid_var, time_offset, spaces, self.boundary_mask)
+
+            if isinstance(node.value, ast.Subscript):
+                time_slice = node.slice
+                if isinstance(time_slice, ast.Constant) and type(time_slice.value) == int:
+                    time_offset = time_slice.value
+                elif isinstance(time_slice, ast.UnaryOp) and type(time_slice.op) == ast.USub and isinstance(time_slice.operand, ast.Constant) and type(time_slice.operand.value) == int:
+                    time_offset = -time_slice.operand.value
+                else:
+                    self.syntax_error(
+                        node.value, f"Invalid time dimension subscript to '{node.value.__class__.__name__}")
+                node = node.value
+            else:
+                time_offset = 0 if context(node.ctx) == "store" else -1
+
+            return extract_space(node, time_offset)
+
+        elif isinstance(node, ast.Attribute):
+            value = self.resolve_local(node.value)
+
+            if value is None or not isinstance(value.type, Structure) or node.attr not in value.type.elements_map:
+                return None
+            else:
+                return Access(location, value.type.elements_map[node.attr], context(node.ctx), value, node.attr)
+
+        elif isinstance(node, ast.Name):
+            try:
+                variable = self.scope[node.id]
+                t = variable.type.element if isinstance(
+                    variable.type, Pointer) else variable.type
+                return Identifier(self.location(node), t, context(node.ctx), variable)
+            except KeyError:
+                return None
+
+        else:
+            self.syntax_error(
+                node, f"Python syntax '{node.__class__.__name__}' is currently unsupported")
+
+    def visit_Name(self, node: ast.Name):
+        local = self.resolve_local(node)
+        return self.parse_constant(node, self.resolve_global(node)) if local is None else local
+
+    def visit_Attribute(self, node: ast.Attribute):
+        local = self.resolve_local(node)
+        return self.parse_constant(node, self.resolve_global(node)) if local is None else local
+
+    def visit_Subscript(self, node: ast.Subscript):
+        return self.resolve_local(node)
+
+    def visit_Call(self, node: ast.Call):
+        from xgrid.lang.operator import Operator
+
+        func_name = None
+        self_type = None
+
+        if isinstance(node.func, ast.Attribute) and (local_obj := self.resolve_local(node.func.value)) is not None:
+            if isinstance(local_obj.type, Structure):
+                func = getattr(
+                    local_obj.type.dataclass, node.func.attr, None)
+                func_name = f"{local_obj.type.dataclass.__qualname__}.{node.func.attr}"
+                self_type = local_obj.type
+            else:
+                # fixed method call, in the future ?
+                self.syntax_error(
+                    node, f"Invalid method call on type {local_obj.type}")
+
+            args: list[Expression] = [local_obj]
+        else:
+            func = self.resolve_global(node.func)
+            args = []
+
+        # specially handle cast expression
+        if func == cast:
+            if len(node.args) != 2:
+                self.syntax_error(
+                    node, f"Cast requires 2 arguments, got {len(node.args)}")
+            target_type = parse_annotation(self.resolve_global(node.args[0]))
+            if target_type is None:
+                self.syntax_error(node, f"Invalid cast type")
+            return Cast(self.location(node), target_type, self.visit(node.args[1]))
+
+        args.extend(self.visit(i) for i in node.args)
+
+        # specially handle type constructor
+        if isinstance(func, type):
+            internal_type = parse_annotation(func)
+            if internal_type is None or not isinstance(internal_type, Structure):
+                self.syntax_error(
+                    node, f"Invalid type constructor '{func.__name__}'")
+
+            func = Constructor(internal_type, Signature(
+                list(internal_type.elements), internal_type))
+            func_name = f"{internal_type.name}.constructor"
+
+        # type check the function and arguments
+        if not isinstance(func, Operator) and not isinstance(func, Constructor):
+            # check the lazy method flag
+            method_flag = getattr(func, "__xgrid_method", None)
+            if method_flag is not None and self_type is not None:
+                func = Operator(func, "function",
+                                method_flag[0], method_flag[1], self_type)
+            else:
+                self.syntax_error(
+                    node, f"Invalid call to object '{func}', it is not an operator")
+
+        if func_name is None:
+            func_name = func.name  # type: ignore
+
+        if (expected := len(func.signature.arguments)) != len(args):
+            self.syntax_error(
+                node, f"Operator '{func_name}' requires {expected} arguments, but got {len(args)}")
+
+        if isinstance(func, Operator) and func.mode == "external" and func.typecheck_override is not None:
+            try:
+                return_type = func.typecheck_override([i.type for i in args])
+            except Exception as e:
+                self.syntax_error(node, e.args[0])
+
+            if func.name in ("shape", "dimension"):
+                if not isinstance(args[0], Identifier):
+                    self.syntax_error(
+                        node, f"Incompatible '{func.name}' to argument '{args[0]}'")
+
+                return GridInfo(self.location(node), Integer(calcsize("i")), cast(Literal["shape", "dimension"], func.name), args[0].variable, args[1] if func.name == "shape" else None)
+        else:
+            for id, (arg_name, arg_type) in enumerate(func.signature.arguments):
+                if arg_type != args[id].type:
+                    self.syntax_error(
+                        node, f"Incompatible type '{args[id].type}' with '{arg_type}' of argument '{arg_name}, operator '{func_name}'")
+            return_type = func.signature.return_type
+
+        return Call(self.location(node), return_type, func, args)
```

### Comparing `xgrid-0.0.1/xgrid/lang/ir/__init__.py` & `xgrid-0.0.2/xgrid/lang/ir/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from dataclasses import dataclass
-from typing import Any
-
-from xgrid.util.console import ElementFormat, Elementable, idvar
-from xgrid.util.typing import BaseType
-
-
-@dataclass
-class Location:
-    file: str
-    func: str
-    line: int
-
-    def __repr__(self) -> str:
-        return f"File {self.file}, line {self.line}, at {self.func}"
-
-
-@dataclass
-class IR(Elementable):
-    location: Location
-
-
-@dataclass
-class Variable(Elementable):
-    name: str
-    type: BaseType
-
-    def write(self, format: ElementFormat):
-        format.print(idvar("%" + self.name))
+from dataclasses import dataclass
+from typing import Any
+
+from xgrid.util.console import ElementFormat, Elementable, idvar
+from xgrid.util.typing import BaseType
+
+
+@dataclass
+class Location:
+    file: str
+    func: str
+    line: int
+
+    def __repr__(self) -> str:
+        return f"File {self.file}, line {self.line}, at {self.func}"
+
+
+@dataclass
+class IR(Elementable):
+    location: Location
+
+
+@dataclass
+class Variable(Elementable):
+    name: str
+    type: BaseType
+
+    def write(self, format: ElementFormat):
+        format.print(idvar("%" + self.name))
```

### Comparing `xgrid-0.0.1/xgrid/lang/ir/expression.py` & `xgrid-0.0.2/xgrid/lang/ir/expression.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-from dataclasses import dataclass
-from enum import Enum
-from typing import Literal
-
-import xgrid.lang.operator as op
-from xgrid.lang.ir import IR, Variable
-from xgrid.util.console import ElementFormat, idconst, idfunc, idtype, kw, plain
-from xgrid.util.typing import BaseType
-from xgrid.util.typing.reference import Grid, Pointer
-from xgrid.util.typing.value import Structure
-
-
-@dataclass
-class Expression(IR):
-    type: BaseType
-
-    def write(self, format: ElementFormat):
-        pass
-
-
-class BinaryOperator(Enum):
-    Add = "+"
-    Sub = "-"
-    Mul = "*"
-    Div = "/"
-    Pow = "^"
-    Mod = "%"
-
-    Eq = "=="
-    Gt = ">"
-    Ge = ">="
-    Lt = "<"
-    Le = "<="
-    Neq = "!="
-
-    And = "&&"
-    Or = "||"
-
-    def is_compare(self) -> bool:
-        return self in (BinaryOperator.Eq, BinaryOperator.Gt, BinaryOperator.Ge, BinaryOperator.Lt, BinaryOperator.Le, BinaryOperator.Neq)
-
-    def is_logic(self) -> bool:
-        return self in (BinaryOperator.And, BinaryOperator.Or)
-
-
-class UnaryOperator(Enum):
-    Pos = "+"
-    Neg = "-"
-    Not = "!"
-
-
-@dataclass
-class Binary(Expression):
-    left: Expression
-    right: Expression
-    operator: BinaryOperator
-
-    def write(self, format: ElementFormat):
-        format.print(plain("("), self.left, plain(
-            self.operator.value), self.right, plain(")"))
-
-
-@dataclass
-class Unary(Expression):
-    right: Expression
-    operator: UnaryOperator
-
-    def write(self, format: ElementFormat):
-        format.print(
-            plain("("), plain(self.operator.value), self.right, plain(")"))
-
-
-@dataclass
-class Condition(Expression):
-    condition: Expression
-    body: Expression
-    orelse: Expression
-
-    def write(self, format: ElementFormat):
-        format.print(plain("("), self.condition, plain("?"),
-                     self.body, plain(":"), self.orelse, plain(")"))
-
-
-@dataclass
-class Constant(Expression):
-    value: int | float | bool
-
-    def write(self, format: ElementFormat):
-        format.print(idconst(repr(self.value)))
-
-
-@dataclass
-class Cast(Expression):
-    value: Expression
-
-    def write(self, format: ElementFormat):
-        format.print(self.value, plain("as"), idtype(repr(self.type)))
-
-
-@dataclass
-class Terminal(Expression):
-    context: Literal["load", "store"]
-
-
-@dataclass
-class Identifier(Terminal):
-    variable: Variable
-
-    def write(self, format: ElementFormat):
-        if isinstance(self.variable.type, Pointer):
-            format.print(kw("ref"))
-        format.print(self.variable)
-
-
-@dataclass
-class Stencil(Terminal):
-    variable: Variable
-    time_offset: int
-    space_offset: list[int]
-    boundary_mask: int = 0
-
-    def __post_init__(self):
-        assert isinstance(self.variable.type, Grid)
-
-    def write(self, format: ElementFormat):
-        offset = f"[{', '.join(map(str, self.space_offset))}][{self.time_offset}]"
-        format.print(self.variable, plain(offset))
-
-
-@dataclass
-class Access(Terminal):
-    value: Terminal
-    attribute: str
-
-    def write(self, format: ElementFormat):
-        format.print(self.value, plain(f".{self.attribute}"))
-
-
-@dataclass
-class Signature:
-    arguments: list[tuple[str, BaseType]]
-    return_type: BaseType
-
-    def __post_init__(self):
-        self.argnames_map = dict(self.arguments)
-
-
-@dataclass
-class Constructor(ElementFormat):
-    type: Structure
-    signature: Signature
-
-
-@dataclass
-class Call(Expression):
-    operator: "op.Operator | Constructor"
-    arguments: list[Expression]
-
-    def write(self, format: ElementFormat):
-        arglist = []
-        for arg in self.arguments:
-            arglist.append(arg)
-            arglist.append(plain(","))
-        if any(arglist):
-            arglist.pop()
-
-        if isinstance(self.operator, Constructor):
-            format.print(idtype(repr(self.operator.type)), plain(
-                "("), *arglist, plain(")"))
-        else:
-            format.print(idfunc(self.operator.name), plain(
-                "("), *arglist, plain(")"))
-
-
-@dataclass
-class GridInfo(Expression):
-    info: Literal["shape", "dimension"]
-    variable: Variable
-    dimension: Expression | None
-
-    def write(self, format: ElementFormat):
-        format.print(kw(self.info), plain("("), self.variable)
-        if self.dimension is not None:
-            format.print(self.dimension)
-        format.print(plain(")"))
+from dataclasses import dataclass
+from enum import Enum
+from typing import Literal
+
+import xgrid.lang.operator as op
+from xgrid.lang.ir import IR, Variable
+from xgrid.util.console import ElementFormat, idconst, idfunc, idtype, kw, plain
+from xgrid.util.typing import BaseType
+from xgrid.util.typing.reference import Grid, Pointer
+from xgrid.util.typing.value import Structure
+
+
+@dataclass
+class Expression(IR):
+    type: BaseType
+
+    def write(self, format: ElementFormat):
+        pass
+
+
+class BinaryOperator(Enum):
+    Add = "+"
+    Sub = "-"
+    Mul = "*"
+    Div = "/"
+    Pow = "^"
+    Mod = "%"
+
+    Eq = "=="
+    Gt = ">"
+    Ge = ">="
+    Lt = "<"
+    Le = "<="
+    Neq = "!="
+
+    And = "&&"
+    Or = "||"
+
+    def is_compare(self) -> bool:
+        return self in (BinaryOperator.Eq, BinaryOperator.Gt, BinaryOperator.Ge, BinaryOperator.Lt, BinaryOperator.Le, BinaryOperator.Neq)
+
+    def is_logic(self) -> bool:
+        return self in (BinaryOperator.And, BinaryOperator.Or)
+
+
+class UnaryOperator(Enum):
+    Pos = "+"
+    Neg = "-"
+    Not = "!"
+
+
+@dataclass
+class Binary(Expression):
+    left: Expression
+    right: Expression
+    operator: BinaryOperator
+
+    def write(self, format: ElementFormat):
+        format.print(plain("("), self.left, plain(
+            self.operator.value), self.right, plain(")"))
+
+
+@dataclass
+class Unary(Expression):
+    right: Expression
+    operator: UnaryOperator
+
+    def write(self, format: ElementFormat):
+        format.print(
+            plain("("), plain(self.operator.value), self.right, plain(")"))
+
+
+@dataclass
+class Condition(Expression):
+    condition: Expression
+    body: Expression
+    orelse: Expression
+
+    def write(self, format: ElementFormat):
+        format.print(plain("("), self.condition, plain("?"),
+                     self.body, plain(":"), self.orelse, plain(")"))
+
+
+@dataclass
+class Constant(Expression):
+    value: int | float | bool
+
+    def write(self, format: ElementFormat):
+        format.print(idconst(repr(self.value)))
+
+
+@dataclass
+class Cast(Expression):
+    value: Expression
+
+    def write(self, format: ElementFormat):
+        format.print(self.value, plain("as"), idtype(repr(self.type)))
+
+
+@dataclass
+class Terminal(Expression):
+    context: Literal["load", "store"]
+
+
+@dataclass
+class Identifier(Terminal):
+    variable: Variable
+
+    def write(self, format: ElementFormat):
+        if isinstance(self.variable.type, Pointer):
+            format.print(kw("ref"))
+        format.print(self.variable)
+
+
+@dataclass
+class Stencil(Terminal):
+    variable: Variable
+    time_offset: int
+    space_offset: list[int]
+    boundary_mask: int = 0
+
+    def __post_init__(self):
+        assert isinstance(self.variable.type, Grid)
+
+    def write(self, format: ElementFormat):
+        offset = f"[{', '.join(map(str, self.space_offset))}][{self.time_offset}]"
+        format.print(self.variable, plain(offset))
+
+
+@dataclass
+class Access(Terminal):
+    value: Terminal
+    attribute: str
+
+    def write(self, format: ElementFormat):
+        format.print(self.value, plain(f".{self.attribute}"))
+
+
+@dataclass
+class Signature:
+    arguments: list[tuple[str, BaseType]]
+    return_type: BaseType
+
+    def __post_init__(self):
+        self.argnames_map = dict(self.arguments)
+
+
+@dataclass
+class Constructor(ElementFormat):
+    type: Structure
+    signature: Signature
+
+
+@dataclass
+class Call(Expression):
+    operator: "op.Operator | Constructor"
+    arguments: list[Expression]
+
+    def write(self, format: ElementFormat):
+        arglist = []
+        for arg in self.arguments:
+            arglist.append(arg)
+            arglist.append(plain(","))
+        if any(arglist):
+            arglist.pop()
+
+        if isinstance(self.operator, Constructor):
+            format.print(idtype(repr(self.operator.type)), plain(
+                "("), *arglist, plain(")"))
+        else:
+            format.print(idfunc(self.operator.name), plain(
+                "("), *arglist, plain(")"))
+
+
+@dataclass
+class GridInfo(Expression):
+    info: Literal["shape", "dimension"]
+    variable: Variable
+    dimension: Expression | None
+
+    def write(self, format: ElementFormat):
+        format.print(kw(self.info), plain("("), self.variable)
+        if self.dimension is not None:
+            format.print(self.dimension)
+        format.print(plain(")"))
```

### Comparing `xgrid-0.0.1/xgrid/lang/ir/statement.py` & `xgrid-0.0.2/xgrid/lang/ir/statement.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from dataclasses import dataclass
-from sys import stdout
-from typing import TextIO
-
-from xgrid.lang.ir import IR, Variable
-from xgrid.lang.ir.expression import Expression, Signature, Terminal
-from xgrid.util.console import ElementFormat, idfunc, idtype, idvar, kw, plain
-
-
-@dataclass
-class Statement(IR):
-    def write(self, format: ElementFormat):
-        pass
-
-
-@dataclass
-class Definition(Statement):
-    name: str
-    mode: str
-    signature: Signature
-    scope: dict[str, Variable]
-    body: list[Statement]
-
-    def write(self, format: ElementFormat):
-        args = [plain("(")]
-        for name, type in self.signature.arguments:
-            args.extend((idtype(repr(type)), idvar("%"+name)))
-            args.append(plain(","))
-        if any(args):
-            args.pop()
-        args.append(plain(")"))
-        format.println(kw(self.mode), idtype(repr(self.signature.return_type)), idfunc(
-            self.name), *args, kw("requires"))
-        with format.indent():
-            for name, var in self.scope.items():
-                if name not in self.signature.argnames_map:
-                    format.println(var, plain(":"), idtype(repr(var.type)))
-        format.println(kw("begin"))
-        with format.indent():
-            format.print(*self.body)
-        format.println(kw("end"))
-
-    def show(self, *, indent_size: int = 2, device: TextIO = stdout):
-        format = ElementFormat()
-        self.write(format)
-        format.write(device)
-
-
-@dataclass
-class Return(Statement):
-    value: Expression | None
-
-    def write(self, format: ElementFormat):
-        format.println(kw("return"), plain(
-            "") if self.value is None else self.value)
-
-
-@dataclass
-class Break(Statement):
-    def write(self, format: ElementFormat):
-        format.println(kw("break"))
-
-
-@dataclass
-class Continue(Statement):
-    def write(self, format: ElementFormat):
-        format.println(kw("continue"))
-
-
-@dataclass
-class If(Statement):
-    condition: Expression
-    body: list[Statement]
-    orelse: list[Statement]
-
-    def write(self, format: ElementFormat):
-        format.println(kw("if"), self.condition, kw("do"))
-        with format.indent():
-            format.print(*self.body)
-        if any(self.orelse):
-            format.println(kw("else"))
-            with format.indent():
-                format.print(*self.orelse)
-        format.println(kw("end"))
-
-
-@dataclass
-class While(Statement):
-    condition: Expression
-    body: list[Statement]
-
-    def write(self, format: ElementFormat):
-        format.println(kw("while"), self.condition, kw("do"))
-        with format.indent():
-            format.print(*self.body)
-        format.println(kw("end"))
-
-
-@dataclass
-class Evaluation(Statement):
-    value: Expression
-
-    def write(self, format: ElementFormat):
-        format.println(kw("evaluate"), self.value)
-
-
-@dataclass
-class Assignment(Statement):
-    terminal: Terminal
-    value: Expression
-
-    def write(self, format: ElementFormat):
-        format.println(self.terminal, plain(":"), idtype(
-            repr(self.terminal.type)), plain("="), self.value)
-
-
-@dataclass
-class Inline(Statement):
-    source: str
-
-    def write(self, format: ElementFormat):
-        format.println(kw("inline"), kw("begin"))
-        with format.indent():
-            format.println(plain(self.source))
-        format.println(kw("end"))
-
-
-@dataclass
-class For(Statement):
-    variable: Variable
-    start: Expression
-    end: Expression
-    step: Expression
-    body: list[Statement]
-
-    def write(self, format: ElementFormat):
-        format.println(kw("for"), idvar("%" + self.variable.name), kw("in"),
-                       self.start, plain(":"), self.end, plain(":"), self.step)
-        with format.indent():
-            format.print(*self.body)
+from dataclasses import dataclass
+from sys import stdout
+from typing import TextIO
+
+from xgrid.lang.ir import IR, Variable
+from xgrid.lang.ir.expression import Expression, Signature, Terminal
+from xgrid.util.console import ElementFormat, idfunc, idtype, idvar, kw, plain
+
+
+@dataclass
+class Statement(IR):
+    def write(self, format: ElementFormat):
+        pass
+
+
+@dataclass
+class Definition(Statement):
+    name: str
+    mode: str
+    signature: Signature
+    scope: dict[str, Variable]
+    body: list[Statement]
+
+    def write(self, format: ElementFormat):
+        args = [plain("(")]
+        for name, type in self.signature.arguments:
+            args.extend((idtype(repr(type)), idvar("%"+name)))
+            args.append(plain(","))
+        if any(args):
+            args.pop()
+        args.append(plain(")"))
+        format.println(kw(self.mode), idtype(repr(self.signature.return_type)), idfunc(
+            self.name), *args, kw("requires"))
+        with format.indent():
+            for name, var in self.scope.items():
+                if name not in self.signature.argnames_map:
+                    format.println(var, plain(":"), idtype(repr(var.type)))
+        format.println(kw("begin"))
+        with format.indent():
+            format.print(*self.body)
+        format.println(kw("end"))
+
+    def show(self, *, indent_size: int = 2, device: TextIO = stdout):
+        format = ElementFormat()
+        self.write(format)
+        format.write(device)
+
+
+@dataclass
+class Return(Statement):
+    value: Expression | None
+
+    def write(self, format: ElementFormat):
+        format.println(kw("return"), plain(
+            "") if self.value is None else self.value)
+
+
+@dataclass
+class Break(Statement):
+    def write(self, format: ElementFormat):
+        format.println(kw("break"))
+
+
+@dataclass
+class Continue(Statement):
+    def write(self, format: ElementFormat):
+        format.println(kw("continue"))
+
+
+@dataclass
+class If(Statement):
+    condition: Expression
+    body: list[Statement]
+    orelse: list[Statement]
+
+    def write(self, format: ElementFormat):
+        format.println(kw("if"), self.condition, kw("do"))
+        with format.indent():
+            format.print(*self.body)
+        if any(self.orelse):
+            format.println(kw("else"))
+            with format.indent():
+                format.print(*self.orelse)
+        format.println(kw("end"))
+
+
+@dataclass
+class While(Statement):
+    condition: Expression
+    body: list[Statement]
+
+    def write(self, format: ElementFormat):
+        format.println(kw("while"), self.condition, kw("do"))
+        with format.indent():
+            format.print(*self.body)
+        format.println(kw("end"))
+
+
+@dataclass
+class Evaluation(Statement):
+    value: Expression
+
+    def write(self, format: ElementFormat):
+        format.println(kw("evaluate"), self.value)
+
+
+@dataclass
+class Assignment(Statement):
+    terminal: Terminal
+    value: Expression
+
+    def write(self, format: ElementFormat):
+        format.println(self.terminal, plain(":"), idtype(
+            repr(self.terminal.type)), plain("="), self.value)
+
+
+@dataclass
+class Inline(Statement):
+    source: str
+
+    def write(self, format: ElementFormat):
+        format.println(kw("inline"), kw("begin"))
+        with format.indent():
+            format.println(plain(self.source))
+        format.println(kw("end"))
+
+
+@dataclass
+class For(Statement):
+    variable: Variable
+    start: Expression
+    end: Expression
+    step: Expression
+    body: list[Statement]
+
+    def write(self, format: ElementFormat):
+        format.println(kw("for"), idvar("%" + self.variable.name), kw("in"),
+                       self.start, plain(":"), self.end, plain(":"), self.step)
+        with format.indent():
+            format.print(*self.body)
```

### Comparing `xgrid-0.0.1/xgrid/util/ffi.py` & `xgrid-0.0.2/xgrid/util/ffi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,94 @@
-import os
-import ctypes
-from hashlib import md5
-from shutil import which
-from subprocess import PIPE, Popen
-from typing import IO, Callable, Iterable, cast
-
-from xgrid.util.logging import Logger
-from xgrid.util.typing import BaseType, Void
-
-
-class Library:
-    def __init__(self, name: str) -> None:
-        self.logger = Logger(self)
-        self.dylib = ctypes.cdll.LoadLibrary(name)
-
-    def function(self, entry_point: str, argtypes: list[BaseType], restype: BaseType) -> Callable:
-        handler = getattr(self.dylib, entry_point)
-        if not handler:
-            self.logger.dead(f"failed to get function '{entry_point}")
-
-        for argt in argtypes:
-            if isinstance(argt, Void):
-                self.logger.dead("unexpected void type in arguments")
-
-        if not isinstance(restype, Void):
-            handler.restype = restype.ctype
-
-        def wrapper(*args):
-            if len(args) != len(argtypes):
-                raise TypeError(
-                    f"this function takes {len(argtypes)} argument ({len(args)} given)")
-            return restype.deserialize(handler(*map(lambda x: x[0](x[1]), zip(map(lambda x: x.serialize, argtypes), args))))
-        return wrapper
-
-
-class Compiler:
-    "compiler driver to perform compiling and linking to dynamic library"
-
-    def __init__(self, *, cacheroot: str, cc: Iterable[str]) -> None:
-        self.logger = Logger(self)
-
-        self.cacheroot = os.path.join(".", cacheroot)
-        if not os.path.exists(self.cacheroot):
-            os.makedirs(self.cacheroot)
-
-        def search_cc(seq: Iterable[str]) -> str:
-            for cc in seq:
-                which_cc = which(cc)
-                if which_cc:
-                    return which_cc
-            self.logger.dead(f"failed to locate cc in {seq}")
-        self.cc = search_cc(cc)
-
-        self.logger.info(
-            f"compiler initialized with cacheroot = '{self.cacheroot}', cc = '{self.cc}'")
-
-    def compile(self, source: str, cflags: Iterable[str] = []):
-        args = [self.cc, "-fpic", "-shared"]
-        args.extend(cflags)
-
-        source = f"// {' '.join(args)}\n" + source
-
-        name = os.path.join(self.cacheroot, md5(
-            source.encode()).hexdigest() + ".c")
-        libname = name + ".so"
-
-        cached = False
-
-        if os.path.exists(name):
-            with open(name, "r") as sf:
-                cached = sf.read() == source
-
-        if not cached:
-            with open(name, "w") as sf:
-                sf.write(source)
-
-            args.extend([name, "-o", libname])
-
-            process = Popen(args, stderr=PIPE)
-            if process.wait() != 0:
-                err_msg = cast(IO[bytes], process.stderr).read().decode()
-                self.logger.dead(
-                    f"failed to compile '{name}' due to:", err_msg)
-
-        self.logger.info(
-            f"jit compiled '{name}' {'with' if cached else 'without'} cache to '{libname}'")
-
-        return libname
+import os
+import ctypes
+from hashlib import md5
+from shutil import which
+from subprocess import PIPE, Popen
+import sys
+from typing import IO, Callable, Iterable, cast
+
+from xgrid.util.logging import Logger
+from xgrid.util.typing import BaseType, Void
+
+
+class Library:
+    def __init__(self, name: str) -> None:
+        self.logger = Logger(self)
+        self.dylib = ctypes.cdll.LoadLibrary(name)
+
+    def function(self, entry_point: str, argtypes: list[BaseType], restype: BaseType) -> Callable:
+        handler = getattr(self.dylib, entry_point)
+        if not handler:
+            self.logger.dead(f"failed to get function '{entry_point}")
+
+        for argt in argtypes:
+            if isinstance(argt, Void):
+                self.logger.dead("unexpected void type in arguments")
+
+        if not isinstance(restype, Void):
+            handler.restype = restype.ctype
+
+        def wrapper(*args):
+            if len(args) != len(argtypes):
+                raise TypeError(
+                    f"this function takes {len(argtypes)} argument ({len(args)} given)")
+            return restype.deserialize(handler(*map(lambda x: x[0](x[1]), zip(map(lambda x: x.serialize, argtypes), args))))
+        return wrapper
+
+
+class Compiler:
+    "compiler driver to perform compiling and linking to dynamic library"
+
+    def __init__(self, *, cacheroot: str, cc: Iterable[str]) -> None:
+        self.logger = Logger(self)
+
+        self.cacheroot = os.path.join(".", cacheroot)
+        if not os.path.exists(self.cacheroot):
+            os.makedirs(self.cacheroot)
+
+        def search_cc(seq: Iterable[str]) -> str:
+            for cc in seq:
+                which_cc = which(cc)
+                if which_cc:
+                    return which_cc
+            self.logger.dead(f"failed to locate cc in {seq}")
+        self.cc = search_cc(cc)
+
+        self.logger.info(
+            f"compiler initialized with cacheroot = '{self.cacheroot}', cc = '{self.cc}'")
+
+    def compile(self, source: str, cflags: Iterable[str] = []):
+        args = [self.cc, "-shared"]
+
+        if sys.platform != "win32":
+            args.append("-fpic")
+
+        args.extend(cflags)
+
+        source = f"// {' '.join(args)}\n" + source
+
+        name = os.path.join(self.cacheroot, md5(
+            source.encode()).hexdigest() + ".c")
+        libname = name + ".so"
+
+        cached = False
+
+        if os.path.exists(name):
+            with open(name, "r") as sf:
+                cached = sf.read() == source
+
+        if not cached:
+            with open(name, "w") as sf:
+                sf.write(source)
+
+            args.extend([name, "-o", libname])
+
+            process = Popen(args, stderr=PIPE)
+            if process.wait() != 0:
+                err_msg = cast(IO[bytes], process.stderr).read().decode()
+                self.logger.dead(
+                    f"failed to compile '{name}' due to:", err_msg)
+
+        self.logger.info(
+            f"jit compiled '{name}' {'with' if cached else 'without'} cache to '{libname}'")
+
+        return libname
```

### Comparing `xgrid-0.0.1/xgrid/util/init.py` & `xgrid-0.0.2/xgrid/util/init.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-from dataclasses import asdict, dataclass
-import sys
-from typing import Literal
-from xgrid.util.logging import Logger
-
-
-logger = Logger("xgrid")
-
-
-@dataclass
-class Configuration:
-    parallel: bool
-    cc: list[str]
-    cacheroot: str
-    comment: bool
-    overstep: Literal["none", "limit", "wrap"]
-    opt_level: Literal[0, 1, 2, 3]
-    precision: Literal["float", "double"]
-
-    def __repr__(self) -> str:
-        return repr(asdict(self))
-
-    @property
-    def cflags(self):
-        flags = []
-
-        if self.parallel:
-            flags.append("-fopenmp")
-
-        flags.append(f"-O{self.opt_level}")
-
-        flags.append(f"-lm")
-
-        return flags
-
-    @property
-    def fsize(self):
-        return 4 if self.precision == "float" else 8
-
-
-_config: Configuration | None = None
-
-
-def get_config() -> Configuration:
-    if _config is None:
-        logger.dead(f"Please call init first to initialize")
-    return _config
-
-
-def init(*, parallel: bool = True, cc: list[str] = ["gcc", "clang"], cacheroot: str = ".xgrid", comment: bool = False, overstep: Literal["none", "limit", "wrap"] = "none", opt_level: Literal[0, 1, 2, 3] = 2, precision: Literal["float", "double"] = "float") -> None:
-    global _config
-
-    if sys.version_info < (3, 10):
-        logger.fail(
-            f"Minimum Python 3.10 is required, current version is {sys.version_info}")
-
-    if sys.platform == "win32":
-        if not any(filter(shutil.which, cc)):
-            solutions = ["    1. LLVM (https://llvm.org/)",
-                         "    2. MinGW-w64 (https://www.mingw-w64.org/)",
-                         "    3. MSYS2 (https://www.msys2.org/)",
-                         "    4. Cygwin (https://www.cygwin.com/)"]
-            logger.fail(
-                f"Failed to find cc within {cc}, possible solutions are:", *solutions)
-
-    _config = Configuration(parallel, cc, cacheroot,
-                            comment, overstep, opt_level, precision)
-
-    logger.info(f"initialized with configuration: {_config}")
+from dataclasses import asdict, dataclass
+import sys
+from typing import Literal
+from xgrid.util.logging import Logger
+
+
+logger = Logger("xgrid")
+
+
+@dataclass
+class Configuration:
+    parallel: bool
+    cc: list[str]
+    cacheroot: str
+    comment: bool
+    overstep: Literal["none", "limit", "wrap"]
+    opt_level: Literal[0, 1, 2, 3]
+    precision: Literal["float", "double"]
+
+    def __repr__(self) -> str:
+        return repr(asdict(self))
+
+    @property
+    def cflags(self):
+        flags = []
+
+        if self.parallel:
+            flags.append("-fopenmp")
+
+        flags.append(f"-O{self.opt_level}")
+
+        flags.append(f"-lm")
+
+        return flags
+
+    @property
+    def fsize(self):
+        return 4 if self.precision == "float" else 8
+
+
+_config: Configuration | None = None
+
+
+def get_config() -> Configuration:
+    if _config is None:
+        logger.dead(f"Please call init first to initialize")
+    return _config
+
+
+def init(*, parallel: bool = True, cc: list[str] = ["gcc", "clang"], cacheroot: str = ".xgrid", comment: bool = False, overstep: Literal["none", "limit", "wrap"] = "none", opt_level: Literal[0, 1, 2, 3] = 2, precision: Literal["float", "double"] = "float") -> None:
+    global _config
+
+    if sys.version_info < (3, 10):
+        logger.fail(
+            f"Minimum Python 3.10 is required, current version is {sys.version_info}")
+
+    if sys.platform == "win32":
+        import shutil
+
+        if not any(filter(shutil.which, cc)):
+            solutions = ["    1. LLVM (https://llvm.org/)",
+                         "    2. MinGW-w64 (https://www.mingw-w64.org/)",
+                         "    3. MSYS2 (https://www.msys2.org/)",
+                         "    4. Cygwin (https://www.cygwin.com/)"]
+            logger.fail(
+                f"Failed to find cc within {cc}, possible solutions are:", *solutions)
+
+    _config = Configuration(parallel, cc, cacheroot,
+                            comment, overstep, opt_level, precision)
+
+    logger.info(f"initialized with configuration: {_config}")
```

### Comparing `xgrid-0.0.1/xgrid/util/logging.py` & `xgrid-0.0.2/xgrid/util/logging.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from enum import Enum
-from typing import NoReturn
-from xgrid.util.console import Console, Style, Foreground, stdout, stderr
-
-
-class LogLevel(Enum):
-    info = 0
-    done = 1
-    warn = 2
-    fail = 3
-    dead = 4
-
-    @property
-    def style(self) -> Style:
-        return [Style.bold, Style.bold, Style.bold, Style.bold, Style.bold][self.value]
-
-    @property
-    def foreground(self) -> Foreground:
-        return [Foreground.blue, Foreground.green, Foreground.yellow, Foreground.red, Foreground.purple][self.value]
-
-
-class Logger:
-    """basic logging system, supports colored prompt"""
-
-    stdouts: list[Console] = [stdout]
-    stderrs: list[Console] = [stderr]
-    level = LogLevel.info
-
-    def __init__(self, obj: object | str) -> None:
-        self.name = obj if isinstance(
-            obj, str) else f"{obj.__module__}.{obj.__class__.__qualname__}@{id(obj)}"
-
-    def log(self, level: LogLevel, *msg: str) -> None:
-        first_line = True
-        if level.value >= Logger.level.value:
-            targets = Logger.stdouts if level.value <= LogLevel.done.value else Logger.stderrs
-            for target in targets:
-                for line in msg:
-                    if first_line:
-                        target.print("[ ").print(level.name, level.style, level.foreground).println(
-                            f" | {self.name} ] {line}")
-                        first_line = False
-                    else:
-                        target.println(line)
-
-    def info(self, *msg: str) -> None:
-        self.log(LogLevel.info, *msg)
-
-    def done(self, *msg: str) -> None:
-        self.log(LogLevel.done, *msg)
-
-    def warn(self, *msg: str) -> None:
-        self.log(LogLevel.warn, *msg)
-
-    def fail(self, *msg: str) -> None:
-        self.log(LogLevel.fail, *msg)
-
-    def dead(self, *msg: str) -> NoReturn:
-        self.log(LogLevel.dead, *msg)
-        raise Exception(msg)
+from enum import Enum
+from typing import NoReturn
+from xgrid.util.console import Console, Style, Foreground, stdout, stderr
+
+
+class LogLevel(Enum):
+    info = 0
+    done = 1
+    warn = 2
+    fail = 3
+    dead = 4
+
+    @property
+    def style(self) -> Style:
+        return [Style.bold, Style.bold, Style.bold, Style.bold, Style.bold][self.value]
+
+    @property
+    def foreground(self) -> Foreground:
+        return [Foreground.blue, Foreground.green, Foreground.yellow, Foreground.red, Foreground.purple][self.value]
+
+
+class Logger:
+    """basic logging system, supports colored prompt"""
+
+    stdouts: list[Console] = [stdout]
+    stderrs: list[Console] = [stderr]
+    level = LogLevel.info
+
+    def __init__(self, obj: object | str) -> None:
+        self.name = obj if isinstance(
+            obj, str) else f"{obj.__module__}.{obj.__class__.__qualname__}@{id(obj)}"
+
+    def log(self, level: LogLevel, *msg: str) -> None:
+        first_line = True
+        if level.value >= Logger.level.value:
+            targets = Logger.stdouts if level.value <= LogLevel.done.value else Logger.stderrs
+            for target in targets:
+                for line in msg:
+                    if first_line:
+                        target.print("[ ").print(level.name, level.style, level.foreground).println(
+                            f" | {self.name} ] {line}")
+                        first_line = False
+                    else:
+                        target.println(line)
+
+    def info(self, *msg: str) -> None:
+        self.log(LogLevel.info, *msg)
+
+    def done(self, *msg: str) -> None:
+        self.log(LogLevel.done, *msg)
+
+    def warn(self, *msg: str) -> None:
+        self.log(LogLevel.warn, *msg)
+
+    def fail(self, *msg: str) -> None:
+        self.log(LogLevel.fail, *msg)
+
+    def dead(self, *msg: str) -> NoReturn:
+        self.log(LogLevel.dead, *msg)
+        raise Exception(msg)
```

### Comparing `xgrid-0.0.1/xgrid/util/typing/annotation.py` & `xgrid-0.0.2/xgrid/util/typing/annotation.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from dataclasses import fields, is_dataclass
-import struct
-from typing import Any, Generic, TypeVar, get_args, get_origin
-from xgrid.util.init import get_config
-
-from xgrid.util.typing import BaseType, Ignore, Void
-import xgrid.util.typing.value as val
-import xgrid.util.typing.reference as ref
-
-
-Length = TypeVar("Length")
-
-
-Value = TypeVar("Value")
-
-
-class Annotation:
-    ...
-
-
-class ptr(Annotation, Generic[Value]):
-    def addr(self) -> int: ...
-
-
-class grid(Annotation, Generic[Value, Length]):
-    def __getitem__(self, key) -> Any: ...
-
-    def __setitem__(self, key, value) -> Any: ...
-
-
-def parse_annotation(annotation, glbs=globals()) -> BaseType | None:
-    if annotation is None:
-        return Void()
-
-    if type(annotation) == str:
-        annotation = glbs[annotation]
-
-    if annotation is Any:
-        return Ignore()
-
-    if annotation in (int, float, bool):
-        return {int: val.Integer(struct.calcsize("i")), float: val.Floating(get_config().fsize), bool: val.Boolean()}[annotation]
-
-    if is_dataclass(annotation) and isinstance(annotation, type):
-        elements = []
-        for field in fields(annotation):
-            t = parse_annotation(field.type)
-            if not isinstance(t, val.Value):
-                return None
-            elements.append((field.name, t))
-        return val.Structure(annotation, annotation.__name__, tuple(elements))
-
-    org, arg = get_origin(annotation), get_args(annotation)
-
-    if len(arg) not in (1, 2) or org is None:
-        return None
-
-    val_type = parse_annotation(arg[0])
-    if not isinstance(val_type, val.Value):
-        return None
-
-    if org == ptr and len(arg) == 1:
-        return ref.Pointer(val_type)
-
-    if org == grid and len(arg) == 2 and type(arg[1]) == int:
-        return ref.Grid(val_type, arg[1])
-
-    return None
+from dataclasses import fields, is_dataclass
+import struct
+from typing import Any, Generic, TypeVar, get_args, get_origin
+from xgrid.util.init import get_config
+
+from xgrid.util.typing import BaseType, Ignore, Void
+import xgrid.util.typing.value as val
+import xgrid.util.typing.reference as ref
+
+
+Length = TypeVar("Length")
+
+
+Value = TypeVar("Value")
+
+
+class Annotation:
+    ...
+
+
+class ptr(Annotation, Generic[Value]):
+    def addr(self) -> int: ...
+
+
+class grid(Annotation, Generic[Value, Length]):
+    def __getitem__(self, key) -> Any: ...
+
+    def __setitem__(self, key, value) -> Any: ...
+
+
+def parse_annotation(annotation, glbs=globals()) -> BaseType | None:
+    if annotation is None:
+        return Void()
+
+    if type(annotation) == str:
+        annotation = glbs[annotation]
+
+    if annotation is Any:
+        return Ignore()
+
+    if annotation in (int, float, bool):
+        return {int: val.Integer(struct.calcsize("i")), float: val.Floating(get_config().fsize), bool: val.Boolean()}[annotation]
+
+    if is_dataclass(annotation) and isinstance(annotation, type):
+        elements = []
+        for field in fields(annotation):
+            t = parse_annotation(field.type)
+            if not isinstance(t, val.Value):
+                return None
+            elements.append((field.name, t))
+        return val.Structure(annotation, annotation.__name__, tuple(elements))
+
+    org, arg = get_origin(annotation), get_args(annotation)
+
+    if len(arg) not in (1, 2) or org is None:
+        return None
+
+    val_type = parse_annotation(arg[0])
+    if not isinstance(val_type, val.Value):
+        return None
+
+    if org == ptr and len(arg) == 1:
+        return ref.Pointer(val_type)
+
+    if org == grid and len(arg) == 2 and type(arg[1]) == int:
+        return ref.Grid(val_type, arg[1])
+
+    return None
```

### Comparing `xgrid-0.0.1/xgrid/util/typing/value.py` & `xgrid-0.0.2/xgrid/util/typing/value.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import ctypes
-from dataclasses import astuple, dataclass
-from xgrid.util.typing import BaseType
-
-
-@dataclass
-class Value(BaseType):
-    @property
-    def abbr(self) -> str:
-        return ""
-
-
-@dataclass
-class Boolean(Value):
-    @property
-    def ctype(self):
-        return ctypes.c_bool
-
-    def serialize(self, value):
-        return ctypes.c_bool(value)
-
-    def __repr__(self) -> str:
-        return "Boolean"
-    
-    @property
-    def abbr(self) -> str:
-        return "b"
-
-
-@dataclass
-class Number(Value):
-    width_bytes: int
-
-    @property
-    def width_bits(self) -> int:
-        return self.width_bytes * 8
-
-
-@dataclass
-class Integer(Number):
-    __concrete_typing__ = True
-
-    def __post_init__(self):
-        assert self.width_bytes in (1, 2, 4, 8)
-        self._ctype = {1: ctypes.c_int8, 2: ctypes.c_int16,
-                       4: ctypes.c_int32, 8: ctypes.c_int64}[self.width_bytes]
-
-    @property
-    def ctype(self):
-        return self._ctype
-
-    def serialize(self, value):
-        return self._ctype(value)
-
-    def __repr__(self) -> str:
-        return f"Integer({self.width_bits})"
-    
-    @property
-    def abbr(self) -> str:
-        return f"i{self.width_bits}"
-
-
-@dataclass
-class Floating(Number):
-    __concrete_typing__ = True
-
-    def __post_init__(self):
-        assert self.width_bytes in (4, 8)
-        self._ctype = ctypes.c_float if self.width_bytes == 4 else ctypes.c_double
-
-    @property
-    def ctype(self):
-        return self._ctype
-
-    def serialize(self, value):
-        return self._ctype(value)
-
-    def __repr__(self) -> str:
-        return f"Floating({self.width_bits})"
-    
-    @property
-    def abbr(self) -> str:
-        return f"f{self.width_bits}"
-
-
-@dataclass
-class Structure(Value):
-    __concrete_typing__ = True
-
-    dataclass: type
-    name: str
-    elements: tuple[tuple[str, Value], ...]
-
-    def __post_init__(self):
-        self.elements_map = dict(self.elements)
-        self._ctype = type(f"st{self.name}",
-                           (ctypes.Structure,), {"_fields_": [(x[0], x[1].ctype) for x in self.elements]})
-
-    @property
-    def ctype(self):
-        return self._ctype
-
-    def serialize(self, value):
-        return self._ctype(*astuple(value))
-
-    def deserialize(self, value):
-        return self.dataclass(*[getattr(value, attr_tuple[0]) for attr_tuple in self.elements])
-
-    def __repr__(self) -> str:
-        return self.name
-
-    @property
-    def abbr(self) -> str:
+import ctypes
+from dataclasses import astuple, dataclass
+from xgrid.util.typing import BaseType
+
+
+@dataclass
+class Value(BaseType):
+    @property
+    def abbr(self) -> str:
+        return ""
+
+
+@dataclass
+class Boolean(Value):
+    @property
+    def ctype(self):
+        return ctypes.c_bool
+
+    def serialize(self, value):
+        return ctypes.c_bool(value)
+
+    def __repr__(self) -> str:
+        return "Boolean"
+    
+    @property
+    def abbr(self) -> str:
+        return "b"
+
+
+@dataclass
+class Number(Value):
+    width_bytes: int
+
+    @property
+    def width_bits(self) -> int:
+        return self.width_bytes * 8
+
+
+@dataclass
+class Integer(Number):
+    __concrete_typing__ = True
+
+    def __post_init__(self):
+        assert self.width_bytes in (1, 2, 4, 8)
+        self._ctype = {1: ctypes.c_int8, 2: ctypes.c_int16,
+                       4: ctypes.c_int32, 8: ctypes.c_int64}[self.width_bytes]
+
+    @property
+    def ctype(self):
+        return self._ctype
+
+    def serialize(self, value):
+        return self._ctype(value)
+
+    def __repr__(self) -> str:
+        return f"Integer({self.width_bits})"
+    
+    @property
+    def abbr(self) -> str:
+        return f"i{self.width_bits}"
+
+
+@dataclass
+class Floating(Number):
+    __concrete_typing__ = True
+
+    def __post_init__(self):
+        assert self.width_bytes in (4, 8)
+        self._ctype = ctypes.c_float if self.width_bytes == 4 else ctypes.c_double
+
+    @property
+    def ctype(self):
+        return self._ctype
+
+    def serialize(self, value):
+        return self._ctype(value)
+
+    def __repr__(self) -> str:
+        return f"Floating({self.width_bits})"
+    
+    @property
+    def abbr(self) -> str:
+        return f"f{self.width_bits}"
+
+
+@dataclass
+class Structure(Value):
+    __concrete_typing__ = True
+
+    dataclass: type
+    name: str
+    elements: tuple[tuple[str, Value], ...]
+
+    def __post_init__(self):
+        self.elements_map = dict(self.elements)
+        self._ctype = type(f"st{self.name}",
+                           (ctypes.Structure,), {"_fields_": [(x[0], x[1].ctype) for x in self.elements]})
+
+    @property
+    def ctype(self):
+        return self._ctype
+
+    def serialize(self, value):
+        return self._ctype(*astuple(value))
+
+    def deserialize(self, value):
+        return self.dataclass(*[getattr(value, attr_tuple[0]) for attr_tuple in self.elements])
+
+    def __repr__(self) -> str:
+        return self.name
+
+    @property
+    def abbr(self) -> str:
         return f"st{self.name}"
```

### Comparing `xgrid-0.0.1/xgrid/xgrid/__init__.py` & `xgrid-0.0.2/xgrid/xgrid/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import numpy as np
-from xgrid.util.logging import Logger
-from xgrid.util.typing.annotation import parse_annotation
-from xgrid.util.typing.value import Boolean, Floating, Integer, Structure, Value
-import xgrid.util.typing.reference as ref
-
-from ctypes import c_int32, POINTER
-
-
-def parse_numpy_dtype(dtype: Value):
-    if isinstance(dtype, Boolean):
-        return np.bool_
-    elif isinstance(dtype, Integer):
-        return {8: np.int8, 16: np.int16, 32: np.int32, 64: np.int64}[dtype.width_bits]
-    elif isinstance(dtype, Floating):
-        return {32: np.float32, 64: np.float64}[dtype.width_bits]
-    elif isinstance(dtype, Structure):
-        return [(x[0], parse_numpy_dtype(x[1])) for x in dtype.elements]
-
-
-class Grid:
-    def __init__(self, shape: tuple[int, ...], dtype: type) -> None:
-        self.logger = Logger(self)
-
-        dtype_parsed = parse_annotation(dtype)
-        if not isinstance(dtype_parsed, Value):
-            self.logger.dead(
-                f"Grid element should be value instead of '{dtype_parsed}'")
-        self.numpy_dtype = parse_numpy_dtype(dtype_parsed)
-
-        # properties
-        self.element = dtype_parsed
-        self.shape = shape
-
-        # internal typing used for serialization
-        self.typing = ref.Grid(self.element, self.dimension)
-
-        self._data = [np.zeros(shape=shape, dtype=self.numpy_dtype)]
-
-        # boundary condition
-        self.boundary = np.zeros(shape=shape, dtype=np.int32)
-
-    def _extend_time(self, depth: int):
-        while len(self._data) < depth:
-            self._data.append(
-                np.zeros(shape=self.shape, dtype=self.numpy_dtype))
-        self._data = self._data[:depth]
-
-    def _op_invoke(self, depth: int, tick: bool):
-        self._extend_time(depth)
-
-        if tick:
-            last = self._data.pop()
-            self._data.insert(0, last)
-
-    @property
-    def dimension(self):
-        return len(self.shape)
-
-    def serialize(self):
-        boundary_mask = self.boundary.ctypes.data_as(POINTER(c_int32))
-        data = (POINTER(self.element.ctype) * len(self._data))(*
-                                                               [data.ctypes.data_as(POINTER(self.element.ctype)) for data in self._data])
-
-        return self.typing.ctype(len(self._data),
-                                 (c_int32 * self.dimension)(*self.shape),
-                                 data,
-                                 boundary_mask)
-
-    @property
-    def now(self):
-        return self._data[0]
-
-    def fill(self, data: np.ndarray, time: int = 0):
-        if data.shape != self.now.shape or data.dtype != self.now.dtype:
-            self.logger.dead(
-                f"Unable to fill grid with incompatible shape or data type")
-
-        self._extend_time(abs(time))
-        self._data[time] = data.copy()
-
-    def __getitem__(self, slice):
-        return self.now[slice]
-
-    def __setitem__(self, slice, value):
-        self.now[slice] = value
+import numpy as np
+from xgrid.util.logging import Logger
+from xgrid.util.typing.annotation import parse_annotation
+from xgrid.util.typing.value import Boolean, Floating, Integer, Structure, Value
+import xgrid.util.typing.reference as ref
+
+from ctypes import c_int32, POINTER
+
+
+def parse_numpy_dtype(dtype: Value):
+    if isinstance(dtype, Boolean):
+        return np.bool_
+    elif isinstance(dtype, Integer):
+        return {8: np.int8, 16: np.int16, 32: np.int32, 64: np.int64}[dtype.width_bits]
+    elif isinstance(dtype, Floating):
+        return {32: np.float32, 64: np.float64}[dtype.width_bits]
+    elif isinstance(dtype, Structure):
+        return [(x[0], parse_numpy_dtype(x[1])) for x in dtype.elements]
+
+
+class Grid:
+    def __init__(self, shape: tuple[int, ...], dtype: type) -> None:
+        self.logger = Logger(self)
+
+        dtype_parsed = parse_annotation(dtype)
+        if not isinstance(dtype_parsed, Value):
+            self.logger.dead(
+                f"Grid element should be value instead of '{dtype_parsed}'")
+        self.numpy_dtype = parse_numpy_dtype(dtype_parsed)
+
+        # properties
+        self.element = dtype_parsed
+        self.shape = shape
+
+        # internal typing used for serialization
+        self.typing = ref.Grid(self.element, self.dimension)
+
+        self._data = [np.zeros(shape=shape, dtype=self.numpy_dtype)]
+
+        # boundary condition
+        self.boundary = np.zeros(shape=shape, dtype=np.int32)
+
+    def _extend_time(self, depth: int):
+        while len(self._data) < depth:
+            self._data.append(
+                np.zeros(shape=self.shape, dtype=self.numpy_dtype))
+        self._data = self._data[:depth]
+
+    def _op_invoke(self, depth: int, tick: bool):
+        self._extend_time(depth)
+
+        if tick:
+            last = self._data.pop()
+            self._data.insert(0, last)
+
+    @property
+    def dimension(self):
+        return len(self.shape)
+
+    def serialize(self):
+        boundary_mask = self.boundary.ctypes.data_as(POINTER(c_int32))
+        data = (POINTER(self.element.ctype) * len(self._data))(*
+                                                               [data.ctypes.data_as(POINTER(self.element.ctype)) for data in self._data])
+
+        return self.typing.ctype(len(self._data),
+                                 (c_int32 * self.dimension)(*self.shape),
+                                 data,
+                                 boundary_mask)
+
+    @property
+    def now(self):
+        return self._data[0]
+
+    def fill(self, data: np.ndarray, time: int = 0):
+        if data.shape != self.now.shape or data.dtype != self.now.dtype:
+            self.logger.dead(
+                f"Unable to fill grid with incompatible shape or data type")
+
+        self._extend_time(abs(time))
+        self._data[time] = data.copy()
+
+    def __getitem__(self, slice):
+        return self.now[slice]
+
+    def __setitem__(self, slice, value):
+        self.now[slice] = value
```

### Comparing `xgrid-0.0.1/PKG-INFO` & `xgrid-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgrid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Domain-specific language for developing partial differential equation solvers
 Project-URL: Homepage, https://github.com/yhl1219/xgrid
 Project-URL: Bug Tracker, https://github.com/yhl1219/xgrid/issues
 Author-email: yhl1219 <yhliu2000@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -72,8 +72,8 @@
 assert np.sum(result.now) == np.dot(a.now, b.now)
 ```
 
 ## Examples
 
 Solve the 2D Cavity flow with `xgrid`, see in examples folder.
 
-![cavity](./imgs/cavity.png)
+![cavity](https://github.com/yhl1219/xgrid/blob/main/imgs/cavity.png)
```

