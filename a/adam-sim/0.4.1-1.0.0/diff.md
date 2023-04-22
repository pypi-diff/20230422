# Comparing `tmp/adam_sim-0.4.1.tar.gz` & `tmp/adam_sim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_sim-0.4.1.tar", last modified: Mon Mar 27 15:21:39 2023, max compression
+gzip compressed data, was "adam_sim-1.0.0.tar", last modified: Sat Apr 22 21:29:04 2023, max compression
```

## Comparing `adam_sim-0.4.1.tar` & `adam_sim-1.0.0.tar`

### file list

```diff
@@ -1,102 +1,173 @@
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1063 2023-02-09 11:58:56.000000 adam_sim-0.4.1/LICENSE
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2994 2023-03-27 15:21:39.169432 adam_sim-0.4.1/PKG-INFO
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2349 2023-03-22 15:06:35.000000 adam_sim-0.4.1/README.md
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.157432 adam_sim-0.4.1/adam/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      144 2023-03-14 16:29:33.000000 adam_sim-0.4.1/adam/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.157432 adam_sim-0.4.1/adam/assets/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    21447 2023-03-27 15:13:11.000000 adam_sim-0.4.1/adam/assets/adam.xml
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/assets/meshes/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   306784 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/base.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    64184 2023-02-01 11:08:16.000000 adam_sim-0.4.1/adam/assets/meshes/body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     6084 2023-03-27 14:59:36.000000 adam_sim-0.4.1/adam/assets/meshes/body1.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1484 2023-03-27 15:04:53.000000 adam_sim-0.4.1/adam/assets/meshes/body2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     6284 2023-03-27 15:04:53.000000 adam_sim-0.4.1/adam/assets/meshes/body3.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    48684 2023-03-27 15:04:53.000000 adam_sim-0.4.1/adam/assets/meshes/body4.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   234684 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/end_effector_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/end_effector_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   514984 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/forearm_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   983584 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/forearm_body_2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1147584 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/forearm_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   307884 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/forearm_link_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/forearm_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/forearm_rubber_2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/shoulder_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/shoulder_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/shoulder_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/shoulder_screws.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   461284 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_link_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_rubber_2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_rubber_3.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/upperarm_screws.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_1_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_1_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_1_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_2_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_2_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_2_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_3_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_3_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-02-03 07:39:46.000000 adam_sim-0.4.1/adam/assets/meshes/wrist_3_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      917 2023-03-22 17:34:13.000000 adam_sim-0.4.1/adam/assets/scene.xml
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/core/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)        0 2023-03-14 16:40:26.000000 adam_sim-0.4.1/adam/core/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/core/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       41 2023-02-09 09:47:24.000000 adam_sim-0.4.1/adam/core/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3191 2023-02-27 15:54:43.000000 adam_sim-0.4.1/adam/core/entities/configuration.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      207 2023-03-22 16:10:17.000000 adam_sim-0.4.1/adam/entities/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/features/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-03-22 15:06:35.000000 adam_sim-0.4.1/adam/features/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/features/configurations/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       58 2023-02-09 09:27:22.000000 adam_sim-0.4.1/adam/features/configurations/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2038 2023-02-27 16:31:54.000000 adam_sim-0.4.1/adam/features/configurations/configurations_manager.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/features/configurations/data/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    20048 2023-02-09 09:29:48.000000 adam_sim-0.4.1/adam/features/configurations/data/configurations_test.csv
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/features/map_maker/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-02-21 08:15:40.000000 adam_sim-0.4.1/adam/features/map_maker/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.165432 adam_sim-0.4.1/adam/features/map_maker/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      154 2023-02-21 15:35:33.000000 adam_sim-0.4.1/adam/features/map_maker/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     4509 2023-02-27 16:26:44.000000 adam_sim-0.4.1/adam/features/map_maker/entities/body.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1017 2023-02-27 16:27:40.000000 adam_sim-0.4.1/adam/features/map_maker/entities/box.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1106 2023-02-27 16:28:00.000000 adam_sim-0.4.1/adam/features/map_maker/entities/capsule.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      946 2023-02-27 16:28:12.000000 adam_sim-0.4.1/adam/features/map_maker/entities/cube.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1094 2023-02-27 16:28:22.000000 adam_sim-0.4.1/adam/features/map_maker/entities/cylinder.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      864 2023-02-27 16:28:29.000000 adam_sim-0.4.1/adam/features/map_maker/entities/sphere.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     4017 2023-02-27 16:11:42.000000 adam_sim-0.4.1/adam/features/map_maker/map_maker.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/adam/features/map_maker/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       34 2023-02-21 09:28:59.000000 adam_sim-0.4.1/adam/features/map_maker/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      946 2023-02-21 11:24:29.000000 adam_sim-0.4.1/adam/features/map_maker/use_cases/xml_parser.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/adam/features/simulation/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       35 2023-02-09 09:52:13.000000 adam_sim-0.4.1/adam/features/simulation/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/adam/features/simulation/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      266 2023-03-27 14:17:36.000000 adam_sim-0.4.1/adam/features/simulation/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      691 2023-03-27 14:21:32.000000 adam_sim-0.4.1/adam/features/simulation/entities/adam_info.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      460 2023-03-27 14:16:53.000000 adam_sim-0.4.1/adam/features/simulation/entities/base_data.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1691 2023-02-27 15:45:16.000000 adam_sim-0.4.1/adam/features/simulation/entities/collision.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      778 2023-03-27 14:19:08.000000 adam_sim-0.4.1/adam/features/simulation/entities/manipulator_data.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1044 2023-03-27 13:49:50.000000 adam_sim-0.4.1/adam/features/simulation/entities/point.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2351 2023-03-22 16:47:35.000000 adam_sim-0.4.1/adam/features/simulation/entities/system.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1665 2023-03-27 13:47:35.000000 adam_sim-0.4.1/adam/features/simulation/entities/vector.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     7759 2023-03-22 17:27:04.000000 adam_sim-0.4.1/adam/features/simulation/simulation.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/adam/features/simulation/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      200 2023-02-27 12:48:32.000000 adam_sim-0.4.1/adam/features/simulation/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    10168 2023-03-27 15:17:43.000000 adam_sim-0.4.1/adam/features/simulation/use_cases/collision_detector.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3628 2023-03-22 17:17:35.000000 adam_sim-0.4.1/adam/features/simulation/use_cases/control_visualizer.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1063 2023-02-27 15:08:28.000000 adam_sim-0.4.1/adam/features/simulation/use_cases/controller.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3993 2023-03-27 14:23:54.000000 adam_sim-0.4.1/adam/features/simulation/use_cases/data_manager.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1327 2023-03-22 17:18:36.000000 adam_sim-0.4.1/adam/features/simulation/use_cases/viewer.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/adam_sim.egg-info/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2994 2023-03-27 15:21:39.000000 adam_sim-0.4.1/adam_sim.egg-info/PKG-INFO
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3035 2023-03-27 15:21:39.000000 adam_sim-0.4.1/adam_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)        1 2023-03-27 15:21:39.000000 adam_sim-0.4.1/adam_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       59 2023-03-27 15:21:39.000000 adam_sim-0.4.1/adam_sim.egg-info/requires.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)        5 2023-03-27 15:21:39.000000 adam_sim-0.4.1/adam_sim.egg-info/top_level.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      902 2023-03-27 15:20:35.000000 adam_sim-0.4.1/pyproject.toml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-03-27 15:21:39.169432 adam_sim-0.4.1/setup.cfg
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-03-27 15:21:39.169432 adam_sim-0.4.1/tests/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      687 2023-03-22 16:20:45.000000 adam_sim-0.4.1/tests/test_1.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      498 2023-03-22 17:37:14.000000 adam_sim-0.4.1/tests/test_2.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1063 2023-04-12 06:42:52.000000 adam_sim-1.0.0/LICENSE
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3532 2023-04-22 21:29:04.543120 adam_sim-1.0.0/PKG-INFO
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2887 2023-04-14 09:53:02.000000 adam_sim-1.0.0/README.md
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       40 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/core/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      815 2023-04-17 10:50:13.000000 adam_sim-1.0.0/adam_sim/core/topics.yaml
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      353 2023-04-13 11:45:34.000000 adam_sim-1.0.0/adam_sim/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3134 2023-04-13 11:45:06.000000 adam_sim-1.0.0/adam_sim/entities/acceleration.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6411 2023-04-19 11:37:53.000000 adam_sim-1.0.0/adam_sim/entities/configuration.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3065 2023-04-19 07:31:45.000000 adam_sim-1.0.0/adam_sim/entities/point.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2351 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/entities/system.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1665 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/entities/vector.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2782 2023-04-13 11:36:34.000000 adam_sim-1.0.0/adam_sim/entities/velocity.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      121 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       23 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     7765 2023-04-20 13:03:37.000000 adam_sim-1.0.0/adam_sim/features/adam/adam.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       57 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/adam_repository_factory.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       53 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      929 2023-04-20 13:05:27.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       63 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.511122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1225 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      853 2023-04-12 10:53:15.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2491 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      952 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5817 2023-04-12 10:29:53.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5832 2023-04-12 10:30:17.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   306784 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    64184 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6084 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     6284 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    48684 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   234684 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   514984 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   983584 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1147584 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   307884 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   461284 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1043 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      442 2023-04-20 13:08:10.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/simulated_adam_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      703 2023-04-18 10:04:19.000000 adam_sim-1.0.0/adam_sim/features/adam/entities/adam_info.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       44 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-20 13:04:57.000000 adam_sim-1.0.0/adam_sim/features/adam/repository/adam_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       27 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1384 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/use_cases/viewer.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       23 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      427 2023-04-19 09:57:15.000000 adam_sim-1.0.0/adam_sim/features/base/base.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       57 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/base_repository_factory.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       53 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      666 2023-04-20 13:11:50.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       63 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      640 2023-04-20 13:12:00.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      475 2023-04-13 12:23:56.000000 adam_sim-1.0.0/adam_sim/features/base/entities/base_info.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       44 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      403 2023-04-20 13:08:40.000000 adam_sim-1.0.0/adam_sim/features/base/repository/base_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/data_manager/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/data_manager/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/data_manager/data/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)    20048 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/data_manager/data/configurations_test.csv
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5901 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/data_manager/data/end_effector_positions_test.csv
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3330 2023-04-19 07:32:30.000000 adam_sim-1.0.0/adam_sim/features/data_manager/data_manager.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       37 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/communication/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       71 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      328 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       76 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2010 2023-04-20 13:01:18.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       31 2023-04-18 07:57:00.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1947 2023-04-22 11:00:16.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       78 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2011 2023-04-22 10:57:14.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       31 2023-04-22 10:57:33.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1949 2023-04-22 10:59:24.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       86 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3634 2023-04-20 13:00:00.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       48 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     4434 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       88 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3643 2023-04-20 13:00:17.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       48 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     4439 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      667 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/manipulator_repository_factory.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/entities/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       79 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/entities/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1698 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/entities/collision.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1008 2023-04-13 11:47:19.000000 adam_sim-1.0.0/adam_sim/features/manipulator/entities/manipulator_info.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     2528 2023-04-19 09:56:54.000000 adam_sim-1.0.0/adam_sim/features/manipulator/manipulator.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/repository/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       58 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/repository/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1103 2023-04-20 12:59:27.000000 adam_sim-1.0.0/adam_sim/features/manipulator/repository/manipulator_repository.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       73 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3761 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/control_visualizer.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     5109 2023-04-12 10:03:03.000000 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/farm.py
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim.egg-info/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     3532 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/PKG-INFO
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     9827 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/SOURCES.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)        1 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/dependency_links.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       75 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/requires.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)        9 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/top_level.txt
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      921 2023-04-22 21:28:41.000000 adam_sim-1.0.0/pyproject.toml
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-04-22 21:29:04.543120 adam_sim-1.0.0/setup.cfg
+drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/tests/
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      743 2023-04-13 10:35:02.000000 adam_sim-1.0.0/tests/test_basic_usage.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1541 2023-04-13 11:22:46.000000 adam_sim-1.0.0/tests/test_collisions.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      494 2023-04-19 11:02:01.000000 adam_sim-1.0.0/tests/test_configuration.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      344 2023-04-13 10:42:23.000000 adam_sim-1.0.0/tests/test_control.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)     1021 2023-04-19 08:23:30.000000 adam_sim-1.0.0/tests/test_data_manager.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-13 11:20:44.000000 adam_sim-1.0.0/tests/test_export_scene.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      752 2023-04-13 11:07:55.000000 adam_sim-1.0.0/tests/test_farm.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      604 2023-04-20 14:31:17.000000 adam_sim-1.0.0/tests/test_real_communication.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      854 2023-04-13 11:59:15.000000 adam_sim-1.0.0/tests/test_returning_info.py
+-rw-rw-r--   0 vistor    (1000) vistor    (1000)      533 2023-04-13 12:17:49.000000 adam_sim-1.0.0/tests/test_velocity.py
```

### Comparing `adam_sim-0.4.1/LICENSE` & `adam_sim-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/PKG-INFO` & `adam_sim-1.0.0/adam_sim.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6164 616d  : 2.1.Name: adam
-00000020: 5f73 696d 0a56 6572 7369 6f6e 3a20 302e  _sim.Version: 0.
-00000030: 342e 310a 5375 6d6d 6172 793a 2041 2073  4.1.Summary: A s
+00000020: 2d73 696d 0a56 6572 7369 6f6e 3a20 312e  -sim.Version: 1.
+00000030: 302e 300a 5375 6d6d 6172 793a 2041 2073  0.0.Summary: A s
 00000040: 696d 756c 6174 6f72 206f 6620 4144 414d  imulator of ADAM
 00000050: 2028 4175 746f 6e6f 6d6f 7573 2044 6f6d   (Autonomous Dom
 00000060: 6573 7469 6320 416d 6269 6465 7874 726f  estic Ambidextro
 00000070: 7573 204d 616e 6970 756c 6174 6f72 292c  us Manipulator),
 00000080: 2061 206d 6f62 696c 6520 726f 626f 7420   a mobile robot 
 00000090: 6d61 6e69 7075 6c61 746f 7220 636f 6e73  manipulator cons
 000000a0: 6973 7469 6e67 206f 6620 6120 6261 7365  isting of a base
