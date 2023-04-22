# Comparing `tmp/pyl3dmd-0.0.9.tar.gz` & `tmp/pyl3dmd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyl3dmd-0.0.9.tar", last modified: Fri Apr 21 19:21:18 2023, max compression
+gzip compressed data, was "pyl3dmd-0.1.0.tar", last modified: Sat Apr 22 16:45:19 2023, max compression
```

## Comparing `pyl3dmd-0.0.9.tar` & `pyl3dmd-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 19:21:18.590963 pyl3dmd-0.0.9/
--rw-rw-rw-   0        0        0      753 2023-04-21 19:21:18.589965 pyl3dmd-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 19:21:18.579993 pyl3dmd-0.0.9/pyl3dmd/
--rw-rw-rw-   0        0        0      908 2023-02-08 02:47:17.000000 pyl3dmd-0.0.9/pyl3dmd/__init__.py
--rw-rw-rw-   0        0        0     7700 2023-02-14 04:41:39.000000 pyl3dmd-0.0.9/pyl3dmd/cpsa.py
--rw-rw-rw-   0        0        0    15385 2023-02-08 02:50:24.000000 pyl3dmd-0.0.9/pyl3dmd/descriptors1set.py
--rw-rw-rw-   0        0        0    24929 2023-02-08 02:54:20.000000 pyl3dmd-0.0.9/pyl3dmd/descriptors2set.py
--rw-rw-rw-   0        0        0    11137 2023-02-08 02:54:29.000000 pyl3dmd-0.0.9/pyl3dmd/descriptors3set.py
--rw-rw-rw-   0        0        0     7700 2023-02-08 02:52:49.000000 pyl3dmd-0.0.9/pyl3dmd/descriptors4set.py
--rw-rw-rw-   0        0        0     3086 2023-02-08 02:52:27.000000 pyl3dmd-0.0.9/pyl3dmd/descriptors5set.py
--rw-rw-rw-   0        0        0     4278 2023-02-08 02:52:17.000000 pyl3dmd-0.0.9/pyl3dmd/descriptors6set.py
--rw-rw-rw-   0        0        0     2966 2023-02-14 04:42:15.000000 pyl3dmd-0.0.9/pyl3dmd/distancedistancematrixdescriptors.py
--rw-rw-rw-   0        0        0     2573 2023-02-14 04:42:09.000000 pyl3dmd-0.0.9/pyl3dmd/geary.py
--rw-rw-rw-   0        0        0    24925 2023-02-14 04:42:04.000000 pyl3dmd-0.0.9/pyl3dmd/geometricdescriptors.py
--rw-rw-rw-   0        0        0     3895 2023-02-08 02:51:59.000000 pyl3dmd-0.0.9/pyl3dmd/getadjacencyanddistancematrices.py
--rw-rw-rw-   0        0        0     8781 2023-02-17 06:58:03.000000 pyl3dmd-0.0.9/pyl3dmd/getatomicproperties.py
--rw-rw-rw-   0        0        0    11133 2023-02-14 04:42:26.000000 pyl3dmd-0.0.9/pyl3dmd/getaway.py
--rw-rw-rw-   0        0        0    10918 2023-04-21 19:20:13.000000 pyl3dmd-0.0.9/pyl3dmd/getinfofromlammpsdatafile.py
--rw-rw-rw-   0        0        0    11194 2023-02-08 02:50:57.000000 pyl3dmd-0.0.9/pyl3dmd/getinfofromlammpstrajfile.py
--rw-rw-rw-   0        0        0     2607 2023-02-14 04:42:53.000000 pyl3dmd-0.0.9/pyl3dmd/moran.py
--rw-rw-rw-   0        0        0     2283 2023-02-14 04:42:48.000000 pyl3dmd-0.0.9/pyl3dmd/moreaubroto.py
--rw-rw-rw-   0        0        0     2413 2023-02-14 04:42:43.000000 pyl3dmd-0.0.9/pyl3dmd/morse.py
--rw-rw-rw-   0        0        0     9558 2023-02-13 17:27:02.000000 pyl3dmd-0.0.9/pyl3dmd/pyl3dmd.py
--rw-rw-rw-   0        0        0     2438 2023-02-14 04:43:08.000000 pyl3dmd-0.0.9/pyl3dmd/rdf.py
--rw-rw-rw-   0        0        0     3271 2023-02-08 02:55:13.000000 pyl3dmd-0.0.9/pyl3dmd/removehydrogenfrommolecule.py
--rw-rw-rw-   0        0        0    15383 2023-02-14 04:43:20.000000 pyl3dmd-0.0.9/pyl3dmd/topologyconnectivity3Ddescriptors.py
--rw-rw-rw-   0        0        0     3082 2023-02-14 04:43:37.000000 pyl3dmd-0.0.9/pyl3dmd/whim.py
-drwxrwxrwx   0        0        0        0 2023-04-21 19:21:18.587972 pyl3dmd-0.0.9/pyl3dmd.egg-info/
--rw-rw-rw-   0        0        0      753 2023-04-21 19:21:18.000000 pyl3dmd-0.0.9/pyl3dmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2023-04-21 19:21:18.000000 pyl3dmd-0.0.9/pyl3dmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 19:21:18.000000 pyl3dmd-0.0.9/pyl3dmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 19:21:18.000000 pyl3dmd-0.0.9/pyl3dmd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 19:21:18.591961 pyl3dmd-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2272 2023-04-21 19:17:24.000000 pyl3dmd-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:45:19.382943 pyl3dmd-0.1.0/
+-rw-rw-rw-   0        0        0      753 2023-04-22 16:45:19.381948 pyl3dmd-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-22 16:45:19.373968 pyl3dmd-0.1.0/pyl3dmd/
+-rw-rw-rw-   0        0        0      908 2023-02-08 02:47:17.000000 pyl3dmd-0.1.0/pyl3dmd/__init__.py
+-rw-rw-rw-   0        0        0     7700 2023-02-14 04:41:39.000000 pyl3dmd-0.1.0/pyl3dmd/cpsa.py
+-rw-rw-rw-   0        0        0    19226 2023-04-22 16:38:51.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors1set.py
+-rw-rw-rw-   0        0        0    27100 2023-04-22 16:37:16.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors2set.py
+-rw-rw-rw-   0        0        0    11685 2023-04-22 16:40:28.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors3set.py
+-rw-rw-rw-   0        0        0     7700 2023-02-17 11:13:14.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors4set.py
+-rw-rw-rw-   0        0        0     3086 2023-02-17 11:13:14.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors5set.py
+-rw-rw-rw-   0        0        0     4278 2023-02-17 11:13:14.000000 pyl3dmd-0.1.0/pyl3dmd/descriptors6set.py
+-rw-rw-rw-   0        0        0     2966 2023-02-14 04:42:15.000000 pyl3dmd-0.1.0/pyl3dmd/distancedistancematrixdescriptors.py
+-rw-rw-rw-   0        0        0     2573 2023-02-14 04:42:09.000000 pyl3dmd-0.1.0/pyl3dmd/geary.py
+-rw-rw-rw-   0        0        0    24925 2023-02-14 04:42:04.000000 pyl3dmd-0.1.0/pyl3dmd/geometricdescriptors.py
+-rw-rw-rw-   0        0        0     5432 2023-04-22 16:37:44.000000 pyl3dmd-0.1.0/pyl3dmd/getadjacencyanddistancematrices.py
+-rw-rw-rw-   0        0        0     8781 2023-02-17 06:58:03.000000 pyl3dmd-0.1.0/pyl3dmd/getatomicproperties.py
+-rw-rw-rw-   0        0        0    11133 2023-02-14 04:42:26.000000 pyl3dmd-0.1.0/pyl3dmd/getaway.py
+-rw-rw-rw-   0        0        0    10918 2023-04-21 19:20:13.000000 pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpsdatafile.py
+-rw-rw-rw-   0        0        0    11194 2023-02-08 02:50:57.000000 pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpstrajfile.py
+-rw-rw-rw-   0        0        0     2607 2023-02-14 04:42:53.000000 pyl3dmd-0.1.0/pyl3dmd/moran.py
+-rw-rw-rw-   0        0        0     2283 2023-02-14 04:42:48.000000 pyl3dmd-0.1.0/pyl3dmd/moreaubroto.py
+-rw-rw-rw-   0        0        0     2413 2023-02-14 04:42:43.000000 pyl3dmd-0.1.0/pyl3dmd/morse.py
+-rw-rw-rw-   0        0        0     9558 2023-02-13 17:27:02.000000 pyl3dmd-0.1.0/pyl3dmd/pyl3dmd.py
+-rw-rw-rw-   0        0        0     2438 2023-02-14 04:43:08.000000 pyl3dmd-0.1.0/pyl3dmd/rdf.py
+-rw-rw-rw-   0        0        0     5408 2023-04-22 16:44:14.000000 pyl3dmd-0.1.0/pyl3dmd/removehydrogenfrommolecule.py
+-rw-rw-rw-   0        0        0    15383 2023-02-14 04:43:20.000000 pyl3dmd-0.1.0/pyl3dmd/topologyconnectivity3Ddescriptors.py
+-rw-rw-rw-   0        0        0     3082 2023-02-14 04:43:37.000000 pyl3dmd-0.1.0/pyl3dmd/whim.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:45:19.380949 pyl3dmd-0.1.0/pyl3dmd.egg-info/
+-rw-rw-rw-   0        0        0      753 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      781 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:45:19.000000 pyl3dmd-0.1.0/pyl3dmd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 16:45:19.383940 pyl3dmd-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2272 2023-04-22 16:42:36.000000 pyl3dmd-0.1.0/setup.py
```

### Comparing `pyl3dmd-0.0.9/PKG-INFO` & `pyl3dmd-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl3dmd
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors
 Author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 Author-email: panwarp@msoe.edu
 Keywords: Python,LAMMPS,Molecular Dynamics Simulations,Molecular Descriptors,Machine Learning,MD Simulations,3-Dimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/__init__.py` & `pyl3dmd-0.1.0/pyl3dmd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/cpsa.py` & `pyl3dmd-0.1.0/pyl3dmd/cpsa.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/descriptors1set.py` & `pyl3dmd-0.1.0/pyl3dmd/topologyconnectivity3Ddescriptors.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
