# Comparing `tmp/chesscomwrapper-0.0.6.tar.gz` & `tmp/chesscomwrapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscomwrapper-0.0.6.tar", last modified: Sat Apr 22 17:01:02 2023, max compression
+gzip compressed data, was "chesscomwrapper-0.0.8.tar", last modified: Sat Apr 22 17:26:33 2023, max compression
```

## Comparing `chesscomwrapper-0.0.6.tar` & `chesscomwrapper-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.460727 chesscomwrapper-0.0.6/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.464727 chesscomwrapper-0.0.6/app/chesscomwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/app/chesscomwrapper/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/apimanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessclub.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesscountry.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessleaderboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessstreamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessteammatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesstournament.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/dailypuzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/lazy_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/playerarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/teammatchboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/tournamentround.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/src/tournamentroundgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/app/chesscomwrapper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.464727 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 17:01:02.000000 chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:01:02.468727 chesscomwrapper-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-22 17:00:46.000000 chesscomwrapper-0.0.6/tests/test_chesswrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.636775 chesscomwrapper-0.0.8/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.636775 chesscomwrapper-0.0.8/app/chesscomwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.640775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/apimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesscountry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessleaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessstreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessteammatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesstournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/dailypuzzle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.640775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/archivehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/clubhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/countryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/dailypuzzlehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/leaderboardshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/playerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/roundhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/roundinfohandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/streamerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchboardhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/teammatchhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/chesscomhandlers/tournamenthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/noneerrorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/errorhandlers/raisererrorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/handlers/requesthandlers/singletonrequesthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/lazy_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/clubmember.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/club/clubprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/country/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/country/countryinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/leaderboards/leaderboardsinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/chessplayerprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/chessplayerstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playerclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playergames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/playertournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/player/titledcategory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/puzzle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/puzzle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/puzzle/puzzleinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.644775 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/streamer/chessstreamerinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/teammatchboardinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/teammatch/teammatchinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentroundgroupinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentroundplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamentsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/models/tournament/tournamnetroundinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/playerarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/teammatchboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/tournamentround.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/src/tournamentroundgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/app/chesscomwrapper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.640775 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 17:26:33.000000 chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:26:33.648776 chesscomwrapper-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-04-22 17:26:18.000000 chesscomwrapper-0.0.8/tests/test_chesswrapper.py
```

### Comparing `chesscomwrapper-0.0.6/LICENSE.txt` & `chesscomwrapper-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.6/PKG-INFO` & `chesscomwrapper-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscomwrapper
-Version: 0.0.6
+Version: 0.0.8
 Summary: A wrapper for the chess.com API
 Home-page: https://github.com/nicpanozzo/chesscom-api-wrapper
 Author: Nicola Panozzo
 Author-email: nicolapanoz@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper/src/apimanager.py` & `chesscomwrapper-0.0.8/app/chesscomwrapper/src/apimanager.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessclub.py` & `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessclub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from app.chesscomwrapper.src.lazy_decorator import lazy_property
 from .models.player.playerclub import PlayerClub
 from .models.club.clubmember import ClubMember
 from .handlers.chesscomhandlers.clubhandler import ClubHandler
 import functools
 
 
 class Club(object):
```

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesscountry.py` & `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesscountry.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from app.chesscomwrapper.src.lazy_decorator import lazy_property
 from .handlers.chesscomhandlers.countryhandler import CountryHandler
 import functools
 
 
 class ChessCountry(object):
     def __init__(self, abbr, lazy = True) -> None:
         self.code = abbr
```

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chessplayer.py` & `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chessplayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Optional
 
 from .models.player.titledcategory import TitledCategory
 
 from .models.player.playerclub import PlayerClub
 
 from .models.player.playertournament import PlayerTournaments
-from .lazy_decorator import lazy_property
 from .playerarchive import PlayerArchive
 from .handlers.chesscomhandlers.playerhandler import PlayerHandler
 from .models.player.chessplayerstats import ChessPlayerStats
 from .models.player.chessplayerprofile import ChessPlayerProfile
 from .models.player.playergames import ChesscomGame, ChesscomGameToMove
 # from chesswrapper.chessplayerstats import ChessPlayerStats
 # from chessplayerprofile import ChessPlayerProfile
```

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper/src/chesswrapper.py` & `chesscomwrapper-0.0.8/app/chesscomwrapper/src/chesswrapper.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper/src/playerarchive.py` & `chesscomwrapper-0.0.8/app/chesscomwrapper/src/playerarchive.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.6/app/chesscomwrapper.egg-info/PKG-INFO` & `chesscomwrapper-0.0.8/app/chesscomwrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chesscomwrapper
-Version: 0.0.6
+Version: 0.0.8
 Summary: A wrapper for the chess.com API
 Home-page: https://github.com/nicpanozzo/chesscom-api-wrapper
 Author: Nicola Panozzo
 Author-email: nicolapanoz@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chesscomwrapper-0.0.6/setup.py` & `chesscomwrapper-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.6/tests/test_chesswrapper.py` & `chesscomwrapper-0.0.8/tests/test_chesswrapper.py`

 * *Files identical despite different names*

