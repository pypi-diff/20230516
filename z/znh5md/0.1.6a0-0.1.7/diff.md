# Comparing `tmp/znh5md-0.1.6a0.tar.gz` & `tmp/znh5md-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znh5md-0.1.6a0.tar", max compression
+gzip compressed data, was "znh5md-0.1.7.tar", max compression
```

## Comparing `znh5md-0.1.6a0.tar` & `znh5md-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0    13575 2023-02-10 13:53:08.586838 znh5md-0.1.6a0/LICENSE
--rw-r--r--   0        0        0     2613 2023-03-28 13:29:46.018406 znh5md-0.1.6a0/README.md
--rw-r--r--   0        0        0     1083 2023-04-03 14:36:35.844540 znh5md-0.1.6a0/pyproject.toml
--rw-r--r--   0        0        0      299 2023-03-26 12:05:45.098922 znh5md-0.1.6a0/znh5md/__init__.py
--rw-r--r--   0        0        0     1404 2023-04-03 11:34:58.022893 znh5md-0.1.6a0/znh5md/cli.py
--rw-r--r--   0        0        0     3589 2023-04-03 13:19:42.924739 znh5md-0.1.6a0/znh5md/format/__init__.py
--rw-r--r--   0        0        0      249 2023-03-26 13:37:32.418733 znh5md-0.1.6a0/znh5md/io/__init__.py
--rw-r--r--   0        0        0     9426 2023-04-03 11:34:58.032893 znh5md-0.1.6a0/znh5md/io/base.py
--rw-r--r--   0        0        0     7142 2023-04-03 11:34:58.032893 znh5md-0.1.6a0/znh5md/io/reader.py
--rw-r--r--   0        0        0      179 2023-03-26 12:05:45.108922 znh5md-0.1.6a0/znh5md/utils.py
--rw-r--r--   0        0        0     9109 2023-04-03 14:33:48.496359 znh5md-0.1.6a0/znh5md/znh5md/__init__.py
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 znh5md-0.1.6a0/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-05-16 13:50:54.924529 znh5md-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3004 2023-05-16 13:50:54.934529 znh5md-0.1.7/README.md
+-rw-r--r--   0        0        0     1189 2023-05-16 13:50:54.934529 znh5md-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-05-16 13:50:54.934529 znh5md-0.1.7/znh5md/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-16 13:00:33.797385 znh5md-0.1.7/znh5md/cli.py
+-rw-r--r--   0        0        0     3638 2023-05-16 13:00:33.807385 znh5md-0.1.7/znh5md/format/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-16 13:50:54.934529 znh5md-0.1.7/znh5md/io/__init__.py
+-rw-r--r--   0        0        0     9759 2023-05-16 13:50:54.934529 znh5md-0.1.7/znh5md/io/base.py
+-rw-r--r--   0        0        0    11166 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/io/reader.py
+-rw-r--r--   0        0        0      179 2023-03-26 12:05:45.108922 znh5md-0.1.7/znh5md/utils.py
+-rw-r--r--   0        0        0      268 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/base.py
+-rw-r--r--   0        0        0     4402 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/h5ase.py
+-rw-r--r--   0        0        0     7393 2023-05-16 13:50:54.944529 znh5md-0.1.7/znh5md/znh5md/h5dask.py
+-rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 znh5md-0.1.7/PKG-INFO
```

### Comparing `znh5md-0.1.6a0/LICENSE` & `znh5md-0.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -244,8 +244,8 @@
    (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
    SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 CONTRIBUTION AGREEMENT
 
 By contributing to the BVLC/caffe repository through pull-request, comment,
 or otherwise, the contributor releases their content to the
-license and copyright terms herein.
+license and copyright terms herein.
```

### Comparing `znh5md-0.1.6a0/README.md` & `znh5md-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnH5MD/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnH5MD?branch=main)
 [![PyPI version](https://badge.fury.io/py/znh5md.svg)](https://badge.fury.io/py/znh5md)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnH5MD/HEAD)
 
 # ZnH5MD - High Performance Interface for H5MD Trajectories
 
-ZnH5MD allows easy access to simulation results from H5MD trajectories.
+ZnH5MD allows easy access to simulation results from H5MD trajectories. It
+provides a Python interface and can convert existing data to H5MD files as well
+as export to other formats.
+
+```
+pip install znh5md["dask"]
+```
 
 ## Example
-In the following example we investigate an H5MD dump from LAMMPS with 1000 atoms and 201 configurations:
+
+In the following example we investigate an H5MD dump from LAMMPS with 1000 atoms
+and 201 configurations:
 
 ```python
 import znh5md
 
 traj = znh5md.DaskH5MD("file.h5", time_chunk_size=500, species_chunk_size=100)
 
 print(traj.file.time_dependent_groups)
@@ -30,36 +38,51 @@
 # You can iterate through the data
 for item in traj.position.batch(size=27, axis=0):
     for x in item.batch(size=17, axis=1):
         print(x.value.compute())
 ```
 
 ## ASE Atoms
+
 You can use ZnH5MD to store ASE Atoms objects in the H5MD format.
 
-> ZnH5MD does not support all features of ASE Atoms objects. It s important to note that unsupported parts are silently ignored and no error is raised.
+> ZnH5MD does not support all features of ASE Atoms objects. It s important to
+> note that unsupported parts are silently ignored and no error is raised.
 
 > The ASEH5MD interface will not provide any time and step information.
 
-> If you have a list of Atoms with different PBC values, you can use `znh5md.io.AtomsReader(atoms, use_pbc_group=True)`. This will create a `pbc` group in `box/` that also contains `step` and `time`. This is not an official H5MD specification so it can cause issues with other tools. If you don't specify this, the pbc of the first atoms in the list will be applied.
+> If you have a list of Atoms with different PBC values, you can use
+> `znh5md.io.AtomsReader(atoms, use_pbc_group=True)`. This will create a `pbc`
+> group in `box/` that also contains `step` and `time`. This is not an official
+> H5MD specification so it can cause issues with other tools. If you don't
+> specify this, the pbc of the first atoms in the list will be applied.
 
 ```python
 import znh5md
 import ase
 
 atoms: list[ase.Atoms]
 
 db = znh5md.io.DataWriter(filename="db.h5")
 db.initialize_database_groups()
 
-db.add(znh5md.io.AtomsReader(atoms))
+db.add(znh5md.io.AtomsReader(atoms)) # or znh5md.io.ChemfilesReader
 
 data = znh5md.ASEH5MD("db.h5")
 data.get_atoms_list() == atoms
 ```
 
 ## CLI
+
 ZnH5MD provides a small set of CLI tools:
 
 - `znh5md view <file.h5>` to view the File using `ase.visualize`
-- `znh5md export <file.h5> <file.xyz>` to export the file to `.xyz` or any other supported file format
-- `znh5md convert <file.xyz> <file.h5>` to save a `file.xyz` as `file.h5` in the H5MD standard.
+- `znh5md export <file.h5> <file.xyz>` to export the file to `.xyz` or any other
+  supported file format
+- `znh5md convert <file.xyz> <file.h5>` to save a `file.xyz` as `file.h5` in the
+  H5MD standard.
+
+## More examples
+
+A complete documentation is still work in progress. In the meantime, I can
+recommend looking at the tests, especially `test_znh5md.py` to learn more about
+slicing and batching.
```

### Comparing `znh5md-0.1.6a0/pyproject.toml` & `znh5md-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "znh5md"
-version = "0.1.6a0"
+version = "0.1.7"
 description = "High Performance Interface for H5MD Trajectories"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 h5py = "^3.7.0"
-dask = {extras = ["array"], version = "^2022.11.1"}
+dask = {extras = ["array"], version = "^2022.11.1", optional = true}
 ase = "^3.22.1"
 tqdm = "^4.65.0"
-typer = "^0.7.0"
+chemfiles = "^0.10.3"
+typer = {extras = ["all"], version = "^0.7.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 ruff = "^0.0.256"
 pytest = "^7.2.0"
 graphviz = "^0.20.1"
@@ -27,14 +28,17 @@
 
 [tool.poetry.group.notebook.dependencies]
 jupyterlab = "^3.5.0"
 
 [tool.poetry.scripts]
 znh5md = 'znh5md.cli:app'
 
+[tool.poetry.extras]
+dask = ["dask"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 90
 preview = true
@@ -51,8 +55,8 @@
     "D213", "D203", "N802", "N801"
 ]
 
 exclude = [
     "tmp",
     "tests",
     "docs",
-]
+]
```

### Comparing `znh5md-0.1.6a0/znh5md/cli.py` & `znh5md-0.1.7/znh5md/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     data = znh5md.ASEH5MD(file)
     ase.visualize.view(data.get_atoms_list())
 
 
 @app.command()
 def export(file: str, output: str):
-    """export a H5MD File into the output file."""
+    """Export a H5MD File into the output file."""
     import znh5md
 
     data = znh5md.ASEH5MD(file)
     for atom in tqdm.tqdm(data.get_atoms_list(), ncols=120):
         ase.io.write(output, atom, append=True)
```

### Comparing `znh5md-0.1.6a0/znh5md/format/__init__.py` & `znh5md-0.1.7/znh5md/format/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     boundary: str = "boundary"
     position: str = "position"
     energy: str = "energy"
     species: str = "species"
     forces: str = "forces"
     stress: str = "stress"
     velocity: str = "velocity"
+    momentum: str = "momentum"
     pbc: str = "pbc"
     dimension: str = "dimension"
 
     @staticmethod
     def encode_boundary(value) -> np.ndarray:
         return np.array(
             [
@@ -52,14 +53,15 @@
 
 
 PARTICLES_GRP = [
     GRP.position,
     GRP.species,
     GRP.forces,
     GRP.velocity,
+    GRP.momentum,
     GRP.pbc,
     GRP.dimension,
     GRP.edges,
     GRP.boundary,
 ]
 
 OBSERVABLES_GRP = [GRP.energy, GRP.stress]
```

### Comparing `znh5md-0.1.6a0/znh5md/io/base.py` & `znh5md-0.1.7/znh5md/io/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,23 @@
         -------
         typing.Iterator[typing.Dict[str, ExplicitStepTimeChunk]]
             A dictionary of chunks. The key is the name of the group.
             Each chunk containing the data for one group.
         """
         raise NotImplementedError()
 
+    def _fill_with_nan(self, data: list) -> np.ndarray:
+        max_n_particles = max(x.shape[0] for x in data)
+        dimensions = data[0].shape[1:]
+
+        result = np.full((len(data), max_n_particles, *dimensions), np.nan)
+        for i, x in enumerate(data):
+            result[i, : x.shape[0], ...] = x
+        return result
+
 
 @dataclasses.dataclass
 class DataWriter:
     filename: str
     particles_path: str = "particles/atoms"
     observables_path: str = "observables/atoms"
```

### Comparing `znh5md-0.1.6a0/znh5md/io/reader.py` & `znh5md-0.1.7/znh5md/io/reader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 import logging
 import typing
 
 import ase.io
+import chemfiles
 import numpy as np
 import tqdm
 from ase.calculators.calculator import PropertyNotImplementedError
 
 from znh5md.format import GRP
 from znh5md.io.base import DataReader, FixedStepTimeChunk
 
@@ -39,23 +40,14 @@
     atoms: list[ase.Atoms]
     frames_per_chunk: int = 100  # must be larger than 1
     step: int = 1
     time: float = 1
     use_pbc_group: bool = False
     save_atoms_results: bool = True
 
-    def _fill_with_nan(self, data: list) -> np.ndarray:
-        max_n_particles = max(x.shape[0] for x in data)
-        dimensions = data[0].shape[1:]
-
-        result = np.full((len(data), max_n_particles, *dimensions), np.nan)
-        for i, x in enumerate(data):
-            result[i, : x.shape[0], ...] = x
-        return result
-
     def _get_positions(self, atoms: list[ase.Atoms]) -> np.ndarray:
         data = [x.get_positions() for x in atoms]
         try:
             return np.array(data).astype(float)
         except ValueError:
             return self._fill_with_nan(data).astype(float)
 
@@ -73,14 +65,21 @@
     def _get_forces(self, atoms: list[ase.Atoms]) -> np.ndarray:
         data = [x.get_forces() for x in atoms]
         try:
             return np.array(data).astype(float)
         except ValueError:
             return self._fill_with_nan(data).astype(float)
 
+    def _get_momenta(self, atoms: list[ase.Atoms]) -> np.ndarray:
+        data = [x.arrays["momenta"] for x in atoms]
+        try:
+            return np.array(data).astype(float)
+        except ValueError:
+            return self._fill_with_nan(data).astype(float)
+
     def _get_stress(self, atoms: list[ase.Atoms]) -> np.ndarray:
         return np.array([x.get_stress() for x in atoms]).astype(float)
 
     def _get_edges(self, atoms: list[ase.Atoms]) -> np.ndarray:
         return np.array([x.get_cell() for x in atoms]).astype(float)
 
     def _get_pbc(self, atoms: list[ase.Atoms]) -> np.ndarray:
@@ -109,14 +108,15 @@
                 GRP.position: self._get_positions,
                 GRP.energy: self._get_energy,
                 GRP.species: self._get_species,
                 GRP.forces: self._get_forces,
                 GRP.stress: self._get_stress,
                 GRP.edges: self._get_edges,
                 GRP.boundary: self._get_boundary,
+                GRP.momentum: self._get_momenta,
             }
             if self.use_pbc_group:
                 functions[GRP.pbc] = self._get_pbc
 
             for name in group_names or functions:
                 if name not in functions:
                     raise ValueError(f"Value {name} not supported")
@@ -124,15 +124,15 @@
                 try:
                     value = functions[name](self.atoms[start_index:stop_index])
                     data[name] = FixedStepTimeChunk(
                         value=value,
                         step=self.step,
                         time=self.time,
                     )
-                except (PropertyNotImplementedError, RuntimeError) as err:
+                except (PropertyNotImplementedError, RuntimeError, KeyError) as err:
                     if group_names is not None:
                         # if the property was specifically selected, raise the error
                         raise err
                     else:
                         log.debug(f"Skipping {name} because {err}")
 
             if self.atoms[0].calc is not None and self.save_atoms_results:
@@ -195,7 +195,111 @@
             if len(atoms_list) == self.frames_per_chunk:
                 reader.atoms = atoms_list
                 yield from reader.yield_chunks()
                 atoms_list = []
         if len(atoms_list) > 0:
             reader.atoms = atoms_list
             yield from reader.yield_chunks()
+
+
+@dataclasses.dataclass
+class ChemfilesReader(DataReader):
+    filename: str
+    format: str = ""
+    frames_per_chunk: int = 5000
+    step: int = 1
+    time: float = 1
+
+    def yield_chunks(self) -> typing.Iterator[typing.Dict[str, FixedStepTimeChunk]]:
+        with chemfiles.Trajectory(self.filename, format=self.format) as trajectory:
+            positions = []
+            species = []
+            energy = []
+            cell = []
+            pbc = []
+            for frame in tqdm.tqdm(trajectory, total=trajectory.nsteps):
+                positions.append(np.copy(frame.positions))
+                species.append(np.copy([atom.atomic_number for atom in frame.atoms]))
+                cell.append(np.copy(frame.cell.lengths))
+
+                if "energy" in frame.list_properties():
+                    energy.append(np.copy(frame["energy"]).astype(float))
+                if "pbc" in frame.list_properties():
+                    pbc.append(
+                        [True if x == "T" else False for x in frame["pbc"].split()]
+                    )
+
+                if len(positions) == self.frames_per_chunk:
+                    positions = self._fill_with_nan(positions).astype(float)
+                    species = self._fill_with_nan(species).astype(float)
+
+                    data = {
+                        GRP.position: FixedStepTimeChunk(
+                            value=positions,
+                            step=self.step,
+                            time=self.time,
+                        ),
+                        GRP.species: FixedStepTimeChunk(
+                            value=species,
+                            step=self.step,
+                            time=self.time,
+                        ),
+                        GRP.edges: FixedStepTimeChunk(
+                            value=np.stack(cell),
+                            step=self.step,
+                            time=self.time,
+                        ),
+                    }
+                    if len(energy) > 0:
+                        data[GRP.energy] = FixedStepTimeChunk(
+                            value=np.stack(energy),
+                            step=self.step,
+                            time=self.time,
+                        )
+                    if len(pbc) > 0:
+                        data[GRP.pbc] = FixedStepTimeChunk(
+                            value=np.stack(pbc),
+                            step=self.step,
+                            time=self.time,
+                        )
+
+                    yield data
+
+                    positions = []
+                    species = []
+                    energy = []
+                    cell = []
+                    pbc = []
+            if len(positions) > 0:
+                positions = self._fill_with_nan(positions).astype(float)
+                species = self._fill_with_nan(species).astype(float)
+
+                data = {
+                    GRP.position: FixedStepTimeChunk(
+                        value=positions,
+                        step=self.step,
+                        time=self.time,
+                    ),
+                    GRP.species: FixedStepTimeChunk(
+                        value=species,
+                        step=self.step,
+                        time=self.time,
+                    ),
+                    GRP.edges: FixedStepTimeChunk(
+                        value=np.stack(cell),
+                        step=self.step,
+                        time=self.time,
+                    ),
+                }
+                if len(energy) > 0:
+                    data[GRP.energy] = FixedStepTimeChunk(
+                        value=np.stack(energy),
+                        step=self.step,
+                        time=self.time,
+                    )
+                if len(pbc) > 0:
+                    data[GRP.pbc] = FixedStepTimeChunk(
+                        value=np.stack(pbc),
+                        step=self.step,
+                        time=self.time,
+                    )
+                yield data
```

### Comparing `znh5md-0.1.6a0/PKG-INFO` & `znh5md-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: znh5md
-Version: 0.1.6a0
+Version: 0.1.7
 Summary: High Performance Interface for H5MD Trajectories
 License: Apache-2.0
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dask
 Requires-Dist: ase (>=3.22.1,<4.0.0)
-Requires-Dist: dask[array] (>=2022.11.1,<2023.0.0)
+Requires-Dist: chemfiles (>=0.10.3,<0.11.0)
+Requires-Dist: dask[array] (>=2022.11.1,<2023.0.0) ; extra == "dask"
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnH5MD/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnH5MD?branch=main)
 [![PyPI version](https://badge.fury.io/py/znh5md.svg)](https://badge.fury.io/py/znh5md)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnH5MD/HEAD)
 
 # ZnH5MD - High Performance Interface for H5MD Trajectories
 
-ZnH5MD allows easy access to simulation results from H5MD trajectories.
+ZnH5MD allows easy access to simulation results from H5MD trajectories. It
+provides a Python interface and can convert existing data to H5MD files as well
+as export to other formats.
+
+```
+pip install znh5md["dask"]
+```
 
 ## Example
-In the following example we investigate an H5MD dump from LAMMPS with 1000 atoms and 201 configurations:
+
+In the following example we investigate an H5MD dump from LAMMPS with 1000 atoms
+and 201 configurations:
 
 ```python
 import znh5md
 
 traj = znh5md.DaskH5MD("file.h5", time_chunk_size=500, species_chunk_size=100)
 
 print(traj.file.time_dependent_groups)
@@ -50,37 +60,52 @@
 # You can iterate through the data
 for item in traj.position.batch(size=27, axis=0):
     for x in item.batch(size=17, axis=1):
         print(x.value.compute())
 ```
 
 ## ASE Atoms
+
 You can use ZnH5MD to store ASE Atoms objects in the H5MD format.
 
-> ZnH5MD does not support all features of ASE Atoms objects. It s important to note that unsupported parts are silently ignored and no error is raised.
+> ZnH5MD does not support all features of ASE Atoms objects. It s important to
+> note that unsupported parts are silently ignored and no error is raised.
 
 > The ASEH5MD interface will not provide any time and step information.
 
-> If you have a list of Atoms with different PBC values, you can use `znh5md.io.AtomsReader(atoms, use_pbc_group=True)`. This will create a `pbc` group in `box/` that also contains `step` and `time`. This is not an official H5MD specification so it can cause issues with other tools. If you don't specify this, the pbc of the first atoms in the list will be applied.
+> If you have a list of Atoms with different PBC values, you can use
+> `znh5md.io.AtomsReader(atoms, use_pbc_group=True)`. This will create a `pbc`
+> group in `box/` that also contains `step` and `time`. This is not an official
+> H5MD specification so it can cause issues with other tools. If you don't
+> specify this, the pbc of the first atoms in the list will be applied.
 
 ```python
 import znh5md
 import ase
 
 atoms: list[ase.Atoms]
 
 db = znh5md.io.DataWriter(filename="db.h5")
 db.initialize_database_groups()
 
-db.add(znh5md.io.AtomsReader(atoms))
+db.add(znh5md.io.AtomsReader(atoms)) # or znh5md.io.ChemfilesReader
 
 data = znh5md.ASEH5MD("db.h5")
 data.get_atoms_list() == atoms
 ```
 
 ## CLI
+
 ZnH5MD provides a small set of CLI tools:
 
 - `znh5md view <file.h5>` to view the File using `ase.visualize`
-- `znh5md export <file.h5> <file.xyz>` to export the file to `.xyz` or any other supported file format
-- `znh5md convert <file.xyz> <file.h5>` to save a `file.xyz` as `file.h5` in the H5MD standard.
+- `znh5md export <file.h5> <file.xyz>` to export the file to `.xyz` or any other
+  supported file format
+- `znh5md convert <file.xyz> <file.h5>` to save a `file.xyz` as `file.h5` in the
+  H5MD standard.
+
+## More examples
+
+A complete documentation is still work in progress. In the meantime, I can
+recommend looking at the tests, especially `test_znh5md.py` to learn more about
+slicing and batching.
```

