# Comparing `tmp/cfr-0.4.5.tar.gz` & `tmp/cfr-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.4.5.tar", last modified: Fri Apr 14 08:23:26 2023, max compression
+gzip compressed data, was "cfr-0.4.6.tar", last modified: Sat Apr 22 18:56:26 2023, max compression
```

## Comparing `cfr-0.4.5.tar` & `cfr-0.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.180477 cfr-0.4.5/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.4.5/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1693 2023-04-14 08:23:26.180080 cfr-0.4.5/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1129 2023-03-03 14:30:05.000000 cfr-0.4.5/README.rst
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:25.856174 cfr-0.4.5/bin/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.4.5/bin/cfr
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.073004 cfr-0.4.5/cfr/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.4.5/cfr/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18148 2023-04-14 08:22:21.000000 cfr-0.4.5/cfr/climate.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.179292 cfr-0.4.5/cfr/da/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.4.5/cfr/da/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.4.5/cfr/da/enkf.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18762 2023-04-12 21:07:20.000000 cfr-0.4.5/cfr/gcm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.4.5/cfr/ml.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60727 2023-04-14 08:22:33.000000 cfr-0.4.5/cfr/proxy.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44966 2023-04-06 02:13:26.000000 cfr-0.4.5/cfr/psm.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49933 2023-04-09 06:47:02.000000 cfr-0.4.5/cfr/reconjob.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.4.5/cfr/reconres.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17830 2023-04-06 07:20:24.000000 cfr-0.4.5/cfr/ts.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    20677 2023-03-27 06:51:18.000000 cfr-0.4.5/cfr/utils.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.4.5/cfr/visual.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-14 08:23:26.178239 cfr-0.4.5/cfr.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1693 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      374 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.4.5/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-04-14 08:23:25.000000 cfr-0.4.5/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-04-14 08:23:26.180574 cfr-0.4.5/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1415 2023-04-14 08:21:20.000000 cfr-0.4.5/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.570985 cfr-0.4.6/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1516 2023-03-03 14:30:05.000000 cfr-0.4.6/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1676 2023-04-22 18:56:26.570465 cfr-0.4.6/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1112 2023-04-18 00:48:45.000000 cfr-0.4.6/README.rst
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.554034 cfr-0.4.6/bin/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3905 2023-03-03 14:30:05.000000 cfr-0.4.6/bin/cfr
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.563558 cfr-0.4.6/cfr/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      640 2023-03-24 19:14:09.000000 cfr-0.4.6/cfr/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    18148 2023-04-14 08:22:21.000000 cfr-0.4.6/cfr/climate.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.569798 cfr-0.4.6/cfr/da/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       22 2023-03-03 14:30:05.000000 cfr-0.4.6/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    16319 2023-03-26 05:47:23.000000 cfr-0.4.6/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22484 2023-04-17 17:43:24.000000 cfr-0.4.6/cfr/gcm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7623 2023-03-03 14:30:05.000000 cfr-0.4.6/cfr/ml.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    61428 2023-04-22 04:02:32.000000 cfr-0.4.6/cfr/proxy.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    44996 2023-04-22 03:20:57.000000 cfr-0.4.6/cfr/psm.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    49933 2023-04-09 06:47:02.000000 cfr-0.4.6/cfr/reconjob.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2311 2023-03-26 06:27:24.000000 cfr-0.4.6/cfr/reconres.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    17830 2023-04-06 07:20:24.000000 cfr-0.4.6/cfr/ts.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    20957 2023-04-22 04:02:16.000000 cfr-0.4.6/cfr/utils.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    54810 2023-04-06 07:30:44.000000 cfr-0.4.6/cfr/visual.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-04-22 18:56:26.568539 cfr-0.4.6/cfr.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1676 2023-04-22 18:56:26.565061 cfr-0.4.6/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      374 2023-04-22 18:56:26.565563 cfr-0.4.6/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-04-22 18:56:26.566306 cfr-0.4.6/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-03-03 14:35:18.000000 cfr-0.4.6/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      203 2023-04-22 18:56:26.567925 cfr-0.4.6/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-04-22 18:56:26.568630 cfr-0.4.6/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-04-22 18:56:26.571084 cfr-0.4.6/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1415 2023-04-22 07:25:43.000000 cfr-0.4.6/setup.py
```

### Comparing `cfr-0.4.5/LICENSE` & `cfr-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/PKG-INFO` & `cfr-0.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.4.5
+Version: 0.4.6
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
@@ -19,16 +19,15 @@
 ***********************************************************
 `cfr`: a Python package for Climate Field Reconstruction
 ***********************************************************
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
-+ the analysis/visualization of the proxy records,
-+ the processing of the climate model simulations and instrumental observations,
++ the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
 + the calibration and running of the proxy system models (PSMs, `Evans et al., 2013 <https://doi.org/10.1016/j.quascirev.2013.05.024>`_),
 + the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR (`Hakim et al., 2016 <https://doi.org/10.1002/2016JD024751>`_; `Tardif et al., 2019 <https://doi.org/https://doi.org/10.5194/cp-15-1251-2019>`_) and GraphEM (`Guillot et al., 2015 <https://doi.org/10.1214/14-AOAS794>`_), and
 + the validation of the reconstructions, etc.
 
 For more details, please refer to the documentation linked below.
 
 Documentation
