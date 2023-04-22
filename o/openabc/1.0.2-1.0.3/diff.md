# Comparing `tmp/openabc-1.0.2.tar.gz` & `tmp/openabc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openabc-1.0.2.tar", last modified: Fri Apr 14 21:42:59 2023, max compression
+gzip compressed data, was "openabc-1.0.3.tar", last modified: Sat Apr 22 03:38:08 2023, max compression
```

## Comparing `openabc-1.0.2.tar` & `openabc-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/
--rw-rw----   0 sliu     (61642) sliu     (61642)     1080 2023-04-14 18:10:57.000000 openabc-1.0.2/LICENSE
--rw-rw----   0 sliu     (61642) sliu     (61642)      121 2023-04-14 20:42:49.000000 openabc-1.0.2/MANIFEST.in
--rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-14 21:42:59.000000 openabc-1.0.2/PKG-INFO
--rw-rw----   0 sliu     (61642) sliu     (61642)     1094 2023-04-14 21:02:42.000000 openabc-1.0.2/README.md
--rw-rw----   0 sliu     (61642) sliu     (61642)      428 2023-04-14 21:37:17.000000 openabc-1.0.2/pyproject.toml
--rw-rw----   0 sliu     (61642) sliu     (61642)       38 2023-04-14 21:42:59.000000 openabc-1.0.2/setup.cfg
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/
--rw-rw----   0 sliu     (61642) sliu     (61642)       23 2023-04-14 21:37:29.000000 openabc-1.0.2/src/openabc/__init__.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/
--rw-rw----   0 sliu     (61642) sliu     (61642)       73 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11969 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/cg_model.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/
--rw-rw----   0 sliu     (61642) sliu     (61642)      114 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     1317 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/angle_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4121 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/bond_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)      717 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/dihedral_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9168 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/nonbonded_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     3281 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4779 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/hps_model.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     3058 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/hps_zero_offset_model.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9863 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/moff_mrg_model.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/parameters/
--rw-rw----   0 sliu     (61642) sliu     (61642)     4287 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/HPS_KR_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)     4904 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)    11557 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv
--rw-rw----   0 sliu     (61642) sliu     (61642)     3372 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/parse_hps_parameters.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     1231 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/parse_moff_parameters.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    12545 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parameters/template_MOFF.top
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/forcefields/parsers/
--rw-rw----   0 sliu     (61642) sliu     (61642)      110 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4016 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/hps_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9129 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/moff_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     7485 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/parsers/mrg_parser.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     7347 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/forcefields/rigid.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc/utils/
--rw-rw----   0 sliu     (61642) sliu     (61642)     9312 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/CA2AA.py
--rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-04-14 18:10:24.000000 openabc-1.0.2/src/openabc/utils/__init__.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11095 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/helper_functions.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     4916 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/insert.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    11519 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/legacy_shadow_map.py
--rw-rw----   0 sliu     (61642) sliu     (61642)     9102 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/replica_exchange.py
--rw-rw----   0 sliu     (61642) sliu     (61642)    15174 2023-04-14 18:10:25.000000 openabc-1.0.2/src/openabc/utils/shadow_map.py
-drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/
--rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/PKG-INFO
--rw-rw----   0 sliu     (61642) sliu     (61642)     1562 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/SOURCES.txt
--rw-rw----   0 sliu     (61642) sliu     (61642)        1 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/dependency_links.txt
--rw-rw----   0 sliu     (61642) sliu     (61642)        8 2023-04-14 21:42:59.000000 openabc-1.0.2/src/openabc.egg-info/top_level.txt
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1080 2023-04-14 18:10:57.000000 openabc-1.0.3/LICENSE
+-rw-rw----   0 sliu     (61642) sliu     (61642)      121 2023-04-14 20:42:49.000000 openabc-1.0.3/MANIFEST.in
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-22 03:38:08.000000 openabc-1.0.3/PKG-INFO
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1094 2023-04-14 21:02:42.000000 openabc-1.0.3/README.md
+-rw-rw----   0 sliu     (61642) sliu     (61642)      428 2023-04-22 03:20:37.000000 openabc-1.0.3/pyproject.toml
+-rw-rw----   0 sliu     (61642) sliu     (61642)       38 2023-04-22 03:38:08.000000 openabc-1.0.3/setup.cfg
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/
+-rw-rw----   0 sliu     (61642) sliu     (61642)       23 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/__init__.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/
+-rw-rw----   0 sliu     (61642) sliu     (61642)       73 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11969 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/cg_model.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      114 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1316 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/angle_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4121 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/bond_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)      716 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/dihedral_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9268 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/nonbonded_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3281 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4779 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/hps_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3058 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/hps_zero_offset_model.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9863 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/moff_mrg_model.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/parameters/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4287 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/HPS_KR_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4904 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11557 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv
+-rw-rw----   0 sliu     (61642) sliu     (61642)     3372 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/parse_hps_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1231 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/parse_moff_parameters.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    12545 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parameters/template_MOFF.top
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/forcefields/parsers/
+-rw-rw----   0 sliu     (61642) sliu     (61642)      110 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     4016 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/hps_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9129 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/moff_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7485 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/parsers/mrg_parser.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     7347 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/forcefields/rigid.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc/utils/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9311 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/CA2AA.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/__init__.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11105 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/helper_functions.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     5142 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/insert.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    11519 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/legacy_shadow_map.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)     9107 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/replica_exchange.py
+-rw-rw----   0 sliu     (61642) sliu     (61642)    15160 2023-04-22 03:27:46.000000 openabc-1.0.3/src/openabc/utils/shadow_map.py
+drwxrwx---   0 sliu     (61642) sliu     (61642)        0 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1377 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/PKG-INFO
+-rw-rw----   0 sliu     (61642) sliu     (61642)     1562 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/SOURCES.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)        1 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/dependency_links.txt
+-rw-rw----   0 sliu     (61642) sliu     (61642)        8 2023-04-22 03:38:08.000000 openabc-1.0.3/src/openabc.egg-info/top_level.txt
```

### Comparing `openabc-1.0.2/LICENSE` & `openabc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/PKG-INFO` & `openabc-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openabc
-Version: 1.0.2
+Version: 1.0.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openabc-1.0.2/README.md` & `openabc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/cg_model.py` & `openabc-1.0.3/src/openabc/forcefields/cg_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 from openmmplumed import PlumedForce
 from openabc.forcefields.rigid import createRigidBodies
 import openabc.utils.helper_functions as helper_functions
 import sys
 import os
 
 class CGModel(object):
-    '''
+    """
     The general class with general methods that can be inherited by any other CG model classes. 
     
     Each child class of CGModel has to set self.bonded_attr_names, which is used to append molecules and set rigid bodies. 
-    '''
+    """
     def __init__(self):
-        '''
+        """
         Initialize. 
-        '''
+        """
         self.atoms = None
         
     def append_mol(self, new_mol, verbose=False):
-        '''
+        """
         The method can append new molecules by concatenating atoms and bonded interaction information saved in dataframes. 
         
         Parameters
         ----------
         new_mol : a consistent parser object or CG model object
             The object of a new molecule including atom and bonded interaction information. 
         
         verbose : bool
             Whether to report the appended attributes. 
         
-        '''
+        """
         new_atoms = new_mol.atoms.copy()
         if hasattr(self, 'atoms'):
             if self.atoms is None:
                 add_index = 0
                 self.atoms = new_atoms
             else:
                 add_index = len(self.atoms.index)
@@ -61,36 +61,36 @@
                             combined_attr = pd.concat([getattr(self, each_attr_name).copy(), new_attr], 
                                                       ignore_index=True)
                             setattr(self, each_attr_name, combined_attr)
                     else:
                         setattr(self, each_attr_name, new_attr)
     
     def atoms_to_pdb(self, cg_pdb, reset_serial=True):
-        '''
+        """
         Save atoms to pdb as topology will be read from the pdb file.
         PDB file is required for OpenMM simulation.
         
         Parameters
         ----------
         cg_pdb : str
             Output path for CG PDB file.
         
         reset_serial : bool
             Reset serial to 1, 2, ...
         
-        '''
+        """
         # do not write charge due to pdb space limit
         atoms = self.atoms.copy()
         atoms.loc[:, 'charge'] = ''
         if reset_serial:
             atoms['serial'] = list(range(1, len(atoms.index) + 1))
         helper_functions.write_pdb(atoms, cg_pdb)
     
     def create_system(self, top, use_pbc=True, box_a=500, box_b=500, box_c=500, remove_cmmotion=True):
-        '''
+        """
         Create OpenMM system for simulation. 
         Need to further add forces to this OpenMM system. 
         
         Parameters
         ----------
         top : OpenMM Topology
             The OpenMM topology. 
@@ -106,15 +106,15 @@
         
         box_c : float or int
             Box length along z-axis. 
         
         remove_cmmotion : bool
             Whether to add CMMotionRemover to remove center of mass motions. 
         
