# Comparing `tmp/flarespy-0.8.3.tar.gz` & `tmp/flarespy-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.8.3.tar", max compression
+gzip compressed data, was "flarespy-0.8.4.tar", max compression
```

## Comparing `flarespy-0.8.3.tar` & `flarespy-0.8.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.3/LICENSE
--rw-r--r--   0        0        0      428 2023-04-22 01:33:10.846417 flarespy-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.3/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.3/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.3/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25175 2023-04-22 01:27:55.396445 flarespy-0.8.3/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     6922 2023-04-22 01:27:55.389977 flarespy-0.8.3/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-22 01:33:10.844221 flarespy-0.8.3/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.8.4/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-22 16:11:30.424936 flarespy-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.8.4/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.8.4/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.8.4/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    29302 2023-04-22 16:09:52.872651 flarespy-0.8.4/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     7337 2023-04-22 03:01:00.209257 flarespy-0.8.4/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-22 16:11:30.422987 flarespy-0.8.4/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.8.4/PKG-INFO
```

### Comparing `flarespy-0.8.3/LICENSE` & `flarespy-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.3/src/flarespy/Flare_model.py` & `flarespy-0.8.4/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.3/src/flarespy/data/model.dat` & `flarespy-0.8.4/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.8.3/src/flarespy/flarefinder.py` & `flarespy-0.8.4/src/flarespy/flarefinder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import warnings
 
 import lightkurve as lk
 import numpy as np
 import pandas as pd
-from astropy import units as u
 from astropy.stats import mad_std
 from astropy.utils.exceptions import AstropyUserWarning
 from astroquery.exceptions import TableParseError
 from astroquery.vizier import Vizier
 from astroquery.jplhorizons import Horizons
 from astroquery.mast import Catalogs
 from astroquery.simbad import Simbad
@@ -16,14 +15,15 @@
 from matplotlib.offsetbox import AnchoredText
 from matplotlib.ticker import MaxNLocator
 from wotan import flatten
 
 from .utils import (
     CANDIDATES_COLUMNS,
     STELLAR_PARAMETER_COLUMNS,
+    calculate_stellar_luminosity,
     extend,
     fill_gaps,
     find_consecutive,
     get_flare_probability,
     query_gaia_dr3_id,
 )
 
@@ -33,17 +33,14 @@
 CUSTOM_SIMBAD.add_votable_fields("otype")
 CUSTOM_SIMBAD.add_votable_fields("otypes")
 
 VIZIER = Vizier(columns=["Plx", "Gmag", "BP-RP"])
 
 EXCLUDED_OTYPES = ["CataclyV*", "CataclyV*_Candidate", "Nova", "Nova_Candidate"]
 
-# Zero point TESS flux (from Sullivan 2017)
-TESS_FLUX0 = 4.03e-6 * u.erg / u.s / u.cm**2
-
 
 def load_from_lightkurve(lc):
     with warnings.catch_warnings():
         warnings.simplefilter("error", category=lk.LightkurveWarning)
 
         try:
             lc.meta["ZERO_CENTERED"] = False
@@ -67,14 +64,26 @@
 class FlareLightCurve(lk.LightCurve):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.meta["stellar_parameters"] = None
         self.meta["candidates"] = None
 
     def _generate_model(self):
+        """
+        Generate a model for the light curve.
+
+        This method generates a model for the light curve by computing a percentile-based
+        representation of the flux values.
+
+        Returns
+        -------
+        model_flux : ndarray
+            The model flux values.
+        """
+
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=RuntimeWarning)
             pg = self.to_periodogram()
             period = pg.period_at_max_power.value
             snr = pg.max_power / np.nanmedian(pg.power)
 
             if period < 10 and snr > 5:
@@ -114,14 +123,21 @@
             trend_folded_flux = trend_folded_flux_list[index]
             folded_lc = folded_lc_list[index]
 
             return trend_folded_flux[folded_lc.time_original.argsort()] - 1
         return 0
 
     def _mask_eclipse(self):
+        """
+        Mask the eclipses in the light curve.
+
+        This method masks the eclipses present in the light curve by setting the corresponding
+        flux values to NaN (Not a Number).
+        """
+
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=AstropyUserWarning)
 
             sigma = mad_std(self.flux, ignore_nan=True)
             eclipse_mask = self.flux < np.nanmedian(self.flux) - 3 * sigma
             if hasattr(self.flux, "mask"):
                 eclipse_mask = np.logical_xor(eclipse_mask, self.flux.mask)
