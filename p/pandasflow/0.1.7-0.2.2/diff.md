# Comparing `tmp/pandasflow-0.1.7.tar.gz` & `tmp/pandasflow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasflow-0.1.7.tar", last modified: Sun Apr 16 13:34:06 2023, max compression
+gzip compressed data, was "pandasflow-0.2.2.tar", last modified: Sat Apr 22 16:09:53 2023, max compression
```

## Comparing `pandasflow-0.1.7.tar` & `pandasflow-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:34:06.169701 pandasflow-0.1.7/
--rw-rw-rw-   0        0        0    35823 2023-04-09 14:36:14.000000 pandasflow-0.1.7/LICENCE
--rw-rw-rw-   0        0        0      694 2023-04-16 13:34:06.169701 pandasflow-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-04-16 10:16:48.000000 pandasflow-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 13:34:06.165658 pandasflow-0.1.7/pandasflow/
--rw-rw-rw-   0        0        0      343 2023-04-16 13:32:33.000000 pandasflow-0.1.7/pandasflow/__init__.py
--rw-rw-rw-   0        0        0      395 2023-04-15 15:57:08.000000 pandasflow-0.1.7/pandasflow/get_import.py
--rw-rw-rw-   0        0        0      217 2023-04-14 13:37:47.000000 pandasflow-0.1.7/pandasflow/mean_error.py
--rw-rw-rw-   0        0        0      614 2023-04-13 15:00:40.000000 pandasflow-0.1.7/pandasflow/reset_mi.py
--rw-rw-rw-   0        0        0     2690 2023-04-16 13:29:59.000000 pandasflow-0.1.7/pandasflow/train_test_split.py
--rw-rw-rw-   0        0        0     2936 2023-04-16 13:25:55.000000 pandasflow-0.1.7/pandasflow/train_valid_test_split.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:34:06.168738 pandasflow-0.1.7/pandasflow.egg-info/
--rw-rw-rw-   0        0        0      694 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-16 13:34:06.000000 pandasflow-0.1.7/pandasflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 13:34:06.169701 pandasflow-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-04-16 13:33:39.000000 pandasflow-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.326039 pandasflow-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 13:51:54.000000 pandasflow-0.2.2/LICENCE
+-rw-rw-rw-   0        0        0      694 2023-04-22 16:09:53.326039 pandasflow-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-04-16 13:51:54.000000 pandasflow-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.319501 pandasflow-0.2.2/pandasflow/
+-rw-rw-rw-   0        0        0      284 2023-04-22 16:08:39.000000 pandasflow-0.2.2/pandasflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.323175 pandasflow-0.2.2/pandasflow/dev/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:26:55.000000 pandasflow-0.2.2/pandasflow/dev/__init__.py
+-rw-rw-rw-   0        0        0      666 2023-04-17 12:24:03.000000 pandasflow-0.2.2/pandasflow/dev/err_mean_diff.py
+-rw-rw-rw-   0        0        0      395 2023-04-16 13:51:54.000000 pandasflow-0.2.2/pandasflow/get_import.py
+-rw-rw-rw-   0        0        0      217 2023-04-17 10:11:12.000000 pandasflow-0.2.2/pandasflow/mean_error.py
+-rw-rw-rw-   0        0        0      614 2023-04-16 13:51:54.000000 pandasflow-0.2.2/pandasflow/reset_mi.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.324173 pandasflow-0.2.2/pandasflow/split/
+-rw-rw-rw-   0        0        0      120 2023-04-22 15:43:30.000000 pandasflow-0.2.2/pandasflow/split/__init__.py
+-rw-rw-rw-   0        0        0     2622 2023-04-22 16:08:20.000000 pandasflow-0.2.2/pandasflow/split/train_test.py
+-rw-rw-rw-   0        0        0     3087 2023-04-22 16:08:39.000000 pandasflow-0.2.2/pandasflow/split/train_valid_test.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:09:53.322470 pandasflow-0.2.2/pandasflow.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-22 16:09:53.000000 pandasflow-0.2.2/pandasflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 16:09:53.326039 pandasflow-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-04-16 13:51:54.000000 pandasflow-0.2.2/setup.py
```

### Comparing `pandasflow-0.1.7/LICENCE` & `pandasflow-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `pandasflow-0.1.7/PKG-INFO` & `pandasflow-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.1.7
+Version: 0.2.2
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.1.7/pandasflow/reset_mi.py` & `pandasflow-0.2.2/pandasflow/reset_mi.py`

 * *Files identical despite different names*

