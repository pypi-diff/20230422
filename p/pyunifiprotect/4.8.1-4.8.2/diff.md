# Comparing `tmp/pyunifiprotect-4.8.1.tar.gz` & `tmp/pyunifiprotect-4.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunifiprotect-4.8.1.tar", last modified: Mon Apr 17 03:07:52 2023, max compression
+gzip compressed data, was "pyunifiprotect-4.8.2.tar", last modified: Sat Apr 22 15:33:02 2023, max compression
```

## Comparing `pyunifiprotect-4.8.1.tar` & `pyunifiprotect-4.8.2.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.139799 pyunifiprotect-4.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/.bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.bin/format-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.bin/install-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/.bin/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.bin/lib/common.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.bin/lint-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.bin/test-code
--rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.bin/update-requirements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.111799 pyunifiprotect-4.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.github/workflows/test-live-AngellusMortis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/LIVE_DATA_CI.md
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-17 03:07:52.139799 pyunifiprotect-4.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/TESTDATA.md
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.119799 pyunifiprotect-4.8.1/docs/overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/docs/overrides/partials/toc-item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.123799 pyunifiprotect-4.8.1/pyunifiprotect/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47822 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.127799 pyunifiprotect-4.8.1/pyunifiprotect/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34254 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/cameras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/chimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/doorlocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/lights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/liveviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/cli/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.127799 pyunifiprotect-4.8.1/pyunifiprotect/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34536 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    72373 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/data/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/release_cache.json
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.127799 pyunifiprotect-4.8.1/pyunifiprotect/test_util/
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/test_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/test_util/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/pyunifiprotect/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.123799 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-17 03:07:52.000000 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-17 03:07:52.000000 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:07:52.000000 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 03:07:52.000000 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-17 03:07:52.000000 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 03:07:52.000000 pyunifiprotect-4.8.1/pyunifiprotect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 03:07:52.139799 pyunifiprotect-4.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.131799 pyunifiprotect-4.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.131799 pyunifiprotect-4.8.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_chime.py
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_doorlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_nvr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/data/test_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:52.135799 pyunifiprotect-4.8.1/tests/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_bootstrap.json
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_camera.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_camera_heatmap.png
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_camera_snapshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_camera_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_camera_video.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_chime.json
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_constants.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_doorlock.json
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_event_smart_track.json
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_light.json
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_liveview.json
--rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_raw_events.json
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_viewport.json
--rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/sample_data/sample_ws_messages.json
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/test_api_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/test_api_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-17 03:07:33.000000 pyunifiprotect-4.8.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/format-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      381 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/install-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.bin/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/lib/common.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/lint-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/test-code
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.bin/update-requirements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.388002 pyunifiprotect-4.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.github/workflows/test-live-AngellusMortis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.392002 pyunifiprotect-4.8.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/LIVE_DATA_CI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/TESTDATA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20591 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/docs/overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/docs/overrides/partials/toc-item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/pyunifiprotect/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47822 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.400002 pyunifiprotect-4.8.2/pyunifiprotect/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/chimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/doorlocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/liveviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/cli/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.400002 pyunifiprotect-4.8.2/pyunifiprotect/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34837 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72566 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33277 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/data/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/release_cache.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.404003 pyunifiprotect-4.8.2/pyunifiprotect/test_util/
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/test_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/test_util/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/pyunifiprotect/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.396002 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 15:33:02.000000 pyunifiprotect-4.8.2/pyunifiprotect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.404003 pyunifiprotect-4.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.404003 pyunifiprotect-4.8.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29621 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_chime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_doorlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_nvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11232 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/data/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:33:02.412003 pyunifiprotect-4.8.2/tests/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239461 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_bootstrap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_heatmap.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_snapshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50760 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_camera_video.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_chime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_constants.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_doorlock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_event_smart_track.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_light.json
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_liveview.json
+-rw-r--r--   0 runner    (1001) docker     (123)   854579 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_raw_events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_viewport.json
+-rw-r--r--   0 runner    (1001) docker     (123)   159864 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/sample_data/sample_ws_messages.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_api_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_api_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-22 15:32:46.000000 pyunifiprotect-4.8.2/tests/test_utils.py
```

### Comparing `pyunifiprotect-4.8.1/.bin/lib/common.sh` & `pyunifiprotect-4.8.2/.bin/lib/common.sh`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.bin/lint-code` & `pyunifiprotect-4.8.2/.bin/lint-code`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.bin/update-requirements` & `pyunifiprotect-4.8.2/.bin/update-requirements`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.devcontainer/devcontainer.json` & `pyunifiprotect-4.8.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.github/workflows/ci.yaml` & `pyunifiprotect-4.8.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.github/workflows/docker.yml` & `pyunifiprotect-4.8.2/.github/workflows/docker.yml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 env:
   DEFAULT_PYTHON: "3.11"
 
 jobs:
   docker:
     name: Build Docker Image
     runs-on: ubuntu-latest
+    environment:
+      name: release
+
     steps:
       - name: Check repo
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
```