-        '''
+        """
         self.top = top
         self.use_pbc = use_pbc
         self.system = mm.System()
         if self.use_pbc:
             box_vec_a = np.array([box_a, 0, 0])*unit.nanometer
             box_vec_b = np.array([0, box_b, 0])*unit.nanometer
             box_vec_c = np.array([0, 0, box_c])*unit.nanometer
@@ -123,15 +123,15 @@
         for each in mass:
             self.system.addParticle(each)
         if remove_cmmotion:
             force = mm.CMMotionRemover()
             self.system.addForce(force)
     
     def set_rigid_bodies(self, rigid_coord, rigid_bodies, keep_unchanged=[]):
-        '''
+        """
         Set rigid bodies and remove bonded interactions within the same rigid body. 
         
         Directly run `createRigidBodies` if the user does not want to change any bonded interactions or exclusions.
         
         Parameters
         ----------
         rigid_coord : Quantity, shape = (n_atoms, 3)
@@ -139,15 +139,15 @@
         
         rigid_bodies : list 
             A list includes many sublists. Atoms in each sublist are recognized as one rigid body. 
         
         keep_unchanged : list
             A list including attribute names that user intends to keep unchanged. 
         
-        '''
+        """
         rigid_body_id_dict = {}
         for i in range(len(self.atoms.index)):
             rigid_body_id_dict[i] = None
         for i in range(len(rigid_bodies)):
             for j in rigid_bodies[i]:
                 rigid_body_id_dict[j] = i
         for each_attr_name in self.bonded_attr_names:
@@ -167,63 +167,63 @@
                                 flag = False
                         if flag:
                             new_attr.loc[len(new_attr.index)] = row
                     setattr(self, each_attr_name, new_attr)
         createRigidBodies(self.system, rigid_coord, rigid_bodies)
         
     def add_plumed(self, plumed_script_path):
-        '''
+        """
         Add OpenMM plumed. 
         
         Parameters
         ----------
         plumed_script_path : str
             Input plumed script path. 
         
         Reference
         ---------
             PLUMED website: https://www.plumed.org/
         
-        '''
+        """
         with open(plumed_script_path, 'r') as input_reader:
             force = PlumedForce(input_reader.read())
         self.system.addForce(force)
     
     def save_system(self, system_xml='system.xml'):
-        '''
+        """
         Save system to readable xml format. 
         
         Parameters
         ----------
         system_xml : str
             Output system xml file path. 
         
-        '''
+        """
         with open(system_xml, 'w') as output_writer:
             output_writer.write(mm.XmlSerializer.serialize(self.system))
     
     def save_state(self, state_xml='state.xml'):
-        '''
+        """
         Save simulation state to readable xml format. 
         
         Parameters
         ----------
         state_xml : str
             Output state xml file path. 
         
-        '''
+        """
         with open(state_xml, 'w') as output_writer:
             state = self.simulation.context.getState(getPositions=True, getVelocities=True, getForces=True, 
                                                      getEnergy=True, getParameters=True, 
                                                      enforcePeriodicBox=self.use_pbc)
             output_writer.write(mm.XmlSerializer.serialize(state))
     
     def set_simulation(self, integrator, platform_name='CPU', properties={'Precision': 'mixed'}, init_coord=None):
         platform = mm.Platform.getPlatformByName(platform_name)
-        '''
+        """
         Set OpenMM simulation.
         
         Parameters
         ----------
         integrator : OpenMM Integrator
             OpenMM integrator. 
         
@@ -232,31 +232,31 @@
         
         properties : dict
             OpenMM simulation platform properties. 
         
         init_coord : None or array-like
             Initial coordinate. 
         
-        '''
+        """
         print(f'Use platform: {platform_name}')
         if platform_name in ['CUDA', 'OpenCL']:
             if 'Precision' not in properties:
                 properties['Precision'] = 'mixed'
             precision = properties['Precision']
             print(f'Use precision: {precision}')
             self.simulation = app.Simulation(self.top, self.system, integrator, platform, properties)
         else:
             self.simulation = app.Simulation(self.top, self.system, integrator, platform)
         if init_coord is not None:
             self.simulation.context.setPositions(init_coord)
     
     def move_COM_to_box_center(self):
-        '''
+        """
         Move center of mass (COM) to simulation box center. 
-        '''
+        """
         print('Move center of mass (COM) to box center')
         state = self.simulation.context.getState(getPositions=True, enforcePeriodicBox=self.use_pbc)
         positions = np.array(state.getPositions().value_in_unit(unit.nanometer))
         n_atoms = positions.shape[0]
         mass = []
         for i in range(n_atoms):
             mass.append(self.system.getParticleMass(i).value_in_unit(unit.dalton))
@@ -268,15 +268,15 @@
         box_vec_c = np.array(box_vec_c.value_in_unit(unit.nanometer))
         box_center = 0.5*(box_vec_a + box_vec_b + box_vec_c)
         center_of_mass = np.average(positions, axis=0, weights=weights)
         positions = positions - center_of_mass + box_center
         self.simulation.context.setPositions(positions*unit.nanometer)
     
     def add_reporters(self, report_interval, output_dcd='output.dcd', report_dcd=True, report_state=True):
-        '''
+        """
         Add reporters for OpenMM simulation. 
         
         Parameters
         ----------
         report_interval : int
             Report dcd and report state interval.
         
@@ -285,15 +285,15 @@
         
         report_dcd : bool
             Whether to output dcd file. 
         
         report_state : bool
             Whether to output simulation state. 
         
-        '''
+        """
         if report_dcd:
             dcd_reporter = app.DCDReporter(output_dcd, report_interval, enforcePeriodicBox=self.use_pbc)
             self.simulation.reporters.append(dcd_reporter)
         if report_state:
             state_reporter = app.StateDataReporter(sys.stdout, report_interval, step=True, time=True, 
                                                    potentialEnergy=True, kineticEnergy=True, totalEnergy=True, 
                                                    temperature=True, speed=True)
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/functional_terms/angle_terms.py` & `openabc-1.0.3/src/openabc/forcefields/functional_terms/angle_terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pandas as pd
 import simtk.openmm as mm
 import simtk.openmm.app as app
 import simtk.unit as unit
 import sys
 import os
 
-
 def harmonic_angle_term(df_angles, use_pbc, force_group=2):
     angles = mm.HarmonicAngleForce()
     for i, row in df_angles.iterrows():
         a1 = int(row['a1'])
         a2 = int(row['a2'])
         a3 = int(row['a3'])
         theta0 = row['theta0']
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/functional_terms/bond_terms.py` & `openabc-1.0.3/src/openabc/forcefields/functional_terms/bond_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/functional_terms/dihedral_terms.py` & `openabc-1.0.3/src/openabc/forcefields/functional_terms/dihedral_terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pandas as pd
 import simtk.openmm as mm
 import simtk.openmm.app as app
 import simtk.unit as unit
 import sys
 import os
 
-
 def periodic_dihedral_term(df_dihedrals, use_pbc, force_group=3):
     dihedrals = mm.PeriodicTorsionForce()
     for i, row in df_dihedrals.iterrows():
         a1 = int(row['a1'])
         a2 = int(row['a2'])
         a3 = int(row['a3'])
         a4 = int(row['a4'])
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/functional_terms/nonbonded_terms.py` & `openabc-1.0.3/src/openabc/forcefields/functional_terms/nonbonded_terms.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,19 @@
     '''
     MOFF+MRG model nonbonded contact term.
     '''
     eta_value = eta.value_in_unit(unit.nanometer**-1)
     r0_value = r0.value_in_unit(unit.nanometer)
     cutoff_value = cutoff.value_in_unit(unit.nanometer)
     contacts = mm.CustomNonbondedForce(f'''energy;
-               energy=(alpha_con/(r^12)-0.5*epsilon_con*(1+tanh({eta_value}*({r0_value}-r)))-offset)*step({cutoff_value}-r);
-               offset=alpha_con/({cutoff_value}^12)-0.5*epsilon_con*(1+tanh({eta_value}*({r0_value}-{cutoff_value})));
+               energy=(energy1+energy2-offset1-offset2)*step({cutoff_value}-r);
+               energy1=alpha_con/(r^12);
+               energy2=-0.5*epsilon_con*(1+tanh({eta_value}*({r0_value}-r)));
+               offset1=alpha_con/({cutoff_value}^12);
+               offset2=-0.5*epsilon_con*(1+tanh({eta_value}*({r0_value}-{cutoff_value})));
                alpha_con=alpha_con_map(atom_type1, atom_type2);
                epsilon_con=epsilon_con_map(atom_type1, atom_type2);
                ''')
     n_atom_types = alpha_map.shape[0]
     discrete_2d_alpha_map = mm.Discrete2DFunction(n_atom_types, n_atom_types, alpha_map.ravel().tolist())
     discrete_2d_epsilon_map = mm.Discrete2DFunction(n_atom_types, n_atom_types, epsilon_map.ravel().tolist())
     contacts.addTabulatedFunction('alpha_con_map', discrete_2d_alpha_map)
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py` & `openabc-1.0.3/src/openabc/forcefields/functional_terms/zero_offset_nonbonded_terms.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/hps_model.py` & `openabc-1.0.3/src/openabc/forcefields/hps_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,42 +15,42 @@
                 'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
                 'LEU', 'LYS', 'MET', 'PHE', 'PRO',
                 'SER', 'THR', 'TRP', 'TYR', 'VAL']
 
 _kcal_to_kj = 4.184
 
 class HPSModel(CGModel):
-    '''
+    """
     A class for HPS model that represents a mixture of HPS model proteins. 
     
     This class inherits CGModel class. 
-    '''
+    """
     def __init__(self):
-        '''
+        """
         Initialize. 
