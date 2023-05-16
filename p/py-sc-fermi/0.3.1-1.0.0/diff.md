# Comparing `tmp/py-sc-fermi-0.3.1.tar.gz` & `tmp/py-sc-fermi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sc-fermi-0.3.1.tar", last modified: Mon Nov  7 10:39:08 2022, max compression
+gzip compressed data, was "py-sc-fermi-1.0.0.tar", last modified: Wed Jan 25 09:08:03 2023, max compression
```

## Comparing `py-sc-fermi-0.3.1.tar` & `py-sc-fermi-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-07 10:39:08.155930 py-sc-fermi-0.3.1/
--rw-r--r--   0 alex       (501) staff       (20)     1085 2022-05-26 12:13:56.000000 py-sc-fermi-0.3.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     2209 2022-11-07 10:39:08.155652 py-sc-fermi-0.3.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1809 2022-10-17 13:05:23.000000 py-sc-fermi-0.3.1/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-07 10:39:08.154098 py-sc-fermi-0.3.1/py_sc_fermi/
--rw-r--r--   0 alex       (501) staff       (20)       22 2022-11-02 17:21:51.000000 py-sc-fermi-0.3.1/py_sc_fermi/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-07 10:39:08.155281 py-sc-fermi-0.3.1/py_sc_fermi/cli/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-05-26 12:13:56.000000 py-sc-fermi-0.3.1/py_sc_fermi/cli/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2358 2022-11-02 17:21:37.000000 py-sc-fermi-0.3.1/py_sc_fermi/cli/sc_fermi_solve.py
--rw-r--r--   0 alex       (501) staff       (20)     6440 2022-11-01 14:30:02.000000 py-sc-fermi-0.3.1/py_sc_fermi/defect_charge_state.py
--rw-r--r--   0 alex       (501) staff       (20)    15695 2022-11-01 14:30:02.000000 py-sc-fermi-0.3.1/py_sc_fermi/defect_species.py
--rw-r--r--   0 alex       (501) staff       (20)    13262 2022-11-02 17:24:25.000000 py-sc-fermi-0.3.1/py_sc_fermi/defect_system.py
--rw-r--r--   0 alex       (501) staff       (20)     7983 2022-11-01 14:30:02.000000 py-sc-fermi-0.3.1/py_sc_fermi/dos.py
--rw-r--r--   0 alex       (501) staff       (20)    12208 2022-11-02 17:18:38.000000 py-sc-fermi-0.3.1/py_sc_fermi/inputs.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2022-11-07 10:39:08.155086 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     2209 2022-11-07 10:39:08.000000 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      459 2022-11-07 10:39:08.000000 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2022-11-07 10:39:08.000000 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       71 2022-11-07 10:39:08.000000 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       28 2022-11-07 10:39:08.000000 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2022-11-07 10:39:08.000000 py-sc-fermi-0.3.1/py_sc_fermi.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2022-11-07 10:39:08.155994 py-sc-fermi-0.3.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      895 2022-10-17 17:16:36.000000 py-sc-fermi-0.3.1/setup.py
+drwxr-xr-x   0 bjm42      (501) staff       (20)        0 2023-01-25 09:08:03.771757 py-sc-fermi-1.0.0/
+-rw-r--r--   0 bjm42      (501) staff       (20)     1085 2022-05-03 21:31:12.000000 py-sc-fermi-1.0.0/LICENSE
+-rw-r--r--   0 bjm42      (501) staff       (20)     3924 2023-01-25 09:08:03.771333 py-sc-fermi-1.0.0/PKG-INFO
+-rw-r--r--   0 bjm42      (501) staff       (20)     3524 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/README.md
+drwxr-xr-x   0 bjm42      (501) staff       (20)        0 2023-01-25 09:08:03.755858 py-sc-fermi-1.0.0/py_sc_fermi/
+-rw-r--r--   0 bjm42      (501) staff       (20)       22 2023-01-25 08:46:37.000000 py-sc-fermi-1.0.0/py_sc_fermi/__init__.py
+drwxr-xr-x   0 bjm42      (501) staff       (20)        0 2023-01-25 09:08:03.770467 py-sc-fermi-1.0.0/py_sc_fermi/cli/
+-rw-r--r--   0 bjm42      (501) staff       (20)        0 2022-05-03 21:31:12.000000 py-sc-fermi-1.0.0/py_sc_fermi/cli/__init__.py
+-rw-r--r--   0 bjm42      (501) staff       (20)     2358 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/py_sc_fermi/cli/sc_fermi_solve.py
+-rw-r--r--   0 bjm42      (501) staff       (20)     6460 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/py_sc_fermi/defect_charge_state.py
+-rw-r--r--   0 bjm42      (501) staff       (20)    15677 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/py_sc_fermi/defect_species.py
+-rw-r--r--   0 bjm42      (501) staff       (20)    13995 2023-01-25 08:19:49.000000 py-sc-fermi-1.0.0/py_sc_fermi/defect_system.py
+-rw-r--r--   0 bjm42      (501) staff       (20)     7773 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/py_sc_fermi/dos.py
+-rw-r--r--   0 bjm42      (501) staff       (20)    12210 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/py_sc_fermi/inputs.py
+drwxr-xr-x   0 bjm42      (501) staff       (20)        0 2023-01-25 09:08:03.765668 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/
+-rw-r--r--   0 bjm42      (501) staff       (20)     3924 2023-01-25 09:08:03.000000 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/PKG-INFO
+-rw-r--r--   0 bjm42      (501) staff       (20)      459 2023-01-25 09:08:03.000000 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/SOURCES.txt
+-rw-r--r--   0 bjm42      (501) staff       (20)        1 2023-01-25 09:08:03.000000 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/dependency_links.txt
+-rw-r--r--   0 bjm42      (501) staff       (20)       71 2023-01-25 09:08:03.000000 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/entry_points.txt
+-rw-r--r--   0 bjm42      (501) staff       (20)       28 2023-01-25 09:08:03.000000 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/requires.txt
+-rw-r--r--   0 bjm42      (501) staff       (20)       12 2023-01-25 09:08:03.000000 py-sc-fermi-1.0.0/py_sc_fermi.egg-info/top_level.txt
+-rw-r--r--   0 bjm42      (501) staff       (20)       38 2023-01-25 09:08:03.771849 py-sc-fermi-1.0.0/setup.cfg
+-rw-r--r--   0 bjm42      (501) staff       (20)      895 2023-01-22 13:32:18.000000 py-sc-fermi-1.0.0/setup.py
```

### Comparing `py-sc-fermi-0.3.1/LICENSE` & `py-sc-fermi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-sc-fermi-0.3.1/py_sc_fermi/cli/sc_fermi_solve.py` & `py-sc-fermi-1.0.0/py_sc_fermi/cli/sc_fermi_solve.py`

 * *Files identical despite different names*

### Comparing `py-sc-fermi-0.3.1/py_sc_fermi/defect_charge_state.py` & `py-sc-fermi-1.0.0/py_sc_fermi/defect_charge_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
          fixed_concentration (float): fixed concentration per unit cell
     """
 
     def __init__(
         self,
         charge: int,
         degeneracy: int = 1,
-        energy: float = None,
-        fixed_concentration: float = None,
+        energy: Optional[float] = None,
+        fixed_concentration: Optional[float] = None,
     ):
         if energy == None and fixed_concentration == None:
             raise ValueError(
                 """You must specify either a fixed concentration or energy for 
                 this defect! \n Note, if you specify both, the concentration
                 will treated as fixed"""
             )
```

### Comparing `py-sc-fermi-0.3.1/py_sc_fermi/defect_species.py` & `py-sc-fermi-1.0.0/py_sc_fermi/defect_species.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
 
     def __init__(
         self,
         name: str,
         nsites: int,
         charge_states: Dict[int, DefectChargeState],
-        fixed_concentration: float = None,
+        fixed_concentration: Optional[float] = None,
     ):
         """Instantiate a DefectSpecies object."""
 
         self._name = name
         self._nsites = nsites
         self._charge_states = charge_states
         self._fixed_concentration = fixed_concentration
@@ -54,17 +54,15 @@
 
         Returns:
             int: site degeneracy fot ``DefectSpecies``
         """
         return self._nsites
 
     @property