```

### Comparing `cfr-0.4.5/README.rst` & `cfr-0.4.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 ***********************************************************
 `cfr`: a Python package for Climate Field Reconstruction
 ***********************************************************
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
-+ the analysis/visualization of the proxy records,
-+ the processing of the climate model simulations and instrumental observations,
++ the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
 + the calibration and running of the proxy system models (PSMs, `Evans et al., 2013 <https://doi.org/10.1016/j.quascirev.2013.05.024>`_),
 + the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR (`Hakim et al., 2016 <https://doi.org/10.1002/2016JD024751>`_; `Tardif et al., 2019 <https://doi.org/https://doi.org/10.5194/cp-15-1251-2019>`_) and GraphEM (`Guillot et al., 2015 <https://doi.org/10.1214/14-AOAS794>`_), and
 + the validation of the reconstructions, etc.
 
 For more details, please refer to the documentation linked below.
 
 Documentation
```

### Comparing `cfr-0.4.5/bin/cfr` & `cfr-0.4.6/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/__init__.py` & `cfr-0.4.6/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/climate.py` & `cfr-0.4.6/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/da/enkf.py` & `cfr-0.4.6/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/gcm.py` & `cfr-0.4.6/cfr/gcm.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     coefficient_efficiency,
     p_header,
     p_hint,
     p_success,
     p_fail,
     p_warning,
     year_float2datetime,
+    regrid_field_curv_rect,
 )
 
 class GCMCase:
     ''' The class for postprocessing a GCM simulation case (e.g., CESM)
     
     Args:
         dirpath (str): the directory path where the reconstruction results are stored.
@@ -304,20 +305,22 @@
             fig.suptitle(title)
 
         if 'fig' in locals():
             return fig, ax
         else:
             return ax
             
-    def calc_slab_ocn_forcing(self, ds_clim, time_name='month', lat_name='TLAT', lon_name='TLONG',
+    def calc_som_forcings(self, ds_clim, time_name='month', lat_name='TLAT', lon_name='TLONG',
                               z_name='z_t', hblt_name='HBLT', temp_name='TEMP', salt_name='SALT',
                               uvel_name='UVEL', vvel_name='VVEL', shf_name='SHF', qflux_name='QFLUX',
                               anglet_name='ANGLET', region_mask_name='REGION_MASK',
-                              save_path=None, save_format='NETCDF4_CLASSIC'):
+                              save_path=None, save_format='NETCDF3_CLASSIC'):
         ''' Calculate the slab ocean forcing
