# Comparing `tmp/elex-solver-1.0.2.tar.gz` & `tmp/elex-solver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elex-solver-1.0.2.tar", last modified: Wed Sep 14 17:02:25 2022, max compression
+gzip compressed data, was "elex-solver-1.1.0.tar", last modified: Fri Apr 21 22:08:11 2023, max compression
```

## Comparing `elex-solver-1.0.2.tar` & `elex-solver-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 liue       (503) staff       (20)        0 2022-09-14 17:02:25.594711 elex-solver-1.0.2/
--rw-r--r--   0 liue       (503) staff       (20)     1459 2022-09-14 17:02:25.594795 elex-solver-1.0.2/PKG-INFO
--rw-r--r--   0 liue       (503) staff       (20)     1118 2022-09-14 16:48:48.000000 elex-solver-1.0.2/README.md
--rw-r--r--   0 liue       (503) staff       (20)      104 2022-09-14 17:02:25.595104 elex-solver-1.0.2/setup.cfg
--rw-r--r--   0 liue       (503) staff       (20)     1420 2022-09-14 17:00:19.000000 elex-solver-1.0.2/setup.py
-drwxr-xr-x   0 liue       (503) staff       (20)        0 2022-09-14 17:02:25.592567 elex-solver-1.0.2/src/
-drwxr-xr-x   0 liue       (503) staff       (20)        0 2022-09-14 17:02:25.593777 elex-solver-1.0.2/src/elex_solver.egg-info/
--rw-r--r--   0 liue       (503) staff       (20)     1459 2022-09-14 17:02:25.000000 elex-solver-1.0.2/src/elex_solver.egg-info/PKG-INFO
--rw-r--r--   0 liue       (503) staff       (20)      397 2022-09-14 17:02:25.000000 elex-solver-1.0.2/src/elex_solver.egg-info/SOURCES.txt
--rw-r--r--   0 liue       (503) staff       (20)        1 2022-09-14 17:02:25.000000 elex-solver-1.0.2/src/elex_solver.egg-info/dependency_links.txt
--rw-r--r--   0 liue       (503) staff       (20)        1 2022-09-14 16:50:32.000000 elex-solver-1.0.2/src/elex_solver.egg-info/not-zip-safe
--rw-r--r--   0 liue       (503) staff       (20)       13 2022-09-14 17:02:25.000000 elex-solver-1.0.2/src/elex_solver.egg-info/requires.txt
--rw-r--r--   0 liue       (503) staff       (20)       11 2022-09-14 17:02:25.000000 elex-solver-1.0.2/src/elex_solver.egg-info/top_level.txt
-drwxr-xr-x   0 liue       (503) staff       (20)        0 2022-09-14 17:02:25.594452 elex-solver-1.0.2/src/elexsolver/
--rw-r--r--   0 liue       (503) staff       (20)     3174 2022-09-14 16:48:48.000000 elex-solver-1.0.2/src/elexsolver/QuantileRegressionSolver.py
--rw-r--r--   0 liue       (503) staff       (20)      936 2022-09-14 16:48:48.000000 elex-solver-1.0.2/src/elexsolver/TransitionMatrixSolver.py
--rw-r--r--   0 liue       (503) staff       (20)        0 2022-09-14 16:48:48.000000 elex-solver-1.0.2/src/elexsolver/__init__.py
--rw-r--r--   0 liue       (503) staff       (20)      885 2022-09-14 16:48:48.000000 elex-solver-1.0.2/src/elexsolver/logging.py
+drwxr-xr-x   0 bronnerl (290512236) 1978051377        0 2023-04-21 22:08:11.278476 elex-solver-1.1.0/
+-rw-r--r--   0 bronnerl (290512236) 1978051377     1544 2023-04-21 22:08:11.278655 elex-solver-1.1.0/PKG-INFO
+-rw-r--r--   0 bronnerl (290512236) 1978051377     1203 2023-04-21 22:07:18.000000 elex-solver-1.1.0/README.md
+-rw-r--r--   0 bronnerl (290512236) 1978051377      104 2023-04-21 22:08:11.279552 elex-solver-1.1.0/setup.cfg
+-rw-r--r--   0 bronnerl (290512236) 1978051377     1417 2023-04-21 22:07:18.000000 elex-solver-1.1.0/setup.py
+drwxr-xr-x   0 bronnerl (290512236) 1978051377        0 2023-04-21 22:08:11.269834 elex-solver-1.1.0/src/
+drwxr-xr-x   0 bronnerl (290512236) 1978051377        0 2023-04-21 22:08:11.274413 elex-solver-1.1.0/src/elex_solver.egg-info/
+-rw-r--r--   0 bronnerl (290512236) 1978051377     1544 2023-04-21 22:08:11.000000 elex-solver-1.1.0/src/elex_solver.egg-info/PKG-INFO
+-rw-r--r--   0 bronnerl (290512236) 1978051377      420 2023-04-21 22:08:11.000000 elex-solver-1.1.0/src/elex_solver.egg-info/SOURCES.txt
+-rw-r--r--   0 bronnerl (290512236) 1978051377        1 2023-04-21 22:08:11.000000 elex-solver-1.1.0/src/elex_solver.egg-info/dependency_links.txt
+-rw-r--r--   0 bronnerl (290512236) 1978051377        1 2023-04-17 20:32:54.000000 elex-solver-1.1.0/src/elex_solver.egg-info/not-zip-safe
+-rw-r--r--   0 bronnerl (290512236) 1978051377       13 2023-04-21 22:08:11.000000 elex-solver-1.1.0/src/elex_solver.egg-info/requires.txt
+-rw-r--r--   0 bronnerl (290512236) 1978051377       11 2023-04-21 22:08:11.000000 elex-solver-1.1.0/src/elex_solver.egg-info/top_level.txt
+drwxr-xr-x   0 bronnerl (290512236) 1978051377        0 2023-04-21 22:08:11.277047 elex-solver-1.1.0/src/elexsolver/
+-rw-r--r--   0 bronnerl (290512236) 1978051377     5007 2023-04-21 22:07:18.000000 elex-solver-1.1.0/src/elexsolver/QuantileRegressionSolver.py
+-rw-r--r--   0 bronnerl (290512236) 1978051377      935 2023-04-21 22:07:18.000000 elex-solver-1.1.0/src/elexsolver/TransitionMatrixSolver.py
+-rw-r--r--   0 bronnerl (290512236) 1978051377        0 2023-04-17 20:31:56.000000 elex-solver-1.1.0/src/elexsolver/__init__.py
+-rw-r--r--   0 bronnerl (290512236) 1978051377      920 2023-04-21 22:07:18.000000 elex-solver-1.1.0/src/elexsolver/logging.py
+drwxr-xr-x   0 bronnerl (290512236) 1978051377        0 2023-04-21 22:08:11.277804 elex-solver-1.1.0/tests/
+-rw-r--r--   0 bronnerl (290512236) 1978051377    11217 2023-04-21 22:07:18.000000 elex-solver-1.1.0/tests/test_quantile.py
```

### Comparing `elex-solver-1.0.2/PKG-INFO` & `elex-solver-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elex-solver
-Version: 1.0.2
+Version: 1.1.0
 Summary: A package for optimization solvers
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -31,11 +31,17 @@
 
 Set up a virtual environment and run:
 ```
 > pip install -r requirements.txt
 > pip install -r requirements-dev.txt 
 ```
 
