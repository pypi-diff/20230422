# Comparing `tmp/proceduraldata-1.1.3.tar.gz` & `tmp/proceduraldata-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proceduraldata-1.1.3.tar", last modified: Sun Nov 27 08:22:29 2022, max compression
+gzip compressed data, was "proceduraldata-2.0.4.tar", last modified: Sat Apr 22 09:24:54 2023, max compression
```

## Comparing `proceduraldata-1.1.3.tar` & `proceduraldata-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2022-11-27 08:22:29.389280 proceduraldata-1.1.3/
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     1072 2022-04-05 11:37:57.000000 proceduraldata-1.1.3/LICENSE
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     2856 2022-11-27 08:22:29.389280 proceduraldata-1.1.3/PKG-INFO
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     1342 2022-10-16 10:00:46.000000 proceduraldata-1.1.3/README.rst
-drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2022-11-27 08:22:29.381279 proceduraldata-1.1.3/pdata/
--rw-rw-r--   0 govenius  (1000) govenius  (1000)      305 2022-04-05 11:19:21.000000 proceduraldata-1.1.3/pdata/__init__.py
--rw-rw-r--   0 govenius  (1000) govenius  (1000)       53 2022-11-27 06:48:14.000000 proceduraldata-1.1.3/pdata/_metadata.py
-drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2022-11-27 08:22:29.385280 proceduraldata-1.1.3/pdata/analysis/
--rwxrwxr-x   0 govenius  (1000) govenius  (1000)      306 2022-04-05 11:19:41.000000 proceduraldata-1.1.3/pdata/analysis/__init__.py
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     6971 2022-06-11 10:57:58.000000 proceduraldata-1.1.3/pdata/analysis/dataexplorer.py
--rw-rw-r--   0 govenius  (1000) govenius  (1000)    36769 2022-11-26 14:55:37.000000 proceduraldata-1.1.3/pdata/analysis/dataview.py
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     7486 2022-09-27 19:39:45.000000 proceduraldata-1.1.3/pdata/helpers.py
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     2834 2022-10-27 06:05:39.000000 proceduraldata-1.1.3/pdata/jupyter_helpers.py
--rw-rw-r--   0 govenius  (1000) govenius  (1000)    13699 2022-11-26 15:01:40.000000 proceduraldata-1.1.3/pdata/procedural_data.py
-drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2022-11-27 08:22:29.389280 proceduraldata-1.1.3/proceduraldata.egg-info/
--rw-rw-r--   0 govenius  (1000) govenius  (1000)     2856 2022-11-27 08:22:29.000000 proceduraldata-1.1.3/proceduraldata.egg-info/PKG-INFO
--rw-rw-r--   0 govenius  (1000) govenius  (1000)      415 2022-11-27 08:22:29.000000 proceduraldata-1.1.3/proceduraldata.egg-info/SOURCES.txt
--rw-rw-r--   0 govenius  (1000) govenius  (1000)        1 2022-11-27 08:22:29.000000 proceduraldata-1.1.3/proceduraldata.egg-info/dependency_links.txt
--rw-rw-r--   0 govenius  (1000) govenius  (1000)      122 2022-11-27 08:22:29.000000 proceduraldata-1.1.3/proceduraldata.egg-info/requires.txt
--rw-rw-r--   0 govenius  (1000) govenius  (1000)        6 2022-11-27 08:22:29.000000 proceduraldata-1.1.3/proceduraldata.egg-info/top_level.txt
--rw-rw-r--   0 govenius  (1000) govenius  (1000)      735 2022-11-27 08:22:29.393281 proceduraldata-1.1.3/setup.cfg
--rw-rw-r--   0 govenius  (1000) govenius  (1000)       37 2022-04-03 12:24:52.000000 proceduraldata-1.1.3/setup.py
+drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2023-04-22 09:24:53.994950 proceduraldata-2.0.4/
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     1072 2022-04-05 11:37:57.000000 proceduraldata-2.0.4/LICENSE
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     3089 2023-04-22 09:24:53.994950 proceduraldata-2.0.4/PKG-INFO
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     1575 2023-02-02 18:45:51.000000 proceduraldata-2.0.4/README.rst
+drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2023-04-22 09:24:53.986949 proceduraldata-2.0.4/pdata/
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)      305 2022-04-05 11:19:21.000000 proceduraldata-2.0.4/pdata/__init__.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)       53 2023-04-22 09:17:30.000000 proceduraldata-2.0.4/pdata/_metadata.py
+drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2023-04-22 09:24:53.990949 proceduraldata-2.0.4/pdata/analysis/
+-rwxrwxr-x   0 govenius  (1000) govenius  (1000)      306 2022-04-05 11:19:41.000000 proceduraldata-2.0.4/pdata/analysis/__init__.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)    10871 2023-04-22 09:11:16.000000 proceduraldata-2.0.4/pdata/analysis/dataexplorer.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)    49462 2023-04-22 08:55:23.000000 proceduraldata-2.0.4/pdata/analysis/dataview.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     1681 2022-12-30 17:38:30.000000 proceduraldata-2.0.4/pdata/hdf5tools.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     8299 2023-03-04 11:44:05.000000 proceduraldata-2.0.4/pdata/helpers.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     2834 2022-10-27 06:05:39.000000 proceduraldata-2.0.4/pdata/jupyter_helpers.py
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)    17611 2023-01-31 18:38:29.000000 proceduraldata-2.0.4/pdata/procedural_data.py
+drwxrwxr-x   0 govenius  (1000) govenius  (1000)        0 2023-04-22 09:24:53.994950 proceduraldata-2.0.4/proceduraldata.egg-info/
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)     3089 2023-04-22 09:24:53.000000 proceduraldata-2.0.4/proceduraldata.egg-info/PKG-INFO
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)      434 2023-04-22 09:24:53.000000 proceduraldata-2.0.4/proceduraldata.egg-info/SOURCES.txt
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)        1 2023-04-22 09:24:53.000000 proceduraldata-2.0.4/proceduraldata.egg-info/dependency_links.txt
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)      129 2023-04-22 09:24:53.000000 proceduraldata-2.0.4/proceduraldata.egg-info/requires.txt
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)        6 2023-04-22 09:24:53.000000 proceduraldata-2.0.4/proceduraldata.egg-info/top_level.txt
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)      743 2023-04-22 09:24:53.998950 proceduraldata-2.0.4/setup.cfg
+-rw-rw-r--   0 govenius  (1000) govenius  (1000)       37 2022-04-03 12:24:52.000000 proceduraldata-2.0.4/setup.py
```

### Comparing `proceduraldata-1.1.3/LICENSE` & `proceduraldata-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proceduraldata-1.1.3/PKG-INFO` & `proceduraldata-2.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: proceduraldata
-Version: 1.1.3
+Version: 2.0.4
 Summary: Simple-to-understand and robust data storage for experimental data
 Home-page: https://pdata.readthedocs.io/
 Author: Joonas Govenius
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-pdata: Simple-to-understand and robust data storage for experimental data
-=========================================================================
+pdata: Straightforward and robust data storage for experimental data
+====================================================================
 
 This *procedural* data storage package provides a self-contained
 interface **focused exclusively on storing and reading experimental
 data**, using an approach **independent of the specific measurement
 framework used for instrument control**.
 
 The main goals are to provide an interface that:
 
-  * Maximizes the amount of automatically stored metadata, without relying on the experimenter specifying which values are worthy of saving.
-  * Is "procedural" rather than "functional" in terms of the API the experimenter sees, as procedural programming tends to be easier to understand for a typical experimental physicist.
+  * Automatically stores a lot of metadata, including parameters that change during a measurement.
+  * Is *procedural* rather than *functional* in terms of the API the experimenter sees, as procedural programming tends to be easier to understand for a typical experimental physicist.
+  * Uses standard Python flow-control constructs (for, while, if, etc.) for looping over setpoints.
   * The API aims to be self-explanatory, wherever possible.
 
 In practice, the experimenter calls an explicit :code:`add_points(<new
 data points>)` function to add rows to a traditional table of data
 points, with user-defined columns. In the background, **pdata
-automatically records all changes to instrument parameters**, each
+automatically records all changes to instrument parameters** each
 time :code:`add_points` is called.
 