-    def charge_states(
-        self,
-    ) -> Dict[int, DefectChargeState]:
+    def charge_states(self,) -> Dict[int, DefectChargeState]:
         """
 
         Returns:
             Dict[int, DefectChargeState]: The charge states of this defect species as s dictionary of
             ``{charge (int): DefectChargeState}`` key-value pairs"""
         return self._charge_states
 
@@ -309,17 +307,15 @@
             will be returned.
         """
         if self.fixed_concentration:
             return self.fixed_concentration
         else:
             return sum(self.charge_state_concentrations(e_fermi, temperature).values())
 
-    def fixed_conc_charge_states(
-        self,
-    ) -> Dict[int, DefectChargeState]:
+    def fixed_conc_charge_states(self,) -> Dict[int, DefectChargeState]:
         """get ``DefectChargeState`` objects of this ``DefectSpecies`` with fixed
         concentration (i.e those for which ``DefectChargeState.fixed_concentration != None``)
 
         Returns:
             Dict[int, DefectChargeState]: key-value pairs of charge on fixed
             concentration ``DefectChargeState`` objects, and the charge state
             which is variable, i.e. ``{DefectChargeState.charge : DefectChargeState}``
```

### Comparing `py-sc-fermi-0.3.1/py_sc_fermi/defect_system.py` & `py-sc-fermi-1.0.0/py_sc_fermi/defect_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,14 @@
         """
         # initial guess
         emin = self.dos.emin()
         emax = self.dos.emax()
         direction = +1.0
         e_fermi = (emin + emax) / 2.0
         step = 1.0
-        converged = False
         reached_e_min = False
         reached_e_max = False
 
         # loop until convergence or max number of steps reached
         for i in range(self.n_trial_steps):
             q_tot = self.q_tot(e_fermi=e_fermi)
             if e_fermi > emax:
@@ -163,15 +162,14 @@
                 direction = -1.0
             if e_fermi < emin:
                 if reached_e_max or reached_e_min:
                     raise RuntimeError(f"No solution found between {emin} and {emax}")
                 reached_e_min = True
                 direction = +1.0
             if abs(q_tot) < self.convergence_tolerance:
-                converged = True
                 break
             if q_tot > 0.0:
                 if direction == +1.0:
                     step *= 0.25
                     direction = -1.0
             elif q_tot < 0.0:
                 if direction == -1.0:
@@ -188,23 +186,24 @@
         which summarises key properties of the defect system."""
         print(self._get_report_string())
 
     def _get_report_string(self) -> str:
         """generate string to facilitate self.report()"""
         string = ""
         e_fermi = self.get_sc_fermi()[0]