### Comparing `pyunifiprotect-4.8.1/.github/workflows/docs.yml` & `pyunifiprotect-4.8.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.github/workflows/pypi.yml` & `pyunifiprotect-4.8.2/.github/workflows/pypi.yml`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,18 @@
   DEFAULT_PYTHON: "3.11"
 
 jobs:
 
   pypi:
     name: Publish to PyPi
     runs-on: ubuntu-latest
+    environment:
+      name: release
+    permissions:
+      id-token: write
 
     steps:
     - name: Check repo
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
@@ -41,11 +45,8 @@
         python -m pip install --upgrade pip
         pip install build
 
     - name: Build package
       run: python -m build
 
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
-      with:
-        user: __token__
-        password: ${{ secrets.PYPI_API_TOKEN }}
+      uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `pyunifiprotect-4.8.1/.github/workflows/test-live-AngellusMortis.yml` & `pyunifiprotect-4.8.2/.github/workflows/test-live-AngellusMortis.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.gitignore` & `pyunifiprotect-4.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.vscode/launch.json` & `pyunifiprotect-4.8.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/.vscode/tasks.json` & `pyunifiprotect-4.8.2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/Dockerfile` & `pyunifiprotect-4.8.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/LICENSE` & `pyunifiprotect-4.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/LIVE_DATA_CI.md` & `pyunifiprotect-4.8.2/LIVE_DATA_CI.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/PKG-INFO` & `pyunifiprotect-4.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.8.1
+Version: 4.8.2
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.8.1/README.md` & `pyunifiprotect-4.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/TESTDATA.md` & `pyunifiprotect-4.8.2/TESTDATA.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/dev-requirements.txt` & `pyunifiprotect-4.8.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/docs/api.md` & `pyunifiprotect-4.8.2/docs/api.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/docs/cli.md` & `pyunifiprotect-4.8.2/docs/cli.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/docs/dev.md` & `pyunifiprotect-4.8.2/docs/dev.md`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/mkdocs.yml` & `pyunifiprotect-4.8.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyproject.toml` & `pyunifiprotect-4.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/api.py` & `pyunifiprotect-4.8.2/pyunifiprotect/api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/__init__.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/backup.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/backup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             await conn.run_sync(Base.metadata.create_all)
 
 
 class EventTypeChoice(str, Enum):
     MOTION = d.EventType.MOTION.value
     RING = d.EventType.RING.value
     SMART_DETECT = d.EventType.SMART_DETECT.value
+    SMART_DETECT_LINE = d.EventType.SMART_DETECT_LINE.value
 
 
 class EventSmartType(Base):
     __tablename__ = "event_smart_type"
 
     id = Column(Integer, primary_key=True)
     event_id = Column(String(24), ForeignKey("event.id"), nullable=False)
@@ -177,15 +178,15 @@
                 camera_slug = camera.display_name.lower().replace(" ", ctx.seperator) + ctx.seperator
                 display_name = camera.display_name
             if self.end is not None:
                 length = self.end - self.start
 
             event_type = str(self.event_type)
             event_type_pretty = f"{event_type.title()} Event"
-            if event_type == d.EventType.SMART_DETECT.value:
+            if event_type in (d.EventType.SMART_DETECT.value, d.EventType.SMART_DETECT_LINE.value):
                 smart_types = list(self.smart_types)
                 smart_types.sort()
                 event_type = f"{event_type}[{','.join(smart_types)}]"
                 smart_types_title = [s.title() for s in smart_types]
                 event_type_pretty = f"Smart Detection ({', '.join(smart_types_title)})"
 
             start_local = local_datetime(self.start)