-In addition, pdata provides useful helpers for reading back the
-automatically recorded instrument parameters.
+In addition, pdata provides useful helpers for reading back the data,
+including automatically recorded instrument parameters, basic helpers
+for visualization, and good export capabilities to other tools for
+further analysis.
+
+Getting started/Full documentation
+----------------------------------
 
 See the `documentation <http://pdata.readthedocs.io>`_ at RTD for
 instructions on getting started.
 
 MIT License
 
 Copyright (c) 2016 Joonas Govenius
```

### Comparing `proceduraldata-1.1.3/README.rst` & `proceduraldata-2.0.4/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-pdata: Simple-to-understand and robust data storage for experimental data
-=========================================================================
+pdata: Straightforward and robust data storage for experimental data
+====================================================================
 
 This *procedural* data storage package provides a self-contained
 interface **focused exclusively on storing and reading experimental
 data**, using an approach **independent of the specific measurement
 framework used for instrument control**.
 
 The main goals are to provide an interface that:
 
-  * Maximizes the amount of automatically stored metadata, without relying on the experimenter specifying which values are worthy of saving.
-  * Is "procedural" rather than "functional" in terms of the API the experimenter sees, as procedural programming tends to be easier to understand for a typical experimental physicist.
+  * Automatically stores a lot of metadata, including parameters that change during a measurement.
+  * Is *procedural* rather than *functional* in terms of the API the experimenter sees, as procedural programming tends to be easier to understand for a typical experimental physicist.
+  * Uses standard Python flow-control constructs (for, while, if, etc.) for looping over setpoints.
   * The API aims to be self-explanatory, wherever possible.
 
 In practice, the experimenter calls an explicit :code:`add_points(<new
 data points>)` function to add rows to a traditional table of data
 points, with user-defined columns. In the background, **pdata
-automatically records all changes to instrument parameters**, each
+automatically records all changes to instrument parameters** each
 time :code:`add_points` is called.
 
-In addition, pdata provides useful helpers for reading back the
-automatically recorded instrument parameters.
+In addition, pdata provides useful helpers for reading back the data,
+including automatically recorded instrument parameters, basic helpers
+for visualization, and good export capabilities to other tools for
+further analysis.
+
+Getting started/Full documentation
+----------------------------------
 
 See the `documentation <http://pdata.readthedocs.io>`_ at RTD for
 instructions on getting started.
```

### Comparing `proceduraldata-1.1.3/pdata/analysis/dataview.py` & `proceduraldata-2.0.4/pdata/analysis/dataview.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 import datetime
 import pytz
 from dateutil import tz
 from collections import OrderedDict
 
 UNIX_EPOCH = datetime.datetime(1970, 1, 1, 0, 0, tzinfo = pytz.utc)
 
