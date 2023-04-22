# Comparing `tmp/spotify_to_ytmusic-0.1.3.tar.gz` & `tmp/spotify_to_ytmusic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_ytmusic-0.1.3.tar", last modified: Tue Apr 18 21:04:33 2023, max compression
+gzip compressed data, was "spotify_to_ytmusic-0.1.4.tar", last modified: Sat Apr 22 07:01:23 2023, max compression
```

## Comparing `spotify_to_ytmusic-0.1.3.tar` & `spotify_to_ytmusic-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.246796 spotify_to_ytmusic-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.250796 spotify_to_ytmusic-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.250796 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/settings.ini.example
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/tests/test_spotipy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.429120 spotify_to_ytmusic-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.433120 spotify_to_ytmusic-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.433120 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/settings.ini.example
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.433120 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/tests/test_spotipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.1.3/.github/workflows/coverage.yml` & `spotify_to_ytmusic-0.1.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/.github/workflows/pythonpublish.yml` & `spotify_to_ytmusic-0.1.4/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/.gitignore` & `spotify_to_ytmusic-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/LICENSE` & `spotify_to_ytmusic-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/PKG-INFO` & `spotify_to_ytmusic-0.1.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_to_ytmusic
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spotify_to_ytmusic-0.1.3/README.rst` & `spotify_to_ytmusic-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/pyproject.toml` & `spotify_to_ytmusic-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/controllers.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/controllers.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/main.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/main.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/match.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/match.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/settings.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/settings.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/setup.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     settings["youtube"]["headers"] = json.dumps(ytmusicapi.setup_oauth())
     settings.save()
 
 
 def setup_spotify():
     settings = Settings()
     credentials = {
-        "client_credentials": input(
-            "Paste your client credentials from the Spotify developer dashboard:"
+        "client_id": input(
+            "Paste your client id from the Spotify developer dashboard:"
         ),
-        "client_secrets": input("Paste your client secret from the Spotify developer dashboard:"),
+        "client_secret": input("Paste your client secret from the Spotify developer dashboard:"),
     }
     settings["spotify"].update(credentials)
     settings.save()
 
 
 def setup_file(file: Path):
     if not file:
```

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/spotify.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/spotify.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/ytmusic.py` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/PKG-INFO` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-to-ytmusic
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/SOURCES.txt` & `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.3/tests/test_cli.py` & `spotify_to_ytmusic-0.1.4/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import shutil
 import time
 import unittest
 from io import StringIO
 from pathlib import Path
 from unittest import mock
 
@@ -23,38 +24,46 @@
         self.assertEqual(len(vars(args)), 3)
 
     def test_create(self):
         with mock.patch("sys.argv", ["", "all", "sigmatics"]):
             main()
 
         with mock.patch(
-            "sys.argv", ["", "create", TEST_PLAYLIST, "-n", "test", "-i", "test-playlist", "-d"]
+            "sys.argv", ["", "create", TEST_PLAYLIST, "-n", "spotify_to_ytmusic", "-i", "test-playlist", "-d"]
         ):
             main()
 
         time.sleep(2)
-        with mock.patch("sys.argv", ["", "update", TEST_PLAYLIST, "test"]):
+        with mock.patch("sys.argv", ["", "update", TEST_PLAYLIST, "spotify_to_ytmusic"]):
             main()
 
         time.sleep(2)
-        with mock.patch("sys.argv", ["", "remove", "test"]), mock.patch(
+        with mock.patch("sys.argv", ["", "remove", "spotify\_to\_ytmusic"]), mock.patch(
             "sys.stdout", new=StringIO()
         ) as fakeOutput, mock.patch("builtins.input", side_effect="y"):
             main()
             assert (
                 int(fakeOutput.getvalue().splitlines()[-1][0]) >= 2
             )  # assert number of lines deleted
 
     def test_setup(self):
         tmp_path = Path(__file__).parent.joinpath("settings.tmp")
         example_path = Settings.filepath.parent.joinpath("settings.ini.example")
         shutil.copy(example_path, tmp_path)
-        with mock.patch("sys.argv", ["", "setup"]), mock.patch("builtins.input", return_value="3"):
+        with mock.patch("sys.argv", ["", "setup"]), mock.patch(
+            "builtins.input", return_value="3"
+        ), mock.patch(
+            "ytmusicapi.auth.oauth.YTMusicOAuth.get_token_from_code",
+            return_value=json.loads(Settings()["youtube"]["headers"]),
+        ):
             main()
             assert tmp_path.is_file()
+            settings = Settings()
+            assert settings["spotify"]["client_id"] == "3"
+            assert settings["spotify"]["client_secret"] == "3"
             tmp_path.unlink()
 
         with mock.patch("sys.argv", ["", "setup", "--file", example_path.as_posix()]), mock.patch(
             "spotify_to_ytmusic.settings.Settings.filepath", tmp_path
         ):
             main()
             assert tmp_path.is_file()
```

### Comparing `spotify_to_ytmusic-0.1.3/tests/test_spotipy.py` & `spotify_to_ytmusic-0.1.4/tests/test_spotipy.py`

 * *Files identical despite different names*

