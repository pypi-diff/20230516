# Comparing `tmp/cashocs-2.0.0b0.tar.gz` & `tmp/cashocs-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashocs-2.0.0b0.tar", last modified: Wed Apr 19 07:32:32 2023, max compression
+gzip compressed data, was "cashocs-2.0.0rc0.tar", last modified: Tue May 16 08:07:41 2023, max compression
```

## Comparing `cashocs-2.0.0b0.tar` & `cashocs-2.0.0rc0.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.222852 cashocs-2.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-04-19 07:32:32.222852 cashocs-2.0.0b0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    10400 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.206852 cashocs-2.0.0b0/cashocs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4552 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.206852 cashocs-2.0.0b0/cashocs/_cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_cli/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.206852 cashocs-2.0.0b0/cashocs/_constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26020 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_constraints/constrained_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_constraints/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.206852 cashocs-2.0.0b0/cashocs/_database/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_database/form_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_database/function_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_database/geometry_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_database/parameter_database.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.206852 cashocs-2.0.0b0/cashocs/_forms/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_forms/control_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_forms/form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_forms/general_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_forms/shape_form_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_forms/shape_regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/cost_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_optimization/line_search/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/line_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/line_search/armijo_line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/line_search/line_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/line_search/polynomial_line_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_optimization/optimal_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimal_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimal_control/box_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimal_control/control_variable_abstractions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21003 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimal_control/optimal_control_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/gradient_descent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/l_bfgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/ncg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28611 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/optimization_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23189 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_optimization/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_pde_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/adjoint_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4260 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/control_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/hessian_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/pde_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9443 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/shape_gradient_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_pde_problems/state_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.210852 cashocs-2.0.0b0/cashocs/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_utils/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_utils/interpolations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/_utils/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/cashocs/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/boundary_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/deformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    25763 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/mesh_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/mesh_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/geometry/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/cashocs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/io/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/io/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/io/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/io/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/cashocs/nonlinear_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/nonlinear_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/nonlinear_solvers/linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/nonlinear_solvers/newton_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/nonlinear_solvers/picard_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/cashocs/space_mapping/
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/space_mapping/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/space_mapping/optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/cashocs/space_mapping/shape_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.206852 cashocs-2.0.0b0/cashocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-04-19 07:32:32.000000 cashocs-2.0.0b0/cashocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-19 07:32:32.000000 cashocs-2.0.0b0/cashocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:32:32.000000 cashocs-2.0.0b0/cashocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 07:32:32.000000 cashocs-2.0.0b0/cashocs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-19 07:32:32.000000 cashocs-2.0.0b0/cashocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 07:32:32.000000 cashocs-2.0.0b0/cashocs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/documented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/documented/cashocs_as_solver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/cashocs_as_solver/control_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/cashocs_as_solver/shape_solver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/documented/misc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/misc/xdmf_io/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/misc/xdmf_io/demo_xdmf_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/documented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/box_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5441 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/constraints/demo_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/control_boundary_conditions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/dirichlet_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8197 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/heat_equation/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/iterative_solvers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7527 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/monolithic_problems/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6405 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/multiple_variables/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8034 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.214852 cashocs-2.0.0b0/demos/documented/optimal_control/neumann_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/nonlinear_pdes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/picard_iteration/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11379 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/poisson/demo_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/pre_post_callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/scalar_control_tracking/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/sparse_control/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/state_constraints/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6600 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/optimal_control/stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/optimal_control/stokes/demo_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/documented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/custom_scalar_product/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/eikonal_stiffness/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5712 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/inverse_tomography/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/p_laplacian/
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/regularization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5398 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/regularization/demo_regularization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/remeshing/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9439 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/remeshing/demo_remeshing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/scaling/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/scaling/demo_scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/shape_poisson/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/shape_stokes/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/test_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/undocumented/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/undocumented/optimal_control/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/undocumented/optimal_control/different_state_adjoint_spaces/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/demos/undocumented/shape_optimization/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/undocumented/shape_optimization/custom_functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/demos/undocumented/shape_optimization/pipe_optimization/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.202852 cashocs-2.0.0b0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.218852 cashocs-2.0.0b0/docs/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4739 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/docs/source/jupytext_process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3179 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:32:32.222852 cashocs-2.0.0b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:32:32.222852 cashocs-2.0.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_control_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_log_level.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_nonlinear_solvers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_optimal_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_optimal_control_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_optimal_control_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_p_laplacian.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_pde_problems.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_picard_iterations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_remeshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_shape_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40063 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_shape_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_shape_optimization_space_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_topology_optimization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-04-19 07:32:23.000000 cashocs-2.0.0b0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.583758 cashocs-2.0.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-05-16 08:07:41.583758 cashocs-2.0.0rc0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10425 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/cashocs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4550 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.559757 cashocs-2.0.0rc0/cashocs/_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11080 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_cli/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.559757 cashocs-2.0.0rc0/cashocs/_constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_constraints/constrained_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_constraints/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.559757 cashocs-2.0.0rc0/cashocs/_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_database/form_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_database/function_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_database/geometry_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_database/parameter_database.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5287 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.559757 cashocs-2.0.0rc0/cashocs/_forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_forms/control_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_forms/form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_forms/general_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_forms/shape_form_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22652 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_forms/shape_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.563758 cashocs-2.0.0rc0/cashocs/_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/cost_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.563758 cashocs-2.0.0rc0/cashocs/_optimization/line_search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/line_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/line_search/armijo_line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/line_search/line_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/line_search/polynomial_line_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.563758 cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/box_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/control_variable_abstractions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21515 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/optimal_control_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.563758 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/gradient_descent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13523 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/l_bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/ncg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29701 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/optimization_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.563758 cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24150 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/shape_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.567758 cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18603 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/topology_optimization_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_optimization/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.567758 cashocs-2.0.0rc0/cashocs/_pde_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/adjoint_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4272 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/control_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17636 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/hessian_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/pde_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9445 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/shape_gradient_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7315 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_pde_problems/state_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.567758 cashocs-2.0.0rc0/cashocs/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_utils/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_utils/interpolations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/_utils/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.567758 cashocs-2.0.0rc0/cashocs/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/boundary_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/deformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26872 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/mesh_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/mesh_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/geometry/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/cashocs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31284 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/io/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/io/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/io/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/cashocs/nonlinear_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/nonlinear_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/nonlinear_solvers/linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/nonlinear_solvers/newton_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/nonlinear_solvers/picard_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/cashocs/space_mapping/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/space_mapping/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36090 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/space_mapping/optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37353 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/cashocs/space_mapping/shape_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.559757 cashocs-2.0.0rc0/cashocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-05-16 08:07:41.000000 cashocs-2.0.0rc0/cashocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-16 08:07:41.000000 cashocs-2.0.0rc0/cashocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:07:41.000000 cashocs-2.0.0rc0/cashocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 08:07:41.000000 cashocs-2.0.0rc0/cashocs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 08:07:41.000000 cashocs-2.0.0rc0/cashocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 08:07:41.000000 cashocs-2.0.0rc0/cashocs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/demos/documented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.551757 cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/control_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7337 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/shape_solver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7422 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.551757 cashocs-2.0.0rc0/demos/documented/misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/misc/xdmf_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/misc/xdmf_io/demo_xdmf_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/demos/documented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/optimal_control/box_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5441 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/box_constraints/demo_box_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/optimal_control/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/constraints/demo_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/optimal_control/control_boundary_conditions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4275 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/optimal_control/dirichlet_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8197 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/optimal_control/heat_equation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/heat_equation/demo_heat_equation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.571758 cashocs-2.0.0rc0/demos/documented/optimal_control/iterative_solvers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7527 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/monolithic_problems/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6405 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/multiple_variables/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8034 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/neumann_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5100 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/neumann_control/demo_neumann_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/nonlinear_pdes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4503 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/picard_iteration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11379 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/poisson/demo_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/pre_post_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/scalar_control_tracking/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4956 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/sparse_control/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/sparse_control/demo_sparse_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/state_constraints/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6600 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/state_constraints/demo_state_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/optimal_control/stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7851 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/optimal_control/stokes/demo_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/demos/documented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/custom_scalar_product/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/eikonal_stiffness/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5712 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/inverse_tomography/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13339 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/p_laplacian/
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/regularization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5398 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/regularization/demo_regularization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/remeshing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9439 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/remeshing/demo_remeshing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/scaling/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/scaling/demo_scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/shape_poisson/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/shape_stokes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10178 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/space_mapping_semilinear_transmission/
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.575758 cashocs-2.0.0rc0/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/test_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/demos/undocumented/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/demos/undocumented/optimal_control/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.579758 cashocs-2.0.0rc0/demos/undocumented/optimal_control/different_state_adjoint_spaces/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.579758 cashocs-2.0.0rc0/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2535 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/demos/undocumented/shape_optimization/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.579758 cashocs-2.0.0rc0/demos/undocumented/shape_optimization/custom_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/undocumented/shape_optimization/custom_functional/custom_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.579758 cashocs-2.0.0rc0/demos/undocumented/shape_optimization/pipe_optimization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.555757 cashocs-2.0.0rc0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.579758 cashocs-2.0.0rc0/docs/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4751 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/docs/source/jupytext_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3179 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:07:41.583758 cashocs-2.0.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:07:41.583758 cashocs-2.0.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7691 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_control_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19518 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2945 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_log_level.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_nonlinear_solvers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25328 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_optimal_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6571 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_optimal_control_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_optimal_control_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_p_laplacian.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3343 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_pde_problems.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_picard_iterations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7247 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_remeshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_shape_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40742 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_shape_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13604 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_shape_optimization_space_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_topology_optimization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8955 2023-05-16 08:07:30.000000 cashocs-2.0.0rc0/tests/test_utils.py
```

### Comparing `cashocs-2.0.0b0/COPYING` & `cashocs-2.0.0rc0/COPYING`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/PKG-INFO` & `cashocs-2.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.0b0
+Version: 2.0.0rc0
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
 Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
@@ -327,14 +327,14 @@
 
 
 .. readme_start_about
 
 Contact / About
 ===============
 
-I'm `Sebastian Blauth <https://www.itwm.fraunhofer.de/en/departments/tv/staff/sebastian-blauth.html>`_, a scientific employee at `Fraunhofer ITWM
+I'm `Sebastian Blauth <https://sblauth.github.io/>`_, a scientific employee at `Fraunhofer ITWM
 <https://www.itwm.fraunhofer.de/en.html>`_. I have developed this project as part of my PhD thesis.
 If you have any questions / suggestions / feedback, etc., you can contact me
 via `sebastian.blauth@itwm.fraunhofer.de
-<mailto:sebastian.blauth@itwm.fraunhofer.de>`_.
+<mailto:sebastian.blauth@itwm.fraunhofer.de>`_. For more information, visit my website at `<https://sblauth.github.io/>`_.
 
 .. readme_end_about