-        '''
+        """
         self.atoms = None
         self.bonded_attr_names = ['protein_bonds', 'exclusions']
         
     def add_protein_bonds(self, force_group=1):
-        '''
+        """
         Add protein bonds. 
         
         Parameters
         ----------
         force_group : int
             Force group. 
         
-        '''
+        """
         print('Add protein bonds.')
         force = bond_terms.harmonic_bond_term(self.protein_bonds, self.use_pbc, force_group)
         self.system.addForce(force)
     
     def add_contacts(self, hydropathy_scale='Urry', epsilon=0.2*_kcal_to_kj, mu=1, delta=0.08, force_group=2):
-        '''
+        """
         Add nonbonded contacts. 
         
         The raw hydropathy scale is scaled and shifted by: mu*lambda - delta
         
         Parameters
         ----------
         hydropathy_scale : str
@@ -64,15 +64,15 @@
         
         delta : float or int
             Hydropathy shift factor. 
         
         force_group : int
             Force group. 
             
-        '''
+        """
         print('Add nonbonded contacts.')
         resname_list = self.atoms['resname'].tolist()
         atom_types = [_amino_acids.index(x) for x in resname_list]
         if hydropathy_scale == 'KR':
             print('Use KR hydropathy scale.')
             df_contact_parameters = pd.read_csv(f'{__location__}/parameters/HPS_KR_parameters.csv')
         elif hydropathy_scale == 'Urry':
@@ -91,15 +91,15 @@
         print(f'Scale factor mu = {mu} and shift delta = {delta}.')
         lambda_ah_map = mu*lambda_ah_map - delta
         force = nonbonded_terms.hps_ah_term(atom_types, self.exclusions, self.use_pbc, epsilon, sigma_ah_map, 
                                             lambda_ah_map, force_group)
         self.system.addForce(force)
     
     def add_dh_elec(self, ldby=1*unit.nanometer, dielectric_water=80.0, cutoff=3.5*unit.nanometer, force_group=3):
-        '''
+        """
         Add Debye-Huckel electrostatic interactions. 
         
         Parameters
         ----------
         ldby : Quantity
             Debye length. 
         
@@ -108,26 +108,26 @@
         
         cutoff : Quantity
             Cutoff distance. 
         
         force_group : int
             Force group. 
         
-        '''
+        """
         print('Add Debye-Huckel electrostatic interactions.')
         print(f'Set Debye length as {ldby.value_in_unit(unit.nanometer)} nm.')
         print(f'Set water dielectric as {dielectric_water}.')
         charges = self.atoms['charge'].tolist()
         force = nonbonded_terms.dh_elec_term(charges, self.exclusions, self.use_pbc, ldby, dielectric_water, cutoff, 
                                              force_group)
         self.system.addForce(force)
 
     def add_all_default_forces(self):
-        '''
+        """
         Add all the forces with default settings. 
-        '''
+        """
         print('Add all the forces with default settings.')
         self.add_protein_bonds(force_group=1)
         self.add_contacts(force_group=2)
         self.add_dh_elec(force_group=3)
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/hps_zero_offset_model.py` & `openabc-1.0.3/src/openabc/forcefields/hps_zero_offset_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
                 'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
                 'LEU', 'LYS', 'MET', 'PHE', 'PRO',
                 'SER', 'THR', 'TRP', 'TYR', 'VAL']
 
 _kcal_to_kj = 4.184
 
 class HPSZeroOffsetModel(HPSModel):
-    '''
+    """
     An HPS model with zero offset for nonbonded interactions. 
     This model is only used for comparisons, as HOOMD-Blue HPS model does not shift nonbonded potential to zero at cutoff. 
-    '''
+    """
     def add_contacts(self, hydropathy_scale='Urry', epsilon=0.2*_kcal_to_kj, mu=1, delta=0.08, force_group=2):
         print('Add nonbonded contacts.')
         resname_list = self.atoms['resname'].tolist()
         atom_types = [_amino_acids.index(x) for x in resname_list]
         if hydropathy_scale == 'KR':
             print('Use KR hydropathy scale.')
             df_contact_parameters = pd.read_csv(f'{__location__}/parameters/HPS_KR_parameters.csv')
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/moff_mrg_model.py` & `openabc-1.0.3/src/openabc/forcefields/moff_mrg_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,135 +14,135 @@
                 'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
                 'LEU', 'LYS', 'MET', 'PHE', 'PRO',
                 'SER', 'THR', 'TRP', 'TYR', 'VAL']
 
 _nucleotides = ['DA', 'DC', 'DG', 'DT']
 
 class MOFFMRGModel(CGModel):
-    '''
+    """
     A class for MOFF+MRG model that represents a mixture of MOFF proteins and MRG DNA. 
-    '''
+    """
     def __init__(self):
-        '''
+        """
         Initialize. 
-        '''
+        """
         self.atoms = None
         self.bonded_attr_names = ['protein_bonds', 'protein_angles', 'protein_dihedrals', 'native_pairs', 'dna_bonds', 
                                   'dna_angles', 'dna_fan_bonds', 'exclusions']
 
     def add_protein_bonds(self, force_group=1):
-        '''
+        """
         Add protein bonds.
         
         Parameters
         ----------
         
         force_group : int
             Force group. 
         
-        '''
+        """
         if hasattr(self, 'protein_bonds'):
             print('Add protein bonds.')
             force = functional_terms.harmonic_bond_term(self.protein_bonds, self.use_pbc, force_group)
             self.system.addForce(force)
 
     def add_protein_angles(self, force_group=2):
-        '''
+        """
         Add protein angles.
         
         Parameters
         ----------
         force_group : int
             Force group. 
         
-        '''
+        """
         if hasattr(self, 'protein_angles'):
             print('Add protein angles.')
             force = functional_terms.harmonic_angle_term(self.protein_angles, self.use_pbc, force_group)
             self.system.addForce(force)
     
     def add_protein_dihedrals(self, k_dihedral_1=3.0, k_dihedral_3=1.5, force_group=3):
-        '''
+        """
         Add protein dihedrals. 
         
         Parameters
         ----------
         force_group : int
             Force group. 
         
-        '''
+        """
         if hasattr(self, 'protein_dihedrals'):
             print('Add protein dihedrals.')
             force = functional_terms.periodic_dihedral_term(self.protein_dihedrals, self.use_pbc, force_group)
             self.system.addForce(force)
     
     def add_native_pairs(self, force_group=4):
-        '''
+        """
         Add native pairs. 
         
         Parameters
         ----------
         force_group : int
             Force group.
         
-        '''
+        """
         if hasattr(self, 'native_pairs'):
             print('Add native pairs.')
             force = functional_terms.native_pair_12_10_term(self.native_pairs, self.use_pbc, force_group)
             self.system.addForce(force)
 
     def add_dna_bonds(self, force_group=5):
-        '''
+        """
         Add DNA bonds. 
         
         Parameters
         ----------
         force_group : int
             Force group. 
         
-        '''
+        """
         if hasattr(self, 'dna_bonds'):
             print('Add DNA bonds.')
             force = functional_terms.class2_bond_term(self.dna_bonds, self.use_pbc, force_group)
             self.system.addForce(force)
     
     def add_dna_angles(self, force_group=6):
-        '''
+        """
         Add DNA angles. 
         
         Parameters
         ----------
         force_group : int
             Force group. 
         
-        '''
+        """
         if hasattr(self, 'dna_angles'):
             print('Add DNA angles.')
             force = functional_terms.class2_angle_term(self.dna_angles, self.use_pbc, force_group)
             self.system.addForce(force)
         
     def add_dna_fan_bonds(self, force_group=7):
-        '''
+        """
         Add DNA fan bonds. 
         
         Parameters
         ----------
         force_group : int
             Force group. 
         
-        '''
+        """
         if hasattr(self, 'dna_fan_bonds'):
             print('Add DNA fan bonds.')
             force = functional_terms.class2_bond_term(self.dna_fan_bonds, self.use_pbc, force_group)
             self.system.addForce(force)
     
     def add_contacts(self, eta=0.7/unit.angstrom, r0=8*unit.angstrom, cutoff=2.0*unit.nanometer, 
                      alpha_protein_dna=1.6264e-3, alpha_dna_dna=1.678e-5, epsilon_protein_dna=0, epsilon_dna_dna=0, 
                      force_group=8):
-        '''
+        """
         Add nonbonded contacts for MOFF protein and MRG DNA. 
         
         For amino acids, the CA atom type indices are 0-19, and CG nucleotide atom type index is 20. 
         
         The potential expression is: alpha/r^12 - 0.5*epsilon*(1 + tanh(eta*(r0 - r)))
         
         Parameters
@@ -167,15 +167,15 @@
         
         epsilon_dna_dna : float or int
             DNA-DNA interaction parameter epsilon. 
         
         force_group : int
             Force group.  
         
