# Comparing `tmp/navarp-1.4.0.tar.gz` & `tmp/navarp-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\navarp-1.4.0.tar", last modified: Mon Jun 20 22:04:01 2022, max compression
+gzip compressed data, was "dist\navarp-1.5.0.tar", last modified: Sat Apr 22 10:49:22 2023, max compression
```

## Comparing `navarp-1.4.0.tar` & `navarp-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/
--rw-rw-rw-   0        0        0      177 2021-06-08 16:38:35.000000 navarp-1.4.0/AUTHORS.rst
--rw-rw-rw-   0        0        0    33864 2021-05-06 13:58:56.000000 navarp-1.4.0/LICENSE
--rw-rw-rw-   0        0        0       60 2021-05-07 12:10:35.000000 navarp-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1426 2022-06-20 22:04:01.000000 navarp-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2022-06-20 21:07:38.000000 navarp-1.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/navarp/
--rw-rw-rw-   0        0        0      164 2022-06-20 21:07:38.000000 navarp-1.4.0/navarp/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/navarp/extras/
--rw-rw-rw-   0        0        0        0 2021-06-08 17:07:08.000000 navarp-1.4.0/navarp/extras/__init__.py
--rw-rw-rw-   0        0        0     7527 2021-07-05 16:53:28.000000 navarp-1.4.0/navarp/extras/simulation.py
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/navarp/gui/
--rw-rw-rw-   0        0        0     5182 2021-07-02 15:12:51.000000 navarp-1.4.0/navarp/gui/about.ui
--rw-rw-rw-   0        0        0     4215 2021-07-02 15:12:51.000000 navarp-1.4.0/navarp/gui/export.ui
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/navarp/gui/icons/
--rw-rw-rw-   0        0        0     6740 2021-05-06 13:58:56.000000 navarp-1.4.0/navarp/gui/icons/navarp.svg
--rw-rw-rw-   0        0        0    91844 2021-11-23 17:08:49.000000 navarp-1.4.0/navarp/gui/main.ui
--rw-rw-rw-   0        0        0    78419 2022-06-20 21:07:38.000000 navarp-1.4.0/navarp/navarp_gui.py
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/navarp/utils/
--rw-rw-rw-   0        0        0        0 2021-05-06 13:58:56.000000 navarp-1.4.0/navarp/utils/__init__.py
--rw-rw-rw-   0        0        0     7347 2021-06-08 16:38:35.000000 navarp-1.4.0/navarp/utils/fermilevel.py
--rw-rw-rw-   0        0        0     4615 2022-06-20 21:07:38.000000 navarp-1.4.0/navarp/utils/isocut.py
--rw-rw-rw-   0        0        0    53757 2021-12-15 13:38:10.000000 navarp-1.4.0/navarp/utils/isomclass.py
--rw-rw-rw-   0        0        0    22274 2021-11-25 09:57:33.000000 navarp-1.4.0/navarp/utils/kinterp.py
--rw-rw-rw-   0        0        0    24339 2021-06-08 16:38:35.000000 navarp-1.4.0/navarp/utils/ktransf.py
--rw-rw-rw-   0        0        0    85818 2022-06-20 21:39:46.000000 navarp-1.4.0/navarp/utils/navfile.py
--rw-rw-rw-   0        0        0    18855 2021-07-02 15:12:51.000000 navarp-1.4.0/navarp/utils/navplt.py
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/navarp.egg-info/
--rw-rw-rw-   0        0        0     1426 2022-06-20 22:04:00.000000 navarp-1.4.0/navarp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      635 2022-06-20 22:04:00.000000 navarp-1.4.0/navarp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-20 22:04:00.000000 navarp-1.4.0/navarp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-06-20 22:04:00.000000 navarp-1.4.0/navarp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2022-06-20 22:04:00.000000 navarp-1.4.0/navarp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-06-20 22:04:00.000000 navarp-1.4.0/navarp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-20 22:04:01.000000 navarp-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2216 2022-06-20 21:07:38.000000 navarp-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-20 22:04:01.000000 navarp-1.4.0/test/
--rw-rw-rw-   0        0        0      417 2019-07-12 08:39:36.000000 navarp-1.4.0/test/test_screen_res.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/
+-rw-rw-rw-   0        0        0      177 2021-06-08 16:38:35.000000 navarp-1.5.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0    33864 2021-05-06 13:58:56.000000 navarp-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2021-05-07 12:10:35.000000 navarp-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1426 2023-04-22 10:49:22.000000 navarp-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-04-22 10:43:10.000000 navarp-1.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp/
+-rw-rw-rw-   0        0        0      164 2023-04-22 10:43:10.000000 navarp-1.5.0/navarp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp/extras/
+-rw-rw-rw-   0        0        0        0 2021-06-08 17:07:08.000000 navarp-1.5.0/navarp/extras/__init__.py
+-rw-rw-rw-   0        0        0     7527 2021-07-05 16:53:28.000000 navarp-1.5.0/navarp/extras/simulation.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp/gui/
+-rw-rw-rw-   0        0        0     5182 2021-07-02 15:12:51.000000 navarp-1.5.0/navarp/gui/about.ui
+-rw-rw-rw-   0        0        0     4215 2021-07-02 15:12:51.000000 navarp-1.5.0/navarp/gui/export.ui
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp/gui/icons/
+-rw-rw-rw-   0        0        0     6740 2021-05-06 13:58:56.000000 navarp-1.5.0/navarp/gui/icons/navarp.svg
+-rw-rw-rw-   0        0        0    91844 2021-11-23 17:08:49.000000 navarp-1.5.0/navarp/gui/main.ui
+-rw-rw-rw-   0        0        0    78424 2023-04-22 10:43:10.000000 navarp-1.5.0/navarp/navarp_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp/utils/
+-rw-rw-rw-   0        0        0        0 2021-05-06 13:58:56.000000 navarp-1.5.0/navarp/utils/__init__.py
+-rw-rw-rw-   0        0        0     7347 2021-06-08 16:38:35.000000 navarp-1.5.0/navarp/utils/fermilevel.py
+-rw-rw-rw-   0        0        0     4615 2022-06-20 21:07:38.000000 navarp-1.5.0/navarp/utils/isocut.py
+-rw-rw-rw-   0        0        0    53757 2021-12-15 13:38:10.000000 navarp-1.5.0/navarp/utils/isomclass.py
+-rw-rw-rw-   0        0        0    22274 2021-11-25 09:57:33.000000 navarp-1.5.0/navarp/utils/kinterp.py
+-rw-rw-rw-   0        0        0    24339 2021-06-08 16:38:35.000000 navarp-1.5.0/navarp/utils/ktransf.py
+-rw-rw-rw-   0        0        0    87848 2023-04-22 10:43:10.000000 navarp-1.5.0/navarp/utils/navfile.py
+-rw-rw-rw-   0        0        0    18855 2021-07-02 15:12:51.000000 navarp-1.5.0/navarp/utils/navplt.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp.egg-info/
+-rw-rw-rw-   0        0        0     1426 2023-04-22 10:49:20.000000 navarp-1.5.0/navarp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      635 2023-04-22 10:49:22.000000 navarp-1.5.0/navarp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 10:49:20.000000 navarp-1.5.0/navarp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-22 10:49:21.000000 navarp-1.5.0/navarp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2023-04-22 10:49:21.000000 navarp-1.5.0/navarp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-22 10:49:21.000000 navarp-1.5.0/navarp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 10:49:22.000000 navarp-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2216 2023-04-22 10:43:10.000000 navarp-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 10:49:22.000000 navarp-1.5.0/test/
+-rw-rw-rw-   0        0        0      417 2019-07-12 08:39:36.000000 navarp-1.5.0/test/test_screen_res.py
```

### Comparing `navarp-1.4.0/LICENSE` & `navarp-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/PKG-INFO` & `navarp-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navarp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Navigation tool for ARPES data.
 Home-page: https://gitlab.com/fbisti/navarp
 Author: Federico Bisti
 Author-email: federico.bisti@univaq.it
 License: GPLv3+
 Keywords: navarp
 Platform: UNKNOWN