```

### Comparing `cashocs-2.0.0b0/README.rst` & `cashocs-2.0.0rc0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -292,14 +292,14 @@
 
 
 .. readme_start_about
 
 Contact / About
 ===============
 
-I'm `Sebastian Blauth <https://www.itwm.fraunhofer.de/en/departments/tv/staff/sebastian-blauth.html>`_, a scientific employee at `Fraunhofer ITWM
+I'm `Sebastian Blauth <https://sblauth.github.io/>`_, a scientific employee at `Fraunhofer ITWM
 <https://www.itwm.fraunhofer.de/en.html>`_. I have developed this project as part of my PhD thesis.
 If you have any questions / suggestions / feedback, etc., you can contact me
 via `sebastian.blauth@itwm.fraunhofer.de
-<mailto:sebastian.blauth@itwm.fraunhofer.de>`_.
+<mailto:sebastian.blauth@itwm.fraunhofer.de>`_. For more information, visit my website at `<https://sblauth.github.io/>`_.
 
 .. readme_end_about
```

### Comparing `cashocs-2.0.0b0/cashocs/__init__.py` & `cashocs-2.0.0rc0/cashocs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from cashocs.io import convert
 from cashocs.io import import_mesh
 from cashocs.io import load_config
 from cashocs.nonlinear_solvers import linear_solve
 from cashocs.nonlinear_solvers import newton_solve
 from cashocs.nonlinear_solvers import picard_iteration
 
-__version__ = "2.0.0-beta0"
+__version__ = "2.0.0-rc0"
 
 __citation__ = """
 @Article{Blauth2021cashocs,
     author   = {Sebastian Blauth},
     journal  = {SoftwareX},
     title    = {{cashocs: A Computational, Adjoint-Based Shape Optimization and
         Optimal Control Software}},
```

### Comparing `cashocs-2.0.0b0/cashocs/_cli/__init__.py` & `cashocs-2.0.0rc0/cashocs/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_cli/_convert.py` & `cashocs-2.0.0rc0/cashocs/_cli/_convert.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_constraints/__init__.py` & `cashocs-2.0.0rc0/cashocs/_constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_constraints/constrained_problems.py` & `cashocs-2.0.0rc0/cashocs/_constraints/constrained_problems.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,15 +341,15 @@
         super().__init__(
             state_forms,
             bcs_list,
             cost_functional_form,
             states,
             adjoints,
             constraint_list,
-            config,
+            config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
             preconditioner_forms=preconditioner_forms,
         )
 
         self.controls = controls
```

### Comparing `cashocs-2.0.0b0/cashocs/_constraints/constraints.py` & `cashocs-2.0.0rc0/cashocs/_constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_constraints/solvers.py` & `cashocs-2.0.0rc0/cashocs/_constraints/solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_database/__init__.py` & `cashocs-2.0.0rc0/cashocs/_database/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_database/database.py` & `cashocs-2.0.0rc0/cashocs/_database/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
 """Main Database for all of cashocs."""
 
 from __future__ import annotations
 
-from typing import List, TYPE_CHECKING
+from typing import List, Optional, TYPE_CHECKING
 
 import fenics
 
 from cashocs._database import form_database
 from cashocs._database import function_database
 from cashocs._database import geometry_database
 from cashocs._database import parameter_database
@@ -42,27 +42,29 @@
     def __init__(
         self,
         config: io.Config,
         states: List[fenics.Function],
         adjoints: List[fenics.Function],
         state_ksp_options: List[_typing.KspOption],
         adjoint_ksp_options: List[_typing.KspOption],
+        gradient_ksp_options: Optional[List[_typing.KspOption]],
         cost_functional_list: List[_typing.CostFunctional],
         state_forms: List[ufl.Form],
         bcs_list: List[List[fenics.DirichletBC]],
         preconditioner_forms: List[ufl.Form],
     ) -> None:
         """Initialize the database.
 
         Args:
             config: The configuration for the problem.
             states: The list of state variables.
             adjoints: The list of adjoint variables.
             state_ksp_options: The list of ksp options for the state system.
             adjoint_ksp_options: The list of ksp options for the adjoint system.
+            gradient_ksp_options: The list of ksp options for computing the gradient.
             cost_functional_list: The list of cost functionals.
             state_forms: The list of state forms.
             bcs_list: The list of Dirichlet boundary conditions for the state system.
             preconditioner_forms: The list of forms for the preconditioner. The default
                 is `None`, so that the preconditioner matrix is the same as the system
                 matrix.
 
@@ -72,12 +74,13 @@
 
         self.function_db = function_database.FunctionDatabase(states, adjoints)
         self.parameter_db = parameter_database.ParameterDatabase(
             self.function_db,
             config,
             state_ksp_options,
             adjoint_ksp_options,
+            gradient_ksp_options,
         )
         self.geometry_db = geometry_database.GeometryDatabase(self.function_db)
         self.form_db = form_database.FormDatabase(
             cost_functional_list, state_forms, bcs_list, preconditioner_forms
         )
```

### Comparing `cashocs-2.0.0b0/cashocs/_database/form_database.py` & `cashocs-2.0.0rc0/cashocs/_database/form_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_database/function_database.py` & `cashocs-2.0.0rc0/cashocs/_database/function_database.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_database/geometry_database.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/pde_problem.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,32 +11,44 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
-"""Database for geometry."""
+"""General PDE problem."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+import abc
+from typing import List, TYPE_CHECKING, Union
 
 import fenics
 
 if TYPE_CHECKING:
-    from cashocs._database import function_database
+    from cashocs._database import database
 
 
-class GeometryDatabase:
-    """Database for geometry parameters."""
+class PDEProblem(abc.ABC):
+    """Base class for a PDE problem."""
 
-    def __init__(self, function_db: function_database.FunctionDatabase) -> None:
-        """Initializes the geometry database.
+    def __init__(self, db: database.Database) -> None:
+        """Initializes self.
 
         Args:
-            function_db: The database for function parameters.
+            db: The database of the problem
 
         """