-
 import numpy as np
 
 def caltopologyconnectivitydescriptors(xyz, mass, bond, angle, dihedral, adjMat, disMat):
     TCdes = {}
     
     massheavy, M, bondheavy, angleheavy, dihedralheavy = removehydrogen(xyz, mass, bond, angle, dihedral)
     G, Gx, Gy, Gz = calgeometricdistancematrix(M)
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/descriptors2set.py` & `pyl3dmd-0.1.0/pyl3dmd/geometricdescriptors.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
-
-
 import numpy as np
 
 
 def calgeometricdescriptors(xyz, mass, charge, bond, angle, dihedral, density, disMat):
     nB = len(bond)
     GMdes = {}
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/descriptors3set.py` & `pyl3dmd-0.1.0/pyl3dmd/getaway.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
-
-
 """
 GETAWAY Descriptors - Geometry, topology, and atom-weights assembly (GETAWAY) descriptors
 """
 
 from math import inf
 import numpy as np
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/descriptors4set.py` & `pyl3dmd-0.1.0/pyl3dmd/descriptors4set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/descriptors5set.py` & `pyl3dmd-0.1.0/pyl3dmd/descriptors5set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/descriptors6set.py` & `pyl3dmd-0.1.0/pyl3dmd/descriptors6set.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/distancedistancematrixdescriptors.py` & `pyl3dmd-0.1.0/pyl3dmd/distancedistancematrixdescriptors.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/geary.py` & `pyl3dmd-0.1.0/pyl3dmd/geary.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/geometricdescriptors.py` & `pyl3dmd-0.1.0/pyl3dmd/descriptors2set.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
+
+
 import numpy as np
 
 
 def calgeometricdescriptors(xyz, mass, charge, bond, angle, dihedral, density, disMat):