-        '''
+        """
         print('Add protein and DNA nonbonded contacts.')
         atom_types = []
         for i, row in self.atoms.iterrows():
             if (row['resname'] in _amino_acids) and (row['name'] == 'CA'):
                 atom_types.append(_amino_acids.index(row['resname']))
             elif (row['resname'] in _nucleotides) and (row['name'] == 'NU'):
                 atom_types.append(20)
@@ -199,15 +199,15 @@
         force = functional_terms.moff_mrg_contact_term(atom_types, self.exclusions, self.use_pbc, alpha_map, 
                                                        epsilon_map, eta, r0, cutoff, force_group)
         self.system.addForce(force)
     
     def add_elec_switch(self, salt_conc=150.0*unit.millimolar, temperature=300.0*unit.kelvin, 
                         cutoff1=1.2*unit.nanometer, cutoff2=1.5*unit.nanometer, switch_coeff=[1, 0, 0, -10, 15, -6], 
                         add_native_pair_elec=True, force_group=9):
-        '''
+        """
         Add electrostatic interaction with switch function. 
         
         The switch function switches potential to zero within range cutoff1 < r <= cutoff2. 
         
         Parameters
         ----------
         salt_conc : Quantity
@@ -227,15 +227,15 @@
         
         add_native_pair_elec : bool
             Whether to add electrostatic interactions between native pairs. 
         
         force_group : int
             Force group. 
         
-        '''
+        """
         print('Add protein and DNA electrostatic interactions with distance-dependent dielectric and switch.')
         charges = self.atoms['charge'].tolist()
         force1 = functional_terms.ddd_dh_elec_switch_term(charges, self.exclusions, self.use_pbc, salt_conc, 
                                                           temperature, cutoff1, cutoff2, switch_coeff, force_group)
         self.system.addForce(force1)
         if add_native_pair_elec and hasattr(self, 'native_pairs'):
             print('Add electrostatic interactions between native pair atoms.')
@@ -249,17 +249,17 @@
                                                                    temperature, cutoff1, cutoff2, switch_coeff, 
                                                                    force_group)
             self.system.addForce(force2)
         else:
             print('Do not add electrostatic interactions between native pair atoms.')
         
     def add_all_default_forces(self):
-        '''
+        """
         Add all the forces with default settings. 
-        '''
+        """
         print('Add all the forces with default settings.')
         self.add_protein_bonds()
         self.add_protein_angles()
         self.add_protein_dihedrals()
         self.add_native_pairs()
         self.add_dna_bonds()
         self.add_dna_angles()
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/parameters/HPS_KR_parameters.csv` & `openabc-1.0.3/src/openabc/forcefields/parameters/HPS_KR_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv` & `openabc-1.0.3/src/openabc/forcefields/parameters/HPS_Urry_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv` & `openabc-1.0.3/src/openabc/forcefields/parameters/MOFF_contact_parameters.csv`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/parameters/parse_hps_parameters.py` & `openabc-1.0.3/src/openabc/forcefields/parameters/parse_hps_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pandas as pd
 
-'''
+"""
 Use this script to produce the .csv files for HPS model nonbonded interaction parameters. 
 There are two sets of hydrophobicity scales (KR scale and Urry scale). 
-'''
+"""
 
 _amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
                 'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
                 'LEU', 'LYS', 'MET', 'PHE', 'PRO',
                 'SER', 'THR', 'TRP', 'TYR', 'VAL']
 
 _normalized_KR_hydropathy_scale = dict(ALA=0.730, ARG=0.000, ASN=0.432, ASP=0.378,
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/parameters/parse_moff_parameters.py` & `openabc-1.0.3/src/openabc/forcefields/parameters/parse_moff_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
 import sys
 import os
 
-'''
+"""
 Use this script to produce the .csv files for MOFF nonbonded interaction parameters. 
 The nonbonded interaction form is: abs(epsilon)*(sigma^12)/(r^12)-0.5*epsilon*(1+tanh(eta*(r0-r))).
 Set alpha=abs(epsilon)*(sigma^12).
-'''
+"""
 df_contact_parameters = pd.DataFrame(columns=['atom_type1', 'atom_type2', 'alpha', 'epsilon', 'sigma'])
 
 with open('template_MOFF.top', 'r') as input_reader:
     template_MOFF_lines = input_reader.readlines()
 
 n_lines = len(template_MOFF_lines)
 for i in range(n_lines):
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/parameters/template_MOFF.top` & `openabc-1.0.3/src/openabc/forcefields/parameters/template_MOFF.top`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/forcefields/parsers/hps_parser.py` & `openabc-1.0.3/src/openabc/forcefields/parsers/hps_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,41 +21,41 @@
                                   GLN=0.0, GLU=-1.0, GLY=0.0, HIS=0.5, ILE=0.0,
                                   LEU=0.0, LYS=1.0, MET=0.0, PHE=0.0, PRO=0.0,
                                   SER=0.0, THR=0.0, TRP=0.0, TYR=0.0, VAL=0.0)
 
 _kcal_to_kj = 4.184
 
 class HPSParser(object):
-    '''
+    """
     HPS protein parser.
-    '''
+    """
     def __init__(self, ca_pdb, default_parse=True):
-        '''
+        """
         Initialize a protein with HPS model.
         
         Parameters
         ----------
         ca_pdb : str
             Path for the CA pdb file. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
-        '''
+        """
         self.pdb = ca_pdb
         self.atoms = helper_functions.parse_pdb(ca_pdb)
         # check if all the atoms are protein CA atoms
         assert ((self.atoms['resname'].isin(_amino_acids)).all() and self.atoms['name'].eq('CA').all())
         if default_parse:
             print('Parse molecule with default settings.')
             self.parse_mol()
     
     @classmethod
     def from_atomistic_pdb(cls, atomistic_pdb, ca_pdb, write_TER=False, default_parse=True):
-        '''
+        """
         Initialize an HPS model protein from atomistic pdb. 
         
         Parameters
         ----------
         atomistic_pdb : str
             Path for the atomistic pdb file. 
         
@@ -64,35 +64,35 @@
         
         write_TER : bool
             Whether to write TER between two chains. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
-        '''
+        """
         helper_functions.atomistic_pdb_to_ca_pdb(atomistic_pdb, ca_pdb, write_TER)
         return cls(ca_pdb, default_parse)
     
     def parse_mol(self, exclude12=True, mass_dict=_hps_amino_acid_mass_dict, 
                      charge_dict=_hps_amino_acid_charge_dict):
-        '''
+        """
         Parse molecule. 
         
         Parameters
         ----------
         exclude12 : bool
             Whether to exclude nonbonded interactions between 1-2 atoms. 
         
         mass_dict : dict
             Mass dictionary. 
         
         charge_dict : dict
             Charge dictionary. 
         
-        '''
+        """
         bonds = []
         n_atoms = len(self.atoms.index)
         for atom1 in range(n_atoms):
             chain1 = self.atoms.loc[atom1, 'chainID']
             if atom1 < n_atoms - 1:
                 atom2 = atom1 + 1
                 chain2 = self.atoms.loc[atom2, 'chainID']
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/parsers/moff_parser.py` & `openabc-1.0.3/src/openabc/forcefields/parsers/moff_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,45 +23,45 @@
                                     GLN=0.0, GLU=-1.0, GLY=0.0, HIS=0.25, ILE=0.0,
                                     LEU=0.0, LYS=1.0, MET=0.0, PHE=0.0, PRO=0.0,
                                     SER=0.0, THR=0.0, TRP=0.0, TYR=0.0, VAL=0.0)
 
 _kcal_to_kj = 4.184
 
 class MOFFParser(object):
-    '''
+    """
     MOFF protein parser.
-    '''
+    """
     def __init__(self, atomistic_pdb, ca_pdb, default_parse=True):
-        '''
+        """
         Initialize a protein with MOFF model. 
         
         Parameters
         ----------
         atomistic_pdb : str
             Path for the atomistic pdb file. 
         
         ca_pdb : str
             path for the CA pdb file. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
-        '''
+        """
         self.atomistic_pdb = atomistic_pdb
         self.pdb = ca_pdb
         self.atoms = helper_functions.parse_pdb(ca_pdb)
         # check if all the atoms are protein CA atoms
         assert ((self.atoms['resname'].isin(_amino_acids)).all() and self.atoms['name'].eq('CA').all())
         if default_parse:
             print('Parse molecule with default settings.')
             self.parse_mol()
 
     @classmethod
     def from_atomistic_pdb(cls, atomistic_pdb, ca_pdb, write_TER=False, default_parse=True):
-        '''
+        """
         Initialize an HPS model protein from atomistic pdb. 
         
         Parameters
         ----------
         atomistic_pdb : str
             Path for the atomistic pdb file. 
         
@@ -70,20 +70,20 @@
             
         write_TER : bool
             Whether to write TER between two chains. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
-        '''
+        """
         helper_functions.atomistic_pdb_to_ca_pdb(atomistic_pdb, ca_pdb, write_TER)
         return cls(atomistic_pdb, ca_pdb, default_parse)
     
     def parse_exclusions(self, exclude12=True, exclude13=True, exclude14=True, exclude_native_pairs=True):
-        '''
+        """
         Parse nonbonded exclusions based on bonds, angles, dihedrals, and native pairs.
         
         Parameters
         ----------
         exclude12 : bool
             Whether to exclude nonbonded interactions between 1-2 atom pairs. 
         
@@ -92,15 +92,15 @@
         
         exclude14 : bool
             Whether to exclude nonbonded interactions between 1-4 atom pairs. 
         
         exclude_native_pairs : bool
             Whether to exclude nonbonded interactions between native pairs. 
         
-        '''
+        """
         exclusions = []
         if exclude12 and hasattr(self, 'protein_bonds'):
             for i, row in self.protein_bonds.iterrows():
                 exclusions.append((int(row['a1']), int(row['a2'])))
         if exclude13 and hasattr(self, 'protein_angles'):
             for i, row in self.protein_angles.iterrows():
                 exclusions.append((int(row['a1']), int(row['a3'])))
@@ -112,15 +112,15 @@
                 exclusions.append((int(row['a1']), int(row['a2'])))
         exclusions = np.array(sorted(exclusions))
         self.exclusions = pd.DataFrame(exclusions, columns=['a1', 'a2']).drop_duplicates(ignore_index=True)
         
     def parse_mol(self, get_native_pairs=True, frame=0, radius=0.1, bonded_radius=0.05, cutoff=0.6, box=None, 
                   use_pbc=False, exclude12=True, exclude13=True, exclude14=True, exclude_native_pairs=True, 
                   mass_dict=_moff_amino_acid_mass_dict, charge_dict=_moff_amino_acid_charge_dict):
-        '''
+        """
         Parse molecule.
         
         Parameters
         ----------
         get_native_pairs : bool
             Whether to get native pairs from atomistic pdb with shadow algorithm. 
         
@@ -159,15 +159,15 @@
         
         mass_dict : dict
             Mass dictionary. 
         
         charge_dict : dict
             Charge dictionary. 
         
-        '''
+        """
         # set bonds, angles, and dihedrals
         bonds, angles, dihedrals = [], [], []
         n_atoms = len(self.atoms.index)
         for atom1 in range(n_atoms):
             chain1 = self.atoms.loc[atom1, 'chainID']
             if atom1 < n_atoms - 1:
                 atom2 = atom1 + 1
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/parsers/mrg_parser.py` & `openabc-1.0.3/src/openabc/forcefields/parsers/mrg_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,31 +27,31 @@
                                              [9.55, -45.9, 50.2], 
                                              [13.78, -52.7, 50], 
                                              [13.86, -56.8, 50], 
                                              [36.26, -77, 50]])
 _r0_mrg_dna_fan_bonds = np.array([1.71, 1.635, 1.47, 1.345, 1.23, 1.13, 0.99, 0.92, 1.02, 1.25, 1.69])
 
 class MRGdsDNAParser(object):
-    '''
+    """
     MRG dsDNA parser. 
     Note this parser only works on one dsDNA!
-    '''
+    """
     def __init__(self, cg_pdb, default_parse=True):
-        '''
+        """
         Initialize a dsDNA with MRG model. 
         
         Parameters
         ----------
         cg_pdb : str
             Path for the CG dsDNA pdb. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
-        '''
+        """
         self.pdb = cg_pdb
         self.atoms = helper_functions.parse_pdb(self.pdb)
         # check if all the atoms are CG nucleotide atoms
         atom_names = self.atoms['name']
         assert (self.atoms['resname'].isin(_nucleotides).all() and atom_names.eq('NU').all())
         # check if there are only 2 chains
         unique_chainID = list(set(self.atoms['chainID'].tolist()))
@@ -66,15 +66,15 @@
         assert second_half_atoms['chainID'].eq(second_half_atoms['chainID'].iloc[0]).all()
         if default_parse:
             print('Parse molecule with default settings.')
             self.parse_mol()
     
     @classmethod
     def from_atomistic_pdb(cls, atomistic_pdb, cg_pdb, write_TER=False, default_parse=True):
-        '''
+        """
         Initialize an MRG model dsDNA from atomistic pdb. 
         
         Parameters
         ----------
         atomistic_pdb : str
             Path for the atomistic dsDNA pdb file. 
         
@@ -83,44 +83,44 @@
         
         write_TER : bool
             Whether to write TER between two chains. 
         
         default_parse : bool
             Whether to parse with default settings. 
         
-        '''
+        """
         helper_functions.atomistic_pdb_to_nucleotide_pdb(atomistic_pdb, cg_pdb, write_TER)
         return cls(cg_pdb, default_parse)
     
     def parse_exclusions(self, exclude12=True, exclude13=True):
-        '''
+        """
         Parse nonbonded exclusions based on bonds and angles. 
         Note nonbonded interactions are not excluded for atom pairs with fan bonds. 
         
         Parameters
         ----------
         exclude12 : bool
             Whether to exclude nonbonded interactions between 1-2 atom pairs. 
         
         exclude13 : bool
             Whether to exclude nonbonded interactions between 1-3 atom pairs. 
         
-        '''
+        """
         exclusions = []
         if exclude12 and hasattr(self, 'dna_bonds'):
             for i, row in self.dna_bonds.iterrows():
                 exclusions.append((int(row['a1']), int(row['a2'])))
         if exclude13 and hasattr(self, 'dna_angles'):
             for i, row in self.dna_angles.iterrows():
                 exclusions.append((int(row['a1']), int(row['a3'])))
         exclusions = np.array(sorted(exclusions))
         self.exclusions = pd.DataFrame(exclusions, columns=['a1', 'a2']).drop_duplicates(ignore_index=True)
     
     def parse_mol(self, exclude12=True, exclude13=True, bonded_energy_scale=0.9, mass=325, charge=-1):
-        '''
+        """
         Parse molecule.
         
         Parameters
         ----------
         exclude12 : bool
             Whether to exclude nonbonded interactions between 1-2 atom pairs. 
         
@@ -132,15 +132,15 @@
         
         mass : float or int
             Mass of CG nucleotide bead. 
         
         charge : float or int
             Charge of each CG nucleotide bead. 
         
-        '''
+        """
         # set bonds and angles
         bonds, angles = [], []
         n_atoms = len(self.atoms.index)
         for atom1 in range(n_atoms):
             chain1 = self.atoms.loc[atom1, 'chainID']
             if atom1 < n_atoms - 1:
                 atom2 = atom1 + 1
```