+## Precommit
+To run pre-commit for linting, run:
+```
+pre-commit run --all-files
+```
+
 ## Testing
 ```
 > tox
 ```
```

### Comparing `elex-solver-1.0.2/README.md` & `elex-solver-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,17 @@
 
 Set up a virtual environment and run:
 ```
 > pip install -r requirements.txt
 > pip install -r requirements-dev.txt 
 ```
 
+## Precommit
+To run pre-commit for linting, run:
+```
+pre-commit run --all-files
+```
+
 ## Testing
 ```
 > tox
 ```
```

### Comparing `elex-solver-1.0.2/src/elex_solver.egg-info/PKG-INFO` & `elex-solver-1.1.0/src/elex_solver.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elex-solver
-Version: 1.0.2
+Version: 1.1.0
 Summary: A package for optimization solvers
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
@@ -31,11 +31,17 @@
 
 Set up a virtual environment and run:
 ```
 > pip install -r requirements.txt
 > pip install -r requirements-dev.txt 
 ```
 
+## Precommit
+To run pre-commit for linting, run:
+```
+pre-commit run --all-files
+```
+
 ## Testing
 ```
 > tox
 ```
```

### Comparing `elex-solver-1.0.2/src/elexsolver/QuantileRegressionSolver.py` & `elex-solver-1.1.0/src/elexsolver/QuantileRegressionSolver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import logging
+import warnings
 
 import cvxpy as cp
 import numpy as np
 
 from elexsolver.logging import initialize_logging
 
 initialize_logging()
 
 LOG = logging.getLogger(__name__)
 