+    
     nB = len(bond)
     GMdes = {}
     
     gc, s2v, k3, k4 = calgeometriccenter(xyz)
     rcm = calcenterofmass(xyz,mass)
     Lx, Ly, Lz = calmoleculelength(xyz)
     Rg = calradiusofgyration(xyz,rcm,mass)
@@ -525,36 +528,86 @@
         M = molecular matrix consist of x, y, z coordinates of heavy atoms of a molecule
         massheavy = masses of heady atoms in a molecule
         bondheavy = atom ids of heavy atoms connected by bonds in a molecule
         angleheavy = atom ids of heavy atoms that are in angle interaction in a molecule
         dihedralheavy = atom ids of heavy atoms that are in dihedral or torsional interaction in a molecule
     """
     # Idenstify hydrogen atoms to deleted
-    idxdeletexyz = np.where(mass < 1.2)
+    idxdeletexyz = [i for i, mass in enumerate(mass) if mass < 1.2]
     if len(idxdeletexyz)>=1:
         # Mass
         massheavy = np.delete(mass, idxdeletexyz, 0) # Coordinates of only heavy atoms
         
         # Molecular matrix consist of x, y, z cartesian coordinates of the molecule
         M = np.delete(xyz, idxdeletexyz, 0) # Coordinates of only heavy atoms
-        
+            
         # Update bond table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(bond, np.array(idxdeletexyz)+1)
         idxkeepbond = [i for i in range(len(check)) if np.all(check[i,:] == [False, False])]
         bondheavy = bond[idxkeepbond,:] # Bonds between only heavy atoms
         
         # Update angle table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(angle, np.array(idxdeletexyz)+1)
         idxkeepangle = [i for i in range(len(check)) if np.all(check[i,:] == [False, False, False])]
         angleheavy = angle[idxkeepangle,:] # Angles between only heavy atoms
         
         # Update dihedral table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(dihedral, np.array(idxdeletexyz)+1)
         idxkeepdihedral = [i for i in range(len(check)) if np.all(check[i,:] == [False, False, False, False])]
         dihedralheavy = dihedral[idxkeepdihedral,:] # Dihedralheavy = between only heavy atoms
+        
+        
+        # Get a list of all atom IDs # sorted(list(set([a for b in bondheavy for a in b])))
+        atom_ids = list(set([a for b in bondheavy for a in b]))
+        
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+        
+        # Update the bond list with the new IDs
+        new_bond_list = []
+        for atom1, atom2 in bondheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_bond_list.append((new_atom1, new_atom2))
+        
+        bondheavy = np.array(new_bond_list)
+        
+        # Get a list of all atom IDs # sorted(list(set([a for b in bondheavy for a in b])))
+        atom_ids = list(set([a for b in angleheavy for a in b]))
+        
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+        
+        # Update the angle list with the new IDs
+        new_angle_list = []
+        for atom1, atom2, atom3 in angleheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_atom3 = id_map[atom3]
+            new_angle_list.append((new_atom1, new_atom2, new_atom3))
+        
+        angleheavy = np.array(new_angle_list)
+      
+        # Get a list of all atom IDs # sorted(list(set([a for b in bondheavy for a in b])))
+        atom_ids = list(set([a for b in dihedralheavy for a in b]))
+        
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+        
+        # Update the dihedral list with the new IDs
+        new_dihedral_list = []
+        for atom1, atom2, atom3, atom4 in dihedralheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_atom3 = id_map[atom3]
+            new_atom4 = id_map[atom4]
+            new_dihedral_list.append((new_atom1, new_atom2, new_atom3, new_atom4))
+        
+        dihedralheavy = np.array(new_dihedral_list)
+
     else:
         # If no heavy atoms then keep as it is
         massheavy = mass
         M = xyz
         bondheavy = bond
         angleheavy = angle
         dihedralheavy = dihedral
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/getadjacencyanddistancematrices.py` & `pyl3dmd-0.1.0/pyl3dmd/getadjacencyanddistancematrices.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,30 +24,63 @@
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 from math import inf
 import numpy as np
 
+"""
 def removehydrogen(masses, bonds):