+column_name_regex = r"[\w\d\s\-+%=/*&]+"
+column_unit_regex = r"[\w\d\s\-+%=/*&]*"
+
 class PDataSingle():
     ''' Class for reading in the contents of a single pdata data directory.
         Almost always passed on to DataView for actual analysis. '''
 
     def __init__(self, path, convert_timestamps=True, parse_comments=False):
       '''Parse data stored in the specified directory path.
 
@@ -65,96 +68,83 @@
             diff_names.append((int(m.group(1)), int(m.group(2)), m.group(0)))
             continue
         diff_names.sort(key=lambda x: x[1]) # secondary sort on .diff<n>
         diff_names.sort(key=lambda x: x[0]) # primary sort on .row-<n>
         return diff_names
 
       def parse_tabular_data(f):
-        # First analyze the first data row and the header rows preceding it.
-        self._comments = []
-        converters = {}
-        rowno = 0
-        comment = ""
-        while True:
-          line = f.readline()
-          if not isinstance(line, str): line = line.decode('utf-8')
-          if len(line) == 0: break # EOF
-
-          line = line.strip()
-          if len(line) == 0: continue # empty line
-
-          if line.startswith('#'): # comment line
-            comment += line[1:].strip() + '\n'
-            continue
-
-          # Otherwise this is a data row
-          comment = comment.strip()
-          if len(comment) > 0:
-            # Store comment(s) preceding this data row
-            self._comments.append((rowno, comment))
-
-          # The comment rows preceding the first data row contain the table header
-          # that defines the column names. Store it for later parsing.
-          if rowno==0: self._table_header = comment
-
-          # Determine the number of columns from the first data row
-          if rowno==0: ncols = len(line.split('\t'))
-
-          # Determine, based on the first data row, whether any columns contain
-          # time stamps. Convert them into seconds since Unix epoch.
-          if rowno==0 and convert_timestamps:
-            for i,c in enumerate(line.split('\t')):
-              try:
-                PDataSingle._parse_timestamp(c)
-                converters[i] = lambda x: PDataSingle._parse_timestamp(x.decode('utf-8'))
-                logging.info('Column %s appears to contain timestamps. Converting them to seconds since Unix epoch. (Disable by setting convert_timestamps=False.)', i)
-              except ValueError:
-                pass # Not a timestamp
-
-          rowno += 1
-          comment = ""
-
-          # Done parsing the header. We can stop here if parsing comments after first data row is not requested.
-          if not parse_comments: break
-
-        # Store header even if there were zero data rows
-        if rowno==0: self._table_header = comment
+        # First extract the first data row and the header rows preceding it.
+        header = PDataSingle._extract_header(f, parse_all_comments=parse_comments)
+        self._comments = header["comments"]
+
+        #print("\n" + header["table_header"])
+        #if "first_data_row" in header.keys(): print(header["first_data_row"])
+        #time.sleep(0.1)
 
         # Now parse the stored header
-        if not hasattr(self, "_table_header"):
+        if not "table_header" in header.keys():
           logging.warning(f"No header found in tabular data of {self._path}")
-          self._column_names, self._units = [], []
+          self._column_names, self._units, dtypes = [], [], []
+        else:
+          self._column_names, self._units = PDataSingle._parse_columns_from_header(header["table_header"])
+          dtypes, converters = PDataSingle._parse_dtypes_from_header(header["table_header"],
+                                                                                 convert_timestamps=convert_timestamps)
+
+        self._column_name_to_index = dict( (n, i) for i,n in enumerate(self._column_names) )
+
+        if "first_data_row" in header.keys():
+          # Analyze first data row
+          inferred_dtypes, inferred_converters = PDataSingle._infer_dtypes_from_first_data_row(
+              header["first_data_row"],
+              convert_timestamps=(dtypes==None and convert_timestamps))
         else:
-          self._column_names, self._units = PDataSingle._parse_columns_from_header(self._table_header)
+          inferred_dtypes, inferred_converters = dict( (i, float) for i in range(len(self._column_names)) ), {}
+
+        assert len(self._column_names) == len(inferred_dtypes.keys()), "The number of columns in the header and first data row do not match."
+        if dtypes is None:
+          dtypes = inferred_dtypes
+          converters = inferred_converters
+
+        assert len(self._column_names) == len(dtypes.keys()), "The number of columns in the header and number of parsed dtypes do not match."
+        dtypes = list( dtypes[i] for i in range(len(dtypes.keys())) )
+
+        if "first_data_row" in header.keys():
+          # Parse the actual numerical data.
+          #
+          # Use "col{i}" as names, rather than self._column_names,
+          # since pdata column names may contain characters not
+          # allowed in numpy structured arrays.
+          f.seek(0)
+          self._data = np.genfromtxt(f,
+                                     delimiter="\t",
+                                     comments="#",
+                                     converters=dict( (f"col{i}", c) for i,c in converters.items() ),
+                                     dtype=dtypes,
+                                     names=list(f"col{i}" for i in range(len(self._column_names))) )
 
-        if rowno > 0:
-          assert len(self._column_names) == ncols, "The number of columns in the header and data do not seem to match."
+          # If the data contains just a single row, genfromtxt returns a 0D array! Fortunately reshaping still works.
+          # Note: In Numpy >= 1.23.0, setting ndmin for genfromtxt might also solve this but that remains untested.
+          try:
+            len(self._data)
+          except TypeError:
+            self._data = self._data.reshape((-1,))
+
+          # Parse the footer as well, if any
+          self._footer = PDataSingle._parse_footer(PDataSingle._extract_footer(f))
+          #print("\n\n"); print(footer); time.sleep(0.1)
 
-        self._column_name_to_index = dict((self._column_names[i], i) for i in range(len(self._column_names)) )
+        else:
+          logging.warning(f"No data rows in tabular_data of {self._path}")
+          self._data = np.array([], dtype=np.dtype(list( (f"col{i}", dt) for i,dt in enumerate(dtypes) )))
+          self._footer = {}
 
-        # Parse the actual numerical data
-        f.seek(0)
-        self._data = np.genfromtxt(f,
-                                   delimiter="\t",
-                                   comments="#",
-                                   converters=converters,
-                                   dtype=float) # Assume all columns contain floats
-
-        # If the data contains just a single row or a single column,
-        # genfromtxt returns a 1D vector instead of a 2D array, so convert it to 2D.
-        # Note: In Numpy >= 1.23.0, setting ndmin=2 for genfromtxt might also solve this but that remains untested.
-        if rowno>0 and len(self._data.shape) == 1: self._data = self._data.reshape((-1, ncols))
-
-        if parse_comments:
-          # rowno should equal the number of data rows, if comments were parsed and
-          # no new data was added between the two passes through the file.
-          assert len(self._data) >= rowno, 'Unexcepted number of data rows: %s vs %s' % (len(self._data), rowno)
+        #print("\n" + repr(self._data)); time.sleep(0.1)
 
         if len(self._data) > 0:
-          assert len(self._data[0]) == ncols, 'Unexcepted number of data columns: %s vs %s' % (len(self._data[0]), ncols)
+          assert len(self._data[0]) == len(self._column_names), 'Unexcepted number of data columns: %s vs %s' % (len(self._data[0]), len(self._column_names))
 
 
       ###########################################################
       # Actually parse the data using the helper functions above
       ###########################################################
 
       # Parse main data file (possibly compressed)
@@ -184,14 +174,20 @@
             add_snapshot_diff(row, tar.extractfile(fname))
 
       else: # uncompressed snapshot diffs as separate files
         for row,j,fname in parse_snapshot_diff_names(os.listdir(path)):
           with open(os.path.join(path, fname)) as f:
             add_snapshot_diff(row, f)
 
+      if "snapshot_diffs_preceding_rows" in self._footer.keys():
+        # Check that snapshot diff rows parsed from file names match the info in the footer
+        assert all( i==j for i,j in zip(self._footer["snapshot_diffs_preceding_rows"],
+                                        [ r for r,s in self._snapshots[1:] ] )
+                   ), "Snapshot diff rows parsed from file names don't match rows listed in tabular data footer."
+
 
     def name(self): return os.path.split(self._path)[-1]
     def filename(self): return self._path
     def dimension_names(self): return self._column_names
     def dimension_units(self): return self._units
     def npoints(self): return len(self._data)
     def data(self): return self._data
@@ -199,52 +195,264 @@
     def comments(self):
       return self._comments
 
     def settings(self):
       return self._snapshots
 
     def __getitem__(self, key):
-      return self._data[:, self._column_name_to_index[key]]
+      return self._data[f"col{self._column_name_to_index[key]}"]
 
     @staticmethod
     def _parse_timestamp(s):
       t = datetime.datetime.strptime(s, '%Y-%m-%d %H:%M:%S.%f')
       return (t.astimezone() - UNIX_EPOCH).total_seconds()
 
     @staticmethod
+    def _extract_header(f, parse_all_comments=False):
+      """ Extract header and first data row from tabular data file f. """
+      r = {} # Dict for results to return
+      r["comments"] = []
+      rowno = 0
+      comment = ""
+      while True:
+        line = f.readline()
+        if not isinstance(line, str): line = line.decode('utf-8')
+        if len(line) == 0: break # EOF
+
+        line = line.strip()
+        if len(line) == 0: continue # empty line
+
+        if line.startswith('#'): # comment line
+          comment += line[1:].strip() + '\n'
+          continue
+
+        # Otherwise this is a data row
+        comment = comment.strip()
+        if len(comment) > 0:
+          # Store comment(s) preceding this data row
+          r["comments"].append((rowno, comment))
+
+        # The comment rows preceding the first data row contain the
+        # table header that defines the column names. Store the
+        # header and the first data row for later parsing.
+        if rowno==0:
+          r["table_header"] = comment
+          r["first_data_row"] = line
+
+        rowno += 1
+        comment = ""
+
+        # Done parsing the header. We can stop here if not requested
+        # to parse all comments, also after first data row.
+        if not parse_all_comments: break
+
+      # Store header even if there were zero data rows
+      if rowno==0:
+        # Header is in the "comment" variable at this point. But
+        # "comment" may also contant a footer so strip everything
+        # after "Measurement ended at".
+        table_header = []
+        for line in comment.split("\n"):
+          if line.strip().startswith("Measurement ended at "): break
+          table_header.append(line)
+        r["table_header"] = "\n".join(table_header)
+
+      return r
+
+    @staticmethod
+    def _infer_dtypes_from_first_data_row(line, convert_timestamps):
+      """Infer data types from the first data row (in case the information
+         is not available in the table header).
+      """
+      converters = {}
+      dtypes = {}
+      for i,c in enumerate(line.split('\t')):
+        c = c.strip().lower()
+
+        if c in ["true", "false"]:
+          dtypes[i] = bool
+          continue
+
+        if convert_timestamps:
+          # If col is a time stamp, convert it into seconds since Unix epoch.
+          try:
+            PDataSingle._parse_timestamp(c)
+            converters[i] = lambda x: PDataSingle._parse_timestamp(x.decode('utf-8'))
+            dtypes[i] = float
+            logging.info(f'Column {i} appears to contain timestamps. Converting them to seconds since Unix epoch. (Disable by setting convert_timestamps=False.)')
+            continue
+          except ValueError:
+            pass # Not a timestamp
+
+        try:
+          # Convert all numerical types to float, including
+          # integers. This is a bit safer, in case the first row looks
+          # like an int but other rows contain floats.
+          float(c)
+          dtypes[i] = float
+          continue
+        except ValueError:
+          pass # Not a float, int, or similar number
+
+        # Otherwise parse this column as str
+        dtypes[i] = str
+
+      return dtypes, converters
+
+    @staticmethod
+    def _parse_dtypes_from_header(s, convert_timestamps):
+      """Check for dtype specification in the
+         "Column dtypes: float\tfloat\tint\t..." format. """
+      m = re.search(r'(?m)^\s*Column dtypes:\s*(.*?)?$', s)
+      if m==None or len(m.groups()) != 1: return None, None
+
+      dtypes = {}
+      converters = {}
+      for i,dt in enumerate(m.group(1).split("\t")):
+        dt = dt.strip()
+        if dt.startswith("numpy."):
+          try:
+            dtypes[i] = getattr(np, dt[len("numpy."):])
+          except AttributeError:
+            logging.warning(f"Column {i} dtype = {dt} seems like a numpy data type based on prefix, "
+                            f"but numpy.{dt} doesn't exist. Falling back to str.")
+            dtypes[i] = str
+        elif dt.startswith("builtins."):
+          dtypes[i] = eval(dt[len("builtins."):])
+        elif dt in ["datetime.datetime", "datetime"]:
+          if convert_timestamps:
+            dtypes[i] = float
+            converters[i] = lambda x: PDataSingle._parse_timestamp(x.decode('utf-8'))
+          else:
+            logging.info(f'Column {i} contains timestamps. Converting them to seconds since Unix epoch. (Disable by setting convert_timestamps=False.)')
+            dtypes[i] = datetime.datetime
+            converters[i] = lambda x: dtypes[i](x.decode('utf-8'))
+        else:
+          if not dt in [ "None" ]:
+            logging.warning(f"Column {i} dtype = {dt} unrecognized. Falling back to str.")
+          dtypes[i] = str
+
+      return dtypes, converters
+
+    @staticmethod
     def _parse_columns_from_header(s):
+      """Parse column names and units from table header. Asssume that the
+         last non-empty header line has them in the "Column name
+         (unit)\t" format. If not, fall back to assuming similar but
+         simpler legacy QCoDeS format.
+      """
+      # Split into lines and keep only non-empty ones
+      column_names_and_units = [ l for l in s.split('\n') if len(l.strip())>0 ]
+      if len(column_names_and_units) == 0: return [],[]
+
       try:
-        # Try assuming the "Column name (unit)\t" format in pdata
         cols = []
         units = []
-        for c in s.split('\t'):
-          m = re.match(r'([\w\d\s]+)\s+\(([\w\d\s]*)\)', c.strip())
+        for c in column_names_and_units[-1].split('\t'):
+          m = re.match(f'({column_name_regex})\s+\(({column_unit_regex})\)', c.strip())
           cols.append(m.group(1))
           units.append(m.group(2))
 
       except AttributeError:
         # Try assuming the legacy format used in QCoDeS (qcodes/data/gnuplot_format.py)
-        s = s.split('\n')[-2] # Second to last header row contains the tab separated column names
-        cols = [ c.strip().strip('"') for c in s.split('\t') ]
-        units = [ '' for i in range(len(cols))]
+        try:
+          # Last row contains the number of data points --> ignore
+          if column_names_and_units[-1].strip().isdigit(): del column_names_and_units[-1]
+
+          cols = [ c.strip().strip('"') for c in column_names_and_units[-1].split('\t') ]
+          units = [ '' for i in range(len(cols))]
+        except IndexError:
+          logging.warning(f"Could not parse tabular data header. Header: {s}")
+          raise
 
       return cols, units
 
+    @staticmethod
+    def _extract_footer(f, chunk_size=4096):
+      """Return tabular data footer from file object f. The footer contains,
+         by defition, all rows following the last data row (= last
+         non-empty row not starting with #).
+
+         Assumes that current position is already at the end of the
+         file.
+
+         If there are zero data rows, the parsed string may also
+         include the header.
+
+      """
+
+      b = isinstance(f.read(0), bytes) # Check whether we read bytes or strings from f
+
+      tail = b"" if b else ""
+      while True:
+        try:
+          # Append one more chunk to tail
+          f.seek(-min(f.tell(), (1 + (len(tail)>0))*chunk_size), os.SEEK_CUR)
+          tail = f.read(chunk_size) + tail
+        except IOError:
+          # Read entire file into tail
+          logging.debug(f"Could not read footer in chunks from end of file object {f} --> Reading entire file.")
+          f.seek(0)
+          tail = f.read()
+          break
+
+        # Check whether tail already contains non-comment rows.
+        # If so, we must have read the entire footer already
+        if any( not (l.strip().startswith(b"#" if b else "#") or len(l.strip())==0)
+                for l in tail.split(b"\n" if b else "\n") ):
+          break
+
+      # Remove non-comment rows:
+      footer = []
+      for l in reversed(tail.split(b"\n" if b else "\n")):
+        l = l.strip()
+        if len(l)==0: continue
+        if b: l = l.decode("utf-8")
+        if not l.startswith("#"): break
+        footer.append(l[1:].strip())
+
+      return "\n".join(reversed(footer))
+
+    @staticmethod
+    def _parse_footer(raw_footer):
+
+      r = { "raw_footer": raw_footer }
+
+      # Parse information from standard rows in the footer.
+      m = re.search(r'(?m)^\s*Snapshot diffs preceding rows \(0-based index\):\s*(.*?)?$', raw_footer)
+      if m!=None and len(m.groups()) == 1:
+        try:
+          r["snapshot_diffs_preceding_rows"] = np.array([ int(i) for i in m.group(1).split(",") ]
+                                                        if m.group(1).strip() != "" else [],
+                                                        dtype=int)
+        except:
+          logging.exception(f"Failed to parse snapshot diff row spec '{m.group(1)}' into a list of ints.")
+
+      m = re.search(r'(?m)^\s*Measurement ended at\s+(.*?)?$', raw_footer)
+      if m!=None and len(m.groups()) == 1:
+        try:
+          r["measurement_ended_at"] = datetime.datetime.strptime(m.group(1), '%Y-%m-%d %H:%M:%S.%f')
+        except:
+          logging.exception(f"Failed to parse measurement end time '{m.group(1)}' into a datetime object.")
+
+      return r
+
+
 class DataView():
     '''
     Class for post-processing measurement data. Main features are:
       * Concatenating multiple separate data objects
       * Creating "virtual" columns by parsing comments or snapshot files
         or by applying arbitrary functions to the data
       * Dividing the rows into "sweeps" based on various criteria.
 
     See docs/examples/Procedural Data and DataView.ipynb for example use.
     '''
 
-    def __init__(self, data, deep_copy=False, source_column_name='data_source', fill_value=None, **kwargs):
+    def __init__(self, data, deep_copy=False, source_column_name='data_source'):
         '''
         Create a new view of existing data objects for post-processing.
         The original data objects will not be modified.
 
         args:
           data -- Data object(s). Each data object needs to provide the following methods:
                      * name()     # Arbitrary string identifier for the data object