```

### Comparing `navarp-1.4.0/README.rst` & `navarp-1.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 **Documentation site**: `https://fbisti.gitlab.io/navarp <https://fbisti.gitlab.io/navarp>`_
 
 **Author**: Federico Bisti (federico.bisti@univaq.it), for complete list see `AUTHORS.rst <AUTHORS.rst>`_
 
 **License**: GPL
 
-**Version Number**: 1.4.0
+**Version Number**: 1.5.0
 
 .. image:: images/intro.gif
    :width: 90%
 
 Installation
 ============
```

### Comparing `navarp-1.4.0/navarp/extras/simulation.py` & `navarp-1.5.0/navarp/extras/simulation.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/gui/about.ui` & `navarp-1.5.0/navarp/gui/about.ui`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/gui/export.ui` & `navarp-1.5.0/navarp/gui/export.ui`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/gui/icons/navarp.svg` & `navarp-1.5.0/navarp/gui/icons/navarp.svg`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/gui/main.ui` & `navarp-1.5.0/navarp/gui/main.ui`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/navarp_gui.py` & `navarp-1.5.0/navarp/navarp_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 
             # ###############################
             # set ExportDialog
             self.exportDialog.le_exptfiledir.setText(
                 os.path.dirname(file_path))
 
             self.exportDialog.kxbinsSpinBox.setValue(
-                len(self.entry.angles)*1.5)
+                int(len(self.entry.angles)*1.5))
             self.exportDialog.ksbinsSpinBox.setValue(
                 len(self.entry.scans)*5)
 
             # ###############################
             # make the plot
             self.select_mode()
