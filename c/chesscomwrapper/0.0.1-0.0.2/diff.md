# Comparing `tmp/chesscomwrapper-0.0.1.tar.gz` & `tmp/chesscomwrapper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscomwrapper-0.0.1.tar", last modified: Sat Apr 22 10:20:58 2023, max compression
+gzip compressed data, was "chesscomwrapper-0.0.2.tar", last modified: Sat Apr 22 11:06:40 2023, max compression
```

## Comparing `chesscomwrapper-0.0.1.tar` & `chesscomwrapper-0.0.2.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.621225 chesscomwrapper-0.0.1/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1076 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/LICENSE.txt
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      533 2023-04-22 10:20:58.620751 chesscomwrapper-0.0.1/PKG-INFO
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.575281 chesscomwrapper-0.0.1/app/
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.579969 chesscomwrapper-0.0.1/app/chesscomwrapper/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)       90 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/__init__.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.591754 chesscomwrapper-0.0.1/app/chesscomwrapper/src/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      633 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/apimanager.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      515 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessclub.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1902 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandler.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.598936 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1166 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1592 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1484 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1295 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      822 2023-04-19 13:20:32.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     3735 2023-04-20 16:37:11.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      740 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      764 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      841 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      739 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      719 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     2204 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      436 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscountry.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      445 2023-04-19 13:20:36.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessleaderboards.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     2505 2023-04-20 17:05:54.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessplayer.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      763 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessstreamer.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      250 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessteammatch.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      322 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesstournament.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1785 2023-04-20 16:26:00.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesswrapper.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.600564 chesscomwrapper-0.0.1/app/chesscomwrapper/src/club/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/club/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      189 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/club/clubmember.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      793 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/club/clubprofile.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.601621 chesscomwrapper-0.0.1/app/chesscomwrapper/src/country/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/country/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      187 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/country/countryinfo.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      492 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/dailypuzzle.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     2159 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/errorhandler.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.603527 chesscomwrapper-0.0.1/app/chesscomwrapper/src/errorhandlers/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/errorhandlers/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      377 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/errorhandlers/noneerrorhandler.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      210 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/errorhandlers/raisererrorhandler.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.604559 chesscomwrapper-0.0.1/app/chesscomwrapper/src/leaderboards/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/leaderboards/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     3042 2023-04-19 13:26:03.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.609400 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      865 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/chessplayerprofile.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     2947 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/chessplayerstats.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      577 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playerarchive.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      235 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playerclub.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1362 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playergames.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1981 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playertournament.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      280 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/requesthandler.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.610298 chesscomwrapper-0.0.1/app/chesscomwrapper/src/requesthandlers/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/requesthandlers/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1777 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.611276 chesscomwrapper-0.0.1/app/chesscomwrapper/src/streamer/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/streamer/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      413 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/streamer/chessstreamerinfo.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.613613 chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      275 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/teammatchboard.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      643 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     2210 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/teammatchinfo.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.618842 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      833 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentinfo.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      167 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentplayer.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      622 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentround.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      267 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentroundgroup.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     5322 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      276 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentroundplayer.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     1179 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentsettings.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      547 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.620095 chesscomwrapper-0.0.1/app/chesscomwrapper/tests/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        0 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/tests/__init__.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)    16356 2023-04-20 16:39:40.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/tests/test_chesswrapper.py
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)       19 2023-04-19 13:12:48.000000 chesscomwrapper-0.0.1/app/chesscomwrapper/version.py
-drwxr-xr-x   0 nicolapanozzo   (501) staff       (20)        0 2023-04-22 10:20:58.582621 chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      533 2023-04-22 10:20:58.000000 chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/PKG-INFO
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)     3485 2023-04-22 10:20:58.000000 chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)        1 2023-04-22 10:20:58.000000 chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)       42 2023-04-22 10:20:58.000000 chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/requires.txt
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)       16 2023-04-22 10:20:58.000000 chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/top_level.txt
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)       38 2023-04-22 10:20:58.621361 chesscomwrapper-0.0.1/setup.cfg
--rw-r--r--   0 nicolapanozzo   (501) staff       (20)      910 2023-04-19 13:12:47.000000 chesscomwrapper-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/chesscomwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/apimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscountry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessleaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessstreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessteammatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesstournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesswrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/clubmember.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/clubprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/country/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/country/countryinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/dailypuzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/noneerrorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/raisererrorhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playerarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playerclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playergames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playertournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/streamer/chessstreamerinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentround.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/app/chesscomwrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/tests/test_chesswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/tests/test_chesswrapper.py
```

### Comparing `chesscomwrapper-0.0.1/LICENSE.txt` & `chesscomwrapper-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/apimanager.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/apimanager.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessclub.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessclub.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessplayer.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessplayer.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chessstreamer.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessstreamer.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/chesswrapper.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesswrapper.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/club/clubprofile.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/clubprofile.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/errorhandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/chessplayerprofile.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerprofile.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/chessplayerstats.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerstats.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playerarchive.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playerarchive.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playergames.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playergames.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/player/playertournament.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playertournament.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/teammatch/teammatchinfo.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentinfo.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentround.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentround.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamentsettings.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentsettings.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper/tests/test_chesswrapper.py` & `chesscomwrapper-0.0.2/app/chesscomwrapper/tests/test_chesswrapper.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.1/app/chesscomwrapper.egg-info/SOURCES.txt` & `chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.txt
+README.md
 setup.py
 app/chesscomwrapper/__init__.py
 app/chesscomwrapper/version.py
 app/chesscomwrapper.egg-info/PKG-INFO
 app/chesscomwrapper.egg-info/SOURCES.txt
 app/chesscomwrapper.egg-info/dependency_links.txt
 app/chesscomwrapper.egg-info/requires.txt
@@ -65,8 +66,9 @@
 app/chesscomwrapper/src/tournament/tournamentround.py
 app/chesscomwrapper/src/tournament/tournamentroundgroup.py
 app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py
 app/chesscomwrapper/src/tournament/tournamentroundplayer.py
 app/chesscomwrapper/src/tournament/tournamentsettings.py
 app/chesscomwrapper/src/tournament/tournamnetroundinfo.py
 app/chesscomwrapper/tests/__init__.py
-app/chesscomwrapper/tests/test_chesswrapper.py
+app/chesscomwrapper/tests/test_chesswrapper.py
+tests/test_chesswrapper.py
```

### Comparing `chesscomwrapper-0.0.1/setup.py` & `chesscomwrapper-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
-with open('app/chesscomwrapper/README.md') as f:
+with open('README.md') as f:
     long_description = f.read()
 
 exec(open('app/chesscomwrapper/version.py').read())
 
 setup(
     name='chesscomwrapper',
     version=__version__,
     description='A wrapper for the chess.com API',
     package_dir={'': 'app'},
     packages=find_packages(where='app'),
-    long_description=long_description,
+    long_description="long_description",
     long_description_content_type='text/markdown',
     url='https://github.com/nicpanozzo/chesscom-api-wrapper',
     author='Nicola Panozzo',
     author_email='nicolapanoz@gmail.com',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

