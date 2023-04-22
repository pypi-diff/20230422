# Comparing `tmp/kinisi-0.6.4.tar.gz` & `tmp/kinisi-0.6.5.tar.gz`

## Comparing `kinisi-0.6.4.tar` & `kinisi-0.6.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/analyze.py
--rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/analyzer.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/arrhenius.py
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/conductivity_analyzer.py
--rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/diffusion.py
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/diffusion_analyzer.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/jump_diffusion_analyzer.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/matrix.py
--rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/__init__.py
--rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_analyze.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_arrhenius.py
--rw-r--r--   0        0        0    38583 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_diffusion.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_matrix.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_parser.py
--rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.data
--rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.dcd
--rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/inputs/example_XDATCAR.gz
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.4/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.4/LICENSE
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.4/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 kinisi-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 kinisi-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/analyze.py
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/analyzer.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/arrhenius.py
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/conductivity_analyzer.py
+-rw-r--r--   0        0        0    34779 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/diffusion.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/diffusion_analyzer.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/jump_diffusion_analyzer.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/matrix.py
+-rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/__init__.py
+-rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_analyze.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_arrhenius.py
+-rw-r--r--   0        0        0    38583 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_diffusion.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_matrix.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/test_parser.py
+-rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.data
+-rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.dcd
+-rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.5/kinisi/tests/inputs/example_XDATCAR.gz
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.5/LICENSE
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.5/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 kinisi-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 kinisi-0.6.5/PKG-INFO
```

### Comparing `kinisi-0.6.4/kinisi/analyze.py` & `kinisi-0.6.5/kinisi/analyze.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/analyzer.py` & `kinisi-0.6.5/kinisi/analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/arrhenius.py` & `kinisi-0.6.5/kinisi/arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/conductivity_analyzer.py` & `kinisi-0.6.5/kinisi/conductivity_analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/diffusion.py` & `kinisi-0.6.5/kinisi/diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,15 +579,15 @@
             if bootstrap:
                 distro = self.sample_until_normal(coll_motion, n_o[i] / d_squared.shape[0], n_resamples, max_resamples, alpha, random_state)
                 self._distributions.append(distro)
                 self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
                 self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
                 self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
             self._n = np.append(self._n, coll_motion.mean())
-            self._v = np.append(self._v, np.var(coll_motion, ddof=1) / n_o[i] / d_squared.shape[0])
+            self._v = np.append(self._v, np.var(coll_motion, ddof=1) / (n_o[i] / d_squared.shape[0]))
             self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared.flatten()))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
 class MSCDBootstrap(Bootstrap):
@@ -650,15 +650,15 @@
             if bootstrap:
                 distro = self.sample_until_normal(sq_chg_motion, n_o[i] / d_squared.shape[0], n_resamples, max_resamples, alpha, random_state)
                 self._distributions.append(distro)
                 self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
                 self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
                 self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
             self._n = np.append(self._n, sq_chg_motion.mean())
-            self._v = np.append(self._v, np.var(sq_chg_motion, ddof=1) / n_o[i] / d_squared.shape[0])
+            self._v = np.append(self._v, np.var(sq_chg_motion, ddof=1) / (n_o[i] / d_squared.shape[0]))
             self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared.flatten()))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
 def _bootstrap(array: np.ndarray,
```

### Comparing `kinisi-0.6.4/kinisi/diffusion_analyzer.py` & `kinisi-0.6.5/kinisi/diffusion_analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/jump_diffusion_analyzer.py` & `kinisi-0.6.5/kinisi/jump_diffusion_analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/matrix.py` & `kinisi-0.6.5/kinisi/matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/parser.py` & `kinisi-0.6.5/kinisi/parser.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/test_analyze.py` & `kinisi-0.6.5/kinisi/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/test_arrhenius.py` & `kinisi-0.6.5/kinisi/tests/test_arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/test_diffusion.py` & `kinisi-0.6.5/kinisi/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/test_matrix.py` & `kinisi-0.6.5/kinisi/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/test_parser.py` & `kinisi-0.6.5/kinisi/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.data` & `kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.data`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.dcd` & `kinisi-0.6.5/kinisi/tests/inputs/example_LAMMPS.dcd`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/kinisi/tests/inputs/example_XDATCAR.gz` & `kinisi-0.6.5/kinisi/tests/inputs/example_XDATCAR.gz`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/LICENSE` & `kinisi-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/README.md` & `kinisi-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/pyproject.toml` & `kinisi-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.4/PKG-INFO` & `kinisi-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinisi
-Version: 0.6.4
+Version: 0.6.5
 Summary: Efficient estimation of diffusion processes from molecular dynamics.
 Project-URL: homepage, https://github.com/bjmorgan/kinisi
 Project-URL: documentation, https://kinisi.rtfd.io
 Author-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 Maintainer-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 License-Expression: MIT
 License-File: LICENSE
```

