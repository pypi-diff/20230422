# Comparing `tmp/pybdsim-3.1.0.tar.gz` & `tmp/pybdsim-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdsim-3.1.0.tar", last modified: Sun Apr  2 21:27:47 2023, max compression
+gzip compressed data, was "pybdsim-3.1.1.tar", last modified: Sat Apr 22 20:48:00 2023, max compression
```

## Comparing `pybdsim-3.1.0.tar` & `pybdsim-3.1.1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.440224 pybdsim-3.1.0/
--rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.1.0/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.1.0/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.1.0/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.1.0/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-02 21:27:47.440324 pybdsim-3.1.0/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      924 2023-03-19 11:28:25.000000 pybdsim-3.1.0/README.md
--rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.1.0/bitbucket-pipelines.yml
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.409102 pybdsim-3.1.0/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)  1187057 2023-04-02 21:26:31.000000 pybdsim-3.1.0/docs/pybdsim.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.411523 pybdsim-3.1.0/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      291 2023-03-17 15:48:00.000000 pybdsim-3.1.0/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.1.0/docs/source/builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.1.0/docs/source/classes.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.1.0/docs/source/compare.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.1.0/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.1.0/docs/source/convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.1.0/docs/source/data.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.1.0/docs/source/data_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.1.0/docs/source/developer.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12892 2023-03-29 08:13:29.000000 pybdsim-3.1.0/docs/source/fieldmaps.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.414711 pybdsim-3.1.0/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/source/figures/rebdsimFileHistograms.png
--rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/source/figures/rebdsimFileHistogramsWrapped.png
--rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/source/figures/rebdsimFileMembers.png
--rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/source/figures/simpleHistogramPlot.png
--rw-r--r--   0 lnevay     (501) staff       (20)      456 2023-03-22 08:08:12.000000 pybdsim-3.1.0/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2107 2023-03-19 13:20:03.000000 pybdsim-3.1.0/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.1.0/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.1.0/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.1.0/docs/source/support.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    10725 2023-04-02 20:10:03.000000 pybdsim-3.1.0/docs/source/version_history.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.415243 pybdsim-3.1.0/examples/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.419546 pybdsim-3.1.0/examples/1_builder/
--rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/1_builder/1_builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/1_builder/1_testmachine.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/1_builder/1_testmachine.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.422014 pybdsim-3.1.0/examples/2_convert/
--rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/1_madxtfs2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/1_madxtfs2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/2_convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/2_transport2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/2_transport2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/transport_example.dat
--rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/transport_example.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/twiss35tevb1_short.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.1.0/examples/2_convert/twiss35tevb1_short.tar.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.422186 pybdsim-3.1.0/examples/3_optics/
--rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.1.0/examples/3_optics/optics_validation.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.422434 pybdsim-3.1.0/examples/4_uproot/
--rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.1.0/examples/4_uproot/4_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.1.0/examples/examples.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1720 2023-03-28 19:11:18.000000 pybdsim-3.1.0/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-04-02 21:27:47.440591 pybdsim-3.1.0/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.1.0/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.405490 pybdsim-3.1.0/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.425907 pybdsim-3.1.0/src/pybdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.1.0/src/pybdsim/Beam.py
--rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.1.0/src/pybdsim/Builder.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.428454 pybdsim-3.1.0/src/pybdsim/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     8639 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Compare/_BdsimBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.1.0/src/pybdsim/Compare/_ElegantBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Compare/_Mad8BdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23116 2022-02-14 12:30:59.000000 pybdsim-3.1.0/src/pybdsim/Compare/_MadxBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Compare/_MadxMadxComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48472 2022-02-14 12:30:59.000000 pybdsim-3.1.0/src/pybdsim/Compare/_MultipleCodeComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Compare/_SadComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6448 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Compare/_TransportBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      822 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Compare/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2522 2023-03-17 15:48:00.000000 pybdsim-3.1.0/src/pybdsim/Constants.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.430807 pybdsim-3.1.0/src/pybdsim/Convert/
--rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.1.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.1.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
--rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.1.0/src/pybdsim/Convert/_CPyMad2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Convert/_ElegantParamToStrength.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Convert/_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Convert/_Rebdsim2Numpy.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Convert/_SadFlat2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     4460 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Convert/_Transport2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-03-28 19:11:54.000000 pybdsim-3.1.0/src/pybdsim/Convert/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Convert/collimator_analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)    77926 2023-03-22 07:31:37.000000 pybdsim-3.1.0/src/pybdsim/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    69588 2023-03-22 07:35:09.000000 pybdsim-3.1.0/src/pybdsim/DataUproot.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.431328 pybdsim-3.1.0/src/pybdsim/Field/
--rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Field/FieldPlotter.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Field/FieldPlotterVtk.py
--rw-r--r--   0 lnevay     (501) staff       (20)    16876 2023-03-29 09:25:28.000000 pybdsim-3.1.0/src/pybdsim/Field/_Field.py
--rw-r--r--   0 lnevay     (501) staff       (20)      982 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Field/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Geant4.py
--rw-r--r--   0 lnevay     (501) staff       (20)    18656 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Joinhistograms.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3585 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/ModelProcessing.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.405772 pybdsim-3.1.0/src/pybdsim/Obsolete/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.433125 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
--rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Event.py
--rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Model.py
--rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Plots.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Processed.py
--rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Root.py
--rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Run.py
--rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.1.0/src/pybdsim/Optics.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.1.0/src/pybdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)    73311 2023-03-17 15:47:53.000000 pybdsim-3.1.0/src/pybdsim/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.1.0/src/pybdsim/Run.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.433934 pybdsim-3.1.0/src/pybdsim/Testing/
--rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Testing/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48649 2021-06-15 15:09:13.000000 pybdsim-3.1.0/src/pybdsim/Testing/bdsimMadx.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.1.0/src/pybdsim/Testing/trackingTester.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.1.0/src/pybdsim/Visualisation.py
--rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.1.0/src/pybdsim/Writer.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.1.0/src/pybdsim/XSecBias.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3390 2023-03-19 12:59:36.000000 pybdsim-3.1.0/src/pybdsim/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4594 2023-03-19 12:57:06.000000 pybdsim-3.1.0/src/pybdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-04-02 21:27:47.000000 pybdsim-3.1.0/src/pybdsim/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.426678 pybdsim-3.1.0/src/pybdsim.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-02 21:27:47.000000 pybdsim-3.1.0/src/pybdsim.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     5123 2023-04-02 21:27:47.000000 pybdsim-3.1.0/src/pybdsim.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-04-02 21:27:47.000000 pybdsim-3.1.0/src/pybdsim.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.1.0/src/pybdsim.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)      237 2023-04-02 21:27:47.000000 pybdsim-3.1.0/src/pybdsim.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-04-02 21:27:47.000000 pybdsim-3.1.0/src/pybdsim.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.434132 pybdsim-3.1.0/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.1.0/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.435289 pybdsim-3.1.0/tests/test_input/
--rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.1.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
--rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.1.0/tests/test_input/model-model-aper.tfs.gz
--rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.1.0/tests/test_input/model-model-collsettings.dat
--rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.1.0/tests/test_input/model-model.tfs.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.435635 pybdsim-3.1.0/tests/test_output/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.1.0/tests/test_output/.gitkeep
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.436434 pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.437372 pybdsim-3.1.0/tests/test_output/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.406313 pybdsim-3.1.0/tests/test_output2/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.438285 pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.439098 pybdsim-3.1.0/tests/test_output2/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/test_output2/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.439963 pybdsim-3.1.0/tests/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.1.0/tests/tests/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/tests/pybdsim_test_utils.py
--rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.1.0/tests/tests/test_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.1.0/tests/tests/testratio.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.1.0/tests/tests/write_test_outputs.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-02 21:27:47.440097 pybdsim-3.1.0/tests/unit/
--rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.1.0/tests/unit/test_Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.884832 pybdsim-3.1.1/
+-rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.1.1/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.1.1/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.1.1/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.1.1/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-22 20:48:00.884943 pybdsim-3.1.1/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      924 2023-03-19 11:28:25.000000 pybdsim-3.1.1/README.md
+-rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.1.1/bitbucket-pipelines.yml
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.846835 pybdsim-3.1.1/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)  1187057 2023-04-02 21:26:31.000000 pybdsim-3.1.1/docs/pybdsim.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.852374 pybdsim-3.1.1/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      291 2023-03-17 15:48:00.000000 pybdsim-3.1.1/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.1.1/docs/source/builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.1.1/docs/source/classes.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.1.1/docs/source/compare.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.1.1/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.1.1/docs/source/convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.1.1/docs/source/data.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.1.1/docs/source/data_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.1.1/docs/source/developer.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12892 2023-03-29 08:13:29.000000 pybdsim-3.1.1/docs/source/fieldmaps.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.855233 pybdsim-3.1.1/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/rebdsimFileHistograms.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/rebdsimFileHistogramsWrapped.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/rebdsimFileMembers.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/simpleHistogramPlot.png
+-rw-r--r--   0 lnevay     (501) staff       (20)      456 2023-03-22 08:08:12.000000 pybdsim-3.1.1/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2107 2023-03-19 13:20:03.000000 pybdsim-3.1.1/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.1.1/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.1.1/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/support.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11351 2023-04-22 20:36:34.000000 pybdsim-3.1.1/docs/source/version_history.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.855743 pybdsim-3.1.1/examples/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.856900 pybdsim-3.1.1/examples/1_builder/
+-rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/1_builder/1_builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/1_builder/1_testmachine.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/1_builder/1_testmachine.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.859498 pybdsim-3.1.1/examples/2_convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/1_madxtfs2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/1_madxtfs2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/2_convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/2_transport2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/2_transport2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/transport_example.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/transport_example.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.tar.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.859721 pybdsim-3.1.1/examples/3_optics/
+-rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.1.1/examples/3_optics/optics_validation.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.859986 pybdsim-3.1.1/examples/4_uproot/
+-rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.1.1/examples/4_uproot/4_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.1.1/examples/examples.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1731 2023-04-22 17:03:22.000000 pybdsim-3.1.1/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-04-22 20:48:00.885220 pybdsim-3.1.1/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.1.1/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.843051 pybdsim-3.1.1/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.867704 pybdsim-3.1.1/src/pybdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.1.1/src/pybdsim/Beam.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.1.1/src/pybdsim/Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.872250 pybdsim-3.1.1/src/pybdsim/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     8639 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/_BdsimBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.1.1/src/pybdsim/Compare/_ElegantBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    23116 2022-02-14 12:30:59.000000 pybdsim-3.1.1/src/pybdsim/Compare/_MadxBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Compare/_MadxMadxComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48472 2022-02-14 12:30:59.000000 pybdsim-3.1.1/src/pybdsim/Compare/_MultipleCodeComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Compare/_SadComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6448 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Compare/_TransportBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      822 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.1.1/src/pybdsim/Constants.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.875479 pybdsim-3.1.1/src/pybdsim/Convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.1.1/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.1.1/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.1.1/src/pybdsim/Convert/_CPyMad2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_ElegantParamToStrength.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Rebdsim2Numpy.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_SadFlat2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     4460 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Transport2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-03-28 19:11:54.000000 pybdsim-3.1.1/src/pybdsim/Convert/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Convert/collimator_analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    78167 2023-04-22 20:33:46.000000 pybdsim-3.1.1/src/pybdsim/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.1.1/src/pybdsim/DataUproot.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.876345 pybdsim-3.1.1/src/pybdsim/Field/
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Field/FieldPlotter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Field/FieldPlotterVtk.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    16881 2023-04-17 18:48:37.000000 pybdsim-3.1.1/src/pybdsim/Field/_Field.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.1.1/src/pybdsim/Field/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Geant4.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.1.1/src/pybdsim/Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Joinhistograms.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.1.1/src/pybdsim/ModelProcessing.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.843335 pybdsim-3.1.1/src/pybdsim/Obsolete/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.878234 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Event.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Model.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Plots.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Processed.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Root.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Run.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.1.1/src/pybdsim/Optics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.1.1/src/pybdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    74729 2023-04-22 20:35:30.000000 pybdsim-3.1.1/src/pybdsim/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.1.1/src/pybdsim/Run.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.878907 pybdsim-3.1.1/src/pybdsim/Testing/
+-rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Testing/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48649 2021-06-15 15:09:13.000000 pybdsim-3.1.1/src/pybdsim/Testing/bdsimMadx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Testing/trackingTester.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.1.1/src/pybdsim/Visualisation.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.1.1/src/pybdsim/Writer.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.1.1/src/pybdsim/XSecBias.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3390 2023-03-19 12:59:36.000000 pybdsim-3.1.1/src/pybdsim/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.1.1/src/pybdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.868444 pybdsim-3.1.1/src/pybdsim.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     5123 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.1.1/src/pybdsim.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      245 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.879140 pybdsim-3.1.1/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.1.1/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.880208 pybdsim-3.1.1/tests/test_input/
+-rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/model-model-aper.tfs.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/model-model-collsettings.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/model-model.tfs.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.880557 pybdsim-3.1.1/tests/test_output/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_output/.gitkeep
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.881380 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.882124 pybdsim-3.1.1/tests/test_output/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.843893 pybdsim-3.1.1/tests/test_output2/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.883024 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.883781 pybdsim-3.1.1/tests/test_output2/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.884578 pybdsim-3.1.1/tests/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.1.1/tests/tests/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/tests/pybdsim_test_utils.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/tests/test_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.1.1/tests/tests/testratio.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.1.1/tests/tests/write_test_outputs.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.884710 pybdsim-3.1.1/tests/unit/
+-rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/unit/test_Builder.py
```

### Comparing `pybdsim-3.1.0/COPYING.txt` & `pybdsim-3.1.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/LICENSE.txt` & `pybdsim-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/Makefile` & `pybdsim-3.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/PKG-INFO` & `pybdsim-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.1.0/README.md` & `pybdsim-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/bitbucket-pipelines.yml` & `pybdsim-3.1.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/Makefile` & `pybdsim-3.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/make.bat` & `pybdsim-3.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/pybdsim.pdf` & `pybdsim-3.1.1/docs/pybdsim.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/builder.rst` & `pybdsim-3.1.1/docs/source/builder.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/classes.rst` & `pybdsim-3.1.1/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/compare.rst` & `pybdsim-3.1.1/docs/source/compare.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/conf.py` & `pybdsim-3.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/convert.rst` & `pybdsim-3.1.1/docs/source/convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/data.rst` & `pybdsim-3.1.1/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/data_uproot.rst` & `pybdsim-3.1.1/docs/source/data_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/developer.rst` & `pybdsim-3.1.1/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/fieldmaps.rst` & `pybdsim-3.1.1/docs/source/fieldmaps.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/figures/rebdsimFileHistograms.png` & `pybdsim-3.1.1/docs/source/figures/rebdsimFileHistograms.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/figures/rebdsimFileHistogramsWrapped.png` & `pybdsim-3.1.1/docs/source/figures/rebdsimFileHistogramsWrapped.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/figures/rebdsimFileMembers.png` & `pybdsim-3.1.1/docs/source/figures/rebdsimFileMembers.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/figures/simpleHistogramPlot.png` & `pybdsim-3.1.1/docs/source/figures/simpleHistogramPlot.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/installation.rst` & `pybdsim-3.1.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/licence.rst` & `pybdsim-3.1.1/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/moduledocs.rst` & `pybdsim-3.1.1/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/support.rst` & `pybdsim-3.1.1/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/docs/source/version_history.rst` & `pybdsim-3.1.1/docs/source/version_history.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 ===============
 Version History
 ===============
 
