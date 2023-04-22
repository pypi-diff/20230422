# Comparing `tmp/solvation-analysis-0.3.3.tar.gz` & `tmp/solvation-analysis-0.3.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvation-analysis-0.3.3.tar", last modified: Sat Apr 22 01:15:01 2023, max compression
+gzip compressed data, was "solvation-analysis-0.3.3a0.tar", last modified: Sun Apr  9 17:47:02 2023, max compression
```

## Comparing `solvation-analysis-0.3.3.tar` & `solvation-analysis-0.3.3a0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.534945 solvation-analysis-0.3.3/
--rw-r--r--   0 orioncohen   (505) staff       (20)     8081 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 orioncohen   (505) staff       (20)    34684 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/LICENSE
--rw-r--r--   0 orioncohen   (505) staff       (20)      234 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/MANIFEST.in
--rw-r--r--   0 orioncohen   (505) staff       (20)    44841 2023-04-22 01:15:01.169394 solvation-analysis-0.3.3/PKG-INFO
--rw-r--r--   0 orioncohen   (505) staff       (20)     3938 2023-04-17 16:04:27.000000 solvation-analysis-0.3.3/README.md
--rw-r--r--   0 orioncohen   (505) staff       (20)     1926 2023-04-09 20:16:08.000000 solvation-analysis-0.3.3/pyproject.toml
--rw-r--r--   0 orioncohen   (505) staff       (20)      106 2023-04-09 18:08:15.000000 solvation-analysis-0.3.3/requirements.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)      381 2023-04-22 01:15:01.170466 solvation-analysis-0.3.3/setup.cfg
--rw-r--r--   0 orioncohen   (505) staff       (20)     2400 2023-04-05 15:18:21.000000 solvation-analysis-0.3.3/setup.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:15:01.170790 solvation-analysis-0.3.3/solvation_analysis/
--rw-r--r--   0 orioncohen   (505) staff       (20)      335 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/__init__.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      728 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/_column_names.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     8016 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/_utils.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      498 2023-04-22 01:15:01.170885 solvation-analysis-0.3.3/solvation_analysis/_version.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     6570 2023-04-09 17:43:35.000000 solvation-analysis-0.3.3/solvation_analysis/coordination.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10777 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3/solvation_analysis/networking.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     5709 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3/solvation_analysis/pairing.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    13759 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3/solvation_analysis/plotting.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    11231 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/rdf_parser.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    11027 2023-04-09 19:15:47.000000 solvation-analysis-0.3.3/solvation_analysis/residence.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    38245 2023-02-14 18:50:22.000000 solvation-analysis-0.3.3/solvation_analysis/solute.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     8970 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3/solvation_analysis/speciation.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.481790 solvation-analysis-0.3.3/solvation_analysis/tests/
--rw-r--r--   0 orioncohen   (505) staff       (20)      112 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/__init__.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     9536 2023-04-09 18:55:54.000000 solvation-analysis-0.3.3/solvation_analysis/tests/conftest.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.482556 solvation-analysis-0.3.3/solvation_analysis/tests/data/
--rw-r--r--   0 orioncohen   (505) staff       (20)     8196 2022-10-02 21:12:27.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/.DS_Store
--rw-r--r--   0 orioncohen   (505) staff       (20)     2848 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/README.md
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.488237 solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)  1418421 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec.data
--rw-r--r--   0 orioncohen   (505) staff       (20)    14285 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec_elements.csv
--rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)  5563748 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.497284 solvation-analysis-0.3.3/solvation_analysis/tests/data/ea_fec_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)   892516 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   761309 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.468963 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.499930 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/ea/
--rw-r--r--   0 orioncohen   (505) staff       (20)   871090 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/ea/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1023556 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.503357 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/eaf/
--rw-r--r--   0 orioncohen   (505) staff       (20)   874261 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/eaf/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1027396 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.506357 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/fea/
--rw-r--r--   0 orioncohen   (505) staff       (20)   875050 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/fea/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1028356 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.509358 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/feaf/
--rw-r--r--   0 orioncohen   (505) staff       (20)   876623 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/feaf/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1030276 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.512395 solvation-analysis-0.3.3/solvation_analysis/tests/data/iba_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)   721156 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   610100 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.523493 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.530211 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:14:39.534751 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)     2601 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3/solvation_analysis/tests/datafiles.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1596 2023-04-09 17:25:23.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_coordination.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      867 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_networking.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1516 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_pairing.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10037 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_plotting.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     6317 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_rdf_parser.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      961 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_residence.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     4012 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_selection.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    12563 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_solute.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1572 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3/solvation_analysis/tests/test_speciation.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-22 01:15:01.164160 solvation-analysis-0.3.3/solvation_analysis.egg-info/
--rw-r--r--   0 orioncohen   (505) staff       (20)    44841 2023-04-22 01:15:01.000000 solvation-analysis-0.3.3/solvation_analysis.egg-info/PKG-INFO
--rw-r--r--   0 orioncohen   (505) staff       (20)     7068 2023-04-22 01:15:01.000000 solvation-analysis-0.3.3/solvation_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)        1 2023-04-22 01:15:01.000000 solvation-analysis-0.3.3/solvation_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)       88 2023-04-22 01:15:01.000000 solvation-analysis-0.3.3/solvation_analysis.egg-info/requires.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)       19 2023-04-22 01:15:01.000000 solvation-analysis-0.3.3/solvation_analysis.egg-info/top_level.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)    78254 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3/versioneer.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.534578 solvation-analysis-0.3.3a0/
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8081 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 orioncohen   (505) staff       (20)    34684 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/LICENSE
+-rw-r--r--   0 orioncohen   (505) staff       (20)      234 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/MANIFEST.in
+-rw-r--r--   0 orioncohen   (505) staff       (20)    44784 2023-04-09 17:47:02.983612 solvation-analysis-0.3.3a0/PKG-INFO
+-rw-r--r--   0 orioncohen   (505) staff       (20)     3879 2023-04-02 16:17:13.000000 solvation-analysis-0.3.3a0/README.md
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1925 2023-04-09 17:20:57.000000 solvation-analysis-0.3.3a0/pyproject.toml
+-rw-r--r--   0 orioncohen   (505) staff       (20)      106 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/requirements.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)      381 2023-04-09 17:47:02.984218 solvation-analysis-0.3.3a0/setup.cfg
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2400 2023-04-05 15:18:21.000000 solvation-analysis-0.3.3a0/setup.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:47:02.984917 solvation-analysis-0.3.3a0/solvation_analysis/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      335 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/__init__.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      728 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/_column_names.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8016 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/_utils.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      504 2023-04-09 17:47:02.984993 solvation-analysis-0.3.3a0/solvation_analysis/_version.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     6570 2023-04-09 17:43:35.000000 solvation-analysis-0.3.3a0/solvation_analysis/coordination.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10777 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/networking.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     5709 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/pairing.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    13759 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/plotting.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    11231 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/rdf_parser.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10944 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/residence.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    38245 2023-02-14 18:50:22.000000 solvation-analysis-0.3.3a0/solvation_analysis/solute.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8970 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/speciation.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.472765 solvation-analysis-0.3.3a0/solvation_analysis/tests/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      112 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/__init__.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     9536 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/conftest.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.474241 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8196 2022-10-02 21:12:27.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/.DS_Store
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2848 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/README.md
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.481722 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1418421 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec.data
+-rw-r--r--   0 orioncohen   (505) staff       (20)    14285 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_elements.csv
+-rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)  5563748 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.496293 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   892516 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   761309 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.450151 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.500539 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   871090 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1023556 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.503346 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   874261 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1027396 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.506236 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   875050 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1028356 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.509482 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   876623 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1030276 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.512342 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   721156 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   610100 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.525390 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.529744 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:46:45.534331 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2601 2022-09-27 18:34:04.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/datafiles.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1596 2023-04-09 17:25:23.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_coordination.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      867 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_networking.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1516 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_pairing.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10037 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_plotting.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     6317 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_rdf_parser.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      961 2023-02-14 18:28:50.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_residence.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     4012 2022-10-28 18:42:42.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_selection.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    12563 2023-04-02 16:08:07.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_solute.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1572 2023-04-06 16:18:52.000000 solvation-analysis-0.3.3a0/solvation_analysis/tests/test_speciation.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2023-04-09 17:47:02.980183 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/
+-rw-r--r--   0 orioncohen   (505) staff       (20)    44784 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 orioncohen   (505) staff       (20)     7068 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)        1 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)       88 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/requires.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)       19 2023-04-09 17:47:02.000000 solvation-analysis-0.3.3a0/solvation_analysis.egg-info/top_level.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)    78254 2022-08-17 22:41:48.000000 solvation-analysis-0.3.3a0/versioneer.py
```

### Comparing `solvation-analysis-0.3.3/CODE_OF_CONDUCT.md` & `solvation-analysis-0.3.3a0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/LICENSE` & `solvation-analysis-0.3.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/PKG-INFO` & `solvation-analysis-0.3.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvation-analysis
-Version: 0.3.3
+Version: 0.3.3a0
 Summary: A toolkit to analyze solvation structure in molecular dynamics trajectories.
 Author: Orion Cohen
 Author-email: Orion Cohen <orioncohen@berkeley.edu>
 Maintainer-email: Orion Cohen <orioncohen@berkeley.edu>, Hugo MacDermott-Opeskin <hugomacdermott@gmail.com>
 License:                         GNU GENERAL PUBLIC LICENSE 
                                   Version 3, 29 June 2007
         
