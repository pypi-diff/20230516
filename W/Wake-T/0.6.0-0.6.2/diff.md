# Comparing `tmp/Wake-T-0.6.0.tar.gz` & `tmp/Wake-T-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Wake-T/Wake-T/dist/.tmp-j_mnigir/Wake-T-0.6.0.tar", last modified: Fri Mar 10 15:09:06 2023, max compression
+gzip compressed data, was "/home/runner/work/Wake-T/Wake-T/dist/.tmp-hc6z20zm/Wake-T-0.6.2.tar", last modified: Tue May 16 08:58:08 2023, max compression
```

## Comparing `Wake-T-0.6.0.tar` & `Wake-T-0.6.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (116)    35147 2023-03-10 15:08:57.000000 Wake-T-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4097 2023-03-10 15:09:06.000000 Wake-T-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3410 2023-03-10 15:08:57.000000 Wake-T-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/Wake_T.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4097 2023-03-10 15:09:06.000000 Wake-T-0.6.0/Wake_T.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3598 2023-03-10 15:09:06.000000 Wake-T-0.6.0/Wake_T.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-10 15:09:06.000000 Wake-T-0.6.0/Wake_T.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      106 2023-03-10 15:09:06.000000 Wake-T-0.6.0/Wake_T.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2023-03-10 15:09:06.000000 Wake-T-0.6.0/Wake_T.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       90 2023-03-10 15:08:57.000000 Wake-T-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      898 2023-03-10 15:09:06.000000 Wake-T-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       69 2023-03-10 15:08:57.000000 Wake-T-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2086 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_active_plasma_lens.py
--rw-r--r--   0 runner    (1001) docker     (116)     5020 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_beam_deposition.py
--rw-r--r--   0 runner    (1001) docker     (116)     4171 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_beamline.py
--rw-r--r--   0 runner    (1001) docker     (116)     5445 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_bunch_read_save.py
--rw-r--r--   0 runner    (1001) docker     (116)     3021 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_custom_blowout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1983 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_field_element.py
--rw-r--r--   0 runner    (1001) docker     (116)     4831 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_field_gathering.py
--rw-r--r--   0 runner    (1001) docker     (116)     2619 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_fluid_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     3762 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (116)     6558 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_laser_envelope_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     4144 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_laser_initialization.py
--rw-r--r--   0 runner    (1001) docker     (116)     2938 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_multibunch.py
--rw-r--r--   0 runner    (1001) docker     (116)      795 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_no_bunch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2421 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_openpmd_viewer.py
--rw-r--r--   0 runner    (1001) docker     (116)     3260 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_parabolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (116)     3492 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_particle_bunch_species.py
--rw-r--r--   0 runner    (1001) docker     (116)     1402 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_plasma_beamline.py
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_plasma_deposition.py
--rw-r--r--   0 runner    (1001) docker     (116)     2073 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_ramps.py
--rw-r--r--   0 runner    (1001) docker     (116)     3390 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_sc_baxevanis.py
--rw-r--r--   0 runner    (1001) docker     (116)     2924 2023-03-10 15:08:57.000000 Wake-T-0.6.0/tests/test_simple_blowout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/
--rw-r--r--   0 runner    (1001) docker     (116)      680 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/beamline_elements/
--rw-r--r--   0 runner    (1001) docker     (116)      425 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4344 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/active_plasma_lens.py
--rw-r--r--   0 runner    (1001) docker     (116)     1907 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/beamline.py
--rw-r--r--   0 runner    (1001) docker     (116)     4471 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/field_element.py
--rw-r--r--   0 runner    (1001) docker     (116)     6041 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/plasma_ramp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4839 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/plasma_stage.py
--rw-r--r--   0 runner    (1001) docker     (116)    16114 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/beamline_elements/tm_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (116)      309 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6299 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/diagnostics/bunch_analysis.py
--rw-r--r--   0 runner    (1001) docker     (116)    13147 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/diagnostics/openpmd_diag.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/fields/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3659 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/analytical_field.py
--rw-r--r--   0 runner    (1001) docker     (116)     2646 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     1559 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/gather.py
--rw-r--r--   0 runner    (1001) docker     (116)     3197 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (116)     3504 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/numerical_field.py
--rw-r--r--   0 runner    (1001) docker     (116)     8690 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/fields/rz_wakefield.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/particles/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10897 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/deposition.py
--rw-r--r--   0 runner    (1001) docker     (116)     9994 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (116)    12414 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/particle_bunch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/particles/push/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3244 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/push/boris_pusher.py
--rw-r--r--   0 runner    (1001) docker     (116)     5439 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/push/runge_kutta_4.py
--rw-r--r--   0 runner    (1001) docker     (116)     2078 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/particles/push/transfer_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/beam_optics/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/beam_optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9000 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/beam_optics/transfer_matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/collective_effects/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/collective_effects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15619 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/collective_effects/csr.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/em_fields/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/em_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      962 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/em_fields/linear_b_theta.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/laser/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/laser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5337 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/laser/envelope_solver.py
--rw-r--r--   0 runner    (1001) docker     (116)     5288 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/laser/envelope_solver_non_centered.py
--rw-r--r--   0 runner    (1001) docker     (116)    20143 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/laser/laser_pulse.py
--rw-r--r--   0 runner    (1001) docker     (116)     1341 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/laser/tdma.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/
--rw-r--r--   0 runner    (1001) docker     (116)      480 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2098 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/custom_blowout.py
--rw-r--r--   0 runner    (1001) docker     (116)      744 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/focusing_blowout.py
--rw-r--r--   0 runner    (1001) docker     (116)     7448 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/from_pic.py
--rw-r--r--   0 runner    (1001) docker     (116)    10485 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/
--rw-r--r--   0 runner    (1001) docker     (116)       84 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15900 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py
--rw-r--r--   0 runner    (1001) docker     (116)     7721 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py
--rw-r--r--   0 runner    (1001) docker     (116)     7562 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4331 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py
--rw-r--r--   0 runner    (1001) docker     (116)     8466 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py
--rw-r--r--   0 runner    (1001) docker     (116)    11727 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (116)    19861 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py
--rw-r--r--   0 runner    (1001) docker     (116)     9142 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/simple_blowout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/tracking/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      862 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/tracking/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (116)     9874 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/tracking/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-10 15:09:06.000000 Wake-T-0.6.0/wake_t/utilities/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10986 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/utilities/bunch_generation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2272 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/utilities/bunch_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1597 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/utilities/bunch_saving.py
--rw-r--r--   0 runner    (1001) docker     (116)      637 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/utilities/numba.py
--rw-r--r--   0 runner    (1001) docker     (116)     2770 2023-03-10 15:08:57.000000 Wake-T-0.6.0/wake_t/utilities/other.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 08:57:59.000000 Wake-T-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-16 08:58:08.000000 Wake-T-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-16 08:57:59.000000 Wake-T-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/Wake_T.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-16 08:58:08.000000 Wake-T-0.6.2/Wake_T.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 08:58:08.000000 Wake-T-0.6.2/Wake_T.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:58:08.000000 Wake-T-0.6.2/Wake_T.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 08:58:08.000000 Wake-T-0.6.2/Wake_T.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 08:58:08.000000 Wake-T-0.6.2/Wake_T.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 08:57:59.000000 Wake-T-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-16 08:58:08.000000 Wake-T-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 08:57:59.000000 Wake-T-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_active_plasma_lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_beam_deposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_beamline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_bunch_read_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_custom_blowout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_field_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_field_gathering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_fluid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_laser_envelope_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_laser_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_multibunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_no_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_openpmd_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_parabolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_particle_bunch_species.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_plasma_beamline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_plasma_deposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_ramps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_sc_baxevanis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-16 08:57:59.000000 Wake-T-0.6.2/tests/test_simple_blowout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/beamline_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/active_plasma_lens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/beamline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/field_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/plasma_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/plasma_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/beamline_elements/tm_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/diagnostics/bunch_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/diagnostics/openpmd_diag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/analytical_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/numerical_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/fields/rz_wakefield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/particles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/deposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/particle_bunch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/particles/push/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/push/boris_pusher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/push/runge_kutta_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/particles/push/transfer_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/beam_optics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/beam_optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/beam_optics/transfer_matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/collective_effects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/collective_effects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/collective_effects/csr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/em_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/em_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/em_fields/linear_b_theta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/laser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/laser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/laser/envelope_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/laser/envelope_solver_non_centered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/laser/laser_pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/laser/tdma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/custom_blowout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/focusing_blowout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/from_pic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/simple_blowout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/tracking/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/tracking/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:58:08.000000 Wake-T-0.6.2/wake_t/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/utilities/bunch_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/utilities/bunch_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/utilities/bunch_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/utilities/numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-16 08:57:59.000000 Wake-T-0.6.2/wake_t/utilities/other.py
```

### Comparing `Wake-T-0.6.0/LICENSE` & `Wake-T-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/PKG-INFO` & `Wake-T-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wake-T
-Version: 0.6.0
+Version: 0.6.2
 Summary: A fast particle tracking code for plasma accelerators.
 Home-page: https://github.com/AngelFP/Wake-T
 Author: Angel Ferran Pousa
 Author-email: angel.ferran.pousa@desy.de,
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Wake-T-0.6.0/README.md` & `Wake-T-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/Wake_T.egg-info/PKG-INFO` & `Wake-T-0.6.2/Wake_T.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wake-T
-Version: 0.6.0
+Version: 0.6.2
 Summary: A fast particle tracking code for plasma accelerators.
 Home-page: https://github.com/AngelFP/Wake-T
 Author: Angel Ferran Pousa
 Author-email: angel.ferran.pousa@desy.de,
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Wake-T-0.6.0/Wake_T.egg-info/SOURCES.txt` & `Wake-T-0.6.2/Wake_T.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/setup.cfg` & `Wake-T-0.6.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 install_requires = 
 	numpy