@@ -458,15 +459,15 @@
                 await aos.remove(thumb_path)
 
             event_path = event.get_event_path(ctx)
             if event_path.exists():
                 _LOGGER.debug("Delete file %s", event_path)
                 await aos.remove(event_path)
 
-            if event.event_type == d.EventType.SMART_DETECT:
+            if event.event_type in (d.EventType.SMART_DETECT.value, d.EventType.SMART_DETECT_LINE.value):
                 for smart_type in event.smart_detect_types:
                     await db.delete(smart_type)
             await db.delete(event)
             deleted += 1
         await db.commit()
 
     return deleted
@@ -486,15 +487,15 @@
             db_event = Event(id=event.id)
             do_insert = True
         db_event.start_naive = event.start
         db_event.end_naive = event.end
         db_event.camera_mac = event.camera.mac
         db_event.event_type = event.type.value
 
-        if event.type == d.EventType.SMART_DETECT:
+        if event.type in (d.EventType.SMART_DETECT.value, d.EventType.SMART_DETECT_LINE.value):
             types = {e.value for e in event.smart_detect_types}
 
             result = await db.execute(select(EventSmartType).where(EventSmartType.event_id == event.id))
             for event_smart_type in result.unique().scalars():
                 event_type = cast(EventSmartType, event_smart_type)
                 if event_type.smart_type not in types:
                     to_delete.append(event_type)
@@ -546,15 +547,15 @@
             pb.update(task_id, advance=progress)
             _LOGGER.debug("progress: +%s: %s/%s: %s %s", progress, task.completed, task.total, start, end)
 
             events = await ctx.protect.get_events(
                 start,
                 end,
                 limit=100,
-                types=[d.EventType.MOTION, d.EventType.RING, d.EventType.SMART_DETECT],
+                types=[d.EventType.MOTION, d.EventType.RING, d.EventType.SMART_DETECT, d.EventType.SMART_DETECT_LINE],
             )
 
             prev_start = start
             count = 0
             for event in events:
                 start = event.start
                 if event.id not in processed:
@@ -858,15 +859,15 @@
                     if length > ctx.length_cutoff:
                         _LOGGER.warning("Skipping event %s because it is too long (%s)", event.id, length)
                         await tasks.put(QueuedDownload(task=None, args=[]))
                         continue
                     # ensure no tasks are currently in a retry state
                     await no_error_flag.wait()
 
-                    if event.event_type == d.EventType.SMART_DETECT:
+                    if event.event_type in (d.EventType.SMART_DETECT.value, d.EventType.SMART_DETECT_LINE.value):
                         if not event.smart_types.intersection(smart_types_set):
                             continue
 
                     task = loop.create_task(_download_event(ctx, event, verify, force, pb))
                     # waits for a free processing slot
                     await tasks.put(QueuedDownload(task=task, args=[ctx, event, verify, force, pb]))
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/base.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/base.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/cameras.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/cameras.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/chimes.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/chimes.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/doorlocks.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/doorlocks.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/events.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     require_no_event_id(ctx)
     objs: dict[str, d.Event] = ctx.obj.events
     to_print: list[tuple[str, str, datetime]] = []
     longest_event = 0
     for obj in objs.values():
         event_type = obj.type.value
-        if event_type == d.EventType.SMART_DETECT:
+        if event_type in (d.EventType.SMART_DETECT.value, d.EventType.SMART_DETECT_LINE.value):
             event_type = f"{event_type}[{','.join(obj.smart_detect_types)}]"
         if len(event_type) > longest_event:
             longest_event = len(event_type)
         dt = obj.timestamp or obj.start
         dt = local_datetime(dt)
 
         to_print.append((obj.id, event_type, dt))
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/lights.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/lights.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/liveviews.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/liveviews.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/nvr.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/sensors.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/sensors.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/cli/viewers.py` & `pyunifiprotect-4.8.2/pyunifiprotect/cli/viewers.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/__init__.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/base.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
 import asyncio
 from datetime import datetime, timedelta
+from functools import cache
 from ipaddress import IPv4Address
 import logging
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
@@ -92,15 +93,16 @@
         """
         Base class for creating Python objects from UFP JSON data.
 
         Use the static method `.from_unifi_dict()` to create objects from UFP JSON data from then the main class constructor.
         """
         super().__init__(**data)
 
