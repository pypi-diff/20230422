# Comparing `tmp/python-cowsay-1.0.2.tar.gz` & `tmp/python-cowsay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-cowsay-1.0.2.tar", last modified: Sat Feb 25 21:30:46 2023, max compression
+gzip compressed data, was "python-cowsay-1.1.0.tar", last modified: Sat Apr 22 02:58:39 2023, max compression
```

## Comparing `python-cowsay-1.0.2.tar` & `python-cowsay-1.1.0.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-25 21:30:46.252569 python-cowsay-1.0.2/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/LICENSE
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       40 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/MANIFEST.in
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4675 2023-02-25 21:30:46.252439 python-cowsay-1.0.2/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     2905 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/README.md
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      708 2023-02-25 21:27:40.000000 python-cowsay-1.0.2/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-02-25 21:30:46.252604 python-cowsay-1.0.2/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-25 21:30:46.242042 python-cowsay-1.0.2/src/
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-25 21:30:46.242635 python-cowsay-1.0.2/src/cowsay/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     7548 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/__init__.py
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-25 21:30:46.251767 python-cowsay-1.0.2/src/cowsay/cows/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      793 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/TuxStab.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      356 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/armadillo.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      205 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/banana.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      174 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/bill-the-cat.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      639 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/blowfish.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      310 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/bud-frogs.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      123 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/bunny.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      625 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/cat.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      480 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/cheese.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      250 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/clippy.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      230 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/cower.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      569 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/daemon.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      175 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/default.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1284 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/dragon-and-cow.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1000 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/dragon.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      295 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/elephant-in-snake.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      284 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/elephant.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      275 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/elephant2.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      585 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/eyes.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      267 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/fat-banana.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      487 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/flaming-sheep.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      283 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/frogs.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      460 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/ghost.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      411 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/happy-whale.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      257 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/head-in.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      126 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/hellokitty.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      637 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/kiss.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      217 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/kitten.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      296 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/kitty.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      162 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/koala.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      181 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/llama.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      628 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/lobster.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      151 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/lollerskates.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      473 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/meow.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      439 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/milk.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      242 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/moofasa.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      203 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/moose.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      201 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/mutilated.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      884 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/octopus.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      141 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/owl.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      186 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/satanic.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      291 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/seahorse.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      232 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/sheep.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      433 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/skeleton.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      194 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/small.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      854 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/stegosaurus.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      364 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/stimpy.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      280 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/supermilker.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      892 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/surgery.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      428 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/taxi.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      293 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/three-eyes.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1302 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/turkey.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1105 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/turtle.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      215 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/tux.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      392 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/udder.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      317 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/whale.cow
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      248 2022-12-09 22:56:36.000000 python-cowsay-1.0.2/src/cowsay/cows/www.cow
-drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-02-25 21:30:46.252246 python-cowsay-1.0.2/src/python_cowsay.egg-info/
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4675 2023-02-25 21:30:46.000000 python-cowsay-1.0.2/src/python_cowsay.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1829 2023-02-25 21:30:46.000000 python-cowsay-1.0.2/src/python_cowsay.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-02-25 21:30:46.000000 python-cowsay-1.0.2/src/python_cowsay.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        7 2023-02-25 21:30:46.000000 python-cowsay-1.0.2/src/python_cowsay.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.717794 python-cowsay-1.1.0/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1076 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6035 2023-04-22 02:58:39.717662 python-cowsay-1.1.0/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     4265 2023-04-22 02:40:00.000000 python-cowsay-1.1.0/README.md
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      762 2023-04-22 02:58:34.000000 python-cowsay-1.1.0/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)       38 2023-04-22 02:58:39.717831 python-cowsay-1.1.0/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.706985 python-cowsay-1.1.0/src/
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.707488 python-cowsay-1.1.0/src/cowsay/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     8356 2023-04-22 02:27:59.000000 python-cowsay-1.1.0/src/cowsay/__init__.py
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.716932 python-cowsay-1.1.0/src/cowsay/cows/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      793 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/TuxStab.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      356 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/armadillo.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      205 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/banana.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      174 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/bill-the-cat.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      639 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/blowfish.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      310 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/bud-frogs.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      123 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/bunny.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      625 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/cat.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      480 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/cheese.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      250 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/clippy.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      230 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/cower.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      569 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/daemon.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      175 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/default.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1284 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/dragon-and-cow.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1000 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/dragon.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      295 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/elephant-in-snake.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      284 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/elephant.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      275 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/elephant2.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      585 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/eyes.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      267 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/fat-banana.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      487 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/flaming-sheep.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      283 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/frogs.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      460 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/ghost.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      411 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/happy-whale.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      257 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/head-in.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      126 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/hellokitty.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      637 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/kiss.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      217 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/kitten.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      296 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/kitty.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      162 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/koala.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      181 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/llama.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      628 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/lobster.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      151 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/lollerskates.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      473 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/meow.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      439 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/milk.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      242 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/moofasa.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      203 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/moose.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      201 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/mutilated.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      884 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/octopus.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      141 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/owl.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      186 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/satanic.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      291 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/seahorse.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      232 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/sheep.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      433 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/skeleton.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      194 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/small.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      854 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/stegosaurus.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      364 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/stimpy.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      280 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/supermilker.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      892 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/surgery.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      428 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/taxi.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      293 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/three-eyes.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1302 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/turkey.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1105 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/turtle.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      215 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/tux.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      392 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/udder.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      317 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/whale.cow
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)      248 2022-12-09 22:56:36.000000 python-cowsay-1.1.0/src/cowsay/cows/www.cow
+drwxr-xr-x   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        0 2023-04-22 02:58:39.717471 python-cowsay-1.1.0/src/python_cowsay.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     6035 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)     1817 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        1 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) UOA\Domain Users (1403514002)        7 2023-04-22 02:58:39.000000 python-cowsay-1.1.0/src/python_cowsay.egg-info/top_level.txt
```

### Comparing `python-cowsay-1.0.2/LICENSE` & `python-cowsay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/PKG-INFO` & `python-cowsay-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cowsay
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Cowsay clone in Python
 Author: James Finnie-Ansley
 License: MIT License
         
         Copyright (c) 2022 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,15 +57,15 @@
 		-- Calvin Trillin
 """.strip()
 print(cowsay(message))
 ```
 
 Will yield:
 
-```
+```text
  __________________________________________ 
 / The most remarkable thing about my       \
 | mother is that for thirty years she      |
 | served the family nothing but leftovers. |
 | The original meal has never been found.  |
 |                                          |
 \ -- Calvin Trillin                        /
@@ -77,15 +77,15 @@
                 ||     ||
 ```
 
 The parameters for these functions are:
 
 - `message` – a string to wrap in the text bubble
 - `cow='default'` – the name of the cow (valid names from `list_cows`)
-- `preset=None` – the original cowsay presets: `-bggpstwy`
+- `preset=None` – the original cowsay presets: `-bgpstwy`
 - `eyes=Option.eyes` – A custom eye string
 - `tongue=Option.tongue` – A custom tongue string
 - `width=40` – The width of the text bubble
 - `wrap_text=True` – Whether text should be wrapped in the bubble
 - `cowfile=None` – A custom string representing a cow
 
 ### Other Functions
@@ -102,14 +102,15 @@
 The `read_dot_cow` will look for the first heredoc in the steam and extract the
 heredoc contents. If no heredoc exists, the whole stream is used instead. Escape
 characters are then escaped. The default escape characters can be changed by
 passing in an optional `escape` dictionary parameter mapping escape codes to
 their chars.
 
 For example:
+
 ```python
 from io import StringIO
 
 from cowsay import read_dot_cow, cowthink
 
 cow = read_dot_cow(StringIO("""
 $the_cow = <<EOC;