+        string += f"Temperature :      {self.temperature}  (K)\n"
         string += f"SC Fermi level :      {e_fermi}  (eV)\n"
         p0, n0 = self.dos.carrier_concentrations(e_fermi, self.temperature)
         string += "Concentrations:\n"
         string += f"n (electrons)  : {n0 * 1e24 / self.volume} cm^-3\n"
         string += f"p (holes)      : {p0 * 1e24 / self.volume} cm^-3\n"
         for ds in self.defect_species:
             concall = ds.get_concentration(e_fermi, self.temperature)
             if ds.fixed_concentration == None:
-                string += f"{ds.name:9}      : {concall * 1e24 / self.volume} cm^-3\n"
+                string += f"{ds.name:9}      : {concall * 1e24 / self.volume} cm^-3, (percentage of defective sites: {(concall / ds.nsites) * 100:.3} %)\n"
             else:
                 string += (
                     f"{ds.name:9}      : {concall * 1e24 / self.volume} cm^-3 [fixed]\n"
                 )
         string += "\nBreakdown of concentrations for each defect charge state:\n"
         for ds in self.defect_species:
             concall = ds.get_concentration(e_fermi, self.temperature)
@@ -281,17 +280,15 @@
             )
             x = [[x_value][0][0] for x_value in transition_level]
             y = [[y_value][0][1] for y_value in transition_level]
             transition_levels.update({defect_species: [x, y]})
         return transition_levels
 
     def as_dict(
-        self,
-        decomposed: bool = False,
-        per_volume: bool = True,
+        self, decomposed: bool = False, per_volume: bool = True,
     ) -> Dict[str, Any]:
         """Returns a dictionary of the properties of the ``DefectSystem`` object
         after solving for the self-consistent Fermi energy.
 
         Args:
             decomposed (bool, optional): if True, return a dictionary in which the
               concentration of each ``DefectChargeState`` is given explicitly,
@@ -333,7 +330,29 @@
                         * scale
                     )
                     for q in ds.charge_states
                 }
                 for ds in self.defect_species
             }
             return {**run_stats, **decomp_concs}
+
+    def site_percentages(
+        self, 
+    ) -> Dict[str, float]:
+        """Returns a dictionary of the DefectSpecies in the DefectSystem which
+        giving the percentage of the sites in the structure that will host that 
+        defect.
+
+        Returns:
+            Dict[str, Any]: dictionary specifying the per-DefectSpecies site
+            concentrations.
+        """
+
+        e_fermi = self.get_sc_fermi()[0]
+
+        sum_concs = {
+                str(ds.name): float(
+                    (ds.get_concentration(e_fermi, self.temperature) / ds.nsites) * 100
+                )
+                for ds in self.defect_species
+            }
+        return sum_concs
```

### Comparing `py-sc-fermi-0.3.1/py_sc_fermi/dos.py` & `py-sc-fermi-1.0.0/py_sc_fermi/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,26 @@
         dos: np.ndarray,
         edos: np.ndarray,
         bandgap: float,
         nelect: int,
         spin_polarised=False,
     ):
         """Initialise a ``DOS`` instance."""
-        self._dos = dos
+        # self._dos = dos
         self._edos = edos
         self._bandgap = bandgap
         self._nelect = nelect
         self._spin_polarised = spin_polarised
+
+        if self.spin_polarised == True:
+            new_dos = np.sum(dos, axis=0)
+            self._dos = new_dos
+        elif self.spin_polarised == False:
+            self._dos = dos
+
         self.normalise_dos()
 
         if self.bandgap > self.emax():
             raise ValueError(
                 """bandgap > max(self.edos). Please check your bandgap and
                  energy range (self.edos)."""
             )
@@ -102,23 +109,20 @@
             bandgap (Optional[float], optional): bandgap. Defaults to None.
         """
         vr = Vasprun(path_to_vasprun, parse_potcar_file=False)
         densities = vr.complete_dos.densities
         vbm = vr.eigenvalue_band_properties[2]
         edos = vr.complete_dos.energies - vbm
         if len(densities) == 2:
