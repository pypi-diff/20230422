# Comparing `tmp/jupylite_duckdb-0.0.16-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6471 bytes, number of entries: 10
+Zip file size: 7006 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      128 b- defN 23-Apr-21 01:44 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-22 16:19 jupylite_duckdb/_version.py
--rw-rw-rw-  2.0 fat     8901 b- defN 23-Apr-22 16:43 jupylite_duckdb/jdw.py
--rw-rw-rw-  2.0 fat     1643 b- defN 23-Apr-22 16:38 jupylite_duckdb/jdw_magic.py
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Apr-22 17:31 jupylite_duckdb/_version.py
+-rw-rw-rw-  2.0 fat     9097 b- defN 23-Apr-22 17:30 jupylite_duckdb/jdw.py
+-rw-rw-rw-  2.0 fat     1618 b- defN 23-Apr-22 17:28 jupylite_duckdb/jdw_magic.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Apr-22 14:33 jupylite_duckdb/magic.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 16:47 jupylite_duckdb-0.0.16.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1324 b- defN 23-Apr-22 16:47 jupylite_duckdb-0.0.16.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 16:47 jupylite_duckdb-0.0.16.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 16:47 jupylite_duckdb-0.0.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      840 b- defN 23-Apr-22 16:47 jupylite_duckdb-0.0.16.dist-info/RECORD
-10 files, 15440 bytes uncompressed, 5025 bytes compressed:  67.5%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2314 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      840 b- defN 23-Apr-22 17:32 jupylite_duckdb-0.0.17.dist-info/RECORD
+10 files, 16601 bytes uncompressed, 5560 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jupylite_duckdb/jdw_magic.py
 Comment: 
 
 Filename: jupylite_duckdb/magic.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.16.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.17.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.16.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.17.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.16.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.17.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.16.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.17.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.16.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.16"
+__version__="0.0.17"
```

## jupylite_duckdb/jdw.py

```diff
@@ -6,30 +6,32 @@
 # TODO Laundry List
 # - Pass arrow from duckdb_wasm to Python efficiently, altho dependent on pyodide pyarrow?
 # - Register pandas dataframes with duckdb_wasm: maybe use get_table_names to determine
 # what needs to be registered, then register
 # - Update connect to take connect(file)
 # - 
 
+CONNECTION = None
 
 async def future_to_df(result_promise):
     try:
         obj = await result_promise # <class 'pyodide.ffi.JsProxy'>
         a = obj.toArray()
         data = [dict(v) for v in a.object_values()] 
 
         df = DataFrame(data)
         return df
     except Exception as e:
         print(e)
         return None
     
-
-async def query(sql: str, connection: object = None, return_future= False) -> DataFrame:
+async def query(sql: str, connection = None, return_future= False) -> DataFrame:
     """Executes query in a standalone connection"""
+    if connection is None:
+        connection = CONNECTION # if both are None, then a temp db & connection is used
     try:
         if connection is not None:
             result_fut = connection.query(sql)
         else:
             js_function = js.Function('obj', '''
                 async function executeSqlDuckdb() {
                         let c = undefined
@@ -109,17 +111,20 @@
     ''')
 
     js_obj = js.Object()
     js_obj.connectionstr = ":memory:"
 
     result_promise = js_function(js_obj)
 
-    connection = await result_promise
+    thisconnection = await result_promise
 
