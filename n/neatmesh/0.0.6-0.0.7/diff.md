# Comparing `tmp/neatmesh-0.0.6.tar.gz` & `tmp/neatmesh-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neatmesh-0.0.6.tar", last modified: Sat Feb 11 14:04:38 2023, max compression
+gzip compressed data, was "neatmesh-0.0.7.tar", last modified: Sat Apr 22 14:14:10 2023, max compression
```

## Comparing `neatmesh-0.0.6.tar` & `neatmesh-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 14:04:38.169669 neatmesh-0.0.6/
--rw-rw-rw-   0        0        0     1093 2023-02-11 14:00:08.000000 neatmesh-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3898 2023-02-11 14:04:38.169669 neatmesh-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3307 2023-01-08 08:11:50.000000 neatmesh-0.0.6/README.md
--rw-rw-rw-   0        0        0       86 2022-03-17 16:26:16.000000 neatmesh-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      929 2023-02-11 14:04:38.185294 neatmesh-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-11 14:04:38.029877 neatmesh-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-02-11 14:04:38.107168 neatmesh-0.0.6/src/neatmesh/
--rw-rw-rw-   0        0        0      609 2022-09-28 15:59:19.000000 neatmesh-0.0.6/src/neatmesh/__init__.py
--rw-rw-rw-   0        0        0    13246 2023-01-08 08:23:27.000000 neatmesh-0.0.6/src/neatmesh/_analyzer.py
--rw-rw-rw-   0        0        0     2367 2022-09-26 00:23:46.000000 neatmesh-0.0.6/src/neatmesh/_cli.py
--rw-rw-rw-   0        0        0     1646 2022-09-26 17:10:51.000000 neatmesh-0.0.6/src/neatmesh/_common.py
--rw-rw-rw-   0        0        0      486 2022-09-26 00:24:47.000000 neatmesh-0.0.6/src/neatmesh/_exceptions.py
--rw-rw-rw-   0        0        0    12437 2022-09-24 07:10:36.000000 neatmesh-0.0.6/src/neatmesh/_geometry.py
--rw-rw-rw-   0        0        0     3675 2022-09-28 15:59:19.000000 neatmesh-0.0.6/src/neatmesh/_mesh.py
--rw-rw-rw-   0        0        0     8268 2022-09-28 15:59:19.000000 neatmesh-0.0.6/src/neatmesh/_reader.py
--rw-rw-rw-   0        0        0    11969 2023-01-08 08:23:27.000000 neatmesh-0.0.6/src/neatmesh/_reporter.py
-drwxrwxrwx   0        0        0        0 2023-02-11 14:04:38.154078 neatmesh-0.0.6/src/neatmesh.egg-info/
--rw-rw-rw-   0        0        0     3898 2023-02-11 14:04:37.000000 neatmesh-0.0.6/src/neatmesh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      704 2023-02-11 14:04:38.000000 neatmesh-0.0.6/src/neatmesh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 14:04:37.000000 neatmesh-0.0.6/src/neatmesh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-02-11 14:04:37.000000 neatmesh-0.0.6/src/neatmesh.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-02-11 14:04:37.000000 neatmesh-0.0.6/src/neatmesh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-11 14:04:38.000000 neatmesh-0.0.6/src/neatmesh.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-11 14:04:38.169669 neatmesh-0.0.6/tests/
--rw-rw-rw-   0        0        0     1438 2022-09-25 16:20:17.000000 neatmesh-0.0.6/tests/test_analyzer2d.py
--rw-rw-rw-   0        0        0      596 2022-09-26 17:04:13.000000 neatmesh-0.0.6/tests/test_analyzer3d_hex.py
--rw-rw-rw-   0        0        0      962 2022-09-26 17:04:13.000000 neatmesh-0.0.6/tests/test_analyzer3d_tetra.py
--rw-rw-rw-   0        0        0      368 2022-09-28 15:59:19.000000 neatmesh-0.0.6/tests/test_dimensionality.py
--rw-rw-rw-   0        0        0     1911 2022-09-28 15:59:19.000000 neatmesh-0.0.6/tests/test_mesh2d.py
--rw-rw-rw-   0        0        0      537 2022-09-26 17:04:13.000000 neatmesh-0.0.6/tests/test_pyramid_geometry.py
--rw-rw-rw-   0        0        0      648 2022-09-26 17:04:13.000000 neatmesh-0.0.6/tests/test_tri_geometry.py
--rw-rw-rw-   0        0        0      553 2022-09-26 17:04:13.000000 neatmesh-0.0.6/tests/test_wedge_geometry.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.899921 neatmesh-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-02-11 14:00:08.000000 neatmesh-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3898 2023-04-22 14:14:10.899921 neatmesh-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3307 2023-01-08 08:11:50.000000 neatmesh-0.0.7/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-17 16:26:16.000000 neatmesh-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      929 2023-04-22 14:14:10.899921 neatmesh-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.837048 neatmesh-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.868661 neatmesh-0.0.7/src/neatmesh/
+-rw-rw-rw-   0        0        0      307 2023-04-22 13:54:58.000000 neatmesh-0.0.7/src/neatmesh/__init__.py
+-rw-rw-rw-   0        0        0    13410 2023-04-22 14:10:19.000000 neatmesh-0.0.7/src/neatmesh/_analyzer.py
+-rw-rw-rw-   0        0        0     2367 2022-09-26 00:23:46.000000 neatmesh-0.0.7/src/neatmesh/_cli.py
+-rw-rw-rw-   0        0        0     1646 2022-09-26 17:10:51.000000 neatmesh-0.0.7/src/neatmesh/_common.py
+-rw-rw-rw-   0        0        0      486 2022-09-26 00:24:47.000000 neatmesh-0.0.7/src/neatmesh/_exceptions.py
+-rw-rw-rw-   0        0        0    12437 2022-09-24 07:10:36.000000 neatmesh-0.0.7/src/neatmesh/_geometry.py
+-rw-rw-rw-   0        0        0     3981 2023-04-22 13:54:52.000000 neatmesh-0.0.7/src/neatmesh/_mesh.py
+-rw-rw-rw-   0        0        0     8268 2023-04-22 13:54:58.000000 neatmesh-0.0.7/src/neatmesh/_reader.py
+-rw-rw-rw-   0        0        0    12253 2023-04-22 14:11:18.000000 neatmesh-0.0.7/src/neatmesh/_reporter.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.884296 neatmesh-0.0.7/src/neatmesh.egg-info/
+-rw-rw-rw-   0        0        0     3898 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      704 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-22 14:14:10.000000 neatmesh-0.0.7/src/neatmesh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 14:14:10.884296 neatmesh-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1438 2022-09-25 16:20:17.000000 neatmesh-0.0.7/tests/test_analyzer2d.py
+-rw-rw-rw-   0        0        0      596 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_analyzer3d_hex.py
+-rw-rw-rw-   0        0        0      962 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_analyzer3d_tetra.py
+-rw-rw-rw-   0        0        0      368 2022-09-28 15:59:19.000000 neatmesh-0.0.7/tests/test_dimensionality.py
+-rw-rw-rw-   0        0        0     1911 2022-09-28 15:59:19.000000 neatmesh-0.0.7/tests/test_mesh2d.py
+-rw-rw-rw-   0        0        0      537 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_pyramid_geometry.py
+-rw-rw-rw-   0        0        0      648 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_tri_geometry.py
+-rw-rw-rw-   0        0        0      553 2022-09-26 17:04:13.000000 neatmesh-0.0.7/tests/test_wedge_geometry.py
```

### Comparing `neatmesh-0.0.6/LICENSE` & `neatmesh-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/PKG-INFO` & `neatmesh-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neatmesh
-Version: 0.0.6
+Version: 0.0.7
 Summary: Finite Volume Mesh Quality Inspector
 Home-page: https://github.com/eigemx/neatmesh
 Author: Mohamed Emara
 Author-email: mae.emara@gmail.com
 Project-URL: Bug Tracker, https://github.com/eigemx/neatmesh/issues
 Keywords: mesh,scientific,engineering,fvm,fem,finite volume,finite element
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neatmesh-0.0.6/README.md` & `neatmesh-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/setup.cfg` & `neatmesh-0.0.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6561 746d 6573 680d 0a76 6572   = neatmesh..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e36 0d0a 6175  sion = 0.0.6..au
+00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6175  sion = 0.0.7..au
 00000030: 7468 6f72 203d 204d 6f68 616d 6564 2045  thor = Mohamed E
 00000040: 6d61 7261 0d0a 6175 7468 6f72 5f65 6d61  mara..author_ema
 00000050: 696c 203d 206d 6165 2e65 6d61 7261 4067  il = mae.emara@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4669 6e69 7465 2056  ption = Finite V
 00000080: 6f6c 756d 6520 4d65 7368 2051 7561 6c69  olume Mesh Quali
 00000090: 7479 2049 6e73 7065 6374 6f72 0d0a 6c6f  ty Inspector..lo
