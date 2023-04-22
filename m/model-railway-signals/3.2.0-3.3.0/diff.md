# Comparing `tmp/model-railway-signals-3.2.0.tar.gz` & `tmp/model-railway-signals-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/model-railway-signals-3.2.0.tar", last modified: Thu Apr  6 13:26:44 2023, max compression
+gzip compressed data, was "dist/model-railway-signals-3.3.0.tar", last modified: Sat Apr 22 16:49:21 2023, max compression
```

## Comparing `model-railway-signals-3.2.0.tar` & `model-railway-signals-3.3.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/
--rw-r--r--   0 pi        (1000) pi        (1000)      127 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     5616 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     4344 2023-04-06 12:56:39.000000 model-railway-signals-3.2.0/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals/
--rw-r--r--   0 pi        (1000) pi        (1000)     6599 2023-03-25 17:29:52.000000 model-railway-signals-3.2.0/model_railway_signals/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      325 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/__main__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals/editor/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    40363 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    23000 2023-03-25 17:51:24.000000 model-railway-signals-3.2.0/model_railway_signals/editor/configure_point.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21648 2023-03-25 17:52:50.000000 model-railway-signals-3.2.0/model_railway_signals/editor/configure_section.py
--rw-r--r--   0 pi        (1000) pi        (1000)    58458 2023-03-26 20:06:50.000000 model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal.py
--rw-r--r--   0 pi        (1000) pi        (1000)    53245 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal_tab1.py
--rw-r--r--   0 pi        (1000) pi        (1000)    21531 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal_tab2.py
--rw-r--r--   0 pi        (1000) pi        (1000)    34010 2023-03-25 17:35:26.000000 model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal_tab3.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2115 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/editor.py
--rw-r--r--   0 pi        (1000) pi        (1000)    32973 2023-04-06 13:22:53.000000 model-railway-signals-3.2.0/model_railway_signals/editor/menubar.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/
--rw-r--r--   0 pi        (1000) pi        (1000)     5501 2023-04-06 08:55:04.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    29404 2023-04-06 12:06:19.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9563 2023-04-06 08:49:36.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    12181 2023-04-06 08:00:14.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_instruments.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7428 2023-04-06 08:28:36.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_lines.py
--rw-r--r--   0 pi        (1000) pi        (1000)    20303 2023-04-06 11:36:45.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_points.py
--rw-r--r--   0 pi        (1000) pi        (1000)    19032 2023-04-06 08:27:53.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_sections.py
--rw-r--r--   0 pi        (1000) pi        (1000)    50533 2023-04-06 08:29:57.000000 model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_signals.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)      644 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/block_instrument.png
--rw-r--r--   0 pi        (1000) pi        (1000)      284 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/colour_light.png
--rw-r--r--   0 pi        (1000) pi        (1000)      295 2023-03-25 09:50:18.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/ground_disc.png
--rw-r--r--   0 pi        (1000) pi        (1000)      277 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/ground_position.png
--rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/left_hand_point.png
--rw-r--r--   0 pi        (1000) pi        (1000)      170 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/line.png
--rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/right_hand_point.png
--rw-r--r--   0 pi        (1000) pi        (1000)      208 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/semaphore.png
--rw-r--r--   0 pi        (1000) pi        (1000)      670 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/editor/resources/track_section.png
--rw-r--r--   0 pi        (1000) pi        (1000)    52821 2023-04-06 12:01:06.000000 model-railway-signals-3.2.0/model_railway_signals/editor/run_layout.py
--rw-r--r--   0 pi        (1000) pi        (1000)    39689 2023-03-28 08:52:12.000000 model-railway-signals-3.2.0/model_railway_signals/editor/schematic.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6955 2023-04-06 13:00:47.000000 model-railway-signals-3.2.0/model_railway_signals/editor/settings.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals/library/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    46118 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/block_instruments.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6542 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/common.py
--rw-r--r--   0 pi        (1000) pi        (1000)    43683 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/dcc_control.py
--rw-r--r--   0 pi        (1000) pi        (1000)    22911 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/file_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    18681 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/mqtt_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    31806 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/pi_sprog_interface.py
--rw-r--r--   0 pi        (1000) pi        (1000)    26338 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/points.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/
--rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-01.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-02.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-03.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-04.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    30722 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/resources/telegraph-key-01.wav
--rw-r--r--   0 pi        (1000) pi        (1000)    52946 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/signals.py
--rw-r--r--   0 pi        (1000) pi        (1000)    46680 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/signals_colour_lights.py
--rw-r--r--   0 pi        (1000) pi        (1000)    37156 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/signals_common.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7444 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/signals_ground_disc.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9827 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/signals_ground_position.py
--rw-r--r--   0 pi        (1000) pi        (1000)    55637 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/signals_semaphores.py
--rw-r--r--   0 pi        (1000) pi        (1000)    25913 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/track_sections.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13806 2023-03-25 09:50:20.000000 model-railway-signals-3.2.0/model_railway_signals/library/track_sensors.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/model_railway_signals.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     5616 2023-04-06 13:26:41.000000 model-railway-signals-3.2.0/model_railway_signals.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     3016 2023-04-06 13:26:41.000000 model-railway-signals-3.2.0/model_railway_signals.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-06 13:26:41.000000 model-railway-signals-3.2.0/model_railway_signals.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2023-04-06 13:26:41.000000 model-railway-signals-3.2.0/model_railway_signals.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       22 2023-04-06 13:26:41.000000 model-railway-signals-3.2.0/model_railway_signals.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-06 13:26:44.000000 model-railway-signals-3.2.0/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      979 2023-04-06 12:53:37.000000 model-railway-signals-3.2.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)      127 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/MANIFEST.in
+-rw-r--r--   0 pi        (1000) pi        (1000)     5715 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     4435 2023-04-22 16:44:27.000000 model-railway-signals-3.3.0/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6599 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      325 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/__main__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/editor/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    42645 2023-04-21 13:57:37.000000 model-railway-signals-3.3.0/model_railway_signals/editor/common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    17653 2023-04-22 13:10:39.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_instrument.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    20790 2023-04-21 14:01:49.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_point.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21713 2023-04-06 17:26:45.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_section.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    58487 2023-04-06 17:00:22.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    53376 2023-04-09 07:33:17.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab1.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    21575 2023-04-06 17:18:07.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab2.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    34207 2023-04-06 17:10:41.000000 model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab3.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    19118 2023-04-22 16:13:13.000000 model-railway-signals-3.3.0/model_railway_signals/editor/editor.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    18788 2023-04-10 08:10:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/menubar_windows.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/
+-rw-r--r--   0 pi        (1000) pi        (1000)     5501 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    32108 2023-04-10 08:57:59.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9563 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13272 2023-04-22 11:59:29.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_instruments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7428 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_lines.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    20303 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_points.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    19032 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_sections.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    50499 2023-04-06 16:20:27.000000 model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_signals.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      644 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/block_instrument.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      284 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/colour_light.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      295 2023-03-25 09:50:18.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/ground_disc.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      277 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/ground_position.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      247 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/left_hand_point.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      170 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/line.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      246 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/right_hand_point.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      208 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/semaphore.png
+-rw-r--r--   0 pi        (1000) pi        (1000)      670 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/editor/resources/track_section.png
+-rw-r--r--   0 pi        (1000) pi        (1000)    53684 2023-04-22 14:12:59.000000 model-railway-signals-3.3.0/model_railway_signals/editor/run_layout.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    40127 2023-04-22 16:11:15.000000 model-railway-signals-3.3.0/model_railway_signals/editor/schematic.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6955 2023-04-22 16:45:15.000000 model-railway-signals-3.3.0/model_railway_signals/editor/settings.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/library/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    49745 2023-04-21 15:00:53.000000 model-railway-signals-3.3.0/model_railway_signals/library/block_instruments.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6542 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/library/common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    43683 2023-04-06 13:44:14.000000 model-railway-signals-3.3.0/model_railway_signals/library/dcc_control.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    23375 2023-04-21 13:14:12.000000 model-railway-signals-3.3.0/model_railway_signals/library/file_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    18681 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/mqtt_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    31806 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/pi_sprog_interface.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    26355 2023-04-06 17:38:56.000000 model-railway-signals-3.3.0/model_railway_signals/library/points.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/
+-rw-r--r--   0 pi        (1000) pi        (1000)        0 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-01.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-02.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-03.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    80808 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-04.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    30722 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/resources/telegraph-key-01.wav
+-rw-r--r--   0 pi        (1000) pi        (1000)    52852 2023-04-06 15:39:47.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    46658 2023-04-06 15:40:23.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_colour_lights.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    37138 2023-04-06 15:56:51.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_common.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     7412 2023-04-06 16:06:14.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_disc.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9805 2023-04-06 16:04:36.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_position.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    55615 2023-04-06 16:07:03.000000 model-railway-signals-3.3.0/model_railway_signals/library/signals_semaphores.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    25918 2023-04-06 15:44:18.000000 model-railway-signals-3.3.0/model_railway_signals/library/track_sections.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13806 2023-03-25 09:50:20.000000 model-railway-signals-3.3.0/model_railway_signals/library/track_sensors.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     5715 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     3077 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       19 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       22 2023-04-22 16:49:18.000000 model-railway-signals-3.3.0/model_railway_signals.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-22 16:49:21.000000 model-railway-signals-3.3.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      979 2023-04-22 16:44:43.000000 model-railway-signals-3.3.0/setup.py
```

### Comparing `model-railway-signals-3.2.0/PKG-INFO` & `model-railway-signals-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-railway-signals
-Version: 3.2.0
+Version: 3.3.0
 Summary: Create your own DCC model railway signalling scheme
 Home-page: https://github.com/johnrm174/model-railway-signalling
 Author: johnrm174
 Author-email: johnrm17418@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 2, June 1991
 Description: # model-railway-signalling
         
@@ -16,24 +16,25 @@
         
         ## Layout editor
         
         From Release 3.0.0, the schematic editor application enables automated and interlocked layout signalling 
         schemes to be designed and configured without the need to write any code. Note that the editor is in
         active development so any comments and suggestions for future features are welcome.
         
-        What's supported in Release 3.2.0:
+        What's supported in Release 3.3.0:
         * Draw your layout schematic with lines, points, signals and track occupancy sections
         * Define the DCC command sequences to drive the signals and points out on the layout
         * Configure the signals and points to implement protototypical interlocking schemes
         * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
         * Automation of signals as trains traverse the routes that have been configured
         * Save and load your layout schematic and state between running sessions
+        * Block instruments - with interlocking of starting signals
+        * Popup error messages when things go wrong (reduced reliance on logs)
         
         What's coming soon:
-        * Support for block section instruments
         * MQTT networking (for linking layouts)
         * Application documentation
         
         Any bug reports and feedback you may have would be gratefully appreciated - specifically:
         * What aspects are intuitive? What aspects aren't?
         * What aspects do you particularly like?
         * What aspects particularly irritate you?
```

### Comparing `model-railway-signals-3.2.0/README.md` & `model-railway-signals-3.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 ## Layout editor
 
 From Release 3.0.0, the schematic editor application enables automated and interlocked layout signalling 
 schemes to be designed and configured without the need to write any code. Note that the editor is in
 active development so any comments and suggestions for future features are welcome.
 
-What's supported in Release 3.2.0:
+What's supported in Release 3.3.0:
 * Draw your layout schematic with lines, points, signals and track occupancy sections
 * Define the DCC command sequences to drive the signals and points out on the layout
 * Configure the signals and points to implement protototypical interlocking schemes
 * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
 * Automation of signals as trains traverse the routes that have been configured
 * Save and load your layout schematic and state between running sessions
+* Block instruments - with interlocking of starting signals
+* Popup error messages when things go wrong (reduced reliance on logs)
 
 What's coming soon:
-* Support for block section instruments
 * MQTT networking (for linking layouts)
 * Application documentation
 
 Any bug reports and feedback you may have would be gratefully appreciated - specifically:
 * What aspects are intuitive? What aspects aren't?
 * What aspects do you particularly like?
 * What aspects particularly irritate you?
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/__init__.py` & `model-railway-signals-3.3.0/model_railway_signals/__init__.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/common.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #    object_id_selection(integer_entry_box)
 #    dcc_command_entry() - combines dcc_entry_box and state_box
 #    signal_route_selections() - combines int_item_id_entry_box and 5 state_boxes
 #    selection_buttons() - combines 5 RadioButtons
 #    window_controls() - apply/ok/reset/cancel
 #------------------------------------------------------------------------------------
 
-from tkinter import *
+import tkinter as Tk
 
 #------------------------------------------------------------------------------------
 # Class to create a tooltip for a tkinter widget - Acknowledgements to Stack Overflow
 # https://stackoverflow.com/questions/3221956/how-do-i-display-tooltips-in-tkinter
 # Class instance elements intended for external use are:
 #     "text" - to change the tooltip text (e.g. to show error messages)
 #------------------------------------------------------------------------------------
@@ -56,20 +56,20 @@
         
     def showtip(self, event=None):
         x = y = 0
         x, y, cx, cy = self.widget.bbox("insert")
         x += self.widget.winfo_rootx() + 25
         y += self.widget.winfo_rooty() + 20
         # creates a toplevel window
-        self.tw = Toplevel(self.widget)
+        self.tw = Tk.Toplevel(self.widget)
         self.tw.attributes('-topmost',True)
         # Leaves only the label and removes the app window
         self.tw.wm_overrideredirect(True)
         self.tw.wm_geometry("+%d+%d" % (x, y))
