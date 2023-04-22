# Comparing `tmp/nautilus-sampler-0.5.0.tar.gz` & `tmp/nautilus-sampler-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus-sampler-0.5.0.tar", last modified: Sun Apr  2 14:44:36 2023, max compression
+gzip compressed data, was "nautilus-sampler-0.6.0.tar", last modified: Sat Apr 22 16:59:35 2023, max compression
```

## Comparing `nautilus-sampler-0.5.0.tar` & `nautilus-sampler-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5835 2023-04-02 14:29:16.882904 nautilus-sampler-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2022-09-13 17:16:29.198585 nautilus-sampler-0.5.0/LICENSE
--rw-r--r--   0        0        0     2328 2023-02-24 20:22:18.708380 nautilus-sampler-0.5.0/README.md
--rw-r--r--   0        0        0      218 2023-04-02 14:29:41.906705 nautilus-sampler-0.5.0/nautilus/__init__.py
--rw-r--r--   0        0        0      316 2023-04-02 14:28:30.630272 nautilus-sampler-0.5.0/nautilus/bounds/__init__.py
--rw-r--r--   0        0        0    19950 2023-04-02 14:28:30.630272 nautilus-sampler-0.5.0/nautilus/bounds/basic.py
--rw-r--r--   0        0        0    15184 2023-04-02 14:28:30.630272 nautilus-sampler-0.5.0/nautilus/bounds/neural.py
--rw-r--r--   0        0        0    12215 2023-04-02 14:28:30.630272 nautilus-sampler-0.5.0/nautilus/bounds/union.py
--rw-r--r--   0        0        0     5961 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/nautilus/neural.py
--rw-r--r--   0        0        0     5967 2023-02-09 20:46:18.826604 nautilus-sampler-0.5.0/nautilus/prior.py
--rw-r--r--   0        0        0    44873 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/nautilus/sampler.py
--rw-r--r--   0        0        0      676 2023-02-09 20:46:18.827604 nautilus-sampler-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3911 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/tests/test_blobs.py
--rw-r--r--   0        0        0    14243 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/tests/test_bounds.py
--rw-r--r--   0        0        0     5015 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/tests/test_io.py
--rw-r--r--   0        0        0      485 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/tests/test_neural.py
--rw-r--r--   0        0        0      907 2023-04-02 14:28:30.631272 nautilus-sampler-0.5.0/tests/test_pool.py
--rw-r--r--   0        0        0     3714 2023-02-09 20:46:18.827604 nautilus-sampler-0.5.0/tests/test_prior.py
--rw-r--r--   0        0        0     6088 2023-04-02 14:28:30.632272 nautilus-sampler-0.5.0/tests/test_sampler.py
--rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 nautilus-sampler-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7214 2023-04-22 16:20:51.042005 nautilus-sampler-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2022-09-13 17:16:29.198585 nautilus-sampler-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2328 2023-04-08 15:51:59.349856 nautilus-sampler-0.6.0/README.md
+-rw-r--r--   0        0        0      218 2023-04-22 16:22:04.286320 nautilus-sampler-0.6.0/nautilus/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-13 13:59:25.226473 nautilus-sampler-0.6.0/nautilus/bounds/__init__.py
+-rw-r--r--   0        0        0    21190 2023-04-17 13:48:20.350706 nautilus-sampler-0.6.0/nautilus/bounds/basic.py
+-rw-r--r--   0        0        0    17091 2023-04-21 17:37:12.091755 nautilus-sampler-0.6.0/nautilus/bounds/neural.py
+-rw-r--r--   0        0        0    12919 2023-04-18 20:14:08.615652 nautilus-sampler-0.6.0/nautilus/bounds/union.py
+-rw-r--r--   0        0        0     5773 2023-04-17 13:39:44.038203 nautilus-sampler-0.6.0/nautilus/neural.py
+-rw-r--r--   0        0        0     5967 2023-02-09 20:46:18.826604 nautilus-sampler-0.6.0/nautilus/prior.py
+-rw-r--r--   0        0        0    47556 2023-04-17 13:39:44.039203 nautilus-sampler-0.6.0/nautilus/sampler.py
+-rw-r--r--   0        0        0      676 2023-02-09 20:46:18.827604 nautilus-sampler-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3911 2023-04-13 13:59:25.227473 nautilus-sampler-0.6.0/tests/test_blobs.py
+-rw-r--r--   0        0        0    13616 2023-04-17 13:48:20.350706 nautilus-sampler-0.6.0/tests/test_bounds.py
+-rw-r--r--   0        0        0     5450 2023-04-21 17:36:57.153594 nautilus-sampler-0.6.0/tests/test_io.py
+-rw-r--r--   0        0        0      486 2023-04-17 13:39:44.039203 nautilus-sampler-0.6.0/tests/test_neural.py
+-rw-r--r--   0        0        0      907 2023-04-13 13:59:25.228473 nautilus-sampler-0.6.0/tests/test_pool.py
+-rw-r--r--   0        0        0     3714 2023-02-09 20:46:18.827604 nautilus-sampler-0.6.0/tests/test_prior.py
+-rw-r--r--   0        0        0     6064 2023-04-17 13:48:20.350706 nautilus-sampler-0.6.0/tests/test_sampler.py
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 nautilus-sampler-0.6.0/PKG-INFO
```

### Comparing `nautilus-sampler-0.5.0/CHANGELOG.md` & `nautilus-sampler-0.6.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,32 @@
 # Changelog
 
 All notable changes to nautilus will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased]
+## [0.6.0] - 2023-04-22
+
+### Changed
+- The code now uses the more modern `numpy.random.Generator` framework instead of `numpy.random.RandomState`.
+- Added the keyword arguments `n_points_min` and `split_threshold` to the sampler. Previously, they were not accessible.
+- The default value for `n_points_min` is now the number of dimensions plus 50. Previously, it was hard-coded to be the number of dimensions plus 1.
+- The multi-ellipsoidal decomposition has been tweaked with the goal of reducing computational overhead for high-dimensional problems.
+- The default number of parallel processes has been changed to one. By default, the sampler will not use parallelization.
+- Multi-ellipsoidal decomposition now uses Gaussian mixture modeling instead of K-Means. The former typically results in better performance, i.e., smaller boundaries with fewer ellipsoids.
+- Sampling new points can now be parallelized using the `n_jobs` keyword argument.
+
+### Fixed
+- The sampler now correctly writes the random number generator in the sampling phase.
+- The keyword argument `n_jobs` is now being correctly passed when training networks. Previously, all cores were used regardless of `n_jobs`.
+- The sampler doesn't crash when setting `verbose=True`and `n_networks=0`.
+
+### Deprecated
+- The `random_state` keyword argument for the sampler has been deprecated in favor of the new keyword argument `seed`.
 
 ## [0.5.0] - 2023-04-02
 
 ### Changed
 - Introduced neural network ensembles. Instead of relying on a single network, the sampler now uses 4 networks by default. This should lead to better sampling performance. The training of the networks is done in parallel, by default. Which means that on multi-core systems, time spent on neural network training shouldn't increase dramatically. The number of networks and training parallelization can be adjusted by the user.
 - Introduced new bounds that lead to lower overhead for high-dimensional problems. The number of likelihood calls should be close to unaffected by this change.
 - Increased the default number of live points from 1500 to 2000.
```

### Comparing `nautilus-sampler-0.5.0/LICENSE` & `nautilus-sampler-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/README.md` & `nautilus-sampler-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/nautilus/bounds/basic.py` & `nautilus-sampler-0.6.0/nautilus/bounds/basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,43 +12,43 @@
     The :math:`n`-dimensional unit hypercube has :math:`n_{\rm dim}` parameters
     :math:`x_i` with :math:`0 \leq x_i < 1` for all :math:`x_i`.
 
     Attributes
     ----------
     n_dim : int
         Number of dimensions.
-    random_state : numpy.random.RandomState instance
+    rng : numpy.random.Generator
         Determines random number generation.
 
     """
 
     @classmethod
-    def compute(cls, n_dim, random_state=None):
+    def compute(cls, n_dim, rng=None):
         """Compute the bound.
 
         Parameters
         ----------
         n_dim : int
             Number of dimensions.
-        random_state : None or numpy.random.RandomState instance, optional
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : UnitCube
             The bound.
 
         """
         bound = cls()
         bound.n_dim = n_dim
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
         return bound
 
     def contains(self, points):
         """Check whether points are contained in the bound.
 
         Parameters
@@ -62,29 +62,31 @@
         in_bound : bool or numpy.ndarray
             Bool or array of bools describing for each point whether it is
             contained in the bound.
 
         """
         return np.all((points >= 0) & (points < 1), axis=-1)
 
-    def sample(self, n_points=100):
+    def sample(self, n_points=100, pool=None):
         """Sample points from the bound.
 
         Parameters
         ----------
         n_points : int, optional
             How many points to draw. Default is 100.
+        pool : ignored
+            Not used. Present for API consistency.
 
         Returns
         -------
         points : numpy.ndarray
             Points as two-dimensional array of shape (n_points, n_dim).
 
         """
-        points = self.random_state.random(size=(n_points, self.n_dim))
+        points = self.rng.random(size=(n_points, self.n_dim))
         return points
 
     def volume(self):
         """Return the natural log of the volume of the bound.
 
         Returns
         -------
@@ -103,41 +105,54 @@
             HDF5 group to write to.
 
         """
         group.attrs['type'] = 'UnitCube'
         group.attrs['n_dim'] = self.n_dim
 
     @classmethod
-    def read(cls, group, random_state=None):
+    def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
         group : h5py.Group
             HDF5 group to write to.
-        random_state : None or numpy.random.RandomState instance, optional
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : UnitCube
             The bound.
 
         """
         bound = cls()
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
         bound.n_dim = group.attrs['n_dim']
 
         return bound
 
+    def reset(self, rng=None):
+        """Reset random number generation and any progress, if applicable.
+
+        Parameters
+        ----------
+        rng : None or numpy.random.Generator, optional
+            Determines random number generation. If None, random number
+            generation is not reset. Default is None.
+
+        """
+        if rng is not None:
+            self.rng = rng
+
 
 def invert_symmetric_positive_semidefinite_matrix(m):
     """Invert a symmetric positive sem-definite matrix.
 
     This function is faster than numpy.linalg.inv but does not work for
     arbitrary matrices.
 
@@ -152,15 +167,15 @@
         Inverse of the matrix.
 
     """
     m_inv_triangle = dpotri(dpotrf(m)[0])[0]
     return m_inv_triangle + m_inv_triangle.T - np.diag(np.diag(m_inv_triangle))
 
 
-def minimum_volume_enclosing_ellipsoid(points, tol=0, max_iterations=500):
+def minimum_volume_enclosing_ellipsoid(points, tol=0, max_iterations=1000):
     r"""Find an approximation to the minimum volume enclosing ellipsoid (MVEE).
 
     This functions finds an approximation to the MVEE using the Khachiyan
     algorithm.
 
     This function is based on
     http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.116.7691 but
@@ -231,37 +246,41 @@
         :math:`(x - c)^T A (x - c) \leq 1`.
     B : numpy.ndarray
         Cholesky decomposition of the inverse of A.
     B_inv : numpy.ndarray
         Inverse of B.
     log_v : float
         Natural log of the volume of the ellipsoid.
-    random_state : numpy.random.RandomState instance
+    rng : numpy.random.Generator
         Determines random number generation.
 
     """
 
     @classmethod
     def compute(cls, points, enlarge_per_dim=1.1, fast=False,
-                random_state=None):
+                max_iterations=1000, rng=None):
         """Compute the bound.
 
         Parameters
         ----------
         points : numpy.ndarray with shape (n_points, n_dim)
             A 2-D array where each row represents a point.
         enlarge_per_dim : float, optional
             Along each dimension, the ellipsoid is enlarged by this factor.
             Default is 1.1.
         fast : bool, optional
             If True, calculate the bounding ellipsoid from the mean and
             covariance of the points. If False, the ellipsoid (ignoring
-            `enlarge_per_dim` is an approximation to a minimum volume enclosing
-            ellipsoid. Default is False.
-        random_state : None or numpy.random.RandomState instance, optional
+            `enlarge_per_dim`) is an approximation to a minimum volume
+            enclosing ellipsoid. Default is False.
+        max_iterations : int, optional
+            Maximum number of iterations before the minimization algorithm for
+            the minimum volume enclosing ellipsoid is stopped. Ignored if
+            `fast` is True. Default is 1000.
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Raises
         ------
         ValueError
             If `enlarge_per_dim` is smaller than unity or the number of points
             does not exceed the number of dimensions.
@@ -281,15 +300,16 @@
 
         if not points.shape[0] > bound.n_dim:
             raise ValueError('Number of points must be larger than number ' +
                              'dimensions.')
 
         if not fast:
             with threadpool_limits(limits=1):
-                bound.c, bound.A = minimum_volume_enclosing_ellipsoid(points)
+                bound.c, bound.A = minimum_volume_enclosing_ellipsoid(
+                    points, max_iterations=max_iterations)
         else:
             bound.c = np.mean(points, axis=0)
             bound.A = np.linalg.inv(np.atleast_2d(np.cov(
                 points, rowvar=False)))
             scale = np.amax(np.einsum(
                 '...i,ij,...j', points - bound.c, bound.A, points - bound.c))
             bound.A /= scale
@@ -298,18 +318,18 @@
         bound.B = np.linalg.cholesky(np.linalg.inv(bound.A))
         bound.B_inv = np.linalg.inv(bound.B)
         bound.log_v = (np.linalg.slogdet(bound.B)[1] +
                        bound.n_dim * np.log(2.) +
                        bound.n_dim * gammaln(1.5) -
                        gammaln(bound.n_dim / 2.0 + 1))
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
         return bound
 
     def transform(self, points, inverse=False):
         """Transform points into the coordinate frame of the ellipsoid.
 
         Parameters
