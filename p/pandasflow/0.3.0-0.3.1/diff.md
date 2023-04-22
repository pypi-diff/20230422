# Comparing `tmp/pandasflow-0.3.0.tar.gz` & `tmp/pandasflow-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.3.0.tar", last modified: Sat Apr 22 17:39:48 2023, max compression
+gzip compressed data, was "pandasflow-0.3.1.tar", last modified: Sat Apr 22 18:32:10 2023, max compression
```

## Comparing `pandasflow-0.3.0.tar` & `pandasflow-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.207242 pandasflow-0.3.0/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.3.0/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-22 17:39:48.207242 pandasflow-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-16 13:51:54.000000 pandasflow-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.199264 pandasflow-0.3.0/pandasflow/
--rw-rw-rw-   0        0        0      284 2023-04-22 17:39:35.000000 pandasflow-0.3.0/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.203253 pandasflow-0.3.0/pandasflow/dev/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:26:55.000000 pandasflow-0.3.0/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      666 2023-04-17 12:24:03.000000 pandasflow-0.3.0/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      395 2023-04-16 13:51:54.000000 pandasflow-0.3.0/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      217 2023-04-17 10:11:12.000000 pandasflow-0.3.0/pandasflow/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.3.0/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.204250 pandasflow-0.3.0/pandasflow/services/
--rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.3.0/pandasflow/services/__init__.py
--rw-rw-rw-   0        0        0      173 2023-04-22 17:18:00.000000 pandasflow-0.3.0/pandasflow/services/get_column_name.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.205247 pandasflow-0.3.0/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.3.0/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2948 2023-04-22 17:39:05.000000 pandasflow-0.3.0/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3624 2023-04-22 17:30:45.000000 pandasflow-0.3.0/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.202256 pandasflow-0.3.0/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 17:39:48.208239 pandasflow-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.207242 pandasflow-0.3.0/test/
--rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.3.0/test/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.3.0/test/split_tt_test.py
--rw-rw-rw-   0        0        0      337 2023-04-22 17:29:25.000000 pandasflow-0.3.0/test/split_tvt_test.py
--rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.3.0/test/test_get_column_name.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.184682 pandasflow-0.3.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.3.1/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-22 18:32:10.184682 pandasflow-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-16 13:51:54.000000 pandasflow-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.177371 pandasflow-0.3.1/pandasflow/
+-rw-rw-rw-   0        0        0      284 2023-04-22 18:31:51.000000 pandasflow-0.3.1/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.180692 pandasflow-0.3.1/pandasflow/dev/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:26:55.000000 pandasflow-0.3.1/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-04-17 12:24:03.000000 pandasflow-0.3.1/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      395 2023-04-16 13:51:54.000000 pandasflow-0.3.1/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      217 2023-04-17 10:11:12.000000 pandasflow-0.3.1/pandasflow/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.3.1/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.181689 pandasflow-0.3.1/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.3.1/pandasflow/services/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.182687 pandasflow-0.3.1/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.3.1/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-22 18:32:03.000000 pandasflow-0.3.1/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3723 2023-04-22 18:29:28.000000 pandasflow-0.3.1/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.180692 pandasflow-0.3.1/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-22 18:32:10.000000 pandasflow-0.3.1/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 18:32:10.185679 pandasflow-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 18:32:10.184682 pandasflow-0.3.1/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.3.1/test/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.3.1/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      645 2023-04-22 18:31:38.000000 pandasflow-0.3.1/test/split_tvt_test.py
+-rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.3.1/test/test_get_column_name.py
```

### Comparing `pandasflow-0.3.0/LICENCE` & `pandasflow-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.0/PKG-INFO` & `pandasflow-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.3.0/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.3.1/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.0/pandasflow/reset_mi.py` & `pandasflow-0.3.1/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.3.0/pandasflow/split/train_test.py` & `pandasflow-0.3.1/pandasflow/split/train_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandasflow as pdf
-from pandasflow.services import get_column_name
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 def train_test(
 	*arrays,
 	test_size=None,
@@ -46,18 +45,15 @@
 		If None or 0 print all numbers after the decimal point
 	"""
 	
 	df = arrays[0]
 	
 	_stratify = stratify
 	if stratify != None:
-		if type(stratify) == pd.Series:
-			_stratify = df[get_column_name(stratify)]
-		elif type(stratify) == str:
-			_stratify = df[stratify]
+		_stratify = df[stratify]
 	
 	train, test = train_test_split(*arrays, train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=_stratify)
 	
 	train_pie = len(train) / len(arrays[0])
 	test_pie = len(test) / len(arrays[0])
 	
 	amount_len = len(train) + len(test)
@@ -85,21 +81,31 @@
 				   'test',
 				   '---',
 				   'Amount',
 				   'InitData']
 	
 	if target != None:
 		try:
-			table[target] = [train[target].mean(),
-							test[target].mean(),
-							'',
-							'',
-							df[target].mean()]
+			if type(target) is str:
+				table[target] = [train[target].mean(),
+								 test[target].mean(),
+								 '',
+								 '',
+								 df[target].mean()]
+			
+			
+			elif type(target) is list:
+				for col in list(target):
+					table[col] = [train[col].mean(),
+								  test[col].mean(),
+								  '',
+								  '',
+								  df[col].mean()]
 		except KeyError:
-			raise KeyError(target)
+			raise KeyError(*target)
 	
 	print(table)
 	
 	if amount_prop != 1.0 or len(arrays[0]) != amount_len:
 		print('---')
 		print('Some data is droped')
```

### Comparing `pandasflow-0.3.0/pandasflow/split/train_valid_test.py` & `pandasflow-0.3.1/pandasflow/split/train_valid_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandasflow as pdf
-from pandasflow.services import get_column_name
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 def train_valid_test(
 	*arrays,
 	test_size=None,
@@ -54,19 +53,15 @@
 	if test_size in [None, 0]:
 		test_size_pice = ((1 - train_size) / 2) / (1 - train_size)
 	else:
 		test_size_pice = test_size / (1 - train_size)
 	
 	_strat_col = None
 	_stratify = None
-	if stratify != None:
-		if type(stratify) == pd.Series:
-			_strat_col = get_column_name(stratify)
-		elif type(stratify) == str:
-			_strat_col = stratify
+	if stratify != None: _strat_col = stratify
 	
 	if _strat_col != None: _stratify = df[_strat_col]
 	train, valid_test = train_test_split(*arrays, train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=_stratify)
 	
 	if _strat_col != None: _stratify = valid_test[_strat_col]
 	valid, test = train_test_split(valid_test, test_size=test_size_pice, random_state=random_state, shuffle=shuffle, stratify=_stratify)
 	
@@ -98,22 +93,33 @@
 				 ''],
 		
 		
 	})
 	
 	if target != None:
 		try:
-			table[target] = [train[target].mean(),
-							valid[target].mean(),
-							test[target].mean(),
-							'',
-							'',
-							df[target].mean()]
+			if type(target) is str:
+				table[target] = [train[target].mean(),
+							  valid[target].mean(),
+							  test[target].mean(),
+							  '',
+							  '',
+							  df[target].mean()]
+			
+			
+			elif type(target) is list:
+				for col in list(target):
+					table[col] = [train[col].mean(),
+									valid[col].mean(),
+									test[col].mean(),
+									'',
+									'',
+									df[col].mean()]
 		except KeyError:
-			raise KeyError(target)
+			raise KeyError(*target)
 	
 	table.index = ['train',
 				   'valid',
 				   'test',
 				   '---',
 				   'Amount',
 				   'InitData']
```

### Comparing `pandasflow-0.3.0/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.3.1/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.3.0/pandasflow.egg-info/SOURCES.txt` & `pandasflow-0.3.1/pandasflow.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 pandasflow.egg-info/SOURCES.txt
 pandasflow.egg-info/dependency_links.txt
 pandasflow.egg-info/requires.txt
 pandasflow.egg-info/top_level.txt
 pandasflow/dev/__init__.py
 pandasflow/dev/err_mean_diff.py
 pandasflow/services/__init__.py
-pandasflow/services/get_column_name.py
 pandasflow/split/__init__.py
 pandasflow/split/train_test.py
 pandasflow/split/train_valid_test.py
 test/__init__.py
 test/split_tt_test.py
 test/split_tvt_test.py
 test/test_get_column_name.py
```

### Comparing `pandasflow-0.3.0/setup.py` & `pandasflow-0.3.1/setup.py`

 * *Files identical despite different names*