-    """
-    It removes bonds of hydrogen atoms from a molecule using mass of atom
-    """
+
+    #It removes bonds of hydrogen atoms from a molecule using mass of atom
+
     # Idenstify hydrogen atoms to deleted
     idxdeletexyz = np.where(masses < 1.2)
     if len(idxdeletexyz)>=1:
         # Update bonds table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(bonds, np.array(idxdeletexyz)+1)
         idxkeepbond = [i for i in range(len(check)) if np.all(check[i,:] == [False, False])]
         bondheavy = bonds[idxkeepbond,:] # Bonds between only heavy atoms
         
     else:
         bondheavy = bonds
     return bondheavy
+"""
+
+def removehydrogen(masses, bonds):
+    """
+    It removes bonds of hydrogen atoms from a molecule using mass of atom
+    """
+    # Identify hydrogen atoms to be deleted
+    idxdeletexyz = np.where(masses < 1.2)[0]
+    if len(idxdeletexyz) >= 1:
+        # Update bonds table accordingly - Numpy check if elements of array belong to another array
+        check = np.isin(bonds, idxdeletexyz + 1)
+        idxkeepbond = [i for i in range(len(check)) if np.all(check[i, :] == [False, False])]
+        bondheavy = bonds[idxkeepbond, :]  # Bonds between only heavy atoms
+
+        # Get a list of all atom IDs
+        atom_ids = list(set([a for b in bondheavy for a in b]))
+
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+
+        # Update the bond list with the new IDs
+        new_bond_list = []
+        for atom1, atom2 in bondheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_bond_list.append((new_atom1, new_atom2))
+
+        bondheavy = np.array(new_bond_list)
+
+    else:
+        bondheavy = bonds
 
+    return bondheavy
 
 def multModSquareMatrices(M,N):
     """
     Modified matrix-matrix multiplication of sqaure matrices
     # Ref - https://imada.sdu.dk/~rolf/Edu/DM534/E16/IntroCS2016-final.pdf
     size = len(M)
     result = [[inf for x in range(size)] for y in range(size)]