@@ -355,25 +375,25 @@
 
     def sample(self, n_points=100):
         """Sample points from the bound.
 
         Parameters
         ----------
         n_points : int, optional
-            How many points to draw.
+            How many points to draw. Default is 100.
 
         Returns
         -------
         points : numpy.ndarray
             Points as two-dimensional array of shape (n_points, n_dim).
 
         """
-        points = self.random_state.normal(size=(n_points, self.n_dim))
+        points = self.rng.normal(size=(n_points, self.n_dim))
         points = points / np.sqrt(np.sum(points**2, axis=1))[:, np.newaxis]
-        points *= self.random_state.uniform(size=n_points)[:, np.newaxis]**(
+        points *= self.rng.uniform(size=n_points)[:, np.newaxis]**(
             1.0 / self.n_dim)
         points = self.transform(points, inverse=True)
         return points
 
     def volume(self):
         """Return the natural log of the volume of the bound.
 
@@ -395,42 +415,55 @@
 
         """
         group.attrs['type'] = 'Ellipsoid'
         for key in ['n_dim', 'c', 'A', 'B', 'B_inv', 'log_v']:
             group.attrs[key] = getattr(self, key)
 
     @classmethod
-    def read(cls, group, random_state=None):
+    def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
         group: h5py.Group
             HDF5 group to write to.
-        random_state: None or numpy.random.RandomState instance, optional
+        rng: None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound: Ellipsoid
             The bound.
 
         """
         bound = cls()
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
         for key in ['n_dim', 'c', 'A', 'B', 'B_inv', 'log_v']:
             setattr(bound, key, group.attrs[key])
 
         return bound
 
+    def reset(self, rng=None):
+        """Reset random number generation and any progress, if applicable.
+
+        Parameters
+        ----------
+        rng : None or numpy.random.Generator, optional
+            Determines random number generation. If None, random number
+            generation is not reset. Default is None.
+
+        """
+        if rng is not None:
+            self.rng = rng
+
 
 class UnitCubeEllipsoidMixture():
     """Mixture of a unit cube and an ellipsoid.
 
     Dimensions along which an ellipsoid has a smaller volume than a unit cube
     are defined via ellipsoids and vice versa.
 
@@ -440,72 +473,71 @@
         Number of dimensions.
     dim_cube: numpy.ndarray
         Whether the boundary in each dimension is defined via the unit cube.
     cube: UnitCube or None
         Unit cube defining the boundary along certain dimensions.
     ellipsoid: Ellipsoid or None
         Ellipsoid defining the boundary along certain dimensions.
-    random_state: numpy.random.RandomState instance
-        Determines random number generation.
+
     """
 
     @classmethod
-    def compute(cls, points, enlarge_per_dim=1.1, random_state=None):
+    def compute(cls, points, enlarge_per_dim=1.1, rng=None):
         """Compute the bound.
 
         Parameters
         ----------
         points: numpy.ndarray with shape(n_points, n_dim)
             A 2-D array where each row represents a point.
         enlarge_per_dim: float, optional
             Along each dimension, the ellipsoid is enlarged by this factor.
             Default is 1.1.
-        random_state: None or numpy.random.RandomState instance, optional
+        rng: None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound: UnitCubeEllipsoidMixture
             The bound.
 
         """
         bound = cls()
         bound.n_dim = points.shape[1]
 
-        kwargs = dict(enlarge_per_dim=enlarge_per_dim,
-                      random_state=random_state)
+        kwargs = dict(enlarge_per_dim=enlarge_per_dim, max_iterations=100,
+                      rng=rng)
 
         # First, calculate a bounding ellipsoid along all dimensions.
-        ellipsoid = Ellipsoid.compute(points, fast=True, **kwargs)
+        ellipsoid = Ellipsoid.compute(points, **kwargs)
+        ellipsoid_fast = Ellipsoid.compute(points, fast=True, **kwargs)
         bound.dim_cube = np.zeros(bound.n_dim, dtype=bool)
-        # Now, determine which dimensions have a smaller volume when using the
+        # Now, estimate which dimensions have a smaller volume when using the
         # cube.
         for dim in range(bound.n_dim):
-            ellipsoid_dim = Ellipsoid.compute(
+            ellipsoid_dim_fast = Ellipsoid.compute(
                 np.delete(points, dim, axis=1), fast=True, **kwargs)
-            if ellipsoid.volume() > ellipsoid_dim.volume():
-                bound.dim_cube[dim] = True
+            if ellipsoid_fast.volume() > ellipsoid_dim_fast.volume():
+                ellipsoid_dim = Ellipsoid.compute(
+                    np.delete(points, dim, axis=1), fast=False, **kwargs)
+                if ellipsoid.volume() > ellipsoid_dim.volume():
+                    bound.dim_cube[dim] = True
+
+        kwargs['max_iterations'] = 1000
 
         if np.any(bound.dim_cube):
-            bound.cube = UnitCube.compute(
-                np.sum(bound.dim_cube), random_state=random_state)
+            bound.cube = UnitCube.compute(np.sum(bound.dim_cube), rng=rng)
         else:
             bound.cube = None
 
         if np.all(bound.dim_cube):
             bound.ellipsoid = None
         else:
             bound.ellipsoid = Ellipsoid.compute(
                 points[:, np.arange(bound.n_dim)[~bound.dim_cube]], **kwargs)
 
-        if random_state is None:
-            bound.random_state = np.random
-        else:
-            bound.random_state = random_state
-
         return bound
 
     def transform(self, points):
         """Transform points into the frame of the cube-ellipsoid mixture.
 
         Along dimensions where the boundary is not defined via the unit range,
         the coordinates are transformed into the range [-1, +1]. Along all
@@ -560,20 +592,20 @@
 
     def sample(self, n_points=100):
         """Sample points from the bound.
 
         Parameters
         ----------
         n_points: int, optional
-            How many points to draw.
+            How many points to draw. Default is 100.
 
         Returns
         -------
         points: numpy.ndarray
-            Points as two-dimensional array of shape(n_points, n_dim).
+            Points as two-dimensional array of shape (n_points, n_dim).
 
         """
         points = np.zeros((n_points, self.n_dim))
         if self.cube is not None:
             idx = np.arange(self.n_dim)[self.dim_cube]
             points[:, idx] = self.cube.sample(n_points)
         if self.ellipsoid is not None:
@@ -610,46 +642,58 @@
         group.create_dataset('dim_cube', data=self.dim_cube)
         if self.cube is not None:
             self.cube.write(group.create_group('cube'))
         if self.ellipsoid is not None:
             self.ellipsoid.write(group.create_group('ellipsoid'))
 
     @classmethod
-    def read(cls, group, random_state=None):
+    def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
         group: h5py.Group
             HDF5 group to write to.
-        random_state: None or numpy.random.RandomState instance, optional
+        rng: None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound: UnitCubeEllipsoidMixture
             The bound.
 
         """
         bound = cls()
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
-        else:
-            bound.random_state = random_state
+        if rng is None:
+            rng = np.random.default_rng()
 
         bound.n_dim = group.attrs['n_dim']
         bound.dim_cube = np.array(group['dim_cube'])
 
         if np.any(bound.dim_cube):
-            bound.cube = UnitCube.read(
-                group['cube'], random_state=bound.random_state)
+            bound.cube = UnitCube.read(group['cube'], rng=rng)
         else:
             bound.cube = None
 
         if not np.all(bound.dim_cube):
-            bound.ellipsoid = Ellipsoid.read(
-                group['ellipsoid'], random_state=bound.random_state)
+            bound.ellipsoid = Ellipsoid.read(group['ellipsoid'], rng=rng)
         else:
             bound.ellipsoid = None
 
         return bound
+
+    def reset(self, rng=None):
+        """Reset random number generation and any progress, if applicable.
+
+        Parameters
+        ----------
+        rng : None or numpy.random.Generator, optional
+            Determines random number generation. If None, random number
+            generation is not reset. Default is None.
+
+        """
+        if rng is not None:
+            if self.ellipsoid is not None:
+                self.ellipsoid.reset(rng)
+            if self.cube is not None:
+                self.cube.reset(rng)
```

### Comparing `nautilus-sampler-0.5.0/nautilus/bounds/neural.py` & `nautilus-sampler-0.6.0/nautilus/bounds/neural.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """Module implementing multi-dimensional neural network-based bounds."""
 
 import numpy as np
+from functools import partial
 from scipy.stats import percentileofscore
+from threadpoolctl import threadpool_limits
 
 from .basic import Ellipsoid, UnitCubeEllipsoidMixture
 from .union import Union
 from ..neural import NeuralNetworkEmulator
 
 
 class NeuralBound():
     """Neural network-based bound.
 
     Attributes
     ----------
     n_dim : int
         Number of dimensions.
-    random_state : numpy.random or numpy.random.RandomState instance
-        Determines random number generation.
     outer_bound : UnitCubeEllipsoidMixture
         Outer bound around the points above the likelihood threshold.
     emulator : object
         Emulator based on `sklearn.neural_network.MLPRegressor` used to fit and
         predict likelihood scores.
     score_predict_min : float
         Minimum score predicted by the emulator to be considered part of the
         bound.
     """
 
     @classmethod
     def compute(cls, points, log_l, log_l_min, enlarge_per_dim=1.1,
-                n_networks=4, neural_network_kwargs={}, n_jobs='max',
-                random_state=None):
+                n_networks=4, neural_network_kwargs={}, pool=None,
+                rng=None):
         """Compute a neural network-based bound.
 
         Parameters
         ----------
         points : numpy.ndarray with shape (m, n)
             A 2-D array where each row represents a point.
         log_l : numpy.ndarray of length m
@@ -45,38 +45,35 @@
             Along each dimension, the ellipsoid of the outer bound is enlarged
             by this factor. Default is 1.1.
         n_networks : int, optional
             Number of networks used in the emulator. Default is 4.
         neural_network_kwargs : dict, optional
             Non-default keyword arguments passed to the constructor of
             MLPRegressor.
-        n_jobs : int or string, optional
-            Number of parallel jobs to use for training. If the string 'max' is
-            passed, all available cores are used.
-        random_state : None or numpy.random.RandomState instance, optional
+        pool : multiprocessing.Pool, optional
+            Pool used for parallel processing.
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : NeuralBound
             The bound.
 
         """
         bound = cls()
         bound.n_dim = points.shape[1]
 
-        if random_state is None:
-            bound.random_state = np.random
-        else:
-            bound.random_state = random_state
+        if rng is None:
+            rng = np.random.default_rng()
 
         # Determine the outer bound.
         bound.outer_bound = Ellipsoid.compute(
             points[log_l > log_l_min], enlarge_per_dim=enlarge_per_dim,
-            random_state=bound.random_state)
+            rng=rng)
 
         if n_networks == 0:
             bound.emulator = None
             bound.score_predict_min = 0
             return bound
 
         # Train the network.
@@ -90,15 +87,15 @@
         score = np.zeros(len(points))
         select = perc < perc_min
         if np.any(select):
             score[select] = 0.5 * (perc[select] / perc_min)
         score[~select] = 1 - 0.5 * (1 - perc[~select]) / (1 - perc_min)
         bound.emulator = NeuralNetworkEmulator.train(
             points_t, score, n_networks=n_networks,
-            neural_network_kwargs=neural_network_kwargs, n_jobs='max')
+            neural_network_kwargs=neural_network_kwargs, pool=pool)
 
         bound.score_predict_min = np.polyval(np.polyfit(
             score, bound.emulator.predict(points_t), 3), 0.5)
 
         return bound
 
     def contains(self, points):
@@ -121,15 +118,15 @@
 
         in_bound = self.outer_bound.contains(points)
         if np.any(in_bound) and self.emulator is not None:
             points_t = self.outer_bound.transform(points)
             in_bound[in_bound] = (self.emulator.predict(points_t[in_bound]) >
                                   self.score_predict_min)
 
-        return np.squeeze(in_bound)
+        return in_bound
 
     def write(self, group):
         """Write the bound to an HDF5 group.
 
         Parameters
         ----------
         group : h5py.Group
@@ -139,40 +136,38 @@
         group.attrs['n_dim'] = self.n_dim
         group.attrs['score_predict_min'] = self.score_predict_min
         self.outer_bound.write(group.create_group('outer_bound'))
         if self.emulator is not None:
             self.emulator.write(group.create_group('emulator'))
 
     @classmethod
-    def read(cls, group, random_state=None):
+    def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
         group : h5py.Group
             HDF5 group to write to.
-        random_state : None or numpy.random.RandomState instance, optional
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : NeuralBound
             The bound.
 
         """
         bound = cls()
 
-        if random_state is None:
-            bound.random_state = np.random
-        else:
-            bound.random_state = random_state
+        if rng is None:
+            rng = np.random.default_rng()
 
         bound.n_dim = group.attrs['n_dim']
         bound.score_predict_min = group.attrs['score_predict_min']
-        bound.outer_bound = Ellipsoid.read(group['outer_bound'])
+        bound.outer_bound = Ellipsoid.read(group['outer_bound'], rng=rng)
         if 'emulator' in group:
             bound.emulator = NeuralNetworkEmulator.read(group['emulator'])
         else:
             bound.emulator = None
 
         return bound
 
@@ -181,33 +176,36 @@
     """Union of multiple non-overlapping neural network-based bounds.
 
     The bound is the overlap of the union of multiple neural network-based
     bounds and the unit hypercube.
 
     Attributes
     ----------
+    n_dim : int
+        Number of dimensions.
     neural_bounds : list
         List of the individual neural network-based bounds.
     outer_bound : Union
         Outer bound used for sampling.
-    random_state : None or numpy.random.RandomState instance
+    rng : None or numpy.random.Generator
         Determines random number generation.
-    points_sample : numpy.ndarray
+    points : numpy.ndarray
         Points that a call to `sample` will return next.
     n_sample : int
-        Number of points sampled from all ellipsoids.
+        Number of points sampled from the outer bound.
     n_reject : int
-        Number of points rejected due to overlap.
+        Number of points rejected due to not falling into the neural
+        network-based bounds.
     """
 
     @classmethod
     def compute(cls, points, log_l, log_l_min, log_v_target,
                 enlarge_per_dim=1.1, n_points_min=None, split_threshold=100,
-                n_networks=4, neural_network_kwargs={}, n_jobs='max',
-                random_state=None):
+                n_networks=4, neural_network_kwargs={}, pool=None,
+                rng=None):
         """Compute a union of multiple neural network-based bounds.
 
         Parameters
         ----------
         points : numpy.ndarray with shape (m, n)
             A 2-D array where each row represents a point.
         log_l : numpy.ndarray of length m
@@ -231,62 +229,62 @@
             `split_threshold` times the target volume, the multi-ellipsiodal
             bound is split further, if possible. Default is 100.
         n_networks : int, optional
             Number of networks used in the emulator. Default is 4.
         neural_network_kwargs : dict, optional
             Non-default keyword arguments passed to the constructor of
             MLPRegressor.
-        n_jobs : int or string, optional
-            Number of parallel jobs to use for training. If the string 'max' is
-            passed, all available cores are used.
-        random_state : None or numpy.random.RandomState instance, optional
+        pool : multiprocessing.Pool, optional
+            Pool used for parallel processing.
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : NautilusBound
             The bound.
 
         """
         bound = cls()
+        bound.n_dim = points.shape[1]
 
         bound.neural_bounds = []
 
         multi_ellipsoid = Union.compute(
-            points[log_l > log_l_min], enlarge_per_dim=enlarge_per_dim,
+            points[log_l >= log_l_min], enlarge_per_dim=enlarge_per_dim,
             n_points_min=n_points_min, bound_class=Ellipsoid,
-            random_state=random_state)
+            rng=rng)
 
         while multi_ellipsoid.split_bound(allow_overlap=False):
             pass
 
         for ellipsoid in multi_ellipsoid.bounds:
             select = ellipsoid.contains(points)
             bound.neural_bounds.append(NeuralBound.compute(
                 points[select], log_l[select], log_l_min,
                 enlarge_per_dim=enlarge_per_dim, n_networks=n_networks,
-                neural_network_kwargs=neural_network_kwargs, n_jobs=n_jobs,
-                random_state=random_state))
+                neural_network_kwargs=neural_network_kwargs, pool=pool,
+                rng=rng))
 
         bound.outer_bound = Union.compute(
             points[log_l > log_l_min], enlarge_per_dim=enlarge_per_dim,
             n_points_min=n_points_min, bound_class=UnitCubeEllipsoidMixture,
-            random_state=random_state)
+            rng=rng)
 
         while bound.outer_bound.volume() - log_v_target > np.log(
                 split_threshold * enlarge_per_dim**points.shape[1]):
             if not bound.outer_bound.split_bound():
                 break
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
-        bound.points_sample = np.zeros((0, points.shape[1]))
+        bound.points = np.zeros((0, points.shape[1]))
         bound.n_sample = 0
         bound.n_reject = 0
 
         return bound
 
     def contains(self, points):
         """Check whether points are contained in the bound.
@@ -307,71 +305,114 @@
         in_bound = self.outer_bound.contains(points)
         if len(self.neural_bounds) > 0:
             in_bound = in_bound & np.any(
                 [bound.contains(points) for bound in self.neural_bounds],
                 axis=0)
         return in_bound
 
-    def sample(self, n_points=100):
+    @threadpool_limits.wrap(limits=1)
+    def _reset_and_sample(self, n_points=100, rng=None):
+        """Reset the bound, sample points internally and return the result.
+
+        Parameters
+        ----------
+        n_points : int, optional
+            How many points to draw. Default is 100.
+        rng : None or numpy.random.Generator, optional
+            Determines random number generation. If None, random number
+            generation is not reset. Default is None.
+
+        Returns
+        -------
+        bound : NautilusBound
+            The bound.
+
+        """
+        self.reset(rng=rng)
+        self.sample(n_points=n_points, return_points=False)
+        return self
+
+    def sample(self, n_points=100, return_points=True, pool=None):
         """Sample points from the the bound.
 
         Parameters
         ----------
         n_points : int, optional
-            How many points to draw.
+            How many points to draw. Default is 100.
+        return_points : bool, optional
+            If True, return sampled points. Otherwise, sample internally until
+            at least `n_points` are saved.
+        pool : multiprocessing.Pool, optional
+            Pool used for parallel processing.
 
         Returns
         -------
         points : numpy.ndarray
-            If `n_points` is larger than 1, two-dimensional array of shape
-            (n_points, n_dim). Otherwise, a one-dimensional array of shape
-            (n_dim).
-
-        """
-        while len(self.points_sample) < n_points:
-            n_sample = 10000
-            points = self.outer_bound.sample(n_sample)
-            in_bound = np.any([bound.contains(points) for bound in
-                               self.neural_bounds], axis=0)
-            points = points[in_bound]
-            self.points_sample = np.vstack([self.points_sample, points])
-            self.n_sample += n_sample
-            self.n_reject += n_sample - len(points)
-
-        points = self.points_sample[:n_points]
-        self.points_sample = self.points_sample[n_points:]
-        return np.squeeze(points)
+            Points as two-dimensional array of shape (n_points, n_dim).
+
+        """
+        if len(self.points) < n_points:
+            if pool is None:
+                while len(self.points) < n_points:
+                    n_sample = 1000
+                    points = self.outer_bound.sample(n_sample)
+                    in_bound = np.any([bound.contains(points) for bound in
+                                       self.neural_bounds], axis=0)
+                    points = points[in_bound]
+                    self.points = np.vstack([self.points, points])
+                    self.n_sample += n_sample
+                    self.n_reject += n_sample - len(points)
+            else:
+                n_jobs = pool._processes
+                n_points_per_job = (
+                    (max(n_points - len(self.points), 10000)) // n_jobs) + 1
+                func = partial(self._reset_and_sample, n_points_per_job)
+                rngs = [np.random.default_rng(seed) for seed in
+                        np.random.SeedSequence(self.rng.integers(
+                            2**32 - 1)).spawn(n_jobs)]
+                bounds = pool.map(func, rngs)
+                for bound in bounds:
+                    self.points = np.vstack([self.points, bound.points])
+                    self.n_sample += bound.n_sample
+                    self.n_reject += bound.n_reject
+                    self.outer_bound.n_sample += bound.outer_bound.n_sample
+                    self.outer_bound.n_reject += bound.outer_bound.n_reject
+
+        if return_points:
+            points = self.points[:n_points]
+            self.points = self.points[n_points:]
+            return points
 
     def volume(self):
         """Return the natural log of the volume.
 
         Returns
         -------
         log_v : float
             An estimate of the natural log of the volume. Will become more
             accurate as more points are sampled.
 
         """
         if self.n_sample == 0:
-            self.sample()
+            self.sample(return_points=False)
 
         return self.outer_bound.volume() + np.log(
             1.0 - self.n_reject / self.n_sample)
 
     def number_of_networks_and_ellipsoids(self):
         """Return the number of neural networks and sample ellipsoids.
 
         Returns
         -------
         n_networks : int
             The number of neural networks.
         n_ellipsoids : int
             The number of sample ellipsoids.
         """
-        if self.neural_bounds[0].emulator.neural_networks is not None:
+        if self.neural_bounds[0].emulator is not None:
             n_networks = len(self.neural_bounds) * len(
                 self.neural_bounds[0].emulator.neural_networks)
         else:
             n_networks = 0
 
         n_ellipsoids = 0
         for bound in self.outer_bound.bounds:
@@ -385,58 +426,78 @@
         Parameters
         ----------
         group : h5py.Group
             HDF5 group to write to.
 
         """
         group.attrs['type'] = 'NautilusBound'
+        group.attrs['n_dim'] = self.n_dim
         group.attrs['n_neural_bounds'] = len(self.neural_bounds)
 
         for i, neural_bound in enumerate(self.neural_bounds):
             neural_bound.write(group.create_group('neural_bound_{}'.format(i)))
 
         self.outer_bound.write(group.create_group('outer_bound'))
 
-        group.create_dataset('points_sample', data=self.points_sample)
+        group.create_dataset('points', data=self.points)
         group.attrs['n_sample'] = self.n_sample
         group.attrs['n_reject'] = self.n_reject
 
     @classmethod
-    def read(cls, group, random_state=None):
+    def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
         group : h5py.Group
             HDF5 group to write to.
-        random_state : None or numpy.random.RandomState instance, optional
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : NautilusBound
             The bound.
 
         """
         bound = cls()
 
-        if random_state is None:
-            bound.random_state = np.random
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
+
+        bound.n_dim = group.attrs['n_dim']
 
         bound.neural_bounds = []
         i = 0
         while 'neural_bound_{}'.format(i) in group:
             bound.neural_bounds.append(NeuralBound.read(
                 group['neural_bound_{}'.format(i)],
-                random_state=bound.random_state))
+                rng=bound.rng))
             i += 1
 
         bound.outer_bound = Union.read(
-            group['outer_bound'], random_state=random_state)
+            group['outer_bound'], rng=rng)
 
-        bound.points_sample = np.array(group['points_sample'])
+        bound.points = np.array(group['points'])
         bound.n_sample = group.attrs['n_sample']
         bound.n_reject = group.attrs['n_reject']
 
         return bound
+
+    def reset(self, rng=None):
+        """Reset random number generation and any progress, if applicable.
+
+        Parameters
+        ----------
+        rng : None or numpy.random.Generator, optional
+            Determines random number generation. If None, random number
+            generation is not reset. Default is None.
+
+        """
+        self.points = np.zeros((0, self.n_dim))
+        self.n_sample = 0
+        self.n_reject = 0
+        self.outer_bound.reset(rng)
+        if rng is not None:
+            self.rng = rng
```

### Comparing `nautilus-sampler-0.5.0/nautilus/bounds/union.py` & `nautilus-sampler-0.6.0/nautilus/bounds/union.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module implementing unions of basic bounds."""
 
 import itertools
 import numpy as np
 from scipy.special import logsumexp
 from scipy.optimize import minimize
-from sklearn.cluster import KMeans
-from threadpoolctl import threadpool_limits
+from sklearn.mixture import GaussianMixture
 
 from .basic import UnitCube, Ellipsoid, UnitCubeEllipsoidMixture
 
 
 def ellipsoids_overlap(ellipsoids):
     """Determine if ellipsoids overlap.
 
@@ -49,33 +48,38 @@
     enlarge_per_dim : float
         Along each dimension, ellipsoids enlarged by this factor.
     n_points_min : int or None
         The minimum number of points each ellipsoid should have. Effectively,
         ellipsoids with less than twice that number will not be split further.
     cube : UnitCube or None
         If not None, the bound is defined as the overlap with the unit cube.
+    points_bounds : list
+        The points used to create the individual bounds. Used to split bounds
+        further.
     bounds : list
         List of individual bounds.
-    log_v : list
+    log_v : numpy.ndarray
         Natural log of the volume of each individual bound.
-    points : list
-        The points used to create the union. Used to add more bounds.
-    points_sample : numpy.ndarray
+    block : numpy.ndarray
+        List indicating whether a bound should not be split further because
+        the volume would not decrease or the number of points is too low.
+    points : numpy.ndarray
         Points that a call to `sample` will return next.
     n_sample : int
         Number of points sampled from all bounds.
     n_reject : int
         Number of points rejected due to overlap.
-    random_state : numpy.random.RandomState instance
+    rng : numpy.random.Generator
         Determines random number generation.
+
     """
 
     @classmethod
     def compute(cls, points, enlarge_per_dim=1.1, n_points_min=None,
-                unit=True, bound_class=Ellipsoid, random_state=None):
+                unit=True, bound_class=Ellipsoid, rng=None):
         """Compute the bound.
 
         Upon creation, the bound consists of a single individual bound.
 
         Parameters
         ----------
         points : numpy.ndarray with shape (n_points, n_dim)
@@ -89,15 +93,15 @@
             be split further. If None, uses `n_points_min = n_dim + 1`. Default
             is None.
         unit : bool, optional
             If the bound is restricted to the overlap with the unit cube.
         bound_class : class, optional
             Type of the individual bounds, i.e. ellipsoids or unit
             cube-ellipsoid mixtures.
-        random_state : None or numpy.random.RandomState instance, optional
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Raises
         ------
         ValueError
             If `n_points_min` is smaller than the number of dimensions plus
             one.
@@ -120,30 +124,31 @@
                                  'larger than the number of dimensions.')
             bound.n_points_min = n_points_min
 
         if not unit:
             bound.cube = None
         else:
             bound.cube = UnitCube.compute(
-                bound.n_dim, random_state=random_state)
+                bound.n_dim, rng=rng)
 
-        bound.points = [points]
+        bound.points_bounds = [points]
         bound.bounds = [bound_class.compute(
             points, enlarge_per_dim=enlarge_per_dim,
-            random_state=random_state)]
+            rng=rng)]
         bound.log_v = np.array([bound.bounds[0].volume()])
+        bound.block = np.atleast_1d(len(points) < 2 * bound.n_points_min)
 
-        bound.points_sample = np.zeros((0, points.shape[1]))
+        bound.points = np.zeros((0, points.shape[1]))
         bound.n_sample = 0
         bound.n_reject = 0
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
         return bound
 
     def split_bound(self, allow_overlap=True):
         """Split the largest bound in the union.
 
         Parameters