@@ -34,155 +34,188 @@
 00000210: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
 00000220: 5320 496e 6465 7065 6e64 656e 740a 5265  S Independent.Re
 00000230: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
 00000240: 3d33 2e31 300a 4465 7363 7269 7074 696f  =3.10.Descriptio
 00000250: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
 00000260: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
 00000270: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000280: 4e53 450a 0a23 2041 4441 4d20 7369 6d75  NSE..# ADAM simu
-00000290: 6c61 746f 720a 0a5b 215b 7079 7069 2076  lator..[![pypi v
-000002a0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000002b0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000002c0: 7970 692f 762f 6164 616d 2d73 696d 3f6c  ypi/v/adam-sim?l
-000002d0: 6f67 6f3d 7079 7069 295d 2868 7474 7073  ogo=pypi)](https
-000002e0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-000002f0: 6563 742f 6164 616d 2d73 696d 2f29 0a5b  ect/adam-sim/).[
-00000300: 215b 4d49 5420 4c69 6365 6e73 655d 2868  ![MIT License](h
-00000310: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000320: 6473 2e69 6f2f 6261 6467 652f 6c69 6365  ds.io/badge/lice
-00000330: 6e73 652d 4d49 542d 626c 7565 2e73 7667  nse-MIT-blue.svg
-00000340: 3f73 7479 6c65 3d66 6c61 7429 5d28 6874  ?style=flat)](ht
-00000350: 7470 3a2f 2f63 686f 6f73 6561 6c69 6365  tp://choosealice
-00000360: 6e73 652e 636f 6d2f 6c69 6365 6e73 6573  nse.com/licenses
-00000370: 2f6d 6974 2f29 0a5b 215b 646f 6373 5d28  /mit/).[![docs](
-00000380: 6874 7470 733a 2f2f 6261 6467 656e 2e6e  https://badgen.n
-00000390: 6574 2f62 6164 6765 2f72 6561 6474 6865  et/badge/readthe
-000003a0: 646f 6373 2f64 6f63 756d 656e 7461 7469  docs/documentati
-000003b0: 6f6e 2f62 6c75 6529 5d28 6874 7470 733a  on/blue)](https:
-000003c0: 2f2f 6164 616d 2d73 696d 756c 6174 6f72  //adam-simulator
-000003d0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000003e0: 656e 2f6c 6174 6573 742f 290a 0a41 4441  en/latest/)..ADA
-000003f0: 4d20 2841 7574 6f6e 6f6d 6f75 7320 446f  M (Autonomous Do
-00000400: 6d65 7374 6963 2041 6d62 6964 6578 7472  mestic Ambidextr
-00000410: 6f75 7320 4d61 6e69 7075 6c61 746f 7229  ous Manipulator)
-00000420: 2069 7320 6120 6d6f 6269 6c65 2072 6f62   is a mobile rob
-00000430: 6f74 206d 616e 6970 756c 6174 6f72 2063  ot manipulator c
-00000440: 6f6e 7369 7374 696e 6720 6f66 2061 2062  onsisting of a b
-00000450: 6173 6520 7769 7468 2074 776f 2044 6567  ase with two Deg
-00000460: 7265 6573 206f 6620 4672 6565 646f 6d20  rees of Freedom 
-00000470: 2844 6f46 2920 616e 6420 7477 6f20 556e  (DoF) and two Un
-00000480: 6976 6572 7361 6c20 526f 626f 7473 2055  iversal Robots U
-00000490: 5233 206f 6620 3620 446f 4620 6561 6368  R3 of 6 DoF each
-000004a0: 2e0a 0a54 6865 2073 696d 756c 6174 696f  ...The simulatio
-000004b0: 6e20 7761 7320 6275 696c 7420 7573 696e  n was built usin
-000004c0: 6720 5b4d 754a 6f43 6f5d 2868 7474 7073  g [MuJoCo](https
-000004d0: 3a2f 2f6d 756a 6f63 6f2e 6f72 672f 292c  ://mujoco.org/),
-000004e0: 2061 2066 7265 6520 616e 6420 6f70 656e   a free and open
-000004f0: 2073 6f75 7263 6520 7068 7973 6963 7320   source physics 
-00000500: 656e 6769 6e65 2064 6573 6967 6e65 6420  engine designed 
-00000510: 6672 6f6d 2074 6865 2067 726f 756e 6420  from the ground 
-00000520: 7570 2066 6f72 2074 6865 2070 7572 706f  up for the purpo
-00000530: 7365 206f 6620 6d6f 6465 6c2d 6261 7365  se of model-base
-00000540: 6420 6f70 7469 6d69 7a61 7469 6f6e 2c20  d optimization, 
-00000550: 616e 6420 696e 2070 6172 7469 6375 6c61  and in particula
-00000560: 7220 6f70 7469 6d69 7a61 7469 6f6e 2074  r optimization t
-00000570: 6872 6f75 6768 2063 6f6e 7461 6374 732e  hrough contacts.
-00000580: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
-00000590: 6e0a 0a46 6f6c 6c6f 7720 7468 6520 6e65  n..Follow the ne
-000005a0: 7874 2073 7465 7073 2066 6f72 2069 6e73  xt steps for ins
-000005b0: 7461 6c6c 696e 6720 7468 6520 7369 6d75  talling the simu
-000005c0: 6c61 7469 6f6e 206f 6e20 796f 7572 2064  lation on your d
-000005d0: 6576 6963 652e 0a0a 2a2a 5265 7175 6965  evice...**Requie
-000005e0: 7265 6d65 6e74 733a 2a2a 0a2d 2050 7974  rements:**.- Pyt
-000005f0: 686f 6e20 332e 3130 2e30 206f 7220 6869  hon 3.10.0 or hi
-00000600: 6768 6572 0a0a 3e20 2a2a 4e6f 7465 2a2a  gher..> **Note**
-00000610: 3a20 5468 6520 4164 616d 2053 696d 756c  : The Adam Simul
-00000620: 6174 6f72 2077 6f72 6b73 206f 6e20 4c69  ator works on Li
-00000630: 6e75 782c 2057 696e 646f 7773 2061 6e64  nux, Windows and
-00000640: 204d 6163 2e0a 0a23 2323 2049 6e73 7461   Mac...### Insta
-00000650: 6c6c 206d 696e 6963 6f6e 6461 2028 6869  ll miniconda (hi
-00000660: 6768 6c79 2d72 6563 6f6d 6d65 6e64 6564  ghly-recommended
-00000670: 290a 4974 2069 7320 6869 6768 6c79 2072  ).It is highly r
-00000680: 6563 6f6d 6d65 6e64 6564 2074 6f20 696e  ecommended to in
-00000690: 7374 616c 6c20 616c 6c20 7468 6520 6465  stall all the de
-000006a0: 7065 6e64 656e 6369 6573 206f 6e20 6120  pendencies on a 
-000006b0: 6e65 7720 7669 7274 7561 6c20 656e 7669  new virtual envi
-000006c0: 726f 6e6d 656e 742e 2046 6f72 206d 6f72  ronment. For mor
-000006d0: 6520 696e 666f 726d 6174 696f 6e20 6368  e information ch
-000006e0: 6563 6b20 7468 6520 636f 6e64 6120 646f  eck the conda do
-000006f0: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
-00000700: 5b69 6e73 7461 6c6c 6174 696f 6e5d 2868  [installation](h
-00000710: 7474 7073 3a2f 2f63 6f6e 6461 2e69 6f2f  ttps://conda.io/
-00000720: 7072 6f6a 6563 7473 2f63 6f6e 6461 2f65  projects/conda/e
-00000730: 6e2f 6c61 7465 7374 2f75 7365 722d 6775  n/latest/user-gu
-00000740: 6964 652f 696e 7374 616c 6c2f 696e 6465  ide/install/inde
-00000750: 782e 6874 6d6c 2920 616e 6420 5b65 6e76  x.html) and [env
-00000760: 6972 6f6e 6d65 6e74 206d 616e 6167 656d  ironment managem
-00000770: 656e 745d 2868 7474 7073 3a2f 2f63 6f6e  ent](https://con
-00000780: 6461 2e69 6f2f 7072 6f6a 6563 7473 2f63  da.io/projects/c
-00000790: 6f6e 6461 2f65 6e2f 6c61 7465 7374 2f75  onda/en/latest/u
-000007a0: 7365 722d 6775 6964 652f 7461 736b 732f  ser-guide/tasks/
-000007b0: 6d61 6e61 6765 2d65 6e76 6972 6f6e 6d65  manage-environme
-000007c0: 6e74 732e 6874 6d6c 292e 2046 6f72 2063  nts.html). For c
-000007d0: 7265 6174 696e 6720 7468 6520 656e 7669  reating the envi
-000007e0: 726f 6e6d 656e 7420 7573 6520 7468 6520  ronment use the 
-000007f0: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00000800: 6473 206f 6e20 7468 6520 7465 726d 696e  ds on the termin
-00000810: 616c 2e0a 0a60 6060 6261 7368 0a63 6f6e  al...```bash.con
-00000820: 6461 2063 7265 6174 6520 2d6e 2061 6461  da create -n ada
-00000830: 6d20 7079 7468 6f6e 3d3d 332e 3130 2e39  m python==3.10.9
-00000840: 0a63 6f6e 6461 2061 6374 6976 6174 6520  .conda activate 
-00000850: 6164 616d 0a60 6060 0a23 2323 2049 6e73  adam.```.### Ins
-00000860: 7461 6c6c 2066 726f 6d20 7069 700a 5468  tall from pip.Th
-00000870: 6520 4144 414d 2073 696d 756c 6174 6f72  e ADAM simulator
-00000880: 2069 7320 6176 6169 6c61 626c 6520 6173   is available as
-00000890: 2061 2070 6970 2070 6163 6b61 6765 2e20   a pip package. 
-000008a0: 466f 7220 696e 7374 616c 6c69 6e67 2069  For installing i
-000008b0: 7420 6a75 7374 2075 7365 3a0a 6060 600a  t just use:.```.
-000008c0: 7069 7020 696e 7374 616c 6c20 6164 616d  pip install adam
-000008d0: 2d73 696d 0a60 6060 0a0a 2323 2320 496e  -sim.```..### In
-000008e0: 7374 616c 6c20 6672 6f6d 2073 6f75 7263  stall from sourc
-000008f0: 650a 4669 7273 746c 792c 2063 6c6f 6e65  e.Firstly, clone
-00000900: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-00000910: 696e 2079 6f75 7220 7379 7374 656d 2e0a  in your system..
-00000920: 6060 6062 6173 680a 6769 7420 636c 6f6e  ```bash.git clon
-00000930: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00000940: 2e63 6f6d 2f76 6973 746f 726d 752f 6164  .com/vistormu/ad
-00000950: 616d 5f73 696d 756c 6174 6f72 2e67 6974  am_simulator.git
-00000960: 0a60 6060 0a0a 5468 656e 2c20 656e 7465  .```..Then, ente
-00000970: 7220 7468 6520 6469 7265 6374 6f72 7920  r the directory 
-00000980: 616e 6420 696e 7374 616c 6c20 7468 6520  and install the 
-00000990: 7265 7175 6972 6564 2064 6570 656e 6465  required depende
-000009a0: 6e63 6965 730a 6060 6062 6173 680a 6364  ncies.```bash.cd
-000009b0: 2061 6461 6d5f 7369 6d75 6c61 746f 720a   adam_simulator.
-000009c0: 7069 7020 696e 7374 616c 6c20 2d72 2072  pip install -r r
-000009d0: 6571 7569 7265 6d65 6e74 732e 7478 740a  equirements.txt.
-000009e0: 6060 600a 0a23 2320 446f 6375 6d65 6e74  ```..## Document
-000009f0: 6174 696f 6e0a 5468 6520 6f66 6669 6369  ation.The offici
-00000a00: 616c 2064 6f63 756d 656e 7461 7469 6f6e  al documentation
-00000a10: 206f 6620 7468 6520 7061 636b 6167 6520   of the package 
-00000a20: 6973 2061 7661 696c 6162 6c65 206f 6e20  is available on 
-00000a30: 5b52 6561 6420 7468 6520 446f 6373 5d28  [Read the Docs](
-00000a40: 6874 7470 733a 2f2f 6164 616d 2d73 696d  https://adam-sim
-00000a50: 756c 6174 6f72 2e72 6561 6474 6865 646f  ulator.readthedo
-00000a60: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00000a70: 292e 2048 6572 6520 796f 7520 7769 6c6c  ). Here you will
-00000a80: 2066 696e 6420 7468 6520 5b69 6e73 7461   find the [insta
-00000a90: 6c6c 6174 696f 6e20 696e 7374 7275 6374  llation instruct
-00000aa0: 696f 6e73 5d28 6874 7470 733a 2f2f 6164  ions](https://ad
-00000ab0: 616d 2d73 696d 756c 6174 6f72 2e72 6561  am-simulator.rea
-00000ac0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000ad0: 6174 6573 742f 7372 632f 696e 7374 616c  atest/src/instal
-00000ae0: 6c61 7469 6f6e 2e68 746d 6c29 2c20 7468  lation.html), th
-00000af0: 6520 5b41 5049 2072 6566 6572 656e 6365  e [API reference
-00000b00: 5d28 6874 7470 733a 2f2f 6164 616d 2d73  ](https://adam-s
-00000b10: 696d 756c 6174 6f72 2e72 6561 6474 6865  imulator.readthe
-00000b20: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00000b30: 742f 7372 632f 6170 695f 7265 6665 7265  t/src/api_refere
-00000b40: 6e63 652e 6874 6d6c 2920 616e 6420 736f  nce.html) and so
-00000b50: 6d65 205b 6d69 6e69 6d61 6c20 776f 726b  me [minimal work
-00000b60: 696e 6720 6578 616d 706c 6573 5d28 6874  ing examples](ht
-00000b70: 7470 733a 2f2f 6164 616d 2d73 696d 756c  tps://adam-simul
-00000b80: 6174 6f72 2e72 6561 6474 6865 646f 6373  ator.readthedocs
-00000b90: 2e69 6f2f 656e 2f6c 6174 6573 742f 7372  .io/en/latest/sr
-00000ba0: 632f 6578 616d 706c 6573 2e68 746d 6c29  c/examples.html)
-00000bb0: 2e0a                                     ..
+00000280: 4e53 450a 0a23 2041 4441 4d20 5369 6d75  NSE..# ADAM Simu
+00000290: 6c61 746f 720a 0a3c 7020 616c 6967 6e3d  lator..<p align=
+000002a0: 2263 656e 7465 7222 3e0a 2020 2020 3c61  "center">.    <a
+000002b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000002c0: 6974 6875 622e 636f 6d2f 7669 7374 6f72  ithub.com/vistor
+000002d0: 6d75 2f61 6461 6d5f 7369 6d75 6c61 746f  mu/adam_simulato
+000002e0: 7222 3e0a 2020 2020 2020 2020 3c69 6d67  r">.        <img
+000002f0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000300: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000310: 656e 742e 636f 6d2f 7669 7374 6f72 6d75  ent.com/vistormu
+00000320: 2f61 6461 6d5f 7369 6d75 6c61 746f 722f  /adam_simulator/
+00000330: 6d61 7374 6572 2f64 6f63 732f 6173 7365  master/docs/asse
+00000340: 7473 2f61 6461 6d2e 706e 6722 3e0a 2020  ts/adam.png">.  
+00000350: 2020 3c2f 613e 0a3c 2f70 3e0a 0a5b 215b    </a>.</p>..[![
+00000360: 7079 7069 2076 6572 7369 6f6e 5d28 6874  pypi version](ht
+00000370: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000380: 732e 696f 2f70 7970 692f 762f 6164 616d  s.io/pypi/v/adam
+00000390: 2d73 696d 3f6c 6f67 6f3d 7079 7069 295d  -sim?logo=pypi)]
+000003a0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000003b0: 672f 7072 6f6a 6563 742f 6164 616d 2d73  g/project/adam-s
+000003c0: 696d 2f29 0a5b 215b 4d49 5420 4c69 6365  im/).[![MIT Lice
+000003d0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+000003e0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000003f0: 652f 6c69 6365 6e73 652d 4d49 542d 626c  e/license-MIT-bl
+00000400: 7565 2e73 7667 3f73 7479 6c65 3d66 6c61  ue.svg?style=fla
+00000410: 7429 5d28 6874 7470 3a2f 2f63 686f 6f73  t)](http://choos
+00000420: 6561 6c69 6365 6e73 652e 636f 6d2f 6c69  ealicense.com/li
+00000430: 6365 6e73 6573 2f6d 6974 2f29 0a5b 215b  censes/mit/).[![
+00000440: 646f 6373 5d28 6874 7470 733a 2f2f 6261  docs](https://ba
+00000450: 6467 656e 2e6e 6574 2f62 6164 6765 2f72  dgen.net/badge/r
+00000460: 6561 6474 6865 646f 6373 2f64 6f63 756d  eadthedocs/docum
+00000470: 656e 7461 7469 6f6e 2f62 6c75 6529 5d28  entation/blue)](
+00000480: 6874 7470 733a 2f2f 6164 616d 2d73 696d  https://adam-sim
+00000490: 756c 6174 6f72 2e72 6561 6474 6865 646f  ulator.readthedo
+000004a0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+000004b0: 290a 0a41 4441 4d20 2841 7574 6f6e 6f6d  )..ADAM (Autonom
+000004c0: 6f75 7320 446f 6d65 7374 6963 2041 6d62  ous Domestic Amb
+000004d0: 6964 6578 7472 6f75 7320 4d61 6e69 7075  idextrous Manipu
+000004e0: 6c61 746f 7229 2069 7320 6120 6d6f 6269  lator) is a mobi
+000004f0: 6c65 2072 6f62 6f74 206d 616e 6970 756c  le robot manipul
+00000500: 6174 6f72 2063 6f6e 7369 7374 696e 6720  ator consisting 
+00000510: 6f66 2061 2062 6173 6520 7769 7468 2074  of a base with t
+00000520: 776f 2044 6567 7265 6573 206f 6620 4672  wo Degrees of Fr
+00000530: 6565 646f 6d20 2844 6f46 2920 616e 6420  eedom (DoF) and 
+00000540: 7477 6f20 556e 6976 6572 7361 6c20 526f  two Universal Ro
+00000550: 626f 7473 2055 5233 206f 6620 3620 446f  bots UR3 of 6 Do
+00000560: 4620 6561 6368 2e0a 0a54 6865 2073 696d  F each...The sim
+00000570: 756c 6174 696f 6e20 7761 7320 6275 696c  ulation was buil
+00000580: 7420 7573 696e 6720 5b4d 754a 6f43 6f5d  t using [MuJoCo]
+00000590: 2868 7474 7073 3a2f 2f6d 756a 6f63 6f2e  (https://mujoco.
+000005a0: 6f72 672f 292c 2061 2066 7265 6520 616e  org/), a free an
+000005b0: 6420 6f70 656e 2073 6f75 7263 6520 7068  d open source ph
+000005c0: 7973 6963 7320 656e 6769 6e65 2064 6573  ysics engine des
+000005d0: 6967 6e65 6420 6672 6f6d 2074 6865 2067  igned from the g
+000005e0: 726f 756e 6420 7570 2066 6f72 2074 6865  round up for the
+000005f0: 2070 7572 706f 7365 206f 6620 6d6f 6465   purpose of mode
+00000600: 6c2d 6261 7365 6420 6f70 7469 6d69 7a61  l-based optimiza
+00000610: 7469 6f6e 2c20 616e 6420 696e 2070 6172  tion, and in par
+00000620: 7469 6375 6c61 7220 6f70 7469 6d69 7a61  ticular optimiza
+00000630: 7469 6f6e 2074 6872 6f75 6768 2063 6f6e  tion through con
+00000640: 7461 6374 732e 0a0a 2323 2049 6e73 7461  tacts...## Insta
+00000650: 6c6c 6174 696f 6e0a 0a46 6f6c 6c6f 7720  llation..Follow 
+00000660: 7468 6520 6e65 7874 2073 7465 7073 2066  the next steps f
+00000670: 6f72 2069 6e73 7461 6c6c 696e 6720 7468  or installing th
+00000680: 6520 7369 6d75 6c61 7469 6f6e 206f 6e20  e simulation on 
+00000690: 796f 7572 2064 6576 6963 652e 0a0a 2a2a  your device...**
+000006a0: 5265 7175 6965 7265 6d65 6e74 733a 2a2a  Requierements:**
+000006b0: 0a2d 2050 7974 686f 6e20 332e 3130 2e30  .- Python 3.10.0
+000006c0: 206f 7220 6869 6768 6572 0a0a 3e20 2a2a   or higher..> **
+000006d0: 4e6f 7465 2a2a 3a20 5468 6520 4164 616d  Note**: The Adam
+000006e0: 2053 696d 756c 6174 6f72 2077 6f72 6b73   Simulator works
+000006f0: 206f 6e20 4c69 6e75 782c 2057 696e 646f   on Linux, Windo
+00000700: 7773 2061 6e64 204d 6163 2e0a 0a23 2323  ws and Mac...###
+00000710: 2049 6e73 7461 6c6c 206d 696e 6963 6f6e   Install minicon
+00000720: 6461 2028 6869 6768 6c79 2d72 6563 6f6d  da (highly-recom
+00000730: 6d65 6e64 6564 290a 4974 2069 7320 6869  mended).It is hi
+00000740: 6768 6c79 2072 6563 6f6d 6d65 6e64 6564  ghly recommended
+00000750: 2074 6f20 696e 7374 616c 6c20 616c 6c20   to install all 
+00000760: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00000770: 206f 6e20 6120 6e65 7720 7669 7274 7561   on a new virtua
+00000780: 6c20 656e 7669 726f 6e6d 656e 742e 2046  l environment. F
+00000790: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+000007a0: 696f 6e20 6368 6563 6b20 7468 6520 636f  ion check the co
+000007b0: 6e64 6120 646f 6375 6d65 6e74 6174 696f  nda documentatio
+000007c0: 6e20 666f 7220 5b69 6e73 7461 6c6c 6174  n for [installat
+000007d0: 696f 6e5d 2868 7474 7073 3a2f 2f63 6f6e  ion](https://con
+000007e0: 6461 2e69 6f2f 7072 6f6a 6563 7473 2f63  da.io/projects/c
+000007f0: 6f6e 6461 2f65 6e2f 6c61 7465 7374 2f75  onda/en/latest/u
+00000800: 7365 722d 6775 6964 652f 696e 7374 616c  ser-guide/instal
+00000810: 6c2f 696e 6465 782e 6874 6d6c 2920 616e  l/index.html) an
+00000820: 6420 5b65 6e76 6972 6f6e 6d65 6e74 206d  d [environment m
+00000830: 616e 6167 656d 656e 745d 2868 7474 7073  anagement](https
+00000840: 3a2f 2f63 6f6e 6461 2e69 6f2f 7072 6f6a  ://conda.io/proj
+00000850: 6563 7473 2f63 6f6e 6461 2f65 6e2f 6c61  ects/conda/en/la
+00000860: 7465 7374 2f75 7365 722d 6775 6964 652f  test/user-guide/
+00000870: 7461 736b 732f 6d61 6e61 6765 2d65 6e76  tasks/manage-env
+00000880: 6972 6f6e 6d65 6e74 732e 6874 6d6c 292e  ironments.html).
+00000890: 2046 6f72 2063 7265 6174 696e 6720 7468   For creating th
+000008a0: 6520 656e 7669 726f 6e6d 656e 7420 7573  e environment us
+000008b0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+000008c0: 636f 6d6d 616e 6473 206f 6e20 7468 6520  commands on the 
+000008d0: 7465 726d 696e 616c 2e0a 0a60 6060 6261  terminal...```ba
+000008e0: 7368 0a63 6f6e 6461 2063 7265 6174 6520  sh.conda create 
+000008f0: 2d6e 2061 6461 6d20 7079 7468 6f6e 3d3d  -n adam python==
+00000900: 332e 3130 2e39 0a63 6f6e 6461 2061 6374  3.10.9.conda act
+00000910: 6976 6174 6520 6164 616d 0a60 6060 0a23  ivate adam.```.#
+00000920: 2323 2049 6e73 7461 6c6c 2066 726f 6d20  ## Install from 
+00000930: 7069 700a 5468 6520 4144 414d 2073 696d  pip.The ADAM sim
+00000940: 756c 6174 6f72 2069 7320 6176 6169 6c61  ulator is availa
+00000950: 626c 6520 6173 2061 2070 6970 2070 6163  ble as a pip pac
+00000960: 6b61 6765 2e20 466f 7220 696e 7374 616c  kage. For instal
+00000970: 6c69 6e67 2069 7420 6a75 7374 2075 7365  ling it just use
+00000980: 3a0a 6060 600a 7069 7020 696e 7374 616c  :.```.pip instal
+00000990: 6c20 6164 616d 2d73 696d 0a60 6060 0a0a  l adam-sim.```..
+000009a0: 2323 2320 496e 7374 616c 6c20 6672 6f6d  ### Install from
+000009b0: 2073 6f75 7263 650a 4669 7273 746c 792c   source.Firstly,
+000009c0: 2063 6c6f 6e65 2074 6865 2072 6570 6f73   clone the repos
+000009d0: 6974 6f72 7920 696e 2079 6f75 7220 7379  itory in your sy
+000009e0: 7374 656d 2e0a 6060 6062 6173 680a 6769  stem..```bash.gi
+000009f0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000a00: 6769 7468 7562 2e63 6f6d 2f76 6973 746f  github.com/visto
+00000a10: 726d 752f 6164 616d 5f73 696d 756c 6174  rmu/adam_simulat
+00000a20: 6f72 2e67 6974 0a60 6060 0a0a 5468 656e  or.git.```..Then
+00000a30: 2c20 656e 7465 7220 7468 6520 6469 7265  , enter the dire
+00000a40: 6374 6f72 7920 616e 6420 696e 7374 616c  ctory and instal
+00000a50: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
+00000a60: 6570 656e 6465 6e63 6965 730a 6060 6062  ependencies.```b
+00000a70: 6173 680a 6364 2061 6461 6d5f 7369 6d75  ash.cd adam_simu
+00000a80: 6c61 746f 720a 7069 7020 696e 7374 616c  lator.pip instal
+00000a90: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+00000aa0: 732e 7478 740a 6060 600a 0a0a 2323 2320  s.txt.```...### 
+00000ab0: 496e 7374 616c 6c61 7469 6f6e 2066 6f72  Installation for
+00000ac0: 2074 6865 2063 6f6d 6d75 6e69 6361 7469   the communicati
+00000ad0: 6f6e 0a54 6865 2063 6f6d 6d75 6e69 6361  on.The communica
+00000ae0: 7469 6f6e 2075 7365 7320 6d6f 7371 7569  tion uses mosqui
+00000af0: 7474 6f20 6173 2061 2062 726f 6b65 722e  tto as a broker.
+00000b00: 2046 6f72 2069 6e73 7461 6c6c 696e 6720   For installing 
+00000b10: 6974 206f 6e20 796f 7572 2073 7973 7465  it on your syste
+00000b20: 6d2c 2066 6f6c 6c6f 7720 7468 6520 696e  m, follow the in
+00000b30: 7374 7275 6374 696f 6e73 206f 6e20 7468  structions on th
+00000b40: 6520 5b6d 6f73 7175 6974 746f 2077 6562  e [mosquitto web
+00000b50: 7369 7465 5d28 6874 7470 733a 2f2f 6d6f  site](https://mo
+00000b60: 7371 7569 7474 6f2e 6f72 672f 646f 776e  squitto.org/down
+00000b70: 6c6f 6164 2f29 2e0a 0a0a 4974 2069 7320  load/)....It is 
+00000b80: 616c 736f 206e 6563 6573 7361 7279 2074  also necessary t
+00000b90: 6f20 696e 7374 616c 6c20 646f 636b 6572  o install docker
+00000ba0: 2e20 466f 7220 6d6f 7265 2069 6e66 6f72  . For more infor
+00000bb0: 6d61 7469 6f6e 2063 6865 636b 2074 6865  mation check the
+00000bc0: 205b 646f 636b 6572 2064 6f63 756d 656e   [docker documen
+00000bd0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00000be0: 646f 6373 2e64 6f63 6b65 722e 636f 6d2f  docs.docker.com/
+00000bf0: 6765 742d 646f 636b 6572 2f29 2e0a 0a23  get-docker/)...#
+00000c00: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
+00000c10: 5468 6520 6f66 6669 6369 616c 2064 6f63  The official doc
+00000c20: 756d 656e 7461 7469 6f6e 206f 6620 7468  umentation of th
+00000c30: 6520 7061 636b 6167 6520 6973 2061 7661  e package is ava
+00000c40: 696c 6162 6c65 206f 6e20 5b52 6561 6420  ilable on [Read 
+00000c50: 7468 6520 446f 6373 5d28 6874 7470 733a  the Docs](https:
+00000c60: 2f2f 6164 616d 2d73 696d 756c 6174 6f72  //adam-simulator
+00000c70: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000c80: 656e 2f6c 6174 6573 742f 292e 2048 6572  en/latest/). Her
+00000c90: 6520 796f 7520 7769 6c6c 2066 696e 6420  e you will find 
+00000ca0: 7468 6520 5b69 6e73 7461 6c6c 6174 696f  the [installatio
+00000cb0: 6e20 696e 7374 7275 6374 696f 6e73 5d28  n instructions](
+00000cc0: 6874 7470 733a 2f2f 6164 616d 2d73 696d  https://adam-sim
+00000cd0: 756c 6174 6f72 2e72 6561 6474 6865 646f  ulator.readthedo
+00000ce0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000cf0: 7372 632f 696e 7374 616c 6c61 7469 6f6e  src/installation
+00000d00: 2e68 746d 6c29 2c20 7468 6520 5b41 5049  .html), the [API
+00000d10: 2072 6566 6572 656e 6365 5d28 6874 7470   reference](http
+00000d20: 733a 2f2f 6164 616d 2d73 696d 756c 6174  s://adam-simulat
+00000d30: 6f72 2e72 6561 6474 6865 646f 6373 2e69  or.readthedocs.i
+00000d40: 6f2f 656e 2f6c 6174 6573 742f 7372 632f  o/en/latest/src/
+00000d50: 6170 695f 7265 6665 7265 6e63 652e 6874  api_reference.ht
+00000d60: 6d6c 2920 616e 6420 736f 6d65 205b 6d69  ml) and some [mi
+00000d70: 6e69 6d61 6c20 776f 726b 696e 6720 6578  nimal working ex
+00000d80: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
+00000d90: 6164 616d 2d73 696d 756c 6174 6f72 2e72  adam-simulator.r
+00000da0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000db0: 2f6c 6174 6573 742f 7372 632f 6578 616d  /latest/src/exam
+00000dc0: 706c 6573 2e68 746d 6c29 2e0a            ples.html)..
```

### Comparing `adam_sim-0.4.1/README.md` & `adam_sim-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,221 @@
-00000000: 2320 4144 414d 2073 696d 756c 6174 6f72  # ADAM simulator
-00000010: 0a0a 5b21 5b70 7970 6920 7665 7273 696f  ..[![pypi versio
-00000020: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
-00000030: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000040: 2f61 6461 6d2d 7369 6d3f 6c6f 676f 3d70  /adam-sim?logo=p
-00000050: 7970 6929 5d28 6874 7470 733a 2f2f 7079  ypi)](https://py
-00000060: 7069 2e6f 7267 2f70 726f 6a65 6374 2f61  pi.org/project/a
-00000070: 6461 6d2d 7369 6d2f 290a 5b21 5b4d 4954  dam-sim/).[![MIT
-00000080: 204c 6963 656e 7365 5d28 6874 7470 733a   License](https:
-00000090: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000000a0: 2f62 6164 6765 2f6c 6963 656e 7365 2d4d  /badge/license-M
-000000b0: 4954 2d62 6c75 652e 7376 673f 7374 796c  IT-blue.svg?styl
-000000c0: 653d 666c 6174 295d 2868 7474 703a 2f2f  e=flat)](http://
-000000d0: 6368 6f6f 7365 616c 6963 656e 7365 2e63  choosealicense.c
-000000e0: 6f6d 2f6c 6963 656e 7365 732f 6d69 742f  om/licenses/mit/
-000000f0: 290a 5b21 5b64 6f63 735d 2868 7474 7073  ).[![docs](https
-00000100: 3a2f 2f62 6164 6765 6e2e 6e65 742f 6261  ://badgen.net/ba
-00000110: 6467 652f 7265 6164 7468 6564 6f63 732f  dge/readthedocs/
-00000120: 646f 6375 6d65 6e74 6174 696f 6e2f 626c  documentation/bl
-00000130: 7565 295d 2868 7474 7073 3a2f 2f61 6461  ue)](https://ada
-00000140: 6d2d 7369 6d75 6c61 746f 722e 7265 6164  m-simulator.read
-00000150: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000160: 7465 7374 2f29 0a0a 4144 414d 2028 4175  test/)..ADAM (Au
-00000170: 746f 6e6f 6d6f 7573 2044 6f6d 6573 7469  tonomous Domesti
-00000180: 6320 416d 6269 6465 7874 726f 7573 204d  c Ambidextrous M
-00000190: 616e 6970 756c 6174 6f72 2920 6973 2061  anipulator) is a
-000001a0: 206d 6f62 696c 6520 726f 626f 7420 6d61   mobile robot ma
-000001b0: 6e69 7075 6c61 746f 7220 636f 6e73 6973  nipulator consis
-000001c0: 7469 6e67 206f 6620 6120 6261 7365 2077  ting of a base w
-000001d0: 6974 6820 7477 6f20 4465 6772 6565 7320  ith two Degrees 
-000001e0: 6f66 2046 7265 6564 6f6d 2028 446f 4629  of Freedom (DoF)
-000001f0: 2061 6e64 2074 776f 2055 6e69 7665 7273   and two Univers
-00000200: 616c 2052 6f62 6f74 7320 5552 3320 6f66  al Robots UR3 of
-00000210: 2036 2044 6f46 2065 6163 682e 0a0a 5468   6 DoF each...Th
-00000220: 6520 7369 6d75 6c61 7469 6f6e 2077 6173  e simulation was
-00000230: 2062 7569 6c74 2075 7369 6e67 205b 4d75   built using [Mu
-00000240: 4a6f 436f 5d28 6874 7470 733a 2f2f 6d75  JoCo](https://mu
-00000250: 6a6f 636f 2e6f 7267 2f29 2c20 6120 6672  joco.org/), a fr
-00000260: 6565 2061 6e64 206f 7065 6e20 736f 7572  ee and open sour
-00000270: 6365 2070 6879 7369 6373 2065 6e67 696e  ce physics engin
-00000280: 6520 6465 7369 676e 6564 2066 726f 6d20  e designed from 
-00000290: 7468 6520 6772 6f75 6e64 2075 7020 666f  the ground up fo
-000002a0: 7220 7468 6520 7075 7270 6f73 6520 6f66  r the purpose of
-000002b0: 206d 6f64 656c 2d62 6173 6564 206f 7074   model-based opt
-000002c0: 696d 697a 6174 696f 6e2c 2061 6e64 2069  imization, and i
-000002d0: 6e20 7061 7274 6963 756c 6172 206f 7074  n particular opt
-000002e0: 696d 697a 6174 696f 6e20 7468 726f 7567  imization throug
-000002f0: 6820 636f 6e74 6163 7473 2e0a 0a23 2320  h contacts...## 
-00000300: 496e 7374 616c 6c61 7469 6f6e 0a0a 466f  Installation..Fo
-00000310: 6c6c 6f77 2074 6865 206e 6578 7420 7374  llow the next st
-00000320: 6570 7320 666f 7220 696e 7374 616c 6c69  eps for installi
-00000330: 6e67 2074 6865 2073 696d 756c 6174 696f  ng the simulatio
-00000340: 6e20 6f6e 2079 6f75 7220 6465 7669 6365  n on your device
-00000350: 2e0a 0a2a 2a52 6571 7569 6572 656d 656e  ...**Requieremen
-00000360: 7473 3a2a 2a0a 2d20 5079 7468 6f6e 2033  ts:**.- Python 3
-00000370: 2e31 302e 3020 6f72 2068 6967 6865 720a  .10.0 or higher.
-00000380: 0a3e 202a 2a4e 6f74 652a 2a3a 2054 6865  .> **Note**: The
-00000390: 2041 6461 6d20 5369 6d75 6c61 746f 7220   Adam Simulator 
-000003a0: 776f 726b 7320 6f6e 204c 696e 7578 2c20  works on Linux, 
-000003b0: 5769 6e64 6f77 7320 616e 6420 4d61 632e  Windows and Mac.
-000003c0: 0a0a 2323 2320 496e 7374 616c 6c20 6d69  ..### Install mi
-000003d0: 6e69 636f 6e64 6120 2868 6967 686c 792d  niconda (highly-
-000003e0: 7265 636f 6d6d 656e 6465 6429 0a49 7420  recommended).It 
-000003f0: 6973 2068 6967 686c 7920 7265 636f 6d6d  is highly recomm
-00000400: 656e 6465 6420 746f 2069 6e73 7461 6c6c  ended to install
-00000410: 2061 6c6c 2074 6865 2064 6570 656e 6465   all the depende
-00000420: 6e63 6965 7320 6f6e 2061 206e 6577 2076  ncies on a new v
-00000430: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00000440: 6e74 2e20 466f 7220 6d6f 7265 2069 6e66  nt. For more inf
-00000450: 6f72 6d61 7469 6f6e 2063 6865 636b 2074  ormation check t
-00000460: 6865 2063 6f6e 6461 2064 6f63 756d 656e  he conda documen
-00000470: 7461 7469 6f6e 2066 6f72 205b 696e 7374  tation for [inst
-00000480: 616c 6c61 7469 6f6e 5d28 6874 7470 733a  allation](https:
-00000490: 2f2f 636f 6e64 612e 696f 2f70 726f 6a65  //conda.io/proje
-000004a0: 6374 732f 636f 6e64 612f 656e 2f6c 6174  cts/conda/en/lat
-000004b0: 6573 742f 7573 6572 2d67 7569 6465 2f69  est/user-guide/i
-000004c0: 6e73 7461 6c6c 2f69 6e64 6578 2e68 746d  nstall/index.htm
-000004d0: 6c29 2061 6e64 205b 656e 7669 726f 6e6d  l) and [environm
-000004e0: 656e 7420 6d61 6e61 6765 6d65 6e74 5d28  ent management](
-000004f0: 6874 7470 733a 2f2f 636f 6e64 612e 696f  https://conda.io
-00000500: 2f70 726f 6a65 6374 732f 636f 6e64 612f  /projects/conda/
-00000510: 656e 2f6c 6174 6573 742f 7573 6572 2d67  en/latest/user-g
-00000520: 7569 6465 2f74 6173 6b73 2f6d 616e 6167  uide/tasks/manag
-00000530: 652d 656e 7669 726f 6e6d 656e 7473 2e68  e-environments.h
-00000540: 746d 6c29 2e20 466f 7220 6372 6561 7469  tml). For creati
-00000550: 6e67 2074 6865 2065 6e76 6972 6f6e 6d65  ng the environme
-00000560: 6e74 2075 7365 2074 6865 2066 6f6c 6c6f  nt use the follo
-00000570: 7769 6e67 2063 6f6d 6d61 6e64 7320 6f6e  wing commands on
-00000580: 2074 6865 2074 6572 6d69 6e61 6c2e 0a0a   the terminal...
-00000590: 6060 6062 6173 680a 636f 6e64 6120 6372  ```bash.conda cr
-000005a0: 6561 7465 202d 6e20 6164 616d 2070 7974  eate -n adam pyt
-000005b0: 686f 6e3d 3d33 2e31 302e 390a 636f 6e64  hon==3.10.9.cond
-000005c0: 6120 6163 7469 7661 7465 2061 6461 6d0a  a activate adam.
-000005d0: 6060 600a 2323 2320 496e 7374 616c 6c20  ```.### Install 
-000005e0: 6672 6f6d 2070 6970 0a54 6865 2041 4441  from pip.The ADA
-000005f0: 4d20 7369 6d75 6c61 746f 7220 6973 2061  M simulator is a
-00000600: 7661 696c 6162 6c65 2061 7320 6120 7069  vailable as a pi
-00000610: 7020 7061 636b 6167 652e 2046 6f72 2069  p package. For i
-00000620: 6e73 7461 6c6c 696e 6720 6974 206a 7573  nstalling it jus
-00000630: 7420 7573 653a 0a60 6060 0a70 6970 2069  t use:.```.pip i
-00000640: 6e73 7461 6c6c 2061 6461 6d2d 7369 6d0a  nstall adam-sim.
-00000650: 6060 600a 0a23 2323 2049 6e73 7461 6c6c  ```..### Install
-00000660: 2066 726f 6d20 736f 7572 6365 0a46 6972   from source.Fir
-00000670: 7374 6c79 2c20 636c 6f6e 6520 7468 6520  stly, clone the 
-00000680: 7265 706f 7369 746f 7279 2069 6e20 796f  repository in yo
-00000690: 7572 2073 7973 7465 6d2e 0a60 6060 6261  ur system..```ba
-000006a0: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
-000006b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000006c0: 7669 7374 6f72 6d75 2f61 6461 6d5f 7369  vistormu/adam_si
-000006d0: 6d75 6c61 746f 722e 6769 740a 6060 600a  mulator.git.```.
-000006e0: 0a54 6865 6e2c 2065 6e74 6572 2074 6865  .Then, enter the
-000006f0: 2064 6972 6563 746f 7279 2061 6e64 2069   directory and i
-00000700: 6e73 7461 6c6c 2074 6865 2072 6571 7569  nstall the requi
-00000710: 7265 6420 6465 7065 6e64 656e 6369 6573  red dependencies
-00000720: 0a60 6060 6261 7368 0a63 6420 6164 616d  .```bash.cd adam
-00000730: 5f73 696d 756c 6174 6f72 0a70 6970 2069  _simulator.pip i
-00000740: 6e73 7461 6c6c 202d 7220 7265 7175 6972  nstall -r requir
-00000750: 656d 656e 7473 2e74 7874 0a60 6060 0a0a  ements.txt.```..
-00000760: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-00000770: 0a54 6865 206f 6666 6963 6961 6c20 646f  .The official do
-00000780: 6375 6d65 6e74 6174 696f 6e20 6f66 2074  cumentation of t
-00000790: 6865 2070 6163 6b61 6765 2069 7320 6176  he package is av
-000007a0: 6169 6c61 626c 6520 6f6e 205b 5265 6164  ailable on [Read
-000007b0: 2074 6865 2044 6f63 735d 2868 7474 7073   the Docs](https
-000007c0: 3a2f 2f61 6461 6d2d 7369 6d75 6c61 746f  ://adam-simulato
-000007d0: 722e 7265 6164 7468 6564 6f63 732e 696f  r.readthedocs.io
-000007e0: 2f65 6e2f 6c61 7465 7374 2f29 2e20 4865  /en/latest/). He
-000007f0: 7265 2079 6f75 2077 696c 6c20 6669 6e64  re you will find
-00000800: 2074 6865 205b 696e 7374 616c 6c61 7469   the [installati
-00000810: 6f6e 2069 6e73 7472 7563 7469 6f6e 735d  on instructions]
-00000820: 2868 7474 7073 3a2f 2f61 6461 6d2d 7369  (https://adam-si
-00000830: 6d75 6c61 746f 722e 7265 6164 7468 6564  mulator.readthed
-00000840: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000850: 2f73 7263 2f69 6e73 7461 6c6c 6174 696f  /src/installatio
-00000860: 6e2e 6874 6d6c 292c 2074 6865 205b 4150  n.html), the [AP
-00000870: 4920 7265 6665 7265 6e63 655d 2868 7474  I reference](htt
-00000880: 7073 3a2f 2f61 6461 6d2d 7369 6d75 6c61  ps://adam-simula
-00000890: 746f 722e 7265 6164 7468 6564 6f63 732e  tor.readthedocs.
-000008a0: 696f 2f65 6e2f 6c61 7465 7374 2f73 7263  io/en/latest/src
-000008b0: 2f61 7069 5f72 6566 6572 656e 6365 2e68  /api_reference.h
-000008c0: 746d 6c29 2061 6e64 2073 6f6d 6520 5b6d  tml) and some [m
-000008d0: 696e 696d 616c 2077 6f72 6b69 6e67 2065  inimal working e
-000008e0: 7861 6d70 6c65 735d 2868 7474 7073 3a2f  xamples](https:/
-000008f0: 2f61 6461 6d2d 7369 6d75 6c61 746f 722e  /adam-simulator.
-00000900: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00000910: 6e2f 6c61 7465 7374 2f73 7263 2f65 7861  n/latest/src/exa
-00000920: 6d70 6c65 732e 6874 6d6c 292e 0a         mples.html)..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6164 616d  : 2.1.Name: adam
+00000020: 5f73 696d 0a56 6572 7369 6f6e 3a20 312e  _sim.Version: 1.
+00000030: 302e 300a 5375 6d6d 6172 793a 2041 2073  0.0.Summary: A s
+00000040: 696d 756c 6174 6f72 206f 6620 4144 414d  imulator of ADAM
+00000050: 2028 4175 746f 6e6f 6d6f 7573 2044 6f6d   (Autonomous Dom
+00000060: 6573 7469 6320 416d 6269 6465 7874 726f  estic Ambidextro
+00000070: 7573 204d 616e 6970 756c 6174 6f72 292c  us Manipulator),
+00000080: 2061 206d 6f62 696c 6520 726f 626f 7420   a mobile robot 
+00000090: 6d61 6e69 7075 6c61 746f 7220 636f 6e73  manipulator cons
+000000a0: 6973 7469 6e67 206f 6620 6120 6261 7365  isting of a base
+000000b0: 2077 6974 6820 7477 6f20 4465 6772 6565   with two Degree
+000000c0: 7320 6f66 2046 7265 6564 6f6d 2028 446f  s of Freedom (Do
+000000d0: 4629 2061 6e64 2074 776f 2055 6e69 7665  F) and two Unive
+000000e0: 7273 616c 2052 6f62 6f74 7320 5552 3320  rsal Robots UR3 
+000000f0: 6f66 2036 2044 6f46 2065 6163 682e 0a41  of 6 DoF each..A
+00000100: 7574 686f 723a 2056 6973 746f 720a 5072  uthor: Vistor.Pr
+00000110: 6f6a 6563 742d 5552 4c3a 2048 6f6d 6570  oject-URL: Homep
+00000120: 6167 652c 2068 7474 7073 3a2f 2f67 6974  age, https://git
+00000130: 6875 622e 636f 6d2f 7669 7374 6f72 6d75  hub.com/vistormu
+00000140: 2f61 6461 6d5f 7369 6d75 6c61 746f 720a  /adam_simulator.
+00000150: 5072 6f6a 6563 742d 5552 4c3a 2042 7567  Project-URL: Bug
+00000160: 2054 7261 636b 6572 2c20 6874 7470 733a   Tracker, https:
+00000170: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6973  //github.com/vis
+00000180: 746f 726d 752f 6164 616d 5f73 696d 756c  tormu/adam_simul
+00000190: 6174 6f72 2f69 7373 7565 730a 436c 6173  ator/issues.Clas
+000001a0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000001b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001c0: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
+000001d0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+000001e0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+000001f0: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
+00000200: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
+00000210: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000220: 5320 496e 6465 7065 6e64 656e 740a 5265  S Independent.Re
+00000230: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000240: 3d33 2e31 300a 4465 7363 7269 7074 696f  =3.10.Descriptio
+00000250: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000260: 7465 7874 2f6d 6172 6b64 6f77 6e0a 4c69  text/markdown.Li
+00000270: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+00000280: 4e53 450a 0a23 2041 4441 4d20 5369 6d75  NSE..# ADAM Simu
+00000290: 6c61 746f 720a 0a3c 7020 616c 6967 6e3d  lator..<p align=
+000002a0: 2263 656e 7465 7222 3e0a 2020 2020 3c61  "center">.    <a
+000002b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000002c0: 6974 6875 622e 636f 6d2f 7669 7374 6f72  ithub.com/vistor
+000002d0: 6d75 2f61 6461 6d5f 7369 6d75 6c61 746f  mu/adam_simulato
+000002e0: 7222 3e0a 2020 2020 2020 2020 3c69 6d67  r">.        <img
+000002f0: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
+00000300: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00000310: 656e 742e 636f 6d2f 7669 7374 6f72 6d75  ent.com/vistormu
+00000320: 2f61 6461 6d5f 7369 6d75 6c61 746f 722f  /adam_simulator/
+00000330: 6d61 7374 6572 2f64 6f63 732f 6173 7365  master/docs/asse
+00000340: 7473 2f61 6461 6d2e 706e 6722 3e0a 2020  ts/adam.png">.  
+00000350: 2020 3c2f 613e 0a3c 2f70 3e0a 0a5b 215b    </a>.</p>..[![
+00000360: 7079 7069 2076 6572 7369 6f6e 5d28 6874  pypi version](ht
+00000370: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000380: 732e 696f 2f70 7970 692f 762f 6164 616d  s.io/pypi/v/adam
+00000390: 2d73 696d 3f6c 6f67 6f3d 7079 7069 295d  -sim?logo=pypi)]
+000003a0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000003b0: 672f 7072 6f6a 6563 742f 6164 616d 2d73  g/project/adam-s
+000003c0: 696d 2f29 0a5b 215b 4d49 5420 4c69 6365  im/).[![MIT Lice
+000003d0: 6e73 655d 2868 7474 7073 3a2f 2f69 6d67  nse](https://img
+000003e0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000003f0: 652f 6c69 6365 6e73 652d 4d49 542d 626c  e/license-MIT-bl
+00000400: 7565 2e73 7667 3f73 7479 6c65 3d66 6c61  ue.svg?style=fla
+00000410: 7429 5d28 6874 7470 3a2f 2f63 686f 6f73  t)](http://choos
+00000420: 6561 6c69 6365 6e73 652e 636f 6d2f 6c69  ealicense.com/li
+00000430: 6365 6e73 6573 2f6d 6974 2f29 0a5b 215b  censes/mit/).[![
+00000440: 646f 6373 5d28 6874 7470 733a 2f2f 6261  docs](https://ba
+00000450: 6467 656e 2e6e 6574 2f62 6164 6765 2f72  dgen.net/badge/r
+00000460: 6561 6474 6865 646f 6373 2f64 6f63 756d  eadthedocs/docum
+00000470: 656e 7461 7469 6f6e 2f62 6c75 6529 5d28  entation/blue)](
+00000480: 6874 7470 733a 2f2f 6164 616d 2d73 696d  https://adam-sim
+00000490: 756c 6174 6f72 2e72 6561 6474 6865 646f  ulator.readthedo
+000004a0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+000004b0: 290a 0a41 4441 4d20 2841 7574 6f6e 6f6d  )..ADAM (Autonom
+000004c0: 6f75 7320 446f 6d65 7374 6963 2041 6d62  ous Domestic Amb
+000004d0: 6964 6578 7472 6f75 7320 4d61 6e69 7075  idextrous Manipu
+000004e0: 6c61 746f 7229 2069 7320 6120 6d6f 6269  lator) is a mobi
+000004f0: 6c65 2072 6f62 6f74 206d 616e 6970 756c  le robot manipul
+00000500: 6174 6f72 2063 6f6e 7369 7374 696e 6720  ator consisting 
+00000510: 6f66 2061 2062 6173 6520 7769 7468 2074  of a base with t
+00000520: 776f 2044 6567 7265 6573 206f 6620 4672  wo Degrees of Fr
+00000530: 6565 646f 6d20 2844 6f46 2920 616e 6420  eedom (DoF) and 
+00000540: 7477 6f20 556e 6976 6572 7361 6c20 526f  two Universal Ro
+00000550: 626f 7473 2055 5233 206f 6620 3620 446f  bots UR3 of 6 Do
+00000560: 4620 6561 6368 2e0a 0a54 6865 2073 696d  F each...The sim
+00000570: 756c 6174 696f 6e20 7761 7320 6275 696c  ulation was buil
+00000580: 7420 7573 696e 6720 5b4d 754a 6f43 6f5d  t using [MuJoCo]
+00000590: 2868 7474 7073 3a2f 2f6d 756a 6f63 6f2e  (https://mujoco.
+000005a0: 6f72 672f 292c 2061 2066 7265 6520 616e  org/), a free an
+000005b0: 6420 6f70 656e 2073 6f75 7263 6520 7068  d open source ph
+000005c0: 7973 6963 7320 656e 6769 6e65 2064 6573  ysics engine des
+000005d0: 6967 6e65 6420 6672 6f6d 2074 6865 2067  igned from the g
+000005e0: 726f 756e 6420 7570 2066 6f72 2074 6865  round up for the
+000005f0: 2070 7572 706f 7365 206f 6620 6d6f 6465   purpose of mode
+00000600: 6c2d 6261 7365 6420 6f70 7469 6d69 7a61  l-based optimiza
+00000610: 7469 6f6e 2c20 616e 6420 696e 2070 6172  tion, and in par
+00000620: 7469 6375 6c61 7220 6f70 7469 6d69 7a61  ticular optimiza
+00000630: 7469 6f6e 2074 6872 6f75 6768 2063 6f6e  tion through con
+00000640: 7461 6374 732e 0a0a 2323 2049 6e73 7461  tacts...## Insta
+00000650: 6c6c 6174 696f 6e0a 0a46 6f6c 6c6f 7720  llation..Follow 
+00000660: 7468 6520 6e65 7874 2073 7465 7073 2066  the next steps f
+00000670: 6f72 2069 6e73 7461 6c6c 696e 6720 7468  or installing th
+00000680: 6520 7369 6d75 6c61 7469 6f6e 206f 6e20  e simulation on 
+00000690: 796f 7572 2064 6576 6963 652e 0a0a 2a2a  your device...**
+000006a0: 5265 7175 6965 7265 6d65 6e74 733a 2a2a  Requierements:**
+000006b0: 0a2d 2050 7974 686f 6e20 332e 3130 2e30  .- Python 3.10.0
+000006c0: 206f 7220 6869 6768 6572 0a0a 3e20 2a2a   or higher..> **
+000006d0: 4e6f 7465 2a2a 3a20 5468 6520 4164 616d  Note**: The Adam
+000006e0: 2053 696d 756c 6174 6f72 2077 6f72 6b73   Simulator works
+000006f0: 206f 6e20 4c69 6e75 782c 2057 696e 646f   on Linux, Windo
+00000700: 7773 2061 6e64 204d 6163 2e0a 0a23 2323  ws and Mac...###
+00000710: 2049 6e73 7461 6c6c 206d 696e 6963 6f6e   Install minicon
+00000720: 6461 2028 6869 6768 6c79 2d72 6563 6f6d  da (highly-recom
+00000730: 6d65 6e64 6564 290a 4974 2069 7320 6869  mended).It is hi
+00000740: 6768 6c79 2072 6563 6f6d 6d65 6e64 6564  ghly recommended
+00000750: 2074 6f20 696e 7374 616c 6c20 616c 6c20   to install all 
+00000760: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00000770: 206f 6e20 6120 6e65 7720 7669 7274 7561   on a new virtua
+00000780: 6c20 656e 7669 726f 6e6d 656e 742e 2046  l environment. F
+00000790: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+000007a0: 696f 6e20 6368 6563 6b20 7468 6520 636f  ion check the co
+000007b0: 6e64 6120 646f 6375 6d65 6e74 6174 696f  nda documentatio
+000007c0: 6e20 666f 7220 5b69 6e73 7461 6c6c 6174  n for [installat
+000007d0: 696f 6e5d 2868 7474 7073 3a2f 2f63 6f6e  ion](https://con
+000007e0: 6461 2e69 6f2f 7072 6f6a 6563 7473 2f63  da.io/projects/c
+000007f0: 6f6e 6461 2f65 6e2f 6c61 7465 7374 2f75  onda/en/latest/u
+00000800: 7365 722d 6775 6964 652f 696e 7374 616c  ser-guide/instal
+00000810: 6c2f 696e 6465 782e 6874 6d6c 2920 616e  l/index.html) an
+00000820: 6420 5b65 6e76 6972 6f6e 6d65 6e74 206d  d [environment m
+00000830: 616e 6167 656d 656e 745d 2868 7474 7073  anagement](https
+00000840: 3a2f 2f63 6f6e 6461 2e69 6f2f 7072 6f6a  ://conda.io/proj
+00000850: 6563 7473 2f63 6f6e 6461 2f65 6e2f 6c61  ects/conda/en/la
+00000860: 7465 7374 2f75 7365 722d 6775 6964 652f  test/user-guide/
+00000870: 7461 736b 732f 6d61 6e61 6765 2d65 6e76  tasks/manage-env
+00000880: 6972 6f6e 6d65 6e74 732e 6874 6d6c 292e  ironments.html).
+00000890: 2046 6f72 2063 7265 6174 696e 6720 7468   For creating th
+000008a0: 6520 656e 7669 726f 6e6d 656e 7420 7573  e environment us
+000008b0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+000008c0: 636f 6d6d 616e 6473 206f 6e20 7468 6520  commands on the 
+000008d0: 7465 726d 696e 616c 2e0a 0a60 6060 6261  terminal...```ba
+000008e0: 7368 0a63 6f6e 6461 2063 7265 6174 6520  sh.conda create 
+000008f0: 2d6e 2061 6461 6d20 7079 7468 6f6e 3d3d  -n adam python==
+00000900: 332e 3130 2e39 0a63 6f6e 6461 2061 6374  3.10.9.conda act
+00000910: 6976 6174 6520 6164 616d 0a60 6060 0a23  ivate adam.```.#
+00000920: 2323 2049 6e73 7461 6c6c 2066 726f 6d20  ## Install from 
+00000930: 7069 700a 5468 6520 4144 414d 2073 696d  pip.The ADAM sim
+00000940: 756c 6174 6f72 2069 7320 6176 6169 6c61  ulator is availa
+00000950: 626c 6520 6173 2061 2070 6970 2070 6163  ble as a pip pac
+00000960: 6b61 6765 2e20 466f 7220 696e 7374 616c  kage. For instal
+00000970: 6c69 6e67 2069 7420 6a75 7374 2075 7365  ling it just use
+00000980: 3a0a 6060 600a 7069 7020 696e 7374 616c  :.```.pip instal
+00000990: 6c20 6164 616d 2d73 696d 0a60 6060 0a0a  l adam-sim.```..
+000009a0: 2323 2320 496e 7374 616c 6c20 6672 6f6d  ### Install from
+000009b0: 2073 6f75 7263 650a 4669 7273 746c 792c   source.Firstly,
+000009c0: 2063 6c6f 6e65 2074 6865 2072 6570 6f73   clone the repos
+000009d0: 6974 6f72 7920 696e 2079 6f75 7220 7379  itory in your sy
+000009e0: 7374 656d 2e0a 6060 6062 6173 680a 6769  stem..```bash.gi
+000009f0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000a00: 6769 7468 7562 2e63 6f6d 2f76 6973 746f  github.com/visto
+00000a10: 726d 752f 6164 616d 5f73 696d 756c 6174  rmu/adam_simulat
+00000a20: 6f72 2e67 6974 0a60 6060 0a0a 5468 656e  or.git.```..Then
+00000a30: 2c20 656e 7465 7220 7468 6520 6469 7265  , enter the dire
+00000a40: 6374 6f72 7920 616e 6420 696e 7374 616c  ctory and instal
+00000a50: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
+00000a60: 6570 656e 6465 6e63 6965 730a 6060 6062  ependencies.```b
+00000a70: 6173 680a 6364 2061 6461 6d5f 7369 6d75  ash.cd adam_simu
+00000a80: 6c61 746f 720a 7069 7020 696e 7374 616c  lator.pip instal
+00000a90: 6c20 2d72 2072 6571 7569 7265 6d65 6e74  l -r requirement
+00000aa0: 732e 7478 740a 6060 600a 0a0a 2323 2320  s.txt.```...### 
+00000ab0: 496e 7374 616c 6c61 7469 6f6e 2066 6f72  Installation for
+00000ac0: 2074 6865 2063 6f6d 6d75 6e69 6361 7469   the communicati
+00000ad0: 6f6e 0a54 6865 2063 6f6d 6d75 6e69 6361  on.The communica
+00000ae0: 7469 6f6e 2075 7365 7320 6d6f 7371 7569  tion uses mosqui
+00000af0: 7474 6f20 6173 2061 2062 726f 6b65 722e  tto as a broker.
+00000b00: 2046 6f72 2069 6e73 7461 6c6c 696e 6720   For installing 
+00000b10: 6974 206f 6e20 796f 7572 2073 7973 7465  it on your syste
+00000b20: 6d2c 2066 6f6c 6c6f 7720 7468 6520 696e  m, follow the in
+00000b30: 7374 7275 6374 696f 6e73 206f 6e20 7468  structions on th
+00000b40: 6520 5b6d 6f73 7175 6974 746f 2077 6562  e [mosquitto web
+00000b50: 7369 7465 5d28 6874 7470 733a 2f2f 6d6f  site](https://mo
+00000b60: 7371 7569 7474 6f2e 6f72 672f 646f 776e  squitto.org/down
+00000b70: 6c6f 6164 2f29 2e0a 0a0a 4974 2069 7320  load/)....It is 
+00000b80: 616c 736f 206e 6563 6573 7361 7279 2074  also necessary t
+00000b90: 6f20 696e 7374 616c 6c20 646f 636b 6572  o install docker
+00000ba0: 2e20 466f 7220 6d6f 7265 2069 6e66 6f72  . For more infor
+00000bb0: 6d61 7469 6f6e 2063 6865 636b 2074 6865  mation check the
+00000bc0: 205b 646f 636b 6572 2064 6f63 756d 656e   [docker documen
+00000bd0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00000be0: 646f 6373 2e64 6f63 6b65 722e 636f 6d2f  docs.docker.com/
+00000bf0: 6765 742d 646f 636b 6572 2f29 2e0a 0a23  get-docker/)...#
+00000c00: 2320 446f 6375 6d65 6e74 6174 696f 6e0a  # Documentation.
+00000c10: 5468 6520 6f66 6669 6369 616c 2064 6f63  The official doc
+00000c20: 756d 656e 7461 7469 6f6e 206f 6620 7468  umentation of th
+00000c30: 6520 7061 636b 6167 6520 6973 2061 7661  e package is ava
+00000c40: 696c 6162 6c65 206f 6e20 5b52 6561 6420  ilable on [Read 
+00000c50: 7468 6520 446f 6373 5d28 6874 7470 733a  the Docs](https:
+00000c60: 2f2f 6164 616d 2d73 696d 756c 6174 6f72  //adam-simulator
+00000c70: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000c80: 656e 2f6c 6174 6573 742f 292e 2048 6572  en/latest/). Her
+00000c90: 6520 796f 7520 7769 6c6c 2066 696e 6420  e you will find 
+00000ca0: 7468 6520 5b69 6e73 7461 6c6c 6174 696f  the [installatio
+00000cb0: 6e20 696e 7374 7275 6374 696f 6e73 5d28  n instructions](
+00000cc0: 6874 7470 733a 2f2f 6164 616d 2d73 696d  https://adam-sim
+00000cd0: 756c 6174 6f72 2e72 6561 6474 6865 646f  ulator.readthedo
+00000ce0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000cf0: 7372 632f 696e 7374 616c 6c61 7469 6f6e  src/installation
+00000d00: 2e68 746d 6c29 2c20 7468 6520 5b41 5049  .html), the [API
+00000d10: 2072 6566 6572 656e 6365 5d28 6874 7470   reference](http
+00000d20: 733a 2f2f 6164 616d 2d73 696d 756c 6174  s://adam-simulat
+00000d30: 6f72 2e72 6561 6474 6865 646f 6373 2e69  or.readthedocs.i
+00000d40: 6f2f 656e 2f6c 6174 6573 742f 7372 632f  o/en/latest/src/
+00000d50: 6170 695f 7265 6665 7265 6e63 652e 6874  api_reference.ht
+00000d60: 6d6c 2920 616e 6420 736f 6d65 205b 6d69  ml) and some [mi
+00000d70: 6e69 6d61 6c20 776f 726b 696e 6720 6578  nimal working ex
+00000d80: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
+00000d90: 6164 616d 2d73 696d 756c 6174 6f72 2e72  adam-simulator.r
+00000da0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000db0: 2f6c 6174 6573 742f 7372 632f 6578 616d  /latest/src/exam
+00000dc0: 706c 6573 2e68 746d 6c29 2e0a            ples.html)..
```

### Comparing `adam_sim-0.4.1/adam/assets/meshes/base.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/body1.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/body2.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/body3.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/body4.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/end_effector_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/end_effector_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/forearm_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/forearm_body_2.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/forearm_cap.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/forearm_link_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/forearm_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/forearm_rubber_2.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/shoulder_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/shoulder_cap.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/shoulder_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/shoulder_screws.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_cap.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_link_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_rubber_2.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_rubber_3.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/upperarm_screws.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_1_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_1_cap.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_1_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_2_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_2_cap.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_2_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_3_body.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_3_cap.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/meshes/wrist_3_rubber.stl` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/assets/scene.xml` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml`

 * *Files 20% similar despite different names*

#### Comparing `adam_sim-0.4.1/adam/assets/scene.xml` & `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml`

```diff
@@ -1,19 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <mujoco model="adam scene">
-  <include file="adam.xml"/>
+  <compiler angle="radian" meshdir="meshes" texturedir="textures" autolimits="true"/>
   <statistic center="0.3 0 0.4" extent="0.8"/>
