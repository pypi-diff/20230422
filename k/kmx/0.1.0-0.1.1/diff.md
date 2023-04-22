# Comparing `tmp/kmx-0.1.0.tar.gz` & `tmp/kmx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmx-0.1.0.tar", last modified: Sun Mar 12 09:47:39 2023, max compression
+gzip compressed data, was "kmx-0.1.1.tar", last modified: Sat Apr 22 11:19:07 2023, max compression
```

## Comparing `kmx-0.1.0.tar` & `kmx-0.1.1.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)    11357 2023-02-03 17:16:21.000000 kmx-0.1.0/LICENSE
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      259 2023-03-12 09:47:39.281404 kmx-0.1.0/PKG-INFO
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        5 2023-02-03 17:16:21.000000 kmx-0.1.0/README.md
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.261404 kmx-0.1.0/kmx/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        0 2023-02-03 17:20:27.000000 kmx-0.1.0/kmx/__init__.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.269404 kmx-0.1.0/kmx/agents/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1493 2023-03-04 17:03:04.000000 kmx-0.1.0/kmx/agents/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2125 2023-03-04 15:49:43.000000 kmx-0.1.0/kmx/agents/base.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      309 2023-03-03 14:27:52.000000 kmx-0.1.0/kmx/agents/decorators.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     5203 2023-03-04 17:03:04.000000 kmx-0.1.0/kmx/agents/generic.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.277404 kmx-0.1.0/kmx/behaviours/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      472 2023-03-04 17:12:31.000000 kmx-0.1.0/kmx/behaviours/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      845 2023-03-04 17:10:36.000000 kmx-0.1.0/kmx/behaviours/base.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      339 2023-03-04 10:31:03.000000 kmx-0.1.0/kmx/behaviours/decorators.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1684 2023-03-04 18:56:45.000000 kmx-0.1.0/kmx/behaviours/flow.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      917 2023-02-26 21:46:49.000000 kmx-0.1.0/kmx/behaviours/periodic.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      399 2023-02-27 18:39:18.000000 kmx-0.1.0/kmx/behaviours/simple.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.277404 kmx-0.1.0/kmx/containers/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      653 2023-03-03 14:27:52.000000 kmx-0.1.0/kmx/containers/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2227 2023-03-03 14:27:52.000000 kmx-0.1.0/kmx/containers/base.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)    10669 2023-03-08 20:15:09.000000 kmx-0.1.0/kmx/containers/generic.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/db/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      117 2023-02-15 19:11:20.000000 kmx-0.1.0/kmx/db/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      759 2023-02-26 13:01:08.000000 kmx-0.1.0/kmx/db/beanie_db.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      936 2023-03-04 17:15:53.000000 kmx-0.1.0/kmx/exceptions.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/flows/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      154 2023-02-26 14:04:34.000000 kmx-0.1.0/kmx/flows/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1501 2023-02-26 12:29:10.000000 kmx-0.1.0/kmx/flows/db.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      298 2023-02-25 20:36:16.000000 kmx-0.1.0/kmx/flows/exceptions.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     3261 2023-02-25 15:14:18.000000 kmx-0.1.0/kmx/flows/flow.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      103 2023-02-26 14:04:34.000000 kmx-0.1.0/kmx/flows/models.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     9307 2023-03-04 17:17:11.000000 kmx-0.1.0/kmx/flows/processor.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2738 2023-02-26 20:10:25.000000 kmx-0.1.0/kmx/flows/tasks.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/models/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)       42 2023-03-03 14:27:52.000000 kmx-0.1.0/kmx/models/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      232 2023-02-12 17:51:38.000000 kmx-0.1.0/kmx/models/message.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      585 2023-03-08 19:46:17.000000 kmx-0.1.0/kmx/models/rpc.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/services/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        0 2023-02-03 17:23:19.000000 kmx-0.1.0/kmx/services/__init__.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/services/locker/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      417 2023-02-24 22:24:26.000000 kmx-0.1.0/kmx/services/locker/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2185 2023-03-04 17:17:11.000000 kmx-0.1.0/kmx/services/locker/redis.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/services/logger/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      315 2023-02-03 17:28:48.000000 kmx-0.1.0/kmx/services/logger/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      286 2023-02-25 14:31:05.000000 kmx-0.1.0/kmx/services/logger/dummy.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      526 2023-02-03 17:29:37.000000 kmx-0.1.0/kmx/services/logger/logging.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/services/message_consumer/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      380 2023-02-12 17:51:17.000000 kmx-0.1.0/kmx/services/message_consumer/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1173 2023-02-12 17:51:24.000000 kmx-0.1.0/kmx/services/message_consumer/dummy.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1812 2023-02-12 17:51:38.000000 kmx-0.1.0/kmx/services/message_consumer/kafka.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/services/message_producer/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      279 2023-02-14 12:52:41.000000 kmx-0.1.0/kmx/services/message_producer/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)       39 2023-02-05 20:39:00.000000 kmx-0.1.0/kmx/services/message_producer/dummy.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1179 2023-02-05 22:34:42.000000 kmx-0.1.0/kmx/services/message_producer/kafka.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.281404 kmx-0.1.0/kmx/services/rpc/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      343 2023-03-08 19:34:17.000000 kmx-0.1.0/kmx/services/rpc/__init__.py
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2790 2023-03-08 20:17:01.000000 kmx-0.1.0/kmx/services/rpc/redic_rpc_caller.py
-drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-03-12 09:47:39.269404 kmx-0.1.0/kmx.egg-info/
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      259 2023-03-12 09:47:39.000000 kmx-0.1.0/kmx.egg-info/PKG-INFO
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1256 2023-03-12 09:47:39.000000 kmx-0.1.0/kmx.egg-info/SOURCES.txt
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        1 2023-03-12 09:47:39.000000 kmx-0.1.0/kmx.egg-info/dependency_links.txt
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      106 2023-03-12 09:47:39.000000 kmx-0.1.0/kmx.egg-info/requires.txt
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        4 2023-03-12 09:47:39.000000 kmx-0.1.0/kmx.egg-info/top_level.txt
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      104 2023-02-03 17:18:07.000000 kmx-0.1.0/pyproject.toml
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)       38 2023-03-12 09:47:39.281404 kmx-0.1.0/setup.cfg
--rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      588 2023-03-12 09:45:52.000000 kmx-0.1.0/setup.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.230454 kmx-0.1.1/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)    11357 2023-02-27 07:41:42.000000 kmx-0.1.1/LICENSE
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      259 2023-04-22 11:19:07.230454 kmx-0.1.1/PKG-INFO
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        5 2023-02-27 07:41:42.000000 kmx-0.1.1/README.md
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.214454 kmx-0.1.1/kmx/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        0 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/__init__.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.218454 kmx-0.1.1/kmx/agents/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1493 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/agents/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2125 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/agents/base.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      309 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/agents/decorators.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     5203 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/agents/generic.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.218454 kmx-0.1.1/kmx/behaviours/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      472 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/behaviours/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      845 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/behaviours/base.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      339 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/behaviours/decorators.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1799 2023-04-22 11:05:50.000000 kmx-0.1.1/kmx/behaviours/flow.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      917 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/behaviours/periodic.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      399 2023-02-27 16:14:07.000000 kmx-0.1.1/kmx/behaviours/simple.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.218454 kmx-0.1.1/kmx/containers/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      653 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/containers/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2227 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/containers/base.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)    10669 2023-03-29 07:57:54.000000 kmx-0.1.1/kmx/containers/generic.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.222454 kmx-0.1.1/kmx/db/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      117 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/db/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      759 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/db/beanie_db.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      936 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/exceptions.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.222454 kmx-0.1.1/kmx/flows/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      154 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/flows/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1501 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/flows/db.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      298 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/flows/exceptions.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     3261 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/flows/flow.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      103 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/flows/models.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     9186 2023-04-22 10:49:22.000000 kmx-0.1.1/kmx/flows/processor.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2738 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/flows/tasks.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.222454 kmx-0.1.1/kmx/models/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)       42 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/models/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      232 2023-02-27 17:01:43.000000 kmx-0.1.1/kmx/models/message.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      585 2023-03-29 07:57:54.000000 kmx-0.1.1/kmx/models/rpc.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.222454 kmx-0.1.1/kmx/services/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        0 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/__init__.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.226454 kmx-0.1.1/kmx/services/clock/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      495 2023-04-22 09:58:04.000000 kmx-0.1.1/kmx/services/clock/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      997 2023-04-22 10:19:49.000000 kmx-0.1.1/kmx/services/clock/alter_clock.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      501 2023-04-22 09:58:37.000000 kmx-0.1.1/kmx/services/clock/system_clock.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.226454 kmx-0.1.1/kmx/services/locker/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      417 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/locker/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2185 2023-03-07 09:56:53.000000 kmx-0.1.1/kmx/services/locker/redis.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.226454 kmx-0.1.1/kmx/services/logger/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      315 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/logger/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      286 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/logger/dummy.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      526 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/logger/logging.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.226454 kmx-0.1.1/kmx/services/message_consumer/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      380 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/message_consumer/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1173 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/message_consumer/dummy.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1812 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/message_consumer/kafka.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.226454 kmx-0.1.1/kmx/services/message_producer/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      279 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/message_producer/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)       39 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/message_producer/dummy.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1179 2023-02-27 07:41:42.000000 kmx-0.1.1/kmx/services/message_producer/kafka.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.230454 kmx-0.1.1/kmx/services/rpc/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      343 2023-03-29 07:57:54.000000 kmx-0.1.1/kmx/services/rpc/__init__.py
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     2790 2023-03-29 07:57:54.000000 kmx-0.1.1/kmx/services/rpc/redic_rpc_caller.py
+drwxrwxr-x   0 akvarats  (1000) akvarats  (1000)        0 2023-04-22 11:19:07.218454 kmx-0.1.1/kmx.egg-info/
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      259 2023-04-22 11:19:07.000000 kmx-0.1.1/kmx.egg-info/PKG-INFO
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)     1356 2023-04-22 11:19:07.000000 kmx-0.1.1/kmx.egg-info/SOURCES.txt
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        1 2023-04-22 11:19:07.000000 kmx-0.1.1/kmx.egg-info/dependency_links.txt
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      106 2023-04-22 11:19:07.000000 kmx-0.1.1/kmx.egg-info/requires.txt
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)        4 2023-04-22 11:19:07.000000 kmx-0.1.1/kmx.egg-info/top_level.txt
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      104 2023-02-27 07:41:42.000000 kmx-0.1.1/pyproject.toml
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)       38 2023-04-22 11:19:07.230454 kmx-0.1.1/setup.cfg
+-rw-rw-r--   0 akvarats  (1000) akvarats  (1000)      588 2023-04-22 11:18:10.000000 kmx-0.1.1/setup.py
```

### Comparing `kmx-0.1.0/LICENSE` & `kmx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/agents/__init__.py` & `kmx-0.1.1/kmx/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/agents/base.py` & `kmx-0.1.1/kmx/agents/base.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/agents/generic.py` & `kmx-0.1.1/kmx/agents/generic.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/behaviours/base.py` & `kmx-0.1.1/kmx/behaviours/base.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/behaviours/flow.py` & `kmx-0.1.1/kmx/behaviours/flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,24 +23,28 @@
         self.flow_processor: Optional[FlowProcessor] = None
         self.flows: Optional[FlowPack] = None
 
     @abc.abstractmethod
     def create_flows(self) -> FlowPack:
         """ """
 