@@ -151,79 +167,85 @@
                         )
                         lc.flux[(self.time.value >= t_start_ext) & (self.time.value <= t_stop_ext)] = np.nan
 
             self.meta["eclipse_mask"] = np.isnan(lc.flux)
 
         return lc
 
-    def _extend_multiple_events(self, i_start_array, i_stop_array, max_extend_indexes=45):
-        i_start_ext_array = np.zeros_like(i_start_array)
-        i_stop_ext_array = np.zeros_like(i_stop_array)
+    def _extend_multiple_events(self, start_indexes, stop_indexes, max_extend_indexes=45):
+        start_ext_indexes = np.zeros_like(start_indexes)
+        stop_ext_indexes = np.zeros_like(stop_indexes)
 
         lc = self.copy()
         lc.flux[self.eclipse_mask] = np.nan
         lc = lc.remove_nans()
 
-        for i in range(i_start_array.size):
-            i_start = i_start_array[i]
-            t_start = self.time.value[i_start]
-            i_stop = i_stop_array[i]
-            t_stop = self.time.value[i_stop]
+        max_extend_time = (max_extend_indexes + 0.2) * self.meta["TIMEDEL"]
+
+        for i, (start_index, stop_index) in enumerate(zip(start_indexes, stop_indexes)):
+            t_start = self.time.value[start_index]
+            t_stop = self.time.value[stop_index]
 
-            t_max_extend = (max_extend_indexes + 0.2) * self.meta["TIMEDEL"]
             t_start_ext, t_stop_ext = extend(
                 lc.time.value,
                 lc.standardized_flux,
                 t_start,
                 t_stop,
-                t_max_extend,
+                max_extend_time,
                 n_right=2,
             )
-            i_start_ext_array[i] = np.nonzero(self.time.value == t_start_ext)[0][0]
-            i_stop_ext_array[i] = np.nonzero(self.time.value == t_stop_ext)[0][0]
 
-        i_overlap = np.nonzero(i_start_ext_array[1:] <= i_stop_ext_array[:-1])[0] + 1
-        i_overlap_start, i_overlap_stop = find_consecutive(i_overlap, 1)
+            start_ext_indexes[i] = np.nonzero(self.time.value == t_start_ext)[0][0]
+            stop_ext_indexes[i] = np.nonzero(self.time.value == t_stop_ext)[0][0]
+
+        overlap_indexes = np.nonzero(start_ext_indexes[1:] <= stop_ext_indexes[:-1])[0] + 1
+        overlap_start, overlap_stop = find_consecutive(overlap_indexes, 1)
 
-        if i_overlap_start is not None:
-            i_stop_ext_array[i_overlap_start - 1] = i_stop_ext_array[i_overlap_stop]
-            i_start_ext_array = np.delete(i_start_ext_array, i_overlap)
-            i_stop_ext_array = np.delete(i_stop_ext_array, i_overlap)
+        if overlap_start is not None:
+            stop_ext_indexes[overlap_start - 1] = stop_ext_indexes[overlap_stop]
+            start_ext_indexes = np.delete(start_ext_indexes, overlap_indexes)
+            stop_ext_indexes = np.delete(stop_ext_indexes, overlap_indexes)
 
-        return i_start_ext_array, i_stop_ext_array
+        return start_ext_indexes, stop_ext_indexes
 
     def _standardize(self):
+        """
+        Standardize the detrended light curve.
+
+        This method standardizes the detrended light curve by dividing the difference between the
+        flux and 1 by the rolling standard deviation. It then adds the rolling standard deviation
+        and the standardized flux as new columns to the class.
+        """
+
         flux_series = pd.Series(self.detrended_flux.value, index=pd.DatetimeIndex(self.time.datetime))
 
         rolling_window = flux_series.rolling(pd.Timedelta(2, unit="d"), center=True)
         rolling_std = rolling_window.apply(mad_std, kwargs={"ignore_nan": True})
         rolling_std[np.isnan(self.detrended_flux.value)] = np.nan
 
         standardized_flux = (self.detrended_flux.value - 1) / rolling_std
 
         self.add_columns([rolling_std, standardized_flux], names=["rolling_std", "standardized_flux"])
 