-            tdos_data = np.stack(
-                [edos, np.abs(densities[Spin.up]), np.abs(densities[Spin.down])], axis=1
-            )
+            dos = np.array([densities[Spin.up], densities[Spin.down]])
             spin_pol = True
         else:
-            tdos_data = np.stack([edos, np.abs(densities[Spin.up])], axis=1)
+            dos = np.array(densities[Spin.up])
             spin_pol = False
-        edos = tdos_data[:, 0]
-        dos = np.sum(tdos_data[:, 1:], axis=1)
+
         if bandgap is None:
             bandgap = float(vr.eigenvalue_band_properties[0])
         return cls(
             dos=dos, edos=edos, nelect=nelect, bandgap=bandgap, spin_polarised=spin_pol
         )
 
     @classmethod
@@ -133,31 +137,25 @@
 
         Raises:
             ValueError: raises error if density-of-states data not formatted
               correctly with respect to ``self.spin_polarised`` setting.
         """
         nelect = dos_dict["nelect"]
         bandgap = dos_dict["bandgap"]
-        raw_dos = np.array(dos_dict["dos"])
+        dos = np.array(dos_dict["dos"])
         edos = np.array(dos_dict["edos"])
-        shape = raw_dos.shape
+
+        shape = dos.shape
         if len(shape) == 1:
-            new_dos = raw_dos
             spin_pol = False
         elif shape[0] == 2:
-            new_dos = np.sum(raw_dos, axis=0)
             spin_pol = True
-        else:
-            raise ValueError("dos_dict['dos'] is not in the correct format.")
+
         return cls(
-            nelect=nelect,
-            bandgap=bandgap,
-            edos=edos,
-            dos=new_dos,
-            spin_polarised=spin_pol,
+            nelect=nelect, bandgap=bandgap, edos=edos, dos=dos, spin_polarised=spin_pol,
         )
 
     def sum_dos(self) -> np.ndarray:
         """
         Returns:
             np.ndarray: integrated density-of-states up to the valence band maximum
         """
```

### Comparing `py-sc-fermi-0.3.1/py_sc_fermi/inputs.py` & `py-sc-fermi-1.0.0/py_sc_fermi/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from collections import namedtuple
 from dataclasses import dataclass
 import numpy as np
 from py_sc_fermi.defect_species import DefectSpecies
 from py_sc_fermi.defect_charge_state import DefectChargeState
 from py_sc_fermi.dos import DOS
 from pymatgen.core import Structure
-from typing import List
+from typing import Optional, List
 import yaml
 import os
 
 InputFermiData = namedtuple(
-    "InputFermiData",
-    "spin_pol nelect bandgap temperature defect_species",
+    "InputFermiData", "spin_pol nelect bandgap temperature defect_species",
 )
 
 
 @dataclass
 class InputSet:
     dos: DOS
     volume: float
@@ -198,15 +197,15 @@
     lattvec = np.array([[float(s) for s in l.split()] for l in readin[1:4]], order="F")
     lattvec *= factor
     volume = np.linalg.det(lattvec)
     return volume
 
 
 def read_input_fermi(
-    filename: str, volume: float = None, frozen: bool = False
+    filename: str, volume: Optional[float] = None, frozen: bool = False
 ) -> InputFermiData:
     """Return all information from a input file correctly formatted to work
     for `SC-Fermi <https://github.com/jbuckeridge/sc-fermi>`_.
 
     Args:
         filename (str): path to ``SC-Fermi`` -formatted input file.
         volume (float, optional): unit cell volume. Only required if there are
@@ -281,19 +280,15 @@
                 defect_species.append(
                     DefectSpecies(name, 1, {charge_state: defect_charge_state})
                 )
 
     return InputFermiData(spin_pol, nelect, bandgap, temperature, defect_species)
 
 
-def read_dos_data(
-    bandgap: float,
-    nelect: int,
-    filename: str = "totdos.dat",
-) -> DOS:
+def read_dos_data(bandgap: float, nelect: int, filename: str = "totdos.dat",) -> DOS:
     """read density of states data from an `SC-Fermi <https://github.com/jbuckeridge/sc-fermi>`_
     formatted ``totdos.dat`` file.
 
     Args:
         bandgap (float): bandgap of density-of-states data.
         nelect (int): number of electrons in the density-of-states data
         filename (str, optional): path to ``todos.dat`` file. Defaults to "totdos.dat".
```

### Comparing `py-sc-fermi-0.3.1/setup.py` & `py-sc-fermi-1.0.0/setup.py`

 * *Files identical despite different names*