+    def create_flow_processor(self) -> FlowProcessor:
+        """ """
+        return FlowProcessor(
+            flows=self.flows,
+            logger=self.logger,
+            locker=self.locker()
+        )
+
     async def run(self):
         """ 
         Старт поведения по работе с потоками
         """
         self.flows = self.create_flows()
-        self.flow_processor = FlowProcessor(
-            flows=self.flows,
-            logger=self.logger,
-            locker=self.locker()
-        )
+        self.flow_processor = self.create_flow_processor()
 
         self.logger.info(f'Added flows: {",".join(self.flows.flow_names)}')
 
         asyncio.create_task(self.flow_processor.scheduler())
 
     async def run_flow(self, flow: Flow, params: Any = None, delay: int = None):
         """ """
```

### Comparing `kmx-0.1.0/kmx/behaviours/periodic.py` & `kmx-0.1.1/kmx/behaviours/periodic.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/containers/__init__.py` & `kmx-0.1.1/kmx/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/containers/base.py` & `kmx-0.1.1/kmx/containers/base.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/containers/generic.py` & `kmx-0.1.1/kmx/containers/generic.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/db/beanie_db.py` & `kmx-0.1.1/kmx/db/beanie_db.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/exceptions.py` & `kmx-0.1.1/kmx/exceptions.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/flows/db.py` & `kmx-0.1.1/kmx/flows/db.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/flows/flow.py` & `kmx-0.1.1/kmx/flows/flow.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/flows/processor.py` & `kmx-0.1.1/kmx/flows/processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterable, Any
+from typing import AsyncIterable, Any, Optional
 
 import asyncio
 import datetime
 import uuid
 
 from pydantic import BaseModel, ValidationError
 