-	numba
+	numba<0.57
 	scipy
 	aptools~=0.2.0
-	openpmd-api~=0.14.0
+	openpmd-api
 	tqdm
 python_requires = >=3.7
 
 [options.extras_require]
 test = 
 	pytest
 	flake8
```

### Comparing `Wake-T-0.6.0/tests/test_active_plasma_lens.py` & `Wake-T-0.6.2/tests/test_active_plasma_lens.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_beam_deposition.py` & `Wake-T-0.6.2/tests/test_beam_deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_beamline.py` & `Wake-T-0.6.2/tests/test_beamline.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_bunch_read_save.py` & `Wake-T-0.6.2/tests/test_bunch_read_save.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_custom_blowout.py` & `Wake-T-0.6.2/tests/test_custom_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_field_element.py` & `Wake-T-0.6.2/tests/test_field_element.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_field_gathering.py` & `Wake-T-0.6.2/tests/test_field_gathering.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_fluid_model.py` & `Wake-T-0.6.2/tests/test_fluid_model.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_interpolation.py` & `Wake-T-0.6.2/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_laser_envelope_model.py` & `Wake-T-0.6.2/tests/test_laser_envelope_model.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_laser_initialization.py` & `Wake-T-0.6.2/tests/test_laser_initialization.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_multibunch.py` & `Wake-T-0.6.2/tests/test_multibunch.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_no_bunch.py` & `Wake-T-0.6.2/tests/test_no_bunch.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_openpmd_viewer.py` & `Wake-T-0.6.2/tests/test_openpmd_viewer.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_parabolic_profile.py` & `Wake-T-0.6.2/tests/test_parabolic_profile.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_particle_bunch_species.py` & `Wake-T-0.6.2/tests/test_particle_bunch_species.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_plasma_beamline.py` & `Wake-T-0.6.2/tests/test_plasma_beamline.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_plasma_deposition.py` & `Wake-T-0.6.2/tests/test_plasma_deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_ramps.py` & `Wake-T-0.6.2/tests/test_ramps.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_sc_baxevanis.py` & `Wake-T-0.6.2/tests/test_sc_baxevanis.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/tests/test_simple_blowout.py` & `Wake-T-0.6.2/tests/test_simple_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/__init__.py` & `Wake-T-0.6.2/wake_t/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.6.0'
+__version__ = '0.6.2'
 
 
 from .beamline_elements import (PlasmaStage, PlasmaRamp, ActivePlasmaLens,
                                 Drift, Dipole, Quadrupole, Sextupole, Beamline)
 from .physics_models.collective_effects.csr import set_csr_settings
 from .physics_models.laser.laser_pulse import (
     GaussianPulse, LaguerreGaussPulse, FlattenedGaussianPulse)