@@ -608,17 +608,15 @@
 [//]: # (Badges)
 
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://www.numfocus.org/)
 [![Powered by MDAnalysis](https://img.shields.io/badge/powered%20by-MDAnalysis-orange.svg?logoWidth=16&logo=data:image/x-icon;base64,AAABAAEAEBAAAAEAIAAoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJD+XwCY/fEAkf3uAJf97wGT/a+HfHaoiIWE7n9/f+6Hh4fvgICAjwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACT/yYAlP//AJ///wCg//8JjvOchXly1oaGhv+Ghob/j4+P/39/f3IAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJH8aQCY/8wAkv2kfY+elJ6al/yVlZX7iIiI8H9/f7h/f38UAAAAAAAAAAAAAAAAAAAAAAAAAAB/f38egYF/noqAebF8gYaagnx3oFpUUtZpaWr/WFhY8zo6OmT///8BAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgICAn46Ojv+Hh4b/jouJ/4iGhfcAAADnAAAA/wAAAP8AAADIAAAAAwCj/zIAnf2VAJD/PAAAAAAAAAAAAAAAAICAgNGHh4f/gICA/4SEhP+Xl5f/AwMD/wAAAP8AAAD/AAAA/wAAAB8Aov9/ALr//wCS/Z0AAAAAAAAAAAAAAACBgYGOjo6O/4mJif+Pj4//iYmJ/wAAAOAAAAD+AAAA/wAAAP8AAABhAP7+FgCi/38Axf4fAAAAAAAAAAAAAAAAiIiID4GBgYKCgoKogoB+fYSEgZhgYGDZXl5e/m9vb/9ISEjpEBAQxw8AAFQAAAAAAAAANQAAADcAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAjo6Mb5iYmP+cnJz/jY2N95CQkO4pKSn/AAAA7gAAAP0AAAD7AAAAhgAAAAEAAAAAAAAAAACL/gsAkv2uAJX/QQAAAAB9fX3egoKC/4CAgP+NjY3/c3Nz+wAAAP8AAAD/AAAA/wAAAPUAAAAcAAAAAAAAAAAAnP4NAJL9rgCR/0YAAAAAfX19w4ODg/98fHz/i4uL/4qKivwAAAD/AAAA/wAAAP8AAAD1AAAAGwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALGxsVyqqqr/mpqa/6mpqf9KSUn/AAAA5QAAAPkAAAD5AAAAhQAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADkUFBSuZ2dn/3V1df8uLi7bAAAATgBGfyQAAAA2AAAAMwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB0AAADoAAAA/wAAAP8AAAD/AAAAWgC3/2AAnv3eAJ/+dgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA9AAAA/wAAAP8AAAD/AAAA/wAKDzEAnP3WAKn//wCS/OgAf/8MAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIQAAANwAAADtAAAA7QAAAMAAABUMAJn9gwCe/e0Aj/2LAP//AQAAAAAAAAAA)](https://www.mdanalysis.org)
 [![GitHub Actions Status](https://github.com/MDAnalysis/solvation-analysis/workflows/CI/badge.svg)](https://github.com/MDAnalysis/solvation-analysis/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/MDAnalysis/solvation-analysis//branch/main/graph/badge.svg)](https://codecov.io/gh/MDAnalysis/solvation-analysis//branch/main)
 [![docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://solvation-analysis.readthedocs.io/en/latest/)
-[![pub](https://joss.theoj.org/papers/10.21105/joss.05183/status.svg)](https://doi.org/10.21105/joss.05183)
-
-[//]: # ([![DOI]&#40;https://zenodo.org/badge/371804402.svg&#41;]&#40;https://zenodo.org/badge/latestdoi/371804402&#41;)
+[![DOI](https://zenodo.org/badge/371804402.svg)](https://zenodo.org/badge/latestdoi/371804402)
 
 
 ---
 
 Solvation analysis implements a robust, cohesive, and fast set of methods
 for analyzing the solvation structure of a liquid. It seamlessly integrates with
 [MDAnalysis](https://www.mdanalysis.org/), making use of the core AtomGroup
@@ -637,20 +635,22 @@
 ```
 
 ### Contributing
 
 Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you 
 follow the community guidelines outlined in the [MDAnalysis Code of Conduct](https://www.mdanalysis.org/pages/conduct/).
 
-### Citation
+---
+
+#### Acknowledgements
 
-This work is described in [JOSS](https://doi.org/10.21105/joss.05183), please cite it if you make
-use of this package in published work.
+Google Summer of Code and the MDAnalysis team provided funding and support for this project.
 
----
+Main development by @orioncohen, with mentorship from @richardjgowers, @IAlibay, 
+@hmacdope, and @htz1992213.
 
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.5.
 
 
 
 [readthedocs]: (https://solvation-analysis.readthedocs.io/en/latest/)
```

### Comparing `solvation-analysis-0.3.3/README.md` & `solvation-analysis-0.3.3a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 [//]: # (Badges)
 
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://www.numfocus.org/)
 [![Powered by MDAnalysis](https://img.shields.io/badge/powered%20by-MDAnalysis-orange.svg?logoWidth=16&logo=data:image/x-icon;base64,AAABAAEAEBAAAAEAIAAoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJD+XwCY/fEAkf3uAJf97wGT/a+HfHaoiIWE7n9/f+6Hh4fvgICAjwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACT/yYAlP//AJ///wCg//8JjvOchXly1oaGhv+Ghob/j4+P/39/f3IAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJH8aQCY/8wAkv2kfY+elJ6al/yVlZX7iIiI8H9/f7h/f38UAAAAAAAAAAAAAAAAAAAAAAAAAAB/f38egYF/noqAebF8gYaagnx3oFpUUtZpaWr/WFhY8zo6OmT///8BAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgICAn46Ojv+Hh4b/jouJ/4iGhfcAAADnAAAA/wAAAP8AAADIAAAAAwCj/zIAnf2VAJD/PAAAAAAAAAAAAAAAAICAgNGHh4f/gICA/4SEhP+Xl5f/AwMD/wAAAP8AAAD/AAAA/wAAAB8Aov9/ALr//wCS/Z0AAAAAAAAAAAAAAACBgYGOjo6O/4mJif+Pj4//iYmJ/wAAAOAAAAD+AAAA/wAAAP8AAABhAP7+FgCi/38Axf4fAAAAAAAAAAAAAAAAiIiID4GBgYKCgoKogoB+fYSEgZhgYGDZXl5e/m9vb/9ISEjpEBAQxw8AAFQAAAAAAAAANQAAADcAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAjo6Mb5iYmP+cnJz/jY2N95CQkO4pKSn/AAAA7gAAAP0AAAD7AAAAhgAAAAEAAAAAAAAAAACL/gsAkv2uAJX/QQAAAAB9fX3egoKC/4CAgP+NjY3/c3Nz+wAAAP8AAAD/AAAA/wAAAPUAAAAcAAAAAAAAAAAAnP4NAJL9rgCR/0YAAAAAfX19w4ODg/98fHz/i4uL/4qKivwAAAD/AAAA/wAAAP8AAAD1AAAAGwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALGxsVyqqqr/mpqa/6mpqf9KSUn/AAAA5QAAAPkAAAD5AAAAhQAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADkUFBSuZ2dn/3V1df8uLi7bAAAATgBGfyQAAAA2AAAAMwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB0AAADoAAAA/wAAAP8AAAD/AAAAWgC3/2AAnv3eAJ/+dgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA9AAAA/wAAAP8AAAD/AAAA/wAKDzEAnP3WAKn//wCS/OgAf/8MAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIQAAANwAAADtAAAA7QAAAMAAABUMAJn9gwCe/e0Aj/2LAP//AQAAAAAAAAAA)](https://www.mdanalysis.org)
 [![GitHub Actions Status](https://github.com/MDAnalysis/solvation-analysis/workflows/CI/badge.svg)](https://github.com/MDAnalysis/solvation-analysis/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/MDAnalysis/solvation-analysis//branch/main/graph/badge.svg)](https://codecov.io/gh/MDAnalysis/solvation-analysis//branch/main)
 [![docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://solvation-analysis.readthedocs.io/en/latest/)
-[![pub](https://joss.theoj.org/papers/10.21105/joss.05183/status.svg)](https://doi.org/10.21105/joss.05183)
-
-[//]: # ([![DOI]&#40;https://zenodo.org/badge/371804402.svg&#41;]&#40;https://zenodo.org/badge/latestdoi/371804402&#41;)
+[![DOI](https://zenodo.org/badge/371804402.svg)](https://zenodo.org/badge/latestdoi/371804402)
 
 
 ---
 
 Solvation analysis implements a robust, cohesive, and fast set of methods
 for analyzing the solvation structure of a liquid. It seamlessly integrates with
 [MDAnalysis](https://www.mdanalysis.org/), making use of the core AtomGroup
@@ -32,20 +30,22 @@
 ```
 
 ### Contributing
 
 Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you 
 follow the community guidelines outlined in the [MDAnalysis Code of Conduct](https://www.mdanalysis.org/pages/conduct/).
 
-### Citation
+---
+
+#### Acknowledgements
 
-This work is described in [JOSS](https://doi.org/10.21105/joss.05183), please cite it if you make
-use of this package in published work.
+Google Summer of Code and the MDAnalysis team provided funding and support for this project.
 
----
+Main development by @orioncohen, with mentorship from @richardjgowers, @IAlibay, 
+@hmacdope, and @htz1992213.
 
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.5.
 
 
 
 [readthedocs]: (https://solvation-analysis.readthedocs.io/en/latest/)
```

### Comparing `solvation-analysis-0.3.3/pyproject.toml` & `solvation-analysis-0.3.3a0/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 
 
 [project.urls]
 Documentation = 'https://solvation-analysis.readthedocs.io'
 "Issue Tracker" = 'https://github.com/MDAnalysis/solvation-analysis/issues'
-Source = 'https://github.com/MDAnalysis/solvation-analysis'
+Source = 'https://github.com/MDAnalysis/solvation-analysis'
```

### Comparing `solvation-analysis-0.3.3/setup.py` & `solvation-analysis-0.3.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/_column_names.py` & `solvation-analysis-0.3.3a0/solvation_analysis/_column_names.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/_utils.py` & `solvation-analysis-0.3.3a0/solvation_analysis/_utils.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/coordination.py` & `solvation-analysis-0.3.3a0/solvation_analysis/coordination.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/networking.py` & `solvation-analysis-0.3.3a0/solvation_analysis/networking.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/pairing.py` & `solvation-analysis-0.3.3a0/solvation_analysis/pairing.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/plotting.py` & `solvation-analysis-0.3.3a0/solvation_analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/rdf_parser.py` & `solvation-analysis-0.3.3a0/solvation_analysis/rdf_parser.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/residence.py` & `solvation-analysis-0.3.3a0/solvation_analysis/residence.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,16 +113,14 @@
 
     def _calculate_auto_covariance_dict(self):
         partial_index = self.solvation_data.index.droplevel(SOLVENT_ATOM_IX)
         unique_indices = np.unique(partial_index)
         frame_solute_index = pd.MultiIndex.from_tuples(unique_indices, names=partial_index.names)
         auto_covariance_dict = {}
         for res_name, res_solvation_data in self.solvation_data.groupby([SOLVENT]):
-            if isinstance(res_name, tuple):
-                res_name = res_name[0]
             adjacency_mini = calculate_adjacency_dataframe(res_solvation_data)
             adjacency_df = adjacency_mini.reindex(frame_solute_index, fill_value=0)
             auto_covariance = Residence._calculate_auto_covariance(adjacency_df)
             # normalize
             auto_covariance = auto_covariance / np.max(auto_covariance)
             auto_covariance_dict[res_name] = auto_covariance
         return auto_covariance_dict
```

### Comparing `solvation-analysis-0.3.3/solvation_analysis/solute.py` & `solvation-analysis-0.3.3a0/solvation_analysis/solute.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/speciation.py` & `solvation-analysis-0.3.3a0/solvation_analysis/speciation.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/conftest.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/.DS_Store` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/README.md` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec.data` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec.data`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/ea/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/eaf/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/fea/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/feaf/topology.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/datafiles.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/datafiles.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_coordination.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_networking.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_pairing.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_pairing.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_plotting.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_rdf_parser.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_rdf_parser.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_residence.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_residence.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_selection.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_solute.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_solute.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis/tests/test_speciation.py` & `solvation-analysis-0.3.3a0/solvation_analysis/tests/test_speciation.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/solvation_analysis.egg-info/PKG-INFO` & `solvation-analysis-0.3.3a0/solvation_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvation-analysis
-Version: 0.3.3
+Version: 0.3.3a0
 Summary: A toolkit to analyze solvation structure in molecular dynamics trajectories.
 Author: Orion Cohen
 Author-email: Orion Cohen <orioncohen@berkeley.edu>
 Maintainer-email: Orion Cohen <orioncohen@berkeley.edu>, Hugo MacDermott-Opeskin <hugomacdermott@gmail.com>
 License:                         GNU GENERAL PUBLIC LICENSE 
                                   Version 3, 29 June 2007
         
@@ -608,17 +608,15 @@
 [//]: # (Badges)
 
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://www.numfocus.org/)
 [![Powered by MDAnalysis](https://img.shields.io/badge/powered%20by-MDAnalysis-orange.svg?logoWidth=16&logo=data:image/x-icon;base64,AAABAAEAEBAAAAEAIAAoBAAAFgAAACgAAAAQAAAAIAAAAAEAIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJD+XwCY/fEAkf3uAJf97wGT/a+HfHaoiIWE7n9/f+6Hh4fvgICAjwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACT/yYAlP//AJ///wCg//8JjvOchXly1oaGhv+Ghob/j4+P/39/f3IAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAJH8aQCY/8wAkv2kfY+elJ6al/yVlZX7iIiI8H9/f7h/f38UAAAAAAAAAAAAAAAAAAAAAAAAAAB/f38egYF/noqAebF8gYaagnx3oFpUUtZpaWr/WFhY8zo6OmT///8BAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAgICAn46Ojv+Hh4b/jouJ/4iGhfcAAADnAAAA/wAAAP8AAADIAAAAAwCj/zIAnf2VAJD/PAAAAAAAAAAAAAAAAICAgNGHh4f/gICA/4SEhP+Xl5f/AwMD/wAAAP8AAAD/AAAA/wAAAB8Aov9/ALr//wCS/Z0AAAAAAAAAAAAAAACBgYGOjo6O/4mJif+Pj4//iYmJ/wAAAOAAAAD+AAAA/wAAAP8AAABhAP7+FgCi/38Axf4fAAAAAAAAAAAAAAAAiIiID4GBgYKCgoKogoB+fYSEgZhgYGDZXl5e/m9vb/9ISEjpEBAQxw8AAFQAAAAAAAAANQAAADcAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAjo6Mb5iYmP+cnJz/jY2N95CQkO4pKSn/AAAA7gAAAP0AAAD7AAAAhgAAAAEAAAAAAAAAAACL/gsAkv2uAJX/QQAAAAB9fX3egoKC/4CAgP+NjY3/c3Nz+wAAAP8AAAD/AAAA/wAAAPUAAAAcAAAAAAAAAAAAnP4NAJL9rgCR/0YAAAAAfX19w4ODg/98fHz/i4uL/4qKivwAAAD/AAAA/wAAAP8AAAD1AAAAGwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAALGxsVyqqqr/mpqa/6mpqf9KSUn/AAAA5QAAAPkAAAD5AAAAhQAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADkUFBSuZ2dn/3V1df8uLi7bAAAATgBGfyQAAAA2AAAAMwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAB0AAADoAAAA/wAAAP8AAAD/AAAAWgC3/2AAnv3eAJ/+dgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA9AAAA/wAAAP8AAAD/AAAA/wAKDzEAnP3WAKn//wCS/OgAf/8MAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIQAAANwAAADtAAAA7QAAAMAAABUMAJn9gwCe/e0Aj/2LAP//AQAAAAAAAAAA)](https://www.mdanalysis.org)
 [![GitHub Actions Status](https://github.com/MDAnalysis/solvation-analysis/workflows/CI/badge.svg)](https://github.com/MDAnalysis/solvation-analysis/actions?query=workflow%3ACI)
 [![codecov](https://codecov.io/gh/MDAnalysis/solvation-analysis//branch/main/graph/badge.svg)](https://codecov.io/gh/MDAnalysis/solvation-analysis//branch/main)
 [![docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://solvation-analysis.readthedocs.io/en/latest/)
-[![pub](https://joss.theoj.org/papers/10.21105/joss.05183/status.svg)](https://doi.org/10.21105/joss.05183)
-
-[//]: # ([![DOI]&#40;https://zenodo.org/badge/371804402.svg&#41;]&#40;https://zenodo.org/badge/latestdoi/371804402&#41;)
+[![DOI](https://zenodo.org/badge/371804402.svg)](https://zenodo.org/badge/latestdoi/371804402)
 
 
 ---
 
 Solvation analysis implements a robust, cohesive, and fast set of methods
 for analyzing the solvation structure of a liquid. It seamlessly integrates with
 [MDAnalysis](https://www.mdanalysis.org/), making use of the core AtomGroup
@@ -637,20 +635,22 @@
 ```
 
 ### Contributing
 
 Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you 
 follow the community guidelines outlined in the [MDAnalysis Code of Conduct](https://www.mdanalysis.org/pages/conduct/).
 
-### Citation
+---
+
+#### Acknowledgements
 
-This work is described in [JOSS](https://doi.org/10.21105/joss.05183), please cite it if you make
-use of this package in published work.
+Google Summer of Code and the MDAnalysis team provided funding and support for this project.
 
----
+Main development by @orioncohen, with mentorship from @richardjgowers, @IAlibay, 
+@hmacdope, and @htz1992213.
 
 Project based on the 
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.5.
 
 
 
 [readthedocs]: (https://solvation-analysis.readthedocs.io/en/latest/)
```

### Comparing `solvation-analysis-0.3.3/solvation_analysis.egg-info/SOURCES.txt` & `solvation-analysis-0.3.3a0/solvation_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.3/versioneer.py` & `solvation-analysis-0.3.3a0/versioneer.py`

 * *Files identical despite different names*