### Comparing `pandasflow-0.1.7/pandasflow/train_test_split.py` & `pandasflow-0.2.2/pandasflow/split/train_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
-def train_test_split_(
+def train_test(
 	*arrays,
 	test_size=None,
 	train_size=0.8,
 	random_state=42,
 	shuffle=True,
 	stratify=None,
 	round_=None
@@ -39,19 +39,14 @@
 		See :term:`Glossary <random_state>`.
 
 	round_ : int, RandomState more 0 or None, default=None
 		Print the proportion of each array with rounding.
 		If None or 0 print all numbers after the decimal point
 	"""
 	
-	if test_size in [None, 0]:
-		test_size_pice = ((1 - train_size) / 2) / (1 - train_size)
-	else:
-		test_size_pice = test_size / (1 - train_size)
-	
 	train, test = train_test_split(arrays[0], train_size=train_size, random_state=random_state, shuffle=shuffle, stratify=stratify)
 	
 	train_pie = len(train) / len(arrays[0])
 	test_pie = len(test) / len(arrays[0])
 	
 	amount_len = len(train) + len(test)
 	amount_prop = amount_len / len(arrays[0])
@@ -73,18 +68,25 @@
 		print('---')
 		print('Some data is droped')
 	
 	return train, test
 
 
 if __name__ == "__main__":
-	train, test = train_test_split_([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3,
+	train, test = train_test([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3,
 									train_size=0.6,
 									round_=2)
 
+''' return:
 
+train     19  0.58
+test      14  0.42
+---
+Amount    33   1.0
+InitData  33
+'''
```

### Comparing `pandasflow-0.1.7/pandasflow/train_valid_test_split.py` & `pandasflow-0.2.2/pandasflow/split/train_valid_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from sklearn.model_selection import train_test_split
 
-def train_valid_test_split(
+def train_valid_test(
 	*arrays,
 	test_size=None,
 	train_size=0.6,
 	random_state=42,
 	shuffle=True,
 	stratify=None,
 	round_=None
@@ -64,19 +64,35 @@
 	
 	table = pd.DataFrame({
 		#count
 		' ': [len(train), len(valid), len(test), '', amount_len, len(arrays[0])],
 		#proportion
 		'  ': [train_pie, valid_pie, test_pie, '', amount_prop, '']})
 	
-	table.index = ['train', 'valid', 'test', '---', 'Amount', 'InitData']
+	table.index = ['train',
+				   'valid',
+				   'test',
+				   '---',
+				   'Amount',
+				   'InitData']
 	print(table)
 	
+	
 	if amount_prop != 1.0 or len(arrays[0]) != amount_len:
 		print('---')
 		print('Some data is droped')
 	
 	return train, valid, test
 
 
 if __name__ == "__main__":
-	train, valid, test = train_valid_test_split([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3, round_=2)
+	train, valid, test = train_valid_test([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] * 3, round_=2)
+
+'''return:
+
+train     19  0.58
+valid      7  0.21
+test       7  0.21
+---
+Amount    33   1.0
+InitData  33
+'''
```

### Comparing `pandasflow-0.1.7/pandasflow.egg-info/PKG-INFO` & `pandasflow-0.2.2/pandasflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasflow
-Version: 0.1.7
+Version: 0.2.2
 Summary: A set of custom python modules for friendly workflow on pandas
 Home-page: https://github.com/Priboy313/pandasflow
 Author: Priboy313
 Author-email: Priboy313@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pandasflow-0.1.7/setup.py` & `pandasflow-0.2.2/setup.py`

 * *Files identical despite different names*