+  <option timestep="0.017"/>
+  <include file="adam/adam.xml"/>
   <visual>
     <headlight diffuse="0.6 0.6 0.6" ambient="0.3 0.3 0.3" specular="0 0 0"/>
-    <rgba haze="0.15 0.25 0.35 1"/>
+    <rgba haze="0.9 0.9 0.9 1"/>
     <global azimuth="0.0" elevation="-45.0"/>
+    <map fogstart="1" fogend="20" haze="0.7"/>
   </visual>
   <asset>
-    <texture type="skybox" builtin="gradient" rgb1="0.3 0.5 0.7" rgb2="0 0 0" width="512" height="3072"/>
-    <texture type="2d" name="groundplane" builtin="checker" mark="edge" rgb1="0.2 0.3 0.4" rgb2="0.1 0.2 0.3" markrgb="0.8 0.8 0.8" width="300" height="300"/>
-    <material name="groundplane" texture="groundplane" texuniform="true" texrepeat="5 5" reflectance="0.2"/>
+    <texture type="skybox" builtin="gradient" rgb1="0.9 0.9 1.0" rgb2="0.54 0.81 0.94" width="256" height="256"/>
+    <texture type="2d" name="groundplane" file="light-gray-floor-tile.png"/>
+    <material name="groundplane" texture="groundplane" texuniform="true" texrepeat="5 5" reflectance="0.01" specular="0.0" shininess="0.0"/>
   </asset>
   <worldbody>