@@ -165,58 +170,58 @@
             Whether it was possible to split any ellipsoid.
 
         """
         if not allow_overlap and not isinstance(self.bounds[0], Ellipsoid):
             raise ValueError("'allow_overlap' can only be False if " +
                              "bounds are ellipsoids.")
 
-        split_possible = (np.array([len(points) for points in self.points]) >=
-                          2 * self.n_points_min)
-
-        if not np.any(split_possible):
+        if not np.any(~self.block):
             return False
 
-        index = np.argmax(np.where(split_possible, self.log_v, -np.inf))
-        points = self.bounds[index].transform(self.points[index])
+        index = np.argmax(np.where(~self.block, self.log_v, -np.inf))
+        points = self.bounds[index].transform(self.points_bounds[index])
 
-        if self.random_state != np.random:
-            random_state = self.random_state
-        else:
-            random_state = None
-        with threadpool_limits(limits=1):
-            d = KMeans(n_clusters=2, n_init=10, random_state=random_state
-                       ).fit_transform(points)
+        # print('mixture...')
+        labels = GaussianMixture(
+            n_components=2, n_init=10, random_state=self.rng.integers(
+                2**32 - 1)).fit_predict(points)
 
-        labels = np.argmin(d, axis=1)
         if not np.all(np.bincount(labels) >= self.n_points_min):
-            label = np.argmin(np.bincount(labels))
-            labels[np.argsort(d[:, label] - d[:, label - 1])[
-                :self.n_points_min]] = label
-
-        new_bounds = self.bounds.copy()
-        new_bounds.pop(index)
-        points = self.points[index]
+            self.block[index] = True
+            return self.split_bound(allow_overlap=allow_overlap)
+
+        new_bounds = []
+        points = self.points_bounds[index]
         for label in [0, 1]:
             new_bounds.append(type(self.bounds[0]).compute(
                 points[labels == label], enlarge_per_dim=self.enlarge_per_dim,
-                random_state=self.random_state))
+                rng=self.rng))
 
-        if not allow_overlap and ellipsoids_overlap(new_bounds):
+        if not allow_overlap and ellipsoids_overlap(
+                self.bounds[:index] + self.bounds[index+1:] + new_bounds):
             return False
 
-        self.bounds = new_bounds
+        if (logsumexp([new_bounds[0].volume(), new_bounds[1].volume()]) >
+                self.bounds[index].volume()):
+            self.block[index] = True
+            return self.split_bound(allow_overlap=allow_overlap)
+
+        self.points_bounds.pop(index)
+        self.points_bounds.append(points[labels == 0])
+        self.points_bounds.append(points[labels == 1])
+        self.bounds.pop(index)
+        self.bounds = self.bounds + new_bounds
         self.log_v = np.array([bound.volume() for bound in self.bounds])
-        self.points.pop(index)
-        self.points.append(points[labels == 0])
-        self.points.append(points[labels == 1])
+        self.block = np.concatenate(
+            (np.delete(self.block, index),
+             [len(self.points_bounds[-2]) < 2 * self.n_points_min,
+              len(self.points_bounds[-1]) < 2 * self.n_points_min]))
 
         # Reset the sampling.
-        self.points_sample = np.zeros((0, points.shape[1]))
-        self.n_sample = 0
-        self.n_reject = 0
+        self.reset()
 
         return True
 
     def contains(self, points):
         """Check whether points are contained in the bound.
 
         Parameters