@@ -125,21 +126,83 @@
 Nothing is illegal if one hundred businessmen decide to do it.
         -- Andrew Young
 """.strip()
 print(cowthink(message, cowfile=cow))
 ```
 
 Will yield:
-```
+
+```text
  ___________________________________ 
 ( Nothing is illegal if one hundred )
 ( businessmen decide to do it.      )
 (                                   )
 ( -- Andrew Young                   )
  ----------------------------------- 
          o
           o
            ___
           (o o)
          (  V  )
         /--m-m-
 ```
+
+## Full-Width Characters
+
+A bit of a hack at the moment, but if any full-width characters are found in the
+message string, ***all*** characters in the thought bubble are converted to
+full-width. For example:
+
+```text
+　＿＿＿＿＿＿＿＿＿＿＿＿　
+（　喵喵喵。我是一只猫。　）
+　－－－－－－－－－－－－　
+   o
+    o
+
+     |\_/|
+     |o o|__
+     --*--__\
+     C_C_(___)
+```
+
+This works fine when all characters in the message are full-width, but does not
+work so well when there is a mix of full- and neutral-width characters:
+
+```text
+　＿＿＿＿＿＿＿＿＿＿＿＿＿＿＿＿＿　
+（　喵喵喵。Ｉ　ａｍ　ａ　ｃａｔ．　）
+　－－－－－－－－－－－－－－－－－　
+   o
+    o
+
+     |\_/|
+     |o o|__
+     --*--__\
+     C_C_(___)
+```
+
+Each full-width character still only counts as one character when setting the
+text width. For example:
+
+```python
+from cowsay import cowthink
+
+message = "喵喵喵。我是一只猫。我想吃鱼和喝牛奶。"
+print(cowthink(message, cow="kitten", width=10))
+```
+
+Will yield:
+
+```text
+　＿＿＿＿＿＿＿＿＿＿＿＿　
+（　喵喵喵。我是一只猫。　）
+（　我想吃鱼和喝牛奶。　　）
+　－－－－－－－－－－－－　
+   o
+    o
+
+     |\_/|
+     |o o|__
+     --*--__\
+     C_C_(___)
+```
```

### Comparing `python-cowsay-1.0.2/pyproject.toml` & `python-cowsay-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-cowsay"
-version = "1.0.2"
+version = "1.1.0"
 description = "A Cowsay clone in Python"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 keywords = ["cowsay"]
 authors = [{ name = "James Finnie-Ansley" }]
 classifiers = [
@@ -23,7 +23,10 @@
 repository = "https://github.com/James-Ansley/cowsay"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools]
 include-package-data = true
+
+[tool.setuptools.package-data]
+"*" = ["*.cow"]
```

### Comparing `python-cowsay-1.0.2/src/cowsay/__init__.py` & `python-cowsay-1.1.0/src/cowsay/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import re
 from dataclasses import dataclass
 from os import PathLike
 from pathlib import Path, PurePath
 from textwrap import wrap
 from typing import TextIO
+from unicodedata import east_asian_width
 
 HEREDOC_PATTERN = re.compile(
     r'\$.* = <<["\']?(.*)["\']?;?(?P<the_cow>[\w\W]*)\1'
 )
 
 
 @dataclass
@@ -43,36 +44,37 @@
     bl: str = '\\'
     br: str = '/'
 
 
 THOUGHT_OPTIONS = {
     'cowsay': Bubble('\\', '<', '>', '/', '\\', '|', '|', '\\', '/'),
     'cowthink': Bubble('o', '(', ')', '(', ')', '(', ')', '(', ')'),
+    'cowsay': Bubble('\\', '<', '>', '/', '\\', '|', '|', '\\', '/'),
 }
 
 ESCAPES = {
     r'\@': '@',
     r'\$': '$',
     r'\\': '\\',
 }
 
 
-def read_dot_cow(f: TextIO, escapes: dict[str, str]=None) -> str:
+def read_dot_cow(f: TextIO, escapes: dict[str, str] = None) -> str:
     """
     Reads and parses a .cow file to a string. Unescapes characters in doing
     so. This function will search for a heredoc in the .cow file. If found,
     it will extract the cow in the heredoc, otherwise the whole file is used.
 
     :param f: The File to read from
     :param escapes: A dictionary mapping escape codes to their respective
         characters
     :return: The cow
     """
     if escapes is None:
-        escapes=ESCAPES
+        escapes = ESCAPES
     the_cow = f.read()
     match = HEREDOC_PATTERN.search(the_cow)
     if match is not None:
         the_cow = match.group('the_cow')
     for escape, replacement in escapes.items():
         the_cow = the_cow.replace(escape, replacement)
     return the_cow.strip('\r\n')
@@ -180,15 +182,36 @@
                 width=40,
                 wrap_text=True):
     """
     Wraps text is wrap_text is true, then pads text and sets inside a bubble.
     This is the text that appears above the cows
     """
     lines = fit_text(text, width, wrap_text)
-    return wrap_bubble(lines, brackets)
+    return normalise_width(wrap_bubble(lines, brackets))
+
+
+def to_full_width(string):
+    """Converts non-full-width characters to full-width"""
+    # From: https://stackoverflow.com/a/4632373/18307756
+    neutral_width = "".join(chr(i) for i in range(ord(" "), ord("~")))
+    full_width = (
+            "\u3000"  # Full-Width Space
+            + "".join(chr(i) for i in range(ord("！"), ord("～")))
+    )
+    full = str.maketrans(neutral_width, full_width)
+    return string.translate(full)
+
+
+def normalise_width(cow):
+    """
+    If any full-width characters are found, convert all characters to full width
+    """
+    if any(east_asian_width(c) in ("W", "F", "A") for c in cow):
+        return to_full_width(cow)
+    return cow
 
 
 def cowsay(message,
            cow='default',
            preset=None,
            eyes=Option.eyes,
            tongue=Option.tongue,
```

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/TuxStab.cow` & `python-cowsay-1.1.0/src/cowsay/cows/TuxStab.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/blowfish.cow` & `python-cowsay-1.1.0/src/cowsay/cows/blowfish.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/cat.cow` & `python-cowsay-1.1.0/src/cowsay/cows/cat.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/daemon.cow` & `python-cowsay-1.1.0/src/cowsay/cows/daemon.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/dragon-and-cow.cow` & `python-cowsay-1.1.0/src/cowsay/cows/dragon-and-cow.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/dragon.cow` & `python-cowsay-1.1.0/src/cowsay/cows/dragon.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/eyes.cow` & `python-cowsay-1.1.0/src/cowsay/cows/eyes.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/kiss.cow` & `python-cowsay-1.1.0/src/cowsay/cows/kiss.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/lobster.cow` & `python-cowsay-1.1.0/src/cowsay/cows/lobster.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/octopus.cow` & `python-cowsay-1.1.0/src/cowsay/cows/octopus.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/stegosaurus.cow` & `python-cowsay-1.1.0/src/cowsay/cows/stegosaurus.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/surgery.cow` & `python-cowsay-1.1.0/src/cowsay/cows/surgery.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/turkey.cow` & `python-cowsay-1.1.0/src/cowsay/cows/turkey.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/cowsay/cows/turtle.cow` & `python-cowsay-1.1.0/src/cowsay/cows/turtle.cow`

 * *Files identical despite different names*

### Comparing `python-cowsay-1.0.2/src/python_cowsay.egg-info/PKG-INFO` & `python-cowsay-1.1.0/src/python_cowsay.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-cowsay
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Cowsay clone in Python
 Author: James Finnie-Ansley
 License: MIT License
         
         Copyright (c) 2022 James Finnie-Ansley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,15 +57,15 @@
 		-- Calvin Trillin
 """.strip()
 print(cowsay(message))
 ```
 
 Will yield:
 
-```
+```text
  __________________________________________ 
 / The most remarkable thing about my       \
 | mother is that for thirty years she      |
 | served the family nothing but leftovers. |
 | The original meal has never been found.  |
 |                                          |
 \ -- Calvin Trillin                        /
@@ -77,15 +77,15 @@
                 ||     ||
 ```
 
 The parameters for these functions are:
 
 - `message` – a string to wrap in the text bubble
 - `cow='default'` – the name of the cow (valid names from `list_cows`)