```

### Comparing `Wake-T-0.6.0/wake_t/beamline_elements/active_plasma_lens.py` & `Wake-T-0.6.2/wake_t/beamline_elements/active_plasma_lens.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/beamline_elements/beamline.py` & `Wake-T-0.6.2/wake_t/beamline_elements/beamline.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/beamline_elements/field_element.py` & `Wake-T-0.6.2/wake_t/beamline_elements/field_element.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/beamline_elements/plasma_ramp.py` & `Wake-T-0.6.2/wake_t/beamline_elements/plasma_ramp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """
 This module contains the definition of the PlasmaRamp class as well as
 predefined ramp profiles.
 
 """
 
-from typing import Optional, Union
+from typing import Optional, Union, Callable
 from functools import partial
 
 import numpy as np
 
 from wake_t.beamline_elements import PlasmaStage
 
 
+# Define type alias for the ramp profiles.
+Profile = Callable[[float, float, float, float, float], float]
+
+
 def inverse_square_profile(z, decay_length=None, density_top=None,
                            density_down=None, position_down=None):
     if decay_length is None:
         decay_length = position_down / (np.sqrt(density_top/density_down) - 1)
     return density_top / np.square(1 + z/decay_length)
 
 
@@ -53,15 +57,16 @@
     ----------
     length : float
         Length of the plasma ramp in m.
     profile : string or callable
         Longitudinal density profile of the ramp. Possible string values
         are ``'gaussian'``, ``'inverse square'`` and ``'exponential'``.
         A callable might also be provided as a function of the form