@@ -263,25 +471,22 @@
 
         kwargs input:
           deep_copy          -- specifies whether the underlying data is copied or 
                                 only referenced (more error prone, but memory efficient)
           source_column_name -- specifies the name of the (virtual) column that tells which
                                 data object the row originates from. Specify None, if
                                 you don't want this column to be added.
-          fill_value         -- fill value for columns that do not exist in all data objects.
-                                Default is None, in which case the column is omitted entirely.
         '''
 
         self._virtual_dims = {}
 
         if isinstance(data, DataView): # clone
           # these private variables should be immutable so no need to deep copy
           self._dimensions = data._dimensions
           self._units = data._units
-          self._dimension_indices = data._dimension_indices
           self._source_col = data._source_col
           self._comments = data._comments
           self._settings = data._settings
           
           if deep_copy:
             self._data = data._data.copy()
           else:
@@ -291,84 +496,82 @@
           self._mask = data._mask.copy()
 
           for name, fn in data._virtual_dims.items():
               self._virtual_dims[name] = fn
 
           return
 
-        try: # see if a single Data object
+        def get_source_column_name(dat):
+          return f"{dat.name()}_({dat.filename().strip('.dat')})"
+
+        def is_pdatasingle_like(x):
+          return ( hasattr(x, "dimension_names") and hasattr(x, "dimension_units")
+                   and hasattr(x, "name") and hasattr(x, "comments")
+                   and hasattr(x, "data") )
+
+        if is_pdatasingle_like(data): # data is a single Data object
           self._dimensions = data.dimension_names()
           self._units = dict(zip(data.dimension_names(), data.dimension_units()))
-          unmasked = data.data().copy() if deep_copy else data.data()
-          
+          unmasked = dict( (dim, data[dim]) for dim in data.dimension_names() )
+
           if source_column_name != None:
-            n = data.name()
+            n = get_source_column_name(data)
             self._source_col = [n for i in range(data.npoints())]
           else:
             self._source_col = None
 
           self._comments = data.comments()
 
           try:
             self._settings = data.settings()
           except:
             logging.exception("Could not parse the instrument settings file. Doesn't matter if you were not planning to add virtual columns based on values in the snapshot files.")
             self._settings = None
 
-        except MemoryError as e:
-          raise
+        else: # probably data is a sequence of Data objects then
+          assert all(is_pdatasingle_like(dd) for dd in data), "data does not seem to be a PDataSingle-like object, nor a sequence of them: " + repr(data)
 
-        except Exception as e: # probably a sequence of Data objects then
           self._dimensions = set(itertools.chain( *(dd.dimension_names() for dd in data) ))
-          
+
           unmasked = {}
           for dim in self._dimensions:
             unmasked[dim] = []
             for dat in data:
               if len(dat.dimension_names()) == 0:
                 logging.warning("%s seems to contain zero columns. Skipping it..." % (dat.filename()))
-                break
+                continue
 
               n_rows = dat.npoints()
               if n_rows == 0:
                 logging.info("%s seems to contain zero rows. Skipping it..." % (dat.filename()))
-                break
+                continue
 
               try:
                 unmasked[dim].append(dat[dim])
-              except:
-                msg = "Dimension '%s' does not exist in Data object '%s'. " % (dim, str(dat))
-                if fill_value == None:
-                  # ignore dimensions that don't exist in all data objects
-                  del unmasked[dim]
-                  msg += ' Omitting the dimension.'
-                  logging.warning(msg)
-                  break
-                else:
-                  unmasked[dim].append(fill_value + np.zeros(n_rows, dtype=type(fill_value)))
-                  msg += ' Using fill_value = %s (for %d rows)' % (str(fill_value), len(unmasked[dim][-1]))
-                  logging.warning(msg)
+              except KeyError:
+                logging.warning(f"Dimension {dim} does not exist in data object {str(dat)}. Omitting the dimension.")
+                del unmasked[dim]
+                break
 
             # concatenate rows from all files
             if dim in unmasked.keys():
               unmasked[dim] = np.concatenate(unmasked[dim]) if len(unmasked[dim])>0 else np.array([])
 
           # add a column that specifies the source data file
           lens = [ dat.npoints() for dat in data ]
           if source_column_name != None:
-            names = [ '%s_(%s)' % (dat.name(), dat.filename().strip('.dat')) for dat in data ]
+            names = [ get_source_column_name(dat) for dat in data ]
             self._source_col = [ [n for jj in range(l)] for n,l in zip(names,lens) ]
             #self._source_col = [ jj for jj in itertools.chain.from_iterable(self._source_col) ] # flatten
             self._source_col = list(itertools.chain.from_iterable(self._source_col)) # flatten
           else:
             self._source_col = None
-          
+
           # keep only dimensions that could be parsed from all files
           self._dimensions = unmasked.keys()
-          unmasked = np.array([unmasked[k] for k in self._dimensions]).T
 
           # take units from first data set
           self._units = dict(zip(data[0].dimension_names(), data[0].dimension_units()))
 
           # concatenate comments, adjusting row numbers from Data object rows to the corresponding dataview rows
           lens = np.array(lens)
 
@@ -388,34 +591,29 @@
         # Check for existence of multiple settings dicts for a single
         # data row. If they exist, we only care about the last one. --> Remove others.
         for i in range(len(self._settings)-1,0,-1):
           if self._settings[i][0] == self._settings[i-1][0]: del self._settings[i-1]
 
         # Initialize masks
         self._data = unmasked
-        self._mask = np.zeros(len(unmasked), dtype=bool)
+        self._mask = np.zeros(0 if len(unmasked.keys())==0 else
+                              len(unmasked[list(unmasked.keys())[0]]), dtype=bool)
         self._mask_stack = []
 
-        self._dimension_indices = dict([(n,i) for i,n in enumerate(self._dimensions)])
         self.set_mask(False)
 
         if source_column_name != None:
           self.add_virtual_dimension(source_column_name, arr=np.array(self._source_col))
 
     def __getitem__(self, index):
         '''