-        self.mesh: fenics.Mesh = function_db.state_spaces[0].mesh()
-        self.dx: fenics.Measure = fenics.Measure("dx", self.mesh)
-        self.mpi_comm = self.mesh.mpi_comm()
+        self.db = db
+
+        self.config = db.config
+        self.has_solution = False
+
+    @abc.abstractmethod
+    def solve(self) -> Union[fenics.Function, List[fenics.Function]]:
+        """Solves the PDE.
+
+        Returns:
+            The solution of the PDE.
+
+        """
+        pass
```

### Comparing `cashocs-2.0.0b0/cashocs/_database/parameter_database.py` & `cashocs-2.0.0rc0/cashocs/_database/parameter_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
 """Database for parameters."""
 
 from __future__ import annotations
 
-from typing import Dict, List, TYPE_CHECKING
+from typing import Dict, List, Optional, TYPE_CHECKING
 
 from cashocs import _exceptions
 from cashocs import _utils
 
 if TYPE_CHECKING:
     from cashocs import _typing
     from cashocs import io
@@ -35,27 +35,30 @@
 
     def __init__(
         self,
         function_db: function_database.FunctionDatabase,
         config: io.Config,
         state_ksp_options: List[_typing.KspOption],
         adjoint_ksp_options: List[_typing.KspOption],
+        gradient_ksp_options: Optional[List[_typing.KspOption]],
     ) -> None:
         """Initializes the database.
 
         Args:
             function_db: The database for functions.
             config: The configuration.
             state_ksp_options: The list of ksp options for the state system.
             adjoint_ksp_options: The list of ksp options for the adjoint system.
+            gradient_ksp_options: The list of ksp options for computing the gradient.
 
         """
         self.config = config
         self.state_ksp_options = state_ksp_options
         self.adjoint_ksp_options = adjoint_ksp_options
+        self.gradient_ksp_options = gradient_ksp_options
         self.temp_dict: Dict = {}
 
         self._problem_type = ""
         self.state_dim: int = len(function_db.states)
 
         self.display_box_constraints: bool = False
```

### Comparing `cashocs-2.0.0b0/cashocs/_exceptions.py` & `cashocs-2.0.0rc0/cashocs/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_forms/__init__.py` & `cashocs-2.0.0rc0/cashocs/_forms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_forms/control_form_handler.py` & `cashocs-2.0.0rc0/cashocs/_forms/control_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_forms/form_handler.py` & `cashocs-2.0.0rc0/cashocs/_forms/form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_forms/general_form_handler.py` & `cashocs-2.0.0rc0/cashocs/_forms/general_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_forms/shape_form_handler.py` & `cashocs-2.0.0rc0/cashocs/_forms/shape_form_handler.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_forms/shape_regularization.py` & `cashocs-2.0.0rc0/cashocs/_forms/shape_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_loggers.py` & `cashocs-2.0.0rc0/cashocs/_loggers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/__init__.py` & `cashocs-2.0.0rc0/cashocs/_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/cost_functional.py` & `cashocs-2.0.0rc0/cashocs/_optimization/cost_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/line_search/__init__.py` & `cashocs-2.0.0rc0/cashocs/_optimization/line_search/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/line_search/armijo_line_search.py` & `cashocs-2.0.0rc0/cashocs/_optimization/line_search/armijo_line_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
 """Armijo line search algorithm."""
 
 from __future__ import annotations
 
-from typing import List
+from typing import List, Optional, Tuple
 
 import fenics
 from typing_extensions import TYPE_CHECKING
 
 from cashocs import _loggers
 from cashocs._optimization.line_search import line_search
 
@@ -85,29 +85,35 @@
         return False
 
     def search(
         self,
         solver: optimization_algorithms.OptimizationAlgorithm,
         search_direction: List[fenics.Function],
         has_curvature_info: bool,
-    ) -> None:
+    ) -> Tuple[Optional[fenics.Function], bool]:
         """Performs the line search.
 
         Args:
             solver: The optimization algorithm.
             search_direction: The current search direction.
             has_curvature_info: A flag, which indicates whether the direction is
                 (presumably) scaled.
 
+        Returns:
+            A tuple (defo, is_remeshed), where defo is accepted deformation / update
+            or None, in case the update was not successful and is_remeshed is a boolean
+            indicating whether a remeshing has been performed in the line search.
+
         """
         self.initialize_stepsize(solver, search_direction, has_curvature_info)
+        is_remeshed = False
 
         while True:
             if self._check_for_nonconvergence(solver):
-                return None
+                return (None, False)
 
             if self.db.parameter_db.problem_type == "shape":
                 self.decrease_measure_w_o_step = (
                     self.optimization_variable_abstractions.compute_decrease_measure(
                         search_direction
                     )
                 )
@@ -125,14 +131,15 @@
             decrease_measure = self._compute_decrease_measure(search_direction)
 
             if self._satisfies_armijo_condition(
                 objective_step, current_function_value, decrease_measure
             ):
                 if self.optimization_variable_abstractions.requires_remeshing():
                     self.optimization_variable_abstractions.mesh_handler.remesh(solver)
+                    is_remeshed = True
                     break
 
                 if solver.iteration == 0:
                     self.armijo_stepsize_initial = self.stepsize
                 break
 
             else:
@@ -140,15 +147,18 @@
                 self.optimization_variable_abstractions.revert_variable_update()
 
         solver.stepsize = self.stepsize
 
         if not has_curvature_info:
             self.stepsize *= self.beta_armijo
 
-        return None
+        if self.db.parameter_db.problem_type == "shape":
+            return (self.optimization_variable_abstractions.deformation, is_remeshed)
+        else:
+            return (None, False)
 
     def _compute_decrease_measure(
         self, search_direction: List[fenics.Function]
     ) -> float:
         """Computes the decrease measure for use in the Armijo line search.
 
         Args:
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/line_search/line_search.py` & `cashocs-2.0.0rc0/cashocs/_optimization/line_search/line_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
 """General line search."""
 
 from __future__ import annotations
 
 import abc
-from typing import List, TYPE_CHECKING
+from typing import cast, List, Optional, Tuple, TYPE_CHECKING
 
 import fenics
 import numpy as np
+from petsc4py import PETSc
 
 from cashocs import _utils
 
 if TYPE_CHECKING:
     from cashocs import _typing
     from cashocs._database import database
     from cashocs._optimization import optimization_algorithms
@@ -52,14 +53,20 @@
         self.form_handler = optimization_problem.form_handler
         self.state_problem = optimization_problem.state_problem
         self.optimization_variable_abstractions = (
             optimization_problem.optimization_variable_abstractions
         )
         self.cost_functional = optimization_problem.reduced_cost_functional
 
+        if self.db.parameter_db.problem_type == "shape":
+            self.deformation_function = fenics.Function(
+                self.db.function_db.control_spaces[0]
+            )
+            self.global_deformation_vector = self.deformation_function.vector().vec()
+
         self.stepsize = self.config.getfloat("LineSearch", "initial_stepsize")
         self.safeguard_stepsize = self.config.getboolean(
             "LineSearch", "safeguard_stepsize"
         )
 
         self.beta_armijo: float = self.config.getfloat("LineSearch", "beta_armijo")
         self.epsilon_armijo: float = self.config.getfloat(
@@ -90,15 +97,32 @@
         Args:
             solver: The optimization algorithm.
             search_direction: The current search direction.
             has_curvature_info: A flag, which indicates, whether the search direction
                 is (presumably) scaled.
 
         """
