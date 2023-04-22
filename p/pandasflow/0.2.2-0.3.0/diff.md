# Comparing `tmp/pandasflow-0.2.2.tar.gz` & `tmp/pandasflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.2.2.tar", last modified: Sat Apr 22 16:09:53 2023, max compression
+gzip compressed data, was "pandasflow-0.3.0.tar", last modified: Sat Apr 22 17:39:48 2023, max compression
```

## Comparing `pandasflow-0.2.2.tar` & `pandasflow-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.326039 pandasflow-0.2.2/
--rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.2.2/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-22 16:09:53.326039 pandasflow-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-16 13:51:54.000000 pandasflow-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.319501 pandasflow-0.2.2/pandasflow/
--rw-rw-rw-   0        0        0      284 2023-04-22 16:08:39.000000 pandasflow-0.2.2/pandasflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.323175 pandasflow-0.2.2/pandasflow/dev/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:26:55.000000 pandasflow-0.2.2/pandasflow/dev/__init__.py
--rw-rw-rw-   0        0        0      666 2023-04-17 12:24:03.000000 pandasflow-0.2.2/pandasflow/dev/err_mean_diff.py
--rw-rw-rw-   0        0        0      395 2023-04-16 13:51:54.000000 pandasflow-0.2.2/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      217 2023-04-17 10:11:12.000000 pandasflow-0.2.2/pandasflow/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.2.2/pandasflow/reset_mi.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.324173 pandasflow-0.2.2/pandasflow/split/
--rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.2.2/pandasflow/split/__init__.py
--rw-rw-rw-   0        0        0     2622 2023-04-22 16:08:20.000000 pandasflow-0.2.2/pandasflow/split/train_test.py
--rw-rw-rw-   0        0        0     3087 2023-04-22 16:08:39.000000 pandasflow-0.2.2/pandasflow/split/train_valid_test.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.322470 pandasflow-0.2.2/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 16:09:53.326039 pandasflow-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.207242 pandasflow-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.3.0/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-22 17:39:48.207242 pandasflow-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-16 13:51:54.000000 pandasflow-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.199264 pandasflow-0.3.0/pandasflow/
+-rw-rw-rw-   0        0        0      284 2023-04-22 17:39:35.000000 pandasflow-0.3.0/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.203253 pandasflow-0.3.0/pandasflow/dev/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:26:55.000000 pandasflow-0.3.0/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-04-17 12:24:03.000000 pandasflow-0.3.0/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      395 2023-04-16 13:51:54.000000 pandasflow-0.3.0/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      217 2023-04-17 10:11:12.000000 pandasflow-0.3.0/pandasflow/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.3.0/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.204250 pandasflow-0.3.0/pandasflow/services/
+-rw-rw-rw-   0        0        0       89 2023-04-22 17:00:03.000000 pandasflow-0.3.0/pandasflow/services/__init__.py
+-rw-rw-rw-   0        0        0      173 2023-04-22 17:18:00.000000 pandasflow-0.3.0/pandasflow/services/get_column_name.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.205247 pandasflow-0.3.0/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.3.0/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2948 2023-04-22 17:39:05.000000 pandasflow-0.3.0/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3624 2023-04-22 17:30:45.000000 pandasflow-0.3.0/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.202256 pandasflow-0.3.0/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-22 17:39:48.000000 pandasflow-0.3.0/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 17:39:48.208239 pandasflow-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:39:48.207242 pandasflow-0.3.0/test/
+-rw-rw-rw-   0        0        0      102 2023-04-22 17:07:36.000000 pandasflow-0.3.0/test/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-22 17:38:11.000000 pandasflow-0.3.0/test/split_tt_test.py
+-rw-rw-rw-   0        0        0      337 2023-04-22 17:29:25.000000 pandasflow-0.3.0/test/split_tvt_test.py
+-rw-rw-rw-   0        0        0      161 2023-04-22 17:14:08.000000 pandasflow-0.3.0/test/test_get_column_name.py
```

### Comparing `pandasflow-0.2.2/LICENCE` & `pandasflow-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.2.2/PKG-INFO` & `pandasflow-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.2.2
+Version: 0.3.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.2.2/pandasflow/dev/err_mean_diff.py` & `pandasflow-0.3.0/pandasflow/dev/err_mean_diff.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.2.2/pandasflow/reset_mi.py` & `pandasflow-0.3.0/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.2.2/pandasflow/split/train_test.py` & `pandasflow-0.3.0/pandasflow/split/train_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import pandasflow as pdf
+from pandasflow.services import get_column_name
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 def train_test(
 	*arrays,
 	test_size=None,
 	train_size=0.8,
 	random_state=42,
 	shuffle=True,
 	stratify=None,
-	round_=None
+	round_=None,
+	target=None
 ):
 	"""
 	Split arrays or matrices into random train and test subsets.
 
 	Parameters
 	----------
 	*arrays : sequence of indexables with same length / shape[0]
@@ -39,54 +42,70 @@
 		See :term:`Glossary <random_state>`.
 
 	round_ : int, RandomState more 0 or None, default=None
 		Print the proportion of each array with rounding.
 		If None or 0 print all numbers after the decimal point
 	"""
 	
