# Comparing `tmp/mlog_arithmetic_runner-0.0.4-py3-none-any.whl.zip` & `tmp/mlog_arithmetic_runner-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7704 bytes, number of entries: 10
+Zip file size: 7874 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       72 b- defN 22-Nov-03 14:12 mlog_arithmetic_runner/__init__.py
 -rw-r--r--  2.0 unx     2474 b- defN 22-Nov-03 15:03 mlog_arithmetic_runner/__main__.py
 -rw-r--r--  2.0 unx     3096 b- defN 22-Nov-20 03:21 mlog_arithmetic_runner/arithmetic_operators.py
 -rw-r--r--  2.0 unx      575 b- defN 22-Nov-03 14:02 mlog_arithmetic_runner/memory.py
--rw-r--r--  2.0 unx     5565 b- defN 22-Nov-14 15:25 mlog_arithmetic_runner/mlog_processor.py
--rw-r--r--  2.0 unx     1067 b- defN 22-Nov-20 03:25 mlog_arithmetic_runner-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3327 b- defN 22-Nov-20 03:25 mlog_arithmetic_runner-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-20 03:25 mlog_arithmetic_runner-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       23 b- defN 22-Nov-20 03:25 mlog_arithmetic_runner-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      929 b- defN 22-Nov-20 03:25 mlog_arithmetic_runner-0.0.4.dist-info/RECORD
-10 files, 17220 bytes uncompressed, 6082 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     6302 b- defN 23-Apr-22 15:36 mlog_arithmetic_runner/mlog_processor.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-22 15:39 mlog_arithmetic_runner-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3287 b- defN 23-Apr-22 15:39 mlog_arithmetic_runner-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 15:39 mlog_arithmetic_runner-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Apr-22 15:39 mlog_arithmetic_runner-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      929 b- defN 23-Apr-22 15:39 mlog_arithmetic_runner-0.0.5.dist-info/RECORD
+10 files, 17917 bytes uncompressed, 6252 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: mlog_arithmetic_runner/memory.py
 Comment: 
 
 Filename: mlog_arithmetic_runner/mlog_processor.py
 Comment: 
 
-Filename: mlog_arithmetic_runner-0.0.4.dist-info/LICENSE
+Filename: mlog_arithmetic_runner-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: mlog_arithmetic_runner-0.0.4.dist-info/METADATA
+Filename: mlog_arithmetic_runner-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: mlog_arithmetic_runner-0.0.4.dist-info/WHEEL
+Filename: mlog_arithmetic_runner-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: mlog_arithmetic_runner-0.0.4.dist-info/top_level.txt
+Filename: mlog_arithmetic_runner-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mlog_arithmetic_runner-0.0.4.dist-info/RECORD
+Filename: mlog_arithmetic_runner-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlog_arithmetic_runner/mlog_processor.py

```diff
@@ -32,38 +32,60 @@
             # getlink get cells/banks
             "@links": lambda: self.memory_cells + self.memory_banks,
         }
         self.variables = {}
         self.reset()
 
     def assemble_code(self, mlog_code: str):
-        self.code = []
+
+        rawCode = self.solveLabel(mlog_code)
+
+        for tokens in rawCode:
+            self.code.append(tuple(tokens))
+
+    def solveLabel(self, mlog_code):
+        rawCode = []
+        labels = {}
+        todel = []
         for line in mlog_code.splitlines():
-            tokens = tuple(line.split())
+            tokens = line.split()
             if len(tokens) <= 0:
                 continue
-            self.code.append(tokens)
+            rawCode.append(tokens)
+        for j in range(len(rawCode)):
+            tokens = rawCode[j]
+            if len(tokens) == 1 & tokens[0].endswith(":"):
+                labels[tokens[0].strip(":")] = rawCode[j + 1]
+                todel.append(tokens)
+        for label in todel:
+            rawCode.remove(label)
+        for label in labels.keys():
+            index = rawCode.index(labels.get(label))
+            for tokens in rawCode:
+                if (tokens[0] == "jump") & (tokens[1] == label):
+                    tokens[1] = index
+        return rawCode
 
     def reset(self):
         self.current_line = 0
         self.instructions_executed = 0
         self.constants = {
             "true": 1,
             "false": 0,
             "null": None
         }
         self.variables = {}
         for i in range(self.memory_cells):
-            self.constants[f"cell{i+1}"] = MemoryCell(64)
+            self.constants[f"cell{i + 1}"] = MemoryCell(64)
         for i in range(self.memory_banks):
-            self.constants[f"bank{i+1}"] = MemoryCell(512)
+            self.constants[f"bank{i + 1}"] = MemoryCell(512)
 
     def get_variable(self, name: str):
         if name.startswith("@"):
-            return self.lambda_variables.get(name, lambda : None)()
+            return self.lambda_variables.get(name, lambda: None)()
         if name in self.constants:
             return self.constants[name]
         if name in self.variables:
             return self.variables[name]
         try:
             return float(name)
         except ValueError:
@@ -112,17 +134,17 @@
                 self.set_variable(tokens[1], mem.read(pos))
         elif tokens[0] == "getlink":
             # getlink get memory cells/banks ONLY
             link_id = int(self.get_variable(tokens[2]))
             if link_id >= self.get_variable("@links") or link_id < 0:
                 self.set_variable(tokens[1], None)
             elif link_id < self.memory_cells:
-                self.set_variable(tokens[1], self.get_variable(f"cell{link_id+1}"))
+                self.set_variable(tokens[1], self.get_variable(f"cell{link_id + 1}"))
             else:
-                self.set_variable(tokens[1], self.get_variable(f"bank{link_id-self.memory_cells+1}"))
+                self.set_variable(tokens[1], self.get_variable(f"bank{link_id - self.memory_cells + 1}"))
         else:
             raise ValueError(f"Unsupported instruction {tokens[0]}")
         self.instructions_executed += 1
         # Self-loop detected
         if self.next_line == self.current_line:
             return False
         self.current_line = self.next_line
```