@@ -61,31 +94,38 @@
     result = np.zeros([size,size])*inf
     for i in range(size):
         result[i][:] = np.min(M[i] + N.T, axis=1)
     return result
 
 
 
-def caladjacencymatrix(bonds):
-    """
-    Calculate adjacency matrix from bonds
-    """      
+def caladjacencymatrix(bonds):      
     edge = bonds-1
+    edge_u = edge[:,0]
+    edge_v = edge[:,1]
 
     # Number of nodes
     n = np.max(edge)+1
+    #print(edge)
+    # create empty adjacency lists - one for each node
+    adjList = [[] for k in range(n)]
 
     # adjacency matrix - initialize with 0
     adjMatrix = np.zeros((n,n))
 
-    u = edge[:,0]
-    v = edge[:,1]
-    adjMatrix[u,v] = 1
-    adjMatrix[v,u] = 1
-    return adjMatrix
+    # scan the arrays edge_u and edge_v
+    for i in range(len(edge_u)):
+        u = edge_u[i]
+        v = edge_v[i]
+        adjList[u].append(v)
+        adjList[v].append(u)
+        adjMatrix[u][v] = 1
+        adjMatrix[v][u] = 1
+    #print(np.shape(adjMatrix))
+    return adjMatrix, adjList
 
          
 def caldistancematrix(adjMatrix): 
     """
     Calculate edge or 2D distance matrix from adjacency matrix
     """   
     nA = len(adjMatrix)