-        Access the data.
-
-        index may be a slice or a string, in which case it is interpreted
-        as a dimension name.
+        Get the values of a given dimension as a vector.
         '''
-        if isinstance(index, str):
-            return self.column(index)
-        else:
-            return self.data()[index]
+        assert isinstance(index, str), "Data must be indexed using a dimension name. Dimensions in this Dataview: {self.dimensions()}"
+        return self.column(index)
 
     def copy(self, copy_data=False):
         '''
         Make a copy of the view. The returned copy will always have an independent mask.
         
         copy_data -- whether the underlying data is also deep copied.
         '''
@@ -441,15 +639,15 @@
         '''
         return self._mask.copy()
 
     def dimensions(self):
         '''
         Returns a list of all dimensions, both real and virtual.
         '''
-        return list(itertools.chain(self._dimension_indices.keys(), self._virtual_dims.keys()))
+        return list(itertools.chain(self._data.keys(), self._virtual_dims.keys()))
 
     def units(self, d):
         '''
         Returns the units for dimension d
         '''
         return self._units[d]
 
@@ -565,37 +763,38 @@
         This is typically unnecessary, but may be useful
         before adding (cached) virtual columns to
         huge data sets where most rows are masked (because
         the cached virtual columns are computed for
         masked rows as well.)
         '''
         # Removing the real data rows themselves is easy.
-        self._data = self._data[~(self._mask),:]
-        
+        for d in self._data.keys():
+          self._data[d] = self._data[d][~(self._mask)]
+
         # but we have to also adjust the comment & settings line numbers
         s = np.cumsum(self._mask.astype(int))
         def n_masked_before_line(lineno): return s[max(0, min(len(s)-1, lineno-1))]
         self._comments = [ (max(0,lineno-n_masked_before_line(lineno)), comment) for lineno,comment in self._comments ]
         self._settings = [ (max(0,lineno-n_masked_before_line(lineno)), setting) for lineno,setting in self._settings ]
 
         # as well as remove the masked rows from cached virtual columns.
         # However, _virtual_dims is assumed to be immutable in copy() so
         # we must copy it here!
         old_dims = self._virtual_dims
         self._virtual_dims = {}
-        for name, dim in old_dims.iteritems():
+        for name, dim in old_dims.items():
           cached_arr = dim['cached_array']
           if isinstance(cached_arr, np.ndarray):
             cached_arr = cached_arr[~(self._mask)]
           elif cached_arr != None:
             cached_arr = [ val for i,val in enumerate(cached_arr) if not self._mask[i] ]
           self._virtual_dims[name] = { 'fn': dim['fn'], 'cached_array': cached_arr }
 
         # finally remove the obsolete mask(s)
-        self._mask = np.zeros(len(self._data), dtype=bool)
+        self._mask = np.zeros(len(self._data[list(self._data.keys())[0]]), dtype=bool)
         self._mask_stack = []
 
     def single_valued_parameter(self, param):
         ''' If all values in the (virtual) dimension "param" are the same, return that value. '''
         assert len(np.unique(self[param])) == 1 or (all(np.isnan(self[param])) and len(self[param]) > 0), \
             '%s is not single valued for the current unmasked rows: %s' % (param, np.unique(self[param]))
         return self[param][0]
@@ -690,26 +889,14 @@
         '''
         Mask all rows except the specified sweeps (see divide_into_sweeps()).
 
         sl can be a single integer or any slice object compatible with a 1D numpy.ndarray (list of sweeps).
         '''
         self.mask_sweeps(sweep_dimension, sl, unmask_instead=True)
 
-
-    def data(self, deep_copy=False):
-        '''
-        Get the non-masked data as a 2D ndarray.
-
-        kwargs:
-          deep_copy -- copy the returned data so that it is safe to modify it.
-        '''
-        d = self._data[~(self._mask)]
-        if deep_copy: d = d.copy()
-        return d
-
     def column(self, name, deep_copy=False):
         '''
         Get the non-masked entries of dimension 'name' as a 1D ndarray.
         name is the dimension name.
 
         kwargs:
           deep_copy -- copy the returned data so that it is safe to modify it.
@@ -722,16 +909,16 @@
               try:
                 d = d[~(self._mask)] # This works for ndarrays
               except:
                 # workaround to mask native python arrays
                 d = [ x for i,x in enumerate(d) if not self._mask[i] ]
             return d
         else:
-            d = self._data[~(self._mask),self._dimension_indices[name]]
-        
+            d = self._data[name][~(self._mask)]
+
         if deep_copy: d = d.copy()
         return d
 
     non_numpy_array_warning_given = []
     def add_virtual_dimension(self, name, units="", fn=None, arr=None, comment_regex=None, from_set=None, dtype=float, preparser=None, cache_fn_values=True, return_result=False):
         '''
         Makes a computed vector accessible as self[name].
@@ -757,15 +944,15 @@
           return_result   -- return the result directly as an (nd)array instead of adding it as a virtual dimension
         '''
         logging.debug('adding virtual dimension "%s"' % name)
 
         assert (fn != None) + (arr is not None) + (comment_regex != None) + (from_set != None) == 1, 'You must specify exactly one of "fn", "arr", or "comment_regex".'
 
         if arr is not None:
-          assert len(arr) == len(self._mask), '"arr" must be a vector of the same length as the real data columns. If you want to do something fancier, specify your own fn.'
+          assert len(arr) == len(self._mask), f'len(arr)={len(arr)} must be the same as the length of the existing data columns ({len(self._mask)}).'
 
         if from_set != None:
             assert self._settings != None, 'snapshot files were not successfully parsed during dataview initialization.'
 
         if comment_regex != None or from_set != None:
             # construct the column by parsing the comments or snapshots
             use_set = (from_set != None) # shorthand for convenience
@@ -861,7 +1048,118 @@
         if name in self._virtual_dims.keys():
             del self._virtual_dims[name]
         else:
             logging.warning('Virtual dimension "%s" does not exist.' % name)
 
     def remove_virtual_dimensions(self):
         self._virtual_dims = {}