-        self._initial_data = self.dict(exclude=self._get_excluded_changed_fields())
+        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
+        self._initial_data = self.dict(exclude=excludes)
         self._api = api
 
     @classmethod
     def from_unifi_dict(cls, api: Optional[ProtectApiClient] = None, **data: Any) -> Self:
         """
         Main constructor for `ProtectBaseObject`
 
@@ -149,22 +151,24 @@
         obj = super().construct(_fields_set=_fields_set, **values)
         obj._initial_data = obj.dict(exclude=cls._get_excluded_changed_fields())  # pylint: disable=protected-access
         obj._api = api  # pylint: disable=protected-access
 
         return obj
 
     @classmethod
+    @cache
     def _get_excluded_changed_fields(cls) -> Set[str]:
         """
         Helper method for override in child classes for fields that excluded from calculating "changed" state for a
         model (`.initial_data` and `.get_changed()`)
         """
         return set()
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         """
         Helper method for overriding in child classes for remapping UFP JSON keys to Python ones that do not fit the
         simple camel case to snake case formula.
 
         Return format is
         {
@@ -493,20 +497,16 @@
 
         # Always injected above
         del data["api"]
 
         for key in data:
             setattr(self, key, convert_unifi_data(data[key], self.__fields__[key]))
 
-        # Calling dict with no params has a fast path which is MUCH faster
-        # so we pull out the excluded keys after
-        as_dict = self.dict()
-        for key in self._get_excluded_changed_fields().intersection(as_dict):
-            del as_dict[key]
-        self._initial_data = as_dict
+        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
+        self._initial_data = {k: v for k, v in self.__dict__.items() if k not in excludes}
         return self
 
     def get_changed(self) -> Dict[str, Any]:
         return dict_diff(self._initial_data, self.dict())
 
     @property
     def api(self) -> ProtectApiClient:
@@ -525,14 +525,15 @@
     Base class for UFP objects with a `modelKey` attr. Provides `.from_unifi_dict()` static helper method for
     automatically decoding a `modelKey` object into the correct UFP object and type
     """
 
     model: Optional[ModelType]
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "modelKey": "model"}
 
     def unifi_dict(self, data: Optional[Dict[str, Any]] = None, exclude: Optional[Set[str]] = None) -> Dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         if "modelKey" in data and data["modelKey"] is None:
@@ -657,22 +658,25 @@
                 raise BadRequest("Unknown model type")
 
             if not self.api.bootstrap.auth_user.can(self.model, PermissionNode.WRITE, self):
                 if revert_on_fail:
                     self.revert_changes()
                 raise NotAuthorized(f"Do not have write permission for obj: {self.id}")
 
-            new_data = self.dict(exclude=self._get_excluded_changed_fields())
+            excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
+            new_data = self.dict(exclude=excludes)
             updated = self.unifi_dict(data=self.get_changed())
 
             # do not patch when there are no updates
             if updated == {}:
                 return
 
-            read_only_keys = self._get_read_only_fields().intersection(updated.keys())
+            read_only_keys = self.__class__._get_read_only_fields().intersection(  # pylint: disable=protected-access
+                updated.keys()
+            )
             if len(read_only_keys) > 0:
                 self.revert_changes()
                 raise BadRequest(f"The following key(s) are read only: {read_only_keys}")
 
             try:
                 await self._api_update(updated)
             except ClientError:
@@ -725,14 +729,15 @@
     firmware_version: Optional[str]
     is_updating: bool
     is_ssh_enabled: bool
 
     _callback_ping: Optional[TimerHandle] = PrivateAttr(None)
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {
             "mac",
             "host",
             "type",
             "upSince",
             "uptime",
@@ -826,14 +831,15 @@
     bridge_id: Optional[str]
     is_downloading_firmware: Optional[bool]
 
     # TODO:
     # bridgeCandidates
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {
             "connectionHost",
             "connectedSince",
             "state",
             "latestFirmwareVersion",
             "firmwareBuild",
@@ -843,14 +849,15 @@
             "canAdopt",
             "isAttemptingToConnect",
             "bluetoothConnectionState",
             "isDownloadingFirmware",
         }
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "bridge": "bridgeId", "isDownloadingFW": "isDownloadingFirmware"}
 
     async def _api_update(self, data: Dict[str, Any]) -> None:
         if self.model is not None:
             return await self.api.update_device(self.model, self.id, data)
 
@@ -902,15 +909,16 @@
         """Verifies device is adopted and controlled by this NVR."""
 
         return self.is_adopted and not self.is_adopted_by_other
 
     def get_changed(self) -> Dict[str, Any]:
         """Gets dictionary of all changed fields"""
 
-        new_data = self.dict(exclude=self._get_excluded_changed_fields())
+        excludes = self.__class__._get_excluded_changed_fields()  # pylint: disable=protected-access
+        new_data = self.dict(exclude=excludes)
         updated = dict_diff(self._initial_data, new_data)
 
         return updated
 
     async def set_ssh(self, enabled: bool) -> None:
         """Sets ssh status for protect device"""
 
@@ -957,14 +965,15 @@
     last_motion: Optional[datetime]
     is_dark: bool
 
     # not directly from UniFi
     last_motion_event_id: Optional[str] = None
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {"lastMotion", "isDark"}
 
     def unifi_dict(self, data: Optional[Dict[str, Any]] = None, exclude: Optional[Set[str]] = None) -> Dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         if "lastMotionEventId" in data:
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/bootstrap.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     "recordingSchedules",
     "eventStats",
 }
 
 CAMERA_EVENT_ATTR_MAP: Dict[EventType, Tuple[str, str]] = {
     EventType.MOTION: ("last_motion", "last_motion_event_id"),
     EventType.SMART_DETECT: ("last_smart_detect", "last_smart_detect_event_id"),
+    EventType.SMART_DETECT_LINE: ("last_smart_detect", "last_smart_detect_event_id"),
     EventType.SMART_AUDIO_DETECT: ("last_smart_audio_detect", "last_smart_audio_detect_event_id"),
     EventType.RING: ("last_ring", "last_ring_event_id"),
 }
 
 
 def _remove_stats_keys(data: Dict[str, Any], ignore_stats: bool) -> Dict[str, Any]:
     if ignore_stats:
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/convert.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/devices.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
 from collections.abc import Iterable
 from datetime import datetime, timedelta
+from functools import cache
 from ipaddress import IPv4Address
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic.fields import PrivateAttr
@@ -110,18 +111,20 @@
     light_device_settings: LightDeviceSettings
     light_on_settings: LightOnSettings
     light_mode_settings: LightModeSettings
     camera_id: Optional[str]
     is_camera_paired: bool
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "camera": "cameraId"}
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {"isPirMotionDetected", "isLightOn", "isLocating"}
 
     @property
     def camera(self) -> Optional[Camera]:
         """Paired Camera will always be none if no camera is paired"""
 
@@ -493,14 +496,15 @@
     recording_end_lq: Optional[datetime]
     timelapse_start: Optional[datetime]
     timelapse_end: Optional[datetime]
     timelapse_start_lq: Optional[datetime]
     timelapse_end_lq: Optional[datetime]
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "recordingStartLQ": "recordingStartLq",
             "recordingEndLQ": "recordingEndLq",
             "timelapseStartLQ": "timelapseStartLq",
             "timelapseEndLQ": "timelapseEndLq",
@@ -633,14 +637,15 @@
 class HotplugExtender(ProtectBaseObject):
     has_flash: Optional[bool] = None
     has_ir: Optional[bool] = None
     has_radar: Optional[bool] = None
     is_attached: Optional[bool] = None
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "hasIR": "hasIr"}
 
 
 class Hotplug(ProtectBaseObject):
     audio: Optional[bool] = None
     video: Optional[bool] = None
@@ -709,14 +714,15 @@
         # backport support for `is_doorbell` to older versions of Protect
         if "hasChime" in data and "isDoorbell" not in data:
             data["isDoorbell"] = data["hasChime"]
 
         return super().unifi_dict_to_dict(data)
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "hasAutoICROnly": "hasAutoIcrOnly"}
 
     @property
     def has_highfps(self) -> bool:
         return VideoMode.HIGH_FPS in self.video_modes
 
@@ -812,29 +818,32 @@
     last_smart_audio_detect: Optional[datetime] = None
     last_smart_detect_event_id: Optional[str] = None
     last_smart_audio_detect_event_id: Optional[str] = None
     talkback_stream: Optional[TalkbackStream] = None
     _last_ring_timeout: Optional[datetime] = PrivateAttr(None)
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "is2K": "is2k", "is4K": "is4k"}
 
     @classmethod
+    @cache
     def _get_excluded_changed_fields(cls) -> Set[str]:
         return super()._get_excluded_changed_fields() | {
             "last_ring_event_id",
             "last_smart_detect",
             "last_smart_audio_detect",
             "last_smart_detect_event_id",
             "last_smart_audio_detect_event_id",
             "talkback_stream",
         }
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {
             "stats",
             "isDeleting",
             "isRecording",
             "isMotionDetected",
             "isSmartDetected",
@@ -1641,18 +1650,20 @@
 class Viewer(ProtectAdoptableDeviceModel):
     stream_limit: int
     software_version: str
     liveview_id: str
     anonymous_device_id: Optional[UUID] = None
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "liveview": "liveviewId"}
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {"softwareVersion"}
 
     @property
     def liveview(self) -> Optional[Liveview]:
         # user may not have permission to see the liveview
         return self.api.bootstrap.liveviews.get(self.liveview_id)
@@ -1736,18 +1747,20 @@
     last_value_event_id: Optional[str] = None
     last_alarm_event_id: Optional[str] = None
     extreme_value_detected_at: Optional[datetime] = None
     _tamper_timeout: Optional[datetime] = PrivateAttr(None)
     _alarm_timeout: Optional[datetime] = PrivateAttr(None)
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "camera": "cameraId"}
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {
             "batteryStatus",
             "isMotionDetected",
             "leakDetectedAt",
             "tamperingDetectedAt",
             "isOpened",
@@ -2014,18 +2027,20 @@
     led_settings: SensorSettingsBase
     battery_status: SensorBatteryStatus
     camera_id: Optional[str]
     has_homekit: bool
     private_token: str
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "camera": "cameraId", "autoCloseTimeMs": "autoCloseTime"}
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {"credentials", "lockStatus", "batteryStatus"}
 
     @classmethod
     def unifi_dict_to_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if "autoCloseTimeMs" in data and not isinstance(data["autoCloseTimeMs"], timedelta):
             data["autoCloseTimeMs"] = timedelta(milliseconds=data["autoCloseTimeMs"])
@@ -2114,14 +2129,15 @@
 
     # TODO: used for adoption
     # apMac  read only
     # apRssi  read only
     # elementInfo  read only
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {"isProbingForWifi", "lastRing"}
 
     @property
     def cameras(self) -> List[Camera]:
         """Paired Cameras for chime"""
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/nvr.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/nvr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """UniFi Protect Data."""
 from __future__ import annotations
 
 from datetime import datetime, timedelta, tzinfo
+from functools import cache
 from ipaddress import IPv4Address
 import logging
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
@@ -76,14 +77,15 @@
     level: PercentInt
     coord: Tuple[int, int, int, int]
     object_type: SmartDetectObjectType
     zone_ids: List[int]
     duration: timedelta
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "zones": "zoneIds",
         }
 
     @classmethod
@@ -97,14 +99,15 @@
 class SmartDetectTrack(ProtectBaseObject):
     id: str
     payload: List[SmartDetectItem]
     camera_id: str
     event_id: str
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "camera": "cameraId",
             "event": "eventId",
         }
 
@@ -157,14 +160,15 @@
         "status",
         "alarmType",
         "deviceId",
         "mac",
     }
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "from": "fromValue",
             "to": "toValue",
         }
 
@@ -214,14 +218,15 @@
     # description
 
     _smart_detect_events: Optional[List[Event]] = PrivateAttr(None)
     _smart_detect_track: Optional[SmartDetectTrack] = PrivateAttr(None)
     _smart_detect_zones: Optional[Dict[int, CameraZone]] = PrivateAttr(None)
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "camera": "cameraId",
             "heatmap": "heatmapId",
             "user": "userId",
             "thumbnail": "thumbnailId",
@@ -347,15 +352,15 @@
     async def get_smart_detect_track(self) -> SmartDetectTrack:
         """
         Gets smart detect track for given smart detect event.
 
         If event is not a smart detect event, it will raise a `BadRequest`
         """
 
-        if self.type != EventType.SMART_DETECT:
+        if self.type not in (EventType.SMART_DETECT, EventType.SMART_DETECT_LINE):
             raise BadRequest("Not a smart detect event")
 
         if self._smart_detect_track is None:
             self._smart_detect_track = await self.api.get_event_smart_detect_track(self.id)
 
         return self._smart_detect_track
 
@@ -398,14 +403,15 @@
     ucore: int
     discovery_client: int
     piongw: Optional[int] = None
     ems_json_cli: Optional[int] = None
     stacking: Optional[int] = None
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "emsCLI": "emsCli",
             "emsLiveFLV": "emsLiveFlv",
             "emsJsonCLI": "emsJsonCli",
         }
@@ -483,14 +489,15 @@
     life_span: Optional[PercentFloat] = None
     bad_sector: Optional[int] = None
     threshold: Optional[int] = None
     progress: Optional[PercentFloat] = None
     estimate: Optional[timedelta] = None
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "poweronhrs": "powerOnHours",
             "life_span": "lifeSpan",
             "bad_sector": "badSector",
         }
@@ -557,14 +564,15 @@
     action: str
     progress: Optional[PercentFloat] = None
     estimate: Optional[timedelta] = None
     # requires 2.8.14+
     health: Optional[str] = None
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "total_bytes": "totalBytes",
             "used_bytes": "usedBytes",
         }
 
@@ -614,14 +622,15 @@
 class DoorbellSettings(ProtectBaseObject):
     default_message_text: DoorbellText
     default_message_reset_timeout: timedelta
     all_messages: List[DoorbellMessage]
     custom_messages: List[DoorbellText]
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "defaultMessageResetTimeoutMs": "defaultMessageResetTimeout"}
 
     @classmethod
     def unifi_dict_to_dict(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if "defaultMessageResetTimeoutMs" in data:
             data["defaultMessageResetTimeout"] = timedelta(milliseconds=data.pop("defaultMessageResetTimeoutMs"))
@@ -789,22 +798,24 @@
     # wifiSettings
     # smartDetectAgreement
     # dbRecoveryOptions
     # globalCameraSettings
     # portStatus
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {
             **super()._get_unifi_remaps(),
             "recordingRetentionDurationMs": "recordingRetentionDuration",
             "vaultCameras": "vaultCameraIds",
         }
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {
             "version",
             "uiVersion",
             "hardwarePlatform",
             "ports",
             "lastUpdateAt",
@@ -990,14 +1001,15 @@
     camera_ids: List[str]
     cycle_mode: str
     cycle_interval: int
 
     _cameras: Optional[List[Camera]] = PrivateAttr(None)
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "cameras": "cameraIds"}
 
     @property
     def cameras(self) -> List[Camera]:
         if self._cameras is not None:
             return self._cameras
@@ -1012,18 +1024,20 @@
     is_default: bool
     is_global: bool
     layout: int
     slots: List[LiveviewSlot]
     owner_id: str
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "owner": "ownerId"}
 
     @classmethod
+    @cache
     def _get_read_only_fields(cls) -> Set[str]:
         return super()._get_read_only_fields() | {"isDefault", "owner"}
 
     @property
     def owner(self) -> Optional[User]:
         """
         Owner of liveview.
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/types.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/types.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/user.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """UniFi Protect User models."""
 from __future__ import annotations
 
 from datetime import datetime
+from functools import cache
 from typing import Any, Dict, List, Optional, Set
 
 from pydantic.fields import PrivateAttr
 
 from pyunifiprotect.data.base import ProtectBaseObject, ProtectModel, ProtectModelWithId
 from pyunifiprotect.data.types import ModelType, PermissionNode
 
@@ -78,14 +79,15 @@
     email: str
     user_id: str
     name: str
     location: Optional[UserLocation]
     profile_img: Optional[str] = None
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "user": "userId"}
 
     def unifi_dict(self, data: Optional[Dict[str, Any]] = None, exclude: Optional[Set[str]] = None) -> Dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         # id and cloud ID are always the same