-        self.search(solver, search_direction, has_curvature_info)
+        deformation, is_remeshed = self.search(
+            solver, search_direction, has_curvature_info
+        )
+        if deformation is not None:
+            x = fenics.as_backend_type(deformation.vector()).vec()
+
+            if not is_remeshed:
+                transfer_matrix = self.db.geometry_db.transfer_matrix
+            else:
+                transfer_matrix = self.db.geometry_db.old_transfer_matrix
+
+            transfer_matrix = cast(PETSc.Mat, transfer_matrix)
+
+            _, temp = transfer_matrix.getVecs()
+            transfer_matrix.mult(x, temp)
+            self.global_deformation_vector.axpy(1.0, temp)
+            self.deformation_function.vector().apply("")
+
         self.post_line_search()
 
     def initialize_stepsize(
         self,
         solver: optimization_algorithms.OptimizationAlgorithm,
         search_direction: List[fenics.Function],
         has_curvature_info: bool,
@@ -144,23 +168,27 @@
 
     @abc.abstractmethod
     def search(
         self,
         solver: optimization_algorithms.OptimizationAlgorithm,
         search_direction: List[fenics.Function],
         has_curvature_info: bool,
-    ) -> None:
+    ) -> Tuple[Optional[fenics.Function], bool]:
         """Performs a line search.
 
         Args:
             solver: The optimization algorithm.
             search_direction: The current search direction.
             has_curvature_info: A flag, which indicates, whether the search direction
                 is (presumably) scaled.
 
+        Returns:
+            The accepted deformation or None, in case the deformation was not
+            successful.
+
         """
         pass
 
     def post_line_search(self) -> None:
         """Performs tasks after the line search was successful."""
         self.form_handler.update_scalar_product()
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/line_search/polynomial_line_search.py` & `cashocs-2.0.0rc0/cashocs/_optimization/line_search/polynomial_line_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """Polynomial line search algorithm."""
 
 
 from __future__ import annotations
 
 import collections
-from typing import Deque, List
+from typing import Deque, List, Optional, Tuple
 
 import fenics
 import numpy as np
 from typing_extensions import TYPE_CHECKING
 
 from cashocs import _exceptions
 from cashocs import _loggers
@@ -97,31 +97,37 @@
         return False
 
     def search(
         self,
         solver: optimization_algorithms.OptimizationAlgorithm,
         search_direction: List[fenics.Function],
         has_curvature_info: bool,
-    ) -> None:
+    ) -> Tuple[Optional[fenics.Function], bool]:
         """Performs the line search.
 
         Args:
             solver: The optimization algorithm.
             search_direction: The current search direction.
             has_curvature_info: A flag, which indicates whether the direction is
                 (presumably) scaled.
 
+        Returns:
+            The accepted deformation / update or None, in case the update was not
+            successful.
+
         """
         self.initialize_stepsize(solver, search_direction, has_curvature_info)
 
         self.f_vals.clear()
         self.alpha_vals.clear()
+
+        is_remeshed = False
         while True:
             if self._check_for_nonconvergence(solver):
-                return None
+                return (None, False)
 
             if self.db.parameter_db.problem_type == "shape":
                 self.decrease_measure_w_o_step = (
                     self.optimization_variable_abstractions.compute_decrease_measure(
                         search_direction
                     )
                 )
@@ -141,14 +147,15 @@
             decrease_measure = self._compute_decrease_measure(search_direction)
 
             if self._satisfies_armijo_condition(
                 objective_step, current_function_value, decrease_measure
             ):
                 if self.optimization_variable_abstractions.requires_remeshing():
                     self.optimization_variable_abstractions.mesh_handler.remesh(solver)
+                    is_remeshed = True
                     break
 
                 if solver.iteration == 0:
                     self.armijo_stepsize_initial = self.stepsize
                 break
 
             else:
@@ -161,15 +168,18 @@
                 self.optimization_variable_abstractions.revert_variable_update()
 
         solver.stepsize = self.stepsize
 
         if not has_curvature_info:
             self.stepsize /= self.factor_high
 
-        return None
+        if self.db.parameter_db.problem_type == "shape":
+            return (self.optimization_variable_abstractions.deformation, is_remeshed)
+        else:
+            return (None, False)
 
     def _compute_polynomial_stepsize(
         self,
         f_current: float,
         decrease_measure: float,
         f_vals: Deque[float],
         alpha_vals: Deque[float],
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimal_control/__init__.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimal_control/box_constraints.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/box_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimal_control/control_variable_abstractions.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/control_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimal_control/optimal_control_problem.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimal_control/optimal_control_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         riesz_scalar_products: Optional[Union[List[ufl.Form], ufl.Form]] = None,
         control_constraints: Optional[List[List[Union[float, fenics.Function]]]] = None,
         initial_guess: Optional[List[fenics.Function]] = None,
         ksp_options: Optional[Union[_typing.KspOption, List[_typing.KspOption]]] = None,
         adjoint_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
+        gradient_ksp_options: Optional[
+            Union[_typing.KspOption, List[_typing.KspOption]]
+        ] = None,
         desired_weights: Optional[List[float]] = None,
         control_bcs_list: Optional[
             Union[
                 List[List[fenics.DirichletBC]],
                 List[fenics.DirichletBC],
                 fenics.DirichletBC,
             ]
@@ -120,14 +123,18 @@
             ksp_options: A list of dicts corresponding to command line options for
                 PETSc, used to solve the state systems. If this is ``None``, then the
                 direct solver mumps is used (default is ``None``).
             adjoint_ksp_options: A list of dicts corresponding to command line options
                 for PETSc, used to solve the adjoint systems. If this is ``None``, then
                 the same options as for the state systems are used (default is
                 ``None``).
+            gradient_ksp_options: A list of dicts corresponding to command line options
+                for PETSc, used to compute the (shape) gradient. If this is ``None``,
+                either a direct or an iterative method is used (depending on the
+                configuration, section OptimizationRoutine, key gradient_method).
             desired_weights: A list of values for scaling the cost functional terms. If
                 this is supplied, the cost functional has to be given as list of
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration. In case
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
             control_bcs_list: A list of boundary conditions for the control variables.
@@ -147,14 +154,15 @@
             cost_functional_form,
             states,
             adjoints,
             config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
+            gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
             preconditioner_forms=preconditioner_forms,
         )
 
         self.db.function_db.controls = _utils.enlist(controls)
 
         self.db.parameter_db.control_dim = len(self.db.function_db.controls)
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/__init__.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/callback.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/callback.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/gradient_descent.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/l_bfgs.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/l_bfgs.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/ncg.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/ncg.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/newton.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/newton.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_algorithms/optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_problem.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,17 @@
         adjoints: Union[List[fenics.Function], fenics.Function],
         config: Optional[io.Config] = None,
         initial_guess: Optional[Union[List[fenics.Function], fenics.Function]] = None,
         ksp_options: Optional[Union[_typing.KspOption, List[_typing.KspOption]]] = None,
         adjoint_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
+        gradient_ksp_options: Optional[
+            Union[_typing.KspOption, List[_typing.KspOption]]
+        ] = None,
         desired_weights: Optional[List[float]] = None,
         temp_dict: Optional[Dict] = None,
         initial_function_values: Optional[List[float]] = None,
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
     ) -> None:
         r"""Initializes self.
 
@@ -128,14 +131,18 @@
             ksp_options: A list of dicts corresponding to command line options for
                 PETSc, used to solve the state systems. If this is ``None``, then the
                 direct solver mumps is used (default is ``None``).
             adjoint_ksp_options: A list of dicts corresponding to command line options
                 for PETSc, used to solve the adjoint systems. If this is ``None``, then
                 the same options as for the state systems are used (default is
                 ``None``).
+            gradient_ksp_options: A list of dicts corresponding to command line options
+                for PETSc, used to compute the (shape) gradient. If this is ``None``,
+                either a direct or an iterative method is used (depending on the
+                configuration, section OptimizationRoutine, key gradient_method).
             desired_weights: A list of values for scaling the cost functional terms. If
                 this is supplied, the cost functional has to be given as list of
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration. In case
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
             temp_dict: This is a private parameter of the class, required for remeshing.
@@ -177,20 +184,22 @@
             self.config = copy.deepcopy(config)
         self.config.validate_config()
 
         (
             self.initial_guess,
             self.ksp_options,
             self.adjoint_ksp_options,
+            self.gradient_ksp_options,
             self.desired_weights,
             self.preconditioner_forms,
         ) = self._parse_optional_inputs(
             initial_guess,
             ksp_options,
             adjoint_ksp_options,
+            gradient_ksp_options,
             desired_weights,
             preconditioner_forms,
         )
 
         if initial_function_values is not None:
             self.initial_function_values = initial_function_values
 
@@ -201,14 +210,15 @@
 
         self.db = database.Database(
             self.config,
             self.states,
             self.adjoints,
             self.ksp_options,
             self.adjoint_ksp_options,
+            self.gradient_ksp_options,
             self.cost_functional_list,
             self.state_forms,
             self.bcs_list,
             self.preconditioner_forms,
         )
         if temp_dict is not None:
             self.db.parameter_db.temp_dict.update(temp_dict)
@@ -276,32 +286,38 @@
     def _parse_optional_inputs(
         self,
         initial_guess: Optional[Union[List[fenics.Function], fenics.Function]],
         ksp_options: Optional[Union[_typing.KspOption, List[_typing.KspOption]]],
         adjoint_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ],
+        gradient_ksp_options: Optional[
+            Union[_typing.KspOption, List[_typing.KspOption]]
+        ],
         desired_weights: Optional[Union[List[float], float]],
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]],
     ) -> Tuple[
         Optional[List[fenics.Function]],
         List[_typing.KspOption],
         List[_typing.KspOption],
+        Optional[List[_typing.KspOption]],
         Optional[List[float]],
         List[Optional[ufl.Form]],
     ]:
         """Initializes the optional input parameters.
 
         Args:
             initial_guess: List of functions that act as initial guess for the state
                 variables, should be valid input for :py:func:`fenics.assign`.
             ksp_options: A list of dicts corresponding to command line options for
                 PETSc, used to solve the state systems.
             adjoint_ksp_options: A list of dicts corresponding to command line options
                 for PETSc, used to solve the adjoint systems.