+
+    def to_xarray(self, values, coords, fill_value=np.nan,
+                  coarse_graining={}, include_single_valued_params=True):
+        """Create an N-dimensional xarray DataSet out of values, where N is
+           equal to the number of coordinates and values are specified
+           as a list of dataview dimension names, or (<data variable
+           name>, f, <units>) tuples where f(self) returns a vector of
+           length equal to the number of unmasked rows in this
+           DataView. Alternatively, values can be a single dimension
+           name. Coordinates are specified as a list of dimension
+           names. Entries of the xarray corresponding to coordinate
+           combinations that don't exist in this data set are filled
+           with fill_value.
+
+           This is well-suited for N-dimensional parameter/coordinate
+           sweeps that were executed with nested for loops in which
+           the looped coordinate values in each loop were selected
+           mostly independent of other coordinates. Otherwise there
+           will be lots of fill_value's.
+
+           Usually, you'll want to use setpoints, rather than measured
+           values, as coordinates. If a coordinate c is instead a
+           measured value, you probably want to specify coarse
+           graining with coarse_graining={c: <Delta>}, which causes
+           coordinates differing by at most <Delta> to be interpreted
+           as the same coordinate.
+
+           Note that if the same coordinate combination is repeated
+           more than once in the data set, only the last measured
+           value will appear in the output xarray. If you want to
+           preserve information about repetitions, add another
+           coordinate for the repetition number.
+
+           If include_single_valued_params is True, all single valued
+           parameters will be included as attributes of the xarray.
+
+           Spaces, dashes and other special characters in coordinate
+           names are replaced automatically by underscores, as these
+           don't work well with xarray syntax.
+        """
+        # Get unique coordinate values for each coordinate
+        coords = OrderedDict((c, np.unique(self[c])) for c in coords )
+
+        # Mappings from unique coordinate values to coordinate index
+        coord_to_i = dict( (c, dict( (cc,i) for i,cc in enumerate(coords[c]) ))
+                           for c in coords.keys() )
+
+        # Merge similar coordinates
+        for c,delta in coarse_graining.items():
+          coords[c] = list(coords[c]) # since ndarray elements cannot be deleted
+          i = 1
+          while i < len(coords[c]):
+            if coords[c][i] - coords[c][i-1] <= delta:
+              # Map the two coordinates to the same index
+              coord_to_i[c][coords[c][i]] = coord_to_i[c][coords[c][i-1]]
+
+              # Must also decrement all larger index mappings by one
+              for cc in coord_to_i[c].keys():
+                if cc > coords[c][i]: coord_to_i[c][cc] -= 1
+
+              # Delete the nearly identical coordinate
+              del coords[c][i]
+            else:
+              i +=1
+          coords[c] = np.array(coords[c])
+
+        # Special characters to underscores in coordinate names
+        special_chars = r"[\s\-+%=/*&]"
+        dims = list(coords.keys())
+        for i,c in enumerate(dims):
+          if re.search(special_chars, c) is not None:
+            new_c = re.sub(special_chars, "_", c, count=len(c))
+            assert new_c not in dims, f"{new_c} already exists in coords: {dims}"
+            dims[i] = new_c
+
+        # Create the xarrays
+
+        # Also accept a single dimension name as input
+        if isinstance(values, str): values = [ values ]
+
+        import xarray
+        arrays = OrderedDict()
+        if include_single_valued_params: single_valued_params = self.all_single_valued_parameters()
+
+        for value in values:
+          if isinstance(value, str):
+            val_name = value
+            val_vector = self[value]
+            units = self.units(value)
+          else:
+            val_name = value[0]
+            val_vector = value[1](self)
+            units = value[2]
+
+          # Initialize all values as fill_value
+          value_matrix = np.zeros(tuple(len(v) for v in coords.values()), dtype=val_vector.dtype) + fill_value
+
+          # Copy values from self[value] to the correct index in the value_matrix.
+          for i,v in enumerate(val_vector):
+            value_matrix[tuple(coord_to_i[c][self[c][i]] for c in coords.keys())] = v
+
+          # Attributes
+          attrs = { "units": units,
+                    "coord_units": dict((c, self.units(c)) for c in coords.keys()) }
+
+          if include_single_valued_params:
+            for p,v in single_valued_params.items(): attrs[p] = v
+
+          arrays[val_name] = xarray.DataArray(value_matrix, coords=coords.values(), dims=dims, attrs=attrs)
+
+        return xarray.Dataset(arrays)
```

### Comparing `proceduraldata-1.1.3/pdata/helpers.py` & `proceduraldata-2.0.4/pdata/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,34 +12,50 @@
 import numbers
 import collections
 from typing import Any
 
 def preprocess_snapshot(snap, delete_timestamps=True, convert_ndarrays=False):
   '''
   Helper that preprocesses snapshots so that they are compatible with pdata/jsondiff.
-  In particular converts numpy arrays to regular Python lists.
+  In particular converts numpy arrays to regular Python lists, if requested.
   Also, optionally, deletes QCodes timestamp entries from a snapshot dict,
   i.e. dict entries of the form "ts": <str>.
   '''
 
   def preprocesss_dict(d):
     ''' Recursive helper. '''
-    for k in list(d.keys()):
-      if isinstance(d[k], dict): preprocesss_dict(d[k])
-      elif convert_ndarrays and isinstance(d[k], np.ndarray): d[k] = d[k].tolist() # jsondiff doesn't handle ndarrays, unless you use PdataJSONDiffer
-      elif delete_timestamps and k=="ts" and isinstance(d[k], str): del d[k] # QCodes updates these very often
+    for k in get_keys(d):
+      if isinstance(d[k], (collections.abc.Mapping, collections.abc.Sequence)) and not isinstance(d[k], str):
+        preprocesss_dict(d[k])
+      elif convert_ndarrays and isinstance(d[k], np.ndarray):
+        # jsondiff doesn't handle ndarrays by default, but the custom
+        # PdataJSONDiffer below does, so this conversion is no longer
+        # needed and is disabled by default.
+        d[k] = d[k].tolist()
+      elif delete_timestamps and k=="ts" and isinstance(d[k], str):
+        del d[k] # QCodes updates these very often
 
   preprocesss_dict(snap)
   return snap
 
+def get_keys(d, reject_str=True, reject_ndarray=True):
+  """Return keys of d, if d is dict-like, or indices if d is
+     list-like. Raise TypeError for str/ndarray if reject_str/ndarray
+     is True.
+  """
+  if not isinstance(d, (collections.abc.Mapping, collections.abc.Sequence)): raise TypeError()
+  if reject_str and isinstance(d, str): raise TypeError()
+  if reject_ndarray and isinstance(d, np.ndarray): raise TypeError()
+  try: return list(d.keys()) # Assume that d is dict-like
+  except AttributeError: return list(range(0,len(d))) # Assume that d is a list, tuple, or similar
 
 from jsondiff import JsonDiffer
 class PdataJSONDiffer(JsonDiffer):
   """Custom JSON diff creator that handles Numpy ndarrays and lists of
-     only (scalars) as complete blocks. That is, does not create diffs
+     only scalars as complete blocks. That is, does not create diffs
      at element level within ndarrays. This is much faster than the
      default jsondiff list diff creation, and becomes important if the
      snapshots contain e.g. AWG patterns that can be long vectors.
   """
 
   def _obj_diff(self, a, b):
```

### Comparing `proceduraldata-1.1.3/pdata/jupyter_helpers.py` & `proceduraldata-2.0.4/pdata/jupyter_helpers.py`

 * *Files identical despite different names*

### Comparing `proceduraldata-1.1.3/pdata/procedural_data.py` & `proceduraldata-2.0.4/pdata/procedural_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 """
 Class for storing measurement data.
 """
 
 from pdata._metadata import __version__
 
 import os
+import sys
 import numpy as np
 import time
 import datetime
 import logging
 import shutil
 import gzip
 import tarfile
 import contextlib
 import json
 import jsondiff
 import tempfile
 import random
+import re
 
 from pdata.helpers import NumpyJSONEncoder, preprocess_snapshot, PdataJSONDiffer
 import pdata.jupyter_helpers
 