@@ -109,12 +149,15 @@
     Get adjacency and distnace matrices of each molecule in the simulation box
     """
     eachMolsAdjMat = {}
     eachMolsDisMat = {}
     numMols = len(eachMolsBonds)
     for i in range(numMols):
         bonds = eachMolsBonds[i]
+        #print(bonds)
         masses = eachMolsMass[i]
         bondheavy = removehydrogen(masses, bonds)
-        eachMolsAdjMat[i] = caladjacencymatrix(bondheavy)        # Get 2D adjaceny matrix
+        #print(bondheavy)
+
+        eachMolsAdjMat[i], _ = caladjacencymatrix(bondheavy)        # Get 2D adjaceny matrix
         eachMolsDisMat[i] = caldistancematrix(eachMolsAdjMat[i])    # Get 2D distance matrix
     return (eachMolsAdjMat, eachMolsDisMat)
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/getatomicproperties.py` & `pyl3dmd-0.1.0/pyl3dmd/getatomicproperties.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/getaway.py` & `pyl3dmd-0.1.0/pyl3dmd/descriptors3set.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,36 +19,54 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
+
+
 """
 GETAWAY Descriptors - Geometry, topology, and atom-weights assembly (GETAWAY) descriptors
 """
 
 from math import inf
 import numpy as np
 
 
 def removehydrogen(masses, bonds):
     """
     It removes bonds of hydrogen atoms from a molecule using mass of atom
     """
-    # Idenstify hydrogen atoms to deleted
-    idxdeletexyz = np.where(masses < 1.2)
-    if len(idxdeletexyz)>=1:
+    # Identify hydrogen atoms to be deleted
+    idxdeletexyz = np.where(masses < 1.2)[0]
+    if len(idxdeletexyz) >= 1:
         # Update bonds table accordingly - Numpy check if elements of array belong to another array
-        check = np.isin(bonds, np.array(idxdeletexyz)+1)
-        idxkeepbond = [i for i in range(len(check)) if np.all(check[i,:] == [False, False])]
-        bondheavy = bonds[idxkeepbond,:] # Bonds between only heavy atoms
-        
+        check = np.isin(bonds, idxdeletexyz + 1)
+        idxkeepbond = [i for i in range(len(check)) if np.all(check[i, :] == [False, False])]
+        bondheavy = bonds[idxkeepbond, :]  # Bonds between only heavy atoms
+
+        # Get a list of all atom IDs
+        atom_ids = list(set([a for b in bondheavy for a in b]))
+
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+
+        # Update the bond list with the new IDs
+        new_bond_list = []
+        for atom1, atom2 in bondheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_bond_list.append((new_atom1, new_atom2))
+
+        bondheavy = np.array(new_bond_list)
+
     else:
         bondheavy = bonds
+
     return bondheavy
 
 
 def multModSquareMatrices(M,N):
     """
     Modified matrix-matrix multiplication of sqaure matrices
     # Ref - https://imada.sdu.dk/~rolf/Edu/DM534/E16/IntroCS2016-final.pdf
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/getinfofromlammpsdatafile.py` & `pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpsdatafile.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/getinfofromlammpstrajfile.py` & `pyl3dmd-0.1.0/pyl3dmd/getinfofromlammpstrajfile.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/moran.py` & `pyl3dmd-0.1.0/pyl3dmd/moran.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/moreaubroto.py` & `pyl3dmd-0.1.0/pyl3dmd/moreaubroto.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/morse.py` & `pyl3dmd-0.1.0/pyl3dmd/morse.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/pyl3dmd.py` & `pyl3dmd-0.1.0/pyl3dmd/pyl3dmd.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/rdf.py` & `pyl3dmd-0.1.0/pyl3dmd/rdf.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd/topologyconnectivity3Ddescriptors.py` & `pyl3dmd-0.1.0/pyl3dmd/descriptors1set.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of 
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. 
 See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
+
 import numpy as np
 
 def caltopologyconnectivitydescriptors(xyz, mass, bond, angle, dihedral, adjMat, disMat):