-    <light pos="1.0 1.0 5.0" dir="0 0 -1" directional="true"/>
+    <light pos="2.0 2.0 3.0" dir="0 0 -1" directional="true"/>
     <geom name="floor" size="0 0 0.05" type="plane" material="groundplane"/>
   </worldbody>
 </mujoco>
```

### Comparing `adam_sim-0.4.1/adam/features/configurations/data/configurations_test.csv` & `adam_sim-1.0.0/adam_sim/features/data_manager/data/configurations_test.csv`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/features/simulation/entities/adam_info.py` & `adam_sim-1.0.0/adam_sim/features/adam/entities/adam_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass
 
-from .manipulator_data import ManipulatorData
-from .base_data import BaseData
+from ...manipulator.entities import ManipulatorInfo
+from ...base.entities import BaseInfo
 
 
 @dataclass
 class AdamInfo:
     '''
     the ADAM Info class is a dataclass that contains all the information of the simulation
 
     Attributes
     ----------
-    left_manipulator : ~.entities.ConfigurationData
+    left_manipulator : ~.entities.ManipulatorInfo
         the data referring to the left manipulator of the robot
 
-    right_manipulator : ~.entities.CollisionData
+    right_manipulator : ~.entities.ManipulatorInfo
         the data referring to the right manipulator of the robot
 
-    base : ~.entities.BaseData
+    base : ~.entities.BaseInfo
         the data referring to the base of the robot
     '''
-    left_manipulator: ManipulatorData
-    right_manipulator: ManipulatorData
-    base: BaseData
+    left_manipulator: ManipulatorInfo
+    right_manipulator: ManipulatorInfo
+    base: BaseInfo
```