```

### Comparing `navarp-1.4.0/navarp/utils/fermilevel.py` & `navarp-1.5.0/navarp/utils/fermilevel.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/utils/isocut.py` & `navarp-1.5.0/navarp/utils/isocut.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/utils/isomclass.py` & `navarp-1.5.0/navarp/utils/isomclass.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/utils/kinterp.py` & `navarp-1.5.0/navarp/utils/kinterp.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/utils/ktransf.py` & `navarp-1.5.0/navarp/utils/ktransf.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp/utils/navfile.py` & `navarp-1.5.0/navarp/utils/navfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1178,27 +1178,48 @@
     analyzer = NavAnalyzer()
     analyzer._set_def_antares_soleil()
 
     fst_grp = list(h5f.keys())[0]
 
     # deflector angles
     defl_angles = h5f[fst_grp+"/scan_data/actuator_1_1"][()]
+    # check if deflector angles contains NaNs and in the case replace them
+    if np.isnan(defl_angles).any():
+        mask = np.isnan(defl_angles)
+        last_valid = defl_angles[np.invert(mask)][-1]
+        delta = np.round(last_valid - defl_angles[np.invert(mask)][-2], 6)
+        defl_angles[mask] = (
+            last_valid + (1 + np.arange(len(defl_angles[mask]))*delta))
 
     # scans and scan_type
     scans = defl_angles
     scan_type = "deflector"
 
-    hv = h5f[fst_grp+"/ANTARES/Monochromator/energy/data"][()]
-    en_res = h5f[fst_grp+"/ANTARES/Monochromator/resolution/data"][()]
+    # hv and energy resolution from monochromator
+    for key in h5f[fst_grp+"/ANTARES"]:
+        if key == r"Monochromator":
+            hv = h5f[fst_grp+"/ANTARES/Monochromator/energy/data"][()]
+            en_res = h5f[fst_grp+"/ANTARES/Monochromator/resolution/data"][()]
+            break
+        elif key == r"i12-m-c04-op-mono1":
+            hv = h5f[fst_grp+"/ANTARES/i12-m-c04-op-mono1/energy"][()]
+            en_res = h5f[fst_grp+"/ANTARES/i12-m-c04-op-mono1/resolution"][()]
+            break
+        # WARNING: can't find photon energy (hv), using default of 123
+        hv = np.array([123])
+        en_res = 0
 
     mbs_grp = [key for key in h5f[fst_grp+"/ANTARES"] if "MBSAcq" in key][0]
-    mode = h5f[fst_grp+"/ANTARES/"+mbs_grp+"/LensMode/data"][()]
-    epass = h5f[fst_grp+"/ANTARES/"+mbs_grp+"/PASSENERGY/data"][()]
-    mode = decode_h5py(mode)
-    epass = decode_h5py(epass)
+    mbs_grp = fst_grp + "/ANTARES/" + mbs_grp
+    params = {}
+    for key in h5f[mbs_grp]:
+        if isinstance(h5f[mbs_grp][key], h5py.Dataset):
+            params[key] = h5f[mbs_grp][key][()]
+        else:
+            params[key] = h5f[mbs_grp][key][r"data"][()]
 
     angle_min = h5f[fst_grp+"/scan_data/data_04"][()][0]
     angle_mult = h5f[fst_grp+"/scan_data/data_05"][()][0]
     angle_max = h5f[fst_grp+"/scan_data/data_06"][()][0]
     # angle array includes the angle_max so
     angles = np.arange(angle_min, angle_max+angle_mult*0.5, angle_mult)
 
@@ -1231,19 +1252,18 @@
     else:
         hv_note = '{:6.2f}'.format(min(hv))
 
     file_note = (
         "scan_type = {}\n".format(scan_type) +
         "sample = {}\n".format(fst_grp) +
         "hv = {}\n".format(hv_note) +
-        "en_res = {}\n".format(en_res[0]) +
-        "epass = {}\n".format(epass) +
-        "lens_mode = {}\n".format(mode) +
-        " deflector = scan along tilt"
+        "en_res = {}\n".format(en_res[0])
     )
+    for key in params:
+        file_note += "{} = {}\n".format(key, params[key])
 
     # closing h5f-file
     h5f.close()
 
     return NavEntry(scans, angles, energies, data, scan_type, hv, defl_angles,
                     analyzer, file_note, file_path)
 