+            gradient_ksp_options: A list of dicts corresponding to command line options
+                for computing the gradient with PETSc.
             desired_weights: A list of values for scaling the cost functional terms. If
                 this is supplied, the cost functional has to be given as list of
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration.
             preconditioner_forms: The list of forms for the preconditioner. The default
                 is `None`, so that the preconditioner matrix is the same as the system
                 matrix.
@@ -323,14 +339,19 @@
 
         parsed_adjoint_ksp_options: List[_typing.KspOption] = (
             parsed_ksp_options[:]
             if adjoint_ksp_options is None
             else _utils.enlist(adjoint_ksp_options)
         )
 
+        if gradient_ksp_options is None:
+            parsed_gradient_ksp_options = None
+        else:
+            parsed_gradient_ksp_options = _utils.enlist(gradient_ksp_options)
+
         if desired_weights is None:
             parsed_desired_weights = desired_weights
         else:
             parsed_desired_weights = _utils.enlist(desired_weights)
             self.use_scaling = True
 
         if preconditioner_forms is None:
@@ -340,14 +361,15 @@
         else:
             parsed_preconditioner_forms = _utils.enlist(preconditioner_forms)
 
         return (
             parsed_initial_guess,
             parsed_ksp_options,
             parsed_adjoint_ksp_options,
+            parsed_gradient_ksp_options,
             parsed_desired_weights,
             parsed_preconditioner_forms,
         )
 
     def compute_state_variables(self) -> None:
         """Solves the state system.
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/optimization_variable_abstractions.py` & `cashocs-2.0.0rc0/cashocs/_optimization/optimization_variable_abstractions.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
             optimization_problem: The corresponding optimization problem.
             db: The database of the problem.
 
         """
         self.db = db
 
         self.form_handler = optimization_problem.form_handler
+        self.deformation = fenics.Function(self.db.function_db.control_spaces[0])
 
     @abc.abstractmethod
     def compute_decrease_measure(
         self, search_direction: List[fenics.Function]
     ) -> float:
         """Computes the measure of decrease needed for the Armijo test.
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/__init__.py` & `cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/shape_optimization_problem.py` & `cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/shape_optimization_problem.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         config: Optional[io.Config] = None,
         shape_scalar_product: Optional[ufl.Form] = None,
         initial_guess: Optional[List[fenics.Function]] = None,
         ksp_options: Optional[Union[_typing.KspOption, List[_typing.KspOption]]] = None,
         adjoint_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
+        gradient_ksp_options: Optional[
+            Union[_typing.KspOption, List[_typing.KspOption]]
+        ] = None,
         desired_weights: Optional[List[float]] = None,
         temp_dict: Optional[Dict] = None,
         initial_function_values: Optional[List[float]] = None,
         preconditioner_forms: Optional[Union[List[ufl.Form], ufl.Form]] = None,
     ) -> None:
         """Initializes self.
 
@@ -126,14 +129,18 @@
             ksp_options: A list of dicts corresponding to command line options for
                 PETSc, used to solve the state systems. If this is ``None``, then the
                 direct solver mumps is used (default is ``None``).
             adjoint_ksp_options: A list of dicts corresponding to command line options
                 for PETSc, used to solve the adjoint systems. If this is ``None``, then
                 the same options as for the state systems are used (default is
                 ``None``).
+            gradient_ksp_options: A list of dicts corresponding to command line options
+                for PETSc, used to compute the (shape) gradient. If this is ``None``,
+                either a direct or an iterative method is used (depending on the
+                configuration, section OptimizationRoutine, key gradient_method).
             desired_weights: A list of values for scaling the cost functional terms. If
                 this is supplied, the cost functional has to be given as list of
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration. In case
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
             temp_dict: This is a private parameter of the class, required for remeshing.
@@ -153,14 +160,15 @@
             cost_functional_form,
             states,
             adjoints,
             config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
+            gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
             temp_dict=temp_dict,
             initial_function_values=initial_function_values,
             preconditioner_forms=preconditioner_forms,
         )
 
         if shape_scalar_product is None:
@@ -170,14 +178,15 @@
         else:
             deformation_space = shape_scalar_product.arguments()[0].ufl_function_space()
         self.db.function_db.control_spaces = [deformation_space]
         self.db.function_db.gradient = [
             fenics.Function(self.db.function_db.control_spaces[0])
         ]
         self.db.parameter_db.problem_type = "shape"
+        self.db.geometry_db.init_transfer_matrix()
 
         # Initialize the remeshing behavior, and a temp file
         self.do_remesh = self.config.getboolean("Mesh", "remesh")
 
         self._remesh_init()
 
         self.boundaries: fenics.MeshFunction = boundaries
@@ -243,22 +252,24 @@
             self.__init__(  # type: ignore # pylint: disable=unnecessary-dunder-call
                 state_forms,
                 bcs_list,
                 cost_functional_form,
                 states,
                 adjoints,
                 boundaries,
-                config,
-                shape_scalar_product,
-                initial_guess,
-                ksp_options,
-                adjoint_ksp_options,
-                None,
-                temp_dict,
-                self.initial_function_values,
+                config=config,
+                shape_scalar_product=shape_scalar_product,
+                initial_guess=initial_guess,
+                ksp_options=ksp_options,
+                adjoint_ksp_options=adjoint_ksp_options,
+                gradient_ksp_options=gradient_ksp_options,
+                desired_weights=None,
+                temp_dict=temp_dict,
+                initial_function_values=self.initial_function_values,
+                preconditioner_forms=preconditioner_forms,
             )
 
     @__init__.register(CallableFunction)
     def _(self, mesh_parametrization: Callable, mesh_name: str) -> None:
         """Initializes self. Version for remeshing.
 
         Args:
@@ -325,14 +336,17 @@
         if line_search_type == "armijo":
             line_search: ls.LineSearch = ls.ArmijoLineSearch(self.db, self)
         elif line_search_type == "polynomial":
             line_search = ls.PolynomialLineSearch(self.db, self)
         else:
             raise _exceptions.CashocsException("This code cannot be reached.")
 
+        self.global_deformation_vector = line_search.global_deformation_vector
+        self.global_deformation_function = line_search.deformation_function
+
         if self.algorithm.casefold() == "gradient_descent":
             solver: optimization_algorithms.OptimizationAlgorithm = (
                 optimization_algorithms.GradientDescentMethod(
                     self.db, self, line_search
                 )
             )
         elif self.algorithm.casefold() == "lbfgs":
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py` & `cashocs-2.0.0rc0/cashocs/_optimization/shape_optimization/shape_variable_abstractions.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
             optimization_problem: The corresponding optimization problem.
             db: The database of the problem.
 
         """
         super().__init__(optimization_problem, db)
         self.form_handler = cast(_forms.ShapeFormHandler, self.form_handler)
         self.mesh_handler = optimization_problem.mesh_handler