@@ -11,30 +11,34 @@
 
 from kmx.services.locker import Locker
 from kmx.exceptions import LockTimeout
 
 from kmx.services.logger import Logger
 from kmx.services.logger.dummy import DummyLogger
 
+from kmx.services.clock import Clock
+from kmx.services.clock.system_clock import SystemClock
+
 from .flow import Flow, FlowPack
 from .models import FlowRun
 from .tasks import FlowTask
 from .db import DbFlowRun, DbFlowRunState, DbFlowTaskRun, DbFlowTaskRunState, DbActiveFlowRunView, \
     DbFinishedFlowTaskRunView
 from .exceptions import DelayFlowTask, StopFlowRun
 
 
 class FlowProcessor:
 
-    def __init__(self, flows: FlowPack, locker: Locker, logger: Logger | None = None):
+    def __init__(self, flows: FlowPack, locker: Locker, logger: Optional[Logger] = None, clock: Optional[Clock] = None):
         self.flows = flows
         self.locker = locker
         self.start_delay = 1
         self.delay = 0.05
         self.logger = logger or DummyLogger()
+        self.clock = clock or SystemClock()
 
     async def run_flow(self, flow: Flow, params: Any = None, delay: int = None) -> DbFlowRun:
         """
         Run flow
 
         Args:
             flow: flow definition to run
@@ -47,16 +51,16 @@
         flow_run = DbFlowRun(
             flow_name=flow.name,
             uid=str(uuid.uuid4()).replace('-', ''),
             context={
                 'flow_params': params.dict() if isinstance(params, BaseModel) else params
             },
             state=DbFlowRunState.ACTIVE,
-            created_at=datetime.datetime.now(datetime.timezone.utc),
-            delayed_until=datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(seconds=delay) if delay else None,
+            created_at=self.clock.now(),
+            delayed_until=self.clock.now() + datetime.timedelta(seconds=delay) if delay else None,
             finished_at=None
         )
 
         await flow_run.create()
 
         self.logger.info(f'Flow `{flow.name}` started with params {params} and delay {delay} sec')
 
@@ -67,15 +71,15 @@
         self.logger.info('Start flow scheduling')
         await asyncio.sleep(self.start_delay)
         while True:
             has_active_runs = False
             async for flow_run in self.fetch_active_flow_runs():
                 has_active_runs = True
                 if flow_run.delayed_until is not None and \
-                        flow_run.delayed_until > datetime.datetime.now(datetime.timezone.utc):
+                        flow_run.delayed_until > self.clock.now():
                     continue
                 try:
                     async with self.locker.lock(flow_run.uid):
                         await self.handle_active_flow_run(flow_run)
                 except LockTimeout:
                     # поток уже заблокирован, выполняется где-то
                     continue
@@ -118,15 +122,15 @@
         flow = self.flows.get_flow_by_name(flow_run_view.flow_name)
         tasks_to_run = self.get_tasks_to_run(flow, done_task_names)
 
         if not tasks_to_run:
             # There is no a task in the flow to run. Finalize it!
             await flow_run.update(Set({
                 DbFlowRun.state: DbFlowRunState.FINISHED,
-                DbFlowRun.finished_at: datetime.datetime.now(datetime.timezone.utc)  
+                DbFlowRun.finished_at: self.clock.now()
             }))
             self.logger.info(
                 f'Flow `{flow.name}` with params {flow_run.context.get("flow_params")} finished: all tasks completed')
         else:
             for flow_task in tasks_to_run:
                 asyncio.create_task(self.run_task(flow, flow_run, flow_task))
 
@@ -144,15 +148,15 @@
     async def run_task(self, flow: Flow, flow_run: DbFlowRun, flow_task: FlowTask):
         """ """
         # create task_run for flow_task
         task_run = DbFlowTaskRun(
             flow_run_uid=flow_run.uid,
             task_name=flow_task.name,
             state=DbFlowTaskRunState.ACTIVE,
-            created_at=datetime.datetime.now(datetime.timezone.utc),
+            created_at=self.clock.now(),
             finished_at=None
         )
         await task_run.insert()
 
         try:
             context = flow.context_model.parse_obj(
                 flow_run.context) if flow.context_model is not None else flow_run.context
@@ -164,15 +168,15 @@
             context['_error'] = {
                 'code': 'validation-error',
                 'text': f'{e}'
             }
 
             await flow_run.update(Set({
                 DbFlowRun.state: DbFlowTaskRunState.FINISHED,
-                DbFlowRun.finished_at: datetime.datetime.now(datetime.timezone.utc),
+                DbFlowRun.finished_at: self.clock.now(),
                 DbFlowRun.context: context
             }))
             self.logger.error(
                 f'Flow `{flow.name}` with params {context.get("flow_params")} finished with '
                 f'context validation error: {e}')
             return
 
@@ -182,26 +186,25 @@
             context = context.dict() if isinstance(context, BaseModel) else context
             context['_reason'] = {
                 'code': 'worflow-stopped',
                 'text': f'Worflow was stopped: {e}'
             }
             await flow_run.update(Set({
                 DbFlowRun.state: DbFlowTaskRunState.FINISHED,
-                DbFlowRun.finished_at: datetime.datetime.now(datetime.timezone.utc),
+                DbFlowRun.finished_at: self.clock.now(),
                 DbFlowRun.context: context
             }))
             await task_run.delete()
             self.logger.info(
                 f'Flow `{flow.name}` with params {context.get("flow_params")} finished by command: {e}'
             )
 
         except DelayFlowTask as e:
             await flow_run.update(Set({
-                DbFlowRun.delayed_until: datetime.datetime.now(datetime.timezone.utc) + datetime.timedelta(
-                    seconds=e.delay),
+                DbFlowRun.delayed_until: self.clock.now() + datetime.timedelta(seconds=e.delay),
                 DbFlowRun.context: context.dict() if isinstance(context, BaseModel) else context
             }))
             await task_run.delete()
 
         except Exception as e:
             # получено непонятное сообщение, финализируем даг
             self.logger.exception(
@@ -209,15 +212,15 @@
             context = context.dict() if isinstance(context, BaseModel) else context
             context['_reason'] = {
                 'code': 'exception',
                 'text': f'{e}'
             }
             await flow_run.update(Set({
                 DbFlowRun.state: DbFlowTaskRunState.FINISHED,
-                DbFlowRun.finished_at: datetime.datetime.now(datetime.timezone.utc),
+                DbFlowRun.finished_at: self.clock.now(),
                 DbFlowRun.context: context
             }))
             await task_run.delete()
             self.logger.error(
                 f'Flow `{flow.name}` with params {context.get("flow_params")} finished with exception: {e}'
             )
 
@@ -226,9 +229,9 @@
             await flow_run.update(Set({
                 DbFlowRun.context: context.dict() if isinstance(context, BaseModel) else context
             }))
 
             # in any case mark task_run as finished
             await task_run.update(Set({
                 DbFlowTaskRun.state: DbFlowTaskRunState.FINISHED,
-                DbFlowTaskRun.finished_at: datetime.datetime.now(datetime.timezone.utc)
+                DbFlowTaskRun.finished_at: self.clock.now()
             }))
```

### Comparing `kmx-0.1.0/kmx/flows/tasks.py` & `kmx-0.1.1/kmx/flows/tasks.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/models/rpc.py` & `kmx-0.1.1/kmx/models/rpc.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/services/locker/redis.py` & `kmx-0.1.1/kmx/services/locker/redis.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/services/logger/logging.py` & `kmx-0.1.1/kmx/services/logger/logging.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/services/message_consumer/dummy.py` & `kmx-0.1.1/kmx/services/message_consumer/dummy.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/services/message_consumer/kafka.py` & `kmx-0.1.1/kmx/services/message_consumer/kafka.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/services/message_producer/kafka.py` & `kmx-0.1.1/kmx/services/message_producer/kafka.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx/services/rpc/redic_rpc_caller.py` & `kmx-0.1.1/kmx/services/rpc/redic_rpc_caller.py`

 * *Files identical despite different names*

### Comparing `kmx-0.1.0/kmx.egg-info/SOURCES.txt` & `kmx-0.1.1/kmx.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 kmx/flows/models.py
 kmx/flows/processor.py
 kmx/flows/tasks.py
 kmx/models/__init__.py
 kmx/models/message.py
 kmx/models/rpc.py
 kmx/services/__init__.py
+kmx/services/clock/__init__.py
+kmx/services/clock/alter_clock.py
+kmx/services/clock/system_clock.py
 kmx/services/locker/__init__.py
 kmx/services/locker/redis.py
 kmx/services/logger/__init__.py
 kmx/services/logger/dummy.py
 kmx/services/logger/logging.py
 kmx/services/message_consumer/__init__.py
 kmx/services/message_consumer/dummy.py
```

### Comparing `kmx-0.1.0/setup.py` & `kmx-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='kmx',
-    version='0.1.0',
+    version='0.1.1',
     author='akvarats',
 
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
```