-	train, test = train_test_split(arrays[0], train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
+	df = arrays[0]
+	
+	_stratify = stratify
+	if stratify != None:
+		if type(stratify) == pd.Series:
+			_stratify = df[get_column_name(stratify)]
+		elif type(stratify) == str:
+			_stratify = df[stratify]
+	
+	train, test = train_test_split(*arrays, train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=_stratify)
 	
 	train_pie = len(train) / len(arrays[0])
 	test_pie = len(test) / len(arrays[0])
 	
 	amount_len = len(train) + len(test)
 	amount_prop = amount_len / len(arrays[0])
 	
 	if round_ not in [None, 'n', 'N'] and round_ > 0:
 		train_pie = round(train_pie, round_)
 		test_pie = round(test_pie, round_)
 	
 	table = pd.DataFrame({
-		# count
-		' ': [len(train), len(test), '', amount_len, len(arrays[0])],
-		# proportion
-		'  ': [train_pie, test_pie, '', amount_prop, '']})
+		'count': [len(train),
+			  len(test),
+			  '',
+			  amount_len,
+			  len(arrays[0])],
+		
+		'prop': [train_pie,
+			   test_pie,
+			   '',
+			   amount_prop,
+			   '']
+	})
+	
+	table.index = ['train',
+				   'test',
+				   '---',
+				   'Amount',
+				   'InitData']
+	
+	if target != None:
+		try:
+			table[target] = [train[target].mean(),
+							test[target].mean(),
+							'',
+							'',
+							df[target].mean()]
+		except KeyError:
+			raise KeyError(target)
 	
-	table.index = ['train', 'test', '---', 'Amount', 'InitData']
 	print(table)
 	
 	if amount_prop != 1.0 or len(arrays[0]) != amount_len:
 		print('---')
 		print('Some data is droped')
 	
 	return train, test
 
 