+
+        Reference: NCL scripts by Jiang Zhu (jiangzhu@ucar.edu) at:  /glade/u/home/jiangzhu/notebooks/pop_frc_mlt.b.e21.B1850.f19_g17.PaleoCalibr.PI.02.ncl
         '''
         ds_clim = ds_clim.rename({time_name: 'time', 'nlat': 'nj', 'nlon': 'ni'})
         ds_clim.coords['time'] = [cftime.DatetimeNoLeap(1,i,1,0,0,0,0, has_year_zero=True) for i in range(1, 13)]
 
         hbltin = ds_clim[hblt_name]
         hblt_avg = hbltin.mean('time')
         hblttmp = hblt_avg.expand_dims({'time': 12})/100
@@ -500,18 +503,94 @@
         ds_out['area'].attrs['long_name'] = 'area of grid cell in radians squared'
         ds_out['area'].attrs['units'] = 'area'
 
         ds_out['mask'] = ds_clim[region_mask_name]
         ds_out['mask'].attrs['long_name'] = 'domain maskr'
         ds_out['mask'].attrs['units'] = 'unitless'
 
+        ds_out.attrs['title'] = 'Monthly averaged ocean forcing from POP output'
+        ds_out.attrs['conventions'] = 'CCSM data model domain description'
+        ds_out.attrs['source'] = 'cfr.gcm.GCMCase.calc_slab_ocn_forcing (https://github.com/fzhu2e/cfr)'
+        ds_out.attrs['description'] = 'Input data for DOCN7 mixed layer model'
+        ds_out.attrs['note1'] = 'fields computed from 100-yr monthly means from pop'
+        ds_out.attrs['note2'] = 'all fields interpolated to T-grid'
+        ds_out.attrs['note3'] = 'qdp is computed from depth summed ocean column'
+        ds_out.attrs['author'] = 'Feng Zhu (fengzhu@ucar.edu), Jiang Zhu (jiangzhu@ucar.edu)'
+        ds_out.attrs['calendar'] = 'standard'
+        ds_out.attrs['comment'] = 'This data is on the displaced pole grid gx1v7'
+        ds_out.attrs['creation_date'] = datetime.date.today().strftime('%m/%d/%Y')
+
+        if save_path is not None:
+            ds_out.to_netcdf(save_path, format=save_format)
+
+        return ds_out
+
+    def calc_cam_forcings(self, SST, aice, SST_time_name='time', SST_lat_name='TLAT', SST_lon_name='TLONG',
+                          aice_time_name='time', aice_lat_name='TLAT', aice_lon_name='TLON',
+                          save_path=None, save_format='NETCDF3_CLASSIC'):
+        ''' Calculate the forcings for CAM only simulation (F-case)
+
+        Note that the regridding is implemented by `pyresample` here instead of ESMF.
+
+        Reference: NCL scripts by Cecile Hannay (hannay@ucar.edu) at: /glade/u/home/hannay/ncl_scripts/sst/B1850_cmip6
+        '''
+        ds_out = xr.Dataset(
+            coords={
+                'time': SST[SST_time_name],
+                'lat': np.linspace(-89.5, 89.5, 180),
+                'lon': np.linspace(0.5, 359.5, 360),
+            }
+        )
+        ds_out['time'].attrs['information'] = 'middle of month'
+        ds_out['time'].attrs['calendar'] = 'gregorian'
+        ds_out['time'].attrs['units'] = 'days since 0001-01-01 00:00:00'
+
+        ds_out['lat'].attrs['long_name'] = 'latitude'
+        ds_out['lat'].attrs['units'] = 'degrees_north'
+
+        ds_out['lon'].attrs['long_name'] = 'longitude'
+        ds_out['lon'].attrs['units'] = 'degrees_east'
+
+
+        SST_rgd, _, _ = regrid_field_curv_rect(
+            SST.values, SST[SST_lat_name].values, SST[SST_lon_name].values,
+            ds_out.lat.values, ds_out.lon.values)
+
+        aice_rgd, _, _ = regrid_field_curv_rect(
+            aice.values, aice[aice_lat_name].values, aice[aice_lon_name].values,
+            ds_out.lat.values, ds_out.lon.values)
+
+        ds_out['SST'] = xr.DataArray(SST_rgd, coords=ds_out.coords)
+        ds_out['SST'].attrs['long_name'] = 'Sea-Surface temperature'
+        ds_out['SST'].attrs['units']     = 'deg_C'
+
+        ds_out['SEAICE'] = xr.DataArray(aice_rgd*100, coords=ds_out.coords)
+        ds_out['SEAICE'].attrs['long_name'] = 'Sea Ice Concentration'
+        ds_out['SEAICE'].attrs['units']     = '%'
+
+        # Corrections for data consistency
+        # 1) If SST < -1.8 or ice frac >= 90%, SST = -1.8
+        mask = (ds_out['SST'] < -1.8) | (ds_out['SEAICE'] > 90)
+        ds_out['SST'].values[mask] = -1.8
+        # 2) min ice frac is 0%, max ice_frac is 100%
+        mask = ds_out['SEAICE'] < 0
+        ds_out['SEAICE'].values[mask] = 0
+        mask = ds_out['SEAICE'] > 100
+        ds_out['SEAICE'].values[mask] = 100
+        # 3) No sea ice if SST > 4.97
+        mask = ds_out['SST'] > 4.97
+        ds_out['SEAICE'].values[mask] = 0
+
+        ds_out['ICEFRAC'] = ds_out['SEAICE'] / 100.
+
         if save_path is not None:
             ds_out.to_netcdf(save_path, format=save_format)
 
         return ds_out
+        
                 
 
 class GCMCases:
     ''' The class for postprocessing multiple GCM simulation cases (e.g., CESM)
     '''
     def __init__(self, case_dict=None):
         self.case_dict = case_dict
```

### Comparing `cfr-0.4.5/cfr/ml.py` & `cfr-0.4.6/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/proxy.py` & `cfr-0.4.6/cfr/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import xarray as xr
 import pandas as pd
 import numpy as np
 import plotly.express as px
 import copy
 from tqdm import tqdm
 from collections import OrderedDict
+from datetime import datetime
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 import cartopy.crs as ccrs
 from cartopy.util import add_cyclic_point
 from multiprocessing import Pool, cpu_count
 from functools import partial
 import seaborn as sns
@@ -142,14 +143,19 @@
             * 'ice.d18O' : Ice d18O isotopes
         tags (a set of str):
             the tags for the record, to enable tag filtering
     '''
     def __init__(self, pid=None, time=None, value=None, lat=None, lon=None, elev=None, ptype=None, tags=None,
         value_name=None, value_unit=None, time_name=None, time_unit=None, seasonality=None):
         self.pid = pid
