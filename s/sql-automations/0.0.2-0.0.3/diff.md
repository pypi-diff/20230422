# Comparing `tmp/sql_automations-0.0.2-py3-none-any.whl.zip` & `tmp/sql_automations-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 3628 bytes, number of entries: 12
--rw-r--r--  2.0 unx       40 b- defN 23-Apr-15 23:58 src/sql_automations/__init__.py
--rw-r--r--  2.0 unx      722 b- defN 23-Apr-16 19:11 src/sql_automations/sql_cli_tool.py
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-16 00:07 src/sql_automations/big_query/__init__.py
--rw-r--r--  2.0 unx      481 b- defN 23-Apr-16 00:15 src/sql_automations/big_query/execute_sql.py
--rw-r--r--  2.0 unx       34 b- defN 23-Apr-16 00:07 src/sql_automations/data_cleaning/__init__.py
+Zip file size: 4386 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-16 20:31 src/sql_automations/__init__.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Apr-21 22:40 src/sql_automations/output_data.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Apr-16 22:40 src/sql_automations/sql_cli_tool.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-16 19:32 src/sql_automations/big_query/__init__.py
+-rw-r--r--  2.0 unx      480 b- defN 23-Apr-21 21:34 src/sql_automations/big_query/execute_sql.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-16 19:32 src/sql_automations/data_cleaning/__init__.py
 -rw-r--r--  2.0 unx      131 b- defN 23-Apr-16 00:03 src/sql_automations/data_cleaning/read_data.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-16 19:13 sql_automations-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx       82 b- defN 23-Apr-16 19:13 sql_automations-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-16 19:13 sql_automations-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       78 b- defN 23-Apr-16 19:13 sql_automations-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-16 19:13 sql_automations-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1098 b- defN 23-Apr-16 19:13 sql_automations-0.0.2.dist-info/RECORD
-12 files, 2800 bytes uncompressed, 1716 bytes compressed:  38.7%
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 22:40 sql_automations-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx       82 b- defN 23-Apr-21 22:40 sql_automations-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 22:40 sql_automations-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      252 b- defN 23-Apr-21 22:40 sql_automations-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-21 22:40 sql_automations-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1188 b- defN 23-Apr-21 22:40 sql_automations-0.0.3.dist-info/RECORD
+13 files, 4452 bytes uncompressed, 2330 bytes compressed:  47.7%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: src/sql_automations/__init__.py
 Comment: 
 
+Filename: src/sql_automations/output_data.py
+Comment: 
+
 Filename: src/sql_automations/sql_cli_tool.py
 Comment: 
 
 Filename: src/sql_automations/big_query/__init__.py
 Comment: 
 
 Filename: src/sql_automations/big_query/execute_sql.py
@@ -12,26 +15,26 @@
 
 Filename: src/sql_automations/data_cleaning/__init__.py
 Comment: 
 
 Filename: src/sql_automations/data_cleaning/read_data.py
 Comment: 
 
-Filename: sql_automations-0.0.2.dist-info/LICENSE
+Filename: sql_automations-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: sql_automations-0.0.2.dist-info/METADATA
+Filename: sql_automations-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: sql_automations-0.0.2.dist-info/WHEEL
+Filename: sql_automations-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: sql_automations-0.0.2.dist-info/entry_points.txt
+Filename: sql_automations-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: sql_automations-0.0.2.dist-info/top_level.txt
+Filename: sql_automations-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sql_automations-0.0.2.dist-info/RECORD
+Filename: sql_automations-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/sql_automations/__init__.py

```diff
@@ -1,3 +0,0 @@
-00000000: 2320 6672 6f6d 202e 7371 6c5f 636c 695f  # from .sql_cli_
-00000010: 746f 6f6c 2069 6d70 6f72 7420 7371 6c5f  tool import sql_
-00000020: 636c 695f 746f 6f6c                      cli_tool
```

## src/sql_automations/sql_cli_tool.py

```diff
@@ -1,15 +1,14 @@
 """
-Script to read a external .sql file from a GCP connection CLI tool & return as pandas df
+A super lightweight SQL CLI tool for data processing
+Runs any external .sql file in directory against a data warehouse & outputs as a pandas data frame
 
-$ output-data --run=sample 
-$ sql_to_df --run=sample --dir=models
+$ return-dataframe --run=file_name --dir=folder_name
 
 """
-
 #!/usr/bin/env python3 
 import argparse
 from . big_query import execute_sql as ex
 from . data_cleaning import read_data as rd
 
 def run_sql():
     cli_parser = argparse.ArgumentParser()
@@ -25,8 +24,11 @@
     df = ex.execute_sql(filepath)
 
     return df
  
 if __name__ == '__main__':
     run_sql()
 
+# todo: update the run_sql function to be able to handle semi-colons or multiple statements 
+# todo: add -d and -r for non-verbose cli args
+# todo: add a new option that outputs just the table head instead of returning whole df
```

## src/sql_automations/big_query/__init__.py

```diff
@@ -1,3 +0,0 @@
-00000000: 2320 6672 6f6d 202e 6578 6563 7574 655f  # from .execute_
-00000010: 7371 6c20 696d 706f 7274 2065 7865 6375  sql import execu
-00000020: 7465 5f73 716c                           te_sql
```

## src/sql_automations/big_query/execute_sql.py

```diff
@@ -10,8 +10,7 @@
 
 def execute_sql(sql_file):
     query_job = client.query(sql_file)
     result = query_job.result()
     column_names = [field.name for field in result.schema]
     data = pd.DataFrame(data=[row.values() for row in result], columns=column_names)
     return data
-
```

## src/sql_automations/data_cleaning/__init__.py

```diff
@@ -1,3 +0,0 @@
-00000000: 2320 6672 6f6d 202e 7265 6164 5f64 6174  # from .read_dat
-00000010: 6120 696d 706f 7274 2072 6561 645f 6461  a import read_da
-00000020: 7461                                     ta
```