@@ -150,14 +152,15 @@
         if "allPermissions" in data:
             permissions = data.pop("allPermissions")
             data["allPermissions"] = [{"rawPermission": p} for p in permissions]
 
         return super().unifi_dict_to_dict(data)
 
     @classmethod
+    @cache
     def _get_unifi_remaps(cls) -> Dict[str, str]:
         return {**super()._get_unifi_remaps(), "groups": "groupIds"}
 
     def unifi_dict(self, data: Optional[Dict[str, Any]] = None, exclude: Optional[Set[str]] = None) -> Dict[str, Any]:
         data = super().unifi_dict(data=data, exclude=exclude)
 
         if "location" in data and data["location"] is None:
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/data/websocket.py` & `pyunifiprotect-4.8.2/pyunifiprotect/data/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/exceptions.py` & `pyunifiprotect-4.8.2/pyunifiprotect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/stream.py` & `pyunifiprotect-4.8.2/pyunifiprotect/stream.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/test_util/__init__.py` & `pyunifiprotect-4.8.2/pyunifiprotect/test_util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/test_util/anonymize.py` & `pyunifiprotect-4.8.2/pyunifiprotect/test_util/anonymize.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/utils.py` & `pyunifiprotect-4.8.2/pyunifiprotect/utils.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect/websocket.py` & `pyunifiprotect-4.8.2/pyunifiprotect/websocket.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect.egg-info/PKG-INFO` & `pyunifiprotect-4.8.2/pyunifiprotect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyunifiprotect
-Version: 4.8.1
+Version: 4.8.2
 Summary: Unofficial UniFi Protect Python API and CLI
 Author-email: Bjarne Riis <bjarne@briis.com>, Christopher Bailey <cbailey@mort.is>
 Maintainer-email: Christopher Bailey <cbailey@mort.is>, "J. Nick Koston" <nick@koston.org>
 License: MIT
 Project-URL: Source Code, https://github.com/AngellusMortis/pyunifiprotect/
 Project-URL: Documentation, https://angellusmortis.github.io/pyunifiprotect/latest/
 Project-URL: Bug Reports, https://github.com/AngellusMortis/pyunifiprotect/issues/
