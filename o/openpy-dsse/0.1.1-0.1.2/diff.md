# Comparing `tmp/openpy_dsse-0.1.1.tar.gz` & `tmp/openpy_dsse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpy_dsse-0.1.1.tar", max compression
+gzip compressed data, was "openpy_dsse-0.1.2.tar", max compression
```

## Comparing `openpy_dsse-0.1.1.tar` & `openpy_dsse-0.1.2.tar`

### file list

```diff
@@ -1,136 +1,151 @@
--rw-r--r--   0        0        0     3255 2022-11-28 15:56:42.954000 openpy_dsse-0.1.1/LICENSE.md
--rw-r--r--   0        0        0       68 2022-10-25 18:54:21.476000 openpy_dsse-0.1.1/openpy_dsse/__init__.py
--rw-r--r--   0        0        0    12600 2022-12-12 21:16:09.931000 openpy_dsse-0.1.1/openpy_dsse/Algorithm_classification.py
--rw-r--r--   0        0        0     3911 2022-10-25 16:17:19.258000 openpy_dsse-0.1.1/openpy_dsse/base_DSSE.py
--rw-r--r--   0        0        0       58 2022-10-11 19:54:20.428000 openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/__init__.py
--rw-r--r--   0        0        0       60 2022-10-11 19:55:20.245000 openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/Symb_Eqn/__init__.py
--rw-r--r--   0        0        0    18842 2022-08-18 21:16:16.722000 openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py
--rw-r--r--   0        0        0    19333 2022-09-19 23:51:10.547000 openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py
--rw-r--r--   0        0        0    41879 2022-10-23 21:33:52.493000 openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py
--rw-r--r--   0        0        0    35828 2022-12-16 18:46:00.112000 openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py
--rw-r--r--   0        0        0     2698 2022-10-19 14:31:08.646000 openpy_dsse-0.1.1/openpy_dsse/Elec_param_calc_DSS_EST.py
--rw-r--r--   0        0        0     6373 2022-12-16 18:46:00.169000 openpy_dsse-0.1.1/openpy_dsse/error_handling_logging.py
--rw-r--r--   0        0        0    38797 2022-12-14 03:12:46.465000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/13 Node IEEE.png
--rw-r--r--   0        0        0     2638 2022-10-25 16:23:23.002000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0     1605 2022-10-25 15:43:42.867000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0     3421 2022-10-25 16:09:48.529000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0     2977 2022-10-25 15:43:42.868000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0     5580 2022-12-17 23:33:08.430000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0     2905 2022-12-17 23:33:08.476000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     4660 2022-12-17 23:33:08.450000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0     3341 2022-12-17 23:33:08.493000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     3163 2022-10-25 16:31:50.272000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
--rw-r--r--   0        0        0     1280 2022-10-25 16:31:50.273000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     2570 2022-10-25 16:31:50.272000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
--rw-r--r--   0        0        0     1805 2022-10-25 16:31:50.273000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0      137 2022-09-18 23:25:43.017000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Capacitors.DSS
--rw-r--r--   0        0        0       13 2022-12-14 02:33:00.612000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
--rw-r--r--   0        0        0      243 2021-02-04 02:25:46.000000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Node_BusXY.csv
--rw-r--r--   0        0        0     1856 2022-12-14 02:31:34.295000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl
--rw-r--r--   0        0        0     1850 2022-12-14 02:31:34.295000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV
--rw-r--r--   0        0        0    11851 2021-02-04 02:25:46.000000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS
--rw-r--r--   0        0        0     2127 2022-09-18 23:29:29.878000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss
--rw-r--r--   0        0        0     1133 2022-09-19 00:03:40.591000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS
--rw-r--r--   0        0        0     1582 2022-09-19 01:59:14.562000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS
--rw-r--r--   0        0        0      519 2022-12-14 02:31:25.848000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss
--rw-r--r--   0        0        0      187 2022-12-17 23:33:08.911000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
--rw-r--r--   0        0        0       51 2022-12-17 23:33:08.895000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
--rw-r--r--   0        0        0      124 2022-10-24 15:17:02.027000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Capacitor.DSS
--rw-r--r--   0        0        0       13 2022-10-24 15:19:09.160000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/DSSViewIntercom.Txt
--rw-r--r--   0        0        0      143 2022-12-17 23:33:08.924000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
--rw-r--r--   0        0        0       71 2022-12-17 23:33:08.792000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
--rw-r--r--   0        0        0      768 2022-10-24 15:19:05.446000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl
--rw-r--r--   0        0        0     1739 2022-10-24 15:19:05.446000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV
--rw-r--r--   0        0        0     1840 2022-12-17 23:33:08.862000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
--rw-r--r--   0        0        0    10823 2022-12-17 23:33:08.757000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
--rw-r--r--   0        0        0     1472 2022-12-17 23:33:08.881000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
--rw-r--r--   0        0        0      197 2022-12-17 23:33:08.773000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
--rw-r--r--   0        0        0      355 2022-12-17 23:33:08.941000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
--rw-r--r--   0        0        0     1008 2022-12-17 23:33:08.841000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
--rw-r--r--   0        0        0     1180 2022-12-17 23:33:08.818000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
--rw-r--r--   0        0        0      128 2022-12-17 23:33:08.675000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
--rw-r--r--   0        0        0      541 2022-09-18 23:20:45.219000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS
--rw-r--r--   0        0        0      134 2022-09-18 23:27:42.311000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Switchs.DSS
--rw-r--r--   0        0        0      219 2022-09-18 23:22:54.457000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Transformers.DSS
--rw-r--r--   0        0        0      724 2022-09-18 23:21:47.993000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS
--rw-r--r--   0        0        0     2155 2022-12-17 23:33:11.840000 openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json
--rw-r--r--   0        0        0    47954 2022-12-14 02:11:49.565000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/15NodeIEEE.jpg
--rw-r--r--   0        0        0     3084 2022-10-24 17:48:11.843000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0     1889 2022-10-24 18:19:41.758000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0     4133 2022-10-24 17:57:11.996000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0     3615 2022-10-24 17:54:49.897000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0     6505 2022-10-24 17:58:40.985000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0     3717 2022-10-24 17:58:40.987000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     5544 2022-10-24 17:58:40.986000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0     4361 2022-10-24 17:58:40.988000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     1304 2022-08-20 19:35:36.127000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss
--rw-r--r--   0        0        0      993 2022-08-20 19:35:59.738000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss
--rw-r--r--   0        0        0      155 2022-10-12 15:04:24.931000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Master_15node.dss
--rw-r--r--   0        0        0       37 2022-08-19 21:16:18.326000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Voltagebases_15node.dss
--rw-r--r--   0        0        0       71 2022-08-20 19:34:33.391000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Vsource_15node.dss
--rw-r--r--   0        0        0     2516 2022-10-25 15:20:37.158000 openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json
--rw-r--r--   0        0        0    74051 2022-12-14 03:48:49.427000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/37 Node IEEE.png
--rw-r--r--   0        0        0     7337 2022-10-24 16:14:11.101000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0     4457 2022-10-24 17:34:20.149000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0     9994 2022-10-24 16:20:09.853000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0     8699 2022-10-24 15:46:49.590000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0    15074 2022-10-25 15:23:18.255000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0     8673 2022-10-25 15:23:18.256000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0    13356 2022-10-25 15:23:18.256000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0     9644 2022-10-25 15:23:18.257000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     8654 2022-10-25 15:22:33.314000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
--rw-r--r--   0        0        0     3827 2022-10-25 15:22:33.315000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     7342 2022-10-25 15:22:33.315000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
--rw-r--r--   0        0        0     5164 2022-10-25 15:22:33.316000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0     1745 2022-09-20 18:34:51.235000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS
--rw-r--r--   0        0        0       10 2022-12-14 03:15:52.032000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
--rw-r--r--   0        0        0      755 2021-02-04 01:25:46.000000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv
--rw-r--r--   0        0        0     1759 2022-09-20 18:37:06.672000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt
--rw-r--r--   0        0        0     6720 2022-12-14 03:15:50.718000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl
--rw-r--r--   0        0        0     4951 2022-12-14 03:15:50.718000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV
--rw-r--r--   0        0        0    11851 2021-02-04 01:25:46.000000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS
--rw-r--r--   0        0        0     2936 2022-09-20 18:39:03.897000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS
--rw-r--r--   0        0        0     3645 2022-09-20 18:33:23.217000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS
--rw-r--r--   0        0        0      415 2022-12-14 03:15:46.530000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Master_ieee37.DSS
--rw-r--r--   0        0        0      640 2022-10-25 15:23:18.269000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
--rw-r--r--   0        0        0       50 2022-10-25 15:23:18.268000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
--rw-r--r--   0        0        0      396 2022-10-25 15:23:18.269000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
--rw-r--r--   0        0        0       71 2022-10-25 15:23:18.266000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
--rw-r--r--   0        0        0     5335 2022-10-25 15:23:18.267000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
--rw-r--r--   0        0        0     9171 2022-10-25 15:23:18.265000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
--rw-r--r--   0        0        0     3186 2022-10-25 15:23:18.268000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
--rw-r--r--   0        0        0      197 2022-10-25 15:23:18.265000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
--rw-r--r--   0        0        0      348 2022-10-25 15:23:18.269000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
--rw-r--r--   0        0        0     1008 2022-10-25 15:23:18.266000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
--rw-r--r--   0        0        0     1180 2022-10-25 15:23:18.266000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
--rw-r--r--   0        0        0      126 2022-10-25 15:23:18.264000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
--rw-r--r--   0        0        0      535 2022-09-20 16:18:55.459000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS
--rw-r--r--   0        0        0      195 2022-09-20 15:49:32.549000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Substation.DSS
--rw-r--r--   0        0        0      198 2022-09-20 15:49:47.451000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Transformers.DSS
--rw-r--r--   0        0        0     6008 2022-10-25 15:23:21.253000 openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json
--rw-r--r--   0        0        0      806 2022-10-24 12:50:30.976000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json
--rw-r--r--   0        0        0      479 2022-10-24 12:49:41.570000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i_PMU.json
--rw-r--r--   0        0        0      808 2022-10-24 12:49:40.215000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json
--rw-r--r--   0        0        0      693 2022-10-24 12:49:39.143000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json
--rw-r--r--   0        0        0     1696 2022-10-24 17:58:10.585000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json
--rw-r--r--   0        0        0      887 2022-10-24 17:58:10.586000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json
--rw-r--r--   0        0        0     1176 2022-10-24 17:58:10.585000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json
--rw-r--r--   0        0        0      840 2022-10-24 17:58:10.586000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json
--rw-r--r--   0        0        0      242 2022-10-09 12:19:31.150000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/OpenDSS files/Line_4node.dss
--rw-r--r--   0        0        0      234 2022-10-09 12:20:00.111000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/OpenDSS files/Load_4node.dss
--rw-r--r--   0        0        0      154 2022-10-09 12:20:12.673000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/OpenDSS files/Master_4node.dss
--rw-r--r--   0        0        0       34 2022-08-18 13:32:43.243000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/OpenDSS files/Voltagebases_4node.dss
--rw-r--r--   0        0        0       64 2022-08-18 13:36:08.540000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/OpenDSS files/Vsource_4node.dss
--rw-r--r--   0        0        0      653 2022-10-25 15:20:17.411000 openpy_dsse-0.1.1/openpy_dsse/examples/4Node/Results/Results_DSSE_4Node.json
--rw-r--r--   0        0        0     3255 2022-10-25 18:55:11.503000 openpy_dsse-0.1.1/openpy_dsse/LICENSE.md
--rw-r--r--   0        0        0    98902 2022-12-16 18:06:54.863000 openpy_dsse-0.1.1/openpy_dsse/MEAS_from_OpenDSS.py
--rw-r--r--   0        0        0   177831 2022-10-19 15:38:49.924000 openpy_dsse-0.1.1/openpy_dsse/OpenDSS_data_extraction.py
--rw-r--r--   0        0        0    11480 2022-10-19 15:15:50.227000 openpy_dsse-0.1.1/openpy_dsse/Plot_results_DSS_EST.py
--rw-r--r--   0        0        0    14816 2022-12-16 18:46:00.245000 openpy_dsse-0.1.1/openpy_dsse/Readme.md
--rw-r--r--   0        0        0     2771 2022-12-13 21:37:20.521000 openpy_dsse-0.1.1/openpy_dsse/Sample_test_systems_DSS.py
--rw-r--r--   0        0        0     9068 2022-12-12 20:50:34.608000 openpy_dsse-0.1.1/openpy_dsse/state_estimation.py
--rw-r--r--   0        0        0     8194 2022-10-16 15:14:24.719000 openpy_dsse-0.1.1/openpy_dsse/YBus_Matrix_Pos_Seq.py
--rw-r--r--   0        0        0      999 2022-12-17 23:32:38.832000 openpy_dsse-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14823 2022-12-17 23:35:54.405000 openpy_dsse-0.1.1/README.md
--rw-r--r--   0        0        0    41910 1970-01-01 00:00:00.000000 openpy_dsse-0.1.1/setup.py
--rw-r--r--   0        0        0    15971 1970-01-01 00:00:00.000000 openpy_dsse-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3255 2022-11-28 15:56:42.954000 openpy_dsse-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0       68 2022-10-25 18:54:21.476000 openpy_dsse-0.1.2/openpy_dsse/__init__.py
+-rw-r--r--   0        0        0    12460 2022-12-30 19:55:22.918000 openpy_dsse-0.1.2/openpy_dsse/Algorithm_classification.py
+-rw-r--r--   0        0        0     3916 2023-01-24 14:02:27.992000 openpy_dsse-0.1.2/openpy_dsse/base_DSSE.py
+-rw-r--r--   0        0        0      254 2023-04-22 14:51:12.130000 openpy_dsse-0.1.2/openpy_dsse/COM_interface.py
+-rw-r--r--   0        0        0       58 2022-10-11 19:54:20.428000 openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/__init__.py
+-rw-r--r--   0        0        0       60 2022-10-11 19:55:20.245000 openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/Symb_Eqn/__init__.py
+-rw-r--r--   0        0        0    18842 2022-08-18 21:16:16.722000 openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py
+-rw-r--r--   0        0        0    19333 2022-09-19 23:51:10.547000 openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py
+-rw-r--r--   0        0        0    41959 2022-12-29 18:05:55.584000 openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py
+-rw-r--r--   0        0        0    35828 2022-12-16 18:46:00.112000 openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py
+-rw-r--r--   0        0        0     4499 2022-12-31 17:30:43.970000 openpy_dsse-0.1.2/openpy_dsse/Elec_param_calc_DSS_EST.py
+-rw-r--r--   0        0        0     6686 2022-12-30 20:48:27.487000 openpy_dsse-0.1.2/openpy_dsse/error_handling_logging.py
+-rw-r--r--   0        0        0     2638 2022-10-25 16:23:23.002000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0     1605 2022-10-25 15:43:42.867000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0     3421 2022-10-25 16:09:48.529000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0     2977 2022-10-25 15:43:42.868000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     5580 2023-03-08 19:04:07.333000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0     2905 2023-03-08 19:04:07.367000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     4660 2023-03-08 19:04:07.351000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     3341 2023-03-08 19:04:07.389000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     3163 2022-10-25 16:31:50.272000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
+-rw-r--r--   0        0        0     1280 2022-10-25 16:31:50.273000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     2570 2022-10-25 16:31:50.272000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     1805 2022-10-25 16:31:50.273000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0      137 2022-09-18 23:25:43.017000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Capacitors.DSS
+-rw-r--r--   0        0        0       13 2023-01-02 13:26:33.881000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
+-rw-r--r--   0        0        0      243 2021-02-04 02:25:46.000000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Node_BusXY.csv
+-rw-r--r--   0        0        0     1856 2023-01-02 13:26:23.711000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl
+-rw-r--r--   0        0        0     1850 2023-01-02 13:26:23.711000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV
+-rw-r--r--   0        0        0    11851 2021-02-04 02:25:46.000000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS
+-rw-r--r--   0        0        0     2127 2022-09-18 23:29:29.878000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss
+-rw-r--r--   0        0        0     1133 2022-09-19 00:03:40.591000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS
+-rw-r--r--   0        0        0     1582 2022-09-19 01:59:14.562000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS
+-rw-r--r--   0        0        0      519 2023-01-02 13:26:18.681000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss
+-rw-r--r--   0        0        0      187 2023-03-08 19:04:07.640000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
+-rw-r--r--   0        0        0       51 2023-03-08 19:04:07.629000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
+-rw-r--r--   0        0        0      124 2022-10-24 15:17:02.027000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Capacitor.DSS
+-rw-r--r--   0        0        0       13 2022-10-24 15:19:09.160000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/DSSViewIntercom.Txt
+-rw-r--r--   0        0        0      143 2023-03-08 19:04:07.655000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
+-rw-r--r--   0        0        0       71 2023-03-08 19:04:07.547000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
+-rw-r--r--   0        0        0      768 2022-10-24 15:19:05.446000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl
+-rw-r--r--   0        0        0     1739 2022-10-24 15:19:05.446000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV
+-rw-r--r--   0        0        0     1840 2023-03-08 19:04:07.607000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
+-rw-r--r--   0        0        0    10823 2023-03-08 19:04:07.525000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
+-rw-r--r--   0        0        0     1472 2023-03-08 19:04:07.620000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
+-rw-r--r--   0        0        0      197 2023-03-08 19:04:07.537000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
+-rw-r--r--   0        0        0      355 2023-03-08 19:04:07.667000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
+-rw-r--r--   0        0        0     1008 2023-03-08 19:04:07.592000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
+-rw-r--r--   0        0        0     1180 2023-03-08 19:04:07.582000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
+-rw-r--r--   0        0        0      128 2023-03-08 19:04:07.498000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
+-rw-r--r--   0        0        0      541 2022-09-18 23:20:45.219000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS
+-rw-r--r--   0        0        0      134 2022-09-18 23:27:42.311000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Switchs.DSS
+-rw-r--r--   0        0        0      219 2022-09-18 23:22:54.457000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Transformers.DSS
+-rw-r--r--   0        0        0      724 2022-09-18 23:21:47.993000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS
+-rw-r--r--   0        0        0    78005 2023-03-08 19:04:14.530000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png
+-rw-r--r--   0        0        0      416 2023-03-08 19:04:11.395000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json
+-rw-r--r--   0        0        0     2155 2023-03-08 19:04:10.919000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json
+-rw-r--r--   0        0        0     2568 2023-03-08 19:04:11.281000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json
+-rw-r--r--   0        0        0    73688 2023-03-08 19:04:13.212000 openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png
+-rw-r--r--   0        0        0     3084 2022-10-24 17:48:11.843000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0     1889 2022-10-24 18:19:41.758000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0     4133 2022-10-24 17:57:11.996000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0     3615 2022-10-24 17:54:49.897000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     6505 2023-03-08 19:07:23.246000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0     3679 2023-03-08 19:07:23.280000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     5544 2023-03-08 19:07:23.262000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     4367 2023-03-08 19:07:23.297000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     1304 2022-08-20 19:35:36.127000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss
+-rw-r--r--   0        0        0      993 2022-08-20 19:35:59.738000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss
+-rw-r--r--   0        0        0      155 2022-10-12 15:04:24.931000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Master_15node.dss
+-rw-r--r--   0        0        0       37 2022-08-19 21:16:18.326000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Voltagebases_15node.dss
+-rw-r--r--   0        0        0       71 2022-08-20 19:34:33.391000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Vsource_15node.dss
+-rw-r--r--   0        0        0    84900 2023-03-08 19:07:30.754000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png
+-rw-r--r--   0        0        0      417 2023-03-08 19:07:28.003000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json
+-rw-r--r--   0        0        0     2512 2023-03-08 19:07:27.801000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json
+-rw-r--r--   0        0        0     3149 2023-03-08 19:07:27.922000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json
+-rw-r--r--   0        0        0    71312 2023-03-08 19:07:29.069000 openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png
+-rw-r--r--   0        0        0     7337 2022-10-24 16:14:11.101000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0     4457 2022-10-24 17:34:20.149000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0     9994 2022-10-24 16:20:09.853000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0     8699 2022-10-24 15:46:49.590000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0    15079 2023-03-08 19:05:36.302000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0     8672 2023-03-08 19:05:36.328000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0    13354 2023-03-08 19:05:36.318000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     9644 2023-03-08 19:05:36.336000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     8654 2022-10-25 15:22:33.314000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json
+-rw-r--r--   0        0        0     3827 2022-10-25 15:22:33.315000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     7342 2022-10-25 15:22:33.315000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json
+-rw-r--r--   0        0        0     5164 2022-10-25 15:22:33.316000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     1745 2022-09-20 18:34:51.235000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS
+-rw-r--r--   0        0        0       10 2022-12-14 03:15:52.032000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/DSSViewIntercom.Txt
+-rw-r--r--   0        0        0      755 2021-02-04 01:25:46.000000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv
+-rw-r--r--   0        0        0     1759 2022-09-20 18:37:06.672000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt
+-rw-r--r--   0        0        0     6720 2022-12-14 03:15:50.718000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl
+-rw-r--r--   0        0        0     4951 2022-12-14 03:15:50.718000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV
+-rw-r--r--   0        0        0    11851 2021-02-04 01:25:46.000000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS
+-rw-r--r--   0        0        0     2936 2022-09-20 18:39:03.897000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS
+-rw-r--r--   0        0        0     3645 2022-09-20 18:33:23.217000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS
+-rw-r--r--   0        0        0      415 2022-12-14 03:15:46.530000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Master_ieee37.DSS
+-rw-r--r--   0        0        0      640 2023-03-08 19:05:36.581000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss
+-rw-r--r--   0        0        0       50 2023-03-08 19:05:36.568000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusVoltageBases.DSS
+-rw-r--r--   0        0        0      396 2023-03-08 19:05:36.596000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GISCoords.dss
+-rw-r--r--   0        0        0       71 2023-03-08 19:05:36.497000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/GrowthShape.DSS
+-rw-r--r--   0        0        0     5335 2023-03-08 19:05:36.548000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS
+-rw-r--r--   0        0        0     9171 2023-03-08 19:05:36.451000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS
+-rw-r--r--   0        0        0     3186 2023-03-08 19:05:36.560000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS
+-rw-r--r--   0        0        0      197 2023-03-08 19:05:36.464000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LoadShape.DSS
+-rw-r--r--   0        0        0      348 2023-03-08 19:05:36.607000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Master.DSS
+-rw-r--r--   0        0        0     1008 2023-03-08 19:05:36.521000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS
+-rw-r--r--   0        0        0     1180 2023-03-08 19:05:36.511000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS
+-rw-r--r--   0        0        0      126 2023-03-08 19:05:36.423000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Vsource.dss
+-rw-r--r--   0        0        0      535 2022-09-20 16:18:55.459000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS
+-rw-r--r--   0        0        0      195 2022-09-20 15:49:32.549000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Substation.DSS
+-rw-r--r--   0        0        0      198 2022-09-20 15:49:47.451000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Transformers.DSS
+-rw-r--r--   0        0        0   111900 2023-03-08 19:05:44.755000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png
+-rw-r--r--   0        0        0      415 2023-03-08 19:05:41.528000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json
+-rw-r--r--   0        0        0     6014 2023-03-08 19:05:41.138000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json
+-rw-r--r--   0        0        0     7374 2023-03-08 19:05:41.462000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json
+-rw-r--r--   0        0        0    89028 2023-03-08 19:05:43.312000 openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png
+-rw-r--r--   0        0        0      806 2022-10-24 12:50:30.976000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json
+-rw-r--r--   0        0        0      479 2022-10-24 12:49:41.570000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i_PMU.json
+-rw-r--r--   0        0        0      808 2022-10-24 12:49:40.215000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json
+-rw-r--r--   0        0        0      693 2022-10-24 12:49:39.143000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json
+-rw-r--r--   0        0        0     1696 2023-03-03 16:29:22.817000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json
+-rw-r--r--   0        0        0      887 2023-03-03 16:29:22.869000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json
+-rw-r--r--   0        0        0     1176 2023-03-03 16:29:22.831000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json
+-rw-r--r--   0        0        0      840 2023-03-03 16:29:22.884000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json
+-rw-r--r--   0        0        0      242 2022-10-09 12:19:31.150000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/OpenDSS files/Line_4node.dss
+-rw-r--r--   0        0        0      234 2022-10-09 12:20:00.111000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/OpenDSS files/Load_4node.dss
+-rw-r--r--   0        0        0      154 2022-10-09 12:20:12.673000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/OpenDSS files/Master_4node.dss
+-rw-r--r--   0        0        0       34 2022-08-18 13:32:43.243000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/OpenDSS files/Voltagebases_4node.dss
+-rw-r--r--   0        0        0       64 2022-08-18 13:36:08.540000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/OpenDSS files/Vsource_4node.dss
+-rw-r--r--   0        0        0    67777 2023-03-03 16:29:29.956000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png
+-rw-r--r--   0        0        0      417 2023-03-03 16:29:27.537000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/Results/Metrics_4Node.json
+-rw-r--r--   0        0        0      650 2023-03-03 16:29:27.285000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/Results/Results_DSSE_4Node.json
+-rw-r--r--   0        0        0      651 2023-03-03 16:29:27.439000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json
+-rw-r--r--   0        0        0    70469 2023-03-03 16:29:28.854000 openpy_dsse-0.1.2/openpy_dsse/examples/4Node/Results/Vi_DSS_EST_PU_4Node.png
+-rw-r--r--   0        0        0     3255 2022-10-25 18:55:11.503000 openpy_dsse-0.1.2/openpy_dsse/LICENSE.md
+-rw-r--r--   0        0        0    98902 2022-12-16 18:06:54.863000 openpy_dsse-0.1.2/openpy_dsse/MEAS_from_OpenDSS.py
+-rw-r--r--   0        0        0   177867 2023-01-24 14:35:24.540000 openpy_dsse-0.1.2/openpy_dsse/OpenDSS_data_extraction.py
+-rw-r--r--   0        0        0     6324 2022-12-31 23:55:26.357000 openpy_dsse-0.1.2/openpy_dsse/perf_metrics_calc.py
+-rw-r--r--   0        0        0     8151 2022-12-31 23:21:02.670000 openpy_dsse-0.1.2/openpy_dsse/Plot_results_DSS_EST.py
+-rw-r--r--   0        0        0    14816 2022-12-16 18:46:00.245000 openpy_dsse-0.1.2/openpy_dsse/Readme.md
+-rw-r--r--   0        0        0     2771 2022-12-13 21:37:20.521000 openpy_dsse-0.1.2/openpy_dsse/Sample_test_systems_DSS.py
+-rw-r--r--   0        0        0    11515 2023-01-02 14:22:12.369000 openpy_dsse-0.1.2/openpy_dsse/state_estimation.py
+-rw-r--r--   0        0        0     8227 2022-12-29 23:05:58.121000 openpy_dsse-0.1.2/openpy_dsse/YBus_Matrix_Pos_Seq.py
+-rw-r--r--   0        0        0      999 2023-04-22 18:47:03.257000 openpy_dsse-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    15706 2023-04-22 15:09:09.407000 openpy_dsse-0.1.2/README.md
+-rw-r--r--   0        0        0    50021 1970-01-01 00:00:00.000000 openpy_dsse-0.1.2/setup.py
+-rw-r--r--   0        0        0    16846 1970-01-01 00:00:00.000000 openpy_dsse-0.1.2/PKG-INFO
```

### Comparing `openpy_dsse-0.1.1/LICENSE.md` & `openpy_dsse-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/Algorithm_classification.py` & `openpy_dsse-0.1.2/openpy_dsse/Algorithm_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,21 @@
 from functools import reduce
 
 from .base_DSSE import *
 from .MEAS_from_OpenDSS import Normalization_MEAS
 from .YBus_Matrix_Pos_Seq import *
 from .DSSE_algorithms.WLS_alg_1ph import WLS_1ph_state_estimator
 from .DSSE_algorithms.WLS_alg_Pos_Seq import WLS_Pos_state_estimator