-    def _calculate_stellar_luminosity(self):
-        self.meta["lum"] = np.nan
-        if self.stellar_parameters is None:
-            self.query_stellar_parameters()
-
-        # Calculate stellar luminosity
-        t_mag = self.stellar_parameters.Tmag
-        plx = self.stellar_parameters.Plx
-
-        if ~np.isnan(t_mag) and ~np.isnan(plx):
-            plx /= 1000
-            dist = 1 / plx * u.pc
-            flux = 10 ** (-t_mag / 2.5) * TESS_FLUX0
-            lum = 4 * np.pi * dist.to(u.cm) ** 2 * flux
-            self.meta["lum"] = lum.value
-
     def _is_sso(self, i_peak: int, radius: float = 8):
-        """Check if a candidate is caused by a Solar System Object (SSO) encounter."""
+        """
+        Check if a candidate is caused by a Solar System Object (SSO) encounter.
+
+        Parameters
+        ----------
+        i_peak : int
+            The index of the peak in the candidate light curve.
+        radius : float, optional
+            The search radius for SSOs, in arcseconds. Default is 8.
+
+        Returns
+        -------
+        bool
+            True if the candidate is caused by an SSO encounter, False otherwise.
+        """
 
         mask = np.zeros_like(self.time, dtype=bool)
         mask[i_peak] = True
 
         try:
             res = self.query_solar_system_objects(cadence_mask=mask, radius=radius * 21 / 3600, show_progress=False)
         except OSError:
@@ -259,26 +281,50 @@
                     ap_mag[row.Index] = eph["Tmag"].value
             if (ap_mag < 19).any():
                 return True
 
         return False
 
     def _is_at_edge(self, i_start: int, i_stop: int, window: float = 0.1):
-        """Check if a candidate is at the edge of the lightcurve."""
+        """
+        Check if a candidate is at the edge of a segment of the light curve.
+
+        Parameters
+        ----------
+        i_start : int
+            The start index of the candidate in the light curve.
+        i_stop : int
+            The stop index of the candidate in the light curve.
+        window : float, optional
+            The time window (in days) used to check if the candidate is at the edge. Default is 0.1.
+
+        Returns
+        -------
+        bool
+            False if the candidate is not at the edge of a segment of the light curve, True otherwise.
+        """
 
         time = self.time[np.isfinite(self.standardized_flux)].value
         t_start = self.time.value[i_start]
         t_stop = self.time.value[i_stop]
 
         before = np.nonzero((time > t_start - window) & (time < t_start))[0]
         after = np.nonzero((time > t_stop) & (time < t_stop + window))[0]
 
         return False if (before.size and after.size) else True
 
     def query_stellar_parameters(self):
+        """
+        Query the stellar parameters of the target star.
+
+        This method queries various stellar parameters of the target star, such as parallax,
+        Gmag, BP-RP, Tmag, and contamination ratio, from Gaia DR3, TIC, and SIMBAD databases.
+        It also checks if the target star has an excluded object type.
+        """
+
         self.stellar_parameters = pd.Series(index=STELLAR_PARAMETER_COLUMNS, dtype=object)
 
         gaia_dr3_id = query_gaia_dr3_id(self.ticid)
         self.stellar_parameters.gaia_dr3_source_id = gaia_dr3_id
         self.stellar_parameters.obs_duration = np.round(
             self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
         )
@@ -323,15 +369,29 @@
             obj_type = query_result["OTYPE"][0]
             self.stellar_parameters.obj_type = obj_type
 
             if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type.split("|"):
                 self.meta["exclude"] = True
 
     def detrend(self, window_length=0.3):
