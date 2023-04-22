# Comparing `tmp/jupylite_duckdb-0.0.5-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5638 bytes, number of entries: 9
+Zip file size: 5610 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-22 14:48 jupylite_duckdb/_version.py
--rw-rw-rw-  2.0 fat     8833 b- defN 23-Apr-22 14:33 jupylite_duckdb/jdw.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-22 15:13 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-Apr-22 15:13 jupylite_duckdb/jdw.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 15:10 jupylite_duckdb-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1296 b- defN 23-Apr-22 15:10 jupylite_duckdb-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:10 jupylite_duckdb-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 15:10 jupylite_duckdb-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      750 b- defN 23-Apr-22 15:10 jupylite_duckdb-0.0.5.dist-info/RECORD
-9 files, 13610 bytes uncompressed, 4334 bytes compressed:  68.2%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1296 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      750 b- defN 23-Apr-22 15:13 jupylite_duckdb-0.0.6.dist-info/RECORD
+9 files, 13534 bytes uncompressed, 4306 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: jupylite_duckdb/jdw.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.5.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.5.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.5.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.5.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.5.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.5"
+__version__="0.0.6"
```

## jupylite_duckdb/jdw.py

```diff
@@ -17,15 +17,14 @@
     data = [dict(v) for v in a.object_values()] 
 
     df = DataFrame(data)
     return df
 
 async def query(sql: str, connection: object = None, return_future= True) -> DataFrame:
     """Executes query in a standalone connection"""
-    print("Here1")
     try:
         if connection is not None:
             result_promise = connection.query(sql)
         else:
             js_function = js.Function('obj', '''
                 async function executeSqlDuckdb() {
                         let c = undefined
@@ -52,19 +51,17 @@
                         const result = await c.query(sql);
 
                         console.log('Result:', result);
                         return result
                     }
                 return executeSqlDuckdb()
             ''')
-            print("Here3")
             js_obj = js.Object() 
             js_obj.sql = sql
             js_obj.connection = connection
-            print("Here4")
 
             result_fut = js_function(js_obj)    # <class 'pyodide.webloop.PyodideFuture'>
         
         if return_future: 
             return result_fut
         else:
             return await future_to_df(result_fut)
```

## Comparing `jupylite_duckdb-0.0.5.dist-info/LICENSE` & `jupylite_duckdb-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.5.dist-info/METADATA` & `jupylite_duckdb-0.0.6.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupylite-duckdb
-Version: 0.0.5
+Version: 0.0.6
 Summary: Testing
 Home-page: https://github.com/iqmo-org/
 Author: iqmo
 Author-email: info@iqmo.com
 Keywords: jupyterlite duckdb wasm
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