### Comparing `adam_sim-0.4.1/adam/features/simulation/entities/collision.py` & `adam_sim-1.0.0/adam_sim/features/manipulator/entities/collision.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,9 +53,9 @@
     wrist_3: list[str]
     
     @classmethod
     def empty(cls):
         '''
         returns an empty instance of the class
         '''
-        return cls(False, False, False, [], [], [], [], [], [], [])
+        return cls(False, False, False, [False]*6, [], [], [], [], [], [])
```

### Comparing `adam_sim-0.4.1/adam/features/simulation/entities/system.py` & `adam_sim-1.0.0/adam_sim/entities/system.py`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/features/simulation/entities/vector.py` & `adam_sim-1.0.0/adam_sim/entities/vector.py`

 * *Files identical despite different names*

### Comparing `adam_sim-0.4.1/adam/features/simulation/simulation.py` & `adam_sim-1.0.0/adam_sim/features/adam/adam.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,242 @@
 import pkg_resources
 import numpy as np
 
 from distutils.dir_util import copy_tree
 
-from .entities import Configuration, AdamInfo
-from .use_cases import DataManager, ControlVisualizer, Viewer, Controller
+from ..base import Base
+from ..manipulator import Manipulator
+from ...entities import Configuration
+from .entities import AdamInfo
+from .use_cases import Viewer
+from .communication import get_adam_repository
+from .repository import AdamRepository
 
