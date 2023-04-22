# Comparing `tmp/entx_py-1.0.1.tar.gz` & `tmp/entx_py-1.0.2.tar.gz`

## Comparing `entx_py-1.0.1.tar` & `entx_py-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 entx_py-1.0.1/entxpy/__init__.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 entx_py-1.0.1/entxpy/errors.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 entx_py-1.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 entx_py-1.0.1/LICENSE
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 entx_py-1.0.1/README.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 entx_py-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 entx_py-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 entx_py-1.0.2/entxpy/__init__.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 entx_py-1.0.2/entxpy/errors.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 entx_py-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 entx_py-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 entx_py-1.0.2/README.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 entx_py-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 entx_py-1.0.2/PKG-INFO
```

### Comparing `entx_py-1.0.1/entxpy/__init__.py` & `entx_py-1.0.2/entxpy/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,41 +8,41 @@
             self.client = JSONClient(password)
             self.file_path = file_path
         else:
             raise InvalidPath("File does not exist.")
         
     def pack(self):
         if self.file_path.endswith(".py"):
-            with open(self.file_path, "r") as input_file:
+            with open(self.file_path, "r", encoding = "utf-8") as input_file:
                 contents = input_file.read()
                 contents_obj = {
                     "python": contents
                 }
                 new_path = self.file_path[:-3] + ".entxpy"
-                with open(new_path, "w") as output_file:
+                with open(new_path, "w", encoding = "utf-8") as output_file:
                     self.client.dump(contents_obj, output_file)
                     os.remove(self.file_path)
                     self.file_path = new_path
         else:
             raise InvalidOperation("The file to be packed must be a .py file.")
              
     def unpack(self):
         if self.file_path.endswith(".entxpy"):
-            with open(self.file_path, "r") as input_file:
+            with open(self.file_path, "r", encoding = "utf-8") as input_file:
                 decrypted_contents = self.client.load(input_file)
                 new_path = self.file_path[:-7] + ".py"
-                with open(new_path, "w") as output_file:
+                with open(new_path, "w", encoding = "utf-8") as output_file:
                     output_file.write(decrypted_contents["python"])
                     os.remove(self.file_path)
                     self.file_path = new_path
         else:
             raise InvalidOperation("The file to be unpacked must be a .entxpy file.")
     
     def run(self):
         if self.file_path.endswith(".py"):
-            with open(self.file_path, "r") as to_run:
+            with open(self.file_path, "r", encoding = "utf-8") as to_run:
                 exec(to_run)
         elif self.file_path.endswith(".entxpy"):
-            with open(self.file_path, "r") as to_run:
+            with open(self.file_path, "r", encoding = "utf-8") as to_run:
                 exec(self.client.load(to_run)["python"])
         else:
             raise InvalidOperation("File must be either a .py file or a .entxpy file.")
```

### Comparing `entx_py-1.0.1/LICENSE` & `entx_py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `entx_py-1.0.1/README.md` & `entx_py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `entx_py-1.0.1/pyproject.toml` & `entx_py-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "entx-py"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="MaskdDev", email="maskddev@gmail.com" },
 ]
 description = "The python file encryption library."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `entx_py-1.0.1/PKG-INFO` & `entx_py-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entx-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: The python file encryption library.
 Project-URL: Homepage, https://github.com/MaskdDev/entxpy
 Project-URL: Bug Tracker, https://github.com/MaskdDev/entxpy/issues
 Author-email: MaskdDev <maskddev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