+V3.1.1 - 2023 / 04 / 23
+=======================
+
+* Fixed spectra loading and plotting for when the 'p' and 's' prefixes are used
+  in the rebdsim Spectra command to denote primary and secondary particles.
+* Fixed error with default log scale in `Plot.Histogram2D` when no `vmin` was specified.
+* Fix :code:`pybdsim._version_tuple` which should be :code:`pybdsim.__version_tuple__`.
+* Fix import without awkward array which is only required for the [uproot] feature of pybdsim.
+* :code:`pybdsim.Plot.Spectra()` now makes more than one plot if more than 8 particles are specified.
+* Recognised PDG ID 0 as "total" from BDSIM.
+
+
 V3.1.0 - 2023 / 04 / 02
 =======================
 
 * Add the writing and reading of comment lines in field maps.
 * Reduce print out when loading a field map.
 * Clean imports in cpymad interface as well as in Convert functions.
```

### Comparing `pybdsim-3.1.0/examples/1_builder/1_testmachine.png` & `pybdsim-3.1.1/examples/1_builder/1_testmachine.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/1_madxtfs2gmad.png` & `pybdsim-3.1.1/examples/2_convert/1_madxtfs2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/2_convert.rst` & `pybdsim-3.1.1/examples/2_convert/2_convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/2_transport2gmad.png` & `pybdsim-3.1.1/examples/2_convert/2_transport2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/transport_example.dat` & `pybdsim-3.1.1/examples/2_convert/transport_example.dat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/transport_example.pdf` & `pybdsim-3.1.1/examples/2_convert/transport_example.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/twiss35tevb1_short.pdf` & `pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/2_convert/twiss35tevb1_short.tar.gz` & `pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/3_optics/optics_validation.py` & `pybdsim-3.1.1/examples/3_optics/optics_validation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/examples/4_uproot/4_uproot.rst` & `pybdsim-3.1.1/examples/4_uproot/4_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/pyproject.toml` & `pybdsim-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   "fortranformat",
   "pymadx",
   "pymad8",
   "pytransport"
 ]
 
 [project.optional-dependencies]