### Comparing `openabc-1.0.2/src/openabc/forcefields/rigid.py` & `openabc-1.0.3/src/openabc/forcefields/rigid.py`

 * *Files identical despite different names*

### Comparing `openabc-1.0.2/src/openabc/utils/CA2AA.py` & `openabc-1.0.3/src/openabc/utils/CA2AA.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,39 +13,39 @@
 import warnings
 from openabc.utils.helper_functions import parse_pdb, write_pdb
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
 __author__ = 'Cong Wang'
 
-'''
+"""
 This python script calls REMO (https://zhanggroup.org/REMO/) to reconstruct atomic configurations for protein condensates.
-'''
+"""
 
 
 default_REMO_path = __location__ + '/REMO'
 
 def args_parse():
-    '''
+    """
     The function uses argparse module to create and manage the command-line interface.
 
     Returns
     -------
     parser.parse_args(): the parsed command-line arguments object.
-    '''
+    """
     parser = argparse.ArgumentParser()
     parser.add_argument('-i', '--input_file', type=str, help='A string that represents the path to the input protein PDB file')
     parser.add_argument('-N', '--number_of_chains', nargs='+', type=int, help='A list of integers, where each element represents the number of chains for a particular protein type')
     parser.add_argument('-n', '--number_of_residues', nargs='+', type=int, help='A list of integers, where each element represents the number of residues for a particular protein type')
     parser.add_argument('-d', '--debug', action='store_true', help='A boolen variable that has a default value of False. By default this script does not store temporary files')
     return parser.parse_args()
 
 
 def split_protein(input_pdbfile, num_chains, num_residues, output_path):
-    '''
+    """
     Split a PDB file containing multiple chains into individual files, each containing one chain.
     
     Parameters
     ----------
     input_pdbfile : str
         Input pdb file. 
     
@@ -55,15 +55,15 @@
     num_residues : list
         Length of protein chains in the system. Each element of the list represent one type of protein. 
         Note `num_chains` and `num_residues` share the same length unit. 
 
     output_path : str
         The folder where user wants to save output pdb files.  
            
-    '''
+    """
     pdb = parse_pdb(input_pdbfile)
     assert len(num_chains) == len(num_residues)
     protein_types = len(num_chains)
     current_index = 0
     os.makedirs(f'{output_path}', exist_ok=True)
     for i in range(protein_types):
         for j in range(num_chains[i]):
@@ -72,15 +72,15 @@
             current_index += num_residues[i]
     if current_index != len(pdb):
         raise ValueError(f'Number of CA in pdb file not consistant with num_chains and num_residues.')
     return
 
 
 def single_chain_CA2AA(input_pdbfile, output_pdbfile, REMO_path=default_REMO_path, debug=False):
-    '''
+    """
     Reconstruct all-atom representation for a single-chain protein from its alpha carbons using REMO.
     
     Parameters
     ----------
     input_pdbfile : str
         Input pdb file that contains one protein chain. 
     
@@ -93,15 +93,15 @@
     debug : bool, default=False
         If True, temporary files will not be deleted.
     
     References
     ----------
     Yunqi Li and Yang Zhang. REMO: A new protocol to refine full atomic protein models from C-alpha traces by optimizing hydrogen-bonding networks. Proteins, 2009, 76: 665-676.
     https://zhanggroup.org/REMO/.
-    '''
+    """
     REMO_path = os.path.expanduser(REMO_path)
     if not os.path.exists(f'{REMO_path}/REMO.pl'):
         raise FileNotFoundError(f'REMO.pl not found in {REMO_path}')
     output_pdbfile_path = '/'.join(output_pdbfile.split('/')[:-1])
     os.makedirs(output_pdbfile_path, exist_ok=True)
     if debug:
         subprocess.run([f'{REMO_path}/REMO.pl', '0', input_pdbfile])
@@ -111,15 +111,15 @@
                         stderr=subprocess.STDOUT)
     subprocess.run(['mv', f'{input_pdbfile}.h', output_pdbfile])
     subprocess.run(['rm', 'PRHB'])
     return
 
 
 def align_protein(input_pdbfile, reference_pdbfile, output_pdbfile, reference_atoms='CA'):
-    '''
+    """
     Align a protein with the reference protein accoding to positions of alpha carbons.
     
     Parameters
     ----------
     input_pdbfile : str
         Input pdb file to be aligned. 
     