-        label = Label(self.tw, text=self.text, justify='left',
+        label = Tk.Label(self.tw, text=self.text, justify='left',
                        background="#ffffff", relief='solid', borderwidth=1,
                        wraplength = self.wraplength)
         label.pack(ipadx=1)
         
     def hidetip(self):
         tw = self.tw
         self.tw= None
@@ -82,22 +82,22 @@
 #    "get_value" - will return the state (False if disabled) (bool)
 #    "disable" - disables/blanks the CB (i.e. sets it to False)
 #    "enable"  enables/loads the CB (with the last state)
 #    "enable1"/"enable2"/"disable1"/"disable2" - as above but provides an
 #        AND function where both flags need to be set to enable the CB
 #------------------------------------------------------------------------------------
 
-class check_box(Checkbutton):
+class check_box(Tk.Checkbutton):
     def __init__(self, parent_frame, label:str, tool_tip:str, width:int=None, callback=None):
         # Create the local instance configuration variables
         # 'selection' is the current CB state and 'state' is the last entered state
         # 'enabled' is the flag to track whether the checkbox is enabled or not
         self.parent_frame = parent_frame
         self.callback = callback
-        self.selection = BooleanVar(self.parent_frame, False)
+        self.selection = Tk.BooleanVar(self.parent_frame, False)
         self.state = False
         self.enabled0 = True
         self.enabled1 = True
         self.enabled2 = True
         # Create the checkbox and associated tool tip
         if width is None: 
             super().__init__(self.parent_frame, text=label, anchor="w",
@@ -162,26 +162,26 @@
 #    "get_value" - will return the current state (False if disabled) (bool)
 #    "disable" - disables/blanks the CB (i.e. sets it to False)
 #    "enable"  enables/loads the CB (with the last state)
 #    "enable1"/"enable2"/"disable1"/"disable2" - as above but provides an
 #        AND function where both flags need to be set to enable the CB
 #------------------------------------------------------------------------------------
 
-class state_box(Checkbutton):
+class state_box(Tk.Checkbutton):
     def __init__(self, parent_frame, label_off:str, label_on:str, tool_tip:str,
                          width:int=None, callback=None, read_only:bool=False):
         # Create the local instance configuration variables
         # 'selection' is the current CB state and 'state' is the last entered state
         # 'enabled' is the flag to track whether the checkbox is enabled or not
         self.parent_frame = parent_frame
         self.callback = callback
         self.labelon = label_on
         self.labeloff = label_off
         self.read_only = read_only
-        self.selection = BooleanVar(self.parent_frame, False)
+        self.selection = Tk.BooleanVar(self.parent_frame, False)
         self.state = False
         self.enabled0 = True
         self.enabled1 = True
         self.enabled2 = True
         # Create the checkbox and associated tool tip
         if width is None: 
             super().__init__(parent_frame, indicatoron = False,
@@ -262,24 +262,24 @@
 # Class methods/objects intended for use by child classes that inherit:
 #    "set_validation_status" - to be called following external validation
 #    "TT.text" - The tooltip for the entry box (to change the tooltip text)
 #    "entry" - is the current entry box value (may or may not be valid)
 #    "value" - is the last validated value of the entry box
 #------------------------------------------------------------------------------------
 
-class entry_box(Entry):
+class entry_box(Tk.Entry):
     def __init__(self, parent_frame, width:int, tool_tip:str, callback=None):
         # Create the local instance configuration variables
         # 'entry' is the current EB value and 'value' is the last entered value
         # 'enabled' is the flag to track whether the checkbox is enabled or not
         # 'tooltip' is the default tooltip text(if no validation errors are present)
         self.parent_frame = parent_frame
         self.callback = callback
         self.tool_tip = tool_tip
-        self.entry = StringVar(self.parent_frame, "")
+        self.entry = Tk.StringVar(self.parent_frame, "")
         self.value = ""
         self.initial_value = ""
         self.enabled0 =  True
         self.enabled1 =  True
         self.enabled2 =  True
         # Create the entry box, event bindings and associated default tooltip
         super().__init__(self.parent_frame, width=width, textvariable=self.entry, justify='center')
@@ -559,16 +559,16 @@
 #               assigned to this item) or is being changed back to the initial value
 #------------------------------------------------------------------------------------
 
 class object_id_selection(integer_entry_box):
     def __init__(self, parent_frame, label:str, exists_function):
         # This is the function to call to see if the object already exists
         self.exists_function = exists_function
-        # Create a Label frame for the UI element
-        self.frame = LabelFrame(parent_frame, text=label)
+        # Create a Label Frame for the UI element
+        self.frame = Tk.LabelFrame(parent_frame, text=label)
         # Call the common base class init function to create the EB
         tool_tip = ("Enter new ID (1-99) \n" + "Once saved/applied any references "+
                     "to this object will be updated in other objects")
         super().__init__(self.frame, width=3, min_value=1, max_value=99,
                          tool_tip=tool_tip, allow_empty=False)
         # Pack the Entry box centrally in the label frame
         self.pack()
@@ -596,21 +596,21 @@
 #    "disable" - disables/blanks the entry box (and associated state button)
 #    "enable"  enables/loads the entry box (and associated state button)
 #------------------------------------------------------------------------------------
 
 class dcc_command_entry():
     def __init__(self, parent_frame):
         # create a frame to pack the two elements into
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         # Create the address entry box and the associated dcc state box
         self.EB = dcc_entry_box(parent_frame, callback=self.eb_updated)
-        self.EB.pack(side=LEFT)
+        self.EB.pack(side=Tk.LEFT)
         self.CB = state_box(parent_frame, label_off="OFF", label_on="ON",
                     width=4, tool_tip="Set the DCC logic for the command")
-        self.CB.pack(side=LEFT)
+        self.CB.pack(side=Tk.LEFT)
     
     def eb_updated(self):
         if self.EB.entry.get() == "":
             self.CB.disable()
         else: self.CB.enable()
 
     def validate(self):
@@ -646,27 +646,27 @@
 #------------------------------------------------------------------------------------
 
 class route_selections():
     def __init__(self, parent_frame, tool_tip:str, read_only=False, callback=None):
         # create the UI Elements for each of the possible route selections
         self.main = state_box(parent_frame, label_off="MAIN", label_on="MAIN",
                 width=5, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.main.pack(side=LEFT)
+        self.main.pack(side=Tk.LEFT)
         self.lh1 = state_box(parent_frame, label_off="LH1", label_on="LH1",
                 width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.lh1.pack(side=LEFT)
+        self.lh1.pack(side=Tk.LEFT)
         self.lh2 = state_box(parent_frame, label_off="LH2", label_on="LH2",
                 width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.lh2.pack(side=LEFT)
+        self.lh2.pack(side=Tk.LEFT)
         self.rh1 = state_box(parent_frame, label_off="RH1", label_on="RH1",
                 width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.rh1.pack(side=LEFT)
+        self.rh1.pack(side=Tk.LEFT)
         self.rh2 = state_box(parent_frame, label_off="RH2", label_on="RH2",
                 width=4, tool_tip=tool_tip, read_only=read_only, callback=callback)
-        self.rh2.pack(side=LEFT)
+        self.rh2.pack(side=Tk.LEFT)
 
     def enable(self):
         self.main.enable()
         self.lh1.enable()
         self.lh2.enable()
         self.rh1.enable()
         self.rh2.enable()
@@ -708,20 +708,20 @@
 #    "disable" - Disables/blanks EB value and all route selection CBs 
 #------------------------------------------------------------------------------------
 
 class signal_route_selections(route_selections):
     def __init__(self, parent_frame, tool_tip:str, exists_function=None,
                   current_id_function=None, read_only:bool=False):
         self.read_only = read_only
-        # Create a frame to hold all the elements
-        self.frame = Frame(parent_frame)
+        # Create a fFrame to hold all the elements
+        self.frame = Tk.Frame(parent_frame)
         # Call the common base class init function to create the EB
         self.EB = int_item_id_entry_box(self.frame, tool_tip=tool_tip, callback=self.eb_updated,
                     exists_function=exists_function, current_id_function=current_id_function)
-        self.EB.pack(side=LEFT)
+        self.EB.pack(side=Tk.LEFT)
         # Disable the EB (we don't use the disable method as we want to display the value_
         if self.read_only: self.EB.configure(state="disabled")
         # Create the UI Elements for each of the possible route selections
         super().__init__(self.frame, tool_tip, read_only)
 
     def eb_updated(self):
         # Enable/disable the checkboxes depending on the EB state
@@ -749,60 +749,96 @@
         super().set_values(signal[1])
         self.eb_updated()
 
     def get_values(self):
         # each signal comprises [sig_id, [main, lh1, lh2, rh1, rh2]]
         # Where each route element is a boolean value (True or False)
         return ( [ self.EB.get_value(), super().get_values() ])
-   
+
+#------------------------------------------------------------------------------------
+# Class for a signal route interlocking frame - uses multiple instances of the
+# signal_route_selection_element which are created when "set_values" is called
+# Public class instance methods provided by this class are:
+#    "set_values" - Populates the list of interlocked signals and their routes
+#------------------------------------------------------------------------------------
+
+class signal_route_interlocking_frame():
+    def __init__(self, parent_frame):
+        # Create the Label Frame for the Signal Interlocking List 
+        self.frame = Tk.LabelFrame(parent_frame, text="Interlocking with signals")
+        self.frame.pack(padx=2, pady=2, fill='x')
+        # These are the lists that hold the references to the subframes and subclasses
+        self.sigelements = []
+        self.subframe = None
+
+    def set_values(self, sig_interlocking_frame:[[int,[bool,bool,bool,bool,bool]],]):
+        # If the lists are not empty (case of "reloading" the config) then destroy
+        # all the UI elements and create them again (the list may have changed)
+        if self.subframe: self.subframe.destroy()
+        self.subframe = Tk.Frame(self.frame)
+        self.subframe.pack()
+        self.sigelements = []
+        # sig_interlocking_frame is a variable length list where each element is [sig_id, interlocked_routes]
+        if sig_interlocking_frame:
+            for sig_interlocking_routes in sig_interlocking_frame:
+                # sig_interlocking_routes comprises [sig_id, [main, lh1, lh2, rh1, rh2]]
+                # Where each route element is a boolean value (True or False)            
+                self.sigelements.append(signal_route_selections(self.subframe,read_only=True,
+                        tool_tip="Edit the appropriate signals\nto configure interlocking"))
+                self.sigelements[-1].frame.pack()
+                self.sigelements[-1].set_values (sig_interlocking_routes)
+        else:
+            self.label = Tk.Label(self.subframe, text="No interlocked signals")
+            self.label.pack()
+
 #------------------------------------------------------------------------------------
 # Class for a frame containing up to 5 radio buttons
 # Class instance elements to use externally are:
 #    "B1" to "B5 - to access the button widgets (i.e. for reconfiguration)
 # Class instance functions to use externally are:
 #    "set_value" - will set the current value (integer 1-5)
 #    "get_value" - will return the last "valid" value (integer 1-5)
 #------------------------------------------------------------------------------------
 
 class selection_buttons():
     def __init__(self, parent_frame, label:str, tool_tip:str, callback=None, 
                         b1=None, b2=None, b3=None, b4=None, b5=None):
         # Create a labelframe to hold the buttons
-        self.frame = LabelFrame(parent_frame, text=label)
-        self.value = IntVar(self.frame, 0)
+        self.frame = Tk.LabelFrame(parent_frame, text=label)
+        self.value = Tk.IntVar(self.frame, 0)
         # This is the external callback to make when a selection is made
         self.callback = callback
         # Create a subframe (so the buttons are centered)
-        self.subframe = Frame(self.frame)
+        self.subframe = Tk.Frame(self.frame)
         self.subframe.pack()
         # Only create as many buttons as we need
         if b1 is not None:
-            self.B1 = Radiobutton(self.subframe, text=b1, anchor='w',
+            self.B1 = Tk.Radiobutton(self.subframe, text=b1, anchor='w',
                 command=self.updated, variable=self.value, value=1)
-            self.B1.pack(side=LEFT, padx=2, pady=2)
+            self.B1.pack(side=Tk.LEFT, padx=2, pady=2)
             self.B1TT = CreateToolTip(self.B1, tool_tip)
         if b2 is not None:
-            self.B2 = Radiobutton(self.subframe, text=b2, anchor='w',
+            self.B2 = Tk.Radiobutton(self.subframe, text=b2, anchor='w',
                 command=self.updated, variable=self.value, value=2)
-            self.B2.pack(side=LEFT, padx=2, pady=2)
+            self.B2.pack(side=Tk.LEFT, padx=2, pady=2)
             self.B2TT = CreateToolTip(self.B2, tool_tip)
         if b3 is not None:
-            self.B3 = Radiobutton(self.subframe, text=b3, anchor='w',
+            self.B3 = Tk.Radiobutton(self.subframe, text=b3, anchor='w',
                 command=self.updated, variable=self.value, value=3)
-            self.B3.pack(side=LEFT, padx=2, pady=2)
+            self.B3.pack(side=Tk.LEFT, padx=2, pady=2)
             self.B3TT = CreateToolTip(self.B3, tool_tip)
         if b4 is not None:
-            self.B4 = Radiobutton(self.subframe, text=b4, anchor='w',
+            self.B4 = Tk.Radiobutton(self.subframe, text=b4, anchor='w',
                 command=self.updated, variable=self.value, value=4)
-            self.B4.pack(side=LEFT, padx=2, pady=2)
+            self.B4.pack(side=Tk.LEFT, padx=2, pady=2)
             self.B4TT = CreateToolTip(self.B4, tool_tip)
         if b5 is not None:
-            self.B5 = Radiobutton(self.subframe, text=b5, anchor='w', 
+            self.B5 = Tk.Radiobutton(self.subframe, text=b5, anchor='w', 
                 command=self.updated, variable=self.value, value=5)
-            self.B5.pack(side=LEFT, padx=2, pady=2)
+            self.B5.pack(side=Tk.LEFT, padx=2, pady=2)
             self.B5TT = CreateToolTip(self.B5, tool_tip)
             
     def updated(self):
         self.frame.focus()
         if self.callback is not None: self.callback()
 
     def set_value(self, value:int):
@@ -819,28 +855,28 @@
 class window_controls():
     def __init__(self, parent_window, parent_object, load_callback, save_callback):
         # Create the class instance variables
         self.window = parent_window
         self.save_callback = save_callback
         self.load_callback = load_callback
         self.parent_object = parent_object
-        self.frame = Frame(self.window)
+        self.frame = Tk.Frame(self.window)
         self.frame.pack(padx=2, pady=2)
         # Create the buttons and tooltips
-        self.B1 = Button (self.frame, text = "Ok",command=self.ok)
-        self.B1.pack(side=LEFT, padx=2, pady=2)
+        self.B1 = Tk.Button (self.frame, text = "Ok",command=self.ok)
+        self.B1.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT1 = CreateToolTip(self.B1, "Apply selections and close window")
-        self.B2 = Button (self.frame, text = "Apply",command=self.apply)
-        self.B2.pack(side=LEFT, padx=2, pady=2)
+        self.B2 = Tk.Button (self.frame, text = "Apply",command=self.apply)
+        self.B2.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT2 = CreateToolTip(self.B2, "Apply selections")
-        self.B3 = Button (self.frame, text = "Reset",command=self.reset)
-        self.B3.pack(side=LEFT, padx=2, pady=2)
+        self.B3 = Tk.Button (self.frame, text = "Reset",command=self.reset)
+        self.B3.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT3 = CreateToolTip(self.B3, "Abandon edit and reload original configuration")
-        self.B4 = Button (self.frame, text = "Cancel",command=self.cancel)
-        self.B4.pack(side=LEFT, padx=2, pady=2)
+        self.B4 = Tk.Button (self.frame, text = "Cancel",command=self.cancel)
+        self.B4.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT4 = CreateToolTip(self.B4, "Abandon edit and close window")
         
     def apply(self):
         self.window.focus()
         self.save_callback(self.parent_object,False)
         
     def ok(self):
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/configure_point.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/configure_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 #
 # Inherits the following common editor base classes (from common):
 #    common.int_item_id_entry_box
 #    common.check_box
 #    common.dcc_entry_box
 #    common.object_id_selection
 #    common.selection_buttons
+#    common.signal_route_interlocking_frame
 #    common.signal_route_selections
 #    common.window_controls
 #
 #------------------------------------------------------------------------------------
 
 import copy
 
-from tkinter import *
+import tkinter as Tk
 from tkinter import ttk
 
 from . import common
 from . import objects
 
 #------------------------------------------------------------------------------------
 # Function to set the read-only "switched with" parameter. This is the back-reference
@@ -142,29 +143,29 @@
 class also_switch_selection(common.int_item_id_entry_box):
     def __init__(self, parent_frame, parent_object):
         # These are the functions used to validate that the entered signal ID
         # exists on the schematic and is different to the current signal ID
         exists_function = objects.point_exists
         current_id_function = parent_object.pointid.get_value
         # Create the Label Frame for the "also switch" entry box
-        self.frame = LabelFrame(parent_frame, text="Automatic switching")
+        self.frame = Tk.LabelFrame(parent_frame, text="Automatic switching")
         # Call the common base class init function to create the EB
-        self.label1 = Label(self.frame,text="Switch point:")
-        self.label1.pack(side=LEFT, padx=2, pady=2)
+        self.label1 = Tk.Label(self.frame,text="Switch point:")
+        self.label1.pack(side=Tk.LEFT, padx=2, pady=2)
         super().__init__(self.frame, tool_tip = "Enter the ID of another (fully "+
                 "automatic) point to be switched with this point (or leave blank)",
                 exists_function=exists_function, current_id_function=current_id_function)
-        self.pack(side=LEFT, padx=2, pady=2)
+        self.pack(side=Tk.LEFT, padx=2, pady=2)
         # This is the read-only element for the point this point is switched with
-        self.switched_with = StringVar(parent_frame, "")
-        self.label2 = Label(self.frame,text="Switched with:")
-        self.label2.pack(side=LEFT, padx=2, pady=2)
-        self.switched_eb = Entry(self.frame, width=3, textvariable=self.switched_with,
+        self.switched_with = Tk.StringVar(parent_frame, "")
+        self.label2 = Tk.Label(self.frame,text="Switched with:")
+        self.label2.pack(side=Tk.LEFT, padx=2, pady=2)
+        self.switched_eb = Tk.Entry(self.frame, width=3, textvariable=self.switched_with,
                                             justify='center',state="disabled")
-        self.switched_eb.pack(side=LEFT, padx=2, pady=2)
+        self.switched_eb.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT1 = common.CreateToolTip(self.switched_eb, "ID of the point that "+
                                        "will automatically switch this point")
     def validate(self):
         # Do the basic item validation first (exists and not current item ID)
         valid = super().validate(update_validation_status=False)
         if valid and self.entry.get() != "":
             autoswitch = int(self.entry.get())
@@ -201,34 +202,34 @@
 
 class general_settings():
     def __init__(self, parent_frame, parent_object):
         # We need the reference to the parent object so we can call the sibling
         # class method to get the current value of the Point ID for validation
         self.parent_object = parent_object
         # Create a Label frame to hold the general settings
-        self.frame = LabelFrame(parent_frame,text="General configuration")
+        self.frame = Tk.LabelFrame(parent_frame,text="General configuration")
         # Create a subframe to hold the first 2 buttons
-        self.subframe1 = Frame(self.frame)
+        self.subframe1 = Tk.Frame(self.frame)
         self.subframe1.pack()
         self.CB1 = common.check_box(self.subframe1, label="Rotated",width=9,
                         tool_tip="Select to rotate point by 180 degrees")
-        self.CB1.pack(side=LEFT, padx=2, pady=2)
+        self.CB1.pack(side=Tk.LEFT, padx=2, pady=2)
         self.CB2 = common.check_box(self.subframe1, label="Facing point lock", width=16,
                 tool_tip="Select to include a Facing Point Lock (manually switched points only)")
-        self.CB2.pack(side=LEFT, padx=2, pady=2)
+        self.CB2.pack(side=Tk.LEFT, padx=2, pady=2)
         # Create a subframe to hold the second 2 buttons
-        self.subframe2 = Frame(self.frame)
+        self.subframe2 = Tk.Frame(self.frame)
         self.subframe2.pack()
         self.CB3 = common.check_box(self.subframe2, label="Reversed", width=9,
                         tool_tip="Select to reverse the switching logic of the point blades")
-        self.CB3.pack(side=LEFT, padx=2, pady=2)
+        self.CB3.pack(side=Tk.LEFT, padx=2, pady=2)
         self.CB4 = common.check_box(self.subframe2, label="Fully automatic", width=16,
             tool_tip="Select to create the point without manual controls (to be switched "+
                         "with another point)", callback= self.automatic_updated)
-        self.CB4.pack(side=LEFT, padx=2, pady=2)
+        self.CB4.pack(side=Tk.LEFT, padx=2, pady=2)
 
     def automatic_updated(self):
         self.validate()
         # Enable/disable the FPL checkbox based on the 'fully automatic' state
         if self.CB4.get_value(): self.CB2.disable()
         else: self.CB2.enable()
     
@@ -268,28 +269,28 @@
 #    "set_values" - will set the entry/checkbox states [address:int, reversed:bool]
 #    "get_values" - will return the entry/checkbox states (address:int, reversed:bool]
 #------------------------------------------------------------------------------------
 
 class dcc_address_settings(common.dcc_entry_box):
     def __init__(self, parent_frame):
         # Create a Label frame to hold the DCC Address settings
-        self.frame = LabelFrame(parent_frame,text="DCC Address and command logic")
+        self.frame = Tk.LabelFrame(parent_frame,text="DCC Address and command logic")
         # Create the Tkinter Boolean vars to hold the DCC reversed selection
-        self.dccreversed = BooleanVar(self.frame,False)
+        self.dccreversed = Tk.BooleanVar(self.frame,False)
         # Create a DCC Address element and checkbox for the "reversed" selection
         # Call the common base class init function to create the EB. These are
         # created in a seperate subframe so they are centered
-        self.subframe = Frame(self.frame)
+        self.subframe = Tk.Frame(self.frame)
         self.subframe.pack()
         self.EB = common.dcc_entry_box(self.subframe, callback=self.entry_updated)
-        self.EB.pack(side=LEFT, padx=2, pady=2)
+        self.EB.pack(side=Tk.LEFT, padx=2, pady=2)
         # Create the checkbox for the DCC reversed selection
         self.CB = common.check_box(self.subframe, label="Reversed",
                     tool_tip="Select to reverse the DCC command logic")
-        self.CB.pack(side=LEFT, padx=2, pady=2)
+        self.CB.pack(side=Tk.LEFT, padx=2, pady=2)
         
     def entry_updated(self):
         if self.EB.entry.get()=="": self.CB.disable()
         else: self.CB.enable()
         
     def validate(self):
         return(self.EB.validate())
@@ -305,20 +306,20 @@
 #------------------------------------------------------------------------------------
 # Top level Class for the Point Configuration Tab
 #------------------------------------------------------------------------------------
 
 class point_configuration_tab():
     def __init__(self, parent_tab):
         # Create a Frame to hold the Point ID and Point Type Selections
-        self.frame = Frame(parent_tab)
+        self.frame = Tk.Frame(parent_tab)
         self.frame.pack(padx=2, pady=2, fill='x')
         # Create the UI Element for Point ID selection
         self.pointid = common.object_id_selection(self.frame, "Point ID",
                                 exists_function = objects.point_exists) 
-        self.pointid.frame.pack(side=LEFT, padx=2, pady=2, fill='y')
+        self.pointid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='y')
         # Create the UI Element for Point Type selection
         self.pointtype = common.selection_buttons(self.frame, "Point type",
                                       "Select Point Type", None, "RH", "LH")
         self.pointtype.frame.pack(padx=2, pady=2, fill='x')
         # Create the UI element for the general settings
         # Note that the class needs the parent object (to reference siblings)
         self.settings = general_settings(parent_tab, self)
@@ -327,90 +328,50 @@
         # Note that the class needs the parent object (to reference siblings)
         self.alsoswitch = also_switch_selection(parent_tab, self)
         self.alsoswitch.frame.pack(padx=2, pady=2, fill='x')
         # Create the UI element for the DCC Settings 
         self.dccsettings = dcc_address_settings(parent_tab)
         self.dccsettings.frame.pack(padx=2, pady=2, fill='x')
 
-#####################################################################################
-# Classes for the Point "Interlocking" Tab
-#####################################################################################
-
-#------------------------------------------------------------------------------------
-# Class for a signal route interlocking frame - uses multiple instances of the
-# signal_route_selection_element which are created when "set_values" is called
-# Public class instance methods provided by this class are:
-#    "set_values" - Populates the list of interlocked signals and their routes 
-#------------------------------------------------------------------------------------
-
-class signal_route_interlocking_frame():
-    def __init__(self, parent_frame):
-        # Create the Label Frame for the Signal Interlocking List 
-        self.frame = LabelFrame(parent_frame, text="Interlocking with signals")
-        self.frame.pack(padx=2, pady=2, fill='x')
-        # These are the lists that hold the references to the subframes and subclasses
-        self.sigelements = []
-        self.subframe = None
-
-    def set_values(self, sig_interlocking_frame:[[int,[bool,bool,bool,bool,bool]],]):
-        # If the lists are not empty (case of "reloading" the config) then destroy
-        # all the UI elements and create them again (the list may have changed)
-        if self.subframe: self.subframe.destroy()
-        self.subframe = Frame(self.frame)
-        self.subframe.pack()
-        self.sigelements = []
-        # sig_interlocking_frame is a variable length list where each element is [sig_id, interlocked_routes]
-        if sig_interlocking_frame:
-            for sig_interlocking_routes in sig_interlocking_frame:
-                # sig_interlocking_routes comprises [sig_id, [main, lh1, lh2, rh1, rh2]]
-                # Where each route element is a boolean value (True or False)            
-                self.sigelements.append(common.signal_route_selections(self.subframe,read_only=True,
-                        tool_tip="Edit the appropriate signals\nto configure interlocking"))
-                self.sigelements[-1].frame.pack()
-                self.sigelements[-1].set_values (sig_interlocking_routes)
-        else:
-            self.label = Label(self.subframe, text="No interlocked signals")
-            self.label.pack()
-
 #------------------------------------------------------------------------------------
 # Top level Class for the Point Interlocking Tab
 #------------------------------------------------------------------------------------
 
 class point_interlocking_tab():
     def __init__(self, parent_tab):
-        self.signals = signal_route_interlocking_frame(parent_tab)
+        self.signals = common.signal_route_interlocking_frame(parent_tab)
 
 #####################################################################################
 # Top level Class for the Edit Point window
 #####################################################################################
 
 class edit_point():
     def __init__(self, root, object_id):
         # This is the UUID for the object being edited
         self.object_id = object_id
         # Creatre the basic Top Level window
-        self.window = Toplevel(root)
+        self.window = Tk.Toplevel(root)
         self.window.attributes('-topmost',True)
         # Create the Notebook (for the tabs) 
         self.tabs = ttk.Notebook(self.window)
         # When you change tabs tkinter focuses on the first entry box - we don't want this
         # So we bind the tab changed event to a function which will focus on something else 
         self.tabs.bind ('<<NotebookTabChanged>>', self.tab_changed)
         # Create the Window tabs
-        self.tab1 = Frame(self.tabs)
+        self.tab1 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab1, text="Configration")
-        self.tab2 = Frame(self.tabs)
+        self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Interlocking")
         self.tabs.pack()
         self.config = point_configuration_tab(self.tab1)
         self.locking = point_interlocking_tab(self.tab2)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
         self.controls = common.window_controls(self.window, self, load_state, save_state)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
-        self.validation_error = Label(self.window, text="Errors on Form need correcting", fg="red")
+        self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
 
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
         # THIS IS STILL NOT WORKING AS IT LEAVES THE ENTRY BOX HIGHLIGHTED
         # self.window.focus()
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/configure_section.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/configure_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #    common.signal_route_selections
 #    common.window_controls
 #
 #------------------------------------------------------------------------------------
 
 import copy
 
-from tkinter import *
+import tkinter as Tk
 from tkinter import ttk
 
 from . import common
 from . import objects
 
 #------------------------------------------------------------------------------------
 # Function to return the read-only "mirrored by" parameter. This is the back-reference
@@ -185,34 +185,34 @@
         ### to via the MQTT networking - we'll therefore have to use the internal      ###
         ### library function or validate also against a list of subscribed sections    ###
         ### Note that the validation function will also need to change                 ###
         ##################################################################################
         exists_function = objects.section_exists
         current_id_function = parent_object.sectionid.get_value
         # Create the Label Frame for the "mirrored section" entry box
-        self.frame = LabelFrame(parent_frame, text="Link to other track section")
+        self.frame = Tk.LabelFrame(parent_frame, text="Link to other track section")
         # Create a frame for the "Section to mirror" elements
-        self.subframe1 = Frame(self.frame)
+        self.subframe1 = Tk.Frame(self.frame)
         self.subframe1.pack()
         # Call the common base class init function to create the EB
-        self.label1 = Label(self.subframe1,text="Section to mirror:")
-        self.label1.pack(side=LEFT, padx=2, pady=2)
+        self.label1 = Tk.Label(self.subframe1,text="Section to mirror:")
+        self.label1.pack(side=Tk.LEFT, padx=2, pady=2)
         super().__init__(self.subframe1, tool_tip = "Enter the ID of the track section to mirror - This can "+
                     "be a local section or a remote section (subscribed to via MQTT networking)",
                     exists_function=exists_function, current_id_function=current_id_function)
-        self.pack(side=LEFT, padx=2, pady=2)
+        self.pack(side=Tk.LEFT, padx=2, pady=2)
         # Create a frame for the "Mirrored by" elements
-        self.subframe2 = Frame(self.frame)
+        self.subframe2 = Tk.Frame(self.frame)
         self.subframe2.pack()
-        self.mirrored_by = StringVar(parent_frame, "")
-        self.label2 = Label(self.subframe2,text="Mirrored by section:")
-        self.label2.pack(side=LEFT, padx=2, pady=2)
-        self.mirrored_by_eb = Entry(self.subframe2, width=3, textvariable=self.mirrored_by,
+        self.mirrored_by = Tk.StringVar(parent_frame, "")
+        self.label2 = Tk.Label(self.subframe2,text="Mirrored by section:")
+        self.label2.pack(side=Tk.LEFT, padx=2, pady=2)
+        self.mirrored_by_eb = Tk.Entry(self.subframe2, width=3, textvariable=self.mirrored_by,
                                             justify='center',state="disabled")
-        self.mirrored_by_eb.pack(side=LEFT, padx=2, pady=2)
+        self.mirrored_by_eb.pack(side=Tk.LEFT, padx=2, pady=2)
         self.TT1 = common.CreateToolTip(self.mirrored_by_eb, "ID of the track "+
                             "section that that will be mirrored by this section")
 
     def validate(self):
         # Do the basic item validation first (exists and not current item ID)
         valid = super().validate(update_validation_status=False)
         if valid and self.entry.get() != "":
@@ -243,15 +243,15 @@
 # Overriden class methods are
 #    "validate" - Validates the length of the entered text (between 2-10 chars)
 #------------------------------------------------------------------------------------
 
 class default_label_entry(common.entry_box):
     def __init__(self, parent_frame):
         # Create the Label Frame for the "mirrored section" entry box
-        self.frame = LabelFrame(parent_frame, text="Default section label")
+        self.frame = Tk.LabelFrame(parent_frame, text="Default section label")
         super().__init__(self.frame, width=16, tool_tip = "Enter the default label to "+
                          "display when the section is occupied (this defines the default "+
                          "width of the Track Section object on the schematic). The default "+
                          "label should be between 4 and 10 characters")
         self.pack(padx=2, pady=2)
 
     def validate(self):
@@ -269,22 +269,22 @@
 #------------------------------------------------------------------------------------
 # Class for the main Track Section configuration tab
 #------------------------------------------------------------------------------------
 
 class section_configuration_tab():
     def __init__(self, parent_tab):
         # Create a Frame to hold the Section ID and General Settings
-        self.frame1 = Frame(parent_tab)
+        self.frame1 = Tk.Frame(parent_tab)
         self.frame1.pack(padx=2, pady=2, fill='x')
         # Create the UI Element for Section ID selection
         self.sectionid = common.object_id_selection(self.frame1, "Section ID",
                                 exists_function = objects.section_exists) 
-        self.sectionid.frame.pack(side=LEFT, padx=2, pady=2, fill='y')
+        self.sectionid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='y')
         # Create a labelframe for the General settings
-        self.subframe1 = LabelFrame(self.frame1, text="General Settings")
+        self.subframe1 = Tk.LabelFrame(self.frame1, text="General Settings")
         self.subframe1.pack(padx=2, pady=2, fill='x')
         self.readonly = common.check_box(self.subframe1, label="Read only",
                      tool_tip= "Select to make the Track Section non-editable")
         self.readonly.pack(padx=2, pady=2)
         # Create a Label Frame to hold the "Mirror" section. Note that this needs a
         # reference to the parent object to access the current value of Section ID
         self.mirror = mirrored_section(parent_tab, self)
@@ -302,38 +302,38 @@
 # Public class instance methods provided by this class are:
 #    "set_values" - Populates the list of signals and their routes
 #------------------------------------------------------------------------------------
 
 class signal_route_frame():
     def __init__(self, parent_frame, label:str):
         # Create the Label Frame for the Signal Interlocking List 
-        self.frame = LabelFrame(parent_frame, text=label)
+        self.frame = Tk.LabelFrame(parent_frame, text=label)
         self.frame.pack(padx=2, pady=2, fill='x')
         # These are the lists that hold the references to the subframes and subclasses
         self.sigelements = []
         self.subframe = None
 
     def set_values(self, sig_interlocking_frame:[[int,[bool,bool,bool,bool,bool]],]):
         # If the lists are not empty (case of "reloading" the config) then destroy
         # all the UI elements and create them again (the list may have changed)
         if self.subframe: self.subframe.destroy()
-        self.subframe = Frame(self.frame)
+        self.subframe = Tk.Frame(self.frame)
         self.subframe.pack()
         self.sigelements = []
         # sig_interlocking_frame is a variable length list where each element is [sig_id, interlocked_routes]
         if sig_interlocking_frame:
             for sig_interlocking_routes in sig_interlocking_frame:
                 # sig_interlocking_routes comprises [sig_id, [main, lh1, lh2, rh1, rh2]]
                 # Where each route element is a boolean value (True or False)            
                 self.sigelements.append(common.signal_route_selections(self.subframe, read_only=True,
                                     tool_tip="Edit the appropriate signals\nto configure automation"))
                 self.sigelements[-1].frame.pack()
                 self.sigelements[-1].set_values (sig_interlocking_routes)
         else:
-            self.label = Label(self.subframe, text="No automation configured")
+            self.label = Tk.Label(self.subframe, text="No automation configured")
             self.label.pack()
             
 #------------------------------------------------------------------------------------
 # Class for the main Track Section configuration tab
 #------------------------------------------------------------------------------------
 
 class section_automation_tab():
@@ -346,33 +346,33 @@
 #####################################################################################
 
 class edit_section():
     def __init__(self, root, object_id):
         # This is the UUID for the object being edited
         self.object_id = object_id
         # Creatre the basic Top Level window
-        self.window = Toplevel(root)
+        self.window = Tk.Toplevel(root)
         self.window.attributes('-topmost',True)
         # Create the Notebook (for the tabs) 
         self.tabs = ttk.Notebook(self.window)
         # When you change tabs tkinter focuses on the first entry box - we don't want this
         # So we bind the tab changed event to a function which will focus on something else 
         self.tabs.bind ('<<NotebookTabChanged>>', self.tab_changed)
         # Create the Window tabs
-        self.tab1 = Frame(self.tabs)
+        self.tab1 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab1, text="Configration")
-        self.tab2 = Frame(self.tabs)
+        self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Automation")
         self.tabs.pack(fill='x')
         self.config = section_configuration_tab(self.tab1)
         self.automation = section_automation_tab(self.tab2)        
         # Create the common Apply/OK/Reset/Cancel buttons for the window
         self.controls = common.window_controls(self.window, self, load_state, save_state)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
-        self.validation_error = Label(self.window, text="Errors on Form need correcting", fg="red")
+        self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
 
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
         # THIS IS STILL NOT WORKING AS IT LEAVES THE ENTRY BOX HIGHLIGHTED
         # self.window.focus()
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    configure_signal_tab2 - Point and signal interlocking
 #    configure_signal_tab3 - signal automation
 #    common.window_controls - the common load/save/cancel/OK controls
 #------------------------------------------------------------------------------------
 
 import copy
 
-from tkinter import *
+import tkinter as Tk
 from tkinter import ttk
 
 from . import common
 from . import objects
 from . import configure_signal_tab1 
 from . import configure_signal_tab2
 from . import configure_signal_tab3
@@ -359,30 +359,30 @@
 def update_tab1_signal_subtype_selections(signal):
     if signal.config.sigtype.get_value() == signals_common.sig_type.colour_light.value:
         signal.config.subtype.B1.configure(text="2 Asp G/R")
         signal.config.subtype.B2.configure(text="2 Asp G/Y")
         signal.config.subtype.B3.configure(text="2 Asp Y/R")
         signal.config.subtype.B4.configure(text="3 Aspect")
         signal.config.subtype.B5.configure(text="4 Aspect")
-        signal.config.subtype.B3.pack(side=LEFT)
-        signal.config.subtype.B4.pack(side=LEFT)
-        signal.config.subtype.B5.pack(side=LEFT)
+        signal.config.subtype.B3.pack(side=Tk.LEFT)
+        signal.config.subtype.B4.pack(side=Tk.LEFT)
+        signal.config.subtype.B5.pack(side=Tk.LEFT)
     elif signal.config.sigtype.get_value() == signals_common.sig_type.semaphore.value:
         signal.config.subtype.B1.configure(text="Home")
         signal.config.subtype.B2.configure(text="Distant")
         signal.config.subtype.B3.pack_forget()
         signal.config.subtype.B4.pack_forget()
         signal.config.subtype.B5.pack_forget()
     elif signal.config.sigtype.get_value() == signals_common.sig_type.ground_position.value:
         signal.config.subtype.B1.configure(text="Norm (post'96)")
         signal.config.subtype.B2.configure(text="Shunt (post'96)")
         signal.config.subtype.B3.configure(text="Norm (early)")
         signal.config.subtype.B4.configure(text="Shunt (early)")
-        signal.config.subtype.B3.pack(side=LEFT)
-        signal.config.subtype.B4.pack(side=LEFT)
+        signal.config.subtype.B3.pack(side=Tk.LEFT)
+        signal.config.subtype.B4.pack(side=Tk.LEFT)
         signal.config.subtype.B5.pack_forget()
     elif signal.config.sigtype.get_value() == signals_common.sig_type.ground_disc.value:
         signal.config.subtype.B1.configure(text="Normal")
         signal.config.subtype.B2.configure(text="Shunt Ahead")
         signal.config.subtype.B3.pack_forget()
         signal.config.subtype.B4.pack_forget()
         signal.config.subtype.B5.pack_forget()
@@ -854,43 +854,43 @@
 
 class edit_signal:
     def __init__(self, root, object_id):
         self.root=root
         # This is the UUID for the object being edited
         self.object_id = object_id
         # Creatre the basic Top Level window
-        self.window = Toplevel(root)
+        self.window = Tk.Toplevel(root)
         self.window.attributes('-topmost',True)
         # Create the Notebook (for the tabs) 
         self.tabs = ttk.Notebook(self.window)
         # When you change tabs tkinter focuses on the first entry box - we don't want this
         # So we bind the tab changed event to a function which will focus on something else 
         self.tabs.bind ('<<NotebookTabChanged>>', self.tab_changed)
         # Create the Window tabs
-        self.tab1 = Frame(self.tabs)
+        self.tab1 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab1, text="Configration")
-        self.tab2 = Frame(self.tabs)
+        self.tab2 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab2, text="Interlocking")
         self.tabs.pack()
-        self.tab3 = Frame(self.tabs)
+        self.tab3 = Tk.Frame(self.tabs)
         self.tabs.add(self.tab3, text="Automation")
         self.tabs.pack()
         # The config tab needs references to all the 'config changed' callback functions
         self.config = configure_signal_tab1.signal_configuration_tab(self.tab1,
                 self.sig_type_updated, self.sub_type_updated, self.route_type_updated,
                 self.route_selections_updated, self.sig_routes_updated,
                 self.sub_routes_updated, self.dist_routes_updated)
         # The interlocking tab needs the parent object so the sig_id can be accessed for validation
         self.locking = configure_signal_tab2.signal_interlocking_tab(self.tab2, self)
         # The automation tab needs the parent object so the sig_id can be accessed for validation
         self.automation = configure_signal_tab3.signal_automation_tab(self.tab3, self)
         # Create the common Apply/OK/Reset/Cancel buttons for the window
         self.controls = common.window_controls(self.window, self, load_state, save_state)
         # Create the Validation error message (this gets packed/unpacked on apply/save)
-        self.validation_error = Label(self.window, text="Errors on Form need correcting", fg="red")
+        self.validation_error = Tk.Label(self.window, text="Errors on Form need correcting", fg="red")
         # load the initial UI state
         load_state(self)
         
     def tab_changed(self,event):
         # Focus on the top level window to remove focus from the first entry box
         # THIS IS STILL NOT WORKING AS IT LEAVES THE ENTRY BOX HIGHLIGHTED
         # self.window.focus()
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal_tab1.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #------------------------------------------------------------------------------------
 # Functions and sub Classes for the Edit Signal "Configuration" Tab 
 #------------------------------------------------------------------------------------
 
-from tkinter import *
+import tkinter as Tk
 
 from . import common
 from . import objects
 
 #------------------------------------------------------------------------------------
 # Class for the General Settings UI Element - Builds on the common checkbox class
 # Public class instance methods inherited from the base check box class are:
@@ -14,15 +14,15 @@
 #    "get_value" - get the last "validated" value of the Rotate checkbutton (int) 
 #------------------------------------------------------------------------------------
 
 class general_settings(common.check_box):
     def __init__(self, parent_frame):
         # Create a Label frame to hold the general settings UI element
         # Packed onto the parent frame by the creating function/class
-        self.frame = LabelFrame(parent_frame,text="General Config")
+        self.frame = Tk.LabelFrame(parent_frame,text="General Config")
         # Create the "rotate" checkbutton and tool Tip
         super().__init__(self.frame, label="Rotated",
                     tool_tip = "Select to rotate signal by 180 degrees")
         self.pack()
 
 #------------------------------------------------------------------------------------
 # Class for a semaphore route arm element (comprising checkbox and DCC address Box)
@@ -35,22 +35,22 @@
 #------------------------------------------------------------------------------------
 
 class semaphore_route_element():
     def __init__(self, parent_frame, label:str, tool_tip:str, callback=None):
         # Callback for select/deselect of the checkbox
         self.callback = callback
         # Create a frame for the UI element (always packed into the parent frame)
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the checkbox and DCC entry Box (default tool tip for DCC Entry Box)
         self.CB = common.check_box(parent_frame, label=label,
                         tool_tip=tool_tip, callback=self.cb_updated)
-        self.CB.pack(side=LEFT)
+        self.CB.pack(side=Tk.LEFT)
         self.EB = common.dcc_entry_box(parent_frame)
-        self.EB.pack(side=LEFT)
+        self.EB.pack(side=Tk.LEFT)
                 
     def cb_updated(self):
         self.update_eb_state()
         if self.callback is not None: self.callback()
         
     def update_eb_state(self):
         if self.CB.get_value(): self.EB.enable()
@@ -111,19 +111,19 @@
     def __init__(self, parent_frame, label:str,sig_arms_updated_callback=None,
                  sub_arms_updated_callback=None, dist_arms_updated_callback=None):
         # Callback for change in signal arm selections
         self.sig_arms_callback = sig_arms_updated_callback
         self.sub_arms_callback = sub_arms_updated_callback
         self.dist_arms_callback = dist_arms_updated_callback
         # Create a frame for the UI element (always packed into the parent frame)
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the lable and route elements (these are packed by the class instances)
-        self.label = Label(self.frame, anchor='w', width=5, text=label)
-        self.label.pack(side=LEFT)
+        self.label = Tk.Label(self.frame, anchor='w', width=5, text=label)
+        self.label.pack(side=Tk.LEFT)
         self.sig = semaphore_route_element(self.frame, label="Main (home) arm ",
                       tool_tip= "Select to add a home signal arm for this route",
                       callback=self.sig_arms_updated)
         self.sub = semaphore_route_element(self.frame, label="Subsidary arm ",
                     tool_tip="Select to add a subsidary signal arm for this route",
                     callback=self.sub_arms_updated)
         self.dist = semaphore_route_element(self.frame, label="Distant arm ",
@@ -208,15 +208,15 @@
 #    "get_arms" - returns the last "valid" values (enabled/disabled, addresses)
 # The callbacks are made when the signal arms are selected or deselected
 #------------------------------------------------------------------------------------
 
 class semaphore_signal_arms():
     def __init__(self, parent_frame, sig_arms_updated, subs_arms_updated, dist_arms_updated):
         # Create a frame for this UI element (packed by the creating function/class)
-        self.frame = LabelFrame(parent_frame, text="Semaphore Signal Arms and DCC Addresses")
+        self.frame = Tk.LabelFrame(parent_frame, text="Semaphore Signal Arms and DCC Addresses")
         # Create the route group for each route (packed into the frame by the class instances)
         self.main = semaphore_route_group(self.frame, label="Main",
                                 sig_arms_updated_callback=sig_arms_updated,
                                 sub_arms_updated_callback=subs_arms_updated,
                                 dist_arms_updated_callback=dist_arms_updated)
         self.lh1 = semaphore_route_group(self.frame, label="LH1",
                                 sig_arms_updated_callback=sig_arms_updated,
@@ -325,25 +325,25 @@
 #    "get_addresses" - will return a list of the last "valid" entries
 #------------------------------------------------------------------------------------
 
 class dcc_entry_boxes:
     def __init__(self, parent_frame):
         # Create the DCC command entry elements (packed directly into parent frame)
         self.dcc1 = common.dcc_command_entry(parent_frame)
-        self.dcc1.frame.pack(side=LEFT)
+        self.dcc1.frame.pack(side=Tk.LEFT)
         self.dcc2 = common.dcc_command_entry(parent_frame)
-        self.dcc2.frame.pack(side=LEFT)
+        self.dcc2.frame.pack(side=Tk.LEFT)
         self.dcc3 = common.dcc_command_entry(parent_frame)
-        self.dcc3.frame.pack(side=LEFT)
+        self.dcc3.frame.pack(side=Tk.LEFT)
         self.dcc4 = common.dcc_command_entry(parent_frame)
-        self.dcc4.frame.pack(side=LEFT)
+        self.dcc4.frame.pack(side=Tk.LEFT)
         self.dcc5 = common.dcc_command_entry(parent_frame)
-        self.dcc5.frame.pack(side=LEFT)
+        self.dcc5.frame.pack(side=Tk.LEFT)
         self.dcc6 = common.dcc_command_entry(parent_frame)
-        self.dcc6.frame.pack(side=LEFT)
+        self.dcc6.frame.pack(side=Tk.LEFT)
         
     def validate_addresses(self):
         return ( self.dcc1.validate() and
                  self.dcc2.validate() and
                  self.dcc3.validate() and
                  self.dcc4.validate() and
                  self.dcc5.validate() and
@@ -395,19 +395,19 @@
 #    "set_addresses" - will set the values of the entry boxes (pass in a list)
 #    "get_addresses" - will return a list of the last "valid" entries
 #------------------------------------------------------------------------------------
 
 class colour_light_aspect(dcc_entry_boxes):
     def __init__(self, parent_frame, label:str):
         # Create a frame for this UI element (always packed)
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the label for the DCC command sequence
-        self.label = Label(self.frame, width=12, text=label, anchor='w')
-        self.label.pack(side=LEFT)
+        self.label = Tk.Label(self.frame, width=12, text=label, anchor='w')
+        self.label.pack(side=Tk.LEFT)
         # Call the init function of the class we are inheriting from
         # The DCC entry boxes get packed into the frame by the parent class
         super().__init__(self.frame)
 
 #------------------------------------------------------------------------------------
 # Classes to create the DCC entry UI element for colour light signal aspects
 # Class instance methods to use externally are:
@@ -424,31 +424,31 @@
 #------------------------------------------------------------------------------------
 
 class colour_light_aspects():
     def __init__(self, parent_frame, callback=None):
         # Callback for select/deselect of the subsidary signal
         self.callback = callback
         # Create a label frame (packed by the creating function/class)
-        self.frame = LabelFrame(parent_frame,
+        self.frame = Tk.LabelFrame(parent_frame,
                 text="DCC command sequences for Colour Light signal aspects")
         # Create the DCC Entry Elements (packed into the frame by the parent class)
         self.red = colour_light_aspect(self.frame, label="Danger")
         self.grn = colour_light_aspect(self.frame, label="Proceed")
         self.ylw = colour_light_aspect(self.frame, label="Caution")
         self.dylw = colour_light_aspect(self.frame, label="Prelim Caution")
         self.fylw = colour_light_aspect(self.frame, label="Flash Caution")
         self.fdylw = colour_light_aspect(self.frame, label="Flash Prelim")
         # Create a subframe to hold the subsidary signal entry box (always packed)
-        self.subframe = Frame(self.frame)
+        self.subframe = Tk.Frame(self.frame)
         self.subframe.pack()
         self.CB = common.check_box(self.subframe, label="Subsidary signal",   
                     tool_tip="Select to add a seperate calling on aspect",callback=self.sub_updated)
-        self.CB.pack(side=LEFT, padx=2, pady=2)
+        self.CB.pack(side=Tk.LEFT, padx=2, pady=2)
         self.EB = common.dcc_entry_box(self.subframe)
-        self.EB.pack(side=LEFT, padx=2, pady=2)
+        self.EB.pack(side=Tk.LEFT, padx=2, pady=2)
 
     def sub_updated(self):
         self.update_eb_state()
         if self.callback is not None: self.callback()
         
     def update_eb_state(self):
         if self.CB.get_value(): self.EB.enable()
@@ -560,28 +560,28 @@
 #    "get_theatre" - return the values (character & dcc commands) for the theatre
 #------------------------------------------------------------------------------------
 
 class theatre_route_element(dcc_entry_boxes):
     def __init__(self, parent_frame, label:str, width:int, callback=None,
                                 enable_addresses_on_selection:bool=False):
         # Create a frame for this UI element (always packed in the parent frame)
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Callback to make when the route selections change (Theatre Char EB changes)
         self.callback = callback
         # If the enable_addresses_on_selection flag is set to TRUE then the DCC address EBs
         # will be enabled/disabled when the Theatre character is changed. If false then the current
         # state of the EBs (enabled or disabled) remains unchanged. This is to support the MAIN
         # route which will always need a DCC address sequence even if there is no Theartre character
         self.enable_addresses_on_selection = enable_addresses_on_selection
         # Create the label and entry box for the theatre character
-        self.label = Label(self.frame, width=width, text=label, anchor='w')
-        self.label.pack(side=LEFT)
+        self.label = Tk.Label(self.frame, width=width, text=label, anchor='w')
+        self.label.pack(side=Tk.LEFT)
         self.EB = theatre_route_entry_box(self.frame, callback=self.selection_updated)
-        self.EB.pack(side=LEFT)
+        self.EB.pack(side=Tk.LEFT)
         # Call the init function of the class we are inheriting from
         # The DCC entry boxes get packed into the frame by the parent class
         super().__init__(self.frame)
         
     def selection_updated(self):
         self.update_addresses()
         if self.callback is not None: self.callback()
@@ -631,15 +631,15 @@
 # The Callback will be made on route selection change (theatre character EB change)
 #------------------------------------------------------------------------------------
 
 class theatre_route_indications:
     def __init__(self, parent_frame, callback=None):
         # Create a label frame for the route selections. We don't pack this element
         # as the frame gets packed/unpacked depending on UI selections
-        self.frame = LabelFrame(parent_frame, text="Theatre route indications "+
+        self.frame = Tk.LabelFrame(parent_frame, text="Theatre route indications "+
                                         "and associated DCC command sequences")
         # Create the individual route selection elements.
         # The MAIN route DCC address EBs remain enabled even if there is no theatre route
         # The MAIN element is therefore created with enable_addresses_on_selection=False
         self.dark = theatre_route_element(self.frame, label="(Dark)", width=5,
                     callback=callback, enable_addresses_on_selection=True)
         self.main = theatre_route_element(self.frame, label="MAIN", width=5,
@@ -750,29 +750,29 @@
 #    "get_feather" - return the state of the "Feather" checkbox
 #------------------------------------------------------------------------------------
 
 class feather_route_element(dcc_entry_boxes):
     def __init__(self, parent_frame, label:str, width:int, callback=None,
                           enable_addresses_on_selection=False):
         # Create a frame for this UI element (always packed in the parent frame)
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Callback to make when the route selections change (enabled/disabled)
         self.callback = callback
         # If the enable_addresses_on_selection flag is set to TRUE then the DCC address EBs
         # will be enabled/disabled when the route checkbox is changed. If false then the current
         # state of the EBs (enabled or disabled) remains unchanged. This is to support the MAIN
         # route which will always need a DCC address sequence even if there is no feather
         self.enable_addresses_on_selection = enable_addresses_on_selection
         # Create the label and checkbox for the feather route selection
-        self.label = Label(self.frame, width=width, text=label, anchor='w')
-        self.label.pack(side=LEFT)
+        self.label = Tk.Label(self.frame, width=width, text=label, anchor='w')
+        self.label.pack(side=Tk.LEFT)
         self.CB = common.check_box(self.frame, callback=self.selection_updated, label="",
                         tool_tip="Select to add a feather indication for this route")
-        self.CB.pack(side=LEFT)
+        self.CB.pack(side=Tk.LEFT)
         # Call the init function of the class we are inheriting from
         # The DCC entry boxes get packed into the frame by the parent class
         super().__init__(self.frame)
         
     def selection_updated(self):
         self.update_addresses()
         if self.callback is not None: self.callback()
@@ -816,15 +816,15 @@
 # The Callback will be made on route selection change (enabled/disabled)
 #------------------------------------------------------------------------------------
 
 class feather_route_indications:
     def __init__(self, parent_frame, callback):
         # Create a label frame for the route selections. We don't pack this element
         # as the frame gets packed/unpacked depending on UI selections
-        self.frame = LabelFrame(parent_frame, text="Feather Route Indications "+
+        self.frame = Tk.LabelFrame(parent_frame, text="Feather Route Indications "+
                                         "and associated DCC command sequences")
         # Create the individual route selection elements.
         # The MAIN route DCC address EBs remain enabled even if there is no route feather
         # The MAIN element is therefore created with enable_addresses_on_selection=False
         self.dark = feather_route_element(self.frame, label="(Dark)", width=5,
                             callback=callback, enable_addresses_on_selection=True)
         self.main = feather_route_element(self.frame, label="MAIN", width=5,
@@ -949,29 +949,29 @@
 # The Callback will be made on route selection change (enabled/disabled)
 #------------------------------------------------------------------------------------
 
 class route_selections():
     def __init__(self, parent_frame, label:str, tool_tip:str, callback=None, main_signal=False):
         self.main_signal = main_signal
         # Create a label frame for the selections (packed by the calling function/class
-        self.frame = LabelFrame(parent_frame, text=label)
+        self.frame = Tk.LabelFrame(parent_frame, text=label)
         # We use a subframe to center the selections boxes
-        self.subframe = Frame(self.frame)
+        self.subframe = Tk.Frame(self.frame)
         self.subframe.pack(padx=2, pady=2)
         # Create the required selection elements (always packed in the subframe)
         self.main = common.check_box(self.subframe, label="MAIN", tool_tip=tool_tip, callback=callback)
-        self.main.pack(side=LEFT)
+        self.main.pack(side=Tk.LEFT)
         self.lh1 = common.check_box(self.subframe, label="LH1", tool_tip=tool_tip, callback=callback)
-        self.lh1.pack(side=LEFT)
+        self.lh1.pack(side=Tk.LEFT)
         self.lh2 = common.check_box(self.subframe, label="LH2", tool_tip=tool_tip, callback=callback)
-        self.lh2.pack(side=LEFT)
+        self.lh2.pack(side=Tk.LEFT)
         self.rh1 = common.check_box(self.subframe, label="RH1", tool_tip=tool_tip, callback=callback)
-        self.rh1.pack(side=LEFT)
+        self.rh1.pack(side=Tk.LEFT)
         self.rh2 = common.check_box(self.subframe, label="RH2", tool_tip=tool_tip, callback=callback)        
-        self.rh2.pack(side=LEFT)
+        self.rh2.pack(side=Tk.LEFT)
         if self.main_signal: self.main.config(state="disabled")
 
     def enable_selection(self):
         if not self.main_signal: self.main.enable()
         self.lh1.enable()
         self.lh2.enable()
         self.rh1.enable()
@@ -1009,36 +1009,36 @@
 #------------------------------------------------------------------------------------
 
 class signal_configuration_tab:
     def __init__(self, parent_tab, sig_type_updated, sub_type_updated,
                 route_type_updated, route_selections_updated, sig_routes_updated,
                 sub_routes_updated, dist_routes_updated):
         # Create a Frame for the Sig ID and Signal Type Selections (always packed)
-        self.frame1 = Frame(parent_tab)
+        self.frame1 = Tk.Frame(parent_tab)
         self.frame1.pack(padx=2, pady=2, fill='x')
         self.sigid = common.object_id_selection(self.frame1,"Signal ID",
                                 exists_function = objects.signal_exists)
-        self.sigid.frame.pack(side=LEFT, padx=2, pady=2, fill='both')
+        self.sigid.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='both')
         self.sigtype = common.selection_buttons(self.frame1,"Signal Type",
                     "Select signal type",sig_type_updated,"Colour Light",
                         "Ground Pos","Semaphore","Ground Disc")
-        self.sigtype.frame.pack(side=LEFT, padx=2, pady=2, fill='x', expand=True)
+        self.sigtype.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='x', expand=True)
         # Create the UI Element for Signal subtype selection (always packed)
         self.subtype = common.selection_buttons(parent_tab,"Signal Subtype",
                     "Select signal subtype",sub_type_updated,"-","-","-","-","-")
         self.subtype.frame.pack(padx=2, pady=2, fill='x')
         # Create a Frame to hold the Gen settings and Route type Selections (always packed)
-        self.frame2 = Frame(parent_tab)
+        self.frame2 = Tk.Frame(parent_tab)
         self.frame2.pack(padx=2, pady=2, fill='x')
         self.settings = general_settings(self.frame2)
-        self.settings.frame.pack(side=LEFT, padx=2, pady=2, fill='both')
+        self.settings.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='both')
         self.routetype = common.selection_buttons(self.frame2, "Route Indications",
                     "Select the route indications for the main signal", route_type_updated,
                     "None", "Route feathers", "Theatre indicator", "Route arms")
-        self.routetype.frame.pack(side=LEFT, padx=2, pady=2, fill='x', expand=True)
+        self.routetype.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='x', expand=True)
         # Create the Checkboxes and DCC Entry Box frames for the type-specific selections
         # These frames are packed / hidden depending on the signal type and route 
         # indication type selections by the callback functions in "configure_signal.py"
         self.aspects = colour_light_aspects(parent_tab, sub_routes_updated)
         self.theatre = theatre_route_indications(parent_tab, route_selections_updated)
         self.feathers = feather_route_indications(parent_tab, route_selections_updated)
         self.semaphores = semaphore_signal_arms(parent_tab, sig_routes_updated,
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal_tab2.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #------------------------------------------------------------------------------------
 # Functions and sub Classes for the Edit Signal "Interlocking" Tab 
 #------------------------------------------------------------------------------------
 
-from tkinter import *
+import tkinter as Tk
 
 from . import common
 from . import objects
 
 #------------------------------------------------------------------------------------
 # Class for a point interlocking entry element (point_id + point_state)
 # Uses the common int_item_id_entry_box and state_box classes
@@ -20,18 +20,18 @@
 
 class point_interlocking_entry():
     def __init__(self, parent_frame, point_exists_function):
         # Create the point ID entry box and associated state box (packed in the parent frame)
         self.EB = common.int_item_id_entry_box(parent_frame, exists_function=point_exists_function,
                     tool_tip = "Specify the points that need to be set and locked before the "+
                         "signal can be cleared for the route", callback=self.eb_updated)
-        self.EB.pack(side=LEFT)
+        self.EB.pack(side=Tk.LEFT)
         self.CB = common.state_box(parent_frame, label_off=u"\u2192", label_on="\u2191", width=2,
                     tool_tip="Select the required state for the point (normal or switched)")
-        self.CB.pack(side=LEFT)
+        self.CB.pack(side=Tk.LEFT)
                             
     def eb_updated(self):
         if self.EB.entry.get() == "":
             self.CB.disable()
         else: self.CB.enable()
         
     def validate(self):
@@ -83,40 +83,40 @@
         #################################################################################
         instrument_exists_function = objects.instrument_exists
         signal_exists_function = objects.signal_exists
         current_id_function = parent_object.config.sigid.get_value
         instrument_exists_function = objects.instrument_exists
         point_exists_function = objects.point_exists
         # Create a frame for this UI element (always packed into the parent frame)
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the lable and the point interlocking entry elements (these are
         # packed LEFT in the frame by the parent class when created)
-        self.label = Label(self.frame, anchor='w', width=5, text=label)
-        self.label.pack(side = LEFT)
+        self.label = Tk.Label(self.frame, anchor='w', width=5, text=label)
+        self.label.pack(side = Tk.LEFT)
         self.p1 = point_interlocking_entry(self.frame, point_exists_function)
         self.p2 = point_interlocking_entry(self.frame, point_exists_function)
         self.p3 = point_interlocking_entry(self.frame, point_exists_function)
         self.p4 = point_interlocking_entry(self.frame, point_exists_function)
         self.p5 = point_interlocking_entry(self.frame, point_exists_function)
         self.p6 = point_interlocking_entry(self.frame, point_exists_function)
         # Create the signal ahead and instrument ahead elements (always packed)
-        self.label1 = Label(self.frame, text=" Sig:")
-        self.label1.pack(side=LEFT)
+        self.label1 = Tk.Label(self.frame, text=" Sig:")
+        self.label1.pack(side=Tk.LEFT)
         self.sig = common.str_item_id_entry_box(self.frame, exists_function=signal_exists_function,
                         tool_tip = "Enter the ID of the next signal along the specified route - This "+
                         "can be a local signal or a remote signal (subscribed to via MQTT networking)",
                           current_id_function = current_id_function)
-        self.sig.pack(side=LEFT)
-        self.label2 = Label(self.frame, text=" Blk:")
-        self.label2.pack(side=LEFT)
+        self.sig.pack(side=Tk.LEFT)
+        self.label2 = Tk.Label(self.frame, text=" Blk:")
+        self.label2.pack(side=Tk.LEFT)
         self.block = common.int_item_id_entry_box(self.frame, exists_function=instrument_exists_function,
                                 tool_tip="Enter the ID of the local block instrument controlling "+
                                     "access to the next block section along the specified route") 
-        self.block.pack(side=LEFT)
+        self.block.pack(side=Tk.LEFT)
     
     def validate(self):
         # Validates all point, signal and block instrument entries
         valid = (self.p1.validate() and self.p2.validate() and self.p3.validate() and
                  self.p4.validate() and self.p5.validate() and self.p6.validate() and
                  self.sig.validate() and self.block.validate())
         return(valid)
@@ -191,15 +191,15 @@
 #    "enable_block_ahead" - enables the block ahead selections (if the route is enabled)
 #    "disable_block_ahead" - disables the block ahead selections
 #------------------------------------------------------------------------------------
 
 class interlocking_route_frame:
     def __init__(self, parent_window, parent_object):
         # Create a Label Frame for the UI element (packed by the creating function/class)
-        self.frame = LabelFrame(parent_window, text= "Signal routes and point interlocking")
+        self.frame = Tk.LabelFrame(parent_window, text= "Signal routes and point interlocking")
         # Create the route elements (sign, sub, dist) - these are packed in class instancees
         self.main = interlocking_route_group(self.frame, parent_object, "Main")
         self.lh1 = interlocking_route_group(self.frame, parent_object, "LH1")
         self.lh2 = interlocking_route_group(self.frame, parent_object, "LH2")
         self.rh1 = interlocking_route_group(self.frame, parent_object, "RH1")
         self.rh2 = interlocking_route_group(self.frame, parent_object, "RH2")
 
@@ -272,15 +272,15 @@
 class conflicting_signals_element():
     def __init__(self, parent_frame, parent_object, label:str):
         # These are the functions used to validate that the entered signal ID
         # exists on the schematic and is different to the current signal ID
         exists_function = objects.signal_exists
         current_id_function = parent_object.config.sigid.get_value
         # Create the Label Frame for the UI element (packed/unpacked on enable/disable) 
-        self.frame = LabelFrame(parent_frame, text=label+" - interlocking with conflicting signals")
+        self.frame = Tk.LabelFrame(parent_frame, text=label+" - interlocking with conflicting signals")
         self.frame.pack(padx=2, pady=2, fill='x')
         self.frame.grid_columnconfigure(0, weight=1)
         self.frame.grid_columnconfigure(1, weight=1)
         tool_tip = "Specify any signals/routes that would conflict with this signal route"
         self.sig1 = common.signal_route_selections(self.frame, read_only=False, tool_tip = tool_tip,
                     exists_function=exists_function, current_id_function=current_id_function)
         self.sig1.frame.grid(row=0, column=0)
@@ -339,15 +339,15 @@
 #    "get_values" - Populates the list of interlocked signals and their routes 
 #    "validate" - Validates all Entry boxes (Signals exist and not current ID) 
 #------------------------------------------------------------------------------------
 
 class conflicting_signals_frame():
     def __init__(self, parent_frame, parent_object):
         # Create the Label Frame for the UI element (packed by the creating function/class)
-        self.frame = LabelFrame(parent_frame, text="Conflicting signals not locked by the above point selections")
+        self.frame = Tk.LabelFrame(parent_frame, text="Conflicting signals not locked by the above point selections")
         self.main = conflicting_signals_element(self.frame, parent_object, "MAIN Route")
         self.lh1 = conflicting_signals_element(self.frame, parent_object, "LH1 Route")
         self.lh2 = conflicting_signals_element(self.frame, parent_object, "LH2 Route")
         self.rh1 = conflicting_signals_element(self.frame, parent_object, "RH1 Route")
         self.rh2 = conflicting_signals_element(self.frame, parent_object, "RH2 Route")
         
     def validate(self):
@@ -383,15 +383,15 @@
 # Class for the Distant 'interlock with home signals ahead" ui element
 # Inherits from  common.check_box class (get_value/set_value/enable/disable)
 #------------------------------------------------------------------------------------
 
 class interlock_with_signals_ahead(common.check_box):
     def __init__(self, parent_frame):
         # Create the Label Frame for the UI element (packed by the creating function/class)
-        self.frame = LabelFrame(parent_frame, text="Distant signal interlocking")
+        self.frame = Tk.LabelFrame(parent_frame, text="Distant signal interlocking")
         super().__init__(self.frame, label="Interlock distant with all home signals ahead",
                         tool_tip="Select to lock the distant signal at CAUTION if any home signals "+
                         "on the route ahead are at DANGER (if the distant signal is CLEAR it "+
                         "will remain unlocked so it can be returned to CAUTION at any time)")
         self.pack()
 
 #------------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/configure_signal_tab3.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/configure_signal_tab3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #------------------------------------------------------------------------------------
 # Functions and sub Classes for the Edit Signal "Automation" Tab
 #------------------------------------------------------------------------------------
 
-from tkinter import *
+import tkinter as Tk
 
 from . import common
 from . import objects
 
 #------------------------------------------------------------------------------------
 # Class for a Track Sensor Entry Box - based on the common integer_entry_box class
 # Public Class instance methods (inherited from the integer_entry_box) are
@@ -17,19 +17,19 @@
 #------------------------------------------------------------------------------------
 
 class signal_sensor(common.integer_entry_box):
     def __init__(self, parent_frame, parent_object, callback, label:str, tool_tip:str):
         # We need the reference to the parent object so we can call the sibling
         # class method to get the current value of the Signal ID for validation
         self.parent_object = parent_object 
-        self.label = Label(parent_frame, text=label)
-        self.label.pack(side=LEFT, padx=2, pady=2)
+        self.label = Tk.Label(parent_frame, text=label)
+        self.label.pack(side=Tk.LEFT, padx=2, pady=2)
         super().__init__(parent_frame, width=3, min_value=4, max_value=26,
                 callback = callback, tool_tip=tool_tip, allow_empty=True)
-        self.pack(side=LEFT, padx=2, pady=2)
+        self.pack(side=Tk.LEFT, padx=2, pady=2)
             
     def validate(self, update_validation_status=True):
         # Do the basic integer validation first (integer, in range)
         valid = super().validate(update_validation_status=False)
         if valid and self.entry.get() != "":
             new_channel = int(self.entry.get())
             if new_channel == 14 or new_channel == 15:
@@ -61,17 +61,17 @@
 #    "validate" - validate both entry box values and return True/false
 #------------------------------------------------------------------------------------
 
 class signal_passed_sensor_frame:
     def __init__(self, parent_frame, parent_object):
         # The child class instances need the reference to the parent object so they can call
         # the sibling class method to get the current value of the Signal ID for validation
-        self.frame = LabelFrame(parent_frame, text="Track sensors to associate with signal")
+        self.frame = Tk.LabelFrame(parent_frame, text="Track sensors to associate with signal")
         # Create the elements in a subframe so they are centered
-        self.subframe = Frame(self.frame)
+        self.subframe = Tk.Frame(self.frame)
         self.subframe.pack()
         self.passed = signal_sensor(self.subframe, parent_object, callback=self.validate,
                 label="  Signal 'passed' sensor:", tool_tip = "Specify a GPIO channel in "+
                 "the range 4-13 or 16-26 for the signal 'passed' event (or leave blank)")
         self.approach = signal_sensor(self.subframe, parent_object, callback=self.validate,
                 label="  Signal 'approached' sensor:", tool_tip = "Specify a GPIO channel in "+
                 "the range 4-13 or 16-26 for the signal 'approached' event (or leave blank)")
@@ -98,36 +98,36 @@
 #    "get_value" - will return the last "valid" value (integer)
 # Public Class instance methods provided by the section_ahead_frame class:
 #    "validate" - validate all 'section ahead' entry box values and return True/false
 #------------------------------------------------------------------------------------
 
 class section_behind_element(common.int_item_id_entry_box):
     def __init__(self, parent_frame):
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
-        self.label1 = Label(self.frame, width=1)
-        self.label1.pack(side=LEFT)
+        self.label1 = Tk.Label(self.frame, width=1)
+        self.label1.pack(side=Tk.LEFT)
         tool_tip = "Sepecify the track section 'behind' this signal (to be cleared when the signal is passed)"
         super().__init__(self.frame, tool_tip=tool_tip, exists_function=objects.section_exists)
-        self.pack(side=LEFT)
-        self.label = Label(self.frame, text=" ==>")
-        self.label.pack(side=LEFT)
+        self.pack(side=Tk.LEFT)
+        self.label = Tk.Label(self.frame, text=" ==>")
+        self.label.pack(side=Tk.LEFT)
 
 class section_ahead_element(common.int_item_id_entry_box):
     def __init__(self, parent_frame, label):
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
-        self.label1 = Label(self.frame, text=label, width=10)
-        self.label1.pack(side=LEFT)
+        self.label1 = Tk.Label(self.frame, text=label, width=10)
+        self.label1.pack(side=Tk.LEFT)
         tool_tip = ("Specify the track section on the route 'ahead of' the signal "+
                              "(to be occupied when the signal is passed)")
         super().__init__(self.frame, tool_tip=tool_tip, exists_function=objects.section_exists)
-        self.pack(side=LEFT)
-        self.label2 = Label(self.frame, width=1)
-        self.label2.pack(side=LEFT)
+        self.pack(side=Tk.LEFT)
+        self.label2 = Tk.Label(self.frame, width=1)
+        self.label2.pack(side=Tk.LEFT)
                 
 class section_ahead_frame():
     def __init__(self, parent_frame):
         self.main = section_ahead_element(parent_frame, label=" MAIN ==> ")
         self.lh1 = section_ahead_element(parent_frame, label=" LH1 ==> ")
         self.lh2 = section_ahead_element(parent_frame, label=" LH2 ==> ")
         self.rh1 = section_ahead_element(parent_frame, label=" RH1 ==> ")
@@ -147,20 +147,20 @@
 #    "section_ahead.<route>.disable" - disables/blanks the entry box 
 #    "section_ahead.<route>.enable"  enables/loads the entry box
 #------------------------------------------------------------------------------------
 
 class track_occupancy_frame():
     def __init__(self, parent_frame):
         # Create the Label Frame for the UI element (packed by the creating function/class)
-        self.frame = LabelFrame(parent_frame, text="Track occupancy changes")        
-        self.subframe1 = Frame(self.frame)
-        self.subframe1.pack(side=LEFT)
+        self.frame = Tk.LabelFrame(parent_frame, text="Track occupancy changes")        
+        self.subframe1 = Tk.Frame(self.frame)
+        self.subframe1.pack(side=Tk.LEFT)
         self.section_behind = section_behind_element(self.subframe1)
-        self.subframe2 = Frame(self.frame)
-        self.subframe2.pack(side=LEFT)
+        self.subframe2 = Tk.Frame(self.frame)
+        self.subframe2.pack(side=Tk.LEFT)
         self.section_ahead = section_ahead_frame(self.subframe2)
 
     def set_values(self, sections):
         # sections is a list of [section_behind, sections_ahead]
         # where sections_ahead is a list of [MAIN,LH1,LH2,RH1,RH2]
         self.section_behind.set_value(sections[0])
         self.section_ahead.main.set_value(sections[1][0])
@@ -198,15 +198,15 @@
 #     "set_values" - will set the current values (override, auto)
 #     "get_values" - will return the "valid" values (override, auto)
 #------------------------------------------------------------------------------------
 
 class general_settings_frame():
     def __init__(self, parent_frame):
         # Create the Label Frame for the UI element (packed by the creating function/class)
-        self.frame = LabelFrame(parent_frame, text="General settings")
+        self.frame = Tk.LabelFrame(parent_frame, text="General settings")
         self.automatic = common.check_box(self.frame, width=40,
                     label="  Fully automatic signal (no control button)",
                     tool_tip="Select to create without a main signal button "+
                     "(signal will have a default signal state of OFF, but can be "+
                         "overridden to ON via the selections below)")
         self.automatic.pack(padx=2, pady=2)
         self.distant_automatic = common.check_box(self.frame, width=40,
@@ -256,42 +256,42 @@
 #####################################################################################
 
 class timed_signal_route_element():
     def __init__(self, parent_frame, parent_object, label:str):
         # This is the parent object (the signal instance)
         self.parent_object = parent_object
         # Create a frame for the route element
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the route element (selection, sig ID, start delay, aspect change delay)
-        self.label1 = Label(self.frame, width=5, text=label, anchor='w')
-        self.label1.pack(side=LEFT)
+        self.label1 = Tk.Label(self.frame, width=5, text=label, anchor='w')
+        self.label1.pack(side=Tk.LEFT)
         self.route = common.check_box(self.frame, label="", callback=self.route_selected,
                 tool_tip="Select to trigger a timed signal sequence when the signal is passed (for this route)")
-        self.route.pack(side=LEFT)
-        self.label2 = Label(self.frame, text="  Signal to trigger:")
-        self.label2.pack(side=LEFT)
+        self.route.pack(side=Tk.LEFT)
+        self.label2 = Tk.Label(self.frame, text="  Signal to trigger:")
+        self.label2.pack(side=Tk.LEFT)
         self.sig = common.int_item_id_entry_box(self.frame, allow_empty=False,
                 exists_function=objects.signal_exists, tool_tip="Enter the ID of the signal to "+
                    "trigger. This can be the current signal or another semaphore / colour light "+
                             "signal (on the route ahead of the current signal)")
-        self.sig.pack(side=LEFT)
-        self.label3 = Label(self.frame, text="  Start delay:")
-        self.label3.pack(side=LEFT)
+        self.sig.pack(side=Tk.LEFT)
+        self.label3 = Tk.Label(self.frame, text="  Start delay:")
+        self.label3.pack(side=Tk.LEFT)
         self.start = common.integer_entry_box(self.frame, width=3, min_value=0, max_value=60,
                             allow_empty=False, tool_tip="Specify the time delay (in seconds) "+
                             "before triggering the timed sequence (if triggering the current signal " +
                             " then this should be set to zero to trigger when the signal is passed)")
-        self.start.pack(side=LEFT)
-        self.label4 = Label(self.frame, text="  Time delay:")
-        self.label4.pack(side=LEFT)
+        self.start.pack(side=Tk.LEFT)
+        self.label4 = Tk.Label(self.frame, text="  Time delay:")
+        self.label4.pack(side=Tk.LEFT)
         self.delay = common.integer_entry_box(self.frame, width=3, min_value=0, max_value=60,
                             allow_empty=False, tool_tip="Specify the time period (in seconds) "+
                                                         "between signal aspect changes")
-        self.delay.pack(side=LEFT)
+        self.delay.pack(side=Tk.LEFT)
 
     def route_selected(self):
         if self.route.get_value():
             self.sig.enable1()
             self.start.enable1()
             self.delay.enable1()
             # If no siganl ID is configured then set the ID to the current Signal ID
@@ -347,23 +347,23 @@
 # Note that no overall enable/disable functions are provided - External functions 
 # should call the individual enable/disable functions for each route element
 #------------------------------------------------------------------------------------
 
 class timed_signal_frame():
     def __init__(self, parent_frame, parent_object):
         # Create a label frame for the UI element
-        self.frame = LabelFrame(parent_frame, text="Trigger timed signal sequence")
+        self.frame = Tk.LabelFrame(parent_frame, text="Trigger timed signal sequence")
         # Create a subframe for the context label
-        self.subframe1 = Frame(self.frame)
-        self.subframe1.pack(side=LEFT, padx=2, pady=2, fill='both')        
-        self.label = Label(self.frame, text="Routes to\ntrigger", anchor='w')
-        self.label.pack(side=LEFT)
+        self.subframe1 = Tk.Frame(self.frame)
+        self.subframe1.pack(side=Tk.LEFT, padx=2, pady=2, fill='both')        
+        self.label = Tk.Label(self.frame, text="Routes to\ntrigger", anchor='w')
+        self.label.pack(side=Tk.LEFT)
         # Create a subframe for the route elements
-        self.subframe2 = Frame(self.frame)
-        self.subframe2.pack(side=LEFT, padx=2, pady=2, fill='x', expand=True)        
+        self.subframe2 = Tk.Frame(self.frame)
+        self.subframe2.pack(side=Tk.LEFT, padx=2, pady=2, fill='x', expand=True)        
         self.main=timed_signal_route_element(self.subframe2, parent_object, label="MAIN")
         self.lh1=timed_signal_route_element(self.subframe2, parent_object, label="LH1")
         self.lh2=timed_signal_route_element(self.subframe2, parent_object, label="LH2")
         self.rh1=timed_signal_route_element(self.subframe2, parent_object, label="RH1")
         self.rh2=timed_signal_route_element(self.subframe2, parent_object, label="RH2")
         
     def set_values(self, timed_sequence:[[bool,int,int,int],]):
@@ -404,42 +404,42 @@
 #    "set_values" - set the initial values for the check box and radio buttons
 #    "get_values" - get the current values of the check box and radio buttons
 #------------------------------------------------------------------------------------
 
 class approach_control_route_element():
     def __init__(self, parent_frame, label:str):
         # Create a frame for the route element
-        self.frame = Frame(parent_frame)
+        self.frame = Tk.Frame(parent_frame)
         self.frame.pack()
         # Create the route element (selection, sig ID, start delay, aspect change delay)
-        self.label1 = Label(self.frame, width=5, text=label, anchor='w')
-        self.label1.pack(side=LEFT)
+        self.label1 = Tk.Label(self.frame, width=5, text=label, anchor='w')
+        self.label1.pack(side=Tk.LEFT)
         self.route = common.check_box(self.frame, label="", callback=self.route_selected,
                 tool_tip="Select to enable 'Approach Control' for this route")
-        self.route.pack(side=LEFT)
+        self.route.pack(side=Tk.LEFT)
         # Add a bit of white space
-        self.label2 = Label(self.frame, text="   Release on:")
-        self.label2.pack(side=LEFT)
+        self.label2 = Tk.Label(self.frame, text="   Release on:")
+        self.label2.pack(side=Tk.LEFT)
         # Create the approach control mode selection radiobuttons
-        self.selection = IntVar(self.frame, 0)
+        self.selection = Tk.IntVar(self.frame, 0)
         self.approach_mode = 0
         self.red_enabled = True
         self.yel_enabled = True
         self.sig_enabled = True
-        self.B1 = Radiobutton(self.frame, text="Red", anchor='w',
+        self.B1 = Tk.Radiobutton(self.frame, text="Red", anchor='w',
                 command=self.mode_selected, variable=self.selection, value=1)
-        self.B1.pack(side=LEFT)
+        self.B1.pack(side=Tk.LEFT)
         self.B1TT = common.CreateToolTip(self.B1, "Signal will remain at DANGER until the train approaches")
-        self.B2 = Radiobutton(self.frame, text="Yellow", anchor='w',
+        self.B2 = Tk.Radiobutton(self.frame, text="Yellow", anchor='w',
                 command=self.mode_selected, variable=self.selection, value=2)
-        self.B2.pack(side=LEFT)
+        self.B2.pack(side=Tk.LEFT)
         self.B2TT = common.CreateToolTip(self.B2, "Signal will remain at CAUTION until the train approaches")
-        self.B3 = Radiobutton(self.frame, text="Red (on signals ahead)", anchor='w',
+        self.B3 = Tk.Radiobutton(self.frame, text="Red (on signals ahead)", anchor='w',
                 command=self.mode_selected, variable=self.selection, value=3)
-        self.B3.pack(side=LEFT)
+        self.B3.pack(side=Tk.LEFT)
         self.B3TT = common.CreateToolTip(self.B3, "Signal will remain at DANGER until the train approaches "+
                             "(approach control will only be applied if there is a home signal ahead at danger)")
 
     def mode_selected(self):
         self.approach_mode = self.selection.get()
 
     def route_selected(self):
@@ -522,23 +522,23 @@
 # Note that no route enable/disable functions are provided - External functions 
 # should call the individal route_enable/disable functions for each element
 #------------------------------------------------------------------------------------
 
 class approach_control_frame():
     def __init__(self, parent_frame):
         # Create a label frame for the UI element
-        self.frame = LabelFrame(parent_frame, text="Approach control selections")
+        self.frame = Tk.LabelFrame(parent_frame, text="Approach control selections")
         # Create a subframe for the context label
-        self.subframe1 = Frame(self.frame)
-        self.subframe1.pack(side=LEFT, padx=2, pady=2, fill='both')        
-        self.label = Label(self.frame, text="Routes\nsubject to\napproach\ncontrol", anchor='w')
-        self.label.pack(side=LEFT)
+        self.subframe1 = Tk.Frame(self.frame)
+        self.subframe1.pack(side=Tk.LEFT, padx=2, pady=2, fill='both')        
+        self.label = Tk.Label(self.frame, text="Routes\nsubject to\napproach\ncontrol", anchor='w')
+        self.label.pack(side=Tk.LEFT)
         # Create a subframe for the route elements
-        self.subframe2 = Frame(self.frame)
-        self.subframe2.pack(side=LEFT, padx=2, pady=2, fill='x', expand=True)        
+        self.subframe2 = Tk.Frame(self.frame)
+        self.subframe2.pack(side=Tk.LEFT, padx=2, pady=2, fill='x', expand=True)        
         self.main=approach_control_route_element(self.subframe2, label="MAIN")
         self.lh1=approach_control_route_element(self.subframe2, label="LH1")
         self.lh2=approach_control_route_element(self.subframe2, label="LH2")
         self.rh1=approach_control_route_element(self.subframe2, label="RH1")
         self.rh2=approach_control_route_element(self.subframe2, label="RH2")
         
     def enable_release_on_red(self):
@@ -616,19 +616,19 @@
 
 class signal_automation_tab():
     def __init__(self, parent_tab, parent_object):
         # Create the signal sensor frame (always packed)
         self.track_sensors = signal_passed_sensor_frame(parent_tab, parent_object)
         self.track_sensors.frame.pack(padx=2, pady=2, fill='x')
         # Create a Frame for the track occupancy and general settings (always packed)
-        self.frame1 = Frame(parent_tab)
+        self.frame1 = Tk.Frame(parent_tab)
         self.frame1.pack(padx=2, pady=2, fill='x')
         self.track_occupancy = track_occupancy_frame(self.frame1)
-        self.track_occupancy.frame.pack(side=LEFT, padx=2, pady=2)
+        self.track_occupancy.frame.pack(side=Tk.LEFT, padx=2, pady=2)
         self.general_settings = general_settings_frame(self.frame1)
-        self.general_settings.frame.pack(side=LEFT, padx=2, pady=2, fill='both', expand=True)
+        self.general_settings.frame.pack(side=Tk.LEFT, padx=2, pady=2, fill='both', expand=True)
         # Create a Frame for the timed signal configuration (packed according to signal type)
         self.timed_signal = timed_signal_frame(parent_tab, parent_object)
         # Create a Frame for the Signal Approach control (packed according to signal type)
         self.approach_control = approach_control_frame(parent_tab)
 
 ######################################################################################
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/__init__.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 #    objects_signals.default_signal_object - The dictionary of default values for the object
 #
 #------------------------------------------------------------------------------------
 
 import copy 
 import logging
 
+import tkinter as Tk
+
 from . import objects_common
 from . import objects_signals
 from . import objects_points
 from . import objects_lines
 from . import objects_sections
 from . import objects_instruments
 
@@ -247,15 +249,15 @@
     elif new_object_type == objects_common.object_type.signal:
         objects_signals.create_signal(item_type, item_subtype)
     elif new_object_type == objects_common.object_type.point:
          objects_points.create_point(item_type)
     elif new_object_type == objects_common.object_type.section:
         objects_sections.create_section()
     elif new_object_type == objects_common.object_type.instrument:
-        objects_instruments.create_instrument()
+        objects_instruments.create_instrument(item_type)
     # save the current state (for undo/redo)
     save_schematic_state()
     # As we are creating 'new' objects we don't need to process layout changes
     return()
 
 #------------------------------------------------------------------------------------
 # Function to update the configuration of an existing schematic object and re-draw it
@@ -432,46 +434,63 @@
 # Function to set (re-create) all schematic objects (following a file load)
 # Note that there is a dependancy that the main schematic objects dict is empty
 # i.e. any legacy objects existing prior to the load will have been deleted first
 #------------------------------------------------------------------------------------
 
 def set_all(new_objects):
     global logging
+    # List of error messages to report
+    warning_messages = ""
     # For each loaded object, create a new default object of the same type
     # and then copy across each element in turn. This is defensive programming
     # to populate the objects gracefully whilst handling changes to an object
     # structre (e.g. new element introduced since the file was last saved)
     for object_id in new_objects:
+        # Get the item id of the new object - for error reporting
+        # The 'item' and 'itemid' elements are MANDATORY for all objects 
+        item_id = str(new_objects[object_id]["itemid"])
+        # Set the type-specific default object
         new_object_type = new_objects[object_id]["item"]
         if new_object_type == objects_common.object_type.line:
             default_object = objects_lines.default_line_object
         elif new_object_type == objects_common.object_type.signal:
             default_object = objects_signals.default_signal_object
         elif new_object_type == objects_common.object_type.point:
             default_object = objects_points.default_point_object
         elif new_object_type == objects_common.object_type.section:
             default_object = objects_sections.default_section_object
         elif new_object_type == objects_common.object_type.instrument:
             default_object = objects_instruments.default_instrument_object
         else:
             default_object = {}
-            logging.error("LOAD LAYOUT - Object type '"+new_object_type+" not recognised")
+            logging.warning("LOAD LAYOUT - "+new_object_type+" "+item_id+" - Unrecognised object type: '"+new_object_type+"'")
+            warning_messages += (new_object_type+" "+item_id+" - Unrecognised object type - DISCARDED\n")
         # Populate each element at a time and report any elements not recognised
         if default_object != {}:
             objects_common.schematic_objects[object_id] = copy.deepcopy(default_object)
             for element in new_objects[object_id]:
                 if element not in default_object.keys():
-                    logging.warning("LOAD LAYOUT - Unexpected "+new_object_type+" element '"+element+"'")
+                    logging.warning("LOAD LAYOUT - "+new_object_type+" "+item_id+" - Unexpected element: '"+element+"'")
+                    warning_messages += (new_object_type+" "+item_id+" - Unexpected element: '"+element+"'\n")
                 else:
                     objects_common.schematic_objects[object_id][element] = new_objects[object_id][element]        
             # Now report any elements missing from the new object - intended to provide a
             # level of backward capability (able to load old config files into an extended config)
             for element in default_object:
                 if element not in new_objects[object_id].keys():
-                    logging.warning("LOAD LAYOUT - Missing "+new_object_type+" element '"+element+"'")
+                    logging.warning("LOAD LAYOUT - "+new_object_type+" "+item_id+" - Missing element: '"+element+"'")
+                    warning_messages += (new_object_type+" "+item_id+" - Missing element: '"+element+"'\n")
+                    #############################################################################################
+                    # Set any mandatory elements - to prevent the application from breaking
+                    # When loading files saved by old versions of the application (this specifically
+                    # for the block instrument type breaking change from Release 3.2.0 to 3.3.0
+                    if element == "itemtype": objects_common.schematic_objects[object_id][element] = 1
+                    #############################################################################################
+    # Report the error messages
+    if warning_messages != "": display_warnings(warning_messages)
     # Reset the signal/point/section/instrument indexes
     reset_all_schematic_indexes()
     # Redraw (re-create) all items on the schematic with a new bbox
     redraw_all_objects(create_new_bbox=True)
     # Ensure all track sections are in front of any lines
     bring_track_sections_to_the_front()
     # Recalculate point interlocking tables as a 'belt and braces' measure (on the 
@@ -486,9 +505,34 @@
 #------------------------------------------------------------------------------------
 # Function get the current objects dictionary (for saving to file)
 #------------------------------------------------------------------------------------
 
 def get_all():
     return(objects_common.schematic_objects)
 
+#------------------------------------------------------------------------------------
+# Internal Function to generate a popup window to display load errors
+#------------------------------------------------------------------------------------
+
+class display_warnings():
+    def __init__(self, warnings:str):
+        # Create the top level window for the canvas settings
+        winx = objects_common.canvas.winfo_rootx() + 250
+        winy = objects_common.canvas.winfo_rooty() + 50
+        self.window = Tk.Toplevel(objects_common.canvas)
+        self.window.geometry(f'+{winx}+{winy}')
+        self.window.title("Load Warnings")
+        self.window.attributes('-topmost',True)
+        self.label1 = Tk.Label(self.window, font="Helvetica 12 bold", text=
+                    "WARNING - Layout file generated by a different\n"+
+                    "version of the application - Check configuration")
+        self.label1.pack(padx=2, pady=2)
+        self.label2 = Tk.Label(self.window, text=warnings, justify=Tk.LEFT)
+        self.label2.pack(padx=2, pady=2)
+        # Create the close button 
+        self.B1 = Tk.Button (self.window, text = "Ok / Close",command=self.ok)
+        self.B1.pack(padx=2, pady=2)
+
+    def ok(self):
+        self.window.destroy()
 
 ####################################################################################
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_common.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_common.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_lines.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_lines.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_points.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_points.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_sections.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_sections.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/objects/objects_signals.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/objects/objects_signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 from ...library import signals_ground_position
 from ...library import signals_ground_disc
 from ...library import dcc_control
 from ...library import track_sensors
 
 from . import objects_common
 from . import objects_points
-from . import objects_instruments
 from .. import run_layout
 
 #------------------------------------------------------------------------------------
 # Default Signal Objects (i.e. state at creation)
 #------------------------------------------------------------------------------------
 
 # This is the default signal object definition
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/resources/block_instrument.png` & `model-railway-signals-3.3.0/model_railway_signals/editor/resources/block_instrument.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/resources/track_section.png` & `model-railway-signals-3.3.0/model_railway_signals/editor/resources/track_section.png`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/run_layout.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/run_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Accesses the following external library objects directly:
 #    signals_common.route_type - for accessing the enum value
 #    signals_common.sig_type - for accessing the enum value
 #    signals_common.sig_callback_type - for accessing the enum value
 #    points.point_callback_type - for accessing the enum value
 #    track_sections.section_callback_type - for accessing the enum value
 #    block_instruments.block_callback_type - for accessing the enum value
+#    block_instruments.block_section_ahead_clear - for interlocking
 #    signals_colour_lights.signal_sub_type - for accessing the enum value
 #    signals_semaphores.semaphore_sub_type - for accessing the enum value
 #    <MORE COMING>
 #
 # Makes the following external API calls to library modules:
 #    signals.signal_state(sig_id) - For testing the current displayed aspect
 #    signals.update_signal(sig_id, sig_ahead_id) - To update the signal aspect
@@ -220,21 +221,25 @@
 # is a remote signal then we should stop processing (as we have no idea of the
 # signal type) and return home_signal_at_danger=False
 #####################################################################################
 #------------------------------------------------------------------------------------
 
 def distant_signal_ahead_at_caution(signal_object):
     sig_ahead = find_signal_ahead(signal_object)
-    sig_ahead_id = sig_ahead["itemid"]
-    is_distant = ( ( sig_ahead["itemtype"] == signals_common.sig_type.colour_light.value and
-                     sig_ahead["itemsubtype"] == signals_colour_lights.signal_sub_type.distant.value ) or
-                   ( sig_ahead["itemtype"] == signals_common.sig_type.semaphore.value and
-                     sig_ahead["itemsubtype"] == signals_colour_lights.signal_sub_type.distant.value ) )
-    signal_at_caution = (signals.signal_state(sig_ahead_id) == signals_common.signal_state_type.CAUTION)
-    return(is_distant and signal_at_caution)
+    if sig_ahead is not None:
+        sig_ahead_id = sig_ahead["itemid"]
+        is_distant = ( ( sig_ahead["itemtype"] == signals_common.sig_type.colour_light.value and
+                         sig_ahead["itemsubtype"] == signals_colour_lights.signal_sub_type.distant.value ) or
+                       ( sig_ahead["itemtype"] == signals_common.sig_type.semaphore.value and
+                         sig_ahead["itemsubtype"] == signals_colour_lights.signal_sub_type.distant.value ) )
+        signal_at_caution = (signals.signal_state(sig_ahead_id) == signals_common.signal_state_type.CAUTION)
+        distant_signal_at_caution = is_distant and signal_at_caution
+    else:
+        distant_signal_at_caution = False
+    return(distant_signal_at_caution)        
 
 #------------------------------------------------------------------------------------
 # Internal function to find any colour light signals which are configured to update aspects
 # based on the aspect of the signal that has changed (i.e. signals "behind"). The function
 # is recursive and keeps working back along the route until there are no further changes
 # that need propagating backwards. A maximum recursion depth provides a level of protection.
 #####################################################################################
@@ -477,14 +482,22 @@
                 for index, opposing_sig_route in enumerate(opposing_sig_routes):
                     if opposing_sig_route:
                         if (signals.signal_clear(opposing_signal_id,signals_common.route_type(index+1)) or
                             ( has_subsidary(opposing_signal_id) and
                                 signals.subsidary_clear(opposing_signal_id,signals_common.route_type(index+1)))):
                             subsidary_can_be_unlocked = False
                             signal_can_be_unlocked = False
+            # See if the signal is interlocked with a block instrument on the route ahead
+            # Each route comprises: [[p1, p2, p3, p4, p5, p6, p7] signal, block_inst]
+            # The block instrument is the local block instrument - ID is an integer
+            block_instrument = signal_object["pointinterlock"][signal_route.value-1][2]
+            if block_instrument != 0:
+                block_clear = block_instruments.block_section_ahead_clear(block_instrument)
+                if not block_clear and not signals.signal_clear(signal_object["itemid"]):
+                    signal_can_be_unlocked = False
             # The "interlockedahead" flag will only be True if selected and it can only be selected for
             # a semaphore distant, a colour light distant or a semaphore home with secondary distant arms
             # In the latter case then a call to "has_distant_arms" will be true (false for all other types)
             if signal_object["interlockahead"] and home_signal_ahead_at_danger(signal_object):
                 if has_distant_arms(signal_object):
                     # Must be a home semaphore signal with secondary distant arms
                     if not signals.signal_clear(signal_object["itemid"]+100):
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/schematic.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/schematic.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,44 +21,48 @@
 #    objects.paste_objects() - Paste the selected objects (returns a list of new IDs)
 #    objects.undo() / objects.redo() - Undo and re-do functions as you would expect
 #    objects.enable_editing() - Call when 'Edit' Mode is selected 
 #    objects.disable_editing() - Call when 'Run' Mode is selected
 #    configure_signal.edit_signal(root,object_id) - Open signal edit window (on double click)
 #    configure_point.edit_point(root,object_id) - Open point edit window (on double click)
 #    configure_section.edit_section(root,object_id) - Open section edit window (on double click)
+#    configure_instrument.edit_instrument(root,object_id) - Open inst edit window (on double click)
 #    ########################## More to be added ########################################
 #
 # Accesses the following external editor objects directly:
 #    objects.schematic_objects - the dict holding descriptions for all objects
 #    objects.object_type - used to establish the type of the schematic objects
 #
 # Accesses the following external library objects directly:
 #    signals_common.sig_type - Used to access the signal type
 #    signals_colour_lights.signal_sub_type - Used to access the signal subtype
 #    signals_semaphores.semaphore_sub_type - Used to access the signal subtype
 #    signals_ground_position.ground_pos_sub_type - Used to access the signal subtype
 #    signals_ground_disc.ground_disc_sub_type - Used to access the signal subtype
+#    block_instruments.instrument_type - Used to access the block_instrument type
 #    points.point_type - Used to access the point type
 #    ########################## More to be added ########################################
 #
 #------------------------------------------------------------------------------------
 
-from tkinter import *
+import tkinter as Tk
 
 from ..library import signals_common
 from ..library import signals_colour_lights
 from ..library import signals_semaphores
 from ..library import signals_ground_position
 from ..library import signals_ground_disc
+from ..library import block_instruments
 from ..library import points
 
 from . import objects
 from . import configure_signal
 from . import configure_point
 from . import configure_section
+from . import configure_instrument
 
 import importlib.resources
 import logging
 import math
 import copy
 
 #------------------------------------------------------------------------------------
@@ -76,15 +80,14 @@
 schematic_state["editlineend2"] = False
 schematic_state["selectarea"] = False
 schematic_state["selectareabox"] = None      # Tkinter drawing object
 schematic_state["selectedobjects"] = []
 # The Root reference is used when calling a "configure object" module (to open a popup window)
 # The Canvas reference is used for configuring and moving canvas widgets for schematic editing
 # canvas_width / canvas_height / canvas_grid are used for positioning of objects
-canvas = None
 root = None
 canvas = None
 canvas_width = 0
 canvas_height = 0
 canvas_grid = 0
 # The callback to make (for selected canvas events). Currently only the mode change keypress
 # event makes this callback (to enable the application mode to be toggled between edit and run)
@@ -183,15 +186,15 @@
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.signal:
         configure_signal.edit_signal(root, object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.point:
         configure_point.edit_point(root, object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.section:
         configure_section.edit_section(root,object_id)
     elif objects.schematic_objects[object_id]["item"] == objects.object_type.instrument:
-        pass; #################### TODO #############################
+        configure_instrument.edit_instrument(root,object_id)
     return()
 
 #------------------------------------------------------------------------------------
 # Internal function to edit a line object on the canvas. The "editlineend1" and
 # "editlineend2" dictionary elements specify the line end that needs to be moved
 # Only a single Object will be selected when this function is called
 #------------------------------------------------------------------------------------
@@ -603,19 +606,20 @@
 # Externally called Functions to enable/disable schematic editing
 # Either from the Menubar Mode selection or the 'm' key
 #------------------------------------------------------------------------------------
 
 def enable_editing():
     global schematic_state
     global canvas_event_callback
+    global button_frame
     canvas.itemconfig("grid",state="normal")
     # Enable editing of the schematic objects
     objects.enable_editing()
     # Re-pack the subframe containing the "add object" buttons to display it        
-    button_frame.pack(side=RIGHT, expand=False, fill=BOTH)
+    button_frame.pack(side=Tk.RIGHT, expand=False, fill=Tk.BOTH)
     # Bind the Canvas mouse and button events to the various callback functions
     canvas.bind("<Motion>", track_cursor)
     canvas.bind('<Button-1>', left_button_click)
     canvas.bind('<Button-2>', right_button_click)
     canvas.bind('<Button-3>', right_button_click)
     canvas.bind('<Shift-Button-1>', left_shift_click)
     canvas.bind('<ButtonRelease-1>', left_button_release)
@@ -660,97 +664,98 @@
     global button_frame
     global button_images
     global canvas_event_callback
     global logging
     root = root_window
     canvas_event_callback = event_callback
     # Create a frame to hold the two subframes ("add" buttons and drawing canvas)
-    frame = Frame(root_window)
-    frame.pack (expand=True, fill=BOTH)    
+    frame = Tk.Frame(root_window)
+    frame.pack (expand=True, fill=Tk.BOTH)    
     # Create a subframe to hold the canvas and scrollbars
-    canvas_frame = Frame(frame, borderwidth=1)
-    canvas_frame.pack(side=RIGHT, expand=True, fill=BOTH)
+    canvas_frame = Tk.Frame(frame, borderwidth=1)
+    canvas_frame.pack(side=Tk.RIGHT, expand=True, fill=Tk.BOTH)
     # Create a subframe to hold the "add" buttons
-    button_frame = Frame(frame, borderwidth=1)
-    button_frame.pack(side=RIGHT, expand=True, fill=BOTH)
+    button_frame = Tk.Frame(frame, borderwidth=1)
+    button_frame.pack(side=Tk.RIGHT, expand=True, fill=Tk.BOTH)
     # Save the Default values for the canvas as global variables
     canvas_width, canvas_height, canvas_grid = width, height, grid
-    # Create the canvas and scrollbars inside the parentframe
+    # Create the canvas and scrollbars inside the parent frame
     # We also set focus on the canvas so the keypress events will take effect
-    canvas = Canvas(canvas_frame ,bg="grey85", scrollregion=(0, 0, canvas_width, canvas_height))
+    canvas = Tk.Canvas(canvas_frame ,bg="grey85", scrollregion=(0, 0, canvas_width, canvas_height))
     canvas.focus_set()
-    hbar = Scrollbar(canvas_frame, orient=HORIZONTAL)
-    hbar.pack(side=BOTTOM, fill=X)
+    hbar = Tk.Scrollbar(canvas_frame, orient=Tk.HORIZONTAL)
+    hbar.pack(side=Tk.BOTTOM, fill=Tk.X)
     hbar.config(command=canvas.xview)
-    vbar = Scrollbar(canvas_frame, orient=VERTICAL)
-    vbar.pack(side=RIGHT, fill=Y)
+    vbar = Tk.Scrollbar(canvas_frame, orient=Tk.VERTICAL)
+    vbar.pack(side=Tk.RIGHT, fill=Tk.Y)
     vbar.config(command=canvas.yview)
     canvas.config(width=canvas_width, height=canvas_height)
     canvas.config(xscrollcommand=hbar.set, yscrollcommand=vbar.set)
-    canvas.pack(side=LEFT, expand=True, fill=BOTH)
+    canvas.pack(side=Tk.LEFT, expand=True, fill=Tk.BOTH)
     # Define the Object Popup menu for Right Click (something selected)
-    popup1 = Menu(tearoff=0)
+    popup1 = Tk.Menu(tearoff=0)
     popup1.add_command(label="Copy", command=copy_selected_objects)
     popup1.add_command(label="Edit", command=edit_selected_object)
     popup1.add_command(label="Rotate", command=rotate_selected_objects)
     popup1.add_command(label="Delete", command=delete_selected_objects)
     # Define the Canvas Popup menu for Right Click (nothing selected)
-    popup2 = Menu(tearoff=0)
+    popup2 = Tk.Menu(tearoff=0)
     popup2.add_command(label="Paste", command=paste_clipboard_objects)
     popup2.add_command(label="Select all", command=select_all_objects)
     # Now draw the initial grid
     draw_grid()
     # Load the images for the for the "add object" buttons
     resource_folder = 'model_railway_signals.editor.resources'
     file_names = ['line','colour_light','semaphore','ground_position','ground_disc',
                 'left_hand_point','right_hand_point','track_section','block_instrument']
     for file_name in file_names:
         try:
             with importlib.resources.path (resource_folder,(file_name+'.png')) as file_path:
-                button_images[file_name] = PhotoImage(file=file_path)
+                button_images[file_name] = Tk.PhotoImage(file=file_path)
         except:
             logging.error ("SCHEMATIC EDITOR - Error loading image file '"+file_name+".png'")
             button_images[file_name]=None
     # Add The Buttons for creating new objects and adding to the schematic
     # Note that for enumeration types we pass the "value"
-    button1 = Button (button_frame, image=button_images['line'],
+    button1 = Tk.Button (button_frame, image=button_images['line'],
                       command=lambda:objects.create_object(objects.object_type.line))
     button1.pack (padx=2 ,pady=2)
-    button2 = Button (button_frame, image=button_images['colour_light'],
+    button2 = Tk.Button (button_frame, image=button_images['colour_light'],
                       command=lambda:objects.create_object(objects.object_type.signal,
                            signals_common.sig_type.colour_light.value,
                            signals_colour_lights.signal_sub_type.four_aspect.value) )
     button2.pack (padx=2, pady=2)
-    button3 = Button (button_frame, image=button_images['semaphore'],
+    button3 = Tk.Button (button_frame, image=button_images['semaphore'],
                       command=lambda:objects.create_object(objects.object_type.signal,
                            signals_common.sig_type.semaphore.value,
                            signals_semaphores.semaphore_sub_type.home.value))
     button3.pack (padx=2, pady=2)
-    button4 = Button (button_frame, image=button_images['ground_position'],
+    button4 = Tk.Button (button_frame, image=button_images['ground_position'],
                       command=lambda:objects.create_object(objects.object_type.signal,
                            signals_common.sig_type.ground_position.value,
                            signals_ground_position.ground_pos_sub_type.standard.value))
     button4.pack (padx=2, pady=2)
-    button5 = Button (button_frame, image=button_images['ground_disc'],
+    button5 = Tk.Button (button_frame, image=button_images['ground_disc'],
                       command=lambda:objects.create_object(objects.object_type.signal,
                            signals_common.sig_type.ground_disc.value,
                            signals_ground_disc.ground_disc_sub_type.standard.value))
     button5.pack (padx=2, pady=2)
-    button6 = Button (button_frame, image=button_images['left_hand_point'],
+    button6 = Tk.Button (button_frame, image=button_images['left_hand_point'],
                       command=lambda:objects.create_object(objects.object_type.point,
                            points.point_type.LH.value))
     button6.pack (padx=2, pady=2)
-    button7 = Button (button_frame, image=button_images['right_hand_point'],
+    button7 = Tk.Button (button_frame, image=button_images['right_hand_point'],
                       command=lambda:objects.create_object(objects.object_type.point,
                             points.point_type.RH.value))
     button7.pack (padx=2, pady=2)
-    button8 = Button (button_frame, image=button_images['track_section'],
+    button8 = Tk.Button (button_frame, image=button_images['track_section'],
                       command=lambda:objects.create_object(objects.object_type.section))
     button8.pack (padx=2, pady=2)
-    button9 = Button (button_frame, image=button_images['block_instrument'],
-                      command=lambda:objects.create_object(objects.object_type.instrument))
+    button9 = Tk.Button (button_frame, image=button_images['block_instrument'],
+                      command=lambda:objects.create_object(objects.object_type.instrument,
+                            block_instruments.instrument_type.single_line.value))
     button9.pack (padx=2, pady=2)
     # Initialise the Objects package with the required parameters
     objects.initialise(canvas, canvas_width, canvas_height, canvas_grid)
     return()
 
 ####################################################################################
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/editor/settings.py` & `model-railway-signals-3.3.0/model_railway_signals/editor/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # These are the default settings
 #------------------------------------------------------------------------------------
 
 default_settings = {}
 default_settings["general"] = {}
 default_settings["general"]["filename"] = "new_layout.sig"
 default_settings["general"]["editmode"] = True
-default_settings["general"]["version"] = "Version 3.2.0"
+default_settings["general"]["version"] = "Version 3.3.0"
 default_settings["canvas"] = {}
 default_settings["canvas"]["width"] = 1000
 default_settings["canvas"]["height"] = 500
 default_settings["canvas"]["grid"] = 25
 default_settings["logging"] = {}
 default_settings["logging"]["level"] = 2   # Warning
 default_settings["sprog"] = {}
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/block_instruments.py` & `model-railway-signals-3.3.0/model_railway_signals/library/block_instruments.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 # -----------------------------------------------------------------------------------------------
 #
 # Public types and functions: 
 # 
 # block_callback_type (tells the calling program what has triggered the callback)
 #     block_section_ahead_updated - The block section AHEAD of our block section has been updated
 #                             (i.e. the block section state represented by the Repeater indicator)
+#
+# instrument_type - enumeration type - single_line or double_line
 # 
 # create_block_instrument - Creates a Block Section Instrument on the schematic
 #   Mandatory Parameters:
 #       Canvas - The Tkinter Drawing canvas on which the instrument is to be displayed
 #       block_id:int - The local identifier to be used for the Block Instrument 
 #       x:int, y:int - Position of the instrument on the canvas (in pixels)
 #   Optional Parameters:
+#       inst_type:instrument_type - either instrument_type.single_line or instrument_type.double_line
 #       block_callback - The function to call when the repeater indicator on our instrument has been
 #                        updated (i.e. the block changed on the linked instrument) - default: null
 #                        Note that the callback function returns (item_id, callback type)
-#       single_line:bool - for a single line instrument(created without a repeater) - default: False
+#       single_line:bool - DEPRECATED - use inst_type instead
 #       bell_sound_file:str - The filename of the soundfile (in the local package resources
 #                           folder) to use for the bell sound (default "bell-ring-01.wav")
 #       telegraph_sound_file:str - The filename of the soundfile (in the local package resources)
 #                           to use for the Telegraph key sound (default "telegraph-key-01.wav")
 #       linked_to:int/str - the identifier for the "paired" block instrument - can be specified
 #                           either as an integer (representing the ID of a Block Instrument on the
 #                           the local schematic), or a string representing a Block Instrument 
@@ -37,28 +40,28 @@
 # 
 # block_section_ahead_clear(block_id:int) - Returns the state of the ASSOCIATED block instrument
 #           (i.e. the linked instrument controlling the state of the block section ahead of ours)
 #           This can be used to implement full interlocking of the Starter signal in our section
 #           (i.e. signal locked at danger until the box ahead sets their instrument to LINE-CLEAR)
 #           Returned state is: True = LINE-CLEAR, False = LINE-BLOCKED or TRAIN-ON-LINE
 #
-#
 # If you want to use Block Instruments with full sound enabled (bell rings and telegraph key sounds)
 # then you will also need to install the 'simpleaudio' package. Note that for Windows it has a dependency 
 # on Microsoft Visual C++ 14.0 or greater (so you will need to ensure Visual Studio 2015 is installed first)
 # If 'simpleaudio' is not installed then the software will still function correctly (just without sound)
 #
 # -----------------------------------------------------------------------------------------------
 
 from . import common
 from . import mqtt_interface
 from . import file_interface
-from tkinter import *
 from typing import Union
+import tkinter as Tk
 import enum
+import os
 import logging
 import importlib.resources
 
 # We can only use audio for the block instruments if 'simpleaudio' is installed
 # Although this package is supported across different platforms, for Windows
 # it has a dependency on Visual C++ 14.0. As this is quite a faff to install I
 # haven't made audio a hard and fast dependency for the 'model_railway_signals'
@@ -73,14 +76,18 @@
     return (False)
 audio_enabled = is_simpleaudio_installed()
 
 # -------------------------------------------------------------------------
 # Classes used by external functions when calling the create_point function
 # -------------------------------------------------------------------------
     
+class instrument_type(enum.Enum):
+    single_line = 1   # Right Hand point
+    double_line = 2   # Left Hand point
+
 class block_callback_type(enum.Enum):
     block_section_ahead_updated = 51   # The instrument has been updated
 
 # --------------------------------------------------------------------------------
 # Block Instruments are to be added to a global dictionary when created
 # --------------------------------------------------------------------------------
 
@@ -127,27 +134,27 @@
         bell_codes.append ([" 3"," Is line clear for stopping freight train"])
         bell_codes.append ([" 3 - 1"," Is line clear for stopping passenger train"])
         bell_codes.append ([" 3 - 1 - 1"," Is line clear for express freight train"])
         bell_codes.append ([" 4"," Is line clear for express passenger train"])
         bell_codes.append ([" 4 - 1"," Is line clear for mineral or empty waggon train"])
         bell_codes.append ([" 2 - 1"," Train arrived"])
         bell_codes.append ([" 6"," Obstruction danger"])
-        hints_window = Toplevel(common.root_window)
+        hints_window = Tk.Toplevel(common.root_window)
         hints_window.attributes('-topmost',True)
         hints_window.title("Common signal box bell codes")
         hints_window.protocol("WM_DELETE_WINDOW", lambda:close_bell_code_hints(hints_window))
         bell_code_hints_open = True
         for row, item1 in enumerate (bell_codes, start=1):
-            text_entry_box1 = Entry(hints_window,width=8)
+            text_entry_box1 = Tk.Entry(hints_window,width=8)
             text_entry_box1.insert(0,item1[0])
             text_entry_box1.grid(row=row,column=1)
             text_entry_box1.config(state='disabled')
             text_entry_box1.config({'disabledbackground':'white'}) 
             text_entry_box1.config({'disabledforeground':'black'}) 
-            text_entry_box2 = Entry(hints_window,width=40)
+            text_entry_box2 = Tk.Entry(hints_window,width=40)
             text_entry_box2.insert(0,item1[1])
             text_entry_box2.grid(row=row,column=2)
             text_entry_box2.config(state='disabled')
             text_entry_box2.config({'disabledbackground':'white'}) 
             text_entry_box2.config({'disabledforeground':'black'}) 
     return()
 
@@ -346,17 +353,22 @@
             # Set the local block indication to reflect the state that has been set locally
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "hidden")
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "hidden")
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "normal")
             # If linked to another instrument then update the repeater indicator on the other instrument or
             # Publish the initial state to the broker (for other nodes to consume). Note that state will only
             # be published if the MQTT interface has been configured and we are connected to the broker
-            if update_remote_instrument and instruments[str(block_id)]["linkedto"] is not None:
-                if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
-                else: set_repeater_blocked(instruments[str(block_id)]["linkedto"])
+            if update_remote_instrument:
+                if instruments[str(block_id)]["linkedto"] is not None:
+                    if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
+                    else: set_repeater_blocked(instruments[str(block_id)]["linkedto"])
+                # Handle the case of a single line instrument with no linked instrument - in this case we
+                # want to make a callback on block state change to allow interlocking to be processed
+                elif instruments[str(block_id)]["singleline"]:
+                    instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)            
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal Function to set the main block section indicator to CLEAR
 # called when the "CLEAR" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
@@ -387,17 +399,22 @@
             # Set the local block indication to reflect the state that has been set locally
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "hidden")
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "normal")
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "hidden")
             # If linked to another instrument then update the repeater indicator on the other instrument or
             # Publish the initial state to the broker (for other nodes to consume). Note that state will only
             # be published if the MQTT interface has been configured and we are connected to the broker
-            if update_remote_instrument and instruments[str(block_id)]["linkedto"] is not None:
-                if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
-                else: set_repeater_clear(instruments[str(block_id)]["linkedto"])
+            if update_remote_instrument:
+                if instruments[str(block_id)]["linkedto"] is not None:
+                    if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
+                    else: set_repeater_clear(instruments[str(block_id)]["linkedto"])
+                # Handle the case of a single line instrument with no linked instrument - in this case we
+                # want to make a callback on block state change to allow interlocking to be processed
+                elif instruments[str(block_id)]["singleline"]:
+                    instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)            
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal Function to set the main block section indicator to OCCUPIED
 # called when the "OCCUP" button is clicked on the local block instrument
 # Also called for single-line block instruments (without a repeater display)
 # following a state change of the linked remote block instrument
@@ -428,17 +445,22 @@
             # Set the local block indication to reflect the state that has been set locally
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatoroccup"],state = "normal")
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorclear"],state = "hidden")
             instruments[str(block_id)]["canvas"].itemconfigure(instruments[str(block_id)]["myindicatorblock"],state = "hidden")
             # If linked to another instrument then update the repeater indicator on the other instrument or
             # Publish the initial state to the broker (for other nodes to consume). Note that state will only
             # be published if the MQTT interface has been configured and we are connected to the broker
-            if update_remote_instrument and instruments[str(block_id)]["linkedto"] is not None:
-                if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
-                else: set_repeater_occupied(instruments[str(block_id)]["linkedto"])
+            if update_remote_instrument:
+                if instruments[str(block_id)]["linkedto"] is not None:
+                    if isinstance(instruments[str(block_id)]["linkedto"],str): send_mqtt_instrument_updated_event(block_id)
+                    else: set_repeater_occupied(instruments[str(block_id)]["linkedto"])
+                # Handle the case of a single line instrument with no linked instrument - in this case we
+                # want to make a callback on block state change to allow interlocking to be processed
+                elif instruments[str(block_id)]["singleline"]:
+                    instruments[str(block_id)]["extcallback"] (block_id,block_callback_type.block_section_ahead_updated)            
     return ()
 
 # --------------------------------------------------------------------------------
 # Internal function to create the Indicator component of a Block Instrument
 # --------------------------------------------------------------------------------
 
 def create_block_indicator(canvas:int, x:int, y:int, block_id_tag):
@@ -450,98 +472,128 @@
     canvas.create_oval(x-5, y-5, x+5, y+5, fill='black', outline="black", width=0, tags=block_id_tag)
     block = canvas.create_line (x+0, y-5, x+0,  y + 35, fill='black', width = 3, state='normal', tags=block_id_tag)
     clear = canvas.create_line (x-3, y-3, x+25, y + 25, fill='black', width = 3, state='hidden', tags=block_id_tag)
     occup = canvas.create_line (x+3, y-3, x-25, y + 25, fill='black', width = 3 , state='hidden', tags=block_id_tag)
     return (block, clear, occup)
 
 # --------------------------------------------------------------------------------
+# Internal function to load a specified audio file for the bell / telegraph key sounds.
+# If these fail to load for any reason then no sounds will be produced on these events
+# If the filename isn't fully qualified then it assume a file in the resources folder
+# --------------------------------------------------------------------------------
+
+def load_audio_file(audio_filename):
+    audio_object = None
+    if os.path.split(audio_filename)[1] == audio_filename:
+        try:
+            with importlib.resources.path ('model_railway_signals.library.resources',audio_filename) as audio_file:
+                audio_object = simpleaudio.WaveObject.from_wave_file(str(audio_file))
+        except:
+            Tk.messagebox.showerror(parent=common.root_window, title="Load Error",
+                            message="Error loading audio resource file '"+str(audio_filename)+"'")
+            logging.error ("Block Instruments - Error loading audio resource file '"+str(audio_filename)+"'")       
+    else:        
+        try:
+            audio_object = simpleaudio.WaveObject.from_wave_file(str(audio_filename))
+        except:
+            Tk.messagebox.showerror(parent=common.root_window, title="Load Error",
+                            message="Error loading audio file '"+str(audio_filename)+"'")
+            logging.error ("Block Instruments - Error loading audio file '"+str(audio_filename)+"'")       
+    return(audio_object)
+
+# --------------------------------------------------------------------------------
 # Public API function to create a Block  Instrument (drawing objects and internal state)
 # --------------------------------------------------------------------------------
 
 def create_block_instrument (canvas,
                              block_id:int,
                              x:int, y:int,
+                             inst_type:instrument_type = instrument_type.double_line,
                              block_callback = null_callback,
-                             single_line:bool = False,
+                             single_line:bool = False, ############################################################
                              bell_sound_file:str = "bell-ring-01.wav",
                              telegraph_sound_file:str = "telegraph-key-01.wav",
                              linked_to:Union[int,str] = None):
     global instruments
     global audio_enabled
     global logging
     logging.info ("Block Instrument "+str(block_id)+": Creating Block Instrument")
     # Find and store the root window (when the first block instrument is created)
     if common.root_window is None: common.find_root_window(canvas)
+    # Establish whether the ID is a local or remote ID and set the type accordingly
+    # We need to do this for the editor as the editor will give us an int as a string
+    if linked_to is None or linked_to == "":
+        linked_to_id = None
+    else:
+        try: linked_to_id = int(linked_to)
+        except: linked_to_id = str(linked_to)
     # Do some basic validation on the parameters we have been given
     if instrument_exists(block_id):
         logging.error ("Block Instrument "+str(block_id)+": Instrument already exists")
     elif block_id < 1:
         logging.error ("Block Instrument "+str(block_id)+": Block ID must be greater than zero")
-    elif linked_to == block_id:
+    elif linked_to_id == block_id:
         logging.error ("Block Instrument "+str(block_id)+": ID for linked instrument is the same as the instrument to create")   
-    elif isinstance(linked_to,str) and mqtt_interface.split_remote_item_identifier(linked_to) is None:
+    elif isinstance(linked_to_id,str) and mqtt_interface.split_remote_item_identifier(linked_to_id) is None:
         logging.error ("Block Instrument "+str(block_id)+": Compound ID for remote-node instrument is invalid")   
     else:
+        ####################################################################################################################
+        if single_line:
+            logging.warning ("###########################################################################################")
+            logging.warning ("Block Instrument "+str(block_id)+": single_line flag is DEPRECATED - use inst_type")
+            logging.warning ("###########################################################################################")
+        else:
+            single_line = (inst_type == instrument_type.single_line)
+        ####################################################################################################################
         # Define the "Tag" for all drawing objects for this instrument instance
         block_id_tag = "instrument"+str(block_id)
         # Create the Instrument background - this will vary in size depending on single or double line
         if single_line: canvas.create_rectangle (x-60, y-20, x+60, y+150, fill = "saddle brown",tags=block_id_tag)
         else: canvas.create_rectangle (x-60, y-80, x+60, y+150, fill = "saddle brown",tags=block_id_tag)
         # Create the button objects and their callbacks
-        occup_button = Button (canvas, text="OCCUP", padx=common.xpadding, pady=common.ypadding,
+        occup_button = Tk.Button (canvas, text="OCCUP", padx=common.xpadding, pady=common.ypadding,
                     state="normal", relief="raised", font=('Courier',common.fontsize,"normal"),
                     bg=common.bgraised, command = lambda:occup_button_event(block_id))
-        clear_button = Button (canvas, text="CLEAR", padx=common.xpadding, pady=common.ypadding,
+        clear_button = Tk.Button (canvas, text="CLEAR", padx=common.xpadding, pady=common.ypadding,
                     state="normal", relief="raised", font=('Courier',common.fontsize,"normal"),
                     bg=common.bgraised, command = lambda:clear_button_event(block_id))
-        block_button = Button (canvas, text="LINE BLOCKED", padx=common.xpadding, pady=common.ypadding,
+        block_button = Tk.Button (canvas, text="LINE BLOCKED", padx=common.xpadding, pady=common.ypadding,
                     state="normal", relief="sunken", font=('Courier',common.fontsize,"normal"),
                     bg=common.bgsunken, command = lambda:blocked_button_event(block_id))
-        bell_button = Button (canvas, text="TELEGRAPH", padx=common.xpadding, pady=common.ypadding,
+        bell_button = Tk.Button (canvas, text="TELEGRAPH", padx=common.xpadding, pady=common.ypadding,
                     state="normal", relief="raised", font=('Courier',common.fontsize,"normal"),
                     bg="black", fg="white", activebackground="black", activeforeground="white",
                     command = lambda:telegraph_key_button(block_id))
         # Bind a right click on the Telegraph button to open the bell code hints
         bell_button.bind('<Button-2>', lambda event:open_bell_code_hints())
         bell_button.bind('<Button-3>', lambda event:open_bell_code_hints())
         # Create the windows (on the canvas) for the buttons
-        canvas.create_window(x, y+80, window=occup_button, anchor=SE, tags=block_id_tag)
-        canvas.create_window(x, y+80, window=clear_button, anchor=SW, tags=block_id_tag)
-        canvas.create_window(x, y+80, window=block_button, anchor=N, tags=block_id_tag)
-        canvas.create_window(x, y+115, window=bell_button, anchor=N, tags=block_id_tag)
+        canvas.create_window(x, y+80, window=occup_button, anchor=Tk.SE, tags=block_id_tag)
+        canvas.create_window(x, y+80, window=clear_button, anchor=Tk.SW, tags=block_id_tag)
+        canvas.create_window(x, y+80, window=block_button, anchor=Tk.N, tags=block_id_tag)
+        canvas.create_window(x, y+115, window=bell_button, anchor=Tk.N, tags=block_id_tag)
         # Create the main block section indicator for our instrument
         my_ind_block, my_ind_clear, my_ind_occup = create_block_indicator (canvas, x, y, block_id_tag)
         # If this is a double line indicator then create the repeater indicator
         if single_line: rep_ind_block, rep_ind_clear, rep_ind_occup = None, None, None
         else: rep_ind_block, rep_ind_clear, rep_ind_occup = create_block_indicator (canvas, x, y-55, block_id_tag)
         # Try to Load the specified audio files for the bell rings and telegraph key if audio is enabled
         # if these fail to load for any reason then no sounds will be produced on these events
         if audio_enabled:
-            try:
-                with importlib.resources.path ('model_railway_signals.library.resources',bell_sound_file) as sound_file:
-                    bell_audio = simpleaudio.WaveObject.from_wave_file(str(sound_file))
-            except:
-                logging.error ("Block Instruments - Error loading bell audio file '"+str(bell_sound_file)+"'")       
-                bell_audio = None
-            try:
-                with importlib.resources.path ('model_railway_signals.library.resources',telegraph_sound_file) as sound_file:
-                    telegraph_audio = simpleaudio.WaveObject.from_wave_file(str(sound_file))
-            except:
-                logging.error ("Block Instruments - Error loading telegraph audio file '"+str(telegraph_sound_file)+"'")
-                telegraph_audio = None
+            bell_audio = load_audio_file(bell_sound_file)
+            telegraph_audio = load_audio_file(telegraph_sound_file)
         else:
             logging.warning ("Block Instruments - Audio is not enabled - To enable: 'python3 -m pip install simpleaudio'")
             bell_audio = None
             telegraph_audio = None
-
         # Create the dictionary of elements that we need to track
         instruments[str(block_id)] = {}
         instruments[str(block_id)]["canvas"] = canvas                         # Tkinter drawing canvas
         instruments[str(block_id)]["extcallback"] = block_callback            # External callback to make
-        instruments[str(block_id)]["linkedto"] = linked_to                    # Id of the instrument this one is linked to
+        instruments[str(block_id)]["linkedto"] = linked_to_id                    # Id of the instrument this one is linked to
         instruments[str(block_id)]["singleline"] = single_line                # Single line (bi-directional) instrument
         instruments[str(block_id)]["sectionstate"] = None                     # State of this instrument (None = "BLOCKED")
         instruments[str(block_id)]["repeaterstate"] = None                    # State of repeater display (None = "BLOCKED")
         instruments[str(block_id)]["blockbutton"] = block_button              # Tkinter Button object
         instruments[str(block_id)]["clearbutton"] = clear_button              # Tkinter Button object
         instruments[str(block_id)]["occupbutton"] = occup_button              # Tkinter Button object
         instruments[str(block_id)]["bellbutton"] = bell_button                # Tkinter Button object
@@ -567,16 +619,16 @@
             if loaded_state["repeaterstate"] == True: set_repeater_clear(block_id,make_callback=False)
             elif loaded_state["repeaterstate"] == False: set_repeater_occupied(block_id,make_callback=False)
             else: set_repeater_blocked(block_id,make_callback=False)
         # If the associated block instrument is associated with an external node (i.e. has a string-type
         # compound identifier rather than an integer) then subscribe to updates from the remote node and
         # publish the initial state of the local instrument (to be picked up by the remote node). State
         # will only be published if the MQTT interface has been configured and we are connected to the broker
-        if isinstance(linked_to,str):
-            subscribe_to_remote_instrument(linked_to)
+        if isinstance(linked_to_id,str):
+            subscribe_to_remote_instrument(linked_to_id)
             send_mqtt_instrument_updated_event(block_id)
     return ()
 
 # --------------------------------------------------------------------------------
 # Public API function to find out if the block section ahead is clear.
 # This is represented by the current status of the REPEATER Indicator
 # --------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/common.py` & `model-railway-signals-3.3.0/model_railway_signals/library/common.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/dcc_control.py` & `model-railway-signals-3.3.0/model_railway_signals/library/dcc_control.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/file_interface.py` & `model-railway-signals-3.3.0/model_railway_signals/library/file_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,18 +112,19 @@
         # In both cases we check to make sure the file exists on disk before providing as an option
         if load_file_dialog:
             if file_name is not None: default_file_to_load = file_name
             else: default_file_to_load = default_file_name
             if os.path.isfile (default_file_to_load):
                 filename = tkinter.filedialog.askopenfilename(title='Load Layout State',
                                     filetypes=(('sig files','*.sig'),('all files','*.*')),
-                                    initialfile = default_file_to_load )
+                                    initialdir = '.', initialfile = default_file_to_load )
             else:
                 filename = tkinter.filedialog.askopenfilename(title='Load Layout State',
-                                    filetypes=(('sig files','*.sig'),('all files','*.*')) )
+                                    filetypes=(('sig files','*.sig'),('all files','*.*')),
+                                    initialdir = '.')
             # If dialogue is cancelled then Filename will remain as 'None' as nothing will be loaded
             if filename == () or filename == "": filename = None
         # If the 'load_file_dialog' hasn't been specified but a filename has been provided then we use that
         elif file_name is not None: filename = file_name
         # Fall back to a filename derived from the name of the main python script (with a '.sig' extension)
         else: filename = default_file_name
         # if the user clicks on 'Cancel' in the load file dialog then we still want to provide an option
@@ -139,22 +140,26 @@
             try:
                 with open (filename,'r') as file:
                     file_contents=file.read()
                 file.close
             except Exception as exception:
                 logging.error("Load File - Error opening file - Layout will be created in its default state")
                 logging.error("Load File - Reported Exception: "+str(exception))
+                tkinter.messagebox.showerror(title="File Load Error",message=str(exception))
+                filename = None
             else:
                 # The file has been successfuly opened and loaded - Now convert it from the json format back
                 # into the dictionary of signals, points and sections - with exception handling in case it fails
                 try:
                     layout_state = json.loads(file_contents)
                 except Exception as exception:
                     logging.error("Load File - Couldn't read file - Layout will be created in its default state")
                     logging.error("Load File - Reported exception: "+str(exception))
+                    tkinter.messagebox.showerror(title="File Parse Error",message=str(exception))
+                    filename = None
             # Store the filename that was loaded - to use on application quit
             filename_used_for_load = filename
     return(filename)
 
 #-------------------------------------------------------------------------------------------------
 # Function called on application quit to save the current layout state to file. The actual options 
 # presented to the user will depend on the 'save_as_option_enabled' and 'filename' global variables
@@ -257,14 +262,16 @@
             file_contents = json.dumps(dictionary_to_save,indent=4,sort_keys=True)
             try:
                 with open (filename_used_for_save,'w') as file:
                     file.write(file_contents)
                 file.close
             except Exception as exception:
                 logging.error("Save File - Error saving file - Reported exception: "+str(exception))
+                tkinter.messagebox.showerror(title="File Save Error",message=str(exception))
+                quit_application = False
     return (quit_application)
 
 #-------------------------------------------------------------------------------------------------
 # Function called on creation of a signal/point/section/instrument Object to return the initial state
 # from the loaded data. If no layout state has been loaded or the loaded data doesn't include an
 # entry for the Object then we return 'None' and the Object will retain its "as created" default state
 #-------------------------------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/mqtt_interface.py` & `model-railway-signals-3.3.0/model_railway_signals/library/mqtt_interface.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/pi_sprog_interface.py` & `model-railway-signals-3.3.0/model_railway_signals/library/pi_sprog_interface.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/points.py` & `model-railway-signals-3.3.0/model_railway_signals/library/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 #
 #---------------------------------------------------------------------------------------------------
 
 from . import dcc_control
 from . import common
 from . import file_interface
 
-from tkinter import *
+import tkinter as Tk
 import enum
 import logging
 
 # -------------------------------------------------------------------------
 # Classes used by external functions when calling the create_point function
 # -------------------------------------------------------------------------
 
@@ -241,19 +241,19 @@
     elif fpl and auto:
         logging.error ("Point "+str(point_id)+": Automatic point should be created without a facing point lock")
         point_objects = [0,0,0,0]
     else:
         # Define the "Tag" for all drawing objects for this point instance
         point_id_tag = "point"+str(point_id)
         # Create the button objects and their callbacks
-        point_button = Button (canvas, text=str(point_id), state="normal", relief="raised",
+        point_button = Tk.Button (canvas, text=str(point_id), state="normal", relief="raised",
                     font=('Courier',common.fontsize,"normal"),bg= "grey85",
                     padx=common.xpadding, pady=common.ypadding,
                     command = lambda:change_button_event(point_id))
-        fpl_button = Button (canvas,text="L",state="normal", relief="sunken",
+        fpl_button = Tk.Button (canvas,text="L",state="normal", relief="sunken",
                     font=('Courier',common.fontsize,"normal"), bg = "white",
                     padx=common.xpadding, pady=common.ypadding, 
                     command = lambda:fpl_button_event(point_id))
         # Disable the change button if the point has FPL(default state = FPL active)
         if fpl: point_button.config(state="disabled")
 
         if pointtype==point_type.RH:
@@ -271,16 +271,16 @@
                 # point is completely automatic - both buttons are "hidden"
                 point_coords = common.rotate_point (x,y,-10,-20,orientation)
                 canvas.create_window (point_coords,window=point_button,state='hidden',tags=point_id_tag) 
                 canvas.create_window (point_coords,window=fpl_button,state='hidden',tags=point_id_tag)
             elif fpl:
                 # If the point has FPL then both the change and fpl buttons are displayed
                 point_coords = common.rotate_point (x,y,-10,-20,orientation)
-                canvas.create_window (point_coords,anchor=W,window=point_button,tags=point_id_tag) 
-                canvas.create_window (point_coords,anchor=E,window=fpl_button,tags=point_id_tag)
+                canvas.create_window (point_coords,anchor=Tk.W,window=point_button,tags=point_id_tag) 
+                canvas.create_window (point_coords,anchor=Tk.E,window=fpl_button,tags=point_id_tag)
             else:
                 # Point has no FPL so the FPL button is "hidden"
                 point_coords = common.rotate_point (x,y,-10,-20,orientation)
                 canvas.create_window (point_coords,window=point_button,tags=point_id_tag) 
                 canvas.create_window (point_coords,window=fpl_button,state='hidden',tags=point_id_tag)
 
         else: 
@@ -298,16 +298,16 @@
                 # point is completely automatic - both buttons are "hidden"
                 point_coords = common.rotate_point (x,y,-10,+20,orientation)
                 canvas.create_window (point_coords,window=point_button,state='hidden',tags=point_id_tag) 
                 canvas.create_window (point_coords,window=fpl_button,state='hidden',tags=point_id_tag)
             elif fpl:
                 # If the point has FPL then both the change and fpl buttons are displayed
                 point_coords = common.rotate_point (x,y,-10,+20,orientation)
-                canvas.create_window (point_coords,anchor=W,window=point_button,tags=point_id_tag) 
-                canvas.create_window (point_coords,anchor=E,window=fpl_button,tags=point_id_tag)
+                canvas.create_window (point_coords,anchor=Tk.W,window=point_button,tags=point_id_tag) 
+                canvas.create_window (point_coords,anchor=Tk.E,window=fpl_button,tags=point_id_tag)
             else:
                 # Point has no FPL so the FPL button is "hidden"
                 point_coords = common.rotate_point (x,y,-10,+20,orientation)
                 canvas.create_window (point_coords,window=point_button,tags=point_id_tag) 
                 canvas.create_window (point_coords,window=fpl_button,state='hidden',tags=point_id_tag)
                 
         # The "normal" state of the point is the straight through route by default
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-01.wav` & `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-01.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-02.wav` & `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-02.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-03.wav` & `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-03.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/resources/bell-ring-04.wav` & `model-railway-signals-3.3.0/model_railway_signals/library/resources/bell-ring-04.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/resources/telegraph-key-01.wav` & `model-railway-signals-3.3.0/model_railway_signals/library/resources/telegraph-key-01.wav`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/signals.py` & `model-railway-signals-3.3.0/model_railway_signals/library/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,21 +318,18 @@
 #   Mandatory Parameters:
 #       *sig_ids:int - The signals to publish (multiple Signal_IDs can be specified)
 #
 # ------------------------------------------------------------------------------------------
    
 from . import signals_common
 from . import signals_colour_lights
-from . import signals_ground_position
-from . import signals_ground_disc
 from . import signals_semaphores
 from . import mqtt_interface
 
 from typing import Union
-from tkinter import *
 import logging
 
 # -------------------------------------------------------------------------
 # Externally called function to Return the current SWITCHED state of the signal
 # (i.e. the state of the signal button - Used to enable interlocking functions)
 # Note that the DISPLAYED state of the signal may not be CLEAR if the signal is
 # overridden or subject to release on RED - See "signal_displaying_clear"
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/signals_colour_lights.py` & `model-railway-signals-3.3.0/model_railway_signals/library/signals_colour_lights.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from . import common
 from . import signals_common
 from . import dcc_control
 from . import file_interface
 
 from typing import Union
-from tkinter import *
 import logging
 import enum
 
 # -------------------------------------------------------------------------
 # Classes used externally when creating/updating colour light signals 
 # -------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/signals_common.py` & `model-railway-signals-3.3.0/model_railway_signals/library/signals_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from . import dcc_control
 from . import mqtt_interface
 from . import signals_colour_lights
 from . import signals_semaphores
 from . import signals_ground_position
 from . import signals_ground_disc
 
-from tkinter import *
 from typing import Union
+import tkinter as Tk
 import logging
 import enum
 
 # -------------------------------------------------------------------------
 # Global Classes to be used externally when creating/updating signals or 
 # processing button change events - Will apply to more that one signal type
 # -------------------------------------------------------------------------
@@ -409,22 +409,22 @@
     # special case of a semaphore distant signal being created on the same "post" as a semaphore
     # home signal. On this case we label the button as "D" to differentiate it from the main
     # home signal button and then apply the offset to deconflict with the home signal buttons
     if distant_button_offset !=0 : main_button_text = "D"
     elif sig_id < 10: main_button_text = "0" + str(sig_id)
     else: main_button_text = str(sig_id)
     # Create the Signal and Subsidary Button objects and their callbacks
-    sig_button = Button (canvas, text=main_button_text, padx=common.xpadding, pady=common.ypadding,
+    sig_button = Tk.Button (canvas, text=main_button_text, padx=common.xpadding, pady=common.ypadding,
                 state="normal", relief="raised", font=('Courier',common.fontsize,"normal"),
                 bg=common.bgraised, command=lambda:signal_button_event(sig_id))
-    sub_button = Button (canvas, text="S", padx=common.xpadding, pady=common.ypadding,
+    sub_button = Tk.Button (canvas, text="S", padx=common.xpadding, pady=common.ypadding,
                 state="normal", relief="raised", font=('Courier',common.fontsize,"normal"),
                 bg=common.bgraised, command=lambda:subsidary_button_event(sig_id))
     # Signal Passed Button - We only want a small button - hence a small font size
-    passed_button = Button (canvas,text="O",padx=1,pady=1,font=('Courier',2,"normal"),
+    passed_button = Tk.Button (canvas,text="O",padx=1,pady=1,font=('Courier',2,"normal"),
                 command=lambda:sig_passed_button_event(sig_id))
     # Create the 'windows' in which the buttons are displayed. The Subsidary Button is "hidden"
     # if the signal doesn't have an associated subsidary. The Button positions are adjusted
     # accordingly so they always remain in the "right" position relative to the signal
     # Note that we have to cater for the special case of a semaphore distant signal being
     # created on the same post as a semaphore home signal. In this case (signified by a
     # distant_button_offset), we apply the offset to deconflict with the home signal buttons.
@@ -432,16 +432,16 @@
         button_position = common.rotate_point (x,y,distant_button_offset,-25,orientation)
         if not automatic: canvas.create_window(button_position,window=sig_button,tags=tag)
         else: canvas.create_window(button_position,window=sig_button,state='hidden',tags=tag)
         canvas.create_window(button_position,window=sub_button,state='hidden',tags=tag)
     elif subsidary:
         if orientation == 0: button_position = common.rotate_point (x,y,-25,-25,orientation) 
         else: button_position = common.rotate_point (x,y,-35,-25,orientation) 
-        canvas.create_window(button_position,anchor=E,window=sig_button,tags=tag)
-        canvas.create_window(button_position,anchor=W,window=sub_button,tags=tag)          
+        canvas.create_window(button_position,anchor=Tk.E,window=sig_button,tags=tag)
+        canvas.create_window(button_position,anchor=Tk.W,window=sub_button,tags=tag)          
     else:
         button_position = common.rotate_point (x,y,-20,-25,orientation) 
         canvas.create_window(button_position,window=sig_button,tags=tag)
         canvas.create_window(button_position,window=sub_button,state='hidden',tags=tag)
     # Signal passed button is created on the track at the base of the signal
     if sig_passed_button:
         canvas.create_window(x,y,window=passed_button,tags=tag)
@@ -478,21 +478,21 @@
                                       x:int,y:int,
                                       orientation:int,
                                       approach_button:bool):
     global signals
     # Define the "Tag" for all drawing objects for this signal instance
     tag = "signal"+str(sig_id)
     # Create the approach release button - We only want a small button - hence a small font size
-    approach_release_button = Button(canvas,text="O",padx=1,pady=1,font=('Courier',2,"normal"),
+    approach_release_button = Tk.Button(canvas,text="O",padx=1,pady=1,font=('Courier',2,"normal"),
                                         command=lambda:approach_release_button_event (sig_id))
     button_position = common.rotate_point(x,y,-50,0,orientation)
     if approach_button:
-        window = canvas.create_window(button_position,window=approach_release_button,tags=tag)
+        canvas.create_window(button_position,window=approach_release_button,tags=tag)
     else:
-        window = canvas.create_window(button_position,window=approach_release_button,state="hidden",tags=tag)
+        canvas.create_window(button_position,window=approach_release_button,state="hidden",tags=tag)
     # Add the Theatre elements to the dictionary of signal objects
     signals[str(sig_id)]["released"] = False                          # SHARED - State between 'released' and 'passed' events
     signals[str(sig_id)]["releaseonred"] = False                      # SHARED - State of the "Approach Release for the signal
     signals[str(sig_id)]["releaseonyel"] = False                      # SHARED - State of the "Approach Release for the signal
     signals[str(sig_id)]["releasebutton"] = approach_release_button   # SHARED - Button drawing object
     return()
 
@@ -511,15 +511,15 @@
     tag = "signal"+str(sig_id)
     # Draw the theatre route indicator box only if one is specified for this particular signal
     # The text object is created anyway - but 'hidden' if not required for this particular signal
     text_coordinates = common.rotate_point(x,y,xoff,yoff,orientation)
     tag = "signal"+str(sig_id)
     if has_theatre:
         rectangle_coords = common.rotate_line(x,y,xoff-10,yoff+8,xoff+10,yoff-8,orientation)
-        theatre_object = canvas.create_rectangle(rectangle_coords,fill="black",tags=tag)
+        canvas.create_rectangle(rectangle_coords,fill="black",tags=tag)
         theatre_text = canvas.create_text(text_coordinates,fill="white",text="",angle=orientation-90,state='normal',tags=tag)
     else:
         theatre_text = canvas.create_text(text_coordinates,fill="white",text="",angle=orientation-90,state='hidden',tags=tag)
     # Add the Theatre elements to the dictionary of signal objects
     signals[str(sig_id)]["theatretext"]    = "NONE"              # SHARED - Initial Theatre Text to display (none)
     signals[str(sig_id)]["hastheatre"]     = has_theatre         # SHARED - Whether the signal has a theatre display or not
     signals[str(sig_id)]["theatreobject"]  = theatre_text        # SHARED - Text drawing object
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/signals_ground_disc.py` & `model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_disc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # --------------------------------------------------------------------------------
 
 from . import signals_common
 from . import dcc_control
 from . import file_interface
 from . import common
 
-from tkinter import *
 import logging
 import enum
 
 # -------------------------------------------------------------------------
 # Classes used externally when creating/updating Ground Disk signals 
 # -------------------------------------------------------------------------
 
@@ -46,15 +45,15 @@
         # Draw the signal base
         line_coords = common.rotate_line (x,y,0,0,0,-11,orientation)
         canvas.create_line (line_coords,width=2,tags=sig_id_tag)
         line_coords = common.rotate_line (x,y,0,-11,5,-11,orientation)
         canvas.create_line (line_coords,width=2,tags=sig_id_tag)
         # Draw the White disc of the signal
         oval_coords = common.rotate_line (x,y,+5,-21,+21,-5,orientation)
-        posroot = canvas.create_oval(oval_coords,fill="white",outline="black",tags=sig_id_tag)
+        canvas.create_oval(oval_coords,fill="white",outline="black",tags=sig_id_tag)
         # Draw the banner arms for the signal
         if signal_subtype == ground_disc_sub_type.shunt_ahead: arm_colour="yellow3"
         else: arm_colour = "red"
         line_coords = common.rotate_line(x,y,+13,-21,+13,-5,orientation)
         sigon = canvas.create_line(line_coords,fill=arm_colour,width=3,tags=sig_id_tag)
         line_coords = common.rotate_line(x,y,+18,-19,+8,-7,orientation)
         sigoff = canvas.create_line(line_coords,fill=arm_colour,width=3,tags=sig_id_tag)
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/signals_ground_position.py` & `model-railway-signals-3.3.0/model_railway_signals/library/signals_ground_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # --------------------------------------------------------------------------------
 
 from . import signals_common
 from . import dcc_control
 from . import file_interface
 from . import common
 
-from tkinter import *
 import logging
 import enum
 
 # -------------------------------------------------------------------------
 # Classes used externally when creating/updating Ground Disk signals 
 # -------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/signals_semaphores.py` & `model-railway-signals-3.3.0/model_railway_signals/library/signals_semaphores.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from . import common
 from . import signals_common
 from . import dcc_control
 from . import file_interface
 
 from typing import Union
-from tkinter import *
 import logging
 import enum
 
 # -------------------------------------------------------------------------
 # Classes used externally when creating/updating semaphore signals 
 # -------------------------------------------------------------------------
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/track_sections.py` & `model-railway-signals-3.3.0/model_railway_signals/library/track_sections.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 #       *sec_ids:int - The track sections to publish (multiple Section_IDs can be specified)
 # 
 # --------------------------------------------------------------------------------
 
 from . import common
 from . import mqtt_interface
 from . import file_interface
-from tkinter import *
 from typing import Union
+import tkinter as Tk
 import enum
 import logging
 
 # -------------------------------------------------------------------------
 # Classes used by external functions when using track sections
 # -------------------------------------------------------------------------
     
@@ -202,15 +202,15 @@
     if entry_box_window is not None:
         text_entry_box.destroy()
         canvas.delete(entry_box_window)
     # Set the font size and length for the text entry box
     font_size = common.fontsize
     label_length = sections[str(section_id)]["labellength"]
     # Create the entry box and bind the RETURN and ESCAPE events to it
-    text_entry_box = Entry(canvas,width=label_length,font=('Ariel',font_size,"normal"))
+    text_entry_box = Tk.Entry(canvas,width=label_length,font=('Ariel',font_size,"normal"))
     text_entry_box.bind('<Return>', lambda event:update_identifier(section_id))
     text_entry_box.bind('<Escape>', lambda event:cancel_update(section_id))
     # if the section button is already showing occupied then we EDIT the value
     if sections[str(section_id)]["occupied"]:
         text_entry_box.insert(0,sections[str(section_id)]["labeltext"])
     # Create a window on the canvas for the Entry box (overlaying the section button)
     bbox = sections[str(section_id)]["canvas"].bbox("section"+str(section_id))
@@ -238,15 +238,15 @@
     if section_exists(section_id):
         logging.error ("Section "+str(section_id)+": Section already exists")
     elif section_id < 1:
         logging.error ("Section "+str(section_id)+": Section ID must be greater than zero")
     else:
         # Create the button objects and their callbacks
         font_size = common.fontsize
-        section_button = Button (canvas, text=label, state="normal", relief="raised",
+        section_button = Tk.Button (canvas, text=label, state="normal", relief="raised",
                     padx=common.xpadding, pady=common.ypadding, font=('Ariel',font_size,"normal"),
                     bg="grey", fg="grey40", activebackground="grey", activeforeground="grey40",
                     command = lambda:section_button_event(section_id), width = len(label))
         # Note the "Tag" for the drawing objects for this track section (i.e. this window)
         canvas.create_window (x,y,window=section_button,tags="section"+str(section_id))
         # Compile a dictionary of everything we need to track
         sections[str(section_id)] = {"canvas" : canvas,                   # canvas object
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals/library/track_sensors.py` & `model-railway-signals-3.3.0/model_railway_signals/library/track_sensors.py`

 * *Files identical despite different names*

### Comparing `model-railway-signals-3.2.0/model_railway_signals.egg-info/PKG-INFO` & `model-railway-signals-3.3.0/model_railway_signals.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-railway-signals
-Version: 3.2.0
+Version: 3.3.0
 Summary: Create your own DCC model railway signalling scheme
 Home-page: https://github.com/johnrm174/model-railway-signalling
 Author: johnrm174
 Author-email: johnrm17418@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 2, June 1991
 Description: # model-railway-signalling
         
@@ -16,24 +16,25 @@
         
         ## Layout editor
         
         From Release 3.0.0, the schematic editor application enables automated and interlocked layout signalling 
         schemes to be designed and configured without the need to write any code. Note that the editor is in
         active development so any comments and suggestions for future features are welcome.
         
-        What's supported in Release 3.2.0:
+        What's supported in Release 3.3.0:
         * Draw your layout schematic with lines, points, signals and track occupancy sections
         * Define the DCC command sequences to drive the signals and points out on the layout
         * Configure the signals and points to implement protototypical interlocking schemes
         * Configure GPIO sensors and track sections to provide a 'mimic' display of the layout
         * Automation of signals as trains traverse the routes that have been configured
         * Save and load your layout schematic and state between running sessions
+        * Block instruments - with interlocking of starting signals
+        * Popup error messages when things go wrong (reduced reliance on logs)
         
         What's coming soon:
-        * Support for block section instruments
         * MQTT networking (for linking layouts)
         * Application documentation
         
         Any bug reports and feedback you may have would be gratefully appreciated - specifically:
         * What aspects are intuitive? What aspects aren't?
         * What aspects do you particularly like?
         * What aspects particularly irritate you?
```

### Comparing `model-railway-signals-3.2.0/model_railway_signals.egg-info/SOURCES.txt` & `model-railway-signals-3.3.0/model_railway_signals.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 model_railway_signals.egg-info/PKG-INFO
 model_railway_signals.egg-info/SOURCES.txt
 model_railway_signals.egg-info/dependency_links.txt
 model_railway_signals.egg-info/requires.txt
 model_railway_signals.egg-info/top_level.txt
 model_railway_signals/editor/__init__.py
 model_railway_signals/editor/common.py
+model_railway_signals/editor/configure_instrument.py
 model_railway_signals/editor/configure_point.py
 model_railway_signals/editor/configure_section.py
 model_railway_signals/editor/configure_signal.py
 model_railway_signals/editor/configure_signal_tab1.py
 model_railway_signals/editor/configure_signal_tab2.py
 model_railway_signals/editor/configure_signal_tab3.py
 model_railway_signals/editor/editor.py
-model_railway_signals/editor/menubar.py
+model_railway_signals/editor/menubar_windows.py
 model_railway_signals/editor/run_layout.py
 model_railway_signals/editor/schematic.py
 model_railway_signals/editor/settings.py
 model_railway_signals/editor/objects/__init__.py
 model_railway_signals/editor/objects/objects.py
 model_railway_signals/editor/objects/objects_common.py
 model_railway_signals/editor/objects/objects_instruments.py
```

### Comparing `model-railway-signals-3.2.0/setup.py` & `model-railway-signals-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="model-railway-signals",
-    version="3.2.0",
+    version="3.3.0",
     packages=find_packages(),
     include_package_data=True,
     description="Create your own DCC model railway signalling scheme",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/johnrm174/model-railway-signalling",
     author="johnrm174",
```

