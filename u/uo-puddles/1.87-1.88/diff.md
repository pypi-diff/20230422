# Comparing `tmp/uo_puddles-1.87.tar.gz` & `tmp/uo_puddles-1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-1.87.tar", last modified: Wed Mar 15 16:38:12 2023, max compression
+gzip compressed data, was "uo_puddles-1.88.tar", last modified: Fri Apr 21 22:32:05 2023, max compression
```

## Comparing `uo_puddles-1.87.tar` & `uo_puddles-1.88.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:38:12.130773 uo_puddles-1.87/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-15 16:37:59.000000 uo_puddles-1.87/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-15 16:38:12.130773 uo_puddles-1.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-15 16:37:59.000000 uo_puddles-1.87/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-15 16:37:59.000000 uo_puddles-1.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 16:38:12.130773 uo_puddles-1.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-15 16:37:59.000000 uo_puddles-1.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:38:12.130773 uo_puddles-1.87/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-15 16:37:59.000000 uo_puddles-1.87/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-03-15 16:37:59.000000 uo_puddles-1.87/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-03-15 16:37:59.000000 uo_puddles-1.87/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-03-15 16:37:59.000000 uo_puddles-1.87/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-03-15 16:37:59.000000 uo_puddles-1.87/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-15 16:37:59.000000 uo_puddles-1.87/uo_puddles/gremcat_oo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:38:12.130773 uo_puddles-1.87/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-15 16:38:12.000000 uo_puddles-1.87/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-15 16:38:12.000000 uo_puddles-1.87/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 16:38:12.000000 uo_puddles-1.87/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 16:38:12.000000 uo_puddles-1.87/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:32:05.991790 uo_puddles-1.88/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-21 22:31:51.000000 uo_puddles-1.88/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 22:32:05.991790 uo_puddles-1.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 22:31:51.000000 uo_puddles-1.88/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 22:31:51.000000 uo_puddles-1.88/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:32:05.991790 uo_puddles-1.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-21 22:31:51.000000 uo_puddles-1.88/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:32:05.991790 uo_puddles-1.88/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26237 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/gremcat_oo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:32:05.991790 uo_puddles-1.88/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-1.87/LICENSE.txt` & `uo_puddles-1.88/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.87/setup.py` & `uo_puddles-1.88/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="1.87",    #also change pypi_version variable at top of library
+    version="1.88",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-1.87/uo_puddles/cis423.py` & `uo_puddles-1.88/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.87/uo_puddles/good_ai.py` & `uo_puddles-1.88/uo_puddles/good_ai_22.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import matplotlib.pyplot as plt  #concern this is in colab context which is oldish
 
 from sklearn.base import BaseEstimator, TransformerMixin
 
 from sklearn.pipeline import Pipeline
 import pandas as pd
-pd.set_option('mode.chained_assignment', None)  #https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
-
 import numpy as np
-import math
 import random
 from sklearn.model_selection import train_test_split
 from sklearn.impute import KNNImputer
 from sklearn.preprocessing import MinMaxScaler
 
 from sklearn.experimental import enable_halving_search_cv
 from sklearn.model_selection import HalvingGridSearchCV
@@ -19,43 +16,31 @@
 from sklearn.metrics import precision_score, recall_score, f1_score, accuracy_score
 
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.metrics import f1_score#, balanced_accuracy_score, precision_score, recall_score
 from sklearn.model_selection import train_test_split
 from sklearn.linear_model import LogisticRegressionCV
 
-from random import sample, seed, choices
-def the_claw():
-  class_list = ['Smith', 'Jones']
-  return sample(class_list,1)[0]
-
 def hello():
   print('Welcome to AI for Good')
-
-def up_range(n):
-  return list(range(n))
-
+  
 import builtins
 import types