-        self.deformation = fenics.Function(self.db.function_db.control_spaces[0])
 
     def compute_decrease_measure(
         self, search_direction: List[fenics.Function]
     ) -> float:
         """Computes the measure of decrease needed for the Armijo test.
 
         Args:
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/__init__.py` & `cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py` & `cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/descent_topology_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py` & `cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/topology_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/topology_optimization_problem.py` & `cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/topology_optimization_problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
         config: io.Config | None = None,
         riesz_scalar_products: list[ufl.Form] | ufl.Form | None = None,
         initial_guess: list[fenics.Function] | None = None,
         ksp_options: Optional[Union[_typing.KspOption, List[_typing.KspOption]]] = None,
         adjoint_ksp_options: Optional[
             Union[_typing.KspOption, List[_typing.KspOption]]
         ] = None,
+        gradient_ksp_options: Optional[
+            Union[_typing.KspOption, List[_typing.KspOption]]
+        ] = None,
         desired_weights: list[float] | None = None,
     ) -> None:
         r"""Initializes the topology optimization problem.
 
         Args:
             state_forms: The weak form of the state equation (user implemented). Can be
                 either a single UFL form, or a (ordered) list of UFL forms.
@@ -115,14 +118,18 @@
             ksp_options: A list of strings corresponding to command line options for
                 PETSc, used to solve the state systems. If this is ``None``, then the
                 direct solver mumps is used (default is ``None``).
             adjoint_ksp_options: A list of strings corresponding to command line options
                 for PETSc, used to solve the adjoint systems. If this is ``None``, then
                 the same options as for the state systems are used (default is
                 ``None``).
+            gradient_ksp_options: A list of dicts corresponding to command line options
+                for PETSc, used to compute the (shape) gradient. If this is ``None``,
+                either a direct or an iterative method is used (depending on the
+                configuration, section OptimizationRoutine, key gradient_method).
             desired_weights: A list of values for scaling the cost functional terms. If
                 this is supplied, the cost functional has to be given as list of
                 summands. The individual terms are then scaled, so that term `i` has the
                 magnitude of `desired_weights[i]` for the initial iteration. In case
                 that `desired_weights` is `None`, no scaling is performed. Default is
                 `None`.
 
@@ -133,14 +140,15 @@
             cost_functional_form,
             states,
             adjoints,
             config=config,
             initial_guess=initial_guess,
             ksp_options=ksp_options,
             adjoint_ksp_options=adjoint_ksp_options,
+            gradient_ksp_options=gradient_ksp_options,
             desired_weights=desired_weights,
         )
 
         self.db.parameter_db.problem_type = "topology"
         self.mesh_parametrization = None
 
         self.levelset_function = levelset_function
```

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py` & `cashocs-2.0.0rc0/cashocs/_optimization/topology_optimization/topology_variable_abstractions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_optimization/verification.py` & `cashocs-2.0.0rc0/cashocs/_optimization/verification.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/__init__.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/adjoint_problem.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/adjoint_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/control_gradient_problem.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/control_gradient_problem.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,30 +68,28 @@
 
         gradient_tol: float = self.config.getfloat(
             "OptimizationRoutine", "gradient_tol"
         )
 
         gradient_method: str = self.config.get("OptimizationRoutine", "gradient_method")
 
-        if gradient_method.casefold() == "direct":
-            option: _typing.KspOption = copy.deepcopy(_utils.linalg.direct_ksp_options)
-        elif gradient_method.casefold() == "iterative":
-            option = {
-                "ksp_type": "cg",
-                "pc_type": "hypre",
-                "pc_hypre_type": "boomeramg",
-                "pc_hypre_boomeramg_strong_threshold": 0.7,
-                "ksp_rtol": gradient_tol,
-                "ksp_atol": 1e-50,
-                "ksp_max_it": 250,
-            }
-
-        self.riesz_ksp_options = []
-        for _ in range(len(self.db.function_db.gradient)):
-            self.riesz_ksp_options.append(option)
+        if db.parameter_db.gradient_ksp_options is not None:
+            self.riesz_ksp_options = db.parameter_db.gradient_ksp_options
+        else:
+            if gradient_method.casefold() == "direct":
+                option: _typing.KspOption = copy.deepcopy(
+                    _utils.linalg.direct_ksp_options
+                )
+            elif gradient_method.casefold() == "iterative":
+                option = copy.deepcopy(_utils.linalg.iterative_ksp_options)
+                option["ksp_rtol"] = gradient_tol
+
+            self.riesz_ksp_options = []
+            for _ in range(len(self.db.function_db.gradient)):
+                self.riesz_ksp_options.append(option)
 
         self.b_tensors = [
             fenics.PETScVector() for _ in range(len(self.db.function_db.gradient))
         ]
 
     def solve(self) -> List[fenics.Function]:
         """Solves the Riesz projection problem to obtain the gradient.
```

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/hessian_problems.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/hessian_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/pde_problem.py` & `cashocs-2.0.0rc0/cashocs/_database/geometry_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,44 +11,49 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with cashocs.  If not, see <https://www.gnu.org/licenses/>.
 
-"""General PDE problem."""
+"""Database for geometry."""
 
 from __future__ import annotations
 
-import abc
-from typing import List, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 
 import fenics
+import mpi4py.MPI
 
-if TYPE_CHECKING:
-    from cashocs._database import database
-
+from cashocs import _utils
 
-class PDEProblem(abc.ABC):
-    """Base class for a PDE problem."""
+if TYPE_CHECKING:
+    from petsc4py import PETSc
 
-    def __init__(self, db: database.Database) -> None:
-        """Initializes self.
+    from cashocs._database import function_database
 
-        Args:
-            db: The database of the problem
 
-        """
-        self.db = db
+class GeometryDatabase:
+    """Database for geometry parameters."""
 
-        self.config = db.config
-        self.has_solution = False
+    transfer_matrix: PETSc.Mat
+    old_transfer_matrix: PETSc.Mat
 
-    @abc.abstractmethod
-    def solve(self) -> Union[fenics.Function, List[fenics.Function]]:
-        """Solves the PDE.
+    def __init__(self, function_db: function_database.FunctionDatabase) -> None:
+        """Initializes the geometry database.
 
-        Returns:
-            The solution of the PDE.
+        Args:
+            function_db: The database for function parameters.
 
         """
-        pass
+        self.mesh: fenics.Mesh = function_db.state_spaces[0].mesh()
+        self.dx: fenics.Measure = fenics.Measure("dx", self.mesh)
+        self.mpi_comm: mpi4py.MPI.Intracomm = self.mesh.mpi_comm()
+
+        self.function_db = function_db
+
+    def init_transfer_matrix(self) -> None:
+        """Initializes the transfer matrix for computing the global deformation."""
+        interp = _utils.Interpolator(
+            self.function_db.control_spaces[0], self.function_db.control_spaces[0]
+        )
+        self.transfer_matrix = interp.transfer_matrix
```

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/shape_gradient_problem.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/shape_gradient_problem.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,26 +71,21 @@
 
         self.gradient_norm_squared = 1.0
 
         gradient_tol = self.config.getfloat("OptimizationRoutine", "gradient_tol")
 
         gradient_method = self.config.get("OptimizationRoutine", "gradient_method")
 
-        if gradient_method.casefold() == "direct":
+        if db.parameter_db.gradient_ksp_options is not None:
+            self.ksp_options = db.parameter_db.gradient_ksp_options[0]
+        elif gradient_method.casefold() == "direct":
             self.ksp_options = copy.deepcopy(_utils.linalg.direct_ksp_options)
         elif gradient_method.casefold() == "iterative":
-            self.ksp_options = {
-                "ksp_type": "cg",
-                "pc_type": "hypre",
-                "pc_hypre_type": "boomeramg",
-                "pc_hypre_boomeramg_strong_threshold": 0.7,
-                "ksp_rtol": gradient_tol,
-                "ksp_atol": 1e-50,
-                "ksp_max_it": 250,
-            }
+            self.ksp_options = copy.deepcopy(_utils.linalg.iterative_ksp_options)
+            self.ksp_options["ksp_rtol"] = gradient_tol
 
         if (
             self.config.getboolean("ShapeGradient", "use_p_laplacian")
             and self.form_handler.use_fixed_dimensions
         ):
             _loggers.warning(
                 "Incompatible config settings: "
@@ -221,26 +216,23 @@
                 * dx
                 + fenics.Constant(delta)
                 * fenics.dot(self.solution, self.test_vector_field)
                 * dx
             )
 
             gradient_method = config.get("OptimizationRoutine", "gradient_method")
+            gradient_tol = config.get("OptimizationRoutine", "gradient_tol")
 
-            if gradient_method.casefold() == "direct":
+            if db.parameter_db.gradient_ksp_options is not None:
+                self.ksp_options = db.parameter_db.gradient_ksp_options[0]
+            elif gradient_method.casefold() == "direct":
                 self.ksp_options = copy.deepcopy(_utils.linalg.direct_ksp_options)
             elif gradient_method.casefold() == "iterative":
-                self.ksp_options = {
-                    "ksp_type": "cg",
-                    "pc_type": "hypre",
-                    "pc_hypre_type": "boomeramg",
-                    "ksp_rtol": 1e-16,
-                    "ksp_atol": 1e-50,
-                    "ksp_max_it": 100,
-                }
+                self.ksp_options = copy.deepcopy(_utils.linalg.iterative_ksp_options)
+                self.ksp_options["ksp_rtol"] = gradient_tol
 
     def solve(self) -> None:
         """Solves the p-Laplace problem for computing the shape gradient."""
         self.solution.vector().vec().set(0.0)
         self.solution.vector().apply("")
         for nonlinear_form in self.form_list:
             nonlinear_solvers.newton_solve(
```

### Comparing `cashocs-2.0.0b0/cashocs/_pde_problems/state_problem.py` & `cashocs-2.0.0rc0/cashocs/_pde_problems/state_problem.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_typing.py` & `cashocs-2.0.0rc0/cashocs/_typing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_utils/__init__.py` & `cashocs-2.0.0rc0/cashocs/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_utils/forms.py` & `cashocs-2.0.0rc0/cashocs/_utils/forms.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_utils/helpers.py` & `cashocs-2.0.0rc0/cashocs/_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_utils/interpolations.py` & `cashocs-2.0.0rc0/cashocs/_utils/interpolations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/_utils/linalg.py` & `cashocs-2.0.0rc0/cashocs/_utils/linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
     Args:
         ksps: A list of PETSc KSP objects (linear solvers) to which the (command line)
             options are applied to.
         ksp_options: A list of command line options that specify the iterative solver
             from PETSc.
 
     """