-    TCdes = {}
-    
+    TCdes = {}    
     massheavy, M, bondheavy, angleheavy, dihedralheavy = removehydrogen(xyz, mass, bond, angle, dihedral)
     G, Gx, Gy, Gz = calgeometricdistancematrix(M)
     Ginv, Ginv2 = calinversegeometricdistancematrix(G)
     
     disMat3D = G
+    #print(np.shape(adjMat))
     nA = len(massheavy)
     nB = len(bondheavy)
     #verMat = calvertexmatrix(adjMat)
     adjMat3D = cal3Dadjacencymatrix(adjMat, disMat3D)
 
     deltai3D, delta3D = caldirectlyfrom3Dadjacencymatrix(adjMat3D)
     etai3D, sigmai3D, sigma3D, sigmaAvg3D = caldirectlyfrom3Ddistancematrix(disMat3D)
@@ -103,38 +104,146 @@
     idxdeletexyz = [i for i, mass in enumerate(mass) if mass < 1.2]
     if len(idxdeletexyz)>=1:
         # Mass
         massheavy = np.delete(mass, idxdeletexyz, 0) # Coordinates of only heavy atoms
         
         # Molecular matrix consist of x, y, z cartesian coordinates of the molecule
         M = np.delete(xyz, idxdeletexyz, 0) # Coordinates of only heavy atoms
-        
+            
         # Update bond table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(bond, np.array(idxdeletexyz)+1)
         idxkeepbond = [i for i in range(len(check)) if np.all(check[i,:] == [False, False])]
         bondheavy = bond[idxkeepbond,:] # Bonds between only heavy atoms
         
         # Update angle table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(angle, np.array(idxdeletexyz)+1)
         idxkeepangle = [i for i in range(len(check)) if np.all(check[i,:] == [False, False, False])]
         angleheavy = angle[idxkeepangle,:] # Angles between only heavy atoms
         
         # Update dihedral table accordingly - Numpy check if elements of array belong to another array
         check = np.isin(dihedral, np.array(idxdeletexyz)+1)
         idxkeepdihedral = [i for i in range(len(check)) if np.all(check[i,:] == [False, False, False, False])]
         dihedralheavy = dihedral[idxkeepdihedral,:] # Dihedralheavy = between only heavy atoms
+        
+        
+        # Get a list of all atom IDs # sorted(list(set([a for b in bondheavy for a in b])))
+        atom_ids = list(set([a for b in bondheavy for a in b]))
+        
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+        
+        # Update the bond list with the new IDs
+        new_bond_list = []
+        for atom1, atom2 in bondheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_bond_list.append((new_atom1, new_atom2))
+        
+        bondheavy = np.array(new_bond_list)
+        
+        # Get a list of all atom IDs # sorted(list(set([a for b in bondheavy for a in b])))
+        atom_ids = list(set([a for b in angleheavy for a in b]))
+        
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+        
+        # Update the angle list with the new IDs
+        new_angle_list = []
+        for atom1, atom2, atom3 in angleheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_atom3 = id_map[atom3]
+            new_angle_list.append((new_atom1, new_atom2, new_atom3))
+        
+        angleheavy = np.array(new_angle_list)
+      
+        # Get a list of all atom IDs # sorted(list(set([a for b in bondheavy for a in b])))
+        atom_ids = list(set([a for b in dihedralheavy for a in b]))
+        
+        # Create a dictionary to map old IDs to new IDs
+        id_map = {old_id: new_id for new_id, old_id in enumerate(atom_ids, start=1)}
+        
+        # Update the dihedral list with the new IDs
+        new_dihedral_list = []
+        for atom1, atom2, atom3, atom4 in dihedralheavy:
+            new_atom1 = id_map[atom1]
+            new_atom2 = id_map[atom2]
+            new_atom3 = id_map[atom3]
+            new_atom4 = id_map[atom4]
+            new_dihedral_list.append((new_atom1, new_atom2, new_atom3, new_atom4))
+        
+        dihedralheavy = np.array(new_dihedral_list)
+
     else:
         # If no heavy atoms then keep as it is
         massheavy = mass
         M = xyz
         bondheavy = bond
         angleheavy = angle
         dihedralheavy = dihedral
     return (massheavy, M, bondheavy, angleheavy, dihedralheavy)
 
