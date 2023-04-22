# Comparing `tmp/openpy_dsse-0.1.3.tar.gz` & `tmp/openpy_dsse-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpy_dsse-0.1.3.tar", max compression
+gzip compressed data, was "openpy_dsse-0.1.4.tar", max compression
```

## Comparing `openpy_dsse-0.1.3.tar` & `openpy_dsse-0.1.4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
--rw-r--r--   0        0        0     3255 2022-11-28 15:56:42.954000 openpy_dsse-0.1.3/LICENSE.md
--rw-r--r--   0        0        0       68 2022-10-25 18:54:21.476000 openpy_dsse-0.1.3/openpy_dsse/__init__.py
--rw-r--r--   0        0        0    12460 2022-12-30 19:55:22.918000 openpy_dsse-0.1.3/openpy_dsse/Algorithm_classification.py
--rw-r--r--   0        0        0     3916 2023-01-24 14:02:27.992000 openpy_dsse-0.1.3/openpy_dsse/base_DSSE.py
--rw-r--r--   0        0        0      255 2023-04-22 18:55:29.365000 openpy_dsse-0.1.3/openpy_dsse/COM_interface.py
--rw-r--r--   0        0        0       58 2022-10-11 19:54:20.428000 openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/__init__.py
--rw-r--r--   0        0        0       60 2022-10-11 19:55:20.245000 openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/Symb_Eqn/__init__.py
--rw-r--r--   0        0        0    18842 2022-08-18 21:16:16.722000 openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py
--rw-r--r--   0        0        0    19333 2022-09-19 23:51:10.547000 openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py
--rw-r--r--   0        0        0    41959 2022-12-29 18:05:55.584000 openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py
--rw-r--r--   0        0        0    35828 2022-12-16 18:46:00.112000 openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py
--rw-r--r--   0        0        0     4499 2022-12-31 17:30:43.970000 openpy_dsse-0.1.3/openpy_dsse/Elec_param_calc_DSS_EST.py
--rw-r--r--   0        0        0     6686 2022-12-30 20:48:27.487000 openpy_dsse-0.1.3/openpy_dsse/error_handling_logging.py
--rw-r--r--   0        0        0     2638 2022-10-25 16:23:23.002000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0     1605 2022-10-25 15:43:42.867000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0     3421 2022-10-25 16:09:48.529000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0     2977 2022-10-25 15:43:42.868000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0     5580 2023-03-08 19:04:07.333000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0     2905 2023-03-08 19:04:07.367000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     4660 2023-03-08 19:04:07.351000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0     3341 2023-03-08 19:04:07.389000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     3163 2022-10-25 16:31:50.272000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
--rw-r--r--   0        0        0     1280 2022-10-25 16:31:50.273000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     2570 2022-10-25 16:31:50.272000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
--rw-r--r--   0        0        0     1805 2022-10-25 16:31:50.273000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0      137 2022-09-18 23:25:43.017000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Capacitors.DSS
--rw-r--r--   0        0        0       13 2023-01-02 13:26:33.881000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
--rw-r--r--   0        0        0      243 2021-02-04 02:25:46.000000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Node_BusXY.csv
--rw-r--r--   0        0        0     1856 2023-01-02 13:26:23.711000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl
--rw-r--r--   0        0        0     1850 2023-01-02 13:26:23.711000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV
--rw-r--r--   0        0        0    11851 2021-02-04 02:25:46.000000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS
--rw-r--r--   0        0        0     2127 2022-09-18 23:29:29.878000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss
--rw-r--r--   0        0        0     1133 2022-09-19 00:03:40.591000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS
--rw-r--r--   0        0        0     1582 2022-09-19 01:59:14.562000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS
--rw-r--r--   0        0        0      519 2023-01-02 13:26:18.681000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss
--rw-r--r--   0        0        0      187 2023-03-08 19:04:07.640000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
--rw-r--r--   0        0        0       51 2023-03-08 19:04:07.629000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
--rw-r--r--   0        0        0      124 2022-10-24 15:17:02.027000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Capacitor.DSS
--rw-r--r--   0        0        0       13 2022-10-24 15:19:09.160000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/DSSViewIntercom.Txt
--rw-r--r--   0        0        0      143 2023-03-08 19:04:07.655000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
--rw-r--r--   0        0        0       71 2023-03-08 19:04:07.547000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
--rw-r--r--   0        0        0      768 2022-10-24 15:19:05.446000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl
--rw-r--r--   0        0        0     1739 2022-10-24 15:19:05.446000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV
--rw-r--r--   0        0        0     1840 2023-03-08 19:04:07.607000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
--rw-r--r--   0        0        0    10823 2023-03-08 19:04:07.525000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
--rw-r--r--   0        0        0     1472 2023-03-08 19:04:07.620000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
--rw-r--r--   0        0        0      197 2023-03-08 19:04:07.537000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
--rw-r--r--   0        0        0      355 2023-03-08 19:04:07.667000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
--rw-r--r--   0        0        0     1008 2023-03-08 19:04:07.592000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
--rw-r--r--   0        0        0     1180 2023-03-08 19:04:07.582000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
--rw-r--r--   0        0        0      128 2023-03-08 19:04:07.498000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
--rw-r--r--   0        0        0      541 2022-09-18 23:20:45.219000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS
--rw-r--r--   0        0        0      134 2022-09-18 23:27:42.311000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Switchs.DSS
--rw-r--r--   0        0        0      219 2022-09-18 23:22:54.457000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Transformers.DSS
--rw-r--r--   0        0        0      724 2022-09-18 23:21:47.993000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS
--rw-r--r--   0        0        0    78005 2023-03-08 19:04:14.530000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png
--rw-r--r--   0        0        0      416 2023-03-08 19:04:11.395000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json
--rw-r--r--   0        0        0     2155 2023-03-08 19:04:10.919000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json
--rw-r--r--   0        0        0     2568 2023-03-08 19:04:11.281000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json
--rw-r--r--   0        0        0    73688 2023-03-08 19:04:13.212000 openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png
--rw-r--r--   0        0        0     3074 2023-04-22 18:56:15.994000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0     1889 2023-04-22 18:56:16.050000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0     4133 2023-04-22 18:56:16.023000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0     3615 2023-04-22 18:56:16.079000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0     5669 2023-04-22 18:56:16.572000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0     3419 2023-04-22 18:56:16.603000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     5287 2023-04-22 18:56:16.587000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0     4097 2023-04-22 18:56:16.616000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     1304 2022-08-20 19:35:36.127000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss
--rw-r--r--   0        0        0      993 2022-08-20 19:35:59.738000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss
--rw-r--r--   0        0        0      155 2022-10-12 15:04:24.931000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Master_15node.dss
--rw-r--r--   0        0        0       37 2022-08-19 21:16:18.326000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Voltagebases_15node.dss
--rw-r--r--   0        0        0       71 2022-08-20 19:34:33.391000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Vsource_15node.dss
--rw-r--r--   0        0        0    84900 2023-03-08 19:07:30.754000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png
--rw-r--r--   0        0        0      417 2023-03-08 19:07:28.003000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json
--rw-r--r--   0        0        0     2512 2023-03-08 19:07:27.801000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json
--rw-r--r--   0        0        0     3149 2023-03-08 19:07:27.922000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json
--rw-r--r--   0        0        0    71312 2023-03-08 19:07:29.069000 openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png
--rw-r--r--   0        0        0     7337 2022-10-24 16:14:11.101000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0     4457 2022-10-24 17:34:20.149000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0     9994 2022-10-24 16:20:09.853000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0     8699 2022-10-24 15:46:49.590000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0    15079 2023-03-08 19:05:36.302000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0     8672 2023-03-08 19:05:36.328000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0    13354 2023-03-08 19:05:36.318000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0     9644 2023-03-08 19:05:36.336000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     8654 2022-10-25 15:22:33.314000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
--rw-r--r--   0        0        0     3827 2022-10-25 15:22:33.315000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     7342 2022-10-25 15:22:33.315000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
--rw-r--r--   0        0        0     5164 2022-10-25 15:22:33.316000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     1745 2022-09-20 18:34:51.235000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS
--rw-r--r--   0        0        0       10 2022-12-14 03:15:52.032000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
--rw-r--r--   0        0        0      755 2021-02-04 01:25:46.000000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv
--rw-r--r--   0        0        0     1759 2022-09-20 18:37:06.672000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt
--rw-r--r--   0        0        0     6720 2022-12-14 03:15:50.718000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl
--rw-r--r--   0        0        0     4951 2022-12-14 03:15:50.718000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV
--rw-r--r--   0        0        0    11851 2021-02-04 01:25:46.000000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS
--rw-r--r--   0        0        0     2936 2022-09-20 18:39:03.897000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS
--rw-r--r--   0        0        0     3645 2022-09-20 18:33:23.217000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS
--rw-r--r--   0        0        0      415 2022-12-14 03:15:46.530000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Master_ieee37.DSS
--rw-r--r--   0        0        0      640 2023-03-08 19:05:36.581000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
--rw-r--r--   0        0        0       50 2023-03-08 19:05:36.568000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
--rw-r--r--   0        0        0      396 2023-03-08 19:05:36.596000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
--rw-r--r--   0        0        0       71 2023-03-08 19:05:36.497000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
--rw-r--r--   0        0        0     5335 2023-03-08 19:05:36.548000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
--rw-r--r--   0        0        0     9171 2023-03-08 19:05:36.451000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
--rw-r--r--   0        0        0     3186 2023-03-08 19:05:36.560000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
--rw-r--r--   0        0        0      197 2023-03-08 19:05:36.464000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
--rw-r--r--   0        0        0      348 2023-03-08 19:05:36.607000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
--rw-r--r--   0        0        0     1008 2023-03-08 19:05:36.521000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
--rw-r--r--   0        0        0     1180 2023-03-08 19:05:36.511000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
--rw-r--r--   0        0        0      126 2023-03-08 19:05:36.423000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
--rw-r--r--   0        0        0      535 2022-09-20 16:18:55.459000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS
--rw-r--r--   0        0        0      195 2022-09-20 15:49:32.549000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Substation.DSS
--rw-r--r--   0        0        0      198 2022-09-20 15:49:47.451000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Transformers.DSS
--rw-r--r--   0        0        0   111900 2023-03-08 19:05:44.755000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png
--rw-r--r--   0        0        0      415 2023-03-08 19:05:41.528000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json
--rw-r--r--   0        0        0     6014 2023-03-08 19:05:41.138000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json
--rw-r--r--   0        0        0     7374 2023-03-08 19:05:41.462000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json
--rw-r--r--   0        0        0    89028 2023-03-08 19:05:43.312000 openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png
--rw-r--r--   0        0        0      806 2022-10-24 12:50:30.976000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0      479 2022-10-24 12:49:41.570000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0      808 2022-10-24 12:49:40.215000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0      693 2022-10-24 12:49:39.143000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0     1696 2023-03-03 16:29:22.817000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0      887 2023-03-03 16:29:22.869000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     1176 2023-03-03 16:29:22.831000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0      840 2023-03-03 16:29:22.884000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0      242 2022-10-09 12:19:31.150000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/OpenDSS files/Line_4node.dss
--rw-r--r--   0        0        0      234 2022-10-09 12:20:00.111000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/OpenDSS files/Load_4node.dss
--rw-r--r--   0        0        0      154 2022-10-09 12:20:12.673000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/OpenDSS files/Master_4node.dss
--rw-r--r--   0        0        0       34 2022-08-18 13:32:43.243000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/OpenDSS files/Voltagebases_4node.dss
--rw-r--r--   0        0        0       64 2022-08-18 13:36:08.540000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/OpenDSS files/Vsource_4node.dss
--rw-r--r--   0        0        0    68329 2023-04-22 18:57:17.715000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png
--rw-r--r--   0        0        0      417 2023-04-22 18:57:12.973000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Metrics_4Node.json
--rw-r--r--   0        0        0      653 2023-04-22 18:57:12.775000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Results_DSSE_4Node.json
--rw-r--r--   0        0        0      649 2023-04-22 18:57:12.875000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json
--rw-r--r--   0        0        0    70574 2023-04-22 18:57:15.748000 openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Vi_DSS_EST_PU_4Node.png
--rw-r--r--   0        0        0     3255 2022-10-25 18:55:11.503000 openpy_dsse-0.1.3/openpy_dsse/LICENSE.md
--rw-r--r--   0        0        0    98902 2022-12-16 18:06:54.863000 openpy_dsse-0.1.3/openpy_dsse/MEAS_from_OpenDSS.py
--rw-r--r--   0        0        0   177867 2023-01-24 14:35:24.540000 openpy_dsse-0.1.3/openpy_dsse/OpenDSS_data_extraction.py
--rw-r--r--   0        0        0     6324 2022-12-31 23:55:26.357000 openpy_dsse-0.1.3/openpy_dsse/perf_metrics_calc.py
--rw-r--r--   0        0        0     8151 2022-12-31 23:21:02.670000 openpy_dsse-0.1.3/openpy_dsse/Plot_results_DSS_EST.py
--rw-r--r--   0        0        0    14816 2022-12-16 18:46:00.245000 openpy_dsse-0.1.3/openpy_dsse/Readme.md
--rw-r--r--   0        0        0     2771 2022-12-13 21:37:20.521000 openpy_dsse-0.1.3/openpy_dsse/Sample_test_systems_DSS.py
--rw-r--r--   0        0        0    11515 2023-01-02 14:22:12.369000 openpy_dsse-0.1.3/openpy_dsse/state_estimation.py
--rw-r--r--   0        0        0     8227 2022-12-29 23:05:58.121000 openpy_dsse-0.1.3/openpy_dsse/YBus_Matrix_Pos_Seq.py
--rw-r--r--   0        0        0      999 2023-04-22 19:04:34.977000 openpy_dsse-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    15706 2023-04-22 15:09:09.407000 openpy_dsse-0.1.3/README.md
--rw-r--r--   0        0        0    50021 1970-01-01 00:00:00.000000 openpy_dsse-0.1.3/setup.py
--rw-r--r--   0        0        0    16846 1970-01-01 00:00:00.000000 openpy_dsse-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3255 2022-11-28 15:56:42.954000 openpy_dsse-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0       68 2023-04-22 20:18:54.031000 openpy_dsse-0.1.4/openpy_dsse/__init__.py
+-rw-r--r--   0        0        0    12460 2022-12-30 19:55:22.918000 openpy_dsse-0.1.4/openpy_dsse/Algorithm_classification.py
+-rw-r--r--   0        0        0     3916 2023-01-24 14:02:27.992000 openpy_dsse-0.1.4/openpy_dsse/base_DSSE.py
+-rw-r--r--   0        0        0      255 2023-04-22 18:55:29.365000 openpy_dsse-0.1.4/openpy_dsse/COM_interface.py
+-rw-r--r--   0        0        0       58 2022-10-11 19:54:20.428000 openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/__init__.py
+-rw-r--r--   0        0        0       60 2022-10-11 19:55:20.245000 openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/Symb_Eqn/__init__.py
+-rw-r--r--   0        0        0    18842 2022-08-18 21:16:16.722000 openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py
+-rw-r--r--   0        0        0    19333 2022-09-19 23:51:10.547000 openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py
+-rw-r--r--   0        0        0    41959 2022-12-29 18:05:55.584000 openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py
+-rw-r--r--   0        0        0    35828 2022-12-16 18:46:00.112000 openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py
+-rw-r--r--   0        0        0     4499 2022-12-31 17:30:43.970000 openpy_dsse-0.1.4/openpy_dsse/Elec_param_calc_DSS_EST.py
+-rw-r--r--   0        0        0     6686 2022-12-30 20:48:27.487000 openpy_dsse-0.1.4/openpy_dsse/error_handling_logging.py
+-rw-r--r--   0        0        0     2638 2022-10-25 16:23:23.002000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0     1605 2022-10-25 15:43:42.867000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0     3421 2022-10-25 16:09:48.529000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0     2977 2022-10-25 15:43:42.868000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     5580 2023-03-08 19:04:07.333000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0     2905 2023-03-08 19:04:07.367000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     4660 2023-03-08 19:04:07.351000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     3341 2023-03-08 19:04:07.389000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     3163 2022-10-25 16:31:50.272000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
+-rw-r--r--   0        0        0     1280 2022-10-25 16:31:50.273000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     2570 2022-10-25 16:31:50.272000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     1805 2022-10-25 16:31:50.273000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0      137 2022-09-18 23:25:43.017000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Capacitors.DSS
+-rw-r--r--   0        0        0       13 2023-01-02 13:26:33.881000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
+-rw-r--r--   0        0        0      243 2021-02-04 02:25:46.000000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Node_BusXY.csv
+-rw-r--r--   0        0        0     1856 2023-01-02 13:26:23.711000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl
+-rw-r--r--   0        0        0     1850 2023-01-02 13:26:23.711000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV
+-rw-r--r--   0        0        0    11851 2021-02-04 02:25:46.000000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS
+-rw-r--r--   0        0        0     2127 2022-09-18 23:29:29.878000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss
+-rw-r--r--   0        0        0     1133 2022-09-19 00:03:40.591000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS
+-rw-r--r--   0        0        0     1582 2022-09-19 01:59:14.562000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS
+-rw-r--r--   0        0        0      519 2023-01-02 13:26:18.681000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss
+-rw-r--r--   0        0        0      187 2023-03-08 19:04:07.640000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
+-rw-r--r--   0        0        0       51 2023-03-08 19:04:07.629000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
+-rw-r--r--   0        0        0      124 2022-10-24 15:17:02.027000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Capacitor.DSS
+-rw-r--r--   0        0        0       13 2022-10-24 15:19:09.160000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/DSSViewIntercom.Txt
+-rw-r--r--   0        0        0      143 2023-03-08 19:04:07.655000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
+-rw-r--r--   0        0        0       71 2023-03-08 19:04:07.547000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
+-rw-r--r--   0        0        0      768 2022-10-24 15:19:05.446000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl
+-rw-r--r--   0        0        0     1739 2022-10-24 15:19:05.446000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV
+-rw-r--r--   0        0        0     1840 2023-03-08 19:04:07.607000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
+-rw-r--r--   0        0        0    10823 2023-03-08 19:04:07.525000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
+-rw-r--r--   0        0        0     1472 2023-03-08 19:04:07.620000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
+-rw-r--r--   0        0        0      197 2023-03-08 19:04:07.537000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
+-rw-r--r--   0        0        0      355 2023-03-08 19:04:07.667000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
+-rw-r--r--   0        0        0     1008 2023-03-08 19:04:07.592000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
+-rw-r--r--   0        0        0     1180 2023-03-08 19:04:07.582000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
+-rw-r--r--   0        0        0      128 2023-03-08 19:04:07.498000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
+-rw-r--r--   0        0        0      541 2022-09-18 23:20:45.219000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS
+-rw-r--r--   0        0        0      134 2022-09-18 23:27:42.311000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Switchs.DSS
+-rw-r--r--   0        0        0      219 2022-09-18 23:22:54.457000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Transformers.DSS
+-rw-r--r--   0        0        0      724 2022-09-18 23:21:47.993000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS
+-rw-r--r--   0        0        0    78005 2023-03-08 19:04:14.530000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png
+-rw-r--r--   0        0        0      416 2023-03-08 19:04:11.395000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json
+-rw-r--r--   0        0        0     2155 2023-03-08 19:04:10.919000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json
+-rw-r--r--   0        0        0     2568 2023-03-08 19:04:11.281000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json
+-rw-r--r--   0        0        0    73688 2023-03-08 19:04:13.212000 openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png
+-rw-r--r--   0        0        0     3074 2023-04-22 18:56:15.994000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0     1889 2023-04-22 18:56:16.050000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0     4133 2023-04-22 18:56:16.023000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0     3615 2023-04-22 18:56:16.079000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     5669 2023-04-22 18:56:16.572000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0     3419 2023-04-22 18:56:16.603000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     5287 2023-04-22 18:56:16.587000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     4097 2023-04-22 18:56:16.616000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     1304 2022-08-20 19:35:36.127000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss
+-rw-r--r--   0        0        0      993 2022-08-20 19:35:59.738000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss
+-rw-r--r--   0        0        0      155 2022-10-12 15:04:24.931000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Master_15node.dss
+-rw-r--r--   0        0        0       37 2022-08-19 21:16:18.326000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Voltagebases_15node.dss
+-rw-r--r--   0        0        0       71 2022-08-20 19:34:33.391000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Vsource_15node.dss
+-rw-r--r--   0        0        0    84900 2023-03-08 19:07:30.754000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png
+-rw-r--r--   0        0        0      417 2023-03-08 19:07:28.003000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json
+-rw-r--r--   0        0        0     2512 2023-03-08 19:07:27.801000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json
+-rw-r--r--   0        0        0     3149 2023-03-08 19:07:27.922000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json
+-rw-r--r--   0        0        0    71312 2023-03-08 19:07:29.069000 openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png
+-rw-r--r--   0        0        0     7337 2022-10-24 16:14:11.101000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0     4457 2022-10-24 17:34:20.149000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0     9994 2022-10-24 16:20:09.853000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0     8699 2022-10-24 15:46:49.590000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0    15079 2023-03-08 19:05:36.302000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0     8672 2023-03-08 19:05:36.328000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0    13354 2023-03-08 19:05:36.318000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     9644 2023-03-08 19:05:36.336000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     8654 2022-10-25 15:22:33.314000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
+-rw-r--r--   0        0        0     3827 2022-10-25 15:22:33.315000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     7342 2022-10-25 15:22:33.315000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     5164 2022-10-25 15:22:33.316000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     1745 2022-09-20 18:34:51.235000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS
+-rw-r--r--   0        0        0       10 2022-12-14 03:15:52.032000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
+-rw-r--r--   0        0        0      755 2021-02-04 01:25:46.000000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv
+-rw-r--r--   0        0        0     1759 2022-09-20 18:37:06.672000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt
+-rw-r--r--   0        0        0     6720 2022-12-14 03:15:50.718000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl
+-rw-r--r--   0        0        0     4951 2022-12-14 03:15:50.718000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV
+-rw-r--r--   0        0        0    11851 2021-02-04 01:25:46.000000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS
+-rw-r--r--   0        0        0     2936 2022-09-20 18:39:03.897000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS
+-rw-r--r--   0        0        0     3645 2022-09-20 18:33:23.217000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS
+-rw-r--r--   0        0        0      415 2022-12-14 03:15:46.530000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Master_ieee37.DSS
+-rw-r--r--   0        0        0      640 2023-03-08 19:05:36.581000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
+-rw-r--r--   0        0        0       50 2023-03-08 19:05:36.568000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
+-rw-r--r--   0        0        0      396 2023-03-08 19:05:36.596000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
+-rw-r--r--   0        0        0       71 2023-03-08 19:05:36.497000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
+-rw-r--r--   0        0        0     5335 2023-03-08 19:05:36.548000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
+-rw-r--r--   0        0        0     9171 2023-03-08 19:05:36.451000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
+-rw-r--r--   0        0        0     3186 2023-03-08 19:05:36.560000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
+-rw-r--r--   0        0        0      197 2023-03-08 19:05:36.464000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
+-rw-r--r--   0        0        0      348 2023-03-08 19:05:36.607000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
+-rw-r--r--   0        0        0     1008 2023-03-08 19:05:36.521000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
+-rw-r--r--   0        0        0     1180 2023-03-08 19:05:36.511000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
+-rw-r--r--   0        0        0      126 2023-03-08 19:05:36.423000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
+-rw-r--r--   0        0        0      535 2022-09-20 16:18:55.459000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS
+-rw-r--r--   0        0        0      195 2022-09-20 15:49:32.549000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Substation.DSS
+-rw-r--r--   0        0        0      198 2022-09-20 15:49:47.451000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Transformers.DSS
+-rw-r--r--   0        0        0   111900 2023-03-08 19:05:44.755000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png
+-rw-r--r--   0        0        0      415 2023-03-08 19:05:41.528000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json
+-rw-r--r--   0        0        0     6014 2023-03-08 19:05:41.138000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json
+-rw-r--r--   0        0        0     7374 2023-03-08 19:05:41.462000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json
+-rw-r--r--   0        0        0    89028 2023-03-08 19:05:43.312000 openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png
+-rw-r--r--   0        0        0      806 2022-10-24 12:50:30.976000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0      479 2022-10-24 12:49:41.570000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0      808 2022-10-24 12:49:40.215000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0      693 2022-10-24 12:49:39.143000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     1696 2023-03-03 16:29:22.817000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0      887 2023-03-03 16:29:22.869000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     1176 2023-03-03 16:29:22.831000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0      840 2023-03-03 16:29:22.884000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0      242 2022-10-09 12:19:31.150000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/OpenDSS files/Line_4node.dss
+-rw-r--r--   0        0        0      234 2022-10-09 12:20:00.111000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/OpenDSS files/Load_4node.dss
+-rw-r--r--   0        0        0      154 2022-10-09 12:20:12.673000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/OpenDSS files/Master_4node.dss
+-rw-r--r--   0        0        0       34 2022-08-18 13:32:43.243000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/OpenDSS files/Voltagebases_4node.dss
+-rw-r--r--   0        0        0       64 2022-08-18 13:36:08.540000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/OpenDSS files/Vsource_4node.dss
+-rw-r--r--   0        0        0    68329 2023-04-22 18:57:17.715000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png
+-rw-r--r--   0        0        0      417 2023-04-22 18:57:12.973000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Metrics_4Node.json
+-rw-r--r--   0        0        0      653 2023-04-22 18:57:12.775000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Results_DSSE_4Node.json
+-rw-r--r--   0        0        0      649 2023-04-22 18:57:12.875000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json
+-rw-r--r--   0        0        0    70574 2023-04-22 18:57:15.748000 openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Vi_DSS_EST_PU_4Node.png
+-rw-r--r--   0        0        0     3255 2022-10-25 18:55:11.503000 openpy_dsse-0.1.4/openpy_dsse/LICENSE.md
+-rw-r--r--   0        0        0    98902 2022-12-16 18:06:54.863000 openpy_dsse-0.1.4/openpy_dsse/MEAS_from_OpenDSS.py
+-rw-r--r--   0        0        0   177867 2023-01-24 14:35:24.540000 openpy_dsse-0.1.4/openpy_dsse/OpenDSS_data_extraction.py
+-rw-r--r--   0        0        0     6324 2022-12-31 23:55:26.357000 openpy_dsse-0.1.4/openpy_dsse/perf_metrics_calc.py
+-rw-r--r--   0        0        0     8151 2022-12-31 23:21:02.670000 openpy_dsse-0.1.4/openpy_dsse/Plot_results_DSS_EST.py
+-rw-r--r--   0        0        0    14816 2022-12-16 18:46:00.245000 openpy_dsse-0.1.4/openpy_dsse/Readme.md
+-rw-r--r--   0        0        0     2771 2022-12-13 21:37:20.521000 openpy_dsse-0.1.4/openpy_dsse/Sample_test_systems_DSS.py
+-rw-r--r--   0        0        0    11515 2023-01-02 14:22:12.369000 openpy_dsse-0.1.4/openpy_dsse/state_estimation.py
+-rw-r--r--   0        0        0     8227 2022-12-29 23:05:58.121000 openpy_dsse-0.1.4/openpy_dsse/YBus_Matrix_Pos_Seq.py
+-rw-r--r--   0        0        0      999 2023-04-22 20:19:56.374000 openpy_dsse-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    15706 2023-04-22 15:09:09.407000 openpy_dsse-0.1.4/README.md
+-rw-r--r--   0        0        0    50021 1970-01-01 00:00:00.000000 openpy_dsse-0.1.4/setup.py
+-rw-r--r--   0        0        0    16846 1970-01-01 00:00:00.000000 openpy_dsse-0.1.4/PKG-INFO
```

### Comparing `openpy_dsse-0.1.3/LICENSE.md` & `openpy_dsse-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/Algorithm_classification.py` & `openpy_dsse-0.1.4/openpy_dsse/Algorithm_classification.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/base_DSSE.py` & `openpy_dsse-0.1.4/openpy_dsse/base_DSSE.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py` & `openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py` & `openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py` & `openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py` & `openpy_dsse-0.1.4/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/Elec_param_calc_DSS_EST.py` & `openpy_dsse-0.1.4/openpy_dsse/Elec_param_calc_DSS_EST.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/error_handling_logging.py` & `openpy_dsse-0.1.4/openpy_dsse/error_handling_logging.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Results_DSSE_4Node.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Results_DSSE_4Node.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/examples/4Node/Results/Vi_DSS_EST_PU_4Node.png` & `openpy_dsse-0.1.4/openpy_dsse/examples/4Node/Results/Vi_DSS_EST_PU_4Node.png`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/LICENSE.md` & `openpy_dsse-0.1.4/openpy_dsse/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/MEAS_from_OpenDSS.py` & `openpy_dsse-0.1.4/openpy_dsse/MEAS_from_OpenDSS.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/OpenDSS_data_extraction.py` & `openpy_dsse-0.1.4/openpy_dsse/OpenDSS_data_extraction.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/perf_metrics_calc.py` & `openpy_dsse-0.1.4/openpy_dsse/perf_metrics_calc.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/Plot_results_DSS_EST.py` & `openpy_dsse-0.1.4/openpy_dsse/Plot_results_DSS_EST.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/Readme.md` & `openpy_dsse-0.1.4/openpy_dsse/Readme.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/Sample_test_systems_DSS.py` & `openpy_dsse-0.1.4/openpy_dsse/Sample_test_systems_DSS.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/state_estimation.py` & `openpy_dsse-0.1.4/openpy_dsse/state_estimation.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/openpy_dsse/YBus_Matrix_Pos_Seq.py` & `openpy_dsse-0.1.4/openpy_dsse/YBus_Matrix_Pos_Seq.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/pyproject.toml` & `openpy_dsse-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openpy-dsse"
-version = "0.1.3"
+version = "0.1.4"
 description = "Open source library for state estimation of a distribution network modeled in OpenDSS"
 authors = ["Jorge Lara <jlara@iee.unsj.edu.ar>"]
 license = "LICENSE"
 readme = "README.md"
 keywords = ["OpenDSS", "DSSE", "state estimation", "smart grid", "OpenPy-DSSE", "OpenPy_DSSE"]
 
 packages = [{include = "openpy_dsse"}]
```