-- `preset=None` – the original cowsay presets: `-bggpstwy`
+- `preset=None` – the original cowsay presets: `-bgpstwy`
 - `eyes=Option.eyes` – A custom eye string
 - `tongue=Option.tongue` – A custom tongue string
 - `width=40` – The width of the text bubble
 - `wrap_text=True` – Whether text should be wrapped in the bubble
 - `cowfile=None` – A custom string representing a cow
 
 ### Other Functions
@@ -102,14 +102,15 @@
 The `read_dot_cow` will look for the first heredoc in the steam and extract the
 heredoc contents. If no heredoc exists, the whole stream is used instead. Escape
 characters are then escaped. The default escape characters can be changed by
 passing in an optional `escape` dictionary parameter mapping escape codes to
 their chars.
 
 For example:
+
 ```python
 from io import StringIO
 
 from cowsay import read_dot_cow, cowthink
 
 cow = read_dot_cow(StringIO("""
 $the_cow = <<EOC;
@@ -125,21 +126,83 @@
 Nothing is illegal if one hundred businessmen decide to do it.
         -- Andrew Young
 """.strip()
 print(cowthink(message, cowfile=cow))
 ```
 
 Will yield:
-```
+
+```text
  ___________________________________ 
 ( Nothing is illegal if one hundred )
 ( businessmen decide to do it.      )
 (                                   )
 ( -- Andrew Young                   )
  ----------------------------------- 
          o
           o
            ___
           (o o)
          (  V  )
         /--m-m-
 ```
+
+## Full-Width Characters
+
+A bit of a hack at the moment, but if any full-width characters are found in the
+message string, ***all*** characters in the thought bubble are converted to
+full-width. For example:
+
+```text
+　＿＿＿＿＿＿＿＿＿＿＿＿　
+（　喵喵喵。我是一只猫。　）
+　－－－－－－－－－－－－　
+   o
+    o
+
+     |\_/|
+     |o o|__
+     --*--__\
+     C_C_(___)
+```
+
+This works fine when all characters in the message are full-width, but does not
+work so well when there is a mix of full- and neutral-width characters:
+
+```text
+　＿＿＿＿＿＿＿＿＿＿＿＿＿＿＿＿＿　
+（　喵喵喵。Ｉ　ａｍ　ａ　ｃａｔ．　）
+　－－－－－－－－－－－－－－－－－　
+   o
+    o
+
+     |\_/|
+     |o o|__
+     --*--__\
+     C_C_(___)
+```
+
+Each full-width character still only counts as one character when setting the
+text width. For example:
+
+```python
+from cowsay import cowthink
+
+message = "喵喵喵。我是一只猫。我想吃鱼和喝牛奶。"
+print(cowthink(message, cow="kitten", width=10))
+```
+
+Will yield:
+
+```text
+　＿＿＿＿＿＿＿＿＿＿＿＿　
+（　喵喵喵。我是一只猫。　）
+（　我想吃鱼和喝牛奶。　　）
+　－－－－－－－－－－－－　
+   o
+    o
+
+     |\_/|
+     |o o|__
+     --*--__\
+     C_C_(___)
+```
```

### Comparing `python-cowsay-1.0.2/src/python_cowsay.egg-info/SOURCES.txt` & `python-cowsay-1.1.0/src/python_cowsay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
 src/cowsay/__init__.py
 src/cowsay/cows/TuxStab.cow
 src/cowsay/cows/armadillo.cow
 src/cowsay/cows/banana.cow
 src/cowsay/cows/bill-the-cat.cow
```