+        if time is not None:
+            if len(time) == 1:
+                time = [time]
+            if not utils.is_numeric(time):
+                time = utils.datetime2year_float(time)
         self.time = time
         self.value = value
         self.lat = lat
         self.lon = np.mod(lon, 360) if lon is not None else None
         self.elev = elev
         self.ptype = ptype
         self.tags = set() if tags is None else tags
@@ -459,24 +465,33 @@
             proxy_time_max = np.max(self.time)
             pseudo_time_min = np.min(self.pseudo.time)
             pseudo_time_max = np.max(self.pseudo.time)
             time_min = np.max([proxy_time_min, pseudo_time_min])
             time_max = np.min([proxy_time_max, pseudo_time_max])
             mask_proxy = (self.time>=time_min)&(self.time<=time_max)
             mask_pseudo = (self.pseudo.time>=time_min)&(self.pseudo.time<=time_max)
+            if verbose:
+                utils.p_header(f'>>> timespan: ({time_min}, {time_max})')
+
 
         value = self.pseudo.value
 
         if match_var:
             value = value / np.nanstd(value[mask_pseudo]) * np.nanstd(self.value[mask_proxy])
-            if verbose: utils.p_success(f'>>> Variance matched.')
+            if verbose:
+                utils.p_header(f'>>> Var(proxy)={np.nanvar(self.value[mask_proxy])}')
+                utils.p_header(f'>>> Var(pseudoproxy)={np.nanvar(value[mask_pseudo])}')
+                utils.p_success(f'>>> Variance matched.')
 
         if match_mean:
             value = value - np.nanmean(value[mask_pseudo]) + np.nanmean(self.value[mask_proxy])