-        ``'def func(z)'`` that returns the density value at the given
+        ``'def func(z, decay_length, density_top, density_down,
+        position_down)'`` that returns the density value at the given
         position ``z``.
     ramp_type : string
         Possible types are ``'upramp'`` and ``'downramp'``.
     wakefield_model : str
         Wakefield model to be used. Possible values are ``'blowout'``,
         ``'custom_blowout'``, ``'focusing_blowout'``, ``'cold_fluid_1d'`` and
         ``'quasistatic_2d'``.
@@ -105,15 +110,15 @@
     PlasmaStage
 
     """
 
     def __init__(
         self,
         length: float,
-        profile: Optional[str] = 'inverse_square',
+        profile: Optional[Union[str, Profile]] = 'inverse_square',
         ramp_type: Optional[str] = 'upramp',
         wakefield_model: Optional[str] = 'focusing_blowout',
         decay_length: Optional[float] = None,
         plasma_dens_top: Optional[float] = None,
         plasma_dens_down: Optional[float] = None,
         position_down: Optional[float] = None,
         bunch_pusher: Optional[str] = 'rk4',
@@ -124,22 +129,22 @@
     ) -> None:
         self.ramp_type = ramp_type
         if position_down is None:
             position_down = length
         # If a function profile is not provided, generate from presets.
         if not callable(profile):
             if profile in ramp_profiles:
-                ramp_profile = ramp_profiles[profile]
-                profile = partial(
-                    ramp_profile, decay_length=decay_length,
-                    density_top=plasma_dens_top, density_down=plasma_dens_down,
-                    position_down=position_down)
+                profile = ramp_profiles[profile]
             else:
                 raise ValueError(
                     'Ramp profile "{}" not recognized'.format(profile))
+        profile = partial(
+            profile, decay_length=decay_length,
+            density_top=plasma_dens_top, density_down=plasma_dens_down,
+            position_down=position_down)
         self.profile = profile
         super().__init__(
             length=length,
             density=self.ramp_profile,
             wakefield_model=wakefield_model,
             bunch_pusher=bunch_pusher,
             dt_bunch=dt_bunch,
```

### Comparing `Wake-T-0.6.0/wake_t/beamline_elements/plasma_stage.py` & `Wake-T-0.6.2/wake_t/beamline_elements/plasma_stage.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/beamline_elements/tm_elements.py` & `Wake-T-0.6.2/wake_t/beamline_elements/tm_elements.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/diagnostics/bunch_analysis.py` & `Wake-T-0.6.2/wake_t/diagnostics/bunch_analysis.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/diagnostics/openpmd_diag.py` & `Wake-T-0.6.2/wake_t/diagnostics/openpmd_diag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 This module contains the OpenPMDDiagnostics class, which generates the
 openPMD output.
 """
 import os
 from typing import Optional, List