@@ -240,44 +245,44 @@
 
     def sample(self, n_points=100):
         """Sample points from the bound.
 
         Parameters
         ----------
         n_points : int, optional
-            How many points to draw.
+            How many points to draw. Default is 100.
 
         Returns
         -------
         points : numpy.ndarray
             Points as two-dimensional array of shape (n_points, n_dim).
 
         """
-        while len(self.points_sample) < n_points:
-            n_sample = 10000
+        while len(self.points) < n_points:
+            n_sample = 1000
 
             p = np.exp(np.array(self.log_v) - logsumexp(self.log_v))
-            n_per_bound = self.random_state.multinomial(n_sample, p)
+            n_per_bound = self.rng.multinomial(n_sample, p)
 
             points = np.vstack([bound.sample(n) for bound, n in
                                 zip(self.bounds, n_per_bound)])
             if self.cube is not None:
                 points = points[self.cube.contains(points)]
-            self.random_state.shuffle(points)
+            self.rng.shuffle(points)
             n_bound = np.sum([bound.contains(points) for bound in self.bounds],
                              axis=0)
             p = 1 - 1.0 / n_bound
-            points = points[self.random_state.random(size=len(points)) > p]
-            self.points_sample = np.vstack([self.points_sample, points])
+            points = points[self.rng.random(size=len(points)) > p]
+            self.points = np.vstack([self.points, points])
 
             self.n_sample += n_sample
             self.n_reject += n_sample - len(points)
 
-        points = self.points_sample[:n_points]
-        self.points_sample = self.points_sample[n_points:]
+        points = self.points[:n_points]
+        self.points = self.points[n_points:]
         return points
 
     def volume(self):
         """Return the natural log of the volume of the bound.
 
         Returns
         -------
@@ -309,56 +314,77 @@
         if self.cube is not None:
             self.cube.write(group.create_group('cube'))
 
         group.attrs['bound_class'] = self.bounds[0].__class__.__name__
         for i, bound in enumerate(self.bounds):
             bound.write(group.create_group('bound_{}'.format(i)))
 
-        for i in range(len(self.points)):
-            group.create_dataset('points_{}'.format(i), data=self.points[i])
-        group.create_dataset('points_sample', data=self.points_sample)
+        for i, points in enumerate(self.points_bounds):
+            group.create_dataset('points_bound_{}'.format(i), data=points)
+        group.create_dataset('points', data=self.points)
 
     @classmethod
-    def read(cls, group, random_state=None):
+    def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
         group : h5py.Group
             HDF5 group to write to.
-        random_state : None or numpy.random.RandomState instance, optional
+        rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
         Returns
         -------
         bound : MultiEllipsoid
             The bound.
 
         """
         bound = cls()
 
-        if random_state is None:
-            bound.random_state = np.random.RandomState()
+        if rng is None:
+            bound.rng = np.random.default_rng()
         else:
-            bound.random_state = random_state
+            bound.rng = rng
 
         for key in ['n_dim', 'log_v', 'enlarge_per_dim', 'n_points_min',
                     'n_sample', 'n_reject']:
             setattr(bound, key, group.attrs[key])
 
         if group.attrs['unit']:
             bound.cube = UnitCube.read(
-                group['cube'], random_state=bound.random_state)
+                group['cube'], rng=bound.rng)
 
         if group.attrs['bound_class'] == 'Ellipsoid':
             bound_class = Ellipsoid
         else:
             bound_class = UnitCubeEllipsoidMixture
 
         bound.bounds = [bound_class.read(
-            group['bound_{}'.format(i)], random_state=bound.random_state)
+            group['bound_{}'.format(i)], rng=bound.rng)
             for i in range(len(bound.log_v))]
-        bound.points = [np.array(group['points_{}'.format(i)]) for i in
-                        range(len(bound.log_v))]
-        bound.points_sample = np.array(group['points_sample'])
+        bound.points_bounds = [np.array(group['points_bound_{}'.format(i)]) for
+                               i in range(len(bound.log_v))]
+        bound.points = np.array(group['points'])
 
         return bound
+
+    def reset(self, rng=None):
+        """Reset random number generation and any progress, if applicable.
+
+        Parameters
+        ----------
+        rng : None or numpy.random.Generator, optional
+            Determines random number generation. If None, random number
+            generation is not reset. Default is None.
+
+        """
+        self.points = np.zeros((0, self.n_dim))
+        self.n_sample = 0
+        self.n_reject = 0
+
+        if rng is not None:
+            self.rng = rng
+            if self.cube is not None:
+                self.cube.reset(rng)
+            for bound in self.bounds:
+                bound.reset(rng)
```

### Comparing `nautilus-sampler-0.5.0/nautilus/neural.py` & `nautilus-sampler-0.6.0/nautilus/neural.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Module implementing neural network emulators."""
 
 import numpy as np
 import warnings
 from functools import partial
-from multiprocessing import cpu_count, Pool
-from threadpoolctl import threadpool_limits
 from sklearn.neural_network import MLPRegressor
+from threadpoolctl import threadpool_limits
 
 
+@threadpool_limits.wrap(limits=1)
 def train_network(x, y, neural_network_kwargs, random_state):
     """Train a network.
 
     Parameters
     ----------
     x : numpy.ndarray
         Input coordinates.