+
 class QuantileRegressionSolverException(Exception):
     pass
 
+
 class IllConditionedMatrixException(QuantileRegressionSolverException):
     pass
 
-class QuantileRegressionSolver():
 
-    VALID_SOLVERS = {'SCS', 'ECOS', 'MOSEK', 'OSQP', 'CVXOPT', 'GLPK'}
-    KWARGS = {
-        "ECOS": {
-            "max_iters": 10000
-        }
-    }
+class QuantileRegressionSolver:
+
+    VALID_SOLVERS = {"SCS", "ECOS", "MOSEK", "OSQP", "CVXOPT", "GLPK"}
+    KWARGS = {"ECOS": {"max_iters": 10000}}
 
-    CONDITION_WARNING_MIN = 50 # arbitrary
-    CONDITION_ERROR_MIN = 1e+8 # based on scipy
+    CONDITION_WARNING_MIN = 50  # arbitrary
+    CONDITION_ERROR_MIN = 1e8  # based on scipy
 
-    def __init__(self, solver='ECOS'):
+    def __init__(self, solver="ECOS"):
         if solver not in self.VALID_SOLVERS:
             raise ValueError(f"solver must be in {self.VALID_SOLVERS}")
         self.tau = cp.Parameter()
         self.coefficients = None
         self.problem = None
         self.solver = solver
 
@@ -42,52 +42,103 @@
         """
         condition_number = np.linalg.cond(x)
         if condition_number >= self.CONDITION_ERROR_MIN:
             raise IllConditionedMatrixException(
                 f"Ill-conditioned matrix detected. Matrix condition number >= {self.CONDITION_ERROR_MIN}"
             )
         elif condition_number >= self.CONDITION_WARNING_MIN:
-            LOG.warn(f"Ill-conditioned matrix detected. result is not guaranteed to be accurate")
-            return False
-        return True
+            warnings.warn("Warning: Ill-conditioned matrix detected. result is not guaranteed to be accurate")
 
-    def __solve(self, x, y, weights, verbose):
+    def _check_any_element_nan_or_inf(self, x):
         """
-        Sets up the optimization problem and solves it
+        Check whether any element in a matrix or vector is NaN or infinity
+        """
+        if np.any(np.isnan(x)) or np.any(np.isinf(x)):
+            raise ValueError("Array contains NaN or Infinity")
+
+    def _check_intercept(self, x):
+        """
+        Check whether the first column is all 1s (normal intercept) otherwise raises a warning.
+        """
+        if ~np.all(x[:, 0] == 1):
+            warnings.warn("Warning: fit_intercept=True and not all elements of the first columns are 1s")
+
+    def get_loss_function(self, x, y, coefficients, weights):
+        """
+        Get the quantile regression loss function
         """
-        self._check_matrix_condition(x)
-        coefficients = cp.Variable((x.shape[1], ))
         y_hat = x @ coefficients
         residual = y - y_hat
-        loss_function = cp.sum(cp.multiply(weights, 0.5 * cp.abs(residual) + (self.tau.value - 0.5) * residual))
+        return cp.sum(cp.multiply(weights, 0.5 * cp.abs(residual) + (self.tau.value - 0.5) * residual))
+
+    def get_regularizer(self, coefficients, fit_intercept):
+        """
+        Get regularization component of the loss function. Note that this is L2 (ridge) regularization.
+        """
+        # if we are fitting an intercept in the model, then that coefficient should not be regularized.
+        # NOTE: assumes that if fit_intercept=True, that the intercept is in the first column
+        coefficients_to_regularize = coefficients
+        if fit_intercept:
+            coefficients_to_regularize = coefficients[1:]
+        return cp.pnorm(coefficients_to_regularize, p=2) ** 2
+
+    def __solve(self, x, y, weights, lambda_, fit_intercept, verbose):
+        """
+        Sets up the optimization problem and solves it
+        """
+        self._check_matrix_condition(x)
+        coefficients = cp.Variable((x.shape[1],))
+        loss_function = self.get_loss_function(x, y, coefficients, weights)
+        loss_function += lambda_ * self.get_regularizer(coefficients, fit_intercept)
         objective = cp.Minimize(loss_function)
         problem = cp.Problem(objective)
         problem.solve(solver=self.solver, verbose=verbose, **self.KWARGS.get(self.solver, {}))
         return coefficients, problem
 
-    def fit(self, x, y, tau_value=0.5, weights=None, verbose=False, save_problem=False, normalize_weights=True):
+    def fit(
+        self,
+        x,
+        y,
+        tau_value=0.5,
+        weights=None,
+        lambda_=0,
+        fit_intercept=True,
+        verbose=False,
+        save_problem=False,
+        normalize_weights=True,
+    ):
         """
         Fit the (weighted) quantile regression problem.
         Weights should not sum to one.