@@ -133,15 +133,15 @@
     reference_atoms : str, default='CA'
         Name of the atoms that used as reference atoms. Currently only support alpha carbons.
     
     References
     ----------
     Yunqi Li and Yang Zhang. REMO: A new protocol to refine full atomic protein models from C-alpha traces by optimizing hydrogen-bonding networks. Proteins, 2009, 76: 665-676.
     https://zhanggroup.org/REMO/.
-    '''
+    """
     input_pdb = mdtraj.load(input_pdbfile)
     ref_pdb = mdtraj.load(reference_pdbfile)
     input_pdb_CA_index = input_pdb.top.select(f'name=={reference_atoms}')
     ref_pdb_CA_index= ref_pdb.top.select(f'name=={reference_atoms}')
     assert len(input_pdb_CA_index) == len(ref_pdb_CA_index)
     input_pdb_aligned = input_pdb.superpose(
                                             ref_pdb, 
@@ -152,37 +152,36 @@
     output_pdbfile_path = '/'.join(output_pdbfile.split('/')[:-1])
     os.makedirs(output_pdbfile_path, exist_ok=True)
     input_pdb_aligned.save(output_pdbfile)
     return
 
 
 def combine_proteins(pdbfile_lis, output_pdbflie):
-    '''
+    """
     Merge multiple pdb files into a single pdb file.
     
     Parameters
     ----------
     pdbfile_lis : str
         List that contains name of pdb files to be merged. 
     
     output_pdbfile : str
         Merged pdb file.
         
-    '''
-
+    """
     pdb_list = [mdtraj.load(i) for i in pdbfile_lis]
     pdb_combined = pdb_list[0]
     for i in range(len(pdb_list) - 1):
         pdb_combined = pdb_combined.stack(pdb_list[i + 1])
     pdb_combined.save(output_pdbflie)
     return
 
 
 def multiple_chains_CA2AA(input_pdbfile, num_chains, num_residues, REMO_path=default_REMO_path, debug=False):
-    '''
+    """
     Reconstruct all-atom representation of a multiple-chain protein from its alpha carbons. If the name of input file is 'XXX.pdb', then output will be saved as 'XXX_AA.pdb' in the folder where 'XXX.pdb' is located.
     
     Parameters
     ----------
     input_pdbfile : str
         Input pdb file. 
 
@@ -199,15 +198,15 @@
     debug : bool, default=False
         If True, temporary files will not be deleted.
 
     References
     ----------
     Yunqi Li and Yang Zhang. REMO: A new protocol to refine full atomic protein models from C-alpha traces by optimizing hydrogen-bonding networks. Proteins, 2009, 76: 665-676.
     https://zhanggroup.org/REMO/.
-    '''
+    """
     assert len(num_chains) == len(num_residues)
     pdb_name = input_pdbfile.split('/')[-1].split('.')[0]
     split_protein(input_pdbfile, num_chains, num_residues, output_path=f'{pdb_name}/ca_splitted')
     aligned_protein_list = []
     for i in tqdm(range(len(num_chains))):
         for j in tqdm(range(num_chains[i])):
             single_chain_CA2AA(
```

### Comparing `openabc-1.0.2/src/openabc/utils/helper_functions.py` & `openabc-1.0.3/src/openabc/utils/helper_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 import pandas as pd
 import mdtraj
 import sys
 import os
 
-'''
+"""
 Some code is adapted from Open3SPN2. 
 
 Open3SPN2 and OpenAWSEM paper: 
 Lu, Wei, et al. "OpenAWSEM with Open3SPN2: A fast, flexible, and accessible framework for large-scale coarse-grained biomolecular simulations." PLoS computational biology 17.2 (2021): e1008308.
-'''
+"""
 
 _amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
                 'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
                 'LEU', 'LYS', 'MET', 'PHE', 'PRO',
                 'SER', 'THR', 'TRP', 'TYR', 'VAL']
 
 _nucleotides = ['DA', 'DC', 'DG', 'DT']
@@ -21,28 +21,28 @@
 _amino_acid_1_letter_to_3_letters_dict = dict(A='ALA', R='ARG', N='ASN', D='ASP', C='CYS', 
                                               Q='GLN', E='GLU', G='GLY', H='HIS', I='ILE', 
                                               L='LEU', K='LYS', M='MET', F='PHE', P='PRO', 
                                               S='SER', T='THR', W='TRP', Y='TYR', V='VAL')
 
 
 def parse_pdb(pdb_file):
-    '''
+    """
     Load pdb file as pandas dataframe.
     
     Parameters
     ----------
     pdb_file : str
         Path for the pdb file. 
     
     Returns
     -------
     pdb_atoms : pd.DataFrame
         A pandas dataframe includes atom information. 
     
-    '''
+    """
     def pdb_line(line):
         return dict(recname=str(line[0:6]).strip(),
                     serial=int(line[6:11]),
                     name=str(line[12:16]).strip(),
                     altLoc=str(line[16:17]),
                     resname=str(line[17:20]).strip(),
                     chainID=str(line[21:22]),
@@ -65,89 +65,89 @@
                            'resname', 'chainID', 'resSeq', 'iCode',
                            'x', 'y', 'z', 'occupancy', 'tempFactor',
                            'element', 'charge']]
     return pdb_atoms
 
 
 def write_pdb(pdb_atoms, pdb_file, write_TER=False):
-    '''
+    """
     Write pandas dataframe to pdb file. 
     
     Parameters
     ----------
     pdb_atoms : pd.DataFrame
         A pandas dataframe includes atom information. 
     
     pdb_file : str
         Output path for the pdb file. 
     
     write_TER : bool
         Whether to write TER between two chains. 
 
-    '''
+    """
     chainID = None
     with open(pdb_file, 'w') as pdb:
         for i, atom in pdb_atoms.iterrows():
             if chainID is not None:
                 if write_TER and (atom['chainID'] != chainID):
                     pdb.write('TER\n')
             chainID = atom['chainID']
-            pdb_line = f'{atom.recname:<6}{atom.serial:>5} {atom["name"]:^4}{atom.altLoc:1}'+\
-                       f'{atom.resname:<3} {atom.chainID:1}{atom.resSeq:>4}{atom.iCode:1}   '+\
+            pdb_line = f'{atom.recname:<6}{int(atom.serial):>5} {atom["name"]:^4}{atom.altLoc:1}'+\
+                       f'{atom.resname:<3} {atom.chainID:1}{int(atom.resSeq):>4}{atom.iCode:1}   '+\
                        f'{atom.x:>8.3f}{atom.y:>8.3f}{atom.z:>8.3f}' +\
                        f'{atom.occupancy:>6.2f}{atom.tempFactor:>6.2f}'+' ' * 10 +\
                        f'{atom.element:>2}{atom.charge:>2}'
             assert len(pdb_line) == 80, f'An item in the atom table is longer than expected ({len(pdb_line)})\n{pdb_line}'
             pdb.write(pdb_line + '\n')
         pdb.write('END\n')
 
 
 def atomistic_pdb_to_ca_pdb(atomistic_pdb, ca_pdb, write_TER=False):
-    '''
+    """
     Convert atomistic pdb to protein CA pdb. 
     
     Parameters
     ----------
     atomistic_pdb : str
         Path for the atomistic pdb file. 
     
     ca_pdb : str
         Output path for the CA pdb file. 
     
     write_TER : bool
         Whether to write TER between two chains. 
     
-    '''
+    """
     atomistic_pdb_atoms = parse_pdb(atomistic_pdb)
     ca_pdb_atoms = pd.DataFrame(columns=atomistic_pdb_atoms.columns)
     for i, row in atomistic_pdb_atoms.iterrows():
         if (row['resname'] in _amino_acids) and (row['name'] == 'CA'):
             ca_pdb_atoms.loc[len(ca_pdb_atoms.index)] = row
     ca_pdb_atoms['serial'] = list(range(1, len(ca_pdb_atoms.index) + 1))
     ca_pdb_atoms.loc[:, 'charge'] = '' # remove charge
     write_pdb(ca_pdb_atoms, ca_pdb, write_TER)
     
 
 def atomistic_pdb_to_nucleotide_pdb(atomistic_pdb, cg_nucleotide_pdb, write_TER=False):
-    '''
+    """
     Convert atomistic pdb to DNA nucleotide pdb (i.e. one CG bead per nucleotide). 
     The position of each CG nucleotide bead is the geometric center of all the nucleotide atoms in the pdb.
     
     Parameters
     ----------
     atomistic_pdb : str
         Path for the atomistic pdb file. 
 
     cg_nucleotide_pdb : str
         Output path for the CG pdb file. 
     
     write_TER : bool
         Whether to write TER between two chains. 
     
-    '''
+    """
     atomistic_pdb_atoms = parse_pdb(atomistic_pdb)
     atomistic_pdb_atoms = atomistic_pdb_atoms.loc[atomistic_pdb_atoms['resname'].isin(_nucleotides)].copy()
     atomistic_pdb_atoms.index = list(range(len(atomistic_pdb_atoms.index)))
     chainID = atomistic_pdb_atoms['chainID']
     resSeq = atomistic_pdb_atoms['resSeq']
     atomistic_pdb_atoms.index = chainID.astype(str) + '_' + resSeq.astype(str)
     cg_nucleotide_pdb_atoms = pd.DataFrame(columns=atomistic_pdb_atoms.columns)
