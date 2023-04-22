# Comparing `tmp/chesscomwrapper-0.0.2.tar.gz` & `tmp/chesscomwrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chesscomwrapper-0.0.2.tar", last modified: Sat Apr 22 11:06:40 2023, max compression
+gzip compressed data, was "chesscomwrapper-0.0.3.tar", last modified: Sat Apr 22 11:11:09 2023, max compression
```

## Comparing `chesscomwrapper-0.0.2.tar` & `chesscomwrapper-0.0.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/chesscomwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/apimanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscountry.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessleaderboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessstreamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessteammatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesstournament.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesswrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/clubmember.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/clubprofile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/country/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/country/countryinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/dailypuzzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/noneerrorhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandlers/raisererrorhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerstats.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playerarchive.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playerclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playergames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playertournament.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.965160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/streamer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/streamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/streamer/chessstreamerinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentround.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/app/chesscomwrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/tests/test_chesswrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/app/chesscomwrapper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.961160 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 11:06:40.000000 chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:06:40.969160 chesscomwrapper-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-22 11:06:29.000000 chesscomwrapper-0.0.2/tests/test_chesswrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.985921 chesscomwrapper-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-22 11:11:09.985921 chesscomwrapper-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.973921 chesscomwrapper-0.0.3/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.977921 chesscomwrapper-0.0.3/app/chesscomwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.977921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/apimanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscountry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessleaderboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessstreamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessteammatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesstournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesswrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/club/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/club/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/club/clubmember.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/club/clubprofile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/country/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/country/countryinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/dailypuzzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/errorhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/errorhandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/errorhandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/errorhandlers/noneerrorhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/errorhandlers/raisererrorhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/leaderboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/leaderboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/chessplayerprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/chessplayerstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playerarchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playerclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playergames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playertournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/requesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/requesthandlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/requesthandlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/streamer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/streamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/streamer/chessstreamerinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.981921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/teammatchboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/teammatchinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.985921 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentround.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentroundgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentroundplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.985921 chesscomwrapper-0.0.3/app/chesscomwrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/tests/test_chesswrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/app/chesscomwrapper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.977921 chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-22 11:11:09.000000 chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-22 11:11:09.000000 chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 11:11:09.000000 chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 11:11:09.000000 chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 11:11:09.000000 chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 11:11:09.985921 chesscomwrapper-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 11:11:09.985921 chesscomwrapper-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-22 11:10:59.000000 chesscomwrapper-0.0.3/tests/test_chesswrapper.py
```

### Comparing `chesscomwrapper-0.0.2/LICENSE.txt` & `chesscomwrapper-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/apimanager.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/apimanager.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessclub.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessclub.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/archivehandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/clubhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/countryhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/dailypuzzlehandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/leaderboardshandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/playerhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/roundhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/roundinfohandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/streamerhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/teammatchboardhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/teammatchhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesscomhandlers/tournamenthandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessplayer.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessplayer.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chessstreamer.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chessstreamer.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/chesswrapper.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/chesswrapper.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/club/clubprofile.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/club/clubprofile.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/errorhandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/errorhandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/leaderboards/leaderboardsinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerprofile.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/chessplayerprofile.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/chessplayerstats.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/chessplayerstats.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playerarchive.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playerarchive.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playergames.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playergames.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/player/playertournament.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/player/playertournament.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/requesthandlers/singletonrequesthandler.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/teammatchboardinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/teammatch/teammatchinfo.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/teammatch/teammatchinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentinfo.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentround.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentround.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentroundgroupinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamentsettings.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamentsettings.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/src/tournament/tournamnetroundinfo.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper/tests/test_chesswrapper.py` & `chesscomwrapper-0.0.3/app/chesscomwrapper/tests/test_chesswrapper.py`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/app/chesscomwrapper.egg-info/SOURCES.txt` & `chesscomwrapper-0.0.3/app/chesscomwrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chesscomwrapper-0.0.2/setup.py` & `chesscomwrapper-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup(
     name='chesscomwrapper',
     version=__version__,
     description='A wrapper for the chess.com API',
     package_dir={'': 'app'},
     packages=find_packages(where='app'),
-    long_description="long_description",
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nicpanozzo/chesscom-api-wrapper',
     author='Nicola Panozzo',
     author_email='nicolapanoz@gmail.com',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `chesscomwrapper-0.0.2/tests/test_chesswrapper.py` & `chesscomwrapper-0.0.3/tests/test_chesswrapper.py`

 * *Files identical despite different names*