@@ -44,63 +44,61 @@
         coordinates.
     network : sklearn.neural_network.MLPRegressor
         Artifical neural network used for emulation.
 
     """
 
     @classmethod
-    def train(cls, x, y, n_networks=4, neural_network_kwargs={}, n_jobs='max'):
+    def train(cls, x, y, n_networks=4, neural_network_kwargs={}, pool=None):
         """Initialize and train the likelihood neural network emulator.
 
         Parameters
         ----------
         x : numpy.ndarray
             Input coordinates.
         y : numpy.ndarray
             Target values.
         n_networks : int, optional
             Number of networks used in the emulator. Default is 4.
         neural_network_kwargs : dict, optional
             Non-default keyword arguments passed to the constructor of
             MLPRegressor.
-        n_jobs : int or string, optional
-            Number of parallel jobs to use for training. If the string 'max' is
-            passed, all available cores are used.
+        pool : multiprocessing.Pool, optional
+            Pool used for parallel processing.
 
         Returns
         -------
         emulator : NeuralNetworkEmulator
             The likelihood neural network emulator.
 
         """
         emulator = cls()
 
         emulator.mean = np.mean(x, axis=0)
         emulator.scale = np.std(x, axis=0)
 
-        if n_jobs == 'max':
-            n_jobs = cpu_count()
-
         default_neural_network_kwargs = dict(
             hidden_layer_sizes=(100, 50, 20), alpha=0, learning_rate_init=1e-2,
             max_iter=10000, tol=0, n_iter_no_change=10,
             validation_fraction=0.1)
         default_neural_network_kwargs.update(neural_network_kwargs)
         neural_network_kwargs = default_neural_network_kwargs
 
         if 'random_state' in neural_network_kwargs:
             warnings.warn("The 'random_state' keyword argument passed to the" +
                           " neural network is ignored.", Warning, stacklevel=2)
             del neural_network_kwargs['random_state']
 
-        with threadpool_limits(limits=1):
-            with Pool(n_jobs) as pool:
-                emulator.neural_networks = pool.map(partial(
-                    train_network, (x - emulator.mean) / emulator.scale, y,
-                    neural_network_kwargs), range(n_networks))
+        f = partial(train_network, (x - emulator.mean) / emulator.scale, y,
+                    neural_network_kwargs)
+
+        if pool is None:
+            emulator.neural_networks = list(map(f, range(n_networks)))
+        else:
+            emulator.neural_networks = pool.map(f, range(n_networks))
 
         return emulator
 
     def predict(self, x):
         """Calculate the emulator likelihood prediction for a group of points.
 
         Parameters
@@ -110,18 +108,17 @@
 
         Returns
         -------
         y_emu : numpy.ndarray
             Emulated normalized likelihood value of the training points.
 
         """
-        with threadpool_limits(limits=1):
-            return np.mean(
-                [network.predict((x - self.mean) / self.scale) for network in
-                 self.neural_networks], axis=0)
+        return np.mean(
+            [network.predict((x - self.mean) / self.scale) for network in
+             self.neural_networks], axis=0)
 
     def write(self, group):
         """Write the emulator to an HDF5 group.
 
         Parameters
         ----------
         group : h5py.Group
```

### Comparing `nautilus-sampler-0.5.0/nautilus/prior.py` & `nautilus-sampler-0.6.0/nautilus/prior.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/nautilus/sampler.py` & `nautilus-sampler-0.6.0/nautilus/sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Module implementing the Nautilus sampler."""
 
 try:
     import h5py
 except ImportError:
     pass
 import numpy as np
+import warnings
 
 from functools import partial
-from multiprocessing import Pool
+from multiprocessing import Pool, cpu_count
 from pathlib import Path
 from scipy.special import logsumexp
+from threadpoolctl import threadpool_limits
 from tqdm import tqdm
-import warnings
 
 from .bounds import UnitCube, NautilusBound
 
 
 class Sampler():
     """
     A dynamic sampler built upon the framework of importance nested sampling.
@@ -32,33 +33,45 @@
     n_live : int
         Number of live points.
     n_update : int
         The maximum number of additions to the live set before a new bound is
         created.
     n_like_new_bound : int
         The maximum number of likelihood calls before a new bounds is created.
-    enlarge : float
-        Factor by which the volume of ellipsoidal bounds is increased.
+    enlarge_per_dim : float
+        Along each dimension, outer ellipsoidal bounds are enlarged by this
+        factor.
+    n_points_min : int or None, optional
+        The minimum number of points each ellipsoid should have. Effectively,
+        ellipsoids with less than twice that number will not be split further.
+    split_threshold: float, optional
+        Threshold used for splitting the multi-ellipsoidal bound used for
+        sampling. If the volume of the bound prior enlarging is larger than
+        `split_threshold` times the target volume, the multi-ellipsiodal
+        bound is split further, if possible.
+    n_networks : int
+        Number of networks used in the estimator.
     neural_network_kwargs : dict
         Keyword arguments passed to the constructor of
         `sklearn.neural_network.MLPRegressor`.
     n_batch : int
         Number of likelihood evaluations that are performed at each step.
     vectorized : bool
         If True, the likelihood function can receive multiple input sets at
         once.
     pass_dict : bool
         If True, the likelihood function expects model parameters as
         dictionaries.
-    neural_network_thread_limit : int or None
-        Maximum number of threads used by `sklearn`.
     pool : object
         Pool used to parallelize likelihood calls.
-    random_state : np.random.RandomState
-        Random state of the sampler used for random number generation.
+    n_jobs : int or string
+        Number of parallel jobs to use for neural network training and sampling
+        new points.
+    rng : np.random.Generator
+        Random number generator of the sampler.
     n_like : int
         Total number of likelihood evaluations.
     explored : bool, optional
         Whether the space has been explored and the shells have been
         constructed.
     bounds : list
         List of all the constructed bounds.
@@ -87,21 +100,22 @@
     shell_log_v : numpy.ndarray
         Logarithm of the volume of each bound/shell.
 
     """
 
     def __init__(self, prior, likelihood, n_dim=None, n_live=2000,
                  n_update=None, enlarge=None, enlarge_per_dim=1.1,
+                 n_points_min=None, split_threshold=100,
                  n_networks=4, neural_network_kwargs=dict(), prior_args=[],
                  prior_kwargs=dict(), likelihood_args=[],
                  likelihood_kwargs=dict(), n_batch=100,
                  use_neural_networks=None, n_like_new_bound=None,
-                 vectorized=False, pass_dict=None, pool=None, n_jobs='max',
-                 random_state=None, blobs_dtype=None, filepath=None,
-                 resume=True):
+                 vectorized=False, pass_dict=None, pool=None, n_jobs=1,
+                 random_state=None, seed=None,
+                 blobs_dtype=None, filepath=None, resume=True):
         r"""
         Initialize the sampler.
 
         Parameters
         ----------
         prior : function or nautilus.Prior
             Prior describing the mapping of the unit hypercube to the
@@ -119,14 +133,24 @@
             The maximum number of additions to the live set before a new bound
             is created. If None, use `n_live`. Default is None.
         enlarge : float, optional
             Deprecated.
         enlarge_per_dim : float, optional
             Along each dimension, outer ellipsoidal bounds are enlarged by this
             factor. Default is 1.1.
+        n_points_min : int or None, optional
+            The minimum number of points each ellipsoid should have.
+            Effectively, ellipsoids with less than twice that number will not
+            be split further. If None, uses `n_points_min = n_dim + 50`.
+            Default is None.
+        split_threshold: float, optional
+            Threshold used for splitting the multi-ellipsoidal bound used for
+            sampling. If the volume of the bound prior enlarging is larger than
+            `split_threshold` times the target volume, the multi-ellipsiodal
+            bound is split further, if possible. Default is 100.
         n_networks : int, optional
             Number of networks used in the estimator. Default is 4.
         neural_network_kwargs : dict, optional
             Non-default keyword arguments passed to the constructor of
             MLPRegressor.
         prior_args : list, optional
             List of extra positional arguments for `prior`. Only used if
@@ -156,30 +180,31 @@
             it should be able to take an array with shape (n_points, n_dim)
             and return an array with shape (n_points). Similarly, if the
             likelihood function accepts dictionaries, it should be able to
             process dictionaries where each value is an array with shape
             (n_points). Default is False.
         pass_dict : bool or None, optional
             If True, the likelihood function expects model parameters as
-            dictionaries. If false, it expects regular numpy arrays. Default is
+            dictionaries. If False, it expects regular numpy arrays. Default is
             to set it to True if prior was a nautilus.Prior instance and False
             otherwise.
         pool : object or int, optional
             Object with a `map` function used for parallelization of likelihood
             calls, e.g. a multiprocessing.Pool object, or a positive integer.
             If it is an integer, it determines the number of workers in the
             Pool. Default is None.
         n_jobs : int or string, optional
-            Number of parallel jobs to use for neural network training. If the
-            string 'max' is passed, all available cores are used.
-        neural_network_thread_limit : int or None, optional
-            Deprecated.
+            Number of parallel jobs to use for neural network training and
+            sampling new points. If the string 'max' is passed, all available
+            cores are used. Default is 'max'.
         random_state : int or np.random.RandomState, optional
-            Determines random number generation. Pass an int for reproducible
-            results accross different runs. Default is None.
+            Deprecated.
+        seed : int, optional
+            Seed for random number generation used for reproducible results
+            accross different runs. Default is None.
         blobs_dtype : object or None, optional
             Object that can be converted to a data type object describing the
             blobs. If None, this will be inferred from the first blob. Default
             is None.
         filepath : string, pathlib.Path or None, optional
             Path to the file where results are saved. Must have a '.h5' or
             '.hdf5' extension. If None, no results are written. Default is
@@ -189,16 +214,16 @@
             start from scratch and overwrite any previous file. Default is
             True.
 
         Raises
         ------
         ValueError
             If `prior` is a function and `n_dim` is not given or `pass_struct`
-            is set to True. Also, if the dimensionality of the problem is less
-            than 2.
+            is set to True. If the dimensionality of the problem is less than
+            2.
 
         """
         if callable(prior):
             self.prior = partial(prior, *prior_args, **prior_kwargs)
         else:
             self.prior = prior
         self.likelihood = partial(
@@ -219,30 +244,34 @@
         if self.n_dim <= 1:
             raise ValueError(
                 'Cannot run Nautilus with less than 2 parameters.')
 
         self.n_live = n_live
 
         if n_update is None:
-            self.n_update = n_live
-        else:
-            self.n_update = n_update
+            n_update = n_live
+        self.n_update = n_update
 
         if n_like_new_bound is None:
-            self.n_like_new_bound = 10 * n_live
-        else:
-            self.n_like_new_bound = n_like_new_bound
+            n_like_new_bound = 10 * n_live
+        self.n_like_new_bound = n_like_new_bound
 
         if enlarge is not None:
             warnings.warn("The 'enlarge' keyword argument has been " +
                           "deprecated. Use 'enlarge_per_dim', instead.",
                           DeprecationWarning, stacklevel=2)
 
         self.enlarge_per_dim = enlarge_per_dim
 
+        if n_points_min is None:
+            n_points_min = self.n_dim + 50
+        self.n_points_min = n_points_min
+
+        self.split_threshold = split_threshold
+
         if use_neural_networks is not None:
             warnings.warn("The 'use_neural_networks' keyword argument has " +
                           "been deprecated. Set 'n_networks', instead.",
                           DeprecationWarning, stacklevel=2)
 
         self.n_networks = n_networks
 
@@ -254,22 +283,24 @@
         if isinstance(pool, int):
             self.pool = Pool(pool)
         elif pool is not None:
             self.pool = pool
         else:
             self.pool = None
 
+        if n_jobs == 'max':
+            n_jobs = cpu_count()
         self.n_jobs = n_jobs
 
-        if random_state is None:
-            self.random_state = np.random.RandomState()
-        elif isinstance(random_state, int):
-            self.random_state = np.random.RandomState(random_state)
-        else:
-            self.random_state = random_state
+        if random_state is not None:
+            warnings.warn("The 'random_state' keyword argument has been " +
+                          "deprecated. Use 'seed' instead.",
+                          DeprecationWarning, stacklevel=2)
+
+        self.rng = np.random.default_rng(seed)
 
         # The following variables carry the information about the run.
         self.n_like = 0
         self.explored = False
         self.bounds = []
         self.points = []
         self.log_l = []
@@ -282,18 +313,24 @@
         self.shell_log_l_min = np.zeros(0, dtype=float)
         self.shell_log_l = np.zeros(0, dtype=float)
         self.shell_log_v = np.zeros(0, dtype=float)
 
         self.filepath = filepath
         if resume and filepath is not None and Path(filepath).exists():
             with h5py.File(filepath, 'r') as fstream:
+
                 group = fstream['sampler']
-                self.random_state.set_state(
-                    tuple(group.attrs['random_state_{}'.format(i)] for i in
-                          range(5)))
+
+                self.rng.bit_generator.state = dict(
+                    bit_generator='PCG64',
+                    state=dict(
+                        state=int(group.attrs['rng_state']),
+                        inc=int(group.attrs['rng_inc'])),
+                    has_uint32=group.attrs['rng_has_uint32'],
+                    uinteger=group.attrs['rng_uinteger'])
 
                 for key in ['n_like', 'explored', 'shell_n',
                             'shell_n_sample_shell', 'shell_n_sample_bound',
                             'shell_n_eff', 'shell_log_l_min', 'shell_log_l',
                             'shell_log_v']:
                     setattr(self, key, group.attrs[key])
 
@@ -305,20 +342,19 @@
                     try:
                         self.blobs.append(
                             np.array(group['blobs_{}'.format(shell)]))
                         self.blobs_dtype = self.blobs[-1].dtype
                     except KeyError:
                         pass
 
-                self.bounds = [UnitCube.read(fstream['bound_0'],
-                                             random_state=self.random_state), ]
+                self.bounds = [
+                    UnitCube.read(fstream['bound_0'], rng=self.rng), ]
                 for i in range(1, len(self.shell_n)):
                     self.bounds.append(NautilusBound.read(
-                        fstream['bound_{}'.format(i)],
-                        random_state=self.random_state))
+                        fstream['bound_{}'.format(i)], rng=self.rng))
 
     def run(self, f_live=0.01, n_shell=None, n_eff=10000,
             discard_exploration=False, verbose=False):
         """Run the sampler until convergence.
 
         Parameters
         ----------