-uproot = ["uproot", "pandas", "pint"]
+uproot = ["awkward", "uproot", "pandas", "pint"]
 boost_histogram = ["boost-histogram"]
 cpymad = ["cpymad", "mergedeep"]
 pysad = ["pysad"]
 dev = ["pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 homepage = "http://www.pp.rhul.ac.uk/bdsim/pybdsim"
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Beam.py` & `pybdsim-3.1.1/src/pybdsim/Beam.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Builder.py` & `pybdsim-3.1.1/src/pybdsim/Builder.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_BdsimBdsimComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_BdsimBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_ElegantBdsimComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_ElegantBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_Mad8BdsimComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_MadxBdsimComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_MadxBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_MultipleCodeComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_MultipleCodeComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_SadComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_SadComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/_TransportBdsimComparison.py` & `pybdsim-3.1.1/src/pybdsim/Compare/_TransportBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Compare/__init__.py` & `pybdsim-3.1.1/src/pybdsim/Compare/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Constants.py` & `pybdsim-3.1.1/src/pybdsim/Constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 PDGind = {
+    0     : ('Total',                 'Total'),
 #COMMON
     2212  : ('Proton',                'p'),
     -2212 : ('Antiproton',            r'$\overline{p}$'),
     2112  : ('Neutron',               'n'),
-    -2112 : ('Neutron',               'n'),
+    -2112 : ('AntiNeutron',           r'$\overline{n}$'),
     11    : ('Electron',              r'$e^{-}$'),
     -11   : ('Positron',              r'$e^{+}$'),
     22    : ('Photon',                r'$\gamma$'),
     12    : ('Electron Neutrino',     r'$\nu_{e}$'),
     -12   : ('Electron Antineutrino', r'$\overline\nu_{e}$'),
     13    : ('Muon',                  r'$\mu^{-}$'),
     -13   : ('Antimuon',              r'$\mu^{+}$'),
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_CPyMad2Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_CPyMad2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_ElegantParamToStrength.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_ElegantParamToStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Saveline2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_MadxTfs2Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2GmadStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_Rebdsim2Numpy.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_Rebdsim2Numpy.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_SadFlat2Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_SadFlat2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/_Transport2Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Convert/_Transport2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/__init__.py` & `pybdsim-3.1.1/src/pybdsim/Convert/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Convert/collimator_analysis.py` & `pybdsim-3.1.1/src/pybdsim/Convert/collimator_analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Data.py` & `pybdsim-3.1.1/src/pybdsim/Data.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,37 +348,42 @@
 class Spectra:
     def __init__(self, nameIn=None):
         self.name = nameIn
         self.histograms = {}
         self.histogramspy = {}
         self.pdgids = set()
         self.pdgidsSorted = []
+        self.flags = [] # none, primary or secondary
 
-    def append(self, pdgid, hist, path, nameIn=None):
+    def append(self, pdgid, hist, path, nameIn=None, flag=None):
         if nameIn:
             self.name = nameIn
-        self.histograms[pdgid] = hist
-        self.histogramspy[pdgid] = TH1(hist)
+        self.histograms[(pdgid,flag)] = hist
+        self.histogramspy[(pdgid,flag)] = TH1(hist)
         self.pdgids.add(pdgid)
         self._generateSortedList()
 
     def _generateSortedList(self):
-        integrals = {pdgid:h.integral for pdgid,h in self.histogramspy.items()}
+        integrals = {(pdgid,flag):h.integral for (pdgid,flag),h in self.histogramspy.items()}
         integralsSorted = sorted(integrals.items(), key=lambda item: item[1])
-        self.pdgidsSorted = [pdgid for pdgid,_ in sorted(integrals.items(), key=lambda item: item[1], reverse=True)]
+        self.pdgidsSorted = [(pdgid,flag) for (pdgid,flag),_ in sorted(integrals.items(), key=lambda item: item[1], reverse=True)]
 
 def ParseSpectraName(hname):
     # expects a string of the form
     # Top10_Spectra_SamplerName_PDGID
     hn = _re.sub("Top\d+_", "", hname)
     #hn = hname.replace('Top_','')
     hn = hn.replace('Spectra_','')
-    name,nth,pdgid = hn.split('_')
+    vals = hn.split('_')
+    name,nth,pdgid = vals[:3]
+    flag = vals[3] if len(vals) == 4 else 'n'
+    if len(flag) > 1:
+        flag = flag.lower()[0]
     pdgid = int(pdgid)
-    return name+"_"+nth,pdgid
+    return name+"_"+nth,pdgid,flag
 
 class RebdsimFile:
     """
     Class to represent data in rebdsim output file.
 
     :param filename: File to load
     :type filename: str
@@ -543,16 +548,16 @@
             self.histogramspy[path] = hpy
 
     def _PopulateSpectraDictionaries(self):
         for path,hist in self.histograms1d.items():
             hname = str(hist.GetName())
             if 'Spectra' in hname:
                 try:
-                    sname,pdgid = ParseSpectraName(hname)
-                    self.spectra[sname].append(pdgid, hist, path, sname)
+                    sname,pdgid,flag = ParseSpectraName(hname)
+                    self.spectra[sname].append(pdgid, hist, path, sname, flag)
                 except ValueError:
                     pass # could be old data with the word "Spectra" in the name
 
 def CreateEmptyRebdsimFile(outputfilename, nOriginalEvents=1):
     """
     Create an empty rebdsim format file with the layout of folders.
     Returns the ROOT.TFile object.
```

### Comparing `pybdsim-3.1.0/src/pybdsim/DataUproot.py` & `pybdsim-3.1.1/src/pybdsim/DataUproot.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     import uproot as _uproot
 except (ImportError, ImportWarning):
     _logging.warning("Uproot is required for this module to have full functionalities.\n")
     raise ImportError("Uproot is required for this module to work.")
 
 _WITH_ROOT = False
 try:
-    _warnings.simplefilter("ignore")
     import ROOT as _ROOT
     _WITH_ROOT = True
 except ImportError:
-    _logging.warning("ROOT is required for this module to have full functionalities.\n"
-                     "Not all methods will be available.")
+    pass
+    #_logging.warning("ROOT is required for this module to have full functionalities.\n"
+    #                 "Not all methods will be available.")
 
 _WITH_BOOST_HISTOGRAM = False
 try:
     try:
         _warnings.simplefilter("ignore")
         import boost_histogram as bh
         _warnings.simplefilter("default")
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Field/FieldPlotter.py` & `pybdsim-3.1.1/src/pybdsim/Field/FieldPlotter.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Field/FieldPlotterVtk.py` & `pybdsim-3.1.1/src/pybdsim/Field/FieldPlotterVtk.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Field/_Field.py` & `pybdsim-3.1.1/src/pybdsim/Field/_Field.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
 
     :param field2D: field object
     :type field2D: pybdsim.Field._Field.Field2D instance
 
     returns an instance of the same type.
     
     For a 2D field (i.e. function of x,y but can include Bx,By,Bz),
-    for the quadrant \#1, mirror it and generate a bigger field for
+    for the quadrant number 1, mirror it and generate a bigger field for
     all four quadrants.
     
     1. original data
     2. data mirrored in x, (x,Bx) \*= -1
     3. data mirrored in x,y, (x,y,By) \*= -1
     4. data mirrored in y, (y,Bx) \*= -1
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Field/__init__.py` & `pybdsim-3.1.1/src/pybdsim/Field/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 from .FieldPlotter import Plot2DXYBz
 from .FieldPlotter import Plot2DXYFxFyFz
 from .FieldPlotter import Plot3DXY
 from .FieldPlotter import Plot3DXZ
 
 try:
     from .FieldPlotterVtk import Plot3DXYZVtk
-except ImportError :
+except ImportError:
     hasVtk = False
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Geant4.py` & `pybdsim-3.1.1/src/pybdsim/Geant4.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Gmad.py` & `pybdsim-3.1.1/src/pybdsim/Gmad.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,21 +488,21 @@
         f = open(fileName)
         self.s = f.read(-1)
         f.close()
 
         # regular expressions used for matching
 
         # For finding elements
-        self.elementNameRe = "([a-zA-Z0-9._-]+)\s*:\s*([,a-zA-Z0-9=.\*\s/-]+);"
+        self.elementNameRe = r"([a-zA-Z0-9._-]+)\s*:\s*([,a-zA-Z0-9=.\*\s/-]+);"
         # For finding a known element
-        self.elementRe     = "\s*:\s*([,a-zA-Z0-9=.\*\s/-]+);"
+        self.elementRe = r"\s*:\s*([,a-zA-Z0-9=.\*\s/-]+);"
         # For extracting the parameters for an element
-        self.elementValRe  = "([a-zA-Z0-9_-]+)=([a-zA-Z-0-9.eE\*/]+)"
+        self.elementValRe = r"([a-zA-Z0-9_-]+)=([a-zA-Z-0-9.eE\*/]+)"
         # For extracting element type
-        self.elementNameRe1    = "([a-zA-Z0-9._-]+)\s*:\s*([,a-zA-Z0-9._-]+),([,a-zA-Z0-9=.\*\s/-]+);"
+        self.elementNameRe1 = r"([a-zA-Z0-9._-]+)\s*:\s*([,a-zA-Z0-9._-]+),([,a-zA-Z0-9=.\*\s/-]+);"
 
         # determine element names in file
         self.elementNames();
 
     def elementNames(self) :
         '''Make a list of element names, stored in self.elementNameList'''
         self.elementNameList = []
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Joinhistograms.py` & `pybdsim-3.1.1/src/pybdsim/Joinhistograms.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/ModelProcessing.py` & `pybdsim-3.1.1/src/pybdsim/ModelProcessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 
 def GetAxisAlignedBoundingBoxOfCollimator(modelData, collimatorName):
     """
     Inspect pybdsim.Data.ModelData assuming collimator info was stored
     to give an axis aligned bounding box set of ranges in global coordinates.
     """
-    if type(modelData) is not pybdsim.Data.ModelData:
+    import pybdsim as _pybdsim
+    if type(modelData) is not _pybdsim.Data.ModelData:
         raise TypeError("not pybdsim.Data.ModelData instance")
 
     ci = modelData.collimatorInfo[collimatorName]
     gi = modelData.collimatorIndicesByName[collimatorName]
 
     midPos = modelData.midRefPos[gi]
     midRot = modelData.midRefRot[gi]
@@ -31,26 +32,27 @@
     
     
 def GetMaterialIDOfCollimator(modelData, collimatorName):
     """
     Inspect pybdsim.Data.ModelData assuming collimator info was stored
     to give an axis aligned bounding box set of ranges in global coordinates.
     """
-    if type(modelData) is not pybdsim.Data.ModelData:
+    import pybdsim as _pybdsim
+    if type(modelData) is not _pybdsim.Data.ModelData:
         raise TypeError("not pybdsim.Data.ModelData instance")
     ci = modelData.collimatorInfo[collimatorName]
     return modelData.materialNameToID[ci.material]    
 
 def GenerateFullListOfSamplers(inputfile, outputfile):
     """
     inputfile - path to main gmad input file
 
     This will parse the input using the compiled BDSIM
     parser (GMAD), iterate over all the beamline elements
-    and generate a sampler for every elements.  Ignores
+    and generate a sampler for every element.  Ignores
     samplers, but may include already defined ones in your
     own input.
 
     """
     lattice  = _Gmad.Lattice(inputfile)
     samplers = []
     typestoignore = [
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Event.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Event.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Processed.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Processed.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/Root.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Root.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Obsolete/Rebdsim/__init__.py` & `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Optics.py` & `pybdsim-3.1.1/src/pybdsim/Optics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Options.py` & `pybdsim-3.1.1/src/pybdsim/Options.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Plot.py` & `pybdsim-3.1.1/src/pybdsim/Plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,30 +525,68 @@
             _plt.yscale('log', nonposy='clip')
     else:
         _plt.ylim(ymin*0.8, ymax*1.05)
 
     _plt.tight_layout()
     return f
 
-def Spectra(spectra, log=False, xlog=False, xlabel=None, ylabel=None, title=None, scalingFactors=None, xScalingFactors=None, figsize=(10,5), legendKwargs={}, **errorbarKwargs):
-    histograms = [spectra.histogramspy[pdgid] for pdgid in spectra.pdgidsSorted]
-    labels = [_Constants.GetPDGName(pdgid)[1] for pdgid in spectra.pdgidsSorted]
+def Spectra(spectra,
+            log=False, xlog=False,
+            xlabel=None, ylabel=None, title=None,
+            scalingFactors=None, xScalingFactors=None,
+            figsize=(10,5), legendKwargs={}, **errorbarKwargs):
+    """
+    Plot a Spectra object loaded from data that represents a set of histograms.
+
+    returns a list of figure objects.
+    """
+    histograms = [spectra.histogramspy[(pdgid,flag)] for (pdgid,flag) in spectra.pdgidsSorted]
+    
+    labels = []
+    for (pdgid, flag) in spectra.pdgidsSorted:
+        rn = _Constants.GetPDGName(pdgid)[1]
+        if flag != 'n':
+            rn += r" ("+flag+r")"
+        labels.append(rn)        
+            
     if xlabel is None:
         print("Using default xlabel of kinetic energy")
         xlabel="Kinetic Energy (GeV)"
     if ylabel is None:
         h1 = histograms[0]
         if _np.any(_np.diff(h1.xwidths)):
             # uneven binning suspected
             ylabel = "Per-Event Rate"
         else:
             ylabel = "Per-Event Rate / " + str(round(h1.xwidths[0],2)) + " GeV"
     if title is None:
         title = spectra.name
-    Histogram1DMultiple(histograms, labels, log, xlog, xlabel, ylabel, title, scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
+
+    # avoid overly busy plots... if more than 8 lines, split into 2. Copy the total to both.
+    if len(histograms) > 8:
+        histogramsA = histograms[:9]
+        histogramsB = histograms[9:]
+        labelsA = labels[:9]
+        labelsB = labels[9:]
+        if (0,'n') in spectra.pdgidsSorted:
+            # if pdgid of 0, which is the 'total' histogram is present,
+            # then it's integral must be the greatest and it should be first
+            # in the A list, so also put it first in the B list
+            histogramsB.insert(0, histogramsA[0])
+            
+        f1 = Histogram1DMultiple(histogramsA, labelsA, log, xlog, xlabel, ylabel, title,
+                                 scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
+        f2 = Histogram1DMultiple(histogramsB, labelsB, log, xlog, xlabel, ylabel, title,
+                                 scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
+        return [f1,f2]
+    else:
+        f1 = Histogram1DMultiple(histograms, labels, log, xlog, xlabel, ylabel, title,
+                                 scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
+        return [f1]
+
 
 def Histogram1DMultiple(histograms, labels, log=False, xlog=False, xlabel=None, ylabel=None, title=None, scalingFactors=None, xScalingFactors=None, figsize=(10,5), legendKwargs={}, **errorbarKwargs):
     """
     Plot multiple 1D histograms on the same plot. Histograms and labels should 
     be lists of the same length with pybdsim.Data.TH1 objects and strings.
 
     return figure instance
@@ -663,15 +701,15 @@
     ysf = yScalingFactor
     ext = [_np.min(xsf*h.xlowedge),_np.max(xsf*h.xhighedge),_np.min(ysf*h.ylowedge),_np.max(ysf*h.yhighedge)]
     histEmpty = len(h.contents[h.contents!=0]) == 0
     if vmin is None:
         if autovmin and vmin is None and not histEmpty:
             vmin = _np.min(h.contents[h.contents!=0])
         else:
-            vmin = 0
+            vmin = None
     if logNorm:
         d = _copy.deepcopy(sf*h.contents.T)
         norm = _LogNorm(vmin=vmin,vmax=vmax) if vmax is not None else _LogNorm(vmin=vmin)
         ax = f.add_subplot(111)
         im = ax.pcolormesh(h.xedges*xsf, h.yedges*ysf, d, norm=norm, rasterized=True, **imshowKwargs)
         #_plt.imshow(d, extent=ext, origin='lower', aspect=aspect, norm=norm, interpolation='none', **imshowKwargs)
         if colourbar:
@@ -734,14 +772,16 @@
     l = _LogNorm()
     d = l(th3.contents)
     d.data[d.mask] = 0
     colours = _plt.cm.viridis(l(th3.contents))
     colours[:,:,:,3] = d.data
     ax.voxels(fill, facecolors=colours)
     #return colours
+    return f
+    
 
 def Histogram1DRatio(histogram1, histogram2, label1="", label2="", xLogScale=False, yLogScale=False, xlabel=None, ylabel=None, title=None, scalingFactor=1.0, xScalingFactor=1.0, figsize=(6.4, 4.8), ratio=3, histogram1Colour=None, histogram2Colour=None, ratioColour=None, ratioYAxisLimit=None, **errorbarKwargs):
     """
     Plot two histograms with their ratio (#1 / #2) in a subplot below.
 
     :param histogram1: a `pybdsim.Data.TH1` instance
     :param histogram2: a `pybdsim.Data.TH1` instance
@@ -1938,8 +1978,8 @@
 
     if transpose:
         _plt.xlabel('Y (m)')
         _plt.ylabel('Z (m)')
     else:
         _plt.xlabel('Z (m)')
         _plt.ylabel('Y (m)')
-    _plt.tight_layout()
+    _plt.tight_layout()
```

### Comparing `pybdsim-3.1.0/src/pybdsim/Run.py` & `pybdsim-3.1.1/src/pybdsim/Run.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Testing/bdsimMadx.py` & `pybdsim-3.1.1/src/pybdsim/Testing/bdsimMadx.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Testing/trackingTester.py` & `pybdsim-3.1.1/src/pybdsim/Testing/trackingTester.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Visualisation.py` & `pybdsim-3.1.1/src/pybdsim/Visualisation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/Writer.py` & `pybdsim-3.1.1/src/pybdsim/Writer.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/XSecBias.py` & `pybdsim-3.1.1/src/pybdsim/XSecBias.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/_General.py` & `pybdsim-3.1.1/src/pybdsim/_General.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/src/pybdsim/__init__.py` & `pybdsim-3.1.1/src/pybdsim/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 +-----------------+----------------------------------------------------------+
 | Constants       | Constants.                                               |
 +-----------------+----------------------------------------------------------+
 | Convert         | Convert other formats into gmad.                         |
 +-----------------+----------------------------------------------------------+
 | Data            | Read the bdsim output formats.                           |
 +-----------------+----------------------------------------------------------+
-| DataUproot      | Data loading with uproot instead of pyroot.              |
+| DataUproot      | Data loading with uproot instead of pyroot. (optional)   |
 +-----------------+----------------------------------------------------------+
 | Field           | Read and write BDSIM field format files.                 |
 +-----------------+----------------------------------------------------------+
 | Geant4          | Dictionary that contains process and subprocess IDs      |
 +-----------------+----------------------------------------------------------+
 | Gmad            | Create bdsim input files - lattices & options.           |
 +-----------------+----------------------------------------------------------+
 | ModelProcessing | Tools to process existing BDSIM models and generate      |
 |                 | other versions of them.                                  |
 +-----------------+----------------------------------------------------------+
-| Optics          | Optical calculation in development.                      |
+| Optics          | Optical calculation in development. (optional)           |
 +-----------------+----------------------------------------------------------+
 | Options         | Methods to generate bdsim options.                       |
 +-----------------+----------------------------------------------------------+
 | Plot            | Some nice plots for data.                                |
 +-----------------+----------------------------------------------------------+
 | Run             | Run BDSIM programatically.                               |
 +-----------------+----------------------------------------------------------+
@@ -48,54 +48,59 @@
 +-------------+--------------------------------------------------------------+
 | XSecBias    | A cross-section biasing object.                              |
 +-------------+--------------------------------------------------------------+
 
 """
 
 try:
-    from ._version import version as __version__
-    from ._version import version_tuple
+    from ._version import __version__
+    from ._version import __version_tuple__
 except ImportError:
     __version__ = "unknown version"
-    version_tuple = (0, 0, "unknown version")
+    __version_tuple__ = (0, 0, "unknown version")
 
 from . import Beam
 from . import Builder
 from . import Constants
 from . import Convert
 from . import Compare
 from . import Data
-from . import DataUproot
 from . import Field
 from . import Geant4
 from . import Gmad
 from . import Options
 from . import Plot
 from . import Run
 from . import ModelProcessing
 from . import Visualisation
 from . import XSecBias
 from . import _General
 
-try:
-    from . import Optics
-except:
-    pass
-
 __all__ = ['Beam',
            'Builder',
            'Constants',
            'Convert',
            'Compare',
            'Data',
            'DataUproot',
            'Field',
            'Geant4',
            'Gmad',
-           'Optics',
            'Options',
            'Plot',
            'Run',
            'ModelProcessing',
            'Visualisation',
            'XSecBias',
            '_General']
+
+try:
+    from . import Optics
+    __all__.append("Optics")
+except:
+    pass
+
+try:
+    from . import DataUproot
+    __all__.append("DataUproot")
+except:
+    pass
```

### Comparing `pybdsim-3.1.0/src/pybdsim.egg-info/PKG-INFO` & `pybdsim-3.1.1/src/pybdsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.1.0/src/pybdsim.egg-info/SOURCES.txt` & `pybdsim-3.1.1/src/pybdsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz` & `pybdsim-3.1.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_input/model-model-aper.tfs.gz` & `pybdsim-3.1.1/tests/test_input/model-model-aper.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_input/model-model.tfs.gz` & `pybdsim-3.1.1/tests/test_input/model-model.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output/model-model/model_components.gmad` & `pybdsim-3.1.1/tests/test_output/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output/model-model/model_sequence.gmad` & `pybdsim-3.1.1/tests/test_output/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output2/model-model/model_components.gmad` & `pybdsim-3.1.1/tests/test_output2/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/test_output2/model-model/model_sequence.gmad` & `pybdsim-3.1.1/tests/test_output2/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/tests/pybdsim_test_utils.py` & `pybdsim-3.1.1/tests/tests/pybdsim_test_utils.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/tests/test_MadxTfs2Gmad.py` & `pybdsim-3.1.1/tests/tests/test_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/tests/testratio.py` & `pybdsim-3.1.1/tests/tests/testratio.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/tests/write_test_outputs.py` & `pybdsim-3.1.1/tests/tests/write_test_outputs.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.0/tests/unit/test_Builder.py` & `pybdsim-3.1.1/tests/unit/test_Builder.py`

 * *Files identical despite different names*

