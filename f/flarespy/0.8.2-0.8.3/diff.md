# Comparing `tmp/flarespy-0.8.2.tar.gz` & `tmp/flarespy-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.8.2.tar", max compression
+gzip compressed data, was "flarespy-0.8.3.tar", max compression
```

## Comparing `flarespy-0.8.2.tar` & `flarespy-0.8.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.2/LICENSE
--rw-r--r--   0        0        0      428 2023-04-21 10:51:56.703834 flarespy-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.2/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.2/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.2/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25163 2023-04-21 10:51:56.702730 flarespy-0.8.2/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     6907 2023-04-21 10:25:18.842486 flarespy-0.8.2/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-21 10:51:56.700027 flarespy-0.8.2/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.3/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-22 01:33:10.846417 flarespy-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.3/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.3/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.3/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    25175 2023-04-22 01:27:55.396445 flarespy-0.8.3/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     6922 2023-04-22 01:27:55.389977 flarespy-0.8.3/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-22 01:33:10.844221 flarespy-0.8.3/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.3/PKG-INFO
```

### Comparing `flarespy-0.8.2/LICENSE` & `flarespy-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.2/src/flarespy/Flare_model.py` & `flarespy-0.8.3/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.2/src/flarespy/data/model.dat` & `flarespy-0.8.3/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.2/src/flarespy/flarefinder.py` & `flarespy-0.8.3/src/flarespy/flarefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         gaia_dr3_id = query_gaia_dr3_id(self.ticid)
         self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_id
         self.stellar_parameters.obs_duration = np.round(
             self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
         )
 
         # Query parallax, Gmag and BP-RP from Gaia DR3
-        if ~np.isnan(gaia_dr3_id):
+        if isinstance(gaia_dr3_id, str):
             result = VIZIER.query_constraints("I/355/gaiadr3", Source=gaia_dr3_id)[0]
             plx = result["Plx"].data.data[0]
             if plx > 0:
                 self.stellar_parameters["Plx"] = np.round(plx, 4)
             self.stellar_parameters["Gmag"] = np.round(result["Gmag"].data.data[0], 4)
             self.stellar_parameters["BP-RP"] = np.round(result["BP-RP"].data.data[0], 4)
 
@@ -306,15 +306,15 @@
         query_result = None
         with warnings.catch_warnings():
             warnings.simplefilter("error", category=UserWarning)
             try:
                 query_result = CUSTOM_SIMBAD.query_object(self.label)
             except TableParseError:
                 gaia_dr3_id = self.stellar_parameters.gaia_dr3_source_id
-                if ~np.isnan(gaia_dr3_id):
+                if isinstance(gaia_dr3_id, str):
                     try:
                         query_result = CUSTOM_SIMBAD.query_object(f"Gaia DR3 {gaia_dr3_id}")
                     except TableParseError:
                         pass
 
         self.meta["exclude"] = False
         if query_result is None:
```

### Comparing `flarespy-0.8.2/src/flarespy/utils.py` & `flarespy-0.8.3/src/flarespy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,24 +179,24 @@
     if gaia2_source_id != "":
         query = """
                 SELECT dr2_source_id, dr3_source_id
                 FROM gaiadr3.dr2_neighbourhood
                 WHERE dr2_source_id = {gaia2_source_id}
                 """
         cross_result = Gaia.launch_job(query.format(gaia2_source_id=gaia2_source_id)).get_results()
-        return cross_result["dr3_source_id"][0]
+        return str(cross_result["dr3_source_id"][0])
     else:
         with warnings.catch_warnings():
             warnings.simplefilter("error", category=UserWarning)
             try:
                 simbad_result = CUSTOM_SIMBAD.query_object(f"TIC{tic_id}")
                 id_list = simbad_result["IDS"][0].split("|")
                 for i in id_list:
                     if "Gaia DR3" in i:
-                        return i.split(" ")[-1]
+                        return str(i.split(" ")[-1])
             except TableParseError:
                 pass
 
         ra = mast_result["ra"].data.data[0] * u.deg
         dec = mast_result["dec"].data.data[0] * u.deg
         pm_ra = mast_result["pmRA"].data.data[0] * u.mas / u.yr
         pm_dec = mast_result["pmDEC"].data.data[0] * u.mas / u.yr
@@ -206,10 +206,10 @@
                 warnings.filterwarnings("ignore", category=ErfaWarning)
                 coords = coords_j2000.apply_space_motion(new_obstime=Time("J2016"))
         else:
             coords = SkyCoord(ra, dec, frame="icrs")
         radius = u.Quantity(1, u.arcmin)
         gaia_result = Gaia.cone_search_async(coords, radius, columns=["source_id"]).get_results()
         if (gaia_result["dist"] < (3 / 3600)).any():
-            return gaia_result["source_id"].data.data[0]
+            return str(gaia_result["source_id"].data.data[0])
 
     return np.nan
```

### Comparing `flarespy-0.8.2/PKG-INFO` & `flarespy-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