+def multModSquareMatrices(M,N):
+    """
+    Modified matrix-matrix multiplication of sqaure matrices
+    # Ref - https://imada.sdu.dk/~rolf/Edu/DM534/E16/IntroCS2016-final.pdf
+    size = len(M)
+    result = [[inf for x in range(size)] for y in range(size)]
+
+    for i in range(size):
+        for j in range(size):
+            for k in range(size):
+                result[i][j] = min(result[i][j], M[i][k] + N[k][j])
+    """
+    size = len(M)
+    result = np.zeros([size,size])*np.inf
+    for i in range(size):
+        result[i][:] = np.min(M[i] + N.T, axis=1)
+    return result
+
+
+
+def caladjacencymatrix(bonds):
+    """
+    Calculate adjacency matrix from bonds
+    """      
+    edge = bonds-1
+
+    # Number of nodes
+    n = np.max(edge)+1
+
+    # adjacency matrix - initialize with 0
+    adjMatrix = np.zeros((n,n))
+
+    u = edge[:,0]
+    v = edge[:,1]
+    adjMatrix[u,v] = 1
+    adjMatrix[v,u] = 1
+    return adjMatrix
+
+         
+def caldistancematrix(adjMatrix): 
+    """
+    Calculate edge or 2D distance matrix from adjacency matrix
+    """   
+    nA = len(adjMatrix)
+    # Create Edge Wight Matrix with weightage of 1 for all edge
+    W = np.zeros((nA,nA))
+    idx1 = np.where(~np.eye(adjMatrix.shape[0],dtype=bool) & (adjMatrix != 1))
+    idx2 = np.where(~np.eye(adjMatrix.shape[0],dtype=bool) & (adjMatrix == 1))
+    W[idx1[0],idx1[1]] = inf
+    W[idx2[0],idx2[1]] = 1
+                    
+    # Compute the distance matrix iteratively by computation of W^2, W^3, ..., W^5
+    temp = W
+    for i in range(2,nA):
+        temp = multModSquareMatrices(temp,W)
+    disMatrix = np.array(temp)
+    return disMatrix
+
 def calgeometricdistancematrix(M):
     """
     Calculate Euclidean Distance of atoms in a molecule - (numAtoms x numAtoms)
         G = Geometric Distance Matrix
         Ginv = Inverse Geometric Distance Matrix
         Gx = Euclidean distance of atoms in a molecule in x-direction
         Gy = Euclidean distance of atoms in a molecule in y-direction
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd/whim.py` & `pyl3dmd-0.1.0/pyl3dmd/whim.py`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/pyl3dmd.egg-info/PKG-INFO` & `pyl3dmd-0.1.0/pyl3dmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl3dmd
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors
 Author: Pawan Panwar, Quanpeng Yang, Ashlie Martini
 Author-email: panwarp@msoe.edu
 Keywords: Python,LAMMPS,Molecular Dynamics Simulations,Molecular Descriptors,Machine Learning,MD Simulations,3-Dimensional
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pyl3dmd-0.0.9/pyl3dmd.egg-info/SOURCES.txt` & `pyl3dmd-0.1.0/pyl3dmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyl3dmd-0.0.9/setup.py` & `pyl3dmd-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  along with PyL3dMD. If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9' 
+VERSION = '0.1.0' 
 DESCRIPTION = 'Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors'
 LONG_DESCRIPTION = 'PyL3dMD stands for Python LAMMPS 3-Dimensional Molecular Dynamics/Descriptors, a python package for 3D descriptors calculation'
 
 # setup
 setup(
        # name has to be identical with the name of the folder where the package is
         name="pyl3dmd",
```