+RESOURCE_FILE: str = 'features/adam/communication/implementations/simulated_adam_repository/assets/'
 
-class Simulation:
+
+class Adam:
     '''
-    the Simulation class contains all the methods to control and render the ADAM robot.
+    The `Adam` class contains all the methods to control and render the ADAM robot either in simulation or in real life.
+
+    Attributes
+    ----------
+    base : ~.entities.Base
+        the base of the robot
+
+    left_manipulator : ~.entities.Manipulator
+        the left manipulator of the robot
+
+    right_manipulator : ~.entities.Manipulator
+        the right manipulator of the robot
 
     Methods
     -------
-    load_scene:
+    connect:
+        connects to a given host and port
+
+    load:
         loads a given MuJoCo scene. This method is mandatory to call
 
     step:
-        step on the simulation's dynamics
-
-    control:
-        control the manipulators via sliders
+        advance one step in the simulation
 
     render:
-        render the scene
+        renders the scene
 
     close:
-        close all the renderers
-
-    extend_collisions:
-        extends the collision dictionary
+        closes all the visualizers
 
     check_collisions:
-        checks all the collisions in a given configuration path
+        checks if there are any collisions in the scene
 
     export_scene:
-        exports the default ADAM scene to a given directory
+        exports the scene to the specified directory
     '''
 
     def __init__(self) -> None:
-        self.data_manager: DataManager = DataManager()
-        self.left_control_visualizer: ControlVisualizer = ControlVisualizer('Left Manipulator')
-        self.right_control_visualizer: ControlVisualizer = ControlVisualizer('Right Manipulator')
-        self.controller: Controller = Controller()
-        self.viewer: Viewer = Viewer()
+        # Features
+        self.base: Base = Base()
+        self.left_manipulator: Manipulator = Manipulator()
+        self.right_manipulator: Manipulator = Manipulator()
 
-        self.left_control_mode: bool = False
-        self.right_control_mode: bool = False
+        # Use cases
+        self._viewer: Viewer = Viewer()
 
-    def load_scene(self, filename: str | None = None) -> AdamInfo:
+        # Repository
+        self._repository: AdamRepository = None  # type: ignore
+
+        # Variables
+        self._mode: str = ''
+
+    def connect(self, host: str, port: int, rate: int = 30) -> AdamInfo:
         '''
-        loads a given MuJoCo scene.xml
+        connects to a given host and port
 
         Parameters
         ----------
-        filename : str, optional
-            the path to the scene.xml. By default it loads the integrated ADAM scene
+        host : str
+            the host to connect to
 
-        Returns
-        -------
-        out : ~.entities.AdamInfo
-            the initial info of the robot
+        port : int
+            the port to connect to
         '''
-        if filename is None:
-            filename = pkg_resources.resource_filename('adam', 'assets/scene.xml')
+        self._mode = 'real'
 
-        self.controller.init(filename)
+        # Initialize repositories
+        self._repository = get_adam_repository('real')
+        self._repository.init(host, port, rate)
 
-        return self.data_manager.get(self.controller.data)
+        self.left_manipulator._init_repository('left_real', host, port)
+        self.right_manipulator._init_repository('right_real', host, port)
+        self.base._init_repository('real', host, port)
 
-    def extend_collisions(self, collision_dict: dict[int, str]) -> None:
-        '''
-        it extends the collisions dictionary to incorporate new geometries
+        # Get initial info
+        self._repository.step()
 
-        Parameters
-        ----------
-        collision_dict : dict[int, str]
-            the collision dictionary to incorporate
+        left_manipulator_info = self.left_manipulator._repository.get_info()
+        right_manipulator_info = self.right_manipulator._repository.get_info()
+        base_info = self.base._repository.get_info()
 
-        Notes
-        -----
-        in order to get the corresponding ids, please refer to the geometry_list.md on the GitHub page
-        '''
-        self.data_manager.collision_detector.extend_collisions(collision_dict)
+        return AdamInfo(left_manipulator_info, right_manipulator_info, base_info)
 
-    def check_collisions(self, left_configuration_list: list[Configuration], right_configuration_list: list[Configuration]) -> tuple[np.ndarray, np.ndarray]:
+    def load(self, filename: str | None = None) -> AdamInfo:
         '''
-        a method to directly calculate the collisions on a given set of configurations
+        loads a given MuJoCo scene.xml
 
         Parameters
         ----------
-        left_configuration_list : list[~.entities.Configuration]
-            the list of configurations for the left manipulator
-
-        right_configuration_list : list[~.entities.Configuration]
-            the list of configurations for the right manipulator
+        filename : str, optional
+            the path to the scene.xml. By default it loads the integrated ADAM scene
 
         Returns
         -------
-        out : tuple[np.ndarray, np.ndarray]
-            a tuple containing the self collisions and the environment collisions respectively. A given value of the array is 1 if a collision has been detected
+        out : ~.entities.AdamInfo
+            the initial info of the robot
         '''
-        self_collision_array: np.ndarray = np.zeros(len(left_configuration_list))
-        env_collision_array: np.ndarray = np.zeros(len(left_configuration_list))
-        for i, (left_configuration, right_configuration) in enumerate(zip(left_configuration_list, right_configuration_list)):
-            info: AdamInfo = self.step(left_configuration, right_configuration)
-            if info.left_manipulator.collision.self_collision or info.right_manipulator.collision.self_collision:
-                self_collision_array[i] = 1
-            if info.left_manipulator.collision.env_collision or info.right_manipulator.collision.env_collision:
-                env_collision_array[i] = 1
+        self._mode = 'sim'
 
-        return self_collision_array, env_collision_array
+        if filename is None:
+            filename = pkg_resources.resource_filename('adam_sim', RESOURCE_FILE + 'scene.xml')
 
-    def step(self, left_configuration: Configuration, right_configuration: Configuration) -> AdamInfo:
-        '''
-        a step forward on the dynamics of the simulation
+        # Initialize repositories
+        self._repository = get_adam_repository('simulated')
+        self._repository.init(filename)
 
-        Parameters
-        ----------
-        left_configuration : ~.entities.Configuration
-            the configuration to send to the left manipulator
+        self.left_manipulator._init_repository('left_simulated', self._repository.data)
+        self.right_manipulator._init_repository('right_simulated', self._repository.data)
+        self.base._init_repository('simulated', self._repository.data)
+
+        # Get initial info
+        self._repository.step()
+
+        left_manipulator_info = self.left_manipulator._repository.get_info()
+        right_manipulator_info = self.right_manipulator._repository.get_info()
+        base_info = self.base._repository.get_info()
 
-        right_configuration : ~.entities.Configuration
-            the configuration to send to the right manipulator
+        return AdamInfo(left_manipulator_info, right_manipulator_info, base_info)
+
+    def step(self) -> AdamInfo:
+        '''
+        advance one step in the simulation
 
         Returns
         -------
         out : ~.entities.AdamInfo
-            the simulation data
+            the info of the robot at the current step
         '''
-        self.controller.set_configuration(left_configuration, right_configuration)
-        self.controller.step()
+        self._repository.step()
 
-        return self.data_manager.get(self.controller.data)
+        left_manipulator_info = self.left_manipulator._repository.get_info()
+        right_manipulator_info = self.right_manipulator._repository.get_info()
+        base_info = self.base._repository.get_info()
 
-    def control(self, mode: str = 'both') -> AdamInfo:
+        return AdamInfo(left_manipulator_info, right_manipulator_info, base_info)
+
+    def render(self, hide_menu: bool = True) -> None:
         '''
-        a method to control directly the manipulators via sliders
+        renders the scene
 
         Parameters
         ----------
-        mode : str, optional
-            indicates the manipulator to control. Possible values: 'left', 'right', 'both'. 'both' by default
-
-        Returns
-        -------
-        out : ~.entities.AdamInfo
-            the simulation data
+        hide_menu : bool, optional
+            whether to hide the menu or not. By default it is True
         '''
-        if mode == 'left':
-            self.left_control_mode = True
-        elif mode == 'right':
-            self.right_control_mode = True
-        elif mode == 'both':
-            self.left_control_mode = True
-            self.right_control_mode = True
-
-        left_configuration: Configuration = self.controller.get_left_configuration()
-        right_configuration: Configuration = self.controller.get_right_configuration()
+        if self._mode != 'sim':
+            return
 
-        if self.left_control_visualizer.is_active:
-            left_configuration = Configuration(*self.left_control_visualizer.get())
+        self._viewer.init(self._repository.model, self._repository.data)
 
-        if self.right_control_visualizer.is_active:
-            right_configuration = Configuration(*self.right_control_visualizer.get())
+        self.left_manipulator._control_visualizer.render(60)
+        self.right_manipulator._control_visualizer.render(60)
+        self._viewer.render(hide_menu)
 
-        self.controller.set_configuration(left_configuration, right_configuration)
-        self.controller.step()
+    def close(self) -> None:
+        '''
+        closes all the visualizers and connections
+        '''
+        self.left_manipulator._control_visualizer.close()
+        self.right_manipulator._control_visualizer.close()
+        self._viewer.close()
 
-        return self.data_manager.get(self.controller.data)
+        self._repository.close()
+        self.left_manipulator._repository.close()
+        self.right_manipulator._repository.close()
+        self.base._repository.close()
 
-    def render(self, fps: int | None = None, hide_menu: bool = False) -> None:
+    def check_collisions(self, left_configurations: list[Configuration], right_configurations: list[Configuration]) -> tuple[np.ndarray, np.ndarray]:
         '''
-        a method to render the simulation and the configuration sliders
+        checks wether there are self collisions or environment collisions
 
         Parameters
         ----------
-        fps : int, optional
-            the fps of the simulation. None by default
-        '''
-        if not self.viewer.is_active:
-            self.viewer.init(self.controller.model, self.controller.data)
+        left_configurations : list[~.entities.Configuration]
+            the configurations of the left manipulator
 
-        if self.left_control_mode and not self.left_control_visualizer.is_active:
-            self.left_control_visualizer.init(self.controller.get_left_configuration().to_numpy())
+        right_configurations : list[~.entities.Configuration]
+            the configurations of the right manipulator
 
-        if self.right_control_mode and not self.right_control_visualizer.is_active:
-            self.right_control_visualizer.init(self.controller.get_right_configuration().to_numpy())
+        Returns
+        -------
+        out : tuple[np.ndarray, np.ndarray]
+            the first element is an array of the environment collisions and the second element is an array of the self collisions
 
-        self.left_control_visualizer.render(60)
-        self.right_control_visualizer.render(60)
-        self.viewer.render(fps, hide_menu)
+        Raises
+        ------
+        Exception
+            if the robot is not in simulation mode
+        '''
+        if self._mode != 'sim':
+            raise Exception('The check_collisions method is only available in simulation mode')
+
+        env_collisions: np.ndarray = np.zeros(len(left_configurations)).astype(bool)
+        self_collisions: np.ndarray = np.zeros(len(left_configurations)).astype(bool)
+        for i, (left_configuration, right_configuration) in enumerate(zip(left_configurations, right_configurations)):
+            self.left_manipulator.set_to(left_configuration)
+            self.right_manipulator.set_to(right_configuration)
 
-    def close(self) -> None:
-        '''
-        a method to close the rendering if any exists
-        '''
-        if self.viewer.is_active:
-            self.viewer.close()
+            info: AdamInfo = self.step()
 
-        if self.left_control_visualizer.is_active:
-            self.left_control_visualizer.close()
+            if info.left_manipulator.collision.env_collision or info.right_manipulator.collision.env_collision:
+                env_collisions[i] = True
 
-        if self.right_control_visualizer.is_active:
-            self.right_control_visualizer.close()
+            if info.left_manipulator.collision.self_collision or info.right_manipulator.collision.self_collision:
+                self_collisions[i] = True
+
+        return (env_collisions, self_collisions)
 
     @staticmethod
     def export_scene(destination: str) -> None:
         '''
         exports the default ADAM scene to a given directory
 
+        Parameters
+        ----------
         destination : str
             the directory in which to export the scene
 
         Notes
         -----
         Remember that the destination must end with '/'
         '''
-        filename = pkg_resources.resource_filename('adam', 'assets/')
-        copy_tree(filename, destination)
+        filename = pkg_resources.resource_filename('adam_sim', RESOURCE_FILE)
+        copy_tree(filename, destination + 'adam_scene/')
```

### Comparing `adam_sim-0.4.1/adam/features/simulation/use_cases/control_visualizer.py` & `adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/control_visualizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 from matplotlib.widgets import Slider
 
+from ....entities import Configuration
+
 
 GUTTER: float = 0.1
 MARGIN: float = 0.1
 WIDTH: float = 0.03
 TOP_SEP: float = 0.3
 
 
 class ControlVisualizer:
     def __init__(self, title: str) -> None:
         self.title: str = title
         self.is_active: bool = False
 
-    def init(self, initial_configuration: np.ndarray) -> None:
-        plt.ion()
-        self._load_viewer(initial_configuration)
-        self._load_values(initial_configuration)
+    def init(self, initial_configuration: Configuration) -> None:
+        if not self.is_active:
+            plt.ion()
+            self._load_viewer(initial_configuration)
+            self._load_values(initial_configuration)
 
-        self.is_active = True
+            self.is_active = True
 
-    def _load_viewer(self, initial_configuration: np.ndarray) -> None:
+    def _load_viewer(self, initial_configuration: Configuration) -> None:
         self.figure = plt.figure(frameon=False)
         self.figure.suptitle(self.title)
 
         # Axes
         q1_axes = self.figure.add_axes((MARGIN, 1.0-TOP_SEP, 1.0-MARGIN*2.5, WIDTH))
         q2_axes = self.figure.add_axes((MARGIN,  1.0-TOP_SEP-GUTTER, 1.0-MARGIN*2.5, WIDTH))
         q3_axes = self.figure.add_axes((MARGIN,  1.0-TOP_SEP-GUTTER*2.0, 1.0-MARGIN*2.5, WIDTH))
@@ -38,23 +41,23 @@
         self._q1_slider: Slider = Slider(ax=q1_axes, label=r'$\theta_1$', valmin=-np.pi, valmax=np.pi, valinit=initial_configuration[0], valstep=0.0001, color='#aecdd2', valfmt='%.4f')
         self._q2_slider: Slider = Slider(ax=q2_axes, label=r'$\theta_2$', valmin=-np.pi, valmax=np.pi, valinit=initial_configuration[1], valstep=0.0001, color='#aecdd2', valfmt='%.4f')
         self._q3_slider: Slider = Slider(ax=q3_axes, label=r'$\theta_3$', valmin=-np.pi, valmax=np.pi, valinit=initial_configuration[2], valstep=0.0001, color='#aecdd2', valfmt='%.4f')
         self._q4_slider: Slider = Slider(ax=q4_axes, label=r'$\theta_4$', valmin=-np.pi, valmax=np.pi, valinit=initial_configuration[3], valstep=0.0001, color='#aecdd2', valfmt='%.4f')
         self._q5_slider: Slider = Slider(ax=q5_axes, label=r'$\theta_5$', valmin=-np.pi, valmax=np.pi, valinit=initial_configuration[4], valstep=0.0001, color='#aecdd2', valfmt='%.4f')
         self._q6_slider: Slider = Slider(ax=q6_axes, label=r'$\theta_6$', valmin=-np.pi, valmax=np.pi, valinit=initial_configuration[5], valstep=0.0001, color='#aecdd2', valfmt='%.4f')
 