-    return connection
+    global CONNECTION
+    CONNECTION = thisconnection
+    
+    return thisconnection
 
 def register_iiafes():
     syncWrapperConnect_js = js.Function('obj', '''
         function syncWrapperConnect(obj) {
             //delete globalThis.connection;
             (async () => {
                 async function executeSqlDuckdb() {
```

## jupylite_duckdb/jdw_magic.py

```diff
@@ -3,51 +3,46 @@
 from IPython.core.magic import register_line_magic, register_cell_magic
 from IPython.core import magic_arguments
 from IPython.display import display
 import ipywidgets as widgets
 import asyncio
 import jupylite_duckdb as jd
 import functools
+from IPython.core.getipython import get_ipython
 
 
-connection = None
 debug = False
 
-
-async def set_connection(obj, output):
-    global connection
-    with output: 
-        if debug:
-            display(f"Setting connection, type: {type(obj)}") # <class 'pyodide.ffi.JsProxy'>
-        connection = obj
-
-async def display_result(obj, output):
+async def display_result(result, output, outputvar = None):
     with output:
-        if obj is None:
-            display("Empty Result")
-        else:
-            if debug:
-                display(f"Output type: {type(obj)}")
-            display(obj)
+        try:
+            if result is None:
+                display("Empty Result")
+            else:
+                if debug:
+                    display(f"Output type: {type(result)}")
+                display(result)
+                if outputvar is not None: 
+                    get_ipython().user_ns[outputvar] = result  # type: ignore
+        except Exception as e:
+            display(e)
 
-@register_line_magic
+#@register_line_magic
 @register_cell_magic
 @magic_arguments.magic_arguments()
-@magic_arguments.argument('query', nargs="+", help="Query.", type=str)
+@magic_arguments.argument('-output', nargs=1, help="Output.", type=str)
+#@magic_arguments.argument('query', nargs="+", help="Query.", type=str)
 def dql(line = "", cell = ""):
-
+    outputvar = None
     if line:
         args = magic_arguments.parse_argstring(dql, line)
-        sql = ' '.join(args.query)
+        outputvar = args.output[0]
+        #sql = ' '.join(args.query)
+
+    sql = cell
 
-    elif cell:
-        sql= cell
     s_out = widgets.Output(layout={'border': '1px solid black'})
     display(s_out)
 
     with s_out:
-        if connection is None:
-            r = asyncio.get_event_loop().run_until_complete(jd.connect())
-            r.then(functools.partial(set_connection, output=s_out))
-        else:
-            r = asyncio.get_event_loop().run_until_complete(jd.query(sql=sql, return_future=False, connection=connection))
-            r.then(functools.partial(display_result, output=s_out))
+            r = asyncio.get_event_loop().run_until_complete(jd.query(sql=sql, return_future=False))
+            r.then(functools.partial(display_result, outputvar = outputvar, output=s_out))
```

## Comparing `jupylite_duckdb-0.0.16.dist-info/LICENSE` & `jupylite_duckdb-0.0.17.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.16.dist-info/RECORD` & `jupylite_duckdb-0.0.17.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 jupylite_duckdb/__init__.py,sha256=-Z_P6KBbWKDsMsnvKal14k3bbGljgWmFQPEvz7zrLVU,128
-jupylite_duckdb/_version.py,sha256=voboz3J88p7Vx98NFuG4uJFNokzGgZs1Hvr2BKx09sk,22
-jupylite_duckdb/jdw.py,sha256=Q88wi7zsKcGrs6HkqL48sEaHxiDBgZ_s45vtERKHHyg,8901
-jupylite_duckdb/jdw_magic.py,sha256=0vMohhY9K_yDh-UatzVOuWW98ZO6l791F7jaxbH--ZQ,1643
+jupylite_duckdb/_version.py,sha256=GEd_d0cJY-aeYoeZOG699Pnc0HUqdnua0qUTnNIzWpU,22
+jupylite_duckdb/jdw.py,sha256=P3zFLAew-KwZZhRm8ky7HFF7jaujDHJ8_BHd9X6KVKY,9097
+jupylite_duckdb/jdw_magic.py,sha256=3rFnfFdOwc_yUbkGkSeVDmaQw0JSa1koD3VyCqHo3XI,1618
 jupylite_duckdb/magic.py,sha256=okWgdHbcu0ul2BOYNdu9NHwRSoyAG_0m6RiGnw2Bj_k,979
-jupylite_duckdb-0.0.16.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.16.dist-info/METADATA,sha256=ko9_8HEqa3HMNDBpMWtzK7yzwbFeWBOZhV4yGzlN4EU,1324
-jupylite_duckdb-0.0.16.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.16.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.16.dist-info/RECORD,,
+jupylite_duckdb-0.0.17.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.17.dist-info/METADATA,sha256=KJOoPGLlUhs907vlD763KxGh0T5YtkS_3UiVm3QKHBw,2314
+jupylite_duckdb-0.0.17.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.17.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.17.dist-info/RECORD,,
```