```

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect.egg-info/SOURCES.txt` & `pyunifiprotect-4.8.2/pyunifiprotect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/pyunifiprotect.egg-info/requires.txt` & `pyunifiprotect-4.8.2/pyunifiprotect.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/requirements.txt` & `pyunifiprotect-4.8.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/conftest.py` & `pyunifiprotect-4.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_camera.py` & `pyunifiprotect-4.8.2/tests/data/test_camera.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_chime.py` & `pyunifiprotect-4.8.2/tests/data/test_chime.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_common.py` & `pyunifiprotect-4.8.2/tests/data/test_common.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_doorlock.py` & `pyunifiprotect-4.8.2/tests/data/test_doorlock.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_light.py` & `pyunifiprotect-4.8.2/tests/data/test_light.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_nvr.py` & `pyunifiprotect-4.8.2/tests/data/test_nvr.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_sensor.py` & `pyunifiprotect-4.8.2/tests/data/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/data/test_viewer.py` & `pyunifiprotect-4.8.2/tests/data/test_viewer.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/constants.py` & `pyunifiprotect-4.8.2/tests/sample_data/constants.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_bootstrap.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_bootstrap.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_bridge.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_bridge.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_camera.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_camera.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_camera_heatmap.png` & `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_heatmap.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_camera_snapshot.png` & `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_snapshot.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_camera_thumbnail.png` & `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_thumbnail.png`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_camera_video.mp4` & `pyunifiprotect-4.8.2/tests/sample_data/sample_camera_video.mp4`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_chime.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_chime.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_constants.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_constants.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_doorlock.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_doorlock.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_event_smart_track.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_event_smart_track.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_light.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_light.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_liveview.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_liveview.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_raw_events.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_raw_events.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_sensor.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_sensor.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_viewport.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_viewport.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/sample_data/sample_ws_messages.json` & `pyunifiprotect-4.8.2/tests/sample_data/sample_ws_messages.json`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/test_api.py` & `pyunifiprotect-4.8.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/test_api_polling.py` & `pyunifiprotect-4.8.2/tests/test_api_polling.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/test_api_ws.py` & `pyunifiprotect-4.8.2/tests/test_api_ws.py`

 * *Files identical despite different names*

### Comparing `pyunifiprotect-4.8.1/tests/test_utils.py` & `pyunifiprotect-4.8.2/tests/test_utils.py`

 * *Files identical despite different names*