-        """Detrend the lightcurve."""
+        """
+        Detrend the light curve.
+
+        This method detrends the light curve by masking the eclipses, generating a model,
+        and applying a biweight filter to flatten the light curve. The detrended flux is
+        stored in a new column, and the standardized flux is calculated.
+
+        Parameters
+        ----------
+        window_length : float, optional
+            The window length (in days) for the detrending process. Default is 0.3.
+
+        This method detrends the light curve by removing systematic trends using a rolling
+        window approach. It then standardizes the detrended light curve.
+        """
 
         masked_lc = self._mask_eclipse()
         model_flux = self._generate_model()
         detrended_flux, trend_flux = flatten(
             self.time.value,
             masked_lc.flux - model_flux,
             method="biweight",
@@ -342,15 +402,34 @@
         self.add_columns(
             [detrended_flux * self.flux.unit, trend_flux * self.flux.unit],
             names=["detrended_flux", "trend_flux"],
         )
         self._standardize()
 
     def find_candidates(self, n_sigma: float = 3, n_consecutive: int = 2):
-        """Find the candidates of flares."""
+        """
+        Find the candidates of flares.
+
+        This method identifies potential flare candidates in the detrended light curve.
+        It searches for outliers above a certain threshold and groups them into
+        consecutive events. The method then filters out candidates at the edge of the
+        light curve and stores the candidate information in a DataFrame.
+
+        Parameters
+        ----------
+        n_sigma : float, optional
+            The threshold for identifying flare candidates as a multiple of the standard deviation.
+            Default is 3.
+        n_consecutive : int, optional
+            The minimum number of consecutive data points above the threshold to be considered a
+            candidate. Default is 2.
+
+        This method identifies potential flare candidates in the standardized light curve using
+        the specified threshold and number of consecutive data points.
+        """
 
         self.stellar_parameters.gaia_dr3_source_id = query_gaia_dr3_id(self.ticid)
         self.stellar_parameters.obs_duration = np.round(
             self.meta["TIMEDEL"] * np.nonzero(~np.isnan(self.flux.value))[0].size, 4
         )
 
         if not self.exclude:
@@ -384,25 +463,37 @@
                     self.candidates.i_peak = i_peak_array
                     self.candidates.i_stop = i_stop_ext_array
                     self.candidates.t_start = np.round(self.time.value[i_start_ext_array], 7)
                     self.candidates.t_peak = np.round(self.time.value[i_peak_array], 7)
                     self.candidates.t_stop = np.round(self.time.value[i_stop_ext_array], 7)
 
     def detect_sso(self):
-        """Detect if the candidates are caused by SSO encounters."""
+        """
+        Detect if the candidates are caused by SSO encounters.
+
+        This method checks if the flare candidates identified in the light curve are caused by
+        encounters with Solar System Objects (SSOs). It adds a boolean array to the candidates
+        DataFrame indicating whether a candidate is caused by an SSO encounter or not.
+        """
 
         if self.candidates is not None:
             sso = np.zeros(len(self.candidates), dtype=bool)
             for row in self.candidates.itertuples():
                 sso[row.Index] = self._is_sso(row.i_peak)
 
             self.candidates.sso = sso
 
     def calculate_candidate_parameters(self):
-        """Calculate the parameters of the candidates."""
+        """
+        Calculate the parameters of the candidates.
+
+        This method calculates various parameters for the identified flare candidates, such as
+        flare probability, signal-to-noise ratio (SNR), amplitude, duration, equivalent duration
+        (ED), and energy. The calculated parameters are added to the candidates DataFrame.
+        """
 
         if self.candidates is not None:
             proba_array = np.zeros(len(self.candidates))
             snr_array = np.zeros(len(self.candidates))
             for row in self.candidates.itertuples():
                 lc_candidate = self[row.i_start : row.i_stop + 1].remove_nans("standardized_flux")
                 time = lc_candidate.time.value
@@ -415,39 +506,51 @@
                     proba_array[row.Index] = round(get_flare_probability(time, flux), 3)
                 snr_array[row.Index] = round(np.max(flux), 2)
 
             self.candidates.flare_prob = proba_array
             self.candidates.snr = snr_array
 
             if not self.meta["ZERO_CENTERED"]:
+                if self.stellar_parameters is None:
+                    self.query_stellar_parameters()
+
                 amp = np.zeros(len(self.candidates))
                 dur = np.zeros(len(self.candidates))
                 ed = np.zeros(len(self.candidates))
-                self._calculate_stellar_luminosity()
+                stellar_lum = calculate_stellar_luminosity(self.stellar_parameters.Tmag, self.stellar_parameters.Plx)
 
                 n_row = 0
                 for row in self.candidates.itertuples():
                     time = self.time.value[row.i_start : row.i_stop + 1]
                     flux = self.detrended_flux[row.i_start : row.i_stop + 1]
                     amp[n_row] = np.nanmax(flux) - 1
                     dur[n_row] = (time[-1] - time[0]) * 1440
                     mask = np.isnan(flux)
                     ed[n_row] = np.trapz(flux[~mask] - 1, x=time[~mask] * 86400)
                     n_row += 1
 
                 self.candidates.amp = np.round(amp, 3)
                 self.candidates.dur = np.round(dur, 1)
                 self.candidates.ed = np.round(ed, 2)
-                if np.isnan(self.lum):
+                if np.isnan(stellar_lum):
                     self.candidates.energy = np.full(len(self.candidates), np.nan)
                 else:
-                    energy = ed * self.lum
+                    energy = ed * stellar_lum
                     self.candidates.energy = [np.format_float_scientific(x, precision=2) for x in energy]
 
     def find_flares(self):
+        """
+        Find flares in the light curve.
+
+        This method performs a series of steps to identify flares in the light curve. It queries
+        the stellar parameters of the target star, detrends the light curve, finds the flare
+        candidates, detects if the candidates are caused by SSO encounters, and calculates the
+        candidate parameters. The results are stored in the class attributes.
+        """
+
         self.query_stellar_parameters()
         self.detrend()
         self.find_candidates()
         self.detect_sso()
         self.calculate_candidate_parameters()
 
     def plot_candidates(self, figure_folder, threshold=0.5):
```

### Comparing `flarespy-0.8.3/src/flarespy/utils.py` & `flarespy-0.8.4/src/flarespy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     "Gmag",
     "BP-RP",
     "Tmag",
     "cont_ratio",
     "obs_duration",
 ]
 