+        If fit_intercept=True then intercept is assumed to be the first column in `x`
         """
-        if weights is None: # if weights are none, give unit weights
+
+        self._check_any_element_nan_or_inf(x)
+        self._check_any_element_nan_or_inf(y)
+
+        if fit_intercept:
+            self._check_intercept(x)
+
+        if weights is None:  # if weights are none, give unit weights
             weights = [1] * x.shape[0]
         if normalize_weights:
             weights_sum = np.sum(weights)
             if weights_sum == 0:
                 # This should not happen
                 raise ZeroDivisionError
             weights = weights / weights_sum
-        
+
         self.tau.value = tau_value
-        coefficients, problem = self.__solve(x, y, weights, verbose)
+        coefficients, problem = self.__solve(x, y, weights, lambda_, fit_intercept, verbose)
         self.coefficients = coefficients.value
         if save_problem:
             self.problem = problem
         else:
             self.problem = None
 
     def predict(self, x):
         """
         Returns predictions
         """
+        self._check_any_element_nan_or_inf(x)
+
         return self.coefficients @ x.T
```

### Comparing `elex-solver-1.0.2/src/elexsolver/TransitionMatrixSolver.py` & `elex-solver-1.1.0/src/elexsolver/TransitionMatrixSolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import cvxpy as cp
 
-class TransitionMatrixSolver():
+
+class TransitionMatrixSolver:
     def __init__(self):
         self.transition_matrix = None
 
     @staticmethod
     def __get_constraint(X, strict):
         if strict:
             return [cp.sum(X, axis=1) == 1]
         return [cp.sum(X, axis=1) <= 1.1, cp.sum(X, axis=1) >= 0.9]
 
     def __solve(self, A, B, strict):
         transition_matrix = cp.Variable((A.shape[1], B.shape[1]))
-        loss_function = cp.norm(A @ transition_matrix - B, 'fro')
+        loss_function = cp.norm(A @ transition_matrix - B, "fro")
         objective = cp.Minimize(loss_function)
         constraint = TransitionMatrixSolver.__get_constraint(transition_matrix, strict)
         problem = cp.Problem(objective, constraint)
         problem.solve()
         return transition_matrix.value
 
     def fit(self, A, B, strict=False):
```

### Comparing `elex-solver-1.0.2/src/elexsolver/logging.py` & `elex-solver-1.1.0/src/elexsolver/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,9 @@
     """
     Configures logging for the app.
     """
     if not logging_config:
         app_log_level = os.getenv("APP_LOG_LEVEL", "INFO")
         LOGGING_CONFIG["loggers"]["elexsolver"]["level"] = app_log_level
         logging_config = LOGGING_CONFIG
-    logging.config.dictConfig(logging_config)
+    logging.captureWarnings(True)
+    logging.config.dictConfig(logging_config)
```