-from .error_handling_logging import update_logg_file, to_Excel_MEAS
+from .error_handling_logging import update_logg_file, to_Excel_MEAS, elem_YBus, orient, indent
 
 pd.options.mode.chained_assignment = None
 
 #dss = py_dss_interface.DSSDLL()
 data_DSS = OpenDSS_data_collection()
 log_py = logging.getLogger(__name__)
-orient, indent = "index", 1
-
 
 def DSS_EST_save_view(
         results_DSSE: dict, MEAS_dict: dict(),
         path_save: str, name_project: str,
         DSS_coll: bool, View_res: bool, summary: bool):
 
     if View_res:
@@ -133,18 +131,16 @@
         else:
             update_logg_file('Select the configuration: Typ_circ, Alg, coord and method available. See documentation', 4, log_py)
             exit()
 
         DSS_EST_save_view(
             state_estimation, MEAS_study,
             self.path_save, self.name_project, self.DSS_coll, self.View_res, self.summary)
-
         return state_estimation
 
-
 class diff_algorithms(BaseAlgorithm, File_options):
 
     def __init__(
             self,
             Sbas3ph_MVA,
             tolerance,
             max_iter,
@@ -176,15 +172,14 @@
 
         'Obtain initial values of voltage and angle'
         df_Volt_Ang_init = data_DSS.initial_voltage_angle_option(option=self.init_values)
         df_Volt_Ang_init = df_Volt_Ang_init.drop(
             ['num_nodes', 'ph_2', 'ph_3', 'V2(pu)', 'V3(pu)', 'Ang2(rad)', 'Ang3(rad)'], axis=1)
 
         'Get circuit YBus from OpenDSS'
-        elem_YBus = ['vsources', 'lines', 'transformers']
         #initialize class
         YBus_1ph = YBus_Matrix_SeqPos_OpenDSS(data_DSS.allbusnames_aux())
         Ybus_PU = YBus_1ph.YBus_Matrix_pu(
             SbasMVA_3ph=self.Sbas3ph_MVA,
             YBus_Matrix=YBus_1ph.build_YBus_Matrix_Pos_Seq(
                 element=elem_YBus
             )
@@ -256,15 +251,14 @@
             update_logg_file('State estimation through the positive sequence equivalent circuit', 2, log_py)
 
         'Obtain initial values of voltage and angle'
         df_Volt_Ang_init = data_DSS.initial_voltage_angle_option(option=self.init_values)
         df_Volt_Ang_init = df_Volt_Ang_init.drop(
             ['num_nodes', 'ph_2', 'ph_3', 'V2(pu)', 'V3(pu)', 'Ang2(rad)', 'Ang3(rad)'], axis=1)
         'Get circuit YBus from OpenDSS'
-        elem_YBus = ['vsources', 'lines', 'transformers', 'capacitors']
         YBus_SeqPos = YBus_Matrix_SeqPos_OpenDSS(data_DSS.allbusnames_aux())  # start the class
         Ybus_PU = YBus_SeqPos.YBus_Matrix_pu(
             SbasMVA_3ph=self.Sbas3ph_MVA,
             YBus_Matrix=YBus_SeqPos.build_YBus_Matrix_Pos_Seq(element=elem_YBus))
 
         'Obtain measurements according to type and configuration as per study_case_DSSE.py'
         get_MEAS = Normalization_MEAS(
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/base_DSSE.py` & `openpy_dsse-0.1.2/openpy_dsse/base_DSSE.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,16 +48,17 @@
         self.init_values = init_values
         self.successful = False
 
 class functions_DSSE:
     def check_observability(self, num_state_var, num_measurements, log_py):
         if num_measurements < (2 * num_state_var) - 1:
             update_logg_file("System is not observable (cancelling)", 4, log_py)
-            update_logg_file(f'Measurements available: {num_measurements}. '
-                             f'Measurements required: {(2 * num_state_var) - 1}', 3, log_py)
+            update_logg_file(
+                f'Measurements available: {num_measurements}. '
+                f'Measurements required: {(2 * num_state_var) - 1}', 3, log_py)
             exit()
 
             raise UserWarning("Measurements available: %d. Measurements required: %d" %
                               (num_measurements, (2 * num_state_var) - 1))
 
             exit()
         else:
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py` & `openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_1ph.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py` & `openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/Symb_Eqn/sym_func_Pos_Seq.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py` & `openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/WLS_alg_1ph.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,16 +68,23 @@
         Rii_pmu[aux_Rii_pmu, 0] = Ri_ang_pmu[n + aux_pos]
         aux_Rii_pmu += 1
 
     return Rii_pmu
 
 class WLS_1ph_state_estimator:
 
-    def __init__(self, tolerance: int, num_iter_max: int, DF_MEAS_SCADA: pd.DataFrame, DF_MEAS_PMU: pd.DataFrame,
-                 DF_Volt_Ang_initial: pd.DataFrame, YBus_Matrix: np.array):
+    def __init__(
+            self,
+            tolerance: int,
+            num_iter_max: int,
+            DF_MEAS_SCADA: pd.DataFrame,
+            DF_MEAS_PMU: pd.DataFrame,
+            DF_Volt_Ang_initial: pd.DataFrame,
+            YBus_Matrix: np.array
+    ):
         '''
         :param tolerance:
         :param num_iter_max:
         :param DF_MEAS_SCADA:
         :param DF_Volt_Ang_initial: initial values of the state estimator
         :param YBus_Matrix: Corresponds to the Y_Bus Matrix of the system.
         '''
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py` & `openpy_dsse-0.1.2/openpy_dsse/DSSE_algorithms/WLS_alg_Pos_Seq.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/Elec_param_calc_DSS_EST.py` & `openpy_dsse-0.1.2/openpy_dsse/Elec_param_calc_DSS_EST.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,62 +6,97 @@
 # @Software: PyCharm
 
 import pandas as pd
 import numpy as np
 import math
 import cmath
 
-from .OpenDSS_data_extraction import OpenDSS_data_collection, dss
+from openpy_dsse import YBus_Matrix_Pos_Seq
+
+from .OpenDSS_data_extraction import OpenDSS_data_collection, Values_per_unit, dss
+from openpy_dsse.DSSE_algorithms.Symb_Eqn.sym_func_1ph import sym_func_Iij_rec
+from .YBus_Matrix_Pos_Seq import get_G_B_Pos_seq, YBus_Matrix_SeqPos_OpenDSS
+from .error_handling_logging import elem_YBus, orient, indent
 
 data_DSS = OpenDSS_data_collection()
 
 class estimated_electrical_variables:
-
     def __init__(self, I_Ang_EST: bool = False, PQi_EST: bool = False, PQf_EST: bool = False):
         self.I_Ang_EST = I_Ang_EST
         self.PQi_EST = PQi_EST
         self.PQf_EST = PQf_EST
-
-    def Imang_Angle_EST_1ph(self, I_elem_pu_DSS: pd.DataFrame, df_Results_DSSE: pd.DataFrame, YBusMatrix_PU: np.array):
-
+    def Imang_Angle_EST_1ph(
+            self,
+            df_Results_DSSE: pd.DataFrame,
+            SbasMVA_3ph: float,
+            path_save: str,
+            View_res: bool,
+            DSS_col: bool,
+            name_project: str
+    ):
+        I_Ang_EST_DSS = dict()
+        YBus_1ph = YBus_Matrix_SeqPos_OpenDSS(data_DSS.allbusnames_aux())
+        YBusMatrix_PU = YBus_1ph.YBus_Matrix_pu(
+            SbasMVA_3ph=SbasMVA_3ph,
+            YBus_Matrix=YBus_1ph.build_YBus_Matrix_Pos_Seq(
+                element=elem_YBus
+            )
+        )
+        Per_PU = Values_per_unit(SbasMVA_3ph=SbasMVA_3ph)
+        I_elem_pu_DSS = Per_PU.element_Iij_PU(
+            df_element_currents=data_DSS.element_currents_Iij_Ang(
+                element=['lines'])
+        )
         #Current
         I_elem_pu_DSS = I_elem_pu_DSS[['element_name', 'from_bus', 'to_bus', 'I1(pu)', 'ang1(deg)']]
-        DF_Iij_aux_DSS = pd.merge(I_elem_pu_DSS, data_DSS.allbusnames_aux(),
-                                  how='inner', left_on='from_bus', right_on='bus_name', suffixes=('_i', ''))
-
-        DF_Iij_aux_DSS = pd.merge(DF_Iij_aux_DSS, data_DSS.allbusnames_aux(), how='inner', left_on='to_bus',
-                                  right_on='bus_name',
-                                  suffixes=('_j', ''))
-
+        DF_Iij_aux_DSS = pd.merge(
+            I_elem_pu_DSS, data_DSS.allbusnames_aux(),
+            how='inner', left_on='from_bus', right_on='bus_name', suffixes=('_i', '')
+        )
+        DF_Iij_aux_DSS = pd.merge(
+            DF_Iij_aux_DSS, data_DSS.allbusnames_aux(),
+            how='inner', left_on='to_bus', right_on='bus_name', suffixes=('_j', '')
+        )
         DF_Iij_aux_DSS = DF_Iij_aux_DSS.rename(
-            columns={'bus_name_aux_j': 'from_bus_aux', 'bus_name_aux': 'to_bus_aux'})
-
+            columns={'bus_name_aux_j': 'from_bus_aux', 'bus_name_aux': 'to_bus_aux'}
+        )
         DF_I_Ang_estimate = pd.DataFrame(
             columns=['element_name', 'from_bus', 'to_bus', 'I1(pu)', 'ang1(deg)'])
-
         DF_results_WLS = df_Results_DSSE.copy()
         for k in range(len(DF_results_WLS)):
             'angle'
-            DF_results_WLS.at[k, 'Ang1(deg)'] = math.radians(DF_results_WLS.at[k, 'Ang1(deg)'])
-
+            DF_results_WLS.at[k, 'Ang1(deg)_EST'] = math.radians(DF_results_WLS.at[k, 'Ang1(deg)_EST'])
         Matrix_WLS_results = np.array(DF_results_WLS)
-        V_1 = np.array([Matrix_WLS_results[:, 1]]).T
-        Vang_1 = np.array([Matrix_WLS_results[:, 2]]).T
+        V_1 = np.array([Matrix_WLS_results[:, 2]]).T
+        Vang_1 = np.array([Matrix_WLS_results[:, 3]]).T
 
         f29 = sym_func_Iij_rec()
         for index, row in DF_Iij_aux_DSS.iterrows():
             id_name = DF_Iij_aux_DSS['element_name'][index]
             m = DF_Iij_aux_DSS['from_bus_aux'][index] - 1
             n = DF_Iij_aux_DSS['to_bus_aux'][index] - 1
 
             G1, B1 = get_G_B_Pos_seq(m, n, YBusMatrix_PU)
             I_ij = f29(G1, B1, V_1[m][0], Vang_1[m][0], V_1[n][0], Vang_1[n][0])
             I1, ang1 = cmath.polar(I_ij)
-
             DF_I_Ang_estimate = DF_I_Ang_estimate.append({
                 'element_name': id_name,
                 'from_bus': DF_Iij_aux_DSS['from_bus'][index],
                 'to_bus': DF_Iij_aux_DSS['to_bus'][index],
                 'I1(pu)': I1, 'ang1(deg)': math.degrees(ang1) - 180}, ignore_index=True)
 
-        return DF_I_Ang_estimate
+        I_Ang_EST_DSS['df_EST'] = DF_I_Ang_estimate.rename(columns={'I1(pu)': 'I1(pu)_EST', 'ang1(deg)': 'Ang1(deg)_EST'})
+        I_Ang_EST_DSS['df_DSS'] = I_elem_pu_DSS.rename(columns={'I1(pu)': 'I1(pu)_DSS', 'ang1(deg)': 'Ang1(deg)_DSS'})
+        if DSS_col:
+            df_DSS_EST = pd.merge(I_Ang_EST_DSS['df_DSS'], I_Ang_EST_DSS['df_EST'], on=('element_name', 'from_bus', 'to_bus'))
+        else:
+            df_DSS_EST = I_Ang_EST_DSS['df_EST']
+        if View_res:
+            print(df_DSS_EST)
+        if path_save is not None:
+            df_DSS_EST.to_excel(f'{path_save}\Results_I_Ang_from_DSSE_{name_project}.xlsx', index=False)
+
+            df_DSS_EST_json = df_DSS_EST.to_json(orient=orient, indent=indent)
+            with open(f"{path_save}\Results_I_Ang_from_DSSE_{name_project}.json", "w") as outfile:
+                outfile.write(df_DSS_EST_json)
+        return I_Ang_EST_DSS
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/error_handling_logging.py` & `openpy_dsse-0.1.2/openpy_dsse/error_handling_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 script_path = os.path.dirname(os.path.abspath(__file__))
 logger_aux = logging.getLogger(__name__)
 
 orient, indent = "index", 1
 to_Excel_MEAS = False
 Logg_option = False
-
+elem_YBus = ['lines', 'transformers', 'capacitors']
 
 def update_logg_file(msg: str, Typ: int = 0, logger=logger_aux, Logg: bool = Logg_option, Print: bool = True):
     """
     Creates or updates the log_py file. In addition, it prints the message formatted according to the type.
 
     :param msg: Message text to be displayed by console or saved in the log_py file
     :param logger: From function logging.getLogger(__name__)
@@ -117,15 +117,24 @@
     elif aux_path:
         update_logg_file('Error\nYou must indicate a path where the .json files will be saved.', 4, log_py)
         exit()
 
 def estimate_EH(DSS_path, MEAS_path, path_save, Typ_cir, MEAS_SeqPos_path, log_py):
     pass
 
-
+def calc_from_est_EH(
+        DSS_path: str = None,
+        EST_pd: pd.DataFrame = None,
+        EST_path: str = None,
+        I_Ang_EST: bool = False,
+        PQi_EST: bool = False,
+        PQf_EST: bool = False,
+        no_PU: bool = False
+):
+    pass
 def _excel_json(excel_name, save_path, option):
     df_Bus_i = pd.read_excel(f'{save_path}\{excel_name}.xlsx', sheet_name='Bus_i')
     df_Elem_ft = pd.read_excel(f'{save_path}\{excel_name}.xlsx', sheet_name='Elem_ft')
     df_Bus_i_PMU = pd.read_excel(f'{save_path}\{excel_name}.xlsx', sheet_name='Bus_i_PMU')
     df_Elem_ft_PMU = pd.read_excel(f'{save_path}\{excel_name}.xlsx', sheet_name='Elem_ft_PMU')
 
     if option == 'init':
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.dbl`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEE13Nodeckt_Power.DSV`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/IEEELineCodes.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/LineCodes.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Lines.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Loads.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Master13NodeIEEE.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.dbl`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/ieee13nodeckt_Power.DSV`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Sub_transformer.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/OpenDSS files/Voltage_regulators.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992424242424243%*

 * *Differences: {"'3'": "{'V1m(pu)': 0.95306}"}*

```diff
@@ -202,15 +202,15 @@
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
         "STS_Vm": 1,
-        "V1m(pu)": 0.95305,
+        "V1m(pu)": 0.95306,
         "V2m(pu)": -6e-05,
         "V3m(pu)": -6e-05,
         "bus_name": "bus_4",
         "num_nodes": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9820512820512821%*

 * *Differences: {"'3'": "{'STS_Vm': 0, 'Rii_Vm': 0.0, 'V1m(pu)': 0.0, 'V2m(pu)': 0.0, 'V3m(pu)': 0.0, "*

 * *        "'Ang1m(deg)': 0.0, 'Ang2m(deg)': 0.0, 'Ang3m(deg)': 0.0}",*

 * * "'5'": "{'V1m(pu)': 0.97253, 'V2m(pu)': 2e-05, 'V3m(pu)': 2e-05, 'Ang1m(deg)': -0.05835, "*

 * *        "'Ang2m(deg)': 2e-05, 'Ang3m(deg)': 2e-05}"}*

```diff
@@ -116,22 +116,22 @@
         "bus_name": "bus_3",
         "num_nodes": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0
     },
     "3": {
-        "Ang1m(deg)": -0.09151,
-        "Ang2m(deg)": 2e-05,
-        "Ang3m(deg)": 2e-05,
-        "Rii_Vm": 1.10889e-05,
-        "STS_Vm": 1,
-        "V1m(pu)": 0.95313,
-        "V2m(pu)": 2e-05,
-        "V3m(pu)": 2e-05,
+        "Ang1m(deg)": 0.0,
+        "Ang2m(deg)": 0.0,
+        "Ang3m(deg)": 0.0,
+        "Rii_Vm": 0.0,
+        "STS_Vm": 0,
+        "V1m(pu)": 0.0,
+        "V2m(pu)": 0.0,
+        "V3m(pu)": 0.0,
         "bus_name": "bus_4",
         "num_nodes": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0
     },
     "4": {
@@ -146,22 +146,22 @@
         "bus_name": "bus_5",
         "num_nodes": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0
     },
     "5": {
-        "Ang1m(deg)": -0.05815,
-        "Ang2m(deg)": -4e-05,
-        "Ang3m(deg)": -4e-05,
+        "Ang1m(deg)": -0.05835,
+        "Ang2m(deg)": 2e-05,
+        "Ang3m(deg)": 2e-05,
         "Rii_Vm": 1.10889e-05,
         "STS_Vm": 1,
-        "V1m(pu)": 0.97247,
-        "V2m(pu)": -4e-05,
-        "V3m(pu)": -4e-05,
+        "V1m(pu)": 0.97253,
+        "V2m(pu)": 2e-05,
+        "V3m(pu)": 2e-05,
         "bus_name": "bus_9",
         "num_nodes": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0
     },
     "6": {
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991071428571429%*

 * *Differences: {"'0'": "{'Q1mft(pu)': 0.12844}"}*

```diff
@@ -2,15 +2,15 @@
     "0": {
         "I1mft(pu)": 0,
         "I2mft(pu)": 0,
         "I3mft(pu)": 0,
         "P1mft(pu)": 0.1254,
         "P2mft(pu)": -2e-05,
         "P3mft(pu)": -2e-05,
-        "Q1mft(pu)": 0.12847,
+        "Q1mft(pu)": 0.12844,
         "Q2mft(pu)": -2e-05,
         "Q3mft(pu)": -2e-05,
         "Rii_Ift": 0,
         "Rii_PQft": 0.0001,
         "STS_Ift": 0,
         "STS_PQft": 1,
         "element_name": "Line.from_1_to_2",
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'2'": "{'I1mft(pu)': 0.05904, 'I2mft(pu)': -7e-05, 'I3mft(pu)': -7e-05, 'Ang1m(deg)': -45.63928, "*

 * *        "'Ang2m(deg)': -7e-05, 'Ang3m(deg)': -7e-05}",*

 * * "'5'": "{'I1mft(pu)': 0.00651, 'I2mft(pu)': 4e-05, 'I3mft(pu)': 4e-05, 'Ang1m(deg)': -45.53948, "*

 * *        "'Ang2m(deg)': 4e-05, 'Ang3m(deg)': 4e-05}"}*

```diff
@@ -98,20 +98,20 @@
         "num_ph": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0,
         "to_bus": "bus_15"
     },
     "2": {
-        "Ang1m(deg)": -45.64543,
-        "Ang2m(deg)": 8e-05,
-        "Ang3m(deg)": 8e-05,
-        "I1mft(pu)": 0.0592,
-        "I2mft(pu)": 8e-05,
-        "I3mft(pu)": 8e-05,
+        "Ang1m(deg)": -45.63928,
+        "Ang2m(deg)": -7e-05,
+        "Ang3m(deg)": -7e-05,
+        "I1mft(pu)": 0.05904,
+        "I2mft(pu)": -7e-05,
+        "I3mft(pu)": -7e-05,
         "Rii_Ift": 4.44889e-05,
         "STS_Ift": 1,
         "element_name": "Line.from_3_to_4",
         "from_bus": "bus_3",
         "num_ph": 1,
         "ph_1": 1,
         "ph_2": 0,
@@ -149,20 +149,20 @@
         "num_ph": 1,
         "ph_1": 1,
         "ph_2": 0,
         "ph_3": 0,
         "to_bus": "bus_9"
     },
     "5": {
-        "Ang1m(deg)": -45.55481,
-        "Ang2m(deg)": 3e-05,
-        "Ang3m(deg)": 3e-05,
-        "I1mft(pu)": 0.0065,
-        "I2mft(pu)": 3e-05,
-        "I3mft(pu)": 3e-05,
+        "Ang1m(deg)": -45.53948,
+        "Ang2m(deg)": 4e-05,
+        "Ang3m(deg)": 4e-05,
+        "I1mft(pu)": 0.00651,
+        "I2mft(pu)": 4e-05,
+        "I3mft(pu)": 4e-05,
         "Rii_Ift": 1.10889e-05,
         "STS_Ift": 1,
         "element_name": "Line.from_9_to_10",
         "from_bus": "bus_9",
         "num_ph": 1,
         "ph_1": 1,
         "ph_2": 0,
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Line_15node.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/OpenDSS files/Load_15node.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8611111111111113%*

 * *Differences: {"'0'": "{'V1(pu)_DSS': 1.0093943268, 'Ang1(deg)_DSS': 0.0767353721}",*

 * * "'1'": "{'V1(pu)_DSS': 0.9749754489, 'Ang1(deg)_DSS': -0.0505345218, 'Ang1(deg)_EST': 0.1028}",*

 * * "'10'": "{'V1(pu)_DSS': 0.9575286849, 'Ang1(deg)_DSS': -0.0682673309, 'Ang1(deg)_EST': 0.1}",*

 * * "'11'": "{'V1(pu)_DSS': 0.9554739976, 'Ang1(deg)_DSS': -0.0780726925, 'V1(pu)_EST': 0.9551, "*

 * *         "'Ang1(deg)_EST': 0.0996}",*

 * * "'12'": "{'V1(pu)_DSS': 0.9537598652, 'Ang1(deg)_DSS': -0.0862057896, 'V1(pu)_EST': 0.9535, "*

 * *         "'Ang1(deg)_E […]*

```diff
@@ -1,122 +1,122 @@
 {
     "0": {
-        "Ang1(deg)_DSS": 0.0767375249,
+        "Ang1(deg)_DSS": 0.0767353721,
         "Ang1(deg)_EST": 0.1,
         "Bus Nro.": 1,
-        "V1(pu)_DSS": 1.0093941652,
+        "V1(pu)_DSS": 1.0093943268,
         "V1(pu)_EST": 1.0094,
         "bus_name": "bus_1"
     },
     "1": {
-        "Ang1(deg)_DSS": -0.0502951368,
-        "Ang1(deg)_EST": 0.1019,
+        "Ang1(deg)_DSS": -0.0505345218,
+        "Ang1(deg)_EST": 0.1028,
         "Bus Nro.": 2,
-        "V1(pu)_DSS": 0.9749701865,
+        "V1(pu)_DSS": 0.9749754489,
         "V1(pu)_EST": 0.975,
         "bus_name": "bus_2"
     },
     "10": {
-        "Ang1(deg)_DSS": -0.0679005467,
-        "Ang1(deg)_EST": 0.1007,
+        "Ang1(deg)_DSS": -0.0682673309,
+        "Ang1(deg)_EST": 0.1,
         "Bus Nro.": 11,
-        "V1(pu)_DSS": 0.9575210301,
+        "V1(pu)_DSS": 0.9575286849,
         "V1(pu)_EST": 0.9573,
         "bus_name": "bus_11"
     },
     "11": {
-        "Ang1(deg)_DSS": -0.0776827553,
-        "Ang1(deg)_EST": 0.1002,
+        "Ang1(deg)_DSS": -0.0780726925,
+        "Ang1(deg)_EST": 0.0996,
         "Bus Nro.": 12,
-        "V1(pu)_DSS": 0.9554658593,
-        "V1(pu)_EST": 0.9553,
+        "V1(pu)_DSS": 0.9554739976,
+        "V1(pu)_EST": 0.9551,
         "bus_name": "bus_12"
     },
     "12": {
-        "Ang1(deg)_DSS": -0.0858082088,
-        "Ang1(deg)_EST": 0.1032,
+        "Ang1(deg)_DSS": -0.0862057896,
+        "Ang1(deg)_EST": 0.1017,
         "Bus Nro.": 13,
-        "V1(pu)_DSS": 0.9537515569,
-        "V1(pu)_EST": 0.9536,
+        "V1(pu)_DSS": 0.9537598652,
+        "V1(pu)_EST": 0.9535,
         "bus_name": "bus_13"
     },
     "13": {
-        "Ang1(deg)_DSS": -0.1071108076,
-        "Ang1(deg)_EST": 0.1067,
+        "Ang1(deg)_DSS": -0.1075007038,
+        "Ang1(deg)_EST": 0.1055,
         "Bus Nro.": 14,
-        "V1(pu)_DSS": 0.9515140319,
-        "V1(pu)_EST": 0.952,
+        "V1(pu)_DSS": 0.9515221951,
+        "V1(pu)_EST": 0.9519,
         "bus_name": "bus_14"
     },
     "14": {
-        "Ang1(deg)_DSS": -0.1226960965,
-        "Ang1(deg)_EST": 0.1118,
+        "Ang1(deg)_DSS": -0.1230862792,
+        "Ang1(deg)_EST": 0.1107,
         "Bus Nro.": 15,
-        "V1(pu)_DSS": 0.949911986,
-        "V1(pu)_EST": 0.9504,
+        "V1(pu)_DSS": 0.949920105,
+        "V1(pu)_EST": 0.9503,
         "bus_name": "bus_15"
     },
     "2": {
-        "Ang1(deg)_DSS": -0.0548695465,
-        "Ang1(deg)_EST": 0.0993,
+        "Ang1(deg)_DSS": -0.0552016211,
+        "Ang1(deg)_EST": 0.0985,
         "Bus Nro.": 3,
-        "V1(pu)_DSS": 0.9622835359,
+        "V1(pu)_DSS": 0.9622904955,
         "V1(pu)_EST": 0.9623,
         "bus_name": "bus_3"
     },
     "3": {
-        "Ang1(deg)_DSS": -0.0915301826,
-        "Ang1(deg)_EST": 0.0953,
+        "Ang1(deg)_DSS": -0.0919137746,
+        "Ang1(deg)_EST": 0.0963,
         "Bus Nro.": 4,
-        "V1(pu)_DSS": 0.953111372,
+        "V1(pu)_DSS": 0.9531193669,
         "V1(pu)_EST": 0.9531,
         "bus_name": "bus_4"
     },
     "4": {
-        "Ang1(deg)_DSS": -0.096437394,
-        "Ang1(deg)_EST": 0.1054,
+        "Ang1(deg)_DSS": -0.0968286182,
+        "Ang1(deg)_EST": 0.1038,
         "Bus Nro.": 5,
-        "V1(pu)_DSS": 0.9520432794,
-        "V1(pu)_EST": 0.9524,
+        "V1(pu)_DSS": 0.9520514359,
+        "V1(pu)_EST": 0.9523,
         "bus_name": "bus_5"
     },
     "5": {
-        "Ang1(deg)_DSS": -0.0581122674,
+        "Ang1(deg)_DSS": -0.0583730895,
         "Ang1(deg)_EST": 0.0997,
         "Bus Nro.": 6,
-        "V1(pu)_DSS": 0.9725098502,
+        "V1(pu)_DSS": 0.972515543,
         "V1(pu)_EST": 0.9725,
         "bus_name": "bus_9"
     },
     "6": {
-        "Ang1(deg)_DSS": -0.0596440806,
+        "Ang1(deg)_DSS": -0.0599116109,
         "Ang1(deg)_EST": 0.1001,
         "Bus Nro.": 7,
-        "V1(pu)_DSS": 0.9716422375,
-        "V1(pu)_EST": 0.9716,
+        "V1(pu)_DSS": 0.9716480589,
+        "V1(pu)_EST": 0.9717,
         "bus_name": "bus_10"
     },
     "7": {
-        "Ang1(deg)_DSS": -0.0740747356,
-        "Ang1(deg)_EST": 0.1016,
+        "Ang1(deg)_DSS": -0.074349425,
+        "Ang1(deg)_EST": 0.101,
         "Bus Nro.": 8,
-        "V1(pu)_DSS": 0.9673859345,
+        "V1(pu)_DSS": 0.967391932,
         "V1(pu)_EST": 0.9674,
         "bus_name": "bus_6"
     },
     "8": {
-        "Ang1(deg)_DSS": -0.0836552305,
-        "Ang1(deg)_EST": 0.0981,
+        "Ang1(deg)_DSS": -0.0839369621,
+        "Ang1(deg)_EST": 0.1005,
         "Bus Nro.": 9,
-        "V1(pu)_DSS": 0.9643468002,
-        "V1(pu)_EST": 0.9642,
+        "V1(pu)_DSS": 0.9643529542,
+        "V1(pu)_EST": 0.9643,
         "bus_name": "bus_7"
     },
     "9": {
-        "Ang1(deg)_DSS": -0.0788754237,
-        "Ang1(deg)_EST": 0.0967,
+        "Ang1(deg)_DSS": -0.0791572268,
+        "Ang1(deg)_EST": 0.0989,
         "Bus Nro.": 10,
-        "V1(pu)_DSS": 0.9658691103,
-        "V1(pu)_EST": 0.9658,
+        "V1(pu)_DSS": 0.9658752549,
+        "V1(pu)_EST": 0.9659,
         "bus_name": "bus_8"
     }
 }
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788961038961036%*

 * *Differences: {"'0'": "{'P3md(pu)': -0.02804, 'Q3md(pu)': -0.00656}",*

 * * "'1'": "{'V1m(pu)': 0.97638, 'V2m(pu)': 0.98467, 'V3m(pu)': 0.97901}",*

 * * "'10'": "{'P2md(pu)': -0.00562, 'Q3md(pu)': -0.00439}",*

 * * "'11'": "{'P1md(pu)': -0.00302}",*

 * * "'13'": "{'Q3md(pu)': -0.00229}",*

 * * "'15'": "{'P2md(pu)': -0.00231, 'Q3md(pu)': -0.00188}",*

 * * "'16'": "{'P2md(pu)': -0.00907, 'P3md(pu)': -0.00648, 'Q1md(pu)': -0.0014, 'Q3md(pu)': -0.00742}",*

 * * "'17'": "{'V1m(pu)': 0.95783, 'V2m(pu)': 0.97289, 'V3m(pu)': 0.96788}",*

 * * "'18'": "{'P1md(pu)': -0.0 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "0": {
         "P1md(pu)": -0.02186,
         "P2md(pu)": -0.01451,
-        "P3md(pu)": -0.02803,
+        "P3md(pu)": -0.02804,
         "Q1md(pu)": -0.01884,
         "Q2md(pu)": -0.0075,
-        "Q3md(pu)": -0.00657,
+        "Q3md(pu)": -0.00656,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 1,
         "STS_PQd(SM)": 0,
@@ -34,30 +34,30 @@
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 1,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 0,
         "STS_Vm": 1,
-        "V1m(pu)": 0.97803,
-        "V2m(pu)": 0.98565,
-        "V3m(pu)": 0.97984,
+        "V1m(pu)": 0.97638,
+        "V2m(pu)": 0.98467,
+        "V3m(pu)": 0.97901,
         "bus_name": "702",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "10": {
         "P1md(pu)": -0.00062,
-        "P2md(pu)": -0.00563,
+        "P2md(pu)": -0.00562,
         "P3md(pu)": -0.0031,
         "Q1md(pu)": -0.0001,
         "Q2md(pu)": -0.00013,
-        "Q3md(pu)": -0.0044,
+        "Q3md(pu)": -0.00439,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
@@ -68,15 +68,15 @@
         "bus_name": "742",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "11": {
-        "P1md(pu)": -0.00303,
+        "P1md(pu)": -0.00302,
         "P2md(pu)": 5e-05,
         "P3md(pu)": -0.00537,
         "Q1md(pu)": -0.00443,
         "Q2md(pu)": 5e-05,
         "Q3md(pu)": 0.00053,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
@@ -121,15 +121,15 @@
     },
     "13": {
         "P1md(pu)": -4e-05,
         "P2md(pu)": -0.00276,
         "P3md(pu)": -0.00153,
         "Q1md(pu)": -4e-05,
         "Q2md(pu)": 0.00011,
-        "Q3md(pu)": -0.0023,
+        "Q3md(pu)": -0.00229,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
@@ -165,19 +165,19 @@
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "15": {
         "P1md(pu)": 0.00024,
-        "P2md(pu)": -0.00232,
+        "P2md(pu)": -0.00231,
         "P3md(pu)": -0.00115,
         "Q1md(pu)": 0.00024,
         "Q2md(pu)": 0.00039,
-        "Q3md(pu)": -0.00189,
+        "Q3md(pu)": -0.00188,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
@@ -189,19 +189,19 @@
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "16": {
         "P1md(pu)": -0.00109,
-        "P2md(pu)": -0.00908,
-        "P3md(pu)": -0.00649,
-        "Q1md(pu)": -0.00141,
+        "P2md(pu)": -0.00907,
+        "P3md(pu)": -0.00648,
+        "Q1md(pu)": -0.0014,
         "Q2md(pu)": 0.00027,
-        "Q3md(pu)": -0.00744,
+        "Q3md(pu)": -0.00742,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 1,
         "STS_PQd(SM)": 0,
@@ -226,29 +226,29 @@
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 1,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 0,
         "STS_Vm": 1,
-        "V1m(pu)": 0.96043,
-        "V2m(pu)": 0.97463,
-        "V3m(pu)": 0.96887,
+        "V1m(pu)": 0.95783,
+        "V2m(pu)": 0.97289,
+        "V3m(pu)": 0.96788,
         "bus_name": "708",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "18": {
-        "P1md(pu)": -0.00556,
-        "P2md(pu)": -0.00349,
+        "P1md(pu)": -0.00554,
+        "P2md(pu)": -0.00348,
         "P3md(pu)": -0.00042,
-        "Q1md(pu)": 0.00011,
-        "Q2md(pu)": -0.00468,
+        "Q1md(pu)": 0.00012,
+        "Q2md(pu)": -0.00467,
         "Q3md(pu)": -0.00042,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 1,
@@ -262,15 +262,15 @@
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "19": {
         "P1md(pu)": -0.00181,
         "P2md(pu)": -0.00034,
-        "P3md(pu)": -0.00306,
+        "P3md(pu)": -0.00307,
         "Q1md(pu)": -0.00261,
         "Q2md(pu)": -0.00034,
         "Q3md(pu)": -0.00016,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
@@ -333,19 +333,19 @@
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "21": {
         "P1md(pu)": -0.00034,
-        "P2md(pu)": -0.00549,
+        "P2md(pu)": -0.00548,
         "P3md(pu)": -0.00329,
         "Q1md(pu)": -0.00034,
-        "Q2md(pu)": 5e-05,
-        "Q3md(pu)": -0.00455,
+        "Q2md(pu)": 4e-05,
+        "Q3md(pu)": -0.00453,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
@@ -380,18 +380,18 @@
         "bus_name": "710",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "23": {
-        "P1md(pu)": -0.0031,
+        "P1md(pu)": -0.00309,
         "P2md(pu)": -5e-05,
-        "P3md(pu)": -0.00551,
-        "Q1md(pu)": -0.00454,
+        "P3md(pu)": -0.00552,
+        "Q1md(pu)": -0.00453,
         "Q2md(pu)": -5e-05,
         "Q3md(pu)": 0.00043,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
@@ -405,30 +405,30 @@
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "24": {
         "P1md(pu)": -6e-05,
-        "P2md(pu)": -0.00261,
+        "P2md(pu)": -0.0026,
         "P3md(pu)": -0.00147,
         "Q1md(pu)": -6e-05,
         "Q2md(pu)": 6e-05,
-        "Q3md(pu)": -0.00217,
+        "Q3md(pu)": -0.00216,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
         "STS_Vm": 1,
-        "V1m(pu)": 0.95311,
-        "V2m(pu)": 0.96913,
-        "V3m(pu)": 0.96303,
+        "V1m(pu)": 0.95017,
+        "V2m(pu)": 0.96715,
+        "V3m(pu)": 0.96196,
         "bus_name": "736",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "25": {
@@ -452,20 +452,20 @@
         "bus_name": "711",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "26": {
-        "P1md(pu)": -0.00123,
+        "P1md(pu)": -0.00127,
         "P2md(pu)": 0.00019,
-        "P3md(pu)": -0.00239,
-        "Q1md(pu)": -0.00193,
+        "P3md(pu)": -0.00255,
+        "Q1md(pu)": -0.00208,
         "Q2md(pu)": 0.00019,
-        "Q3md(pu)": 0.0004,
+        "Q3md(pu)": 0.00036,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
@@ -476,18 +476,18 @@
         "bus_name": "741",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "27": {
-        "P1md(pu)": -0.00304,
+        "P1md(pu)": -0.00303,
         "P2md(pu)": -1e-05,
-        "P3md(pu)": -0.00548,
-        "Q1md(pu)": -0.00449,
+        "P3md(pu)": -0.00547,
+        "Q1md(pu)": -0.00448,
         "Q2md(pu)": -1e-05,
         "Q3md(pu)": 0.00047,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
@@ -500,19 +500,19 @@
         "bus_name": "740",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "28": {
-        "P1md(pu)": -0.00533,
+        "P1md(pu)": -0.00531,
         "P2md(pu)": -0.00316,
         "P3md(pu)": -0.00018,
         "Q1md(pu)": 0.00025,
-        "Q2md(pu)": -0.00445,
+        "Q2md(pu)": -0.00443,
         "Q3md(pu)": -0.00018,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
@@ -550,29 +550,29 @@
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "3": {
         "P1md(pu)": -0.00321,
         "P2md(pu)": -0.00013,
-        "P3md(pu)": -0.00555,
+        "P3md(pu)": -0.00556,
         "Q1md(pu)": -0.00461,
         "Q2md(pu)": -0.00013,
         "Q3md(pu)": 0.00034,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 1,
         "STS_PQd(SM)": 0,
         "STS_Vm": 1,
-        "V1m(pu)": 0.9764,
-        "V2m(pu)": 0.98389,
-        "V3m(pu)": 0.97768,
+        "V1m(pu)": 0.97467,
+        "V2m(pu)": 0.98289,
+        "V3m(pu)": 0.97678,
         "bus_name": "713",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "30": {
@@ -596,19 +596,19 @@
         "bus_name": "734",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "31": {
-        "P1md(pu)": -0.00766,
-        "P2md(pu)": -0.0041,
+        "P1md(pu)": -0.00763,
+        "P2md(pu)": -0.00409,
         "P3md(pu)": 0.00083,
-        "Q1md(pu)": 0.00155,
-        "Q2md(pu)": -0.00632,
+        "Q1md(pu)": 0.00157,
+        "Q2md(pu)": -0.0063,
         "Q3md(pu)": 0.00083,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 1,
@@ -623,36 +623,36 @@
         "ph_2": 1,
         "ph_3": 1
     },
     "32": {
         "P1md(pu)": -0.00765,
         "P2md(pu)": -0.00421,
         "P3md(pu)": 0.00037,
-        "Q1md(pu)": 0.00097,
-        "Q2md(pu)": -0.00643,
+        "Q1md(pu)": 0.00098,
+        "Q2md(pu)": -0.00644,
         "Q3md(pu)": 0.00037,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 1,
         "STS_PQd(SM)": 0,
         "STS_Vm": 1,
-        "V1m(pu)": 0.94973,
-        "V2m(pu)": 0.96847,
-        "V3m(pu)": 0.9642,
+        "V1m(pu)": 0.94669,
+        "V2m(pu)": 0.96627,
+        "V3m(pu)": 0.9632,
         "bus_name": "738",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "33": {
-        "P1md(pu)": -0.00427,
+        "P1md(pu)": -0.00426,
         "P2md(pu)": -0.00431,
         "P3md(pu)": -0.00431,
         "Q1md(pu)": -0.0022,
         "Q2md(pu)": -0.00222,
         "Q3md(pu)": -0.00217,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
@@ -671,28 +671,28 @@
         "ph_2": 1,
         "ph_3": 1
     },
     "34": {
         "P1md(pu)": -0.00263,
         "P2md(pu)": -0.00151,
         "P3md(pu)": -3e-05,
-        "Q1md(pu)": 0.00016,
+        "Q1md(pu)": 0.00017,
         "Q2md(pu)": -0.00221,
         "Q3md(pu)": -3e-05,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0,
         "Rii_SM": 0.0002778889,
         "Rii_Vm": 0.0001,
         "STS_PQd(0)": 0,
         "STS_PQd(Psd)": 0,
         "STS_PQd(SM)": 1,
         "STS_Vm": 1,
-        "V1m(pu)": 0.96822,
-        "V2m(pu)": 0.97895,
-        "V3m(pu)": 0.97384,
+        "V1m(pu)": 0.96604,
+        "V2m(pu)": 0.97748,
+        "V3m(pu)": 0.97291,
         "bus_name": "729",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "4": {
@@ -740,18 +740,18 @@
         "bus_name": "727",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "6": {
-        "P1md(pu)": -0.00258,
+        "P1md(pu)": -0.00257,
         "P2md(pu)": 0.00027,
-        "P3md(pu)": -0.0048,
-        "Q1md(pu)": -0.0039,
+        "P3md(pu)": -0.00478,
+        "Q1md(pu)": -0.00389,
         "Q2md(pu)": 0.00027,
         "Q3md(pu)": 0.00071,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
         "Rii_SM": 0.0,
         "Rii_Vm": 0.0,
         "STS_PQd(0)": 0,
@@ -812,15 +812,15 @@
         "bus_name": "714",
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "9": {
-        "P1md(pu)": -0.00329,
+        "P1md(pu)": -0.00328,
         "P2md(pu)": -0.0002,
         "P3md(pu)": -0.00561,
         "Q1md(pu)": -0.00468,
         "Q2md(pu)": -0.0002,
         "Q3md(pu)": 0.00028,
         "Rii_0": 0.0,
         "Rii_Psd": 0.0025,
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9903846153846154%*

 * *Differences: {"'18'": "{'V1m(pu)': 0.95789, 'V2m(pu)': 0.97294, 'V3m(pu)': 0.96794, 'Ang1m(deg)': 29.5925, "*

 * *         "'Ang2m(deg)': -90.23715, 'Ang3m(deg)': 148.85664}",*

 * * "'26'": "{'V1m(pu)': 0.94592, 'V2m(pu)': 0.96625, 'V3m(pu)': 0.96252, 'Ang1m(deg)': 29.513, "*

 * *         "'Ang2m(deg)': -90.05277, 'Ang3m(deg)': 148.61348}",*

 * * "'5'": "{'V1m(pu)': 0.96836, 'V2m(pu)': 0.97942, 'V3m(pu)': 0.97411, 'Ang1m(deg)': 29.63339, "*

 * *        "'Ang2m(deg)': -90.34584, 'Ang3m(deg)': 149.04858}"}*

```diff
@@ -146,22 +146,22 @@
         "bus_name": 722,
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "18": {
-        "Ang1m(deg)": 29.82332,
-        "Ang2m(deg)": -90.08636,
-        "Ang3m(deg)": 149.09218,
+        "Ang1m(deg)": 29.5925,
+        "Ang2m(deg)": -90.23715,
+        "Ang3m(deg)": 148.85664,
         "Rii_Vm": 1.10889e-05,
         "STS_Vm": 1,
-        "V1m(pu)": 0.96049,
-        "V2m(pu)": 0.97469,
-        "V3m(pu)": 0.96893,
+        "V1m(pu)": 0.95789,
+        "V2m(pu)": 0.97294,
+        "V3m(pu)": 0.96794,
         "bus_name": 708,
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "19": {
@@ -281,22 +281,22 @@
         "bus_name": 736,
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "26": {
-        "Ang1m(deg)": 29.79543,
-        "Ang2m(deg)": -89.88203,
-        "Ang3m(deg)": 148.88843,
+        "Ang1m(deg)": 29.513,
+        "Ang2m(deg)": -90.05277,
+        "Ang3m(deg)": 148.61348,
         "Rii_Vm": 1.10889e-05,
         "STS_Vm": 1,
-        "V1m(pu)": 0.94903,
-        "V2m(pu)": 0.96845,
-        "V3m(pu)": 0.96353,
+        "V1m(pu)": 0.94592,
+        "V2m(pu)": 0.96625,
+        "V3m(pu)": 0.96252,
         "bus_name": 711,
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "27": {
@@ -461,22 +461,22 @@
         "bus_name": 713,
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "5": {
-        "Ang1m(deg)": 29.82018,
-        "Ang2m(deg)": -90.21673,
-        "Ang3m(deg)": 149.24537,
+        "Ang1m(deg)": 29.63339,
+        "Ang2m(deg)": -90.34584,
+        "Ang3m(deg)": 149.04858,
         "Rii_Vm": 1.10889e-05,
         "STS_Vm": 1,
-        "V1m(pu)": 0.9705,
-        "V2m(pu)": 0.9808,
-        "V3m(pu)": 0.97503,
+        "V1m(pu)": 0.96836,
+        "V2m(pu)": 0.97942,
+        "V3m(pu)": 0.97411,
         "bus_name": 703,
         "num_nodes": 3,
         "ph_1": 1,
         "ph_2": 1,
         "ph_3": 1
     },
     "6": {
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992142857142857%*

 * *Differences: {"'13'": "{'P1mft(pu)': 0.03078, 'P2mft(pu)': 0.01515, 'P3mft(pu)': 0.01784, 'Q1mft(pu)': 0.01164, "*

 * *         "'Q2mft(pu)': 0.01801, 'Q3mft(pu)': 0.00074}",*

 * * "'21'": "{'P1mft(pu)': 0.01021, 'P2mft(pu)': 0.0192, 'Q2mft(pu)': 0.00427, 'Q3mft(pu)': 0.01225}",*

 * * "'3'": "{'P1mft(pu)': 0.04671, 'P2mft(pu)': 0.02779, 'P3mft(pu)': 0.0358, 'Q1mft(pu)': 0.02251, "*

 * *        "'Q2mft(pu)': 0.02436, 'Q3mft(pu)': 0.00645}",*

 * * "'34'": "{'P1mft(pu)': 0.08661, 'P2mft(pu)': 0.06726, 'P3mft(pu)': 0.09416, 'Q1mft(pu)': 0.05629, "*

 * * […]*

```diff
@@ -109,20 +109,20 @@
         "ph_3": 1,
         "to_bus": "722"
     },
     "13": {
         "I1mft(pu)": 0,
         "I2mft(pu)": 0,
         "I3mft(pu)": 0,
-        "P1mft(pu)": 0.03081,
-        "P2mft(pu)": 0.01517,
-        "P3mft(pu)": 0.01767,
-        "Q1mft(pu)": 0.01152,
-        "Q2mft(pu)": 0.01803,
-        "Q3mft(pu)": 0.00069,
+        "P1mft(pu)": 0.03078,
+        "P2mft(pu)": 0.01515,
+        "P3mft(pu)": 0.01784,
+        "Q1mft(pu)": 0.01164,
+        "Q2mft(pu)": 0.01801,
+        "Q3mft(pu)": 0.00074,
         "Rii_Ift": 0,
         "Rii_PQft": 0.0001,
         "STS_Ift": 0,
         "STS_PQft": 1,
         "element_name": "Line.l14",
         "from_bus": "708",
         "num_ph": 3,
@@ -307,20 +307,20 @@
         "ph_3": 1,
         "to_bus": "740"
     },
     "21": {
         "I1mft(pu)": 0,
         "I2mft(pu)": 0,
         "I3mft(pu)": 0,
-        "P1mft(pu)": 0.01023,
-        "P2mft(pu)": 0.01923,
+        "P1mft(pu)": 0.01021,
+        "P2mft(pu)": 0.0192,
         "P3mft(pu)": 0.01551,
         "Q1mft(pu)": 0.00515,
-        "Q2mft(pu)": 0.00428,
-        "Q3mft(pu)": 0.01227,
+        "Q2mft(pu)": 0.00427,
+        "Q3mft(pu)": 0.01225,
         "Rii_Ift": 0,
         "Rii_PQft": 0.0001,
         "STS_Ift": 0,
         "STS_PQft": 1,
         "element_name": "Line.l22",
         "from_bus": "713",
         "num_ph": 3,
@@ -505,20 +505,20 @@
         "ph_3": 1,
         "to_bus": "710"
     },
     "3": {
         "I1mft(pu)": 0,
         "I2mft(pu)": 0,
         "I3mft(pu)": 0,
-        "P1mft(pu)": 0.04676,
-        "P2mft(pu)": 0.02783,
-        "P3mft(pu)": 0.03564,
-        "Q1mft(pu)": 0.02233,
-        "Q2mft(pu)": 0.02435,
-        "Q3mft(pu)": 0.00637,
+        "P1mft(pu)": 0.04671,
+        "P2mft(pu)": 0.02779,
+        "P3mft(pu)": 0.0358,
+        "Q1mft(pu)": 0.02251,
+        "Q2mft(pu)": 0.02436,
+        "Q3mft(pu)": 0.00645,
         "Rii_Ift": 0,
         "Rii_PQft": 0.0001,
         "STS_Ift": 0,
         "STS_PQft": 1,
         "element_name": "Line.l4",
         "from_bus": "702",
         "num_ph": 3,
@@ -615,20 +615,20 @@
         "ph_3": 1,
         "to_bus": "729"
     },
     "34": {
         "I1mft(pu)": 0,
         "I2mft(pu)": 0,
         "I3mft(pu)": 0,
-        "P1mft(pu)": 0.08669,
-        "P2mft(pu)": 0.06734,
-        "P3mft(pu)": 0.09399,
-        "Q1mft(pu)": 0.05586,
-        "Q2mft(pu)": 0.03626,
-        "Q3mft(pu)": 0.0293,
+        "P1mft(pu)": 0.08661,
+        "P2mft(pu)": 0.06726,
+        "P3mft(pu)": 0.09416,
+        "Q1mft(pu)": 0.05629,
+        "Q2mft(pu)": 0.03641,
+        "Q3mft(pu)": 0.0296,
         "Rii_Ift": 0,
         "Rii_PQft": 0.0001,
         "STS_Ift": 0,
         "STS_PQft": 1,
         "element_name": "Line.l35",
         "from_bus": "799",
         "num_ph": 3,
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/AddMarks.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEE37_BusXY.csv`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Isolated.Txt`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.dbl`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/ieee37_Power.DSV`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/IEEELineCodes.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Lines.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Loads.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/BusCoords.dss`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Line.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/LineCode.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Load.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/Spectrum.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/PosSeq circuit/TCC_Curve.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/OpenDSS files/Regulator.DSS`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8356481481481477%*

 * *Differences: {"'0'": "{'V1(pu)_DSS': 0.9999978463, 'Ang1(deg)_DSS': 29.9993976002, 'V1(pu)_EST': 1.0004}",*

 * * "'1'": "{'V1(pu)_DSS': 0.9871461083, 'Ang1(deg)_DSS': 29.7346303293, 'V1(pu)_EST': 0.9875, "*

 * *        "'Ang1(deg)_EST': 30.0002}",*

 * * "'10'": "{'V1(pu)_DSS': 0.9742835493, 'Ang1(deg)_DSS': 29.5596200457, 'V1(pu)_EST': 0.9753}",*

 * * "'11'": "{'V1(pu)_DSS': 0.9787364071, 'Ang1(deg)_DSS': 29.5963657063, 'V1(pu)_EST': 0.9773, "*

 * *         "'Ang1(deg)_EST': 29.958}",*

 * * "'12'": "{'V1(pu)_DSS': 0.9788612321, 'Ang1(deg)_DSS': 29.5 […]*

```diff
@@ -1,290 +1,290 @@
 {
     "0": {
-        "Ang1(deg)_DSS": 29.9993976723,
+        "Ang1(deg)_DSS": 29.9993976002,
         "Ang1(deg)_EST": 30.0,
         "Bus Nro.": 1,
-        "V1(pu)_DSS": 0.9999978411,
-        "V1(pu)_EST": 1.0009,
+        "V1(pu)_DSS": 0.9999978463,
+        "V1(pu)_EST": 1.0004,
         "bus_name": "799"
     },
     "1": {
-        "Ang1(deg)_DSS": 29.7348202449,
-        "Ang1(deg)_EST": 29.9997,
+        "Ang1(deg)_DSS": 29.7346303293,
+        "Ang1(deg)_EST": 30.0002,
         "Bus Nro.": 2,
-        "V1(pu)_DSS": 0.9871426607,
-        "V1(pu)_EST": 0.9881,
+        "V1(pu)_DSS": 0.9871461083,
+        "V1(pu)_EST": 0.9875,
         "bus_name": "701"
     },
     "10": {
-        "Ang1(deg)_DSS": 29.5600447146,
+        "Ang1(deg)_DSS": 29.5596200457,
         "Ang1(deg)_EST": 30.0043,
         "Bus Nro.": 11,
-        "V1(pu)_DSS": 0.9742768096,
-        "V1(pu)_EST": 0.9761,
+        "V1(pu)_DSS": 0.9742835493,
+        "V1(pu)_EST": 0.9753,
         "bus_name": "720"
     },
     "11": {
-        "Ang1(deg)_DSS": 29.5966847236,
-        "Ang1(deg)_EST": 29.972,
+        "Ang1(deg)_DSS": 29.5963657063,
+        "Ang1(deg)_EST": 29.958,
         "Bus Nro.": 12,
-        "V1(pu)_DSS": 0.9787307589,
-        "V1(pu)_EST": 0.9787,
+        "V1(pu)_DSS": 0.9787364071,
+        "V1(pu)_EST": 0.9773,
         "bus_name": "742"
     },
     "12": {
-        "Ang1(deg)_DSS": 29.595688463,
-        "Ang1(deg)_EST": 29.9781,
+        "Ang1(deg)_DSS": 29.5953701519,
+        "Ang1(deg)_EST": 29.9668,
         "Bus Nro.": 13,
-        "V1(pu)_DSS": 0.9788555836,
-        "V1(pu)_EST": 0.9791,
+        "V1(pu)_DSS": 0.9788612321,
+        "V1(pu)_EST": 0.9778,
         "bus_name": "712"
     },
     "13": {
-        "Ang1(deg)_DSS": 29.5592916367,
-        "Ang1(deg)_EST": 30.0029,
+        "Ang1(deg)_DSS": 29.5588603623,
+        "Ang1(deg)_EST": 30.0026,
         "Bus Nro.": 14,
-        "V1(pu)_DSS": 0.9740532994,
-        "V1(pu)_EST": 0.9757,
+        "V1(pu)_DSS": 0.9740601048,
+        "V1(pu)_EST": 0.975,
         "bus_name": "706"
     },
     "14": {
-        "Ang1(deg)_DSS": 29.5609401474,
-        "Ang1(deg)_EST": 29.992,
+        "Ang1(deg)_DSS": 29.5605075656,
+        "Ang1(deg)_EST": 29.9926,
         "Bus Nro.": 15,
-        "V1(pu)_DSS": 0.9738703868,
-        "V1(pu)_EST": 0.975,
+        "V1(pu)_DSS": 0.9738772005,
+        "V1(pu)_EST": 0.9743,
         "bus_name": "725"
     },
     "15": {
-        "Ang1(deg)_DSS": 29.5832912094,
-        "Ang1(deg)_EST": 30.0032,
+        "Ang1(deg)_DSS": 29.5828265342,
+        "Ang1(deg)_EST": 30.003,
         "Bus Nro.": 16,
-        "V1(pu)_DSS": 0.9714760605,
-        "V1(pu)_EST": 0.9719,
+        "V1(pu)_DSS": 0.9714830144,
+        "V1(pu)_EST": 0.9712,
         "bus_name": "707"
     },
     "16": {
-        "Ang1(deg)_DSS": 29.5875031407,
-        "Ang1(deg)_EST": 29.9824,
+        "Ang1(deg)_DSS": 29.5870290061,
+        "Ang1(deg)_EST": 29.984,
         "Bus Nro.": 17,
-        "V1(pu)_DSS": 0.9710067186,
-        "V1(pu)_EST": 0.9703,
+        "V1(pu)_DSS": 0.9710137207,
+        "V1(pu)_EST": 0.9696,
         "bus_name": "724"
     },
     "17": {
-        "Ang1(deg)_DSS": 29.5856858071,
-        "Ang1(deg)_EST": 29.9952,
+        "Ang1(deg)_DSS": 29.5852209302,
+        "Ang1(deg)_EST": 29.9953,
         "Bus Nro.": 18,
-        "V1(pu)_DSS": 0.9711847672,
-        "V1(pu)_EST": 0.9713,
+        "V1(pu)_DSS": 0.9711917222,
+        "V1(pu)_EST": 0.9705,
         "bus_name": "722"
     },
     "18": {
-        "Ang1(deg)_DSS": 29.4258469204,
-        "Ang1(deg)_EST": 30.0012,
+        "Ang1(deg)_DSS": 29.4253207257,
+        "Ang1(deg)_EST": 30.0008,
         "Bus Nro.": 19,
-        "V1(pu)_DSS": 0.9667037333,
-        "V1(pu)_EST": 0.9653,
+        "V1(pu)_DSS": 0.9667122235,
+        "V1(pu)_EST": 0.9659,
         "bus_name": "708"
     },
     "19": {
-        "Ang1(deg)_DSS": 29.4180498285,
-        "Ang1(deg)_EST": 29.9997,
+        "Ang1(deg)_DSS": 29.4174950943,
+        "Ang1(deg)_EST": 29.9995,
         "Bus Nro.": 20,
-        "V1(pu)_DSS": 0.9648965456,
-        "V1(pu)_EST": 0.9635,
+        "V1(pu)_DSS": 0.9649053207,
+        "V1(pu)_EST": 0.9641,
         "bus_name": "733"
     },
     "2": {
-        "Ang1(deg)_DSS": 29.5852107751,
-        "Ang1(deg)_EST": 30.0069,
+        "Ang1(deg)_DSS": 29.5849034281,
+        "Ang1(deg)_EST": 30.0077,
         "Bus Nro.": 3,
-        "V1(pu)_DSS": 0.9802379307,
-        "V1(pu)_EST": 0.982,
+        "V1(pu)_DSS": 0.9802435176,
+        "V1(pu)_EST": 0.9813,
         "bus_name": "702"
     },
     "20": {
-        "Ang1(deg)_DSS": 29.4277587283,
-        "Ang1(deg)_EST": 29.9961,
+        "Ang1(deg)_DSS": 29.4272308224,
+        "Ang1(deg)_EST": 29.9972,
         "Bus Nro.": 21,
-        "V1(pu)_DSS": 0.9664931078,
-        "V1(pu)_EST": 0.9648,
+        "V1(pu)_DSS": 0.966501609,
+        "V1(pu)_EST": 0.9655,
         "bus_name": "732"
     },
     "21": {
-        "Ang1(deg)_DSS": 29.4340225184,
-        "Ang1(deg)_EST": 30.0014,
+        "Ang1(deg)_DSS": 29.4335286235,
+        "Ang1(deg)_EST": 30.0002,
         "Bus Nro.": 22,
-        "V1(pu)_DSS": 0.968631036,
-        "V1(pu)_EST": 0.9672,
+        "V1(pu)_DSS": 0.9686392032,
+        "V1(pu)_EST": 0.9678,
         "bus_name": "709"
     },
     "22": {
-        "Ang1(deg)_DSS": 29.4320439934,
-        "Ang1(deg)_EST": 29.9826,
+        "Ang1(deg)_DSS": 29.4315463213,
+        "Ang1(deg)_EST": 29.9993,
         "Bus Nro.": 23,
-        "V1(pu)_DSS": 0.9682096474,
-        "V1(pu)_EST": 0.965,
+        "V1(pu)_DSS": 0.9682178474,
+        "V1(pu)_EST": 0.9668,
         "bus_name": "731"
     },
     "23": {
-        "Ang1(deg)_DSS": 29.4146710164,
-        "Ang1(deg)_EST": 30.0052,
+        "Ang1(deg)_DSS": 29.4140414971,
+        "Ang1(deg)_EST": 30.0083,
         "Bus Nro.": 24,
-        "V1(pu)_DSS": 0.9611289239,
-        "V1(pu)_EST": 0.959,
+        "V1(pu)_DSS": 0.9611383124,
+        "V1(pu)_EST": 0.9595,
         "bus_name": "710"
     },
     "24": {
-        "Ang1(deg)_DSS": 29.4167199247,
-        "Ang1(deg)_EST": 29.9911,
+        "Ang1(deg)_DSS": 29.4160897102,
+        "Ang1(deg)_EST": 29.9866,
         "Bus Nro.": 25,
-        "V1(pu)_DSS": 0.9608631005,
-        "V1(pu)_EST": 0.9581,
+        "V1(pu)_DSS": 0.9608724951,
+        "V1(pu)_EST": 0.9583,
         "bus_name": "735"
     },
     "25": {
-        "Ang1(deg)_DSS": 29.421707934,
-        "Ang1(deg)_EST": 29.9634,
+        "Ang1(deg)_DSS": 29.4210515907,
+        "Ang1(deg)_EST": 29.9427,
         "Bus Nro.": 26,
-        "V1(pu)_DSS": 0.9603474218,
-        "V1(pu)_EST": 0.9559,
+        "V1(pu)_DSS": 0.9603569473,
+        "V1(pu)_EST": 0.9553,
         "bus_name": "736"
     },
     "26": {
-        "Ang1(deg)_DSS": 29.3915477498,
-        "Ang1(deg)_EST": 30.0015,
+        "Ang1(deg)_DSS": 29.3909098429,
+        "Ang1(deg)_EST": 30.0007,
         "Bus Nro.": 27,
-        "V1(pu)_DSS": 0.9585844454,
-        "V1(pu)_EST": 0.9574,
+        "V1(pu)_DSS": 0.9585940596,
+        "V1(pu)_EST": 0.9586,
         "bus_name": "711"
     },
     "27": {
-        "Ang1(deg)_DSS": 29.3909242562,
-        "Ang1(deg)_EST": 29.9984,
+        "Ang1(deg)_DSS": 29.3902847088,
+        "Ang1(deg)_EST": 30.0012,
         "Bus Nro.": 28,
-        "V1(pu)_DSS": 0.9584405439,
-        "V1(pu)_EST": 0.9571,
+        "V1(pu)_DSS": 0.9584501738,
+        "V1(pu)_EST": 0.9585,
         "bus_name": "741"
     },
     "28": {
-        "Ang1(deg)_DSS": 29.3936075374,
-        "Ang1(deg)_EST": 29.9966,
+        "Ang1(deg)_DSS": 29.3929689339,
+        "Ang1(deg)_EST": 29.9973,
         "Bus Nro.": 29,
-        "V1(pu)_DSS": 0.9583179196,
-        "V1(pu)_EST": 0.9569,
+        "V1(pu)_DSS": 0.95832754,
+        "V1(pu)_EST": 0.9581,
         "bus_name": "740"
     },
     "29": {
-        "Ang1(deg)_DSS": 29.575356144,
-        "Ang1(deg)_EST": 29.9901,
+        "Ang1(deg)_DSS": 29.5749700185,
+        "Ang1(deg)_EST": 29.9908,
         "Bus Nro.": 30,
-        "V1(pu)_DSS": 0.975763436,
-        "V1(pu)_EST": 0.9768,
+        "V1(pu)_DSS": 0.9757697658,
+        "V1(pu)_EST": 0.9761,
         "bus_name": "718"
     },
     "3": {
-        "Ang1(deg)_DSS": 29.5933201684,
-        "Ang1(deg)_EST": 30.0114,
+        "Ang1(deg)_DSS": 29.5930028281,
+        "Ang1(deg)_EST": 30.0173,
         "Bus Nro.": 4,
-        "V1(pu)_DSS": 0.9791687263,
-        "V1(pu)_EST": 0.9806,
+        "V1(pu)_DSS": 0.9791743678,
+        "V1(pu)_EST": 0.98,
         "bus_name": "705"
     },
     "30": {
-        "Ang1(deg)_DSS": 29.4655283137,
-        "Ang1(deg)_EST": 30.0017,
+        "Ang1(deg)_DSS": 29.4651233602,
+        "Ang1(deg)_EST": 30.0104,
         "Bus Nro.": 31,
-        "V1(pu)_DSS": 0.9729767898,
-        "V1(pu)_EST": 0.9749,
+        "V1(pu)_DSS": 0.9729840498,
+        "V1(pu)_EST": 0.9727,
         "bus_name": "744"
     },
     "31": {
-        "Ang1(deg)_DSS": 29.4065825727,
-        "Ang1(deg)_EST": 30.0028,
+        "Ang1(deg)_DSS": 29.4059827552,
+        "Ang1(deg)_EST": 30.0033,
         "Bus Nro.": 32,
-        "V1(pu)_DSS": 0.962137105,
-        "V1(pu)_EST": 0.9608,
+        "V1(pu)_DSS": 0.9621463299,
+        "V1(pu)_EST": 0.9615,
         "bus_name": "734"
     },
     "32": {
-        "Ang1(deg)_DSS": 29.3973508009,
-        "Ang1(deg)_EST": 30.0005,
+        "Ang1(deg)_DSS": 29.3967288468,
+        "Ang1(deg)_EST": 30.0003,
         "Bus Nro.": 33,
-        "V1(pu)_DSS": 0.9599303213,
-        "V1(pu)_EST": 0.9588,
+        "V1(pu)_DSS": 0.9599397716,
+        "V1(pu)_EST": 0.9597,
         "bus_name": "737"
     },
     "33": {
-        "Ang1(deg)_DSS": 29.3936170086,
-        "Ang1(deg)_EST": 30.0002,
+        "Ang1(deg)_DSS": 29.3929854209,
+        "Ang1(deg)_EST": 30.0003,
         "Bus Nro.": 34,
-        "V1(pu)_DSS": 0.959030984,
-        "V1(pu)_EST": 0.9579,
+        "V1(pu)_DSS": 0.9590405345,
+        "V1(pu)_EST": 0.9589,
         "bus_name": "738"
     },
     "34": {
-        "Ang1(deg)_DSS": 29.4690798818,
-        "Ang1(deg)_EST": 29.994,
+        "Ang1(deg)_DSS": 29.4686742202,
+        "Ang1(deg)_EST": 29.9897,
         "Bus Nro.": 35,
-        "V1(pu)_DSS": 0.9725842633,
-        "V1(pu)_EST": 0.9741,
+        "V1(pu)_DSS": 0.9725915298,
+        "V1(pu)_EST": 0.9715,
         "bus_name": "728"
     },
     "35": {
-        "Ang1(deg)_DSS": 29.4670125961,
-        "Ang1(deg)_EST": 30.0057,
+        "Ang1(deg)_DSS": 29.46660638,
+        "Ang1(deg)_EST": 29.9698,
         "Bus Nro.": 36,
-        "V1(pu)_DSS": 0.972799325,
-        "V1(pu)_EST": 0.975,
+        "V1(pu)_DSS": 0.9728065918,
+        "V1(pu)_EST": 0.9708,
         "bus_name": "729"
     },
     "4": {
-        "Ang1(deg)_DSS": 29.5780115065,
-        "Ang1(deg)_EST": 30.0002,
+        "Ang1(deg)_DSS": 29.577672449,
+        "Ang1(deg)_EST": 30.0005,
         "Bus Nro.": 5,
-        "V1(pu)_DSS": 0.9785743035,
-        "V1(pu)_EST": 0.9803,
+        "V1(pu)_DSS": 0.9785802031,
+        "V1(pu)_EST": 0.9795,
         "bus_name": "713"
     },
     "5": {
-        "Ang1(deg)_DSS": 29.4589464328,
-        "Ang1(deg)_EST": 30.0119,
+        "Ang1(deg)_DSS": 29.4585520586,
+        "Ang1(deg)_EST": 30.0172,
         "Bus Nro.": 6,
-        "V1(pu)_DSS": 0.9744329014,
-        "V1(pu)_EST": 0.9763,
+        "V1(pu)_DSS": 0.9744400821,
+        "V1(pu)_EST": 0.9756,
         "bus_name": "703"
     },
     "6": {
-        "Ang1(deg)_DSS": 29.4672816735,
-        "Ang1(deg)_EST": 29.9983,
+        "Ang1(deg)_DSS": 29.466879772,
+        "Ang1(deg)_EST": 29.986,
         "Bus Nro.": 7,
-        "V1(pu)_DSS": 0.9734960753,
-        "V1(pu)_EST": 0.9752,
+        "V1(pu)_DSS": 0.9735033024,
+        "V1(pu)_EST": 0.9728,
         "bus_name": "727"
     },
     "7": {
-        "Ang1(deg)_DSS": 29.4397850748,
-        "Ang1(deg)_EST": 29.995,
+        "Ang1(deg)_DSS": 29.4393149069,
+        "Ang1(deg)_EST": 29.9969,
         "Bus Nro.": 8,
-        "V1(pu)_DSS": 0.9699759611,
-        "V1(pu)_EST": 0.9689,
+        "V1(pu)_DSS": 0.9699838928,
+        "V1(pu)_EST": 0.9693,
         "bus_name": "730"
     },
     "8": {
-        "Ang1(deg)_DSS": 29.5693753371,
-        "Ang1(deg)_EST": 30.0008,
+        "Ang1(deg)_DSS": 29.5689951014,
+        "Ang1(deg)_EST": 30.0007,
         "Bus Nro.": 9,
-        "V1(pu)_DSS": 0.976556679,
-        "V1(pu)_EST": 0.9783,
+        "V1(pu)_DSS": 0.9765629813,
+        "V1(pu)_EST": 0.9775,
         "bus_name": "704"
     },
     "9": {
-        "Ang1(deg)_DSS": 29.5704533798,
-        "Ang1(deg)_EST": 30.0,
+        "Ang1(deg)_DSS": 29.570071682,
+        "Ang1(deg)_EST": 30.0001,
         "Bus Nro.": 10,
-        "V1(pu)_DSS": 0.9764114287,
-        "V1(pu)_EST": 0.9781,
+        "V1(pu)_DSS": 0.9764177384,
+        "V1(pu)_EST": 0.9773,
         "bus_name": "714"
     }
 }
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/Init_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Bus_i_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json` & `openpy_dsse-0.1.2/openpy_dsse/examples/4Node/MEAS_files/MEAS_Elem_ft_PMU.json`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/LICENSE.md` & `openpy_dsse-0.1.2/openpy_dsse/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/MEAS_from_OpenDSS.py` & `openpy_dsse-0.1.2/openpy_dsse/MEAS_from_OpenDSS.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/OpenDSS_data_extraction.py` & `openpy_dsse-0.1.2/openpy_dsse/OpenDSS_data_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 # @Time    : 03/03/2022
 # @Author  : Ing. Jorge Lara
 # @Email   : jlara@iee.unsj.edu.ar
 # @File    : ------------
 # @Software: PyCharm
 import logging
 
-import py_dss_interface
+
+#import py_dss_interface
 import numpy as np
 import pandas as pd
 import scipy as sp
 import math
 from typing import Dict, Tuple, List
 from .error_handling_logging import update_logg_file
+from .COM_interface import dss
 
 log_py = logging.getLogger(__name__)
-dss = py_dss_interface.DSSDLL()
+#dss = py_dss_interface.DSSDLL()
 
 class OpenDSS_data_collection:
     """
     Functions that allow bringing parameters and results from OpenDSS into DataFrame
     """
 
     def allbusnames_aux(self) -> pd.DataFrame:
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/Readme.md` & `openpy_dsse-0.1.2/openpy_dsse/Readme.md`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/Sample_test_systems_DSS.py` & `openpy_dsse-0.1.2/openpy_dsse/Sample_test_systems_DSS.py`

 * *Files identical despite different names*

### Comparing `openpy_dsse-0.1.1/openpy_dsse/state_estimation.py` & `openpy_dsse-0.1.2/openpy_dsse/state_estimation.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 # @Software: PyCharm
 
 from .base_DSSE import BaseAlgorithm
 from .Algorithm_classification import DSSE_algorithms
 from .Sample_test_systems_DSS import Sample_tests
 from .MEAS_from_OpenDSS import MEAS_files
 from .error_handling_logging import *
+from .Elec_param_calc_DSS_EST import estimated_electrical_variables
+from .perf_metrics_calc import performance_metrics
+from .Plot_results_DSS_EST import _Plot_results_DSS_EST
 import pandas as pd
 import logging
 
 log_py = logging.getLogger(__name__)
 
 class init_DSSE(BaseAlgorithm):
 
@@ -120,15 +123,15 @@
         """
         Function to perform circuit state estimation and obtain the estimated values of angle and voltage.
 
         :param summary:
         :param DSS_path: OpenDSS circuit file path. Default is None
         :param MEAS_path: Measurement file path. Default is None
         :param path_save: File path where the results will be saved. Default is None
-        :param Typ_cir:  Can be: '1ph' or 'Pos'. Default is None
+        :param Typ_cir: Can be: '1ph' or 'Pos'. Default is None
         :param ALG: For the moment it is node voltage. Default is 'NV'
         :param coord: For the moment are polar coordinates. Default is 'polar'
         :param method: can be: 'nonlinear', 'linear_PMU' and 'nonlinear_PMU'. Default is 'nonlinear_PMU'
         :param name_project: Name of the project to identify it in the files with results. Default is 'default'
         :param View_res: console display of the state estimator output
         :param summary: Prints by console the summary of the selected algorithm.
         :param DSS_coll: Save or print to console the power flow results along with the estimated status. Default is True
@@ -142,74 +145,142 @@
             self.Sbas3ph_MVA, self.tolerance, self.max_iter, self.init_values, DSS_path, MEAS_path, path_save, Typ_cir,
             ALG, coord, method, name_project, MEAS_Pos, DSS_coll, View_res, summary)
 
         V_Ang_EST = Sel_Alg.addresses_algorithm()
 
         return V_Ang_EST
 
-    def calc_from_est(
+    def param_elect_from_EST(
             self,
             DSS_path: str = None,
-            EST_pd: pd.DataFrame = None,
+            EST_df: pd.DataFrame = None,
             EST_path: str = None,
             I_Ang_EST: bool = False,
             PQi_EST: bool = False,
             PQf_EST: bool = False,
-            no_PU: bool = False
+            no_PU: bool = False,
+            path_save: str = None,
+            View_res: bool = True,
+            DSS_col: bool = True,
+            name_project: str = 'Default'
     ):
         """
         From the estimated status result, other electrical parameters are calculated and can be compared with the OpenDSS results.
 
         :param EST_path:
-        :param EST_pd:
+        :param EST_df:
         :param I_Ang_EST: With estimated voltage and angle, calculate the current between two nodes. Default is 'False'
         :param PQi_EST: With estimated voltage and angle, calculate the node injection power. Default is 'False'
         :param PQf_EST: With estimated voltage and angle, calculate the power flow between two nodes. Default is 'False'
         :param no_PU: Displays results in real values (not per Unit). Default is 'False'
         :param DSS_path:
         :return:
         """
-        print('In development')
+        calc_from_est_EH(DSS_path, EST_df, EST_path, I_Ang_EST, PQi_EST, PQf_EST, no_PU)
+        calc_parameters = estimated_electrical_variables(
+            I_Ang_EST=I_Ang_EST,
+            PQi_EST=PQi_EST,
+            PQf_EST=PQf_EST
+        )
+        if I_Ang_EST:
+            df_Imag_Ang_EST = calc_parameters.Imang_Angle_EST_1ph(
+                df_Results_DSSE=EST_df,
+                SbasMVA_3ph=self.Sbas3ph_MVA,
+                path_save=path_save,
+                View_res=View_res,
+                DSS_col=DSS_col,
+                name_project=name_project
+            )
+            return df_Imag_Ang_EST
 
-    def calc_performance(
+    def performance_metrics(
             self,
-            DSS_path: str = None,
-            EST_pd: pd.DataFrame = None,
-            EST_path: str = None,
-            MAPE: bool = False,
-            MAE: bool = False,
-            RMSE: bool = False
+            V_Bus: dict = None,
+            I_Elem: dict = None,
+            MAPE: bool = True,
+            MAE: bool = True,
+            RMSE: bool = True,
+            path_save: str = None,
+            View_res: bool = False,
+            name_project: str = 'Default'
     ):
         """
         Function to calculate the performance metrics as Mean Absolute Percentage Error (MAPE), Mean Absolute Error (MAE), and Root Mean Square Error (RMSE).
 
         :param MAPE: Calculate the Mean Absolute Percentage Error (MAPE). Default is 'False'
         :param MAE: Calculate the Mean Absolute Error (MAE). Default is 'False'
         :param RMSE: Calculate the Root Mean Square Error (RMSE). Default is 'False'
         :param DSS_path: OpenDSS circuit file path
         :return:
         """
-        print('In development')
+        if V_Bus is not None:
+            V_Bus_DSS_EST = pd.merge(
+                V_Bus['df_DSS'], V_Bus['df_EST'],
+                on=('bus_name', 'Bus Nro.')
+            )
+        if I_Elem is not None:
+            I_Elem_DSS_EST = pd.merge(
+                I_Elem['df_DSS'], I_Elem['df_EST'],
+                on=('element_name', 'from_bus', 'to_bus')
+            )
+        perf = performance_metrics(
+            V_Bus=V_Bus_DSS_EST,
+            I_Elem=I_Elem_DSS_EST,
+        )
+        perf_dict = dict()
+        if MAE:
+            perf_dict['MAE'] = perf.Mean_Absolute_Error()
+        if MAPE:
+            perf_dict['MAPE'] = perf.Mean_Absolute_Percentage_Error()
+        if RMSE:
+            perf_dict['RMSE'] = perf.Root_Mean_Square_Error()
 
-    def plot_results(
+        return perf._dict_merge(MAE, MAPE, RMSE, perf_dict, View_res, path_save, name_project)
+    def Plot_results(
             self,
-            I_Ang_EST: bool = False,
-            PQi_EST: bool = False,
-            PQf_EST: bool = False,
+            V_Bus: dict = None,
+            I_Elem: dict = None,
+            View: bool = True,
             no_PU: bool = False,
-            MAPE: bool = False,
-            MAE: bool = False,
-            RMSE: bool = False
+            path_save: str = None,
+            name_project: str = 'Default'
     ):
         """
 
         :param I_Ang_EST: With estimated voltage and angle, calculate the current between two nodes. Default is 'False'
         :param PQi_EST:
         :param PQf_EST:
         :param no_PU: Displays results in real values (not per Unit). Default is 'False'
         :param MAPE:
         :param MAE:
         :param RMSE:
         :return:
         """
-        print('In development')
+        res_plt = _Plot_results_DSS_EST(
+            name_project,
+            path_save,
+            no_PU,
+            View
+        )
+        if V_Bus is not None:
+            V_Bus_DSS_EST = pd.merge(
+                V_Bus['df_DSS'],
+                V_Bus['df_EST'],
+                on=('bus_name', 'Bus Nro.')
+            )
+            res_plt._Vi_Angi_1ph_Pos(
+                V_Bus_DSS_EST
+            )
+
+        if I_Elem is not None:
+            I_Elem_DSS_EST = pd.merge(
+                I_Elem['df_DSS'],
+                I_Elem['df_EST'],
+                on=('element_name', 'from_bus', 'to_bus')
+            )
+            res_plt._Iij_Angij_1ph_Pos(
+                I_Elem_DSS_EST
+            )
+
+
+
```

### Comparing `openpy_dsse-0.1.1/openpy_dsse/YBus_Matrix_Pos_Seq.py` & `openpy_dsse-0.1.2/openpy_dsse/YBus_Matrix_Pos_Seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 #dss = py_dss_interface.DSSDLL()
 
 class YBus_Matrix_SeqPos_OpenDSS:
 
     def __init__(self, DF_allbusnames_aux: pd.DataFrame):
         self.DF_allbusnames_aux = DF_allbusnames_aux
 
-    def build_YBus_Matrix_Pos_Seq(self, element: List[str]) -> np.array:
+    def build_YBus_Matrix_Pos_Seq(
+            self,
+            element: List[str]
+    ) -> np.array:
 
         nbus = dss.circuit_num_buses()
         Y_Bus = np.zeros((nbus, nbus), dtype=complex)
         DF = self.DF_allbusnames_aux
 
         for ii in element:
             if ii == 'vsources':
```

### Comparing `openpy_dsse-0.1.1/pyproject.toml` & `openpy_dsse-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openpy-dsse"
-version = "0.1.1"
+version = "0.1.2"
 description = "Open source library for state estimation of a distribution network modeled in OpenDSS"
 authors = ["Jorge Lara <jlara@iee.unsj.edu.ar>"]
 license = "LICENSE"
 readme = "README.md"
 keywords = ["OpenDSS", "DSSE", "state estimation", "smart grid", "OpenPy-DSSE", "OpenPy_DSSE"]
 
 packages = [{include = "openpy_dsse"}]
```

### Comparing `openpy_dsse-0.1.1/README.md` & `openpy_dsse-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,33 @@
-# openpy_dsse
+# OpenPY_DSSE
 
-It is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks (OpenDSS) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.
+It is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks ([OpenDSS](https://sourceforge.net/projects/electricdss/)) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.
 
-It is developed within the framework of the OpenREiD project (Integral software for simulation and optimization of electrical distribution networks), of the Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina.
+It is developed within the framework of the[ OpenREiD](https://iee-unsjconicet.org/reid/) project (Integral software for simulation and optimization of electrical distribution networks), of the [Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina](https://iee-unsjconicet.org/).
 
 **Index**
 
+- [Weighted Least Squares](#id0)
 - [Installation](#id1)
 - [How to use](#id2)
   - [Measurements](#id3)
     - [Definition and creation of meters](#id4)
     - [Generate metrics from OpenDSS results](#id5)
   - [Run the state estimation algorithm](#id6)
   - [Sample tests](#id7)
 - [License](#id8)
 
+<div id='id0' />
+
+## Weighted Least Squares (WLS)
+
+The library uses a hybrid weighted least squares algorithm that incorporates traditional and D-PMU measurements. It supports single-phase and multiphase networks that are modeled as electromagnetically decoupled positive sequence impedances. More details can be found in [docs/methodology](https://github.com/jlara6/OpenPy-DSSE/blob/main/docs/methodology/Nonlinear_Hybrid_State_Estimator.ipynb)
+
 <div id='id1' />
+
 ## Installation
 
 With pip
 
 ``pip install py-open-dsse``
 
 Without pip, clone or download the repository, in the dist folder is the .whl file, copy the location of the file, and in the CMD:
@@ -189,17 +197,17 @@
 
 In the path ``:{Python_library_path}/openpy_dsse/examples``, the ``.DSS`` and ``.json`` files of single-phase (``1ph``) and positive sequence equivalent (``Pos``) circuit measurements detailed in Table 11 are located.
 
 **Table 11.** Sample tests
 | **Circuit** | **Tpy_circ** | **Case** |
 |:------------:|:------------:|:--------:|
 |     4Node    |      1ph     |     1    |
-|  15NodeIEEE  |      1ph     |     2    |
-|  13NodeIEEE  |      Pos     |     1    |
-|  37NodeIEEE  |      Pos     |     2    |
+|  [15NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/15NodeIEEE/15NodeIEEE.ipynb)  |      1ph     |     2    |
+|  [13NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/13NodeIEEE/13NodeIEEE.ipynb)  |      Pos     |     1    |
+|  [37NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/37NodeIEEE/37NodeIEEE.ipynb)  |      Pos     |     2    |
 
 The function ``test_circuit(Typ_cir, case)``, returns a dictionary with the keys ``'DSS_file'``, ``'MEAS_path'``, ``'save_path'``, ``'name_project'`` and ``'Typ_cir'`` which correspond to the ``.DSS`` file path, measurement file path, path where results will be saved and circuit type respectively.
 ```Python
 import openpy_dsse
 
 dsse = openpy_dsse.init_DSSE() #Start the class.
```

### Comparing `openpy_dsse-0.1.1/setup.py` & `openpy_dsse-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 packages = \
 ['openpy_dsse',
  'openpy_dsse.DSSE_algorithms',
  'openpy_dsse.DSSE_algorithms.Symb_Eqn']
 
 package_data = \
 {'': ['*'],
- 'openpy_dsse': ['examples/13NodeIEEE/*',
-                 'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
+ 'openpy_dsse': ['examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/13NodeIEEE/MEAS_files/Init_Bus_i.json',
@@ -151,16 +150,39 @@
                  'examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/13NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/13NodeIEEE/OpenDSS files/*',
                  'examples/13NodeIEEE/OpenDSS files/PosSeq circuit/*',
+                 'examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Iij_DSS_EST_no_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Metrics_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json',
                  'examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json',
-                 'examples/15NodeIEEE/*',
+                 'examples/13NodeIEEE/Results/Results_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Results_I_Ang_from_DSSE_13NodeIEEE.json',
+                 'examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png',
+                 'examples/13NodeIEEE/Results/Vi_DSS_EST_PU_13NodeIEEE.png',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/15NodeIEEE/MEAS_files/Init_Bus_i.json',
@@ -218,16 +240,39 @@
                  'examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json',
                  'examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json',
                  'examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json',
                  'examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json',
                  'examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json',
                  'examples/15NodeIEEE/MEAS_files/MEAS_Elem_ft_PMU.json',
                  'examples/15NodeIEEE/OpenDSS files/*',
+                 'examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Iij_DSS_EST_no_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Metrics_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json',
                  'examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json',
-                 'examples/37NodeIEEE/*',
+                 'examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Results_I_Ang_from_DSSE_15NodeIEEE.json',
+                 'examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png',
+                 'examples/15NodeIEEE/Results/Vi_DSS_EST_PU_15NodeIEEE.png',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
                  'examples/37NodeIEEE/MEAS_files/Init_Bus_i.json',
@@ -366,18 +411,66 @@
                  'examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/37NodeIEEE/MEAS_files/Pos_MEAS_Elem_ft_PMU.json',
                  'examples/37NodeIEEE/OpenDSS files/*',
                  'examples/37NodeIEEE/OpenDSS files/PosSeq circuit/*',
+                 'examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Iij_DSS_EST_no_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Metrics_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json',
                  'examples/37NodeIEEE/Results/Results_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Results_I_Ang_from_DSSE_37nodeIEEE.json',
+                 'examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png',
+                 'examples/37NodeIEEE/Results/Vi_DSS_EST_PU_37nodeIEEE.png',
                  'examples/4Node/MEAS_files/*',
                  'examples/4Node/OpenDSS files/*',
-                 'examples/4Node/Results/Results_DSSE_4Node.json']}
+                 'examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png',
+                 'examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png',
+                 'examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png',
+                 'examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png',
+                 'examples/4Node/Results/Iij_DSS_EST_no_PU_4Node.png',
+                 'examples/4Node/Results/Metrics_4Node.json',
+                 'examples/4Node/Results/Metrics_4Node.json',
+                 'examples/4Node/Results/Metrics_4Node.json',
+                 'examples/4Node/Results/Metrics_4Node.json',
+                 'examples/4Node/Results/Metrics_4Node.json',
+                 'examples/4Node/Results/Results_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json',
+                 'examples/4Node/Results/Results_I_Ang_from_DSSE_4Node.json',
+                 'examples/4Node/Results/Vi_DSS_EST_PU_4Node.png',
+                 'examples/4Node/Results/Vi_DSS_EST_PU_4Node.png',
+                 'examples/4Node/Results/Vi_DSS_EST_PU_4Node.png',
+                 'examples/4Node/Results/Vi_DSS_EST_PU_4Node.png',
+                 'examples/4Node/Results/Vi_DSS_EST_PU_4Node.png']}
 
 install_requires = \
 ['colorama==0.4.6',
  'contourpy==1.0.5',
  'cycler==0.11.0',
  'et-xmlfile==1.1.0',
  'fonttools==4.38.0',
@@ -396,17 +489,17 @@
  'scipy==1.9.3',
  'seaborn==0.12.1',
  'six==1.16.0',
  'sympy==1.11.1']
 
 setup_kwargs = {
     'name': 'openpy-dsse',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Open source library for state estimation of a distribution network modeled in OpenDSS',
-    'long_description': '# openpy_dsse\n\nIt is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks (OpenDSS) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.\n\nIt is developed within the framework of the OpenREiD project (Integral software for simulation and optimization of electrical distribution networks), of the Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina.\n\n**Index**\n\n- [Installation](#id1)\n- [How to use](#id2)\n  - [Measurements](#id3)\n    - [Definition and creation of meters](#id4)\n    - [Generate metrics from OpenDSS results](#id5)\n  - [Run the state estimation algorithm](#id6)\n  - [Sample tests](#id7)\n- [License](#id8)\n\n<div id=\'id1\' />\n## Installation\n\nWith pip\n\n``pip install py-open-dsse``\n\nWithout pip, clone or download the repository, in the dist folder is the .whl file, copy the location of the file, and in the CMD:\n\n``pip install {path-save-files}/openpy_dsse-{version}-py3-none-any.whl’``\n\n<div id=\'id2\'/>\n\n## How to use  <a name="id1"></a>\n\nFirst, in the IDE (Integrated Development Environment) of preference, we import the library:\n\n```Python\nimport openpy_dsse\n```\n\nThe object class that contains all the functions of the library is activated as follows:\n\n```Python\ndsse = openpy_dsse.init_DSSE()\n```\n\nThe class ``init_DSSE()``, has default values as shown in table 1 and can be modified as appropriate.\n\n**Table 1.** Description and attributes of function ``init_DSSE()``\n| **Parameters** | **Description** | **Default value** |\n|:---:|---|:---:|\n| ``Sbas3ph_MVA`` | Three-phase system base power     | ``30`` |\n| ``tolerance`` | Convergence tolerance of selected algorithm | ``1e-3`` |\n| ``max_iter`` | Maximum number of iterations of the selected algorithm | ``30`` |\n| ``init_values`` | Initial values for state estimation. With ``flat`` start with 1.0 p.u. / 0° on all buses and with ``dss`` start with OpenDSS voltage and angle results| ``flat`` |\n\nOnce the class is initialized, we can use the functions described below.\n\n<div id=\'id3\' />\n\n### Measurements\n\n<div id=\'id4\' />\n\n#### Definition and creation of meters\n\nThe library supports meters and their respective error variance described in Table 2.\n\n**Table 2.** Measurement type of the ``openpy_dsse`` library.\n\n|              **Meter**                 |                                **Description**                |\n|:--------------------------------------:|---------------------------------------------------------------|\n| $\\left\\|V_{i}\\right\\|$                 | Node voltage magnitude.                                       |\n| $PQ_{ft}$                              | Branch power flow                                             |\n| $\\left\\|I_{ft}\\right\\|$                | Magnitude of branch current.                                  |\n| $PQ_{i}^{SM}$                          | Injection power or node consumption obtained by a smart meter |\n| $PQ_{i}^{0}$                           | Passive node or zero injection power.                         |\n| $PQ_{i}^{PSD}$                         | Artificial node injection power known as pseudo-measurement   |\n| $\\left\\|V_{i}\\right\\|\\angle \\theta$    | Voltage phasor measurement                                    |\n| $\\left\\|I_{ft}\\right\\|\\angle \\delta$   | Current phasor measurement                                              |\n\nThe measurement data per phase **𝜌 (1, 2, 3)** and measurement error variance ``Rii`` of a network modeled in OpenDSS. They must be entered in the ``MEAS_Bus_i.json``, ``MEAS_Elem_ft.json``, ``MEAS_Bus_i_PMU.json`` and ``MEAS_Elem_ft_PMU.json`` files. The ``.json`` measurement files without data are generated with the ``empty_MEAS_files()`` function and the parameters from table 3 must be entered.\n\n**Table 3.** Parameters and description of ``empty_file_MEAS()`` function\n|    **Parameter**   |                           **Description**                         |**Default value** |\n|:------------------:|-------------------------------------------------------------------|:----------------:|\n| ``DSS_path``       | A path of the ``.DSS`` files of the circuit modeled in OpenDSS    | ``None ``        |\n| ``MEAS_path_save`` | Path where the measurement ``.json`` files will be saved          | ``None ``        |\n\nThe description of the identifiers that can be modified is detailed in tables 4, 5, 6, and 7. The other identifiers in the ``.json`` files, are node characteristics or elements extracted from the circuit modeled in OpenDSS, these data should not be modified since they would affect the result of the state estimation algorithm.\n\n**Table 4.** Description of identifiers of the ``MEAS_Bus_i.json`` file.\n\n| **Identifier**     |                                       **Description**                         |\n|:---------------------:|-------------------------------------------------------------------------------|\n| ``STS_Vm``            | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_Vm``            | Variance of voltage magnitude measurement error.                              |\n| ``Vρm(pu)``           | Measurement of voltage magnitude voltage in phase 𝜌.                          |\n| ``STS_PQd(SM)``       | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_SM``            | Measurement error variance of injection power or consumption of a smart meter.|\n| ``STS_PQd(0)``        | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_0``             | Zero or passive injection power measurement error variance.                   |\n| ``STS_PQd(Psd)``      | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_Psd``           | Measurement error variance of pseudo power injection measurement              |\n| ``Pρmd(pu)``          | Measurement of active power injection in phase 𝜌.                             |\n| ``Qρmd(pu)``          | Measurement of reactive power injection in phase 𝜌.                           |\n\n**Table 5.** Description of identifiers of the ``MEAS_Elem_ft.json`` file.\n\n| **Identifier**        | **Description**                                    |\n|:---------------------:|----------------------------------------------------|\n| ``STS_PQft``          | Status (1: Enabled, 0: Disabled)                   |\n| ``Rii_PQft``          | Branch power flow measurement error variance.      |\n| ``Pρmft(pu)``         | Measurement of branch active power in phase 𝜌.     |\n| ``Qρmft(pu)``         | Measurement of branch reactive power in phase 𝜌.   |\n| ``STS_Ift``           | Status (1: Enabled, 0: Disabled)                   |\n| ``Rii_Ift``           | Branch current magnitude error variance.           |\n| ``Iρmft(pu)``         | Measurement of branch current magnitude in phase 𝜌.|\n\n**Table 6.** Description of identifiers of the ``MEAS_Elem_ft_PMU.json`` file.\n| **Identifier**     |                   **Description**           |\n|:---------------------:|---------------------------------------------|\n| ``STS_Vm``            | Status (1: Enabled, 0: Disabled)            |\n| ``Rii_Vm``            | Variance of voltage phasor measurement error|\n| ``Vρm(pu)``           | Measurement of voltage magnitude in phase 𝜌 |\n| ``Angρm(deg)``        | Measurement of volage angle in phase 𝜌      |\n\n**Table 7.** Description of identifiers of the ``MEAS_Elem_ft_PMU.json`` file.\n| **Identifier**    |                 **Description**             |\n|:-----------------:|---------------------------------------------|\n| ``STS_Ift``       | Status (1: Enabled, 0: Disabled)            |\n| ``Rii_Ift``       | Variance of current phasor measurement error|\n| ``Iρmft(pu)``     | Measurement of current magnitude in phase 𝜌 |\n| ``Angρm(deg)``    | Measurement of current angle in phase 𝜌     |\n\n<div id=\'id5\' />\n\n#### Generate metrics from OpenDSS results\n\n##### Initial measurements with uncertainty of measurement error\n\nThe ``empty_init_files_MEAS_Unc()`` function generates ``.json`` files where all the nodes and elements that can participate as measurement in the state estimation algorithm are placed. For this purpose, the parameters of table 8 must be specified.\n\n**Table 8.** Parameters and description of ``empty_file_MEAS()`` function\n|    **Parameters**   |                           **Description**                     | **Default value** |\n|:------------------:|----------------------------------------------------------------|:-----------------:|\n| ``DSS_path``       | A path of the ``.DSS`` files of the circuit modeled in OpenDSS | ``None``          |\n| ``MEAS_path_save`` | Path where the measurement ``.json`` files will be saved       | ``None``          |\n\nIn the ``MEAS_path_save`` path, it generates the files ``Init_Bus_i.json``, ``Init_Elem_ft.json``, ``Init_Bus_i_PMU.json`` and ``Init_Elem_ft_PMU.json``. Depending on the case study, the ``STS`` meter status (1: Enabled, 0: Disabled) and the measurement error rate in ``Unc(%)`` can be modified.\n\n##### Adding random errors and generating measurement files\n\nWith the ``.json`` files generated by the ``empty_file_MEAS()`` function and the changes indicated by the user, with the ``add_error_file_MEAS()`` function and the Parameters described in Table 9.\n\n**Table 9.** Description and attributes of function ``add_error_files_MEAS()``\n| **Parameters** |                        **Description**                        | **Default value**|\n|:--------------:|---------------------------------------------------------------|:----------------:|\n| ``DSS_path``   | A path of the ``.DSS`` files of the circuit modeled in OpenDSS| ``None``         |\n| ``MEAS_path``  | Path of initial ``.json`` files                               | ``None``         |\n| ``seed_DS``    | Random error generation seed                                  | ``1``            |\n\nAdds random errors from a normal distribution to the OpenDSS power flow results, for use as a measurement. The result of generating random errors is contained in the files ``MEAS_Bus_i.json``, ``MEAS_Elem_ft.json``, ``MEAS_Bus_i_PMU.json`` and ``MEAS_Elem_ft_PMU.json``, stored in ``MEAS_path``.\n\n<div id=\'id6\' />\n\n### Run the state estimation algorithm\n\nTo run the state estimation algorithm, function ``estimate()`` is called, it is necessary to enter or change parameters detailed in table 10. \n\n**Table 10.** Parameters and description of ``estimate()`` function\n\n|   **Parameters** |                                   **Description**                                  | **Default value** |\n|:----------------:|------------------------------------------------------------------------------------|:---------------------:|\n| ``DSS_path``     | A path of the ``.DSS`` files of the circuit modeled in OpenDSS.                    | ``None``              |\n| ``MEAS_path``    | Path where measurement files are located.                                          | ``None``              |\n| ``path_save``    | Path where the results will be saved                                               | ``None``              |\n| ``Typ_cir``      | Circuit type, can be ``1ph`` or ``Pos``.                                           | ``None``              |\n| ``ALG``          | Type of algorithm state variables. At the moment ``NV``                            | ``NV``                |\n| ``coord``        | Type of coordinates to solve. For the moment ``polar``.                            | ``Polar``             |\n| ``method``       | Solution method, can be ``nonlinear``, ``linear_PMU`` and ``nonlinear_PMU``.| ``nonlinear_PMU``|\n| ``name_project`` | Project name                                                                       | ``Default``           |\n| ``View_res``     | Displays the result of the selected algorithm by console                           | ``False``             |\n| ``DSS_coll``     | Displays next to the estimated status, the actual status according to OpenDSS      | ``False``             |\n| ``summary``      | Displays a summary of the simulation by console                                    | ``False``             |\n| ``MEAS_Pos``     | ``True`` if it is a ``Pos`` circuit, take the ``.json`` files in positive sequence.| ``False``             |\n\n<div id=\'id7\' />\n\n## Sample tests\n\nIn the path ``:{Python_library_path}/openpy_dsse/examples``, the ``.DSS`` and ``.json`` files of single-phase (``1ph``) and positive sequence equivalent (``Pos``) circuit measurements detailed in Table 11 are located.\n\n**Table 11.** Sample tests\n| **Circuit** | **Tpy_circ** | **Case** |\n|:------------:|:------------:|:--------:|\n|     4Node    |      1ph     |     1    |\n|  15NodeIEEE  |      1ph     |     2    |\n|  13NodeIEEE  |      Pos     |     1    |\n|  37NodeIEEE  |      Pos     |     2    |\n\nThe function ``test_circuit(Typ_cir, case)``, returns a dictionary with the keys ``\'DSS_file\'``, ``\'MEAS_path\'``, ``\'save_path\'``, ``\'name_project\'`` and ``\'Typ_cir\'`` which correspond to the ``.DSS`` file path, measurement file path, path where results will be saved and circuit type respectively.\n```Python\nimport openpy_dsse\n\ndsse = openpy_dsse.init_DSSE() #Start the class.\n\nif __name__ == \'__main__\':\n    net = dsse.test_circuit(Typ_cir=\'1ph\', case=1)\n    \n    #dsse.empty_init_files_MEAS_Unc(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n    #dsse.add_error_files_MEAS(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n    #dsse.empty_MEAS_files(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n\n    #execute the state estimation algorithm\n    Results = dsse.estimate(\n        DSS_path=net[\'DSS_file\'],\n        MEAS_path=net[\'MEAS_path\'],\n        path_save=net[\'save_path\'],\n        Typ_cir=net[\'Typ_cir\'],\n        name_project=net[\'name_project\'],\n        View_res=True,\n        summary=True,\n        DSS_coll=True,\n        #MEAS_Pos=True,\n        #method=\'nonlinear\'\n        #method=\'linear_PMU\',\n    )\n```\n\n<div id=\'id8\' />\n\n### License\n\nLicense: CC BY-NC-SA 4.0\n\n<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />\n\nThis work has a license <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.\n',
+    'long_description': '# OpenPY_DSSE\n\nIt is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks ([OpenDSS](https://sourceforge.net/projects/electricdss/)) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.\n\nIt is developed within the framework of the[ OpenREiD](https://iee-unsjconicet.org/reid/) project (Integral software for simulation and optimization of electrical distribution networks), of the [Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina](https://iee-unsjconicet.org/).\n\n**Index**\n\n- [Weighted Least Squares](#id0)\n- [Installation](#id1)\n- [How to use](#id2)\n  - [Measurements](#id3)\n    - [Definition and creation of meters](#id4)\n    - [Generate metrics from OpenDSS results](#id5)\n  - [Run the state estimation algorithm](#id6)\n  - [Sample tests](#id7)\n- [License](#id8)\n\n<div id=\'id0\' />\n\n## Weighted Least Squares (WLS)\n\nThe library uses a hybrid weighted least squares algorithm that incorporates traditional and D-PMU measurements. It supports single-phase and multiphase networks that are modeled as electromagnetically decoupled positive sequence impedances. More details can be found in [docs/methodology](https://github.com/jlara6/OpenPy-DSSE/blob/main/docs/methodology/Nonlinear_Hybrid_State_Estimator.ipynb)\n\n<div id=\'id1\' />\n\n## Installation\n\nWith pip\n\n``pip install py-open-dsse``\n\nWithout pip, clone or download the repository, in the dist folder is the .whl file, copy the location of the file, and in the CMD:\n\n``pip install {path-save-files}/openpy_dsse-{version}-py3-none-any.whl’``\n\n<div id=\'id2\'/>\n\n## How to use  <a name="id1"></a>\n\nFirst, in the IDE (Integrated Development Environment) of preference, we import the library:\n\n```Python\nimport openpy_dsse\n```\n\nThe object class that contains all the functions of the library is activated as follows:\n\n```Python\ndsse = openpy_dsse.init_DSSE()\n```\n\nThe class ``init_DSSE()``, has default values as shown in table 1 and can be modified as appropriate.\n\n**Table 1.** Description and attributes of function ``init_DSSE()``\n| **Parameters** | **Description** | **Default value** |\n|:---:|---|:---:|\n| ``Sbas3ph_MVA`` | Three-phase system base power     | ``30`` |\n| ``tolerance`` | Convergence tolerance of selected algorithm | ``1e-3`` |\n| ``max_iter`` | Maximum number of iterations of the selected algorithm | ``30`` |\n| ``init_values`` | Initial values for state estimation. With ``flat`` start with 1.0 p.u. / 0° on all buses and with ``dss`` start with OpenDSS voltage and angle results| ``flat`` |\n\nOnce the class is initialized, we can use the functions described below.\n\n<div id=\'id3\' />\n\n### Measurements\n\n<div id=\'id4\' />\n\n#### Definition and creation of meters\n\nThe library supports meters and their respective error variance described in Table 2.\n\n**Table 2.** Measurement type of the ``openpy_dsse`` library.\n\n|              **Meter**                 |                                **Description**                |\n|:--------------------------------------:|---------------------------------------------------------------|\n| $\\left\\|V_{i}\\right\\|$                 | Node voltage magnitude.                                       |\n| $PQ_{ft}$                              | Branch power flow                                             |\n| $\\left\\|I_{ft}\\right\\|$                | Magnitude of branch current.                                  |\n| $PQ_{i}^{SM}$                          | Injection power or node consumption obtained by a smart meter |\n| $PQ_{i}^{0}$                           | Passive node or zero injection power.                         |\n| $PQ_{i}^{PSD}$                         | Artificial node injection power known as pseudo-measurement   |\n| $\\left\\|V_{i}\\right\\|\\angle \\theta$    | Voltage phasor measurement                                    |\n| $\\left\\|I_{ft}\\right\\|\\angle \\delta$   | Current phasor measurement                                              |\n\nThe measurement data per phase **𝜌 (1, 2, 3)** and measurement error variance ``Rii`` of a network modeled in OpenDSS. They must be entered in the ``MEAS_Bus_i.json``, ``MEAS_Elem_ft.json``, ``MEAS_Bus_i_PMU.json`` and ``MEAS_Elem_ft_PMU.json`` files. The ``.json`` measurement files without data are generated with the ``empty_MEAS_files()`` function and the parameters from table 3 must be entered.\n\n**Table 3.** Parameters and description of ``empty_file_MEAS()`` function\n|    **Parameter**   |                           **Description**                         |**Default value** |\n|:------------------:|-------------------------------------------------------------------|:----------------:|\n| ``DSS_path``       | A path of the ``.DSS`` files of the circuit modeled in OpenDSS    | ``None ``        |\n| ``MEAS_path_save`` | Path where the measurement ``.json`` files will be saved          | ``None ``        |\n\nThe description of the identifiers that can be modified is detailed in tables 4, 5, 6, and 7. The other identifiers in the ``.json`` files, are node characteristics or elements extracted from the circuit modeled in OpenDSS, these data should not be modified since they would affect the result of the state estimation algorithm.\n\n**Table 4.** Description of identifiers of the ``MEAS_Bus_i.json`` file.\n\n| **Identifier**     |                                       **Description**                         |\n|:---------------------:|-------------------------------------------------------------------------------|\n| ``STS_Vm``            | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_Vm``            | Variance of voltage magnitude measurement error.                              |\n| ``Vρm(pu)``           | Measurement of voltage magnitude voltage in phase 𝜌.                          |\n| ``STS_PQd(SM)``       | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_SM``            | Measurement error variance of injection power or consumption of a smart meter.|\n| ``STS_PQd(0)``        | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_0``             | Zero or passive injection power measurement error variance.                   |\n| ``STS_PQd(Psd)``      | Status (1: Enabled, 0: Disabled)                                              |\n| ``Rii_Psd``           | Measurement error variance of pseudo power injection measurement              |\n| ``Pρmd(pu)``          | Measurement of active power injection in phase 𝜌.                             |\n| ``Qρmd(pu)``          | Measurement of reactive power injection in phase 𝜌.                           |\n\n**Table 5.** Description of identifiers of the ``MEAS_Elem_ft.json`` file.\n\n| **Identifier**        | **Description**                                    |\n|:---------------------:|----------------------------------------------------|\n| ``STS_PQft``          | Status (1: Enabled, 0: Disabled)                   |\n| ``Rii_PQft``          | Branch power flow measurement error variance.      |\n| ``Pρmft(pu)``         | Measurement of branch active power in phase 𝜌.     |\n| ``Qρmft(pu)``         | Measurement of branch reactive power in phase 𝜌.   |\n| ``STS_Ift``           | Status (1: Enabled, 0: Disabled)                   |\n| ``Rii_Ift``           | Branch current magnitude error variance.           |\n| ``Iρmft(pu)``         | Measurement of branch current magnitude in phase 𝜌.|\n\n**Table 6.** Description of identifiers of the ``MEAS_Elem_ft_PMU.json`` file.\n| **Identifier**     |                   **Description**           |\n|:---------------------:|---------------------------------------------|\n| ``STS_Vm``            | Status (1: Enabled, 0: Disabled)            |\n| ``Rii_Vm``            | Variance of voltage phasor measurement error|\n| ``Vρm(pu)``           | Measurement of voltage magnitude in phase 𝜌 |\n| ``Angρm(deg)``        | Measurement of volage angle in phase 𝜌      |\n\n**Table 7.** Description of identifiers of the ``MEAS_Elem_ft_PMU.json`` file.\n| **Identifier**    |                 **Description**             |\n|:-----------------:|---------------------------------------------|\n| ``STS_Ift``       | Status (1: Enabled, 0: Disabled)            |\n| ``Rii_Ift``       | Variance of current phasor measurement error|\n| ``Iρmft(pu)``     | Measurement of current magnitude in phase 𝜌 |\n| ``Angρm(deg)``    | Measurement of current angle in phase 𝜌     |\n\n<div id=\'id5\' />\n\n#### Generate metrics from OpenDSS results\n\n##### Initial measurements with uncertainty of measurement error\n\nThe ``empty_init_files_MEAS_Unc()`` function generates ``.json`` files where all the nodes and elements that can participate as measurement in the state estimation algorithm are placed. For this purpose, the parameters of table 8 must be specified.\n\n**Table 8.** Parameters and description of ``empty_file_MEAS()`` function\n|    **Parameters**   |                           **Description**                     | **Default value** |\n|:------------------:|----------------------------------------------------------------|:-----------------:|\n| ``DSS_path``       | A path of the ``.DSS`` files of the circuit modeled in OpenDSS | ``None``          |\n| ``MEAS_path_save`` | Path where the measurement ``.json`` files will be saved       | ``None``          |\n\nIn the ``MEAS_path_save`` path, it generates the files ``Init_Bus_i.json``, ``Init_Elem_ft.json``, ``Init_Bus_i_PMU.json`` and ``Init_Elem_ft_PMU.json``. Depending on the case study, the ``STS`` meter status (1: Enabled, 0: Disabled) and the measurement error rate in ``Unc(%)`` can be modified.\n\n##### Adding random errors and generating measurement files\n\nWith the ``.json`` files generated by the ``empty_file_MEAS()`` function and the changes indicated by the user, with the ``add_error_file_MEAS()`` function and the Parameters described in Table 9.\n\n**Table 9.** Description and attributes of function ``add_error_files_MEAS()``\n| **Parameters** |                        **Description**                        | **Default value**|\n|:--------------:|---------------------------------------------------------------|:----------------:|\n| ``DSS_path``   | A path of the ``.DSS`` files of the circuit modeled in OpenDSS| ``None``         |\n| ``MEAS_path``  | Path of initial ``.json`` files                               | ``None``         |\n| ``seed_DS``    | Random error generation seed                                  | ``1``            |\n\nAdds random errors from a normal distribution to the OpenDSS power flow results, for use as a measurement. The result of generating random errors is contained in the files ``MEAS_Bus_i.json``, ``MEAS_Elem_ft.json``, ``MEAS_Bus_i_PMU.json`` and ``MEAS_Elem_ft_PMU.json``, stored in ``MEAS_path``.\n\n<div id=\'id6\' />\n\n### Run the state estimation algorithm\n\nTo run the state estimation algorithm, function ``estimate()`` is called, it is necessary to enter or change parameters detailed in table 10. \n\n**Table 10.** Parameters and description of ``estimate()`` function\n\n|   **Parameters** |                                   **Description**                                  | **Default value** |\n|:----------------:|------------------------------------------------------------------------------------|:---------------------:|\n| ``DSS_path``     | A path of the ``.DSS`` files of the circuit modeled in OpenDSS.                    | ``None``              |\n| ``MEAS_path``    | Path where measurement files are located.                                          | ``None``              |\n| ``path_save``    | Path where the results will be saved                                               | ``None``              |\n| ``Typ_cir``      | Circuit type, can be ``1ph`` or ``Pos``.                                           | ``None``              |\n| ``ALG``          | Type of algorithm state variables. At the moment ``NV``                            | ``NV``                |\n| ``coord``        | Type of coordinates to solve. For the moment ``polar``.                            | ``Polar``             |\n| ``method``       | Solution method, can be ``nonlinear``, ``linear_PMU`` and ``nonlinear_PMU``.| ``nonlinear_PMU``|\n| ``name_project`` | Project name                                                                       | ``Default``           |\n| ``View_res``     | Displays the result of the selected algorithm by console                           | ``False``             |\n| ``DSS_coll``     | Displays next to the estimated status, the actual status according to OpenDSS      | ``False``             |\n| ``summary``      | Displays a summary of the simulation by console                                    | ``False``             |\n| ``MEAS_Pos``     | ``True`` if it is a ``Pos`` circuit, take the ``.json`` files in positive sequence.| ``False``             |\n\n<div id=\'id7\' />\n\n## Sample tests\n\nIn the path ``:{Python_library_path}/openpy_dsse/examples``, the ``.DSS`` and ``.json`` files of single-phase (``1ph``) and positive sequence equivalent (``Pos``) circuit measurements detailed in Table 11 are located.\n\n**Table 11.** Sample tests\n| **Circuit** | **Tpy_circ** | **Case** |\n|:------------:|:------------:|:--------:|\n|     4Node    |      1ph     |     1    |\n|  [15NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/15NodeIEEE/15NodeIEEE.ipynb)  |      1ph     |     2    |\n|  [13NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/13NodeIEEE/13NodeIEEE.ipynb)  |      Pos     |     1    |\n|  [37NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/37NodeIEEE/37NodeIEEE.ipynb)  |      Pos     |     2    |\n\nThe function ``test_circuit(Typ_cir, case)``, returns a dictionary with the keys ``\'DSS_file\'``, ``\'MEAS_path\'``, ``\'save_path\'``, ``\'name_project\'`` and ``\'Typ_cir\'`` which correspond to the ``.DSS`` file path, measurement file path, path where results will be saved and circuit type respectively.\n```Python\nimport openpy_dsse\n\ndsse = openpy_dsse.init_DSSE() #Start the class.\n\nif __name__ == \'__main__\':\n    net = dsse.test_circuit(Typ_cir=\'1ph\', case=1)\n    \n    #dsse.empty_init_files_MEAS_Unc(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n    #dsse.add_error_files_MEAS(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n    #dsse.empty_MEAS_files(DSS_path=net[\'DSS_file\'], MEAS_path=net[\'MEAS_path\'])\n\n    #execute the state estimation algorithm\n    Results = dsse.estimate(\n        DSS_path=net[\'DSS_file\'],\n        MEAS_path=net[\'MEAS_path\'],\n        path_save=net[\'save_path\'],\n        Typ_cir=net[\'Typ_cir\'],\n        name_project=net[\'name_project\'],\n        View_res=True,\n        summary=True,\n        DSS_coll=True,\n        #MEAS_Pos=True,\n        #method=\'nonlinear\'\n        #method=\'linear_PMU\',\n    )\n```\n\n<div id=\'id8\' />\n\n### License\n\nLicense: CC BY-NC-SA 4.0\n\n<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />\n\nThis work has a license <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.\n',
     'author': 'Jorge Lara',
     'author_email': 'jlara@iee.unsj.edu.ar',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `openpy_dsse-0.1.1/PKG-INFO` & `openpy_dsse-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpy-dsse
-Version: 0.1.1
+Version: 0.1.2
 Summary: Open source library for state estimation of a distribution network modeled in OpenDSS
 License: LICENSE
 Keywords: OpenDSS,DSSE,state estimation,smart grid,OpenPy-DSSE,OpenPy_DSSE
 Author: Jorge Lara
 Author-email: jlara@iee.unsj.edu.ar
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -32,32 +32,40 @@
 Requires-Dist: pytz (==2022.6)
 Requires-Dist: scipy (==1.9.3)
 Requires-Dist: seaborn (==0.12.1)
 Requires-Dist: six (==1.16.0)
 Requires-Dist: sympy (==1.11.1)
 Description-Content-Type: text/markdown
 
-# openpy_dsse
+# OpenPY_DSSE
 
-It is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks (OpenDSS) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.
+It is an open-source library developed in Python for estimating distribution networks (DSSE). It communicates with the free software for the simulation of electrical networks ([OpenDSS](https://sourceforge.net/projects/electricdss/)) and collects the results of power flow and distribution system parameters and executes the DSSE, obtaining an estimated state according to the type and location of measurements.
 
-It is developed within the framework of the OpenREiD project (Integral software for simulation and optimization of electrical distribution networks), of the Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina.
+It is developed within the framework of the[ OpenREiD](https://iee-unsjconicet.org/reid/) project (Integral software for simulation and optimization of electrical distribution networks), of the [Instituto de Energía Eléctrica (IEE), UNSJ - CONICET, San Juan - Argentina](https://iee-unsjconicet.org/).
 
 **Index**
 
+- [Weighted Least Squares](#id0)
 - [Installation](#id1)
 - [How to use](#id2)
   - [Measurements](#id3)
     - [Definition and creation of meters](#id4)
     - [Generate metrics from OpenDSS results](#id5)
   - [Run the state estimation algorithm](#id6)
   - [Sample tests](#id7)
 - [License](#id8)
 
+<div id='id0' />
+
+## Weighted Least Squares (WLS)
+
+The library uses a hybrid weighted least squares algorithm that incorporates traditional and D-PMU measurements. It supports single-phase and multiphase networks that are modeled as electromagnetically decoupled positive sequence impedances. More details can be found in [docs/methodology](https://github.com/jlara6/OpenPy-DSSE/blob/main/docs/methodology/Nonlinear_Hybrid_State_Estimator.ipynb)
+
 <div id='id1' />
+
 ## Installation
 
 With pip
 
 ``pip install py-open-dsse``
 
 Without pip, clone or download the repository, in the dist folder is the .whl file, copy the location of the file, and in the CMD:
@@ -227,17 +235,17 @@
 
 In the path ``:{Python_library_path}/openpy_dsse/examples``, the ``.DSS`` and ``.json`` files of single-phase (``1ph``) and positive sequence equivalent (``Pos``) circuit measurements detailed in Table 11 are located.
 
 **Table 11.** Sample tests
 | **Circuit** | **Tpy_circ** | **Case** |
 |:------------:|:------------:|:--------:|
 |     4Node    |      1ph     |     1    |
-|  15NodeIEEE  |      1ph     |     2    |
-|  13NodeIEEE  |      Pos     |     1    |
-|  37NodeIEEE  |      Pos     |     2    |
+|  [15NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/15NodeIEEE/15NodeIEEE.ipynb)  |      1ph     |     2    |
+|  [13NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/13NodeIEEE/13NodeIEEE.ipynb)  |      Pos     |     1    |
+|  [37NodeIEEE](https://github.com/jlara6/OpenPy-DSSE/blob/main/Sample_tests/37NodeIEEE/37NodeIEEE.ipynb)  |      Pos     |     2    |
 
 The function ``test_circuit(Typ_cir, case)``, returns a dictionary with the keys ``'DSS_file'``, ``'MEAS_path'``, ``'save_path'``, ``'name_project'`` and ``'Typ_cir'`` which correspond to the ``.DSS`` file path, measurement file path, path where results will be saved and circuit type respectively.
 ```Python
 import openpy_dsse
 
 dsse = openpy_dsse.init_DSSE() #Start the class.
```