+# Version number of the data format written to disk, following Semantic Versioning (https://semver.org/).
+# This version number should increase much more slowly than the pdata package/release versions.
+ondisk_format_version = (1, 0, 0)
+
 @contextlib.contextmanager
 def run_measurement(get_snapshot,
                     columns, name,
                     data_base_dir='.',
                     dir_name_generator=lambda n: datetime.datetime.now().strftime(f"%Y-%m-%d_%H-%M-%S_{int(1e3*random.random())}") + f"_{n}",
                     autosnap=True, snap_diff_filter=preprocess_snapshot,
-                    compress=True):
+                    compress=True, log_level="inherit"):
   '''
   A simple context manager that runs begin() and end()
   automatically, and gets an updated snapshot of instrument parameters
   each time data is added, using get_snapshot().
 
-  columns defines the tabular data columns, see Measurement class.
+  See docstring of Measurement.__init__ for definition of most arguments.
 
   The directory name for storing the data set is:
     <data_base_dir>/<dir_name_generator(name)>
 
   By default, we filter out timestamps added by QCoDeS from snapshot diffs.
 
-  If you're using QCoDeS, your get_snapshot funciton would typically look like this::
+  If you're using QCoDeS, your get_snapshot function would typically look like this::
 
     import qcodes.station
     with run_measurement(lambda s=qcodes.station.Station.default: s.snapshot(update=True), ...) as m:
       ...
   
   '''
   target_dir = os.path.join(data_base_dir, dir_name_generator(name))
@@ -71,92 +77,111 @@
     * :file:`snapshot.json` -- Instrument parameter snapshot when :code:`run_measurement` started.
     * :file:`snapshot.row-<n>.diff<m>.json` -- `jsondiff <https://pypi.org/project/jsondiff/>`_ of parameter changes, recorded when the there were <n> data rows in tabular_data.dat. <m> is a simple counter, in case multiple diffs are created for the same row.
     * :file:`log.txt` -- copy of messages from the logging module.
     * A copy of the Jupyter notebook (.ipynb) or other measurement script, if possible.
 
   Optionally, the files may be compressed (.gz or .tar.gz).
 
-  Although the format is human readable in the simplest cases, it is
+  Although the format is human-readable in the simplest cases, it is
   meant to be parsed programmatically, i.e., by the dataview module
   (analysis/dataview.py).
 
   For more information, see https://pdata.readthedocs.io/en/latest/
   '''
 
   def __init__(self, columns, target_dir=None, get_snapshot=None,
                autosnap=True, snap_diff_filter=None, omit_readme=False,
-               compress=True):
-    '''
-    Args:
+               compress=True, log_level="inherit"):
+    '''Args:
 
-      columns: a list of strings (column names) or tuples
-               (<column name>, <units> [optional], <formatter> [optional]).
-               Formatter should be a function that takes in a data point
-               and turns it into a str written to the data file.
+      columns: a list of strings (column names) or tuples (<column
+               name>, <units> [optional], <formatter> [optional],
+               <dtype> [optional]).  Formatter should be a function
+               that takes in a data point and turns it into a str
+               written to the data file.  Dtype should be a data type
+               class (e.g. float). analysis.dataview.PDataSingle will
+               use it as a hint while reading the data.
 
       target_dir: full path to where the data directory is to be created.
 
       get_snapshot: function that returns a dict of instrument settings.
 
       autosnap: create snapshot diffs automatically each time add_points()
                 is called.
 
       snap_diff_filter: function applied to the snapshot before computing diffs;
                         useful for filtering things out (e.g. timestamps).
 
       omit_readme: don't create a README file in the data directory.
 
       compress: compress data files when measurement ends
+
+      log_level: log level for log.txt stored in the data
+                 directory. If "inherit", logging.getLogger().level is
+                 used.
     '''
     self._target_dir = target_dir
     self._get_snapshot = get_snapshot
     self._autosnap = True
     self._snap_diff_filter = snap_diff_filter
     self._omit_readme = omit_readme
     self._compress = compress
+    self._log_level = log_level
 
     self._npoints_total = 0
     self._last_snapshot = None
-
+    self._snapshot_diff_rows = []
 
     self._columns = list()
     self._units = list()
     self._formatters = list()
+    self._dtypes = list()
 
     self._check_for_manual_abort()
 
     # Parse columns and units.
     # Units are optional.
     # The formatter is an optional function used for conversion to str.
+    # The data type is an optional data type spec saved as metadata in tabular_data
     for x in columns:
       u = ""
       f = None
+      dt = None
       if isinstance(x, str):
         c = x
       elif len(x) == 2:
         c,u = x
       elif len(x) == 3:
         c,u,f = x
+      elif len(x) == 4:
+        c,u,f,dt = x
       else:
         raise Exception('Did not understand column specification: %s' % x)
 
+      from pdata.analysis.dataview import column_name_regex, column_unit_regex
+      assert re.match(f"^{column_name_regex}$", c) != None, f"Column name '{c}' contains unexpected characters. It does not match the regular expression '^{column_name_regex}$'."
+      assert re.match(f"^{column_unit_regex}$", u) != None, f"Unit '{u}' for column '{c}' contains unexpected characters. It does not match the regular expression '^{column_unit_regex}$'."
+
       self._columns.append(c)
       self._units.append(u)
       self._formatters.append(f)
+      self._dtypes.append(dt)
 
       assert len(self._columns) == len(self._units)
       assert len(self._columns) == len(self._formatters)
 
   def path(self): return self._target_dir
 
   def begin(self):
     '''Creates the data directory, initial snapshot, etc.  Must be called
         before add_points(). The run_measurement() context manager
         calls this automatically.
     '''
+    assert not hasattr(self, "_start_time"), "begin() must be called only once."
+
     if self._target_dir == None:
       self._target_dir = str(datetime.datetime.now()).replace(".", "_").replace(":", "-").replace(" ", "_")
 
     parent_dir, target = os.path.split(self._target_dir)
 
     target = Measurement._path_friendly_str(target)
 
@@ -174,26 +199,56 @@
     self._write_readme()
     self._open_log_file()
     self._copy_jupyter_notebook()
     self.write_snapshot()
 
     self._dat_file = open(os.path.join(self._target_dir, 'tabular_data.dat'), 'w')
 
-    # Write a header, to some extent compatible with the "legacy" QCoDeS format.
+    self._start_time = datetime.datetime.now()
+
+  def _write_tabular_data_header(self):
+    """Write a header in tabular_data.dat.
+
+       The format is to some extent compatible with the "legacy"
+       QCoDeS format, but adds some more metadata.
+
+       This is invoked automatically during the first call to
+       add_points(), rather than during begin(), since we want to
+       infer the column dtypes from the first added points.
+
+    """
     header =  "#\n"
-    header += "# " + "\t".join("%s (%s)" % (c,u) for c,u in zip(self._columns, self._units)) + "\n"
-    header +=  "#\n"
+    header += f"# ondisk_format_version = {'.'.join(map(str, ondisk_format_version))}\n"
+    header += f"# pdata_version = {pdata.__version__}\n"
+    header += f"# jsondiff_version = {jsondiff.__version__}\n"
+    header += f"# numpy_version = {np.__version__}\n"
+    header += f"# python_version = {sys.version}\n"
+    header += "# Measurement started at " + self._start_time.strftime("%Y-%m-%d %H:%M:%S.%f\n")
+    header += "# Column dtypes: " + "\t".join(Measurement._dtype_to_str(dt)
+                                              for dt in self._dtypes) + "\n"
+    header += "#\n"
+    header += "# " + "\t".join(Measurement._replace_disallowed_tabular_data_chars(f"{c} ({u})")
+                               for c,u in zip(self._columns, self._units)) + "\n"
+    header += "#\n"
     try:     self._dat_file.write(header)
     finally: self._dat_file.flush()
 
   def end(self):
-    '''Ends the measurement, i.e. closes and compresses the data set
-        files. The run_measurement() context manager calls this
-        automatically.
+    '''Ends the measurement. Adds final metadata and closes and compresses
+       the data set files. The run_measurement() context manager calls
+       this automatically.
     '''
+    if self._npoints_total == 0: self._write_tabular_data_header()
+
+    footer =  "#\n"
+    footer += "# Measurement ended at " + datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f\n")
+    footer += f"# Snapshot diffs preceding rows (0-based index): {','.join(map(str, self._snapshot_diff_rows))}\n"
+    try:     self._dat_file.write(footer)
+    finally: self._dat_file.flush()
+
     self._close_dat_file()
     self._close_log_file()
 
   def add_points(self, data, snap=None):
     '''Add rows to the data table.
 
         The values for the columns are given
@@ -209,25 +264,28 @@
     for k in data.keys(): assert k in self._columns, '"%s" is not a column in the data table.' % k
 
     for k in self._columns: assert k in data.keys(), f'data must contain "{k}" as a key.'
 
     npts = len(data[self._columns[0]])
     assert all(len(data[k]) == npts for k in data.keys()), 'All appended data columns must be vectors of the same length.'
 