### Comparing `openpy_dsse-0.1.3/README.md` & `openpy_dsse-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.3/setup.py` & `openpy_dsse-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
  'scipy==1.9.3',
  'seaborn==0.12.1',
  'six==1.16.0',
  'sympy==1.11.1']
 
 setup_kwargs = {
     'name': 'openpy-dsse',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Open source library for state estimation of a distribution network modeled in OpenDSS',
     'long_description': '# OpenPY_DSSE\n\nIt is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks ([OpenDSS](https://sourceforge.net/projects/electricdss/)) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.\n\nIt is developed within the framework of the[ OpenREiD](https://iee-unsjconicet.org/reid/) project (Integral software for simulation and optimization of electrical distribution networks), of the [Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina](https://iee-unsjconicet.org/).\n\n**Index**\n\n- [Weighted Least Squares](#id0)\n- [Installation](#id1)\n- [How to use](#id2)\n  - [Measurements](#id3)\n    - [Definition and creation of meters](#id4)\n    - [Generate metrics from OpenDSS results](#id5)\n  - [Run the state estimation algorithm](#id6)\n  - [Sample tests](#id7)\n- [License](#id8)\n\n<div id=\'id0\' />\n\n## Weighted Least Squares (WLS)\n\nThe library uses a hybrid weighted least squares algorithm that incorporates traditional and D-PMU measurements. It supports single-phase and multiphase networks that are modeled as electromagnetically decoupled positive sequence impedances. More details can be found in [docs/methodology](https://github.com/jlara6/OpenPy-DSSE/blob/main/docs/methodology/Nonlinear_Hybrid_State_Estimator.ipynb)\n\n<div id=\'id1\' />\n\n## Installation\n\nWith pip\n\n``pip install py-open-dsse``\n\nWithout pip, clone or download the repository, in the dist folder is the .whl file, copy the location of the file, and in the CMD:\n\n``pip install {path-save-files}/openpy_dsse-{version}-py3-none-any.whl’``\n\n<div id=\'id2\'/>\n\n## How to use  <a name="id1"></a>\n\nFirst, in the IDE (Integrated Development Environment) of preference, we import the library:\n\n```Python\nimport openpy_dsse\n```\n\nThe object class that contains all the functions of the library is activated as follows:\n\n```Python\ndsse = openpy_dsse.init_DSSE()\n```\n\nThe class ``init_DSSE()``, has default values as shown in table 1 and can be modified as appropriate.\n\n**Table 1.** Description and attributes of function ``init_DSSE()``\n| **Parameters** | **Description** | **Default value** |\n|:---:|---|:---:|\n| ``Sbas3ph_MVA`` | Three-phase system base power     | ``30`` |\n| ``tolerance`` | Convergence tolerance of selected algorithm | ``1e-3`` |\n| ``max_iter`` | Maximum number of iterations of the selected algorithm | ``30`` |\n| ``init_values`` | Initial values for state estimation. With ``flat`` start with 1.0 p.u. / 0° on all buses and with ``dss`` start with OpenDSS voltage and angle results| ``flat`` |\n\nOnce the class is initialized, we can use the functions described below.\n\n<div id=\'id3\' />\n\n### Measurements\n\n<div id=\'id4\' />\n\n#### Definition and creation of meters\n\nThe library supports meters and their respective error variance described in Table 2.\n\n**Table 2.** Measurement type of the ``openpy_dsse`` library.\n\n|              **Meter**                 |                                **Description**                |\n|:--------------------------------------:|---------------------------------------------------------------|\n| $\\left\\|V_{i}\\right\\|$                 | Node voltage magnitude.                                       |\n| $PQ_{ft}$                              | Branch power flow                                             |\n| $\\left\\|I_{ft}\\right\\|$                | Magnitude of branch current.                                  |\n| $PQ_{i}^{SM}$                          | Injection power or node consumption obtained by a smart meter |\n| $PQ_{i}^{0}$                           | Passive node or zero injection power.                         |\n| $PQ_{i}^{PSD}$                         | Artificial node injection power known as pseudo-measurement   |\n| $\\left\\|V_{i}\\right\\|\\angle \\theta$    | Voltage phasor measurement                                    |\n| $\\left\\|I_{ft}\\right\\|\\angle \\delta$   | Current phasor measurement                                              |\n\nThe measurement data per phase **𝜌 (1, 2, 3)** and measurement error variance ``Rii`` of a network modeled in OpenDSS. They must be entered in the ``MEAS_Bus_i.json``, ``MEAS_Elem_ft.json``, ``MEAS_Bus_i_PMU.json`` and ``MEAS_Elem_ft_PMU.json`` files. The ``.json`` measurement files without data are generated with the ``empty_MEAS_files()`` function and the parameters from table 3 must be entered.\n\n**Table 3.** Parameters and description of ``empty_file_MEAS()`` function\n|    **Parameter**   |                           **Description**                         |**Default value** |\n|:------------------:|-------------------------------------------------------------------|:----------------:|\n| ``DSS_path``       | A path of the ``.DSS`` files of the circuit modeled in OpenDSS    | ``None ``        |\n| ``MEAS_path_save`` | Path where the measurement ``.json`` files will be saved          | ``None ``        |\n\nThe description of the identifiers that can be modified is detailed in tables 4, 5, 6, and 7. The other identifiers in the ``.json`` files, are node characteristics or elements extracted from the circuit modeled in OpenDSS, these data should not be modified since they would affect the result of the state estimation algorithm.\n\n**Table 4.** Description of identifiers of the ``MEAS_Bus_i.json`` file.\n\n| **Identifier**     |                                       **Description**                         |\n|:---------------------:|-------------------------------------------------------------------------------|\n| ``STS_Vm``            | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_Vm``            | Variance of voltage magnitude measurement error.                              |\n| ``Vρm(pu)``           | Measurement of voltage magnitude voltage in phase 𝜌.                          |\n| ``STS_PQd(SM)``       | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_SM``            | Measurement error variance of injection power or consumption of a smart meter.|\n| ``STS_PQd(0)``        | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_0``             | Zero or passive injection power measurement error variance.                   |\n| ``STS_PQd(Psd)``      | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_Psd``           | Measurement error variance of pseudo power injection measurement              |\n| ``Pρmd(pu)``          | Measurement of active power injection in phase 𝜌.                             |\n| ``Qρmd(pu)``          | Measurement of reactive power injection in phase 𝜌.                           |\n\n**Table 5.** Description of identifiers of the ``MEAS_Elem_ft.json`` file.\n\n| **Identifier**        | **Description**                                    |\n|:---------------------:|----------------------------------------------------|\n| ``STS_PQft``          | Status (1: Enabled, 0: Disabled)                   |\n| ``Rii_PQft``          | Branch power flow measurement error variance.      |\n| ``Pρmft(pu)``         | Measurement of branch active power in phase 𝜌.     |\n| ``Qρmft(pu)``         | Measurement of branch reactive power in phase 𝜌.   |\n| ``STS_Ift``           | Status (1: Enabled, 0: Disabled)                   |\n| ``Rii_Ift``           | Branch current magnitude error variance.           |\n| ``Iρmft(pu)``         | Measurement of branch current magnitude in phase 𝜌.|\n\n**Table 6.** Description of identifiers of the ``MEAS_Elem_ft_PMU.json`` file.\n| **Identifier**     |                   **Description**           |\n|:---------------------:|---------------------------------------------|\n| ``STS_Vm``            | Status (1: Enabled, 0: Disabled)            |\n| ``Rii_Vm``            | Variance of voltage phasor measurement error|\n| ``Vρm(pu)``           | Measurement of voltage magnitude in phase 𝜌 |\n| ``Angρm(deg)``        | Measurement of volage angle in phase 𝜌      |\n\n**Table 7.** Description of identifiers of the ``MEAS_Elem_ft_PMU.json`` file.\n| **Identifier**    |                 **Description**             |\n|:-----------------:|---------------------------------------------|\n| ``STS_Ift``       | Status (1: Enabled, 0: Disabled)            |\n| ``Rii_Ift``       | Variance of current phasor measurement error|\n| ``Iρmft(pu)``     | Measurement of current magnitude in phase 𝜌 |\n| ``Angρm(deg)``    | Measurement of current angle in phase 𝜌     |\n\n<div id=\'id5\' />\n\n#### Generate metrics from OpenDSS results\n\n##### Initial measurements with uncertainty of measurement error\n\nThe ``empty_init_files_MEAS_Unc()`` function generates ``.json`` files where all the nodes and elements that can participate as measurement in the state estimation algorithm are placed. For this purpose, the parameters of table 8 must be specified.\n\n**Table 8.** Parameters and description of ``empty_file_MEAS()`` function\n|    **Parameters**   |                           **Description**                     | **Default value** |\n|:------------------:|----------------------------------------------------------------|:-----------------:|\n| ``DSS_path``       | A path of the ``.DSS`` files of the circuit modeled in OpenDSS | ``None``          |\n| ``MEAS_path_save`` | Path where the measurement ``.json`` files will be saved       | ``None``          |\n\nIn the ``MEAS_path_save`` path, it generates the files ``Init_Bus_i.json``, ``Init_Elem_ft.json``, ``Init_Bus_i_PMU.json`` and ``Init_Elem_ft_PMU.json``. Depending on the case study, the ``STS`` meter status (1: Enabled, 0: Disabled) and the measurement error rate in ``Unc(%)`` can be modified.\n\n##### Adding random errors and generating measurement files\n\nWith the ``.json`` files generated by the ``empty_file_MEAS()`` function and the changes indicated by the user, with the ``add_error_file_MEAS()`` function and the Parameters described in Table 9.\n\n**Table 9.** Description and attributes of function ``add_error_files_MEAS()``\n| **Parameters** |                        **Description**                        | **Default value**|\n|:--------------:|---------------------------------------------------------------|:----------------:|\n| ``DSS_path``   | A path of the ``.DSS`` files of the circuit modeled in OpenDSS| ``None``         |\n| ``MEAS_path``  | Path of initial ``.json`` files                               | ``None``         |\n| ``seed_DS``    | Random error generation seed                                  | ``1``            |\n\nAdds random errors from a normal distribution to the OpenDSS power flow results, for use as a measurement. The result of generating random errors is contained in the files ``MEAS_Bus_i.json``, ``MEAS_Elem_ft.json``, ``MEAS_Bus_i_PMU.json`` and ``MEAS_Elem_ft_PMU.json``, stored in ``MEAS_path``.\n\n<div id=\'id6\' />\n\n### Run the state estimation algorithm\n\nTo run the state estimation algorithm, function ``estimate()`` is called, it is necessary to enter or change parameters detailed in table 10. \n\n**Table 10.** Parameters and description of ``estimate()`` function\n\n|   **Parameters** |                                   **Description**                                  | **Default value** |\n|:----------------:|------------------------------------------------------------------------------------|:---------------------:|\n| ``DSS_path``     | A path of the ``.DSS`` files of the circuit modeled in OpenDSS.                    | ``None``              |\n| ``MEAS_path``    | Path where measurement files are located.                                          | ``None``              |\n| ``path_save``    | Path where the results will be saved                                               | ``None``              |\n| ``Typ_cir``      | Circuit type, can be ``1ph`` or ``Pos``.                                           | ``None``              |\n| ``ALG``          | Type of algorithm state variables. At the moment ``NV``                            | ``NV``                |\n| ``coord``        | Type of coordinates to solve. For the moment ``polar``.                            | ``Polar``             |\n| ``method``       | Solution method, can be ``nonlinear``, ``linear_PMU`` and ``nonlinear_PMU``.| ``nonlinear_PMU``|\n| ``name_project`` | Project name                                                                       | ``Default``           |\n| ``View_res``     | Displays the result of the selected algorithm by console                           | ``False``             |\n| ``DSS_coll``     | Displays next to the estimated status, the actual status according to OpenDSS      | ``False``             |\n| ``summary``      | Displays a summary of the simulation by console                                    | ``False``             |\n| ``MEAS_Pos``     | ``True`` if it is a ``Pos`` circuit, take the ``.json`` files in positive sequence.| ``False``             |\n\n<div id=\'id7\' />\n\n## Sample tests\n\nIn the path ``:{Python_library_path}/openpy_dsse/examples``, the ``.DSS`` and ``.json`` files of single-phase (``1ph``) and positive sequence equivalent (``Pos``) circuit measurements detailed in Table 11 are located.\n\n**Table 11.** Sample tests\n| **Circuit** | **Tpy_circ** | **Case** |\n|:------------:|:------------:|:--------:|\n|     4Node    |      1ph     |     1    |\n|  [15NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/15NodeIEEE/15NodeIEEE.ipynb)  |      1ph     |     2    |\n|  [13NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/13NodeIEEE/13NodeIEEE.ipynb)  |      Pos     |     1    |\n|  [37NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/37NodeIEEE/37NodeIEEE.ipynb)  |      Pos     |     2    |\n\nThe function ``test_circuit(Typ_cir, case)``, returns a dictionary with the keys ``\'DSS_file\'``, ``\'MEAS_path\'``, ``\'save_path\'``, ``\'name_project\'`` and ``\'Typ_cir\'`` which correspond to the ``.DSS`` file path, measurement file path, path where results will be saved and circuit type respectively.\n```Python\nimport openpy_dsse\n\ndsse = openpy_dsse.init_DSSE() #Start the class.\n\nif __name__ == \'__main__\':\n    net = dsse.test_circuit(Typ_cir=\'1ph\', case=1)\n    \n    #dsse.empty_init_files_MEAS_Unc(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n    #dsse.add_error_files_MEAS(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n    #dsse.empty_MEAS_files(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n\n    #execute the state estimation algorithm\n    Results = dsse.estimate(\n        DSS_path=net[\'DSS_file\'],\n        MEAS_path=net[\'MEAS_path\'],\n        path_save=net[\'save_path\'],\n        Typ_cir=net[\'Typ_cir\'],\n        name_project=net[\'name_project\'],\n        View_res=True,\n        summary=True,\n        DSS_coll=True,\n        #MEAS_Pos=True,\n        #method=\'nonlinear\'\n        #method=\'linear_PMU\',\n    )\n```\n\n<div id=\'id8\' />\n\n### License\n\nLicense: CC BY-NC-SA 4.0\n\n<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />\n\nThis work has a license <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.\n',
     'author': 'Jorge Lara',
     'author_email': 'jlara@iee.unsj.edu.ar',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `openpy_dsse-0.1.3/PKG-INFO` & `openpy_dsse-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpy-dsse
-Version: 0.1.3
+Version: 0.1.4
 Summary: Open source library for state estimation of a distribution network modeled in OpenDSS
 License: LICENSE
 Keywords: OpenDSS,DSSE,state estimation,smart grid,OpenPy-DSSE,OpenPy_DSSE
 Author: Jorge Lara
 Author-email: jlara@iee.unsj.edu.ar
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