-if __name__ == "__main__":
-	train, test = train_test([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3,
-									train_size=0.6,
-									round_=2)
-
-''' return:
-
-train     19  0.58
-test      14  0.42
----
-Amount    33   1.0
-InitData  33
-'''
-
-
-
```

### Comparing `pandasflow-0.2.2/pandasflow/split/train_valid_test.py` & `pandasflow-0.3.0/pandasflow/split/train_valid_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import pandasflow as pdf
+from pandasflow.services import get_column_name
+
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
 def train_valid_test(
 	*arrays,
 	test_size=None,
 	train_size=0.6,
 	random_state=42,
 	shuffle=True,
 	stratify=None,
-	round_=None
+	round_=None,
+	target=None
 ):
 	"""
 	Split arrays or matrices into random train, valid and test subsets.
 
 	Parameters
 	----------
 	*arrays : sequence of indexables with same length / shape[0]
@@ -36,63 +40,88 @@
 		Controls the shuffling applied to the data before applying the split.
 		Pass an int for reproducible output across multiple function calls.
 		See :term:`Glossary <random_state>`.
 	
 	round_ : int, RandomState more 0 or None, default=None
 		Print the proportion of each array with rounding.
 		If None or 0 print all numbers after the decimal point
+	
+	target : None, str, pd.Series, default = None
+		Add new columns with mean float proportion for tvt and df
 	"""
 	
+	df = arrays[0]
+	
 	if test_size in [None, 0]:
 		test_size_pice = ((1 - train_size) / 2) / (1 - train_size)
 	else:
 		test_size_pice = test_size / (1 - train_size)
 	
-	train, valid_test = train_test_split(arrays[0], train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
-	valid, test = train_test_split(valid_test, test_size=test_size_pice, random_state=random_state, shuffle=shuffle, stratify=stratify)
-	
-	train_pie = len(train) / len(arrays[0])
-	valid_pie = len(valid) / len(arrays[0])
-	test_pie = len(test) / len(arrays[0])
+	_strat_col = None
+	_stratify = None
+	if stratify != None:
+		if type(stratify) == pd.Series:
+			_strat_col = get_column_name(stratify)
+		elif type(stratify) == str:
+			_strat_col = stratify
+	
+	if _strat_col != None: _stratify = df[_strat_col]
+	train, valid_test = train_test_split(*arrays, train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=_stratify)
+	
+	if _strat_col != None: _stratify = valid_test[_strat_col]
+	valid, test = train_test_split(valid_test, test_size=test_size_pice, random_state=random_state, shuffle=shuffle, stratify=_stratify)
+	
+	train_pie = len(train) / len(df)
+	valid_pie = len(valid) / len(df)
+	test_pie = len(test) / len(df)
 	
 	amount_len = len(train) + len(valid) + len(test)
-	amount_prop = amount_len / len(arrays[0])
+	amount_prop = amount_len / len(df)
 	
 	if round_ not in [None, 'n', 'N'] and round_ > 0:
 		train_pie = round(train_pie, round_)
 		valid_pie = round(valid_pie, round_)
 		test_pie = round(test_pie, round_)
 	
 	table = pd.DataFrame({
-		#count
-		' ': [len(train), len(valid), len(test), '', amount_len, len(arrays[0])],
-		#proportion
-		'  ': [train_pie, valid_pie, test_pie, '', amount_prop, '']})
+		'count': [len(train),
+				len(valid),
+				len(test),
+				'',
+				amount_len,
+				len(df)],
+		
+		'prop': [train_pie,
+				 valid_pie,
+				 test_pie,
+				 '',
+				 amount_prop,
+				 ''],
+		
+		
+	})
+	
+	if target != None:
+		try:
+			table[target] = [train[target].mean(),
+							valid[target].mean(),
+							test[target].mean(),
+							'',
+							'',
+							df[target].mean()]
+		except KeyError:
+			raise KeyError(target)
 	
 	table.index = ['train',
 				   'valid',
 				   'test',
 				   '---',
 				   'Amount',
 				   'InitData']
 	print(table)
 	
 	
-	if amount_prop != 1.0 or len(arrays[0]) != amount_len:
+	if amount_prop != 1.0 or len(df) != amount_len:
 		print('---')
 		print('Some data is droped')
 	
-	return train, valid, test
-
-
-if __name__ == "__main__":
-	train, valid, test = train_valid_test([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3, round_=2)
-
-'''return:
-
-train     19  0.58
-valid      7  0.21
-test       7  0.21
----
-Amount    33   1.0
-InitData  33
-'''
+	return train, valid, test
```

### Comparing `pandasflow-0.2.2/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.3.0/pandasflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.2.2
+Version: 0.3.0
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.2.2/setup.py` & `pandasflow-0.3.0/setup.py`

 * *Files identical despite different names*