-from copy import deepcopy
 
 import numpy as np
 import scipy.constants as ct
 from openpmd_api import (Series, Access, Dataset, Mesh_Record_Component,
                          Unit_Dimension, Geometry)
 
 from wake_t import __version__
@@ -303,17 +302,15 @@
             # properly defined in the openPMD standard.
             fld.geometry = Geometry.thetaMode  # Geometry.cylindrical
             fld.set_attribute('fieldSmoothing', 'none')
             for attr, val in wf_data[field]['attributes'].items():
                 fld.set_attribute(attr, val)
             fld.axis_labels = wf_data[field]['grid']['labels']
             fld.grid_spacing = wf_data[field]['grid']['spacing']
-            global_offset = deepcopy(wf_data[field]['grid']['global_offset'])
-            global_offset[-1] += self._current_z_pos
-            fld.grid_global_offset = global_offset
+            fld.grid_global_offset = wf_data[field]['grid']['global_offset']
 
     def check_species_names(
         self,
         species_list: Optional[List[ParticleBunch]] = []
     ) -> None:
         """ Check that no species have duplicate names. """
         sp_names = []
```

### Comparing `Wake-T-0.6.0/wake_t/fields/analytical_field.py` & `Wake-T-0.6.2/wake_t/fields/analytical_field.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/fields/base.py` & `Wake-T-0.6.2/wake_t/fields/base.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/fields/gather.py` & `Wake-T-0.6.2/wake_t/fields/gather.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/fields/interpolation.py` & `Wake-T-0.6.2/wake_t/fields/interpolation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/fields/numerical_field.py` & `Wake-T-0.6.2/wake_t/fields/numerical_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         bunches: List[ParticleBunch]
     ) -> None:
         """Update field to the next time step.
 
         Parameters
         ----------
         bunches : list
-            List of ``ParticleBunch``es that can be used to recompute/update
+            List of ``ParticleBunch`` that can be used to recompute/update
             the fields.
         """
         if not self.initialized:
             self.initialize_properties(bunches)
         else:
             self.evolve_properties(bunches)
         self.calculate_field(bunches)