@@ -159,15 +159,15 @@
         row[['name', 'occupancy', 'tempFactor', 'element', 'charge']] = ['NU', 1.0, 1.0, '', '']
         cg_nucleotide_pdb_atoms.loc[len(cg_nucleotide_pdb_atoms.index)] = row
     cg_nucleotide_pdb_atoms['serial'] = list(range(1, len(cg_nucleotide_pdb_atoms.index) + 1))
     write_pdb(cg_nucleotide_pdb_atoms, cg_nucleotide_pdb, write_TER)
 
 
 def build_straight_CA_chain(sequence, r0=0.38):
-    '''
+    """
     Build a straight portein CA atom chain with given sequence. 
     
     Parameters
     ----------
     sequence : str
         Protein chain sequence (1 letter for each amino acid). 
     
@@ -175,15 +175,15 @@
         Distance in unit nm between two neighboring CA atoms. 
     
     Returns
     -------
     df_atoms : pd.DataFrame
         A pandas dataframe includes atom information. 
     
-    '''
+    """
     n_atoms = len(sequence)
     data = []
     for i in range(n_atoms):
         resname = _amino_acid_1_letter_to_3_letters_dict[sequence[i]]
         atom_i_dict = {'recname': 'ATOM', 'name': 'CA', 'altLoc': '', 'resname': resname, 'chainID': 'A', 'iCode': '', 
                        'occupancy': 1.0, 'tempFactor': 1.0, 'element': 'C', 'charge': ''}
         data.append(atom_i_dict)
@@ -196,15 +196,15 @@
     z -= np.mean(z)
     df_atoms['z'] = z*10 # convert nm to angstroms
     df_atoms['z'] = df_atoms['z'].round(3)
     return df_atoms
 
 
 def make_mol_whole(coord, box_a, box_b, box_c):
-    '''
+    """
     Use this function to make the molecule whole. 
     This is useful to recover the whole molecule if it is split by box boundary. 
     The position of the first atom is kept. 
     The other atoms are moved so that each one is in the closest periodic image relative to the previous one.
     
     Parameters
     ----------
@@ -221,15 +221,15 @@
         Box length along z-axis. 
     
     Returns
     -------
     new_coord : np.ndarray, shape = (n_atoms, 3)
         Output atom coordinates. 
     
-    '''
+    """
     n_atoms = coord.shape[0]
     new_coord = np.zeros((n_atoms, 3))
     for i in range(n_atoms):
         if i == 0:
             new_coord[i] = coord[i]
         else:
             r0 = new_coord[i - 1]
@@ -249,15 +249,15 @@
             while delta_z >= 0.5*box_c:
                 delta_z -= box_c
             new_coord[i] = r0 + np.array([delta_x, delta_y, delta_z])
     return new_coord
                 
 
 def move_atoms_to_closest_pbc_image(coord, ref_point, box_a, box_b, box_c):
-    '''
+    """
     Move the atom coordinates to the periodic image closest to ref_point. 
     
     Parameters
     ----------
     coord : np.ndarray, shape = (n_atoms, 3)
         Input atom coordinates. 
     
@@ -274,15 +274,15 @@
         Box length along z-axis. 
     
     Returns
     -------
     new_coord : np.ndarray, shape = (n_atoms, 3)
         Output atom coordinates. 
     
-    '''
+    """
     n_atoms = coord.shape[0]
     new_coord = np.zeros((n_atoms, 3))
     for i in range(n_atoms):
         delta_r = coord[i] - ref_point
         delta_x, delta_y, delta_z = delta_r[0], delta_r[1], delta_r[2]
         while delta_x < -0.5*box_a:
             delta_x += box_a
@@ -297,15 +297,15 @@
         while delta_z >= 0.5*box_c:
             delta_z -= box_c
         new_coord[i] = ref_point + np.array([delta_x, delta_y, delta_z])
     return new_coord
         
 
 def compute_rg(coord, mass):
-    '''
+    """
     Compute radius of gyration.
     
     Parameters
     ----------
     coord : np.ndarray, shape = (n_atoms, 3)
         Input atom coordinates. 
     
@@ -313,15 +313,15 @@
         Input atom mass. 
     
     Returns
     -------
     rg : float
         Radius of gyration. 
     
-    '''
+    """
     weights = mass/np.sum(mass)
     r_COM = np.average(coord, axis=0, weights=weights)
     rg_square = np.average(np.sum((coord - r_COM)**2, axis=1), weights=weights)
     rg = rg_square**0.5
     return rg
```

### Comparing `openabc-1.0.2/src/openabc/utils/legacy_shadow_map.py` & `openabc-1.0.3/src/openabc/utils/legacy_shadow_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 import os
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
 __author__ = 'Shuming Liu'
 
 
-'''
+"""
 A python implementation of shadow map algorithm. The related reference is: 
 
 Noel, Jeffrey K., Paul C. Whitford, and José N. Onuchic. "The shadow map: a general contact definition for capturing the dynamics of biomolecular folding and function." The journal of physical chemistry B 116.29 (2012): 8692-8702.
 
 This algorithm is applied to find contacts between residues (a residue can be an amino acid or a nucleotide)
 
 This script also includes some useful functions. 
 
 Legacy means a version to check with SMOG, as old version SMOG has some bugs. 
-'''
+"""
 
 _amino_acids = ['ALA', 'ARG', 'ASN', 'ASP', 'CYS',
                 'GLN', 'GLU', 'GLY', 'HIS', 'ILE',
                 'LEU', 'LYS', 'MET', 'PHE', 'PRO',
                 'SER', 'THR', 'TRP', 'TYR', 'VAL']
 
 
 def get_neighbor_pairs_and_distances(coord, cutoff=0.6, box=None, use_pbc=False):
-    '''
+    """
     Reference: https://docs.mdanalysis.org/1.1.1/documentation_pages/lib/nsgrid.html
     coord is the coordinate, and cutoff is the cutoff distance.
     coord and cutoff should use the same length unit.
     If use_pbc is False, then the box has to be orthogonal. 
     If use_pbc is True, then specify box as np.array([lx, ly, lz, alpha1, alpha2, alpha3]). 
-    '''
+    """
     if use_pbc:
         grid_search = MDAnalysis.lib.nsgrid.FastNS(cutoff, coord.astype(np.float32), box.astype(np.float32), use_pbc)
     else:
         x_min, x_max = np.amin(coord[:, 0]), np.amax(coord[:, 0])
         y_min, y_max = np.amin(coord[:, 1]), np.amax(coord[:, 1])
         z_min, z_max = np.amin(coord[:, 2]), np.amax(coord[:, 2])
         shifted_coord = coord.copy() - np.array([x_min, y_min, z_min])
@@ -54,33 +54,33 @@
     results = grid_search.self_search()
     neighbor_pairs = results.get_pairs()
     neighbor_pair_distances = results.get_pair_distances()
     return neighbor_pairs, neighbor_pair_distances
 
 
 def get_bonded_neighbor_dict(atomistic_pdb):
-    '''
+    """
     Find atoms that are directly connected by bonds.
-    '''
+    """
     traj = mdtraj.load_pdb(atomistic_pdb)
     top = traj.topology
     bond_graph = top.to_bondgraph()
     bonded_neighbor_dict = {}
     for a1 in list(bond_graph.nodes):
         bonded_neighbor_dict[a1.index] = []
         for a2 in bond_graph.neighbors(a1):
             bonded_neighbor_dict[a1.index].append(a2.index)
     return bonded_neighbor_dict
 
 
 def legacy_light_is_blocked(d12, d13, d23, r2, r3):
-    '''
+    """
     Check if the light from atom1 to atom2 is blocked by atom3.
     This is the legacy version, which means it has bug and only used to compare with old SMOG version results. 
-    '''
+    """
     assert d12 > 0
     assert d13 > 0
     assert d23 > 0
     assert r2 >= 0
     assert r3 >= 0
     assert r2 <= d12
     assert r3 <= d13
@@ -91,21 +91,21 @@
         return True
     else:
         return False
 
 
 def legacy_find_res_pairs_from_atomistic_pdb(atomistic_pdb, frame=0, radius=0.1, bonded_radius=0.05, cutoff=0.6, 
                                              box=None, use_pbc=False):
-    '''
+    """
     Find native pairs between residues following the shadow algorithm.
     They algorithm only searches native pairs between residues that do not have 1-2, 1-3, or 1-4 interactions. 
     If two heavy atoms from different residues are in contact, then the two residues are in contact.
     radius and bonded_radius are the shadow radii. 
     This is the legacy version, which means it has bug and only used to compare with old SMOG version results. 
-    '''
+    """
     traj = mdtraj.load_pdb(atomistic_pdb)
     top = traj.topology
     n_atoms = top.n_atoms
     df_atoms, _bonds = top.to_dataframe()
     # in df_atoms, each value in columns 'serial', 'resSeq', and 'chainID' is an integer
     df_atoms.index = list(range(len(df_atoms.index)))
     # set unique_resSeq, which starts from 0