@@ -331,19 +367,21 @@
             the sampler which is 100 unless otherwise specified.
         n_eff : float, optional
             Minimum effective sample size. The algorithm will sample from the
             shells until this is reached. Default is 10000.
         discard_exploration : bool, optional
             Whether to discard points drawn in the exploration phase. This is
             required for a fully unbiased posterior and evidence estimate.
-            Default is True.
+            Default is False.
         verbose : bool, optional
             If True, print additional information. Default is False.
 
         """
+        self._pool = Pool(self.n_jobs) if self.n_jobs > 1 else None
+
         if not self.explored:
 
             if verbose:
                 print('#########################')
                 print('### Exploration Phase ###')
                 print('#########################')
                 print()
@@ -396,14 +434,17 @@
                 print('#########################')
                 print('##### Sampling Phase ####')
                 print('#########################')
                 print()
 
             self.add_points(n_shell=n_shell, n_eff=n_eff, verbose=verbose)
 
+        if self.n_jobs > 1:
+            self._pool.close()
+
     def posterior(self, return_as_dict=None, equal_weight=False,
                   return_blobs=False):
         """Return the posterior sample estimate.
 
         Parameters
         ----------
         return_as_dict : bool or None, optional
@@ -465,15 +506,15 @@
 
         if not return_as_dict and callable(self.prior) and self.pass_dict:
             raise ValueError(
                 'Cannot return points as numpy array. The prior function' +
                 ' only returns dictionaries.')
 
         if equal_weight:
-            select = (self.random_state.random(len(log_w)) <
+            select = (self.rng.random(len(log_w)) <
                       np.exp(log_w - np.amax(log_w)))
             points = points[select]
             log_w = np.ones(len(points)) * np.log(1.0 / np.sum(select))
             log_l = log_l[select]
             if return_blobs:
                 blobs = blobs[select]
 
@@ -546,48 +587,49 @@
                              "from the last bound/shell.")
 
         n_bound = 0
         n_sample = 0
         idx_t = np.zeros(0, dtype=int)
         points_all = []
 
-        while n_sample < self.n_batch:
-            points = np.atleast_2d(self.bounds[index].sample(
-                self.n_batch - n_sample))
-            n_bound += self.n_batch - n_sample
-
-            # Remove points that are actually in another shell.
-            in_shell = np.ones(len(points), dtype=bool)
-            for bound in self.bounds[index:][1:]:
-                in_shell = in_shell & ~bound.contains(points)
-                if np.all(~in_shell):
-                    continue
-            points = points[in_shell]
-
-            # Replace points for which we can use transfer points.
-            replace = np.zeros(len(points), dtype=bool)
-            if shell_t is not None and len(shell_t) > 0:
-                shell_p = self.shell_association(
-                    points, n_max=len(self.bounds) - 1)
-                for shell in range(len(self.bounds) - 1):
-                    idx_1 = np.flatnonzero(shell_t == shell)
-                    idx_2 = np.flatnonzero(shell_p == shell)
-                    n = min(len(idx_1), len(idx_2))
-                    if n > 0:
-                        idx_t = np.append(idx_t, self.random_state.choice(
-                            idx_1, size=n, replace=False))
-                        shell_t[idx_t] = -1
-                        replace[self.random_state.choice(
-                            idx_2, size=n, replace=False)] = True
-
-            points = points[~replace]
-
-            if len(points) > 0:
-                points_all.append(points)
-                n_sample += len(points)
+        with threadpool_limits(limits=1):
+            while n_sample < self.n_batch:
+                points = self.bounds[index].sample(
+                    self.n_batch - n_sample, pool=self._pool)
+                n_bound += self.n_batch - n_sample
+
+                # Remove points that are actually in another shell.
+                in_shell = np.ones(len(points), dtype=bool)
+                for bound in self.bounds[index:][1:]:
+                    in_shell = in_shell & ~bound.contains(points)
+                    if np.all(~in_shell):
+                        continue
+                points = points[in_shell]
+
+                # Replace points for which we can use transfer points.
+                replace = np.zeros(len(points), dtype=bool)
+                if shell_t is not None and len(shell_t) > 0:
+                    shell_p = self.shell_association(
+                        points, n_max=len(self.bounds) - 1)
+                    for shell in range(len(self.bounds) - 1):
+                        idx_1 = np.flatnonzero(shell_t == shell)
+                        idx_2 = np.flatnonzero(shell_p == shell)
+                        n = min(len(idx_1), len(idx_2))
+                        if n > 0:
+                            idx_t = np.append(idx_t, self.rng.choice(
+                                idx_1, size=n, replace=False))
+                            shell_t[idx_t] = -1
+                            replace[self.rng.choice(
+                                idx_2, size=n, replace=False)] = True
+
+                points = points[~replace]
+
+                if len(points) > 0:
+                    points_all.append(points)
+                    n_sample += len(points)
 
         points = np.concatenate(points_all)
 
         if shell_t is None:
             return points, n_bound
         else:
             return points, n_bound, idx_t
@@ -714,31 +756,34 @@
         self.shell_n_eff = np.append(self.shell_n_eff, 0)
         self.shell_log_l = np.append(self.shell_log_l, np.nan)
         self.shell_log_v = np.append(self.shell_log_v, np.nan)
 
         # If this is the first bound, use the UnitCube bound.
         if len(self.bounds) == 0:
             log_l_min = -np.inf
-            self.bounds.append(
-                UnitCube.compute(self.n_dim, random_state=self.random_state))
+            self.bounds.append(UnitCube.compute(self.n_dim, rng=self.rng))
         else:
             if verbose:
                 print('Adding bound {}'.format(len(self.bounds) + 1), end='\r')
             log_l = np.concatenate(self.log_l)
             points = np.concatenate(self.points)[np.argsort(log_l)]
             log_l = np.sort(log_l)
             log_l_min = 0.5 * (log_l[-self.n_live] + log_l[-self.n_live - 1])
-            bound = NautilusBound.compute(
-                points, log_l, log_l_min, self.live_volume(),
-                enlarge_per_dim=self.enlarge_per_dim,
-                n_networks=self.n_networks,
-                neural_network_kwargs=self.neural_network_kwargs,
-                n_jobs=self.n_jobs, random_state=self.random_state)
-            if bound.volume() > self.bounds[-1].volume():
-                bound = self.bounds[-1]
+            with threadpool_limits(limits=1):
+                bound = NautilusBound.compute(
+                    points, log_l, log_l_min, self.live_volume(),
+                    enlarge_per_dim=self.enlarge_per_dim,
+                    n_points_min=self.n_points_min,
+                    split_threshold=self.split_threshold,
+                    n_networks=self.n_networks,
+                    neural_network_kwargs=self.neural_network_kwargs,
+                    pool=self._pool, rng=self.rng)
+                bound.sample(1000, return_points=False, pool=self._pool)
+                if bound.volume() > self.bounds[-1].volume():
+                    bound = self.bounds[-1]
             self.bounds.append(bound)
 
         self.points.append([])
         self.log_l.append([])
         self.blobs.append([])
         self.shell_log_l_min = np.append(self.shell_log_l_min, log_l_min)
 
@@ -1077,28 +1122,25 @@
 
         filepath.parent.mkdir(parents=True, exist_ok=True)
 
         fstream = h5py.File(filepath, 'x')
         group = fstream.create_group('sampler')
 
         for key in ['n_dim', 'n_live', 'n_update', 'n_like_new_bound',
-                    'enlarge_per_dim', 'n_networks', 'n_batch', 'vectorized',
-                    'pass_dict', 'n_like', 'explored', 'shell_n',
-                    'shell_n_sample_shell', 'shell_n_sample_bound',
-                    'shell_n_eff', 'shell_log_l_min', 'shell_log_l',
-                    'shell_log_v']:
+                    'enlarge_per_dim', 'n_points_min', 'split_threshold',
+                    'n_networks', 'n_batch', 'vectorized', 'pass_dict',
+                    'n_like', 'explored', 'shell_n', 'shell_n_sample_shell',
+                    'shell_n_sample_bound', 'shell_n_eff', 'shell_log_l_min',
+                    'shell_log_l', 'shell_log_v']:
             group.attrs[key] = getattr(self, key)
 
         for key in self.neural_network_kwargs.keys():
             group.attrs['neural_network_{}'.format(key)] =\
                 self.neural_network_kwargs[key]
 
-        for i, var in enumerate(self.random_state.get_state()):
-            group.attrs['random_state_{}'.format(i)] = var
-
         for shell in range(len(self.bounds)):
             group.create_dataset(
                 'points_{}'.format(shell), data=self.points[shell],
                 maxshape=(None, self.n_dim))
             group.create_dataset(
                 'log_l_{}'.format(shell), data=self.log_l[shell],
                 maxshape=(None, ))
@@ -1108,14 +1150,20 @@
                 group.create_dataset(
                     'blobs_{}'.format(shell), data=self.blobs[shell],
                     maxshape=tuple(maxshape))
 
         for i, bound in enumerate(self.bounds):
             bound.write(fstream.create_group('bound_{}'.format(i)))
 