```

### Comparing `Wake-T-0.6.0/wake_t/fields/rz_wakefield.py` & `Wake-T-0.6.2/wake_t/fields/rz_wakefield.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/particles/deposition.py` & `Wake-T-0.6.2/wake_t/particles/deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/particles/interpolation.py` & `Wake-T-0.6.2/wake_t/particles/interpolation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/particles/particle_bunch.py` & `Wake-T-0.6.2/wake_t/particles/particle_bunch.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/particles/push/boris_pusher.py` & `Wake-T-0.6.2/wake_t/particles/push/boris_pusher.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/particles/push/runge_kutta_4.py` & `Wake-T-0.6.2/wake_t/particles/push/runge_kutta_4.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/particles/push/transfer_matrix.py` & `Wake-T-0.6.2/wake_t/particles/push/transfer_matrix.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/beam_optics/transfer_matrices.py` & `Wake-T-0.6.2/wake_t/physics_models/beam_optics/transfer_matrices.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/collective_effects/csr.py` & `Wake-T-0.6.2/wake_t/physics_models/collective_effects/csr.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/em_fields/linear_b_theta.py` & `Wake-T-0.6.2/wake_t/physics_models/em_fields/linear_b_theta.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/laser/envelope_solver.py` & `Wake-T-0.6.2/wake_t/physics_models/laser/envelope_solver.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/laser/envelope_solver_non_centered.py` & `Wake-T-0.6.2/wake_t/physics_models/laser/envelope_solver_non_centered.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/laser/laser_pulse.py` & `Wake-T-0.6.2/wake_t/physics_models/laser/laser_pulse.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,21 +111,33 @@
             'rmax': r_max,
             'nz': subgrid_nz if self.use_subgrid else nz,
             'nr': subgrid_nr if self.use_subgrid else nr,
             'nt': nt,
             'dt': dt / nt,
             'use_phase': use_phase
         }
-        if self.a_env is not None and solver_params != self.solver_params:
-            raise ValueError(
-                'Solver parameters cannot be changed once envelope has been '
-                'initialized.'
-            )
-        else:
-            self.solver_params = solver_params
+        # Check if laser pulse has already been initialized.
+        if self.n_steps > 0:
+            # Check that grid parameters have not changed.
+            if (
+                solver_params['zmin'] != self.solver_params['zmin'] and
+                solver_params['zmax'] != self.solver_params['zmax'] and
+                solver_params['rmax'] != self.solver_params['rmax'] and
+                solver_params['nz'] != self.solver_params['nz'] and
+                solver_params['nr'] != self.solver_params['nr']
+            ):
+                raise ValueError(
+                    'Laser envelope grid parameters cannot be changed once '
+                    'envelope has been initialized.'
+                )
+            # If time step has changed, set `n_steps` to 0 so that the
+            # non-centered envelope solver is used for the next step.
+            if solver_params['dt'] != self.solver_params['dt']:
+                self.n_steps = 0
+        self.solver_params = solver_params
 
     def initialize_envelope(self) -> None:
         """Initialize laser envelope arrays."""
         if self.solver_params is None:
             raise ValueError(
                 'Envelope solver parameters not yet set.'
                 'Cannot initialize envelope.')
```

### Comparing `Wake-T-0.6.0/wake_t/physics_models/laser/tdma.py` & `Wake-T-0.6.2/wake_t/physics_models/laser/tdma.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/custom_blowout.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/custom_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/focusing_blowout.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/focusing_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/from_pic.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/from_pic.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_cold_fluid_1x3p.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/b_theta.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/deposition.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_particles.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/ab5.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/plasma_push/rk4.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/psi_and_derivatives.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/solver.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/qs_rz_baxevanis/wakefield.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/physics_models/plasma_wakefields/simple_blowout.py` & `Wake-T-0.6.2/wake_t/physics_models/plasma_wakefields/simple_blowout.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/tracking/progress_bar.py` & `Wake-T-0.6.2/wake_t/tracking/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/tracking/tracker.py` & `Wake-T-0.6.2/wake_t/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/utilities/bunch_generation.py` & `Wake-T-0.6.2/wake_t/utilities/bunch_generation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/utilities/bunch_manipulation.py` & `Wake-T-0.6.2/wake_t/utilities/bunch_manipulation.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/utilities/bunch_saving.py` & `Wake-T-0.6.2/wake_t/utilities/bunch_saving.py`

 * *Files identical despite different names*

### Comparing `Wake-T-0.6.0/wake_t/utilities/other.py` & `Wake-T-0.6.2/wake_t/utilities/other.py`

 * *Files identical despite different names*