-
-#use: @up_no_globals(globals())  #globals is function that returns *current* globals as dict
-#DANGER DANGER: this fails on forward refs. Assumes helper functions all defined before main function. If not will get spurious error.
-def up_no_globals(gfn:dict):
-
-  def wrap(f):
-    new_globals = {'__builtins__': builtins} 
-    # removing keys from globals() storing global values in old_globals
-    for key, val in gfn.items():
+def up_no_globals(f):
+  '''
+  A function decorator that prevents functions from looking up variables in outer scope.
+  '''
+  new_globals = {'__builtins__': builtins} 
+  # removing keys from globals() storing global values in old_globals
+  for key, val in globals().items():
       if  callable(val):
           new_globals[key] = val
-    new_f = types.FunctionType(f.__code__, globals=new_globals, argdefs=f.__defaults__)
-    new_f.__annotations__ = f.__annotations__ # for some reason annotations aren't copied over
-    return new_f
-
-  return wrap
+  new_f = types.FunctionType(f.__code__, globals=new_globals, argdefs=f.__defaults__)
+  new_f.__annotations__ = f.__annotations__ # for some reason annotations aren't copied over
+  return new_f
 
 def up_lottery(student_list):
   random_students = random.sample(student_list, len(student_list))
   table_table = pd.DataFrame(columns=['Table'], index=random_students + ['Blank']*(20-len(student_list)))
   table_table['Table'] = [1]*4 + [2]*4 + [3]*4 + [4]*4 + [5]*4
   return table_table
   
@@ -239,15 +224,15 @@
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: Expecting a table but instead got a {type(table)}!'
   assert isinstance(file_name, str), f'Puddles says: Expecting file_name to be a string but got a {type(file_name)}!'
 
   if not file_name.endswith('.csv'): file_name += '.csv'
   table.to_csv(file_name, index=False)
   return None
 
-def up_knn_probability(table, new_row, k):
+def up_knn(table, new_row, k):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
   assert table.isna().sum().sum()==0, f'Puddles says: table still contains NaN values.'
   for column in table.columns:
     col_list = up_get_column(table, column)
     assert not any([isinstance(x,str) for x in col_list]), f'Puddles says: column {column} contains string values.'
   assert isinstance(new_row, list), f'Puddles says: new_row must be a list but is of type {type(new_row)}'
   assert all([not isinstance(x,str) for x in new_row]), f'Puddles says: expecting a list of numbers but list includes a string!'
@@ -260,15 +245,15 @@
   feature_table = table.drop(columns=last_c)
   labels = table[last_c].to_list()
   assert all([x in [0,1] for x in labels]), f'Puddles says: the target column {last_c} should be binary. Reminder: the target column should be the last column in table.'
   from sklearn.neighbors import KNeighborsClassifier
   neigh = KNeighborsClassifier(n_neighbors=k)
   neigh.fit(feature_table.to_numpy(), labels)
   p = neigh.predict_proba([new_row])
-  return p[0]
+  return [1 if p[0][1]>=.5 else 0, p[0].tolist()]
 
 def up_knn_full(train_table, test_table, target_col, k):
   assert isinstance(train_table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(train_table)}!'
   assert isinstance(test_table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(test_table)}!'
   assert train_table.isna().sum().sum()==0, f'Puddles says: train_table still contains NaN values.'
   assert test_table.isna().sum().sum()==0, f'Puddles says: test_table still contains NaN values.'
   for column in train_table.columns:
@@ -279,15 +264,15 @@
   assert k<=len(train_table), f'Puddles says: k must be <= length of train_table'
   assert all([x in [0,1] for x in up_get_column(train_table,target_col)]), f'Puddles says: the target column {target_col} should be binary.'
 
   from sklearn.neighbors import KNeighborsClassifier
   neigh = KNeighborsClassifier(n_neighbors=k)
   neigh.fit(train_table.drop(columns=target_col).to_numpy(), up_get_column(train_table,target_col))
   p = neigh.predict_proba(up_table_to_list(test_table.drop(columns=target_col)))
-  return p.tolist()  #looks a little strange
+  return p.tolist()
 
 def up_zip_lists(list1, list2):
   if not isinstance(list1, list):
     try:
       list1 = list(list1)
     except:
       assert False, f'Puddles says: Expecting a list for list1 but instead got a {type(list1)}!'