```

### Comparing `neatmesh-0.0.6/src/neatmesh/_analyzer.py` & `neatmesh-0.0.7/src/neatmesh/_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,18 @@
         dot_product = dot(nei_owner_vectors, interior_face_normals)
 
         nei_owner_vectors[dot_product < 0] = -nei_owner_vectors[dot_product < 0]
 
         costheta = dot_normalize(nei_owner_vectors, interior_face_normals)
         self.non_ortho = np.arccos(costheta) * (180.0 / np.pi)
 
+    def surface_area(self) -> float:
+        boundary_faces_mask = self.owner_neighbor[:, 1] == -1
+        return np.sum(self.face_areas[boundary_faces_mask])
+
     def analyze_adjacents_volume_ratio(self) -> None:
         """Calculate the area ratio for each two neighbor cells (max/min)"""
         adjacent_cells_vol = np.take(self.cells_volumes, self.interior_faces, axis=0)
         self.adj_ratio = np.max(
             [
                 adjacent_cells_vol[:, 0] / adjacent_cells_vol[:, 1],
                 adjacent_cells_vol[:, 1] / adjacent_cells_vol[:, 0],
```

### Comparing `neatmesh-0.0.6/src/neatmesh/_cli.py` & `neatmesh-0.0.7/src/neatmesh/_cli.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/src/neatmesh/_common.py` & `neatmesh-0.0.7/src/neatmesh/_common.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/src/neatmesh/_geometry.py` & `neatmesh-0.0.7/src/neatmesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/src/neatmesh/_mesh.py` & `neatmesh-0.0.7/src/neatmesh/_mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """2D and 3D wrappers for neatmesh internals"""
+from typing import Union
+
 import numpy as np
 
 from ._analyzer import Analyzer2D, Analyzer3D
 from ._reader import MeshReader2D, MeshReader3D
 
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-few-public-methods
@@ -92,7 +94,18 @@
         self.pyramid_count = self._analyzer.pyramid_count
         self.wedge_count = self._analyzer.wedge_count
 
         # boundary faces
         self.n_boundary_faces = self._analyzer.n_boundary_faces
         self.boundary_faces_mask = self.owner_neighbor[:, 1] == -1
         self.internal_faces_mask = self.owner_neighbor[:, 1] != -1
+
+
+def read(mesh_file_path: str) -> Union[Mesh2D, Mesh3D]:
+    from ._reader import MeshReader2D, assign_reader
+
+    reader = assign_reader(mesh_file_path)
+
+    if isinstance(reader, MeshReader2D):
+        return Mesh2D(reader)
+    else:
+        return Mesh3D(reader)
```

### Comparing `neatmesh-0.0.6/src/neatmesh/_reader.py` & `neatmesh-0.0.7/src/neatmesh/_reader.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/src/neatmesh/_reporter.py` & `neatmesh-0.0.7/src/neatmesh/_reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             f"Inspecting file [cyan]'{filename}'[/] (file size: {fsize})"
         )
         self.console.print()
 
     def report_bounding_box(self):
         self.console.print("[yellow bold]Mesh bounding box: ")
         for point in self.analyzer.bounding_box():
-            print(f"\t{point}",)
+            print(f"\t({point[0]:.4f}, {point[1]:.4f}, {point[2]:.4f})")
         self.console.print()
 
     def report_concerns(self):
         if self.concerns:
             concerns_table = Table(box=None)
             concerns_table.add_column("", justify="left")
 
@@ -225,15 +225,21 @@
 
 class Reporter3D(Reporter):
     def __init__(self, console: Console, mesh: MeshReader, filename: str) -> None:
         super().__init__(console, mesh, filename)
 
     def report_mesh_volume(self):
         self.console.print(
-            f"Mesh volume = {self.analyzer.mesh_volume:.3f} L^3 (in mesh units)\n"
+            f"Mesh volume = {self.analyzer.mesh_volume:.3f} [L^3] (in mesh units)"
+        )
+
+    def report_mesh_surface_area(self):
+        s_area = self.analyzer.surface_area()
+        self.console.print(
+            f"Mesh surface area = {s_area:.3f} [L^2] (in mesh units)\n"
         )
 
     def report_elements_count(self):
         cell_count = self.analyzer.n_cells
         face_count = self.analyzer.n_faces
         point_count = self.analyzer.n_points
 
@@ -298,14 +304,15 @@
         if not rules:
             self.console.print("No quality rules file found, using defaults.\n")
         else:
             self.console.print(f"Found quality rules file: '{rules['fname']}'\n")
 
         self.report_bounding_box()
         self.report_mesh_volume()
+        self.report_mesh_surface_area()
         self.report_elements_count()
 
         quality_metrics_dict = {
             "Face Area": {"array": self.analyzer.face_areas, "sci_not": True,},
             "Face Aspect Ratio": {
                 "array": self.analyzer.face_aspect_ratios,
                 "sci_not": False,
```

### Comparing `neatmesh-0.0.6/src/neatmesh.egg-info/PKG-INFO` & `neatmesh-0.0.7/src/neatmesh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neatmesh
-Version: 0.0.6
+Version: 0.0.7
 Summary: Finite Volume Mesh Quality Inspector
 Home-page: https://github.com/eigemx/neatmesh
 Author: Mohamed Emara
 Author-email: mae.emara@gmail.com
 Project-URL: Bug Tracker, https://github.com/eigemx/neatmesh/issues
 Keywords: mesh,scientific,engineering,fvm,fem,finite volume,finite element
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neatmesh-0.0.6/src/neatmesh.egg-info/SOURCES.txt` & `neatmesh-0.0.7/src/neatmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_analyzer2d.py` & `neatmesh-0.0.7/tests/test_analyzer2d.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_analyzer3d_hex.py` & `neatmesh-0.0.7/tests/test_analyzer3d_hex.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_analyzer3d_tetra.py` & `neatmesh-0.0.7/tests/test_analyzer3d_tetra.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_mesh2d.py` & `neatmesh-0.0.7/tests/test_mesh2d.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_pyramid_geometry.py` & `neatmesh-0.0.7/tests/test_pyramid_geometry.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_tri_geometry.py` & `neatmesh-0.0.7/tests/test_tri_geometry.py`

 * *Files identical despite different names*

### Comparing `neatmesh-0.0.6/tests/test_wedge_geometry.py` & `neatmesh-0.0.7/tests/test_wedge_geometry.py`

 * *Files identical despite different names*