## Comparing `mlog_arithmetic_runner-0.0.4.dist-info/LICENSE` & `mlog_arithmetic_runner-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlog_arithmetic_runner-0.0.4.dist-info/METADATA` & `mlog_arithmetic_runner-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlog-arithmetic-runner
-Version: 0.0.4
+Version: 0.0.5
 Summary: An Mindustry Logic emulator built for automated testing of compilers.
 Home-page: https://github.com/UMRnInside/MlogArithmeticRunner
 Author: UMRnInside
 Author-email: 30196401+UMRnInside@users.noreply.github.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/UMRnInside/MlogArithmeticRunner/issues
 Platform: UNKNOWN
@@ -64,15 +64,14 @@
   * (Optional, Default) Stop emulation once `@counter` past the end
   * (Optional) Dump memory cells and banks
   * Dump variables into JSON report
 
 
 ## Limitations
   * Does NOT have `@this` yet, so do `@thisx` and `@thisy`
-  * No label or "jump-to-label" support
   * No comment in mlog code
   * (not sure)
 
 ## Python Usage
 ```python
 from mlog_arithmetic_runner import MlogProcessor
 processor = MlogProcessor(ipt=2, memory_cells=0, memory_banks=0)
```

## Comparing `mlog_arithmetic_runner-0.0.4.dist-info/RECORD` & `mlog_arithmetic_runner-0.0.5.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mlog_arithmetic_runner/__init__.py,sha256=8GXTrD3uhf2pevytj5YDROawNU54Nk2oaiuwqneEugc,72
 mlog_arithmetic_runner/__main__.py,sha256=KRV2KrCw7w8hc2r5ddED3J_smxlE5x4jjqlugrNkpCc,2474
 mlog_arithmetic_runner/arithmetic_operators.py,sha256=LDhyhgCaATAOXrdnCFA0N6-hs33iIrZdXF6RmrrNKFc,3096
 mlog_arithmetic_runner/memory.py,sha256=AyvS8jfKbmTi6rspwBPRInxkF2uHMPmmj1EhqPWtJDg,575
-mlog_arithmetic_runner/mlog_processor.py,sha256=5cN3EA0ASVdKSFvAd-dELHZPQUOjm0X5pfCwt2OKazo,5565
-mlog_arithmetic_runner-0.0.4.dist-info/LICENSE,sha256=q0jTskpkyOwKFf24sfdxjz_n3a9bJyzzdo2vJhZmihE,1067
-mlog_arithmetic_runner-0.0.4.dist-info/METADATA,sha256=fNR2ZdVOUZ7t6aEye6atN65JhKFh3AFXGAXMP-4suzQ,3327
-mlog_arithmetic_runner-0.0.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mlog_arithmetic_runner-0.0.4.dist-info/top_level.txt,sha256=zh2Grst6J1FwPruH14pCLsAQLlhWBQ0qd7xfufPbYvI,23
-mlog_arithmetic_runner-0.0.4.dist-info/RECORD,,
+mlog_arithmetic_runner/mlog_processor.py,sha256=sMLlNNPg0G4TZ5uISU-e6MsTLoKl0j7E7URfWI5Z1rc,6302
+mlog_arithmetic_runner-0.0.5.dist-info/LICENSE,sha256=q0jTskpkyOwKFf24sfdxjz_n3a9bJyzzdo2vJhZmihE,1067
+mlog_arithmetic_runner-0.0.5.dist-info/METADATA,sha256=-z4Waq1ONjik71x8hWvevWRRV7cn5tYaqgEimGAL7sk,3287
+mlog_arithmetic_runner-0.0.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mlog_arithmetic_runner-0.0.5.dist-info/top_level.txt,sha256=zh2Grst6J1FwPruH14pCLsAQLlhWBQ0qd7xfufPbYvI,23
+mlog_arithmetic_runner-0.0.5.dist-info/RECORD,,
```