+    fenics.PETScOptions.clear()
     opts = PETSc.Options()
 
     for i in range(len(ksps)):
         opts.clear()
 
         for key, value in ksp_options[i].items():
             opts.setValue(key, value)
```

### Comparing `cashocs-2.0.0b0/cashocs/geometry/__init__.py` & `cashocs-2.0.0rc0/cashocs/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/geometry/boundary_distance.py` & `cashocs-2.0.0rc0/cashocs/geometry/boundary_distance.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/geometry/deformations.py` & `cashocs-2.0.0rc0/cashocs/geometry/deformations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/geometry/measure.py` & `cashocs-2.0.0rc0/cashocs/geometry/measure.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/geometry/mesh.py` & `cashocs-2.0.0rc0/cashocs/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/geometry/mesh_handler.py` & `cashocs-2.0.0rc0/cashocs/geometry/mesh_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from cashocs import _exceptions
 from cashocs import _loggers
 from cashocs import _utils
 from cashocs import io
 from cashocs._optimization import line_search as ls
 from cashocs.geometry import deformations
 from cashocs.geometry import quality
+from cashocs.io.mesh import import_mesh
 
 if TYPE_CHECKING:
     from cashocs import _forms
     from cashocs import _typing
     from cashocs._database import database
     from cashocs._optimization.optimization_algorithms import OptimizationAlgorithm
     from cashocs.geometry import mesh_testing
@@ -632,14 +633,16 @@
             self.db.parameter_db.temp_dict["OptimizationRoutine"][
                 "iteration_counter"
             ] = solver.iteration
             self.db.parameter_db.temp_dict["OptimizationRoutine"][
                 "gradient_norm_initial"
             ] = solver.gradient_norm_initial
 