@@ -1511,15 +1531,19 @@
     """
     # Select the correct loading function depending on the first line
     with open(file_path) as fdat:
         line = fdat.readline()
 
     if 'IGOR' in line:  # Igor itx format
         return load_igorpro_itx(file_path)
-    elif ('[Info]' in line) or ('Frames Per Step' in line):  # Scienta or MBS
+    elif (
+        ('[Info]' in line) or
+        ('Frames Per Step' in line) or
+        ('Lines' in line)
+    ):  # Scienta or MBS
         return load_scienta_or_mbs_txt(file_path)
     else:  # it is unknow
         return None
 
 
 def load_scienta_or_mbs_txt(file_path):
     """Load txt-file from MBS A1Soft or Scienta-Omicro SES program.
@@ -1534,15 +1558,18 @@
     params = {}
     with open(file_path) as fdat:
         line = fdat.readline()
         if '[Info]' in line:  # it is from Scienta-Omicro SES
             dataform = 'scienta'
             separator = '='
             breaking = '[Data 1'
-        elif 'Frames Per Step' in line:  # it is from MBS A1Soft
+        elif (
+            ('Frames Per Step' in line) or
+            ('Lines' in line)
+        ):  # it is from MBS A1Soft
             dataform = 'mbs'
             separator = '\t'
             breaking = 'DATA:'
         else:  # it is unknow
             return None
 
         for line in fdat:
@@ -1600,19 +1627,26 @@
                 for line in fdat:
                     data[0, :, ind0] = np.fromstring(line, sep=' ')[1:]
                     ind0 += 1
                     if ind0 == data.shape[2]:
                         break
 
         elif dataform == 'mbs':
-            angles = np.linspace(
-                float(params['XScaleMin']),
-                float(params['XScaleMax']),
-                int(params['NoS'])
-            )
+            if 'XScaleMin' in params:
+                angles = np.linspace(
+                    float(params['XScaleMin']),
+                    float(params['XScaleMax']),
+                    int(params['NoS'])
+                )
+            elif 'ScaleMin' in params:
+                angles = np.linspace(
+                    float(params['ScaleMin']),
+                    float(params['ScaleMax']),
+                    int(params['NoS'])
+                )
             energies = np.linspace(
                 float(params['Start K.E.']),
                 float(params['End K.E.']),
                 int(params['No. Steps'])
             )
             # WARNING: can't find photon energy (hv), using default value 123
             hv = np.array([123])
@@ -2247,14 +2281,32 @@
         # without checking the consistency, use as energies only the first one
         # since the kinetic energies cannot be different without a hv scan
         if len(entry_out.energies.shape) == 2:
             entry_out.energies = entry_out.energies[0, :]
         if entry_out.scan_type == 'deflector':
             entry_out.defl_angles = entry_out.scans
 
+    # checking if energies scale is in binding energy and
+    # transforming to kinetic energies in the case
+    if 'energy_scale' in entry_info:
+        if 'bin' in entry_info['energy_scale'].lower():
+            if entry_out.scan_type == 'hv':
+                energies = (
+                    entry_out.hv[:, np.newaxis]
+                    - entry_out.analyzer.work_fun
+                    + entry_out.energies[np.newaxis, :]
+                )
+            else:
+                energies = (
+                    entry_out.hv
+                    - entry_out.analyzer.work_fun
+                    + entry_out.energies
+                )
+            entry_out.energies = energies
+
     entry_out.file_note = re.sub(
         "scan_type = [A-Za-z_]+",
         "scan_type = {}".format(entry_out.scan_type),
         entry_out.file_note
     )
 
     entry_out.efermi = entry_out.hv - entry_out.analyzer.work_fun
```

### Comparing `navarp-1.4.0/navarp/utils/navplt.py` & `navarp-1.5.0/navarp/utils/navplt.py`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/navarp.egg-info/PKG-INFO` & `navarp-1.5.0/navarp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navarp
-Version: 1.4.0
+Version: 1.5.0
 Summary: Navigation tool for ARPES data.
 Home-page: https://gitlab.com/fbisti/navarp
 Author: Federico Bisti
 Author-email: federico.bisti@univaq.it
 License: GPLv3+
 Keywords: navarp
 Platform: UNKNOWN
```

### Comparing `navarp-1.4.0/navarp.egg-info/SOURCES.txt` & `navarp-1.5.0/navarp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `navarp-1.4.0/setup.py` & `navarp-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,14 @@
     license="GPLv3+",
     long_description=long_description,
     include_package_data=True,
     keywords='navarp',
     name='navarp',
     packages=find_packages(include=['navarp', 'navarp.*']),
     url='https://gitlab.com/fbisti/navarp',
-    version='1.4.0',
+    version='1.5.0',
     py_modules=['navarp'],
     entry_points='''
         [console_scripts]
         navarp=navarp.navarp_gui:main
     ''',
 )
```