@@ -352,20 +337,14 @@
                                   class_names=['No', 'Yes'],
                                   filled=True)
 
   # Draw graph
   graph = graphviz.Source(dot_data, format="png") 
   return graph
 
-def up_get_random_rows(table, fraction, the_seed):
-  assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
-  assert 0<fraction<=1, f'Puddles says: fraction must be 0<fraction<=1 but is {fraction}.'
-  random_table = table.sample(frac=fraction, random_state=the_seed)
-  return random_table
-
 def up_list_column_names(table):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
   return table.columns.to_list()
 
 def up_product(value_list):
   assert isinstance(value_list, list)
   assert all([type(v)!=str for v in value_list])
@@ -555,8 +534,7 @@
   return None
 
 def stats_please(*, table):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
   return table.describe(include='all').T
 
 
-
```

### Comparing `uo_puddles-1.87/uo_puddles/good_ai_22.py` & `uo_puddles-1.88/uo_puddles/good_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import matplotlib.pyplot as plt  #concern this is in colab context which is oldish
 
 from sklearn.base import BaseEstimator, TransformerMixin
 
 from sklearn.pipeline import Pipeline
 import pandas as pd
+pd.set_option('mode.chained_assignment', None)  #https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
+
 import numpy as np
+import math
 import random
 from sklearn.model_selection import train_test_split
 from sklearn.impute import KNNImputer
 from sklearn.preprocessing import MinMaxScaler
 
 from sklearn.experimental import enable_halving_search_cv
 from sklearn.model_selection import HalvingGridSearchCV
@@ -16,31 +19,60 @@
 from sklearn.metrics import precision_score, recall_score, f1_score, accuracy_score
 
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.metrics import f1_score#, balanced_accuracy_score, precision_score, recall_score
 from sklearn.model_selection import train_test_split
 from sklearn.linear_model import LogisticRegressionCV
 
+import warnings
+
+class puddlesWarning(Warning):
+  def __init__(self, message):
+      self.message = message
+  def __str__(self):
+      return repr(self.message)
+    
+def up_ignore_warnings(yes_no):
+  assert isinstance(yes_no, bool)
+  if yes_no: warnings.filterwarnings("ignore", category=puddlesWarning)
+  else: foo = warnings.filterwarnings("always", category=puddlesWarning)
+  return None
+
+up_ignore_warnings(False)  #start out with warnings
+
+from random import sample, seed, choices
+def the_claw():
+  class_list = ['Smith', 'Jones']
+  return sample(class_list,1)[0]
+
 def hello():
+  warnings.warn('Puddles says this is just for testing', puddlesWarning)
   print('Welcome to AI for Good')
-  
+
+def up_range(n):
+  return list(range(n))
+
 import builtins
 import types
-def up_no_globals(f):
-  '''
-  A function decorator that prevents functions from looking up variables in outer scope.
-  '''
-  new_globals = {'__builtins__': builtins} 
-  # removing keys from globals() storing global values in old_globals
-  for key, val in globals().items():
+
+#use: @up_no_globals(globals())  #globals is function that returns *current* globals as dict
+#DANGER DANGER: this fails on forward refs. Assumes helper functions all defined before main function. If not will get spurious error.
+def up_no_globals(gfn:dict):
+
+  def wrap(f):
+    new_globals = {'__builtins__': builtins} 
+    # removing keys from globals() storing global values in old_globals
+    for key, val in gfn.items():
       if  callable(val):
           new_globals[key] = val
-  new_f = types.FunctionType(f.__code__, globals=new_globals, argdefs=f.__defaults__)
-  new_f.__annotations__ = f.__annotations__ # for some reason annotations aren't copied over
-  return new_f
+    new_f = types.FunctionType(f.__code__, globals=new_globals, argdefs=f.__defaults__)
+    new_f.__annotations__ = f.__annotations__ # for some reason annotations aren't copied over
+    return new_f
+
+  return wrap
 
 def up_lottery(student_list):
   random_students = random.sample(student_list, len(student_list))
   table_table = pd.DataFrame(columns=['Table'], index=random_students + ['Blank']*(20-len(student_list)))
   table_table['Table'] = [1]*4 + [2]*4 + [3]*4 + [4]*4 + [5]*4
   return table_table
   