+            self._update_mesh_transfer_matrix(new_xdmf_file)
+
             self._reinitialize(solver)
             self._check_imported_mesh_quality(solver)
 
     def _check_imported_mesh_quality(self, solver: OptimizationAlgorithm) -> None:
         """Checks the quality of an imported mesh.
 
         This function raises exceptions when the mesh does not satisfy the desired
@@ -667,7 +670,31 @@
         current_mesh_quality = quality.compute_mesh_quality(
             mesh,
             mesh_quality_type,
             mesh_quality_measure,
         )
 
         check_mesh_quality_tolerance(current_mesh_quality, mesh_quality_tol_upper)
+
+    def _update_mesh_transfer_matrix(self, xdmf_filename: str) -> None:
+        """Updates the transfer matrix for the global deformation after remeshing.
+
+        Args:
+            xdmf_filename: The filename for the new mesh (in XDMF format).
+
+        """
+        pre_log_level = (
+            _loggers._cashocs_logger.level  # pylint: disable=protected-access
+        )
+        _loggers.set_log_level(_loggers.LogLevel.WARNING)
+        mesh, _, _, _, _, _ = import_mesh(xdmf_filename)
+        _loggers.set_log_level(pre_log_level)
+
+        deformation_space = fenics.VectorFunctionSpace(mesh, "CG", 1)
+        interpolator = _utils.Interpolator(
+            deformation_space, self.db.function_db.control_spaces[0]
+        )
+        new_transfer_matrix = self.db.geometry_db.transfer_matrix.matMult(
+            interpolator.transfer_matrix
+        )
+        self.db.geometry_db.old_transfer_matrix = self.db.geometry_db.transfer_matrix
+        self.db.geometry_db.transfer_matrix = new_transfer_matrix
```

### Comparing `cashocs-2.0.0b0/cashocs/geometry/mesh_testing.py` & `cashocs-2.0.0rc0/cashocs/geometry/mesh_testing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/geometry/quality.py` & `cashocs-2.0.0rc0/cashocs/geometry/quality.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/io/__init__.py` & `cashocs-2.0.0rc0/cashocs/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/io/config.py` & `cashocs-2.0.0rc0/cashocs/io/config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/io/function.py` & `cashocs-2.0.0rc0/cashocs/io/function.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/io/managers.py` & `cashocs-2.0.0rc0/cashocs/io/managers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/io/mesh.py` & `cashocs-2.0.0rc0/cashocs/io/mesh.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/io/output.py` & `cashocs-2.0.0rc0/cashocs/io/output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/nonlinear_solvers/__init__.py` & `cashocs-2.0.0rc0/cashocs/nonlinear_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/nonlinear_solvers/linear_solver.py` & `cashocs-2.0.0rc0/cashocs/nonlinear_solvers/linear_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/nonlinear_solvers/newton_solver.py` & `cashocs-2.0.0rc0/cashocs/nonlinear_solvers/newton_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/nonlinear_solvers/picard_solver.py` & `cashocs-2.0.0rc0/cashocs/nonlinear_solvers/picard_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/space_mapping/__init__.py` & `cashocs-2.0.0rc0/cashocs/space_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/space_mapping/optimal_control.py` & `cashocs-2.0.0rc0/cashocs/space_mapping/optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs/space_mapping/shape_optimization.py` & `cashocs-2.0.0rc0/cashocs/space_mapping/shape_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/cashocs.egg-info/PKG-INFO` & `cashocs-2.0.0rc0/cashocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashocs
-Version: 2.0.0b0
+Version: 2.0.0rc0
 Summary: Computational Adjoint-Based Shape Optimization and Optimal Control Software
 Author: Sebastian Blauth
 Author-email: sebastian.blauth@itwm.fraunhofer.de
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Documentation, https://cashocs.readthedocs.io/en/latest
 Project-URL: Source, https://github.com/sblauth/cashocs
 Project-URL: Tutorial, https://cashocs.readthedocs.io/en/latest/user
@@ -327,14 +327,14 @@
 
 
 .. readme_start_about
 
 Contact / About
 ===============
 
-I'm `Sebastian Blauth <https://www.itwm.fraunhofer.de/en/departments/tv/staff/sebastian-blauth.html>`_, a scientific employee at `Fraunhofer ITWM
+I'm `Sebastian Blauth <https://sblauth.github.io/>`_, a scientific employee at `Fraunhofer ITWM
 <https://www.itwm.fraunhofer.de/en.html>`_. I have developed this project as part of my PhD thesis.
 If you have any questions / suggestions / feedback, etc., you can contact me
 via `sebastian.blauth@itwm.fraunhofer.de
-<mailto:sebastian.blauth@itwm.fraunhofer.de>`_.
+<mailto:sebastian.blauth@itwm.fraunhofer.de>`_. For more information, visit my website at `<https://sblauth.github.io/>`_.
 
 .. readme_end_about
```

### Comparing `cashocs-2.0.0b0/cashocs.egg-info/SOURCES.txt` & `cashocs-2.0.0rc0/cashocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py` & `cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/control_solver/demo_control_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py` & `cashocs-2.0.0rc0/demos/documented/cashocs_as_solver/shape_solver/demo_shape_solver.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/misc/xdmf_io/demo_xdmf_io.py` & `cashocs-2.0.0rc0/demos/documented/misc/xdmf_io/demo_xdmf_io.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/box_constraints/demo_box_constraints.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/box_constraints/demo_box_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/constraints/demo_constraints.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/constraints/demo_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/control_boundary_conditions/demo_control_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/dirichlet_control/demo_dirichlet_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/heat_equation/demo_heat_equation.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/heat_equation/demo_heat_equation.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/iterative_solvers/demo_iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/monolithic_problems/demo_monolithic_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/multiple_variables/demo_multiple_variables.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/neumann_control/demo_neumann_control.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/neumann_control/demo_neumann_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/nonlinear_pdes/demo_nonlinear_pdes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/picard_iteration/demo_picard_iteration.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/poisson/demo_poisson.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/poisson/demo_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/pre_post_callbacks/demo_pre_post_callbacks.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/scalar_control_tracking/demo_scalar_control_tracking.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/sparse_control/demo_sparse_control.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/sparse_control/demo_sparse_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/state_constraints/demo_state_constraints.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/state_constraints/demo_state_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/optimal_control/stokes/demo_stokes.py` & `cashocs-2.0.0rc0/demos/documented/optimal_control/stokes/demo_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/custom_scalar_product/demo_custom_scalar_product.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/eikonal_stiffness/demo_eikonal_stiffness.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/inverse_tomography/demo_inverse_tomography.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/p_laplacian/demo_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/regularization/demo_regularization.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/regularization/demo_regularization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/remeshing/demo_remeshing.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/remeshing/demo_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/scaling/demo_scaling.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/scaling/demo_scaling.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/shape_poisson/demo_shape_poisson.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/shape_stokes/demo_shape_stokes.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/space_mapping_semilinear_transmission/demo_space_mapping_semilinear_transmission.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py` & `cashocs-2.0.0rc0/demos/documented/shape_optimization/space_mapping_uniform_flow_distribution/demo_space_mapping_uniform_flow_distribution.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/test.py` & `cashocs-2.0.0rc0/demos/test.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/test_mpi.py` & `cashocs-2.0.0rc0/demos/test_mpi.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py` & `cashocs-2.0.0rc0/demos/undocumented/optimal_control/different_state_adjoint_spaces/demo_different_state_adjoint_spaces.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py` & `cashocs-2.0.0rc0/demos/undocumented/optimal_control/dirichlet_control_via_lagrange_multiplier/demo_dirichlet_control_via_lagrange_multiplier.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/undocumented/shape_optimization/custom_functional/custom_functional.py` & `cashocs-2.0.0rc0/demos/undocumented/shape_optimization/custom_functional/custom_functional.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py` & `cashocs-2.0.0rc0/demos/undocumented/shape_optimization/pipe_optimization/pipe_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/docs/source/conf.py` & `cashocs-2.0.0rc0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "cashocs"
 copyright = "2020-2023, Sebastian Blauth"
 author = "Sebastian Blauth"
 
 # The full version, including alpha/beta/rc tags
-release = "2.0.0-beta0"
+release = "2.0.0-rc0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -69,14 +69,15 @@
     "show-inheritance": True,
 }
 autodoc_member_order = "alphabetical"
 autodoc_mock_imports = [
     "fenics",
     "numpy",
     "petsc4py",
+    "mpi4py",
     "ufl",
     "meshio",
     "dolfin",
     "configparser",
     "h5py",
 ]
 autodoc_typehints = "description"
```

### Comparing `cashocs-2.0.0b0/docs/source/jupytext_process.py` & `cashocs-2.0.0rc0/docs/source/jupytext_process.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/pyproject.toml` & `cashocs-2.0.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cashocs"
-version = "2.0.0-beta0"
+version = "2.0.0-rc0"
 description = "Computational Adjoint-Based Shape Optimization and Optimal Control Software"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
 authors = [
 	{name = "Sebastian Blauth"},
 	{email = "sebastian.blauth@itwm.fraunhofer.de"}
@@ -127,12 +127,12 @@
 
 [[tool.mypy.overrides]]
 module = [
 	"fenics.*",
 	"ufl.*",
 	"dolfin.*",
 	"petsc4py",
-    "mpi4py",
+    "mpi4py.*",
 	"meshio",
 	"h5py",
 ]
 ignore_missing_imports = true
```

### Comparing `cashocs-2.0.0b0/tests/conftest.py` & `cashocs-2.0.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_cli.py` & `cashocs-2.0.0rc0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_config.py` & `cashocs-2.0.0rc0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_control_constraints.py` & `cashocs-2.0.0rc0/tests/test_control_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_exceptions.py` & `cashocs-2.0.0rc0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_geometry.py` & `cashocs-2.0.0rc0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_log_level.py` & `cashocs-2.0.0rc0/tests/test_log_level.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_nonlinear_solvers.py` & `cashocs-2.0.0rc0/tests/test_nonlinear_solvers.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_optimal_control.py` & `cashocs-2.0.0rc0/tests/test_optimal_control.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_optimal_control_multiple.py` & `cashocs-2.0.0rc0/tests/test_optimal_control_multiple.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_optimal_control_space_mapping.py` & `cashocs-2.0.0rc0/tests/test_optimal_control_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_output.py` & `cashocs-2.0.0rc0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_p_laplacian.py` & `cashocs-2.0.0rc0/tests/test_p_laplacian.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_pde_problems.py` & `cashocs-2.0.0rc0/tests/test_pde_problems.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_picard_iterations.py` & `cashocs-2.0.0rc0/tests/test_picard_iterations.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_remeshing.py` & `cashocs-2.0.0rc0/tests/test_remeshing.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_shape_constraints.py` & `cashocs-2.0.0rc0/tests/test_shape_constraints.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_shape_optimization.py` & `cashocs-2.0.0rc0/tests/test_shape_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1094,7 +1094,24 @@
 
     mesh.coordinates()[:, :] = initial_coordinates
     mesh.bounding_box_tree().build(mesh)
     sop = cashocs.ShapeOptimizationProblem(e, bcs, J, u, p, boundaries, config)
     with pytest.raises(NotConvergedError) as e_info:
         sop.solve(algorithm="ncg", rtol=1e-3, atol=0.0, max_iter=1000)
     assert "Armijo rule failed." in str(e_info.value)
+
+
+def test_global_deformation():
+    config = cashocs.load_config(dir_path + "/config_sop.ini")
+
+    mesh.coordinates()[:, :] = initial_coordinates
+    mesh.bounding_box_tree().build(mesh)
+    sop = cashocs.ShapeOptimizationProblem(e, bcs, J, u, p, boundaries, config)
+    sop.solve(algorithm="bfgs", rtol=1e-2, atol=0.0, max_iter=7)
+    assert sop.solver.relative_norm < sop.solver.rtol
+
+    optimized_coordinates = mesh.coordinates().copy()
+
+    mesh.coordinates()[:, :] = initial_coordinates
+    mesh.bounding_box_tree().build(mesh)
+    sop.mesh_handler.move_mesh(sop.global_deformation_function)
+    assert np.max(np.abs(optimized_coordinates - mesh.coordinates())) <= 1e-13
```

### Comparing `cashocs-2.0.0b0/tests/test_shape_optimization_space_mapping.py` & `cashocs-2.0.0rc0/tests/test_shape_optimization_space_mapping.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_topology_optimization.py` & `cashocs-2.0.0rc0/tests/test_topology_optimization.py`

 * *Files identical despite different names*

### Comparing `cashocs-2.0.0b0/tests/test_utils.py` & `cashocs-2.0.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