+        rng_state = self.rng.bit_generator.state
+        group.attrs['rng_state'] = str(rng_state['state']['state'])
+        group.attrs['rng_inc'] = str(rng_state['state']['inc'])
+        group.attrs['rng_has_uint32'] = rng_state['has_uint32']
+        group.attrs['rng_uinteger'] = rng_state['uinteger']
+
         fstream.close()
 
     def write_shell_update(self, filepath, shell):
         """Update the sampler data for a single shell.
 
         Parameters
         ----------
@@ -1152,8 +1200,14 @@
         group['points_{}'.format(shell)][...] = self.points[shell]
         group['log_l_{}'.format(shell)].resize(self.log_l[shell].shape)
         group['log_l_{}'.format(shell)][...] = self.log_l[shell]
         if self.blobs_dtype is not None:
             group['blobs_{}'.format(shell)].resize(self.blobs[shell].shape)
             group['blobs_{}'.format(shell)][...] = self.blobs[shell]
 
+        rng_state = self.rng.bit_generator.state
+        group.attrs['rng_state'] = str(rng_state['state']['state'])
+        group.attrs['rng_inc'] = str(rng_state['state']['inc'])
+        group.attrs['rng_has_uint32'] = rng_state['has_uint32']
+        group.attrs['rng_uinteger'] = rng_state['uinteger']
+
         fstream.close()
```

### Comparing `nautilus-sampler-0.5.0/pyproject.toml` & `nautilus-sampler-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/tests/test_blobs.py` & `nautilus-sampler-0.6.0/tests/test_blobs.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/tests/test_bounds.py` & `nautilus-sampler-0.6.0/tests/test_bounds.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pytest
 
+from multiprocessing import Pool
 from scipy.special import gamma
 
 from nautilus import bounds
 from nautilus.bounds.basic import minimum_volume_enclosing_ellipsoid
 from nautilus.bounds.basic import invert_symmetric_positive_semidefinite_matrix
 
 
@@ -52,24 +53,22 @@
     assert points.shape == (n_points, n_dim)
     assert np.all((points >= 0) & (points < 1))
     assert np.all(cube.contains(points))
 
     assert cube.volume() == 0
 
 
-def test_unit_cube_random_state():
-    # Test that passing a random state leads to reproducible results.
+def test_unit_cube_rng():
+    # Test that passing a random number generator leads to reproducible
+    # results.
 
     n_dim, n_points = 7, 1000
-    cube = bounds.UnitCube.compute(
-        n_dim, random_state=np.random.RandomState(0))
-    cube_same = bounds.UnitCube.compute(
-        n_dim, random_state=np.random.RandomState(0))
-    cube_diff = bounds.UnitCube.compute(
-        n_dim, random_state=np.random.RandomState(1))
+    cube = bounds.UnitCube.compute(n_dim, rng=np.random.default_rng(0))
+    cube_same = bounds.UnitCube.compute(n_dim, rng=np.random.default_rng(0))
+    cube_diff = bounds.UnitCube.compute(n_dim, rng=np.random.default_rng(1))
     points = cube.sample(n_points)
     assert np.all(points == cube_same.sample(n_points))
     assert not np.all(points == cube_diff.sample(n_points))
     # We've already sampled from the cube. New samples should be different.
     assert not np.all(points == cube.sample(n_points))
 
     points = np.random.random((n_points, n_dim))
@@ -118,25 +117,25 @@
 
 
 def test_ellipsoid_sample_and_contains(points_on_hypersphere_boundary):
     # Test that the ellipsoidal sampling and boundary work as expected.
 
     ell = bounds.Ellipsoid.compute(
         points_on_hypersphere_boundary, enlarge_per_dim=1.0,
-        random_state=np.random.RandomState(0))
+        rng=np.random.default_rng(0))
     c = np.mean(points_on_hypersphere_boundary)
 
     n_points = 100
     points = ell.sample(n_points)
     assert points.shape == (n_points, points_on_hypersphere_boundary.shape[1])
     assert np.all(np.linalg.norm(points - c, axis=1) < 1 + 1e-9)
     assert np.all(ell.contains(points))
 
     ell = bounds.Ellipsoid.compute(
-        points, enlarge_per_dim=1.1, random_state=np.random.RandomState(0))
+        points, enlarge_per_dim=1.1, rng=np.random.default_rng(0))
     points = ell.sample(n_points)
     assert not np.all(np.linalg.norm(points - c, axis=1) < 1)
     assert np.all(ell.contains(points))
 
 
 def test_ellipsoid_volume(points_on_hypersphere_boundary):
     # Test that the volume of the ellipsoid is accurate.
@@ -150,30 +149,31 @@
                                  gamma(n_dim / 2 + 1)))
 
 
 def test_ellipsoid_transform(random_points_from_hypersphere):
     # Test that the Cholesky decomposition works correctly.
 
     ell = bounds.Ellipsoid.compute(
-        random_points_from_hypersphere, random_state=np.random.RandomState(0))
+        random_points_from_hypersphere, rng=np.random.default_rng(0))
     points = ell.sample(100)
     points_t = ell.transform(points)
     assert np.all(np.abs(points_t) < 1 + 1e-9)
     assert np.allclose(points, ell.transform(points_t, inverse=True))
 
 
-def test_ellipsoid_random_state(random_points_from_hypersphere):
-    # Test that passing a random state leads to reproducible results.
+def test_ellipsoid_rng(random_points_from_hypersphere):
+    # Test that passing a random number generator leads to reproducible
+    # results.
 
     ell = bounds.Ellipsoid.compute(
-        random_points_from_hypersphere, random_state=np.random.RandomState(0))
+        random_points_from_hypersphere, rng=np.random.default_rng(0))
     ell_same = bounds.Ellipsoid.compute(
-        random_points_from_hypersphere, random_state=np.random.RandomState(0))
+        random_points_from_hypersphere, rng=np.random.default_rng(0))
     ell_diff = bounds.Ellipsoid.compute(
-        random_points_from_hypersphere, random_state=np.random.RandomState(1))
+        random_points_from_hypersphere, rng=np.random.default_rng(1))
     n_points = 1000
     points = ell.sample(n_points)
     assert np.all(points == ell_same.sample(n_points))
     assert not np.all(points == ell_diff.sample(n_points))
     assert not np.all(points == ell.sample(n_points))
 
 
@@ -185,101 +185,85 @@
                              n_points_min=5)
 
 
 def test_union_split(random_points_from_hypersphere):
     # Test that adding ellipsoids works correctly.
 
     points = np.concatenate([random_points_from_hypersphere,
-                             random_points_from_hypersphere + 100])
+                             random_points_from_hypersphere + 100,
+                             random_points_from_hypersphere + 101])
 
     union = bounds.Union.compute(
-        points, enlarge_per_dim=1.0 + 1e-9,
-        unit=False, random_state=np.random.RandomState(0))
+        points, enlarge_per_dim=1.0 + 1e-9, unit=False,
+        rng=np.random.default_rng(0))
 
     # When not allowing overlaps, only 2 ellipsoids should be possible.
     while union.split_bound(allow_overlap=False):
         pass
     assert len(union.bounds) == 2
     assert np.all(union.contains(points))
 
-    # It should be possible to add 3 more ellipoids when overlaps are allowed.
-    for i in range(3):
-        assert union.split_bound(allow_overlap=True)
-    assert len(union.bounds) == 5
-    assert np.all(union.contains(points))
-
-    points = np.random.random((20, 10))
-    union = bounds.Union.compute(points)
-    # Check that no new ellipsoid can be added.
+    # It should be possible to add one more ellipoids when overlaps are
+    # allowed.
+    assert union.split_bound()
     assert not union.split_bound()
-
-    # Check that every split leads to ellipsoids with the minimum number of
-    # points.
-    np.random.seed(0)
-    n_points_min = 10
-    for i in range(10):
-        points = np.random.random((2 * n_points_min, 2))
-        union = bounds.Union.compute(points, n_points_min=n_points_min)
-        union.split_bound()
-        assert len(union.points) == 2
-        assert len(union.points[0]) == n_points_min
-        assert len(union.points[1]) == n_points_min
+    assert len(union.bounds) == 3
+    assert np.all(union.contains(points))
 
 
 def test_union_sample_and_contains(random_points_from_hypersphere):
     # Test whether the union sampling and boundary work as expected.
 
     union = bounds.Union.compute(
         random_points_from_hypersphere + 50, enlarge_per_dim=1.0,
-        unit=False, random_state=np.random.RandomState(0))
+        unit=False, rng=np.random.default_rng(0))
     for i in range(4):
         union.split_bound()
 
     n_points = 100
     points = union.sample(n_points)
     assert points.shape == (n_points, random_points_from_hypersphere.shape[1])
     assert np.all(union.contains(points))
 
     union_large = bounds.Union.compute(
-        points, enlarge_per_dim=1.1, unit=False,
-        random_state=np.random.RandomState(0))
+        points, enlarge_per_dim=1.1, unit=False, rng=np.random.default_rng(0))
     points = union_large.sample(n_points)
     assert not np.all(union.contains(points))
 
 
-def test_union_random_state(random_points_from_hypersphere):
-    # Test that passing a random state leads to reproducible results.
+def test_union_rng(random_points_from_hypersphere):
+    # Test that passing a random number generator leads to reproducible
+    # results.
 
     union = bounds.Union.compute(
         random_points_from_hypersphere, unit=False,
-        random_state=np.random.RandomState(0))
+        rng=np.random.default_rng(0))
     union.split_bound()
     union_same = bounds.Union.compute(
         random_points_from_hypersphere, unit=False,
-        random_state=np.random.RandomState(0))
+        rng=np.random.default_rng(0))
     union_same.split_bound()
     union_diff = bounds.Union.compute(
         random_points_from_hypersphere, unit=False,
-        random_state=np.random.RandomState(1))
+        rng=np.random.default_rng(1))
     union_diff.split_bound()
     n_points = 100
     points = union.sample(n_points)
     assert np.all(points == union_same.sample(n_points))
     assert not np.all(points == union_diff.sample(n_points))
     assert not np.all(points == union.sample(n_points))
 
 
 def test_neural_bound_contains(random_points_from_hypercube):
     # Test whether the neural sampling and boundary work as expected.
 
     points = random_points_from_hypercube
     log_l = -np.linalg.norm(points - 0.5, axis=1)
     log_l_min = np.median(log_l)
-    nbound = bounds.NeuralBound.compute(points, log_l, log_l_min, n_networks=1,
-                                        n_jobs=1)
+    nbound = bounds.NeuralBound.compute(points, log_l, log_l_min, n_networks=1)
 
     n_points = 100
     n_dim = random_points_from_hypercube.shape[1]
     points = np.random.random(size=(n_points, n_dim))
     log_l = -np.linalg.norm(points - 0.5, axis=1)
     in_bound = nbound.contains(points)
     assert np.mean(log_l[in_bound] > log_l_min) >= 0.9
@@ -287,16 +271,16 @@
 
 def test_nautilus_bound_sample_and_contains(random_points_from_hypercube):
     # Test whether the nautilus sampling and boundary work as expected.
 
     points = random_points_from_hypercube
     log_l = -np.linalg.norm(points - 0.5, axis=1)
     log_l_min = np.median(log_l)
-    nbound = bounds.NautilusBound.compute(points, log_l, log_l_min,
-                                          np.log(0.5), n_networks=1, n_jobs=1)
+    nbound = bounds.NautilusBound.compute(
+        points, log_l, log_l_min, np.log(0.5), n_networks=1)
 
     n_points = 100
     n_dim = random_points_from_hypercube.shape[1]
     points = np.random.random(size=(n_points, n_dim))
     log_l = -np.linalg.norm(points - 0.5, axis=1)
     in_bound = nbound.contains(points)
     assert np.mean(log_l[in_bound] > log_l_min) >= 0.9
@@ -319,44 +303,27 @@
     log_l = -((np.linalg.norm(points - 0.5, axis=1) - radius) / width)**2
     log_l_min = -1
     points = points[log_l > -100]
     log_l = log_l[log_l > -100]
     log_v_target = np.log(2 * np.pi * radius * width * 2)
 
     nbound = bounds.NautilusBound.compute(
-        points, log_l, log_l_min, log_v_target,
-        split_threshold=1, n_networks=1, n_jobs=1,
-        random_state=np.random.RandomState(0))
+        points, log_l, log_l_min, log_v_target, split_threshold=1,
+        n_networks=1, rng=np.random.default_rng(0))
 
     points = nbound.sample(10000)
     log_l = -((np.linalg.norm(points - 0.5, axis=1) - radius) / width)**2
     # The volume should be close to the true volume where log_l > log_l_min.
     assert np.isclose(nbound.volume(), log_v_target, rtol=0, atol=np.log(2))
     # Most sampled points should have log_l > log_l_min.
     assert np.mean(log_l > log_l_min) > 0.5
     # We should have only one neural network.
     assert nbound.number_of_networks_and_ellipsoids()[0] == 1
 
 
-def test_nautilus_bound_small_target(random_points_from_hypercube):
-    # Test that nothing catastrophic happens if we set the target volume to
-    # effectively 0. This should just result in very aggresive ellipsoid
-    # splitting and make the boundary miss a small part of the parameter space.
-
-    points = random_points_from_hypercube
-    log_l = -np.linalg.norm(points - 0.5, axis=1)
-    log_l_min = np.amin(log_l)
-    nbound = bounds.NautilusBound.compute(
-        points, log_l, log_l_min, -np.inf, n_points_min=20, n_networks=1,
-        n_jobs=1, random_state=np.random.RandomState(0))
-    assert nbound.volume() > -1
-    assert nbound.number_of_networks_and_ellipsoids()[0] == 1
-    assert nbound.number_of_networks_and_ellipsoids()[1] > 10
-
-
 def test_nautilus_bound_two_peaks():
     # Test that the nautilus bound can identify and sample efficienctly from
     # two peaks with wide separations.
 
     np.random.seed(0)
     radius = 1e-5
     points = np.vstack([np.random.normal(size=(1000, 2)) * radius + 0.1,
@@ -367,18 +334,50 @@
             np.linalg.norm(x - 0.1, axis=-1),
             np.linalg.norm(x - 0.9, axis=-1)) / radius
 
     log_l = likelihood(points)
     log_l_min = -1
     log_v_target = np.log(2 * np.pi * radius**2)
     nbound = bounds.NautilusBound.compute(
-        points, log_l, log_l_min, log_v_target, n_networks=1, n_jobs=1,
-        random_state=np.random.RandomState(0))
+        points, log_l, log_l_min, log_v_target, n_networks=1,
+        rng=np.random.default_rng(0))
 
     points = nbound.sample(10000)
     log_l = likelihood(points)
     # The volume should be close to the true volume where log_l > log_l_min.
     assert np.isclose(nbound.volume(), log_v_target, rtol=0, atol=0.1)
     # Most sampled points should have log_l > log_l_min.
     assert np.mean(log_l > log_l_min) > 0.9
     # We should have two neural networks.
     assert nbound.number_of_networks_and_ellipsoids()[0] == 2
+
+
+@pytest.mark.parametrize("n_jobs", [1, 2])
+def test_nautilus_bound_reset_and_sample(random_points_from_hypercube, n_jobs):
+    # Test that resetting the bound works as expected and that we can sample
+    # in parallel.
+
+    points = random_points_from_hypercube
+    log_l = -np.linalg.norm(points - 0.5, axis=1)
+    log_l_min = np.median(log_l)
+
+    if n_jobs > 1:
+        pool = Pool(n_jobs)
+    else:
+        pool = None
+
+    nbound = bounds.NautilusBound.compute(
+        points, log_l, log_l_min, np.log(0.5), n_networks=1, pool=pool,
+        rng=np.random.default_rng(0))
+
+    nbound.reset(np.random.default_rng(0))
+    points_1 = nbound.sample(10000, pool=pool)
+    volume_1 = nbound.volume()
+    nbound.reset(np.random.default_rng(0))
+    points_2 = nbound.sample(10000, pool=pool)
+    volume_2 = nbound.volume()
+
+    if n_jobs > 1:
+        pool.close()
+
+    assert np.all(points_1 == points_2)
+    assert volume_1 == volume_2
```

### Comparing `nautilus-sampler-0.5.0/tests/test_io.py` & `nautilus-sampler-0.6.0/tests/test_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,100 +20,110 @@
 
 def test_neural_io(h5py_group):
     # Test that we can write and read a neural network emulator correctly.
 
     points = np.random.random((100, 2))
     log_l = -np.linalg.norm(points - 0.5, axis=1)
     emulator_write = NeuralNetworkEmulator.train(points, log_l, n_networks=1,
-                                                 n_jobs=1)
+                                                 pool=None)
     emulator_write.write(h5py_group)
     emulator_read = NeuralNetworkEmulator.read(h5py_group)
     assert np.all(emulator_write.predict(points) ==
                   emulator_read.predict(points))
 
 
 @pytest.mark.parametrize("bound_class", [UnitCube, Ellipsoid, Union,
                                          UnitCubeEllipsoidMixture, NeuralBound,
                                          NautilusBound])
-@pytest.mark.parametrize("random_state_sync", [True, False])
-def test_bounds_io(h5py_group, bound_class, random_state_sync):
+@pytest.mark.parametrize("rng_sync", [True, False])
+def test_bounds_io(h5py_group, bound_class, rng_sync):
     # Test that we can write and read a bound correctly. In particular, also
-    # test that the random state is correctly set after writing and reading.
+    # test that the random number generator is correctly set after writing and
+    # reading.
 
     n_dim = 5
     n_points = 100
     np.random.seed(0)
     points = np.random.random((n_points, n_dim))
-    random_state = np.random.RandomState()
+    rng = np.random.default_rng(0)
 
     if bound_class == UnitCube:
         args = (n_dim, )
         kwargs = dict()
     elif bound_class in [Ellipsoid, Union, UnitCubeEllipsoidMixture]:
         args = (points, )
         kwargs = dict()
     else:
         log_l = -np.linalg.norm(points - 0.5, axis=1)
         log_l_min = np.median(log_l)
         if bound_class == NeuralBound:
             args = (points, log_l, log_l_min)
         else:
             args = (points, log_l, log_l_min, np.log(0.5))
-        kwargs = dict(n_networks=1, n_jobs=1)
+        kwargs = dict(n_networks=1, pool=None)
 
-    bound_write = bound_class.compute(*args, **kwargs,
-                                      random_state=random_state)
+    bound_write = bound_class.compute(*args, **kwargs, rng=rng)
     if bound_class == Union:
         bound_write.split_bound()
 
     bound_write.write(h5py_group)
-    if random_state_sync:
-        random_state = np.random.RandomState()
-        random_state.set_state(bound_write.random_state.get_state())
-    else:
-        random_state = None
-    bound_read = bound_class.read(h5py_group, random_state=random_state)
+    rng = np.random.default_rng(1)
+    if rng_sync:
+        if bound_class == NeuralBound:
+            rng = None
+        elif bound_class == UnitCubeEllipsoidMixture:
+            rng.bit_generator.state = bound_write.cube.rng.bit_generator.state
+        else:
+            rng.bit_generator.state = bound_write.rng.bit_generator.state
+
+    bound_read = bound_class.read(h5py_group, rng=rng)
 
     if bound_class != NeuralBound:
         assert (np.all(bound_write.sample(10000) == bound_read.sample(10000))
-                == random_state_sync)
+                == rng_sync)
 
-    if ((random_state_sync or bound_class in [UnitCube, Ellipsoid]) and not
+    if ((rng_sync or bound_class in [UnitCube, Ellipsoid]) and not
             bound_class == NeuralBound):
         assert bound_write.volume() == bound_read.volume()
 
     points = np.random.random((10000, n_dim))
     assert np.all(bound_write.contains(points) == bound_read.contains(points))
 
 
 @pytest.mark.parametrize("blobs", [True, False])
-def test_sampler_io(blobs):
+@pytest.mark.parametrize("discard_exploration", [True, False])
+@pytest.mark.parametrize("n_networks", [0, 1, 2])
+def test_sampler_io(blobs, discard_exploration, n_networks):
     # Test that we can write and read a sampler correctly. In particular, also
-    # test that the random state is correctly set after writing and reading.
-    # Also make sure that the sampler can print out the progress.
+    # test that the random number generator is correctly set after writing and
+    # reading. Also make sure that the sampler can print out the progress.
 
     def prior(x):
         return x
 
     def likelihood(x):
         if blobs:
             return -np.linalg.norm(x - 0.5) * 0.001, x[0]
         else:
             return -np.linalg.norm(x - 0.5) * 0.001
 
     sampler_write = Sampler(prior, likelihood, n_dim=2, n_live=100,
-                            n_networks=1, n_jobs=1, filepath='test.hdf5',
-                            resume=False, random_state=0)
+                            n_networks=n_networks, n_jobs=1,
+                            filepath='test.hdf5', resume=False, seed=0)
     sampler_write.run(f_live=0.45, n_eff=0, verbose=True)
+    sampler_write.explored = False
     sampler_read = Sampler(prior, likelihood, n_dim=2, n_live=100,
-                           n_networks=1, n_jobs=1,  filepath='test.hdf5',
-                           resume=True)
-
-    sampler_write.run(n_eff=1000, verbose=True)
-    sampler_read.run(n_eff=1000, verbose=True)
+                           n_networks=n_networks, n_jobs=1,
+                           filepath='test.hdf5', resume=True)
+    sampler_read.explored = False
+
+    sampler_write.run(f_live=0.45, n_eff=1000,
+                      discard_exploration=discard_exploration, verbose=True)
+    sampler_read.run(f_live=0.45, n_eff=1000,
+                     discard_exploration=discard_exploration, verbose=True)
 
     posterior_write = sampler_write.posterior()
     posterior_read = sampler_read.posterior()
 
     for arr_write, arr_read in zip(posterior_write, posterior_read):
         assert np.all(arr_write == arr_read)
 
@@ -130,15 +140,15 @@
         return x
 
     def likelihood(x):
         return -np.linalg.norm(x - 0.5) * 0.001
 
     sampler = Sampler(prior, likelihood, n_dim=2, n_live=100,
                       n_networks=1, n_jobs=1, filepath='test.hdf5',
-                      resume=False, random_state=0)
+                      resume=False, seed=0)
     sampler.run(n_eff=1000, discard_exploration=True)
 
     assert Path('test.hdf5').is_file()
     assert Path('test_exp.hdf5').is_file()
 
     Path('test.hdf5').unlink()
     Path('test_exp.hdf5').unlink()
```

### Comparing `nautilus-sampler-0.5.0/tests/test_pool.py` & `nautilus-sampler-0.6.0/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/tests/test_prior.py` & `nautilus-sampler-0.6.0/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.5.0/tests/test_sampler.py` & `nautilus-sampler-0.6.0/tests/test_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     sampler.run(f_live=0.45, n_eff=0, verbose=False)
     points, log_w, log_l = sampler.posterior(return_as_dict=pass_dict)
     if custom_prior and pass_dict:
         with pytest.raises(ValueError):
             points, log_w, log_l = sampler.posterior(return_as_dict=False)
 
 
-@pytest.mark.parametrize("n_networks", [0, 1])
+@pytest.mark.parametrize("n_networks", [0, 4])
 @pytest.mark.parametrize("discard_exploration", [True, False])
 def test_sampler_accuracy(n_networks, discard_exploration):
     # Do a basic tests of the sampler accuracy.
 
     n_dim = 2
     mean = np.repeat(0.5, n_dim)
     cov = np.eye(n_dim) * 0.01
@@ -78,15 +78,15 @@
     def prior(x):
         return x
 
     def likelihood(x):
         return multivariate_normal.logpdf(x, mean=mean, cov=cov)
 
     sampler = Sampler(prior, likelihood, n_dim=n_dim, n_live=500,
-                      n_networks=n_networks, n_jobs=1, random_state=0)
+                      n_networks=n_networks, n_jobs=1, seed=0)
     sampler.run(discard_exploration=discard_exploration, f_live=0.1,
                 verbose=False)
 
     assert np.abs(sampler.evidence()) < 0.05
 
     for equal_weight in [True, False]:
         points, log_w, log_l = sampler.posterior(equal_weight=equal_weight)
@@ -113,15 +113,15 @@
     def prior(x):
         return x
 
     def likelihood(x):
         return -np.linalg.norm(x - 0.5)**2 * 0.001
 
     sampler = Sampler(prior, likelihood, n_dim=2, enlarge_per_dim=100,
-                      n_networks=0, n_jobs=1, random_state=0)
+                      n_networks=0, n_jobs=1, seed=0)
     sampler.run(f_live=0.1, n_eff=0)
 
     # The effective sample size should be very close to the number of calls
     # since the likelihood is extremely flat.
     assert np.isclose(sampler.n_like, sampler.effective_sample_size(), rtol=0,
                       atol=1)
     # Only one bound should be left.
@@ -150,15 +150,15 @@
     # the unit cube.
     np.random.seed(0)
     x_0 = np.random.normal(loc=0.5, scale=0.1, size=1000000)
     x_1 = np.random.normal(loc=0.5, scale=np.exp(20 * (x_0 - 0.5)) / 100)
     log_z_true = np.log(np.mean((x_0 > 0) & (x_0 < 1) & (x_1 > 0) & (x_1 < 1)))
 
     sampler = Sampler(prior, likelihood, n_dim=2, n_networks=1, n_jobs=1,
-                      random_state=0)
+                      seed=0)
     sampler.run()
     assert np.isclose(log_z_true, sampler.evidence(), rtol=0, atol=0.1)
     # Check whether the boundaries nautilus drew are strictly nested.
     shell_bound_occupation = sampler.shell_bound_occupation()
     if np.all(shell_bound_occupation ==
               np.tril(np.ones_like(shell_bound_occupation))):
         warnings.warn('The funnel distribution was too easy.', RuntimeWarning)
```

### Comparing `nautilus-sampler-0.5.0/PKG-INFO` & `nautilus-sampler-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus-sampler
-Version: 0.5.0
+Version: 0.6.0
 Summary: Neural Network-Boosted Importance Sampling for Bayesian Statistics
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
```