-            if verbose: utils.p_success(f'>>> Mean matched.')
+            if verbose:
+                utils.p_header(f'>>> Mean(proxy)={np.nanmean(self.value[mask_proxy])}')
+                utils.p_header(f'>>> Mean(pseudoproxy)={np.nanmean(value[mask_pseudo])}')
+                utils.p_success(f'>>> Mean matched.')
 
         self.pseudo.value = value
 
 
 
     def plotly(self, **kwargs):
         time_lb = visual.make_lb(self.time_name, self.time_unit)
```

### Comparing `cfr-0.4.5/cfr/psm.py` & `cfr-0.4.6/cfr/psm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from turtle import color
 import numpy as np
 import pandas as pd
+from datetime import datetime
 from scipy import integrate, signal, stats
 from tqdm import tqdm
 from multiprocessing import cpu_count
 try:
     import statsmodels.formula.api as smf
     from pathos.multiprocessing import ProcessingPool as Pool
     import fbm
```

### Comparing `cfr-0.4.5/cfr/reconjob.py` & `cfr-0.4.6/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/reconres.py` & `cfr-0.4.6/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/ts.py` & `cfr-0.4.6/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr/utils.py` & `cfr-0.4.6/cfr/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -450,14 +450,18 @@
 
     if lats is None:
         if lat_range is not None:
             lats = np.arange(lat_range[0], lat_range[-1]+dlat, dlat)
         else:
             lats = np.arange(np.min(lat_curv), np.max(lat_curv)+dlat, dlat)
 
+    # convert the longitude from (0, 360) to (-180, 180)
+    if np.min(lon_curv) >= 0:
+        lon_curv = (lon_curv+180) % 360 -180
+
     lon_rect, lat_rect = np.meshgrid(lons, lats)
     lon_rect = pyresample.utils.wrap_longitudes(lon_rect)
 
     if roi is None:
         roi = roi_factor * dlon
 
     old_grid = pyresample.geometry.SwathDefinition(lons=lon_curv, lats=lat_curv)
@@ -640,8 +644,12 @@
     for j in range(n):
         coeff = np.ndarray((np.size(f_vec)))
         coeff[regime1] = f_vec1**(-alpha1/2)
         coeff[regime2] = (s*f_vec2)**(-alpha2/2)
         sin_func = np.sin(2*np.pi*k*f0*t[j] + theta)
         y[j] = np.sum(coeff*sin_func)
 
-    return y
+    return y
+
+def is_numeric(obj):
+    attrs = ['__add__', '__sub__', '__mul__', '__truediv__', '__pow__']
+    return all(hasattr(obj, attr) for attr in attrs)
```

### Comparing `cfr-0.4.5/cfr/visual.py` & `cfr-0.4.6/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.4.5/cfr.egg-info/PKG-INFO` & `cfr-0.4.6/cfr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.4.5
+Version: 0.4.6
 Summary: cfr: the Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: paleocliamte reconstruction
 Classifier: Natural Language :: English
@@ -19,16 +19,15 @@
 ***********************************************************
 `cfr`: a Python package for Climate Field Reconstruction
 ***********************************************************
 
 `cfr` aims to provide a universal framework for climate field reconstruction (CFR).
 It provides a toolkit for
 
-+ the analysis/visualization of the proxy records,
-+ the processing of the climate model simulations and instrumental observations,
++ the processing and visualization of the proxy records, climate model simulations, and instrumental observations,
 + the calibration and running of the proxy system models (PSMs, `Evans et al., 2013 <https://doi.org/10.1016/j.quascirev.2013.05.024>`_),
 + the preparation and running of the multiple reconstruction frameworks/algorithms, such as LMR (`Hakim et al., 2016 <https://doi.org/10.1002/2016JD024751>`_; `Tardif et al., 2019 <https://doi.org/https://doi.org/10.5194/cp-15-1251-2019>`_) and GraphEM (`Guillot et al., 2015 <https://doi.org/10.1214/14-AOAS794>`_), and
 + the validation of the reconstructions, etc.
 
 For more details, please refer to the documentation linked below.
 
 Documentation
```

### Comparing `cfr-0.4.5/setup.py` & `cfr-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.4.5',
+    version='0.4.6',
     description='cfr: the Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