+# Zero point TESS flux (from Sullivan 2017)
+TESS_FLUX0 = 4.03e-6 * u.erg / u.s / u.cm**2
+
 
 def extract_features(x):
     abs_energy = np.dot(x, x)
     first_location_of_maximum = np.argmax(x) / len(x)
 
     abs_x = np.abs(x)
     s = np.sum(abs_x)
@@ -79,52 +82,63 @@
             "flux__root_mean_square": [root_mean_square],
             "flux__skewness": [skewness],
             "flux__standard_deviation": [standard_deviation],
         }
     )
 
 
+def calculate_stellar_luminosity(t_mag, plx):
+    if isinstance(t_mag, float) and isinstance(plx, float):
+        plx /= 1000
+        dist = 1 / plx * u.pc
+        flux = 10 ** (-t_mag / 2.5) * TESS_FLUX0
+        lum = 4 * np.pi * dist.to(u.cm) ** 2 * flux
+        return lum.value
+    else:
+        return np.nan
+
+
 def get_flare_probability(time, flux):
     time *= 1440
     time -= time.min()
     feature = extract_features(flux)
 
     return RFC_MODEL.predict_proba(feature)[0][0]
 
 
 def extend(time, flux, t_start, t_stop, t_max_extend, n_sigma=1, n_left=1, n_right=1, mode=1):
     indexes_range = np.nonzero((time >= t_start - t_max_extend) & (time <= t_stop + t_max_extend))[0]
     i_start = np.nonzero(time == t_start)[0][0]
     i_stop = np.nonzero(time == t_stop)[0][0]
 
-    # left
     def condition_left(index):
         if mode == 1:
             return (flux[index - n_left : index] > n_sigma).any()
         elif mode == -1:
             return (flux[index - n_left : index] < n_sigma).any()
         else:
             raise ValueError("mode must be 1 or -1")
 
-    while condition_left(i_start) and i_start > indexes_range[0]:
-        i_start -= 1
-        if i_start < n_left:
-            i_start = 0
-            break
-    i_start = max(0, i_start - 1, indexes_range[0])
-
-    # right
     def condition_right(index):
         if mode == 1:
             return (flux[index + 1 : index + 1 + n_right] > n_sigma).any()
         elif mode == -1:
             return (flux[index + 1 : index + 1 + n_right] < n_sigma).any()
         else:
             raise ValueError("mode must be 1 or -1")
 
+    # Extend left
+    while condition_left(i_start) and i_start > indexes_range[0]:
+        i_start -= 1
+        if i_start < n_left:
+            i_start = 0
+            break
+    i_start = max(0, i_start - 1, indexes_range[0])
+
+    # Extend right
     while condition_right(i_stop) and i_stop < indexes_range[-1]:
         i_stop += 1
         if i_stop + 1 + n_right > time.size:
             i_stop = time.size - 1
             break
     i_stop = min(time.size - 1, i_stop + 1, indexes_range[-1])
 
@@ -135,15 +149,15 @@
     if data is None:
         grouped_data = np.split(indexes, np.nonzero(np.diff(indexes) > gap)[0] + 1)
     else:
         grouped_data = np.split(indexes, np.nonzero(np.diff(data[indexes]) > gap)[0] + 1)
 
     grouped_consecutive_data = [x for x in grouped_data if x.size >= n_consecutive]
 
-    if len(grouped_consecutive_data):
+    if grouped_consecutive_data:
         i_start_array = np.array([x[0] for x in grouped_consecutive_data], dtype=int)
         i_stop_array = np.array([x[-1] for x in grouped_consecutive_data], dtype=int)
         return i_start_array, i_stop_array
     else:
         return None, None
```

### Comparing `flarespy-0.8.3/PKG-INFO` & `flarespy-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.8.3
+Version: 0.8.4
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