@@ -185,19 +185,19 @@
             res_pairs.append([unique_resSeq1, unique_resSeq2])
     res_pairs = np.array(sorted(res_pairs))
     return res_pairs, df_atoms
 
 
 def legacy_find_ca_pairs_from_atomistic_pdb(atomistic_pdb, frame=0, radius=0.1, bonded_radius=0.05, cutoff=0.6, 
                                             box=None, use_pbc=False):
-    '''
+    """
     Find protein CA atom pairs whose residues are in contact.
     CA atom indices are residue indices, as here CA atom contacts represent residue contacts.
     This is the legacy version, which means it has bug and only used to compare with old SMOG version results.
-    '''
+    """
     res_pairs, df_atoms = legacy_find_res_pairs_from_atomistic_pdb(atomistic_pdb, frame, radius, bonded_radius, cutoff, 
                                                                    box, use_pbc)
     # pick out CA atoms for each residue
     dict_res_CA = {}
     for i, row in df_atoms.iterrows():
         if (row['resName'] in _amino_acids) and (row['name'] == 'CA'):
             unique_resSeq = df_atoms.loc[i, 'unique_resSeq']
@@ -212,18 +212,18 @@
     ca_atom_pairs = np.array(ca_atom_pairs)
     traj = mdtraj.load_pdb(atomistic_pdb)
     df_ca_pairs['mu'] = mdtraj.compute_distances(traj, ca_atom_pairs, use_pbc)[frame]
     return df_ca_pairs
 
 
 def load_ca_pairs_from_gmx_top(top_file, ca_pdb, frame=0, use_pbc=False):
-    '''
+    """
     Load native pairs from GROMACS topology file. 
     Note in GROMACS, atom indices start from 1, while in OpenMM, atom indices start from 0.
-    '''
+    """
     with open(top_file, 'r') as input_reader:
         top_file_lines = input_reader.readlines()
     flag = False
     for i in range(len(top_file_lines)):
         if '[ pairs ]' in top_file_lines[i]:
             start_index = i + 2
             flag = True
```

### Comparing `openabc-1.0.2/src/openabc/utils/replica_exchange.py` & `openabc-1.0.3/src/openabc/utils/replica_exchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import simtk.unit as unit
 import sys
 import os
 import torch
 import math
 import time
 
-'''
+"""
 The code is adapted from Xinqiang Ding's script. 
-'''
+"""
 
 # set gas constant R
 GAS_CONSTANT_R = (1.0*unit.BOLTZMANN_CONSTANT_kB*unit.AVOGADRO_CONSTANT_NA).value_in_unit(unit.kilojoule_per_mole/unit.kelvin)
 
 class TemperatureReplicaExchange(object):
-    '''
+    """
     Temperature replica exchange class for performing temperature replica exchange (TRE) simulations. 
     
     Note only positions and scaled velocities are exchanged, while other internal states of the simulations are not exchanged. This means the class may not be properly applied to simulations involving other internal states. For example, Nose-Hoover integrator may not work properly as it includes internal chain states. 
     
     The parallelization is achieved with `torch.distributed`. 
     
     An example of setting environment variables in a slurm job script:
@@ -30,18 +30,19 @@
     
         export MASTER_PORT=$(expr 30000 + $(echo -n ${SLURM_JOBID} | tail -c 4))
     
         master_addr=$(scontrol show hostnames "${SLURM_JOB_NODELIST}" | head -n 1)
     
         export MASTER_ADDR=${master_addr}
     
-    '''
+    """
+    
     def __init__(self, backend, n_replicas, rank, positions, top, system, temperatures, integrator, 
                  platform_name='CUDA', properties={'Precision': 'mixed'}):
-        '''
+        """
         Initialize temperature replica exchange object. 
         
         Parameters
         ----------
         backend : str
             Backend for torch
         
@@ -69,15 +70,15 @@
         properties : dict or None
             The OpenMM simulation platform properties. 
         
         References
         ----------
         https://pytorch.org/docs/stable/distributed.html
 
-        '''
+        """
         self.backend = backend
         self.n_replicas = n_replicas
         assert self.n_replicas == int(os.environ['WORLD_SIZE'])
         self.rank = rank
         torch.distributed.init_process_group(backend, world_size=self.n_replicas, rank=self.rank)
         self.top = top
         self.system = system
@@ -91,15 +92,15 @@
         else:
             self.simulation = app.Simulation(self.top, self.system, self.integrator, platform)
         self.simulation.context.setPositions(positions)
         self.simulation.minimizeEnergy()
         self.simulation.context.setVelocitiesToTemperature(self.temperatures[self.rank])
     
     def add_reporters(self, report_interval, report_state=True, report_dcd=True, output_dcd=None, use_pbc=True):
-        '''
+        """
         Add reporters for OpenMM simulation.
         
         Parameters
         ----------
         report_interval : int
             Report interval.
         
@@ -112,28 +113,28 @@
         output_dcd : str or None
             The output dcd file path. If None, then the output dcd file path is set as output.{self.rank}.dcd. 
         
         use_pbc : bool or None
             Whether to use periodic boundary condition (PBC) to translate atoms so the center of each molecule lies in the same PBC box.
             If None, then determine according to if the simulation system uses PBC. 
         
-        '''
+        """
         if report_state:
             state_reporter = app.StateDataReporter(sys.stdout, report_interval, step=True, time=True, 
                                                    potentialEnergy=True, kineticEnergy=True, totalEnergy=True, 
                                                    temperature=True, speed=True)
             self.simulation.reporters.append(state_reporter)
         if report_dcd:
             if output_dcd is None:
                 output_dcd = f'output.{self.rank}.dcd'
             dcd_reporter = app.DCDReporter(output_dcd, report_interval, enforcePeriodicBox=use_pbc)
             self.simulation.reporters.append(dcd_reporter)
     
     def run_replica_exchange(self, n_steps, exchange_interval, verbose=True):
-        '''
+        """
         Perform replica exchange simulation. 
         
         Exchange atom positions and rescaled velocities. Other state variables are not exchanged. 
         
         The temperature of each replica remains unchanged. 
         
         Parameters
@@ -143,15 +144,15 @@
         
         exchange_interval : int
             Exchange interval. 
         
         verbose : bool
             Whether to report exchange acceptance ratio and simulation speed. 
          
-        '''
+        """
         n_iterations = int(n_steps/exchange_interval)
         n_steps = n_iterations*exchange_interval # reset n_steps in case n_steps % exchange_interval != 0
         n_exchange_attempts = 0
         n_accepted_exchange_attempts = 0
         start_time = time.time()
         for i in range(n_iterations):
             self.simulation.step(exchange_interval)
```

### Comparing `openabc-1.0.2/src/openabc/utils/shadow_map.py` & `openabc-1.0.3/src/openabc/utils/shadow_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas as pd
 import mdtraj
-import MDAnalysis as mda
+from MDAnalysis.lib.nsgrid import FastNS
 import networkx as nx
 import math
 import sys
 import os
 
 __location__ = os.path.dirname(os.path.abspath(__file__))
 
@@ -61,26 +61,26 @@
     
     References
     ----------
     https://docs.mdanalysis.org/1.1.1/documentation_pages/lib/nsgrid.html
     
     '''
     if use_pbc:
-        grid_search = mda.lib.nsgrid.FastNS(cutoff, coord.astype(np.float32), box.astype(np.float32), use_pbc)
+        grid_search = FastNS(cutoff, coord.astype(np.float32), box.astype(np.float32), use_pbc)
     else:
         x_min, x_max = np.amin(coord[:, 0]), np.amax(coord[:, 0])
         y_min, y_max = np.amin(coord[:, 1]), np.amax(coord[:, 1])
         z_min, z_max = np.amin(coord[:, 2]), np.amax(coord[:, 2])
         shifted_coord = coord.copy() - np.array([x_min, y_min, z_min])
         shifted_coord = shifted_coord.astype(np.float32)
         lx = max(1.1*(x_max - x_min), 2.1*cutoff)
         ly = max(1.1*(y_max - y_min), 2.1*cutoff)
         lz = max(1.1*(z_max - z_min), 2.1*cutoff)
         pseudo_box = np.array([lx, ly, lz, 90, 90, 90]).astype(np.float32) # build an orthogonal pseudo box
-        grid_search = mda.lib.nsgrid.FastNS(cutoff, shifted_coord, pseudo_box, use_pbc)
+        grid_search = FastNS(cutoff, shifted_coord, pseudo_box, use_pbc)
     results = grid_search.self_search()
     neighbor_pairs = results.get_pairs()
     neighbor_pair_distances = results.get_pair_distances()
     return neighbor_pairs, neighbor_pair_distances
 
 
 def get_bonded_neighbor_dict(atomistic_pdb):
```

### Comparing `openabc-1.0.2/src/openabc.egg-info/PKG-INFO` & `openabc-1.0.3/src/openabc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openabc
-Version: 1.0.2
+Version: 1.0.3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openabc-1.0.2/src/openabc.egg-info/SOURCES.txt` & `openabc-1.0.3/src/openabc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