@@ -93,28 +125,28 @@
   legal_conditions = {'equals':'==', 'not equals':'!=', '>':'>', '<':'<'}
   assert condition in legal_conditions.keys(), f'Puddles says: condition {condition} incorrect. Must be one of {list(legal_conditions.keys())}'
   assert column_name in table.columns, f'Puddles says: column_name {column_name} is not legal. Check spelling and case. Here are legal columns: {table.columns.to_list()}'
   if 'equals' not in condition and isinstance(value, str):
     assert False, f'Puddles says: expecting value to be a number but is string instead'
 
   if 'equals' in condition and value not in table[column_name].to_list():
-      print(f'Puddles warning: {value} does not appear in {column_name}')
+      warnings.warn(f'Puddles warning: {value} does not appear in {column_name}',puddlesWarning)
 
   op = legal_conditions[condition]
 
   if isinstance(value,int) or isinstance(value,float):
     value = str(value)
   elif isinstance(value,str):
     value = f'"{value}"'
   else:
     assert False, f'Puddles says: tell Steve he has a bug with {value}'
 
   new_table = table.query(f'`{column_name}`' + op + value)
   if len(new_table)==0:
-    print(f'Puddles warning: resulting table is empty')
+    warnings.warn(f'Puddles warning: the new table is empty',puddlesWarning)
 
   return new_table
 
 def up_st_dev(a_list_of_numbers):
   assert isinstance(a_list_of_numbers, list), f'Puddles says: expecting a list but instead got a {type(a_list_of_numbers)}!'
   assert all([not isinstance(x,str) for x in a_list_of_numbers]), f'Puddles says: expecting a list of numbers but list includes a string!'
 
@@ -138,19 +170,19 @@
   assert column_name in table.columns, f'Puddles says: column_name {column_name} is not legal. Check spelling and case. Here are legal columns: {table.columns.to_list()}'
   assert isinstance(mapping_dict, dict), f'Puddles says: expecting mapping_dict to be a dictionary but instead got a {type(mapping_dict)}!'
 
   column_values = table[column_name].to_list()
   mapping_keys = list(mapping_dict.keys())
   keys_unaccounted = set(mapping_keys).difference(set(column_values))
   if keys_unaccounted:
-    print(f'Puddles warning: these keys {keys_unaccounted} do not match any values in the column {column_name}.')
+    warnings.warn(f'Puddles warning: these keys {keys_unaccounted} do not match any values in the column {column_name}.', puddlesWarning)
 
   values_unaccounted = set(column_values).difference(set(mapping_keys))
   if values_unaccounted:
-    print(f'Puddles warning: these values {values_unaccounted} are missing a mapping.')
+    warnings.warn(f'Puddles warning: these values {values_unaccounted} are missing a mapping.', puddlesWarning)
 
   new_table = table.copy()
   new_table[column_name] = table[column_name].replace(mapping_dict)
 
   return new_table
 
 def up_get_column_types(table):
@@ -210,29 +242,29 @@
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: Expecting a table but instead got a {type(table)}!'
   assert isinstance(new_values, list), f'Puddles says: Expecting a list but instead got a {type(new_values)}!'
   assert len(new_values)==len(table), f'Puddles says: length of list is {len(new_values)} but length of table is {len(table)}. Mismatch!'
   
   new_table = table.copy()
   new_table[column_name] = new_values
   if column_name not in table.columns.to_list():