-    if self._npoints_total == 0 and npts>0: self._guess_missing_formatters(data)
+    if self._npoints_total == 0 and npts>0:
+      self._guess_missing_formatters(data)
+      self._write_tabular_data_header()
 
     if snap or (snap == None and self._autosnap): self.write_snapshot()
 
     # Prepare in memory
     rows = "\n".join(
-      "\t".join(f(data[c][i]) for c,f in zip(self._columns, self._formatters))
+      "\t".join(Measurement._replace_disallowed_tabular_data_chars(f(data[c][i]))
+                for c,f in zip(self._columns, self._formatters))
       for i in range(npts) )
     rows += "\n"
 
-    # And write atomically
+    # And write to disk as atomically as possible
     try:     self._dat_file.write(rows)
     finally: self._dat_file.flush()
 
     self._npoints_total += npts
 
     self._check_for_manual_abort()
 
@@ -235,16 +293,17 @@
     ''' Same as add_points but takes scalar inputs for the column values. '''
     for k in data.keys(): assert np.isscalar(data[k]), f'data[{k}] seems to contain more than one value ({data[k]}). Did you mean to call add_point*s* instead?'
     self.add_points(dict( (k, [ data[k] ]) for k in data.keys() ),
                     snap=snap)
 
   def write_snapshot(self, snap=None):
     '''Add a snapshot (delta) file to the data directory. This is called
-automatically whenever you call add_points(), unless you disabled
-autosnapping.'''
+       automatically whenever you call add_points(), unless you
+       disabled autosnapping.
+    '''
     if snap==None:
       snap = self._get_snapshot()
 
     if self._last_snapshot == None:
       with open(os.path.join(self._target_dir, 'snapshot.json'), 'w') as fsnap:
         Measurement._dump_json(snap, fsnap)
 
@@ -260,41 +319,50 @@
 
       i = 0
       while True:
         fname = os.path.join(self._target_dir,
                              'snapshot.row-%u.diff%u.json' % (self._npoints_total, i))
         if not os.path.exists(fname): break
 
-      with open(fname, 'w') as fsnap: Measurement._dump_json(d, fsnap, is_diff=True)
+      self._snapshot_diff_rows.append(self._npoints_total)
+      with open(fname, 'w') as fsnap: Measurement._dump_json(d, fsnap)
 
     self._last_snapshot = snap
 
   def _guess_missing_formatters(self, data):
     '''Given the first points added to the data file, assign reasonable
-        formatters for columns that didn't have one manually specified.
-    '''
+       formatters for columns that didn't have one manually specified.
 
+       Also record original data type of each column.
+    '''
     for i,c in enumerate(self._columns):
-      if self._formatters[i] != None: continue
+      if self._dtypes[i] == None:
+        self._dtypes[i] = type(data[c][0])
 
-      if isinstance(data[c][0], float):
-        self._formatters[i] = lambda x: "%.12e" % x
-      else:
-        self._formatters[i] = str
+      if self._formatters[i] == None:
+        # Infer appropriate formatter
+        if isinstance(data[c][0], float):
+          self._formatters[i] = lambda x: f"{x:.15e}"
+        elif isinstance(data[c][0], complex):
+          self._formatters[i] = lambda x: f"{x.real:.15e}{x.imag:+.15e}j"
+        elif isinstance(data[c][0], datetime.datetime):
+          self._formatters[i] = lambda x: x.strftime('%Y-%m-%d %H:%M:%S.%f')
+        else:
+          self._formatters[i] = str
 
   def _open_log_file(self):
     ''' Open a secondary log file in the data directory. '''
     fn = os.path.join(self._target_dir, 'log.txt')
     if len(logging.getLogger().handlers) > 0:
       formatter = logging.getLogger().handlers[0].formatter
     else:
       formatter = None
 
     self._log_file_handler = logging.FileHandler(fn)
-    self._log_file_handler.setLevel(logging.getLogger().level)
+    self._log_file_handler.setLevel(logging.getLogger().level if self._log_level=="inherit" else self._log_level)
     self._log_file_handler.setFormatter(formatter)
 
     logging.getLogger().addHandler(self._log_file_handler)
     logging.debug('Added log_file_handler. path="%s", formatter="%s"' % (fn, str(formatter)))
 
   def _close_dat_file(self):
     self._dat_file.close()
@@ -369,23 +437,32 @@
     if not hasattr(self, '_abort_signal_initial_mtime'):
       self._abort_signal_initial_mtime = t
       return
 
     if t != self._abort_signal_initial_mtime: raise Exception('Measurement aborted manually.')
 
   @staticmethod
-  def _dump_json(snap, fhandle, is_diff=False):
+  def _dump_json(snap, fhandle):
     json.dump(snap, fhandle, sort_keys=False,
               indent=2, ensure_ascii=False, cls=NumpyJSONEncoder)
 
   @staticmethod
   def _path_friendly_str(s):
     def acceptable_char(x): return x.isalnum() or x in ['#', '-', '=']
     return "".join(x if acceptable_char(x) else '_' for x in s)
 
+  @staticmethod
+  def _replace_disallowed_tabular_data_chars(s): return s.replace("\t","    ").replace("\n", " ").replace("#", " ")
+
+  @staticmethod
+  def _dtype_to_str(dt):
+    """Convert datatype dt to str."""
+    return Measurement._replace_disallowed_tabular_data_chars(
+      f"{dt.__module__}.{dt.__name__}" if hasattr(dt, "__module__") and hasattr(dt, "__name__") else str(dt) )
+
 
 # A bit of a hack allowing controllably aborting a measurement
 # from another process on the same machine.
 abort_signal_file = os.path.join(tempfile.gettempdir(),
                                  'pdata.abort-measurements.signal')
 def abort_measurements():
   '''Abort all measurements running on this machine after their next
```

### Comparing `proceduraldata-1.1.3/proceduraldata.egg-info/PKG-INFO` & `proceduraldata-2.0.4/proceduraldata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: proceduraldata
-Version: 1.1.3
+Version: 2.0.4
 Summary: Simple-to-understand and robust data storage for experimental data
 Home-page: https://pdata.readthedocs.io/
 Author: Joonas Govenius
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-pdata: Simple-to-understand and robust data storage for experimental data
-=========================================================================
+pdata: Straightforward and robust data storage for experimental data
+====================================================================
 
 This *procedural* data storage package provides a self-contained
 interface **focused exclusively on storing and reading experimental
 data**, using an approach **independent of the specific measurement
 framework used for instrument control**.
 
 The main goals are to provide an interface that:
 
-  * Maximizes the amount of automatically stored metadata, without relying on the experimenter specifying which values are worthy of saving.
-  * Is "procedural" rather than "functional" in terms of the API the experimenter sees, as procedural programming tends to be easier to understand for a typical experimental physicist.
+  * Automatically stores a lot of metadata, including parameters that change during a measurement.
+  * Is *procedural* rather than *functional* in terms of the API the experimenter sees, as procedural programming tends to be easier to understand for a typical experimental physicist.
+  * Uses standard Python flow-control constructs (for, while, if, etc.) for looping over setpoints.
   * The API aims to be self-explanatory, wherever possible.
 
 In practice, the experimenter calls an explicit :code:`add_points(<new
 data points>)` function to add rows to a traditional table of data
 points, with user-defined columns. In the background, **pdata
-automatically records all changes to instrument parameters**, each
+automatically records all changes to instrument parameters** each
 time :code:`add_points` is called.
 
-In addition, pdata provides useful helpers for reading back the
-automatically recorded instrument parameters.
+In addition, pdata provides useful helpers for reading back the data,
+including automatically recorded instrument parameters, basic helpers
+for visualization, and good export capabilities to other tools for
+further analysis.
+
+Getting started/Full documentation
+----------------------------------
 
 See the `documentation <http://pdata.readthedocs.io>`_ at RTD for
 instructions on getting started.
 
 MIT License
 
 Copyright (c) 2016 Joonas Govenius
```

### Comparing `proceduraldata-1.1.3/setup.cfg` & `proceduraldata-2.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 	ipython
 	ipympl
 	ipylab
 	notebook
 	ipywidgets
 	matplotlib
 	uncertainties
+	xarray
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

