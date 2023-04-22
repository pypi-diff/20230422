# Comparing `tmp/recon_lw-2.0.0.dev4757666702.tar.gz` & `tmp/recon_lw-2.0.0.dev4773922411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4757666702.tar", last modified: Fri Apr 21 06:18:15 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4773922411.tar", last modified: Sat Apr 22 17:25:30 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4757666702.tar` & `recon_lw-2.0.0.dev4773922411.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-21 06:17:57.000000 recon_lw-2.0.0.dev4757666702/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    19652 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 06:18:15.000000 recon_lw-2.0.0.dev4757666702/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-21 06:17:50.000000 recon_lw-2.0.0.dev4757666702/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-22 17:25:08.000000 recon_lw-2.0.0.dev4773922411/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19709 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13710 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-22 17:25:30.000000 recon_lw-2.0.0.dev4773922411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-22 17:25:00.000000 recon_lw-2.0.0.dev4773922411/setup.py
```

### Comparing `recon_lw-2.0.0.dev4757666702/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4773922411/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4757666702/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4773922411/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4757666702/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4773922411/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,19 +99,20 @@
                                                      ok=False,
                                                      body=result,
                                                      parentId=parent_event["eventId"])
                 update_event["attachedMessageIds"] = [mess["messageId"]]
                 events.append(update_event)
             if log_entries is not None:
                 for log_book in log_entries:
+                    log_book["timestamp"] = mess["timestamp"]
                     log_book["sessionId"] = mess["sessionId"]
                     log_book["book_id"] = book_id
                     log_book["operation"] = operation.__name__
                     log_book["operation_params"] = initial_parameters
-                    if log_books_filter is not None and log_books_filter(log_book):
+                    if log_books_filter is None or log_books_filter(log_book):
                         log_event = recon_lw.create_event("OrderBook:" + mess["sessionId"],
                                                           "OrderBook",
                                                           event_sequence,
                                                           ok=True,
                                                           body=log_book,
                                                           parentId=parent_event["eventId"])
                         log_event["attachedMessageIds"] = [mess["messageId"]]
```

### Comparing `recon_lw-2.0.0.dev4757666702/setup.py` & `recon_lw-2.0.0.dev4773922411/setup.py`

 * *Files identical despite different names*