-    print(f'\n\nPuddles warning: column_name {column_name} is not part of current table so adding new column.\n\n\n')
+    warnings.warn(f'Puddles warning: column_name {column_name} is not part of current table so adding new column.', puddlesWarning)
     new_cols = [column_name] + [col for col in new_table.columns if col != column_name] 
     new_table = new_table[new_cols]
   return new_table
 
 
 def up_write_table(table, file_name):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: Expecting a table but instead got a {type(table)}!'
   assert isinstance(file_name, str), f'Puddles says: Expecting file_name to be a string but got a {type(file_name)}!'
 
   if not file_name.endswith('.csv'): file_name += '.csv'
   table.to_csv(file_name, index=False)
   return None
 
-def up_knn(table, new_row, k):
+def up_knn_probability(table, new_row, k):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
   assert table.isna().sum().sum()==0, f'Puddles says: table still contains NaN values.'
   for column in table.columns:
     col_list = up_get_column(table, column)
     assert not any([isinstance(x,str) for x in col_list]), f'Puddles says: column {column} contains string values.'
   assert isinstance(new_row, list), f'Puddles says: new_row must be a list but is of type {type(new_row)}'
   assert all([not isinstance(x,str) for x in new_row]), f'Puddles says: expecting a list of numbers but list includes a string!'
@@ -245,15 +277,15 @@
   feature_table = table.drop(columns=last_c)
   labels = table[last_c].to_list()
   assert all([x in [0,1] for x in labels]), f'Puddles says: the target column {last_c} should be binary. Reminder: the target column should be the last column in table.'
   from sklearn.neighbors import KNeighborsClassifier
   neigh = KNeighborsClassifier(n_neighbors=k)
   neigh.fit(feature_table.to_numpy(), labels)
   p = neigh.predict_proba([new_row])
-  return [1 if p[0][1]>=.5 else 0, p[0].tolist()]
+  return p[0].tolist()
 
 def up_knn_full(train_table, test_table, target_col, k):
   assert isinstance(train_table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(train_table)}!'
   assert isinstance(test_table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(test_table)}!'
   assert train_table.isna().sum().sum()==0, f'Puddles says: train_table still contains NaN values.'
   assert test_table.isna().sum().sum()==0, f'Puddles says: test_table still contains NaN values.'
   for column in train_table.columns:
@@ -264,15 +296,15 @@
   assert k<=len(train_table), f'Puddles says: k must be <= length of train_table'
   assert all([x in [0,1] for x in up_get_column(train_table,target_col)]), f'Puddles says: the target column {target_col} should be binary.'
 
   from sklearn.neighbors import KNeighborsClassifier
   neigh = KNeighborsClassifier(n_neighbors=k)
   neigh.fit(train_table.drop(columns=target_col).to_numpy(), up_get_column(train_table,target_col))
   p = neigh.predict_proba(up_table_to_list(test_table.drop(columns=target_col)))
-  return p.tolist()
+  return p.tolist()  #looks a little strange
 
 def up_zip_lists(list1, list2):
   if not isinstance(list1, list):
     try:
       list1 = list(list1)
     except:
       assert False, f'Puddles says: Expecting a list for list1 but instead got a {type(list1)}!'
@@ -337,14 +369,20 @@
                                   class_names=['No', 'Yes'],
                                   filled=True)
 
   # Draw graph
   graph = graphviz.Source(dot_data, format="png") 
   return graph
 
+def up_get_random_rows(table, fraction, the_seed):
+  assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
+  assert 0<fraction<=1, f'Puddles says: fraction must be 0<fraction<=1 but is {fraction}.'
+  random_table = table.sample(frac=fraction, random_state=the_seed)
+  return random_table
+
 def up_list_column_names(table):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
   return table.columns.to_list()
 
 def up_product(value_list):
   assert isinstance(value_list, list)
   assert all([type(v)!=str for v in value_list])
@@ -534,7 +572,8 @@
   return None
 
 def stats_please(*, table):
   assert isinstance(table, pd.core.frame.DataFrame), f'Puddles says: expecting a pandas dataframe but instead got a {type(table)}!'
   return table.describe(include='all').T
 
 
+
```

### Comparing `uo_puddles-1.87/uo_puddles/gremcat_df.py` & `uo_puddles-1.88/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.87/uo_puddles/gremcat_oo.py` & `uo_puddles-1.88/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