-    def _load_values(self, initial_configuration: np.ndarray) -> None:
+    def _load_values(self, initial_configuration: Configuration) -> None:
         self.q1: float = initial_configuration[0]
         self.q2: float = initial_configuration[1]
         self.q3: float = initial_configuration[2]
         self.q4: float = initial_configuration[3]
         self.q5: float = initial_configuration[4]
         self.q6: float = initial_configuration[5]
 
-    def get(self) -> np.ndarray:
+    def get(self) -> Configuration:
         def update(val):
             self.q1 = self._q1_slider.val
             self.q2 = self._q2_slider.val
             self.q3 = self._q3_slider.val
             self.q4 = self._q4_slider.val
             self.q5 = self._q5_slider.val
             self.q6 = self._q6_slider.val
@@ -62,17 +65,18 @@
         self._q1_slider.on_changed(update)
         self._q2_slider.on_changed(update)
         self._q3_slider.on_changed(update)
         self._q4_slider.on_changed(update)
         self._q5_slider.on_changed(update)
         self._q6_slider.on_changed(update)
 
-        return np.array([self.q1, self.q2, self.q3, self.q4, self.q5, self.q6])
+        return Configuration(self.q1, self.q2, self.q3, self.q4, self.q5, self.q6)
 
     def render(self, fps: int) -> None:
         if self.is_active:
             plt.draw()
             plt.pause(1.0/fps)
             self.figure.axes.clear()
 
     def close(self) -> None:
-        plt.close()
+        if self.is_active:
+            plt.close()
```

### Comparing `adam_sim-0.4.1/adam/features/simulation/use_cases/data_manager.py` & `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,71 @@
 import numpy as np
 
-from .collision_detector import CollisionDetector
-from ..entities import AdamInfo, ManipulatorData, Collision, Configuration, System, BaseData, Point, Vector
+from ....repository import ManipulatorRepository
+from ......entities import Configuration, Point, System, Velocity, Acceleration
+from ....entities import Collision, ManipulatorInfo
+from .use_cases import CollisionChecker
+
+
+class SimulatedLeftManipulatorRepository(ManipulatorRepository):
+    def init(self, data) -> None:
+        self.data = data
+
+        initial_configuration: Configuration = Configuration(1.5708, 0.58905, -0.098, -1.5708, 3.1415, 0.0)
+        self.data.qpos[0:6] = initial_configuration
+        self.data.ctrl[0:6] = initial_configuration
+
+    def set_configuration(self, configuration: Configuration) -> None:
+        self.data.qpos[0:6] = configuration
+
+    def get_configuration(self) -> Configuration:
+        return Configuration(*self.data.qpos[0:6])
+
+    def set_velocity(self, velocity: Velocity) -> None:
+        self.data.qvel[0:6] = velocity
+
+    def get_velocity(self) -> Velocity:
+        return Velocity(*self.data.qvel[0:6])
+
+    def set_acceleration(self, acceleration: Acceleration) -> None:
+        return super().set_acceleration(acceleration)
+
+    def get_acceleration(self) -> Acceleration:
+        return Acceleration(*self.data.qacc[0:6])
+
+    def get_collisions(self) -> Collision:
+        return CollisionChecker.get(self.data.contact.geom1, self.data.contact.geom2)
+
+    def get_systems(self) -> list[System]:
+        systems: list[System] = [System.from_htm(np.array([[*orientation[0:3], position[0]],
+                                                           [*orientation[3:6], position[1]],
+                                                           [*orientation[6:9], position[2]]]))
+                                 for orientation, position in zip(self.data.xmat[2:9], self.data.xpos[2:9])]
+
+        systems[1] = System(systems[1].position, systems[1].x_axis, -systems[1].z_axis, systems[1].y_axis)
+        system_2_position: Point = Point(*(systems[1].position + Point(*systems[1].x_axis) * 0.24365 * np.cos(self.data.qpos[1]) + Point(*systems[1].y_axis) * 0.24365 * np.sin(self.data.qpos[1])))
+        systems[2] = System(system_2_position, systems[2].z_axis, systems[2].x_axis, systems[2].y_axis)
+        system_3_position: Point = Point(*(systems[2].position + Point(*systems[2].x_axis) * 0.21325 * np.cos(self.data.qpos[2]) + Point(*systems[2].y_axis) * 0.21325 * np.sin(self.data.qpos[2])))
+        systems[3] = System(system_3_position, systems[3].z_axis, systems[3].x_axis, systems[3].y_axis)
+        systems[4] = System(systems[5].position, -systems[4].x_axis, -systems[4].y_axis, systems[4].z_axis)
+        systems[5] = System(systems[6].position, -systems[5].x_axis, systems[5].z_axis, systems[5].y_axis)
+        system_6_position: Point = Point(*(systems[5].position + Point(*systems[5].z_axis) * 0.0819))
+        systems[6] = System(system_6_position, -systems[6].x_axis, systems[6].z_axis, systems[6].y_axis)
+
+        return systems
+
+    def get_info(self) -> ManipulatorInfo:
+        collisions: Collision = self.get_collisions()
+        configuration: Configuration = self.get_configuration()
+        systems: list[System] = self.get_systems()
+        velocity: Velocity = self.get_velocity()
+        acceleration: Acceleration = self.get_acceleration()
+
+        return ManipulatorInfo(systems=systems,
+                               end_effector=systems[-1],
+                               configuration=configuration,
+                               velocity=velocity,
+                               acceleration=acceleration,
+                               collision=collisions)
 
-
-def _get_left_systems(data) -> list[System]:
-    systems: list[System] = [System.from_htm(np.array([[*orientation[0:3], position[0]],
-                                                       [*orientation[3:6], position[1]],
-                                                       [*orientation[6:9], position[2]]]))
-                             for orientation, position in zip(data.xmat[2:9], data.xpos[2:9])]
-
-    systems[1] = System(systems[1].position, systems[1].x_axis, -systems[1].z_axis, systems[1].y_axis)
-    systems[2] = System(systems[3].position, systems[2].z_axis, systems[2].x_axis, systems[2].y_axis)
-    systems[3] = System(systems[4].position, systems[3].z_axis, systems[3].x_axis, systems[3].y_axis)
-    systems[4] = systems[5]
-    systems[5] = System(systems[6].position, -systems[6].x_axis, systems[6].z_axis, systems[6].y_axis)
-
-    step_matrix: np.ndarray = np.array([[np.cos(data.qpos[5]), -np.sin(data.qpos[5]), 0.0, 0.0],
-                                        [np.sin(data.qpos[5]), np.cos(data.qpos[5]), 0.0, 0.0],
-                                        [0.0, 0.0, 1.0, 0.0819],
-                                        [0.0, 0.0, 0.0, 1.0]])
-
-    systems[6] = System.from_htm(systems[5].to_htm() @ step_matrix)
-
-    return systems
-
-
-def _get_right_systems(data) -> list[System]:
-    systems: list[System] = [System.from_htm(np.array([[*orientation[0:3], position[0]],
-                                                       [*orientation[3:6], position[1]],
-                                                       [*orientation[6:9], position[2]]]))
-                             for orientation, position in zip(data.xmat[9:], data.xpos[9:])]
-
-    systems[1] = System(systems[1].position, systems[1].x_axis, -systems[1].z_axis, systems[1].y_axis)
-    systems[2] = System(systems[3].position, systems[2].z_axis, systems[2].x_axis, systems[2].y_axis)
-    systems[3] = System(systems[4].position, systems[3].z_axis, systems[3].x_axis, systems[3].y_axis)
-    systems[4] = systems[5]
-    systems[5] = System(systems[6].position, -systems[6].x_axis, systems[6].z_axis, systems[6].y_axis)
-
-    step_matrix: np.ndarray = np.array([[np.cos(data.qpos[5]), -np.sin(data.qpos[5]), 0.0, 0.0],
-                                        [np.sin(data.qpos[5]), np.cos(data.qpos[5]), 0.0, 0.0],
-                                        [0.0, 0.0, 1.0, 0.0819],
-                                        [0.0, 0.0, 0.0, 1.0]])
-
-    systems[6] = System.from_htm(systems[5].to_htm() @ step_matrix)
-
-    return systems
-
-
-class DataManager:
-    def __init__(self) -> None:
-        self.collision_detector: CollisionDetector = CollisionDetector()
-
-    def get(self, data) -> AdamInfo:
-        # Configurations
-        left_configuration: Configuration = Configuration(*data.qpos[0:6])
-        right_configuration: Configuration = Configuration(*data.qpos[6:12])
-
-        # Collisions
-        left_collision: Collision = self.collision_detector.check_left_manipulator(data.contact.geom1, data.contact.geom2)
-        right_collision: Collision = self.collision_detector.check_right_manipulator(data.contact.geom1, data.contact.geom2)
-
-        # Systems
-        left_systems: list[System] = _get_left_systems(data)
-        right_systems: list[System] = _get_right_systems(data)
-
-        # Velocity
-        left_velocity: float = 0.0
-        right_velocity: float = 0.0
-
-        left_manipulator_data: ManipulatorData = ManipulatorData(left_collision, left_configuration, left_systems, left_velocity)
-        right_manipulator_data: ManipulatorData = ManipulatorData(right_collision, right_configuration, right_systems, right_velocity)
-
-        # Base
-        base_data: BaseData = BaseData(Point(0.0, 0.0, 0.0), Vector(0.0, 0.0, 0.0))
-
-        return AdamInfo(left_manipulator_data, right_manipulator_data, base_data)
+    def close(self) -> None:
+        return super().close()
```

### Comparing `adam_sim-0.4.1/adam/features/simulation/use_cases/viewer.py` & `adam_sim-1.0.0/adam_sim/features/adam/use_cases/viewer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from mujoco_viewer import MujocoViewer
+
 import time
 
 
 class Viewer:
     def __init__(self) -> None:
         self.is_active: bool = False
         self.hidden_menu: bool = False
 
     def init(self, model, data) -> None:
-        self.viewer: MujocoViewer = MujocoViewer(model, data, title='ADAM Simulator')
+        if not self.is_active:
+            self.viewer: MujocoViewer = MujocoViewer(model, data, title='ADAM Simulator')
 
-        self.set_view(center=(0.0, 0.0, 0.5),
-                      azimuth=-135.0,
-                      elevation=-20.0,
-                      distance=3.5,
-                      )
+            self.set_view(center=(0.0, 0.0, 0.5),
+                          azimuth=-135.0,
+                          elevation=-20.0,
+                          distance=3.5,
+                          )
 
-        self.is_active = True
+            self.is_active = True
 
-    def render(self, fps: int | None, hide_menu: bool) -> None:
+    def render(self, hide_menu: bool) -> None:
         if hide_menu and not self.hidden_menu:
             self.viewer._hide_menus = True
             self.hidden_menu = True
 
         self.viewer.render()
 
-        if fps is not None:
-            time.sleep(1.0/fps)
+        # TMP
+        time.sleep(1.0/60.0)
 
     def close(self) -> None:
-        self.viewer.close()
+        if self.is_active:
+            self.viewer.close()
 
     def set_view(self, center: tuple[float, float, float] | None, azimuth: float | None, elevation: float | None, distance: float | None) -> None:
         if center is not None:
             self.viewer.cam.lookat = center
 
         if azimuth is not None:
             self.viewer.cam.azimuth = azimuth
```

### Comparing `adam_sim-0.4.1/pyproject.toml` & `adam_sim-1.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adam_sim"
-version = "0.4.1"
-authors = [
-  { name="Vistor"},
-]
+version = "1.0.0"
+authors = [{ name = "Vistor" }]
 description = "A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 dependencies = [
-    "numpy",
-    "mujoco",
-    "mujoco-python-viewer",
-    "pyyaml",
-    "pandas",
-    "matplotlib",
+  "numpy",
+  "mujoco",
+  "mujoco-python-viewer",
+  "pyyaml",
+  "pandas",
+  "matplotlib",
+  "paho-mqtt",
+  "vclog",  
 ]
 
 [tool.setuptools.package-data]
-"*" = ["*.csv", "*.stl", "*.xml"]
+"*" = ["*.csv", "*.stl", "*.xml", "*.yaml"]
 
 [project.urls]
 "Homepage" = "https://github.com/vistormu/adam_simulator"
-"Bug Tracker" = "https://github.com/vistormu/adam_simulator/issues"
+"Bug Tracker" = "https://github.com/vistormu/adam_simulator/issues"
```

### Comparing `adam_sim-0.4.1/tests/test_1.py` & `adam_sim-1.0.0/tests/test_basic_usage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-from adam import Simulation
-from adam.entities import Configuration, AdamInfo
+from adam_sim import Adam
+from adam_sim.entities import Configuration, AdamInfo
 
 
 def main():
-    sim: Simulation = Simulation()
-    initial_info: AdamInfo = sim.load_scene()
+    adam: Adam = Adam()
+
+    initial_info: AdamInfo = adam.load()
 
     left_configuration: Configuration = initial_info.left_manipulator.configuration
     right_configuration: Configuration = initial_info.right_manipulator.configuration
 
-    for _ in range(100):
+    for _ in range(1000):
+        adam.render()
+
         left_configuration += Configuration(0.0, 0.0, 0.0, 0.0, 0.1, 0.0)
         right_configuration -= Configuration(0.0, 0.0, 0.0, 0.0, 0.1, 0.0)
 
-        sim.render(hide_menu=True)
-        info: AdamInfo = sim.step(left_configuration, right_configuration)
+        adam.right_manipulator.set_to(right_configuration)
+        adam.left_manipulator.set_to(left_configuration)
+
+        info: AdamInfo = adam.step()
 
-    sim.close()
+    adam.close()
 
 
 if __name__ == '__main__':
     main()
```

