# Comparing `tmp/z4d-certified-devices-2.49.tar.gz` & `tmp/z4d-certified-devices-2.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z4d-certified-devices-2.49.tar", last modified: Sat Apr 22 08:49:05 2023, max compression
+gzip compressed data, was "z4d-certified-devices-2.50.tar", last modified: Sat Apr 22 09:59:26 2023, max compression
```

## Comparing `z4d-certified-devices-2.49.tar` & `z4d-certified-devices-2.50.tar`

### file list

```diff
@@ -1,518 +1,518 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.068721 z4d-certified-devices-2.49/z4d_certified_devices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.072721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.072721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LDSENK02F.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LDSENK10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LXEK-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LXEK-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LXEK-7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/ZBEK-14.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/ZBEK-3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.072721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Aotec/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Aotec/WG001-Z01.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.072721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/90201021A.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/90201021B.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/90201024.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/AV201021B.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/AV201024A.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/AV201029A.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.072721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/ZHUM.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/ZMOVE.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/ZPLUG.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CAC221.json
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CCB432.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CDWS312.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CKF204.json
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CKF205.json
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CMS323.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPB206.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPC321.json
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPR412.json
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSP403.json
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danalock/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danalock/V3-BTZB.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/RV001.json
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/eT093WRG.json
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/eT093WRO.json
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/eTRV0100.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/HESZB120.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/HMSZB-110.json
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/MOSZB-140.json
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/SMSZB-120.json
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/SPLZB-131.json
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/SPLZB-132.json
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/ZHEMI101.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Eurotronics/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.076721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.080721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/COSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/COSensor-EM.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/COSensor-N.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/CO_V15.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/CO_YDLV10.json
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/GAS_V15.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/RC-EM.json
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SMOK_V16.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SMOK_YDLV10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmartPlug.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmokeSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmokeSensor-N-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmokeSensor-N.json
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/TS0216.json
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/WarningDevice.json
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI wireless dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/OSL 130 C.json
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/RB 248 T.json
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/RB 285 C.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/SP 120.json
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/SP 220.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Idinio/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Iluminize/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Iluminize/511.201.json
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Iluminize/5120.1200.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE140103020000.json
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE170100510001.json
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE220103020000.json
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LIVOLO/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LIVOLO/TI0001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.084721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LS-Deutschland-GmbH/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.092721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.plug.json
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.router.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sens.json
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.weather.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.092721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Cable outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Connected outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Micromodule switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Mobile outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Teleruptor.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.092721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/Zigate-Router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.092721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nexturn/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.092721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nodon/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.096721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Plug 01.json
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Plug Z3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.096721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/3c4e4fc81ed442efaf69353effcdfc5f.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.096721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/BDP3001.json
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/Dimmablelight.json
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FB56-ZCW08KU1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/Lamp_01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/SA-003-Zigbee.json
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-CL01.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-CT01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-SW01.json
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-SW02.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.100721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/AC201A.json
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/AC211.json
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/AC221.json
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/CB432.json
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/DWS312-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/DWS312.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/KF204.json
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/KF205.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PB206.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PC321.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PIR323-A.json
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PIR323.json
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PR412.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/THS317-ET.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/THS317.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/VBS308.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/WSP402.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.100721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/440400982841.json
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/440400982842.json
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003052501_01.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003052501_02.json
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003053301_01.json
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003053301_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCA001.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT001.json
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT003.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT007.json
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT010.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT015.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT024.json
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LLC010.json
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LOM002.json
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LOM008.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LST002.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTA001.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTC001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTG002.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTW001.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTW004.json
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTW013.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWA001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWA009.json
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWB006.json
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWB010.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/ROM001.json
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/RWL021.json
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML001.json
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML002.json
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML003.json
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML004.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Robb-Smarrt/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/SALUS/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/SALUS/SPE600.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Samotech/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Samotech/SM309.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/iTRV.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/SmartThings/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/SmartThings/outletv4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.104721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/01MINIZB.json
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/66666.json
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/BASICZBR3.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/DONGLE-E_R.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/DS-01.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/DS01.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/MS01.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/MSO1.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/TH01.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/WB-01.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/WB01.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/ZBMINI-L.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.108721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/ZG2858A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.108721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.108721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TUYATEC/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TUYATEC/RH3001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/TUYATEC/RH3040.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0001.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0002.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0003-QS-Zigbee-S05-LN.json
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0003.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0011.json
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0012.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0013.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0041.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0042.json
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0043.json
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0044.json
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0046.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS004F.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0112.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0115.json
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-din.json
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-plug.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0121.json
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0201.json
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0202.json
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0203.json
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0205.json
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0207-extender.json
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0211.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0222.json
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0302.json
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0502A.json
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0505A.json
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0505B.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-SmartAir.json
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_chyvmhay.json
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV.json
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-motion.json
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-radar.json
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-smoke.json
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS1001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TY0202.json
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/fvq6avy.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/ivfvd7h.json
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/kud7u2l.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Woolley/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Woolley/SA-029-1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ynoa/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-SW01.json
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Zehnder/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.116721 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Zemismart/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 08:48:57.000000 z4d-certified-devices-2.49/z4d_certified_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:49:05.072721 z4d-certified-devices-2.49/z4d_certified_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-04-22 08:49:05.000000 z4d-certified-devices-2.49/z4d_certified_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-04-22 08:49:05.000000 z4d-certified-devices-2.49/z4d_certified_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:49:05.000000 z4d-certified-devices-2.49/z4d_certified_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 08:49:05.000000 z4d-certified-devices-2.49/z4d_certified_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:49:04.000000 z4d-certified-devices-2.49/z4d_certified_devices.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.036986 z4d-certified-devices-2.50/z4d_certified_devices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.040986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.040986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LDSENK02F.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LDSENK10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LXEK-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LXEK-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LXEK-7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/ZBEK-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/ZBEK-3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.040986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Aotec/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Aotec/WG001-Z01.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.040986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/90201021A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/90201021B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/90201024.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/AV201021B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/AV201024A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/AV201029A.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.044986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/ZHUM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/ZMOVE.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/ZPLUG.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.048986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CAC221.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CCB432.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CDWS312.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CKF204.json
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CKF205.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CMS323.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPB206.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPC321.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPR412.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSP403.json
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.048986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danalock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danalock/V3-BTZB.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.048986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/RV001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/eT093WRG.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/eT093WRO.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/eTRV0100.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.048986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/HESZB120.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/HMSZB-110.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/MOSZB-140.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/SMSZB-120.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/SPLZB-131.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/SPLZB-132.json
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/ZHEMI101.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.048986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.048986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Eurotronics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.052986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.056986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/COSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/COSensor-EM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/COSensor-N.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/CO_V15.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/CO_YDLV10.json
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/GAS_V15.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/RC-EM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SMOK_V16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SMOK_YDLV10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmartPlug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmokeSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmokeSensor-N-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmokeSensor-N.json
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/TS0216.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/WarningDevice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.068986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI wireless dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.068986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/OSL 130 C.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/RB 248 T.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/RB 285 C.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/SP 120.json
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/SP 220.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.068986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Idinio/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.068986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Iluminize/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Iluminize/511.201.json
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Iluminize/5120.1200.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.072986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE140103020000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE170100510001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE220103020000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.072986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LIVOLO/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LIVOLO/TI0001.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.072986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LS-Deutschland-GmbH/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.084986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.plug.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.router.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.weather.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.088986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Cable outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Connected outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Micromodule switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Mobile outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Teleruptor.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.088986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/Zigate-Router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.088986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nexturn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.088986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nodon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.092986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Plug 01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Plug Z3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.092986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/3c4e4fc81ed442efaf69353effcdfc5f.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.096986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/BDP3001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/Dimmablelight.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FB56-ZCW08KU1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/Lamp_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/SA-003-Zigbee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-CL01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-CT01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-SW01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-SW02.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.100986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/AC201A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/AC211.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/AC221.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/CB432.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/DWS312-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/DWS312.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/KF204.json
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/KF205.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PB206.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PC321.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PIR323-A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PIR323.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PR412.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/THS317-ET.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/THS317.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/VBS308.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/WSP402.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.108986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/440400982841.json
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/440400982842.json
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003052501_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003052501_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003053301_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003053301_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCA001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT003.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT007.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT015.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT024.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LLC010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LOM002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LOM008.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LST002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTA001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTC001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTG002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTW001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTW004.json
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTW013.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWA001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWA009.json
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWB006.json
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWB010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/ROM001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/RWL021.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML003.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML004.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.108986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.108986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Robb-Smarrt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.108986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/SALUS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/SALUS/SPE600.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.108986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Samotech/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Samotech/SM309.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.112986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/iTRV.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.116986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/SmartThings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/SmartThings/outletv4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.116986 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/01MINIZB.json
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/66666.json
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/BASICZBR3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/DONGLE-E_R.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/DS-01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/DS01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/MS01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/MSO1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/TH01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/WB-01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/WB01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/ZBMINI-L.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.120987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/ZG2858A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.120987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.120987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TUYATEC/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TUYATEC/RH3001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/TUYATEC/RH3040.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.140987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0003-QS-Zigbee-S05-LN.json
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0003.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0011.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0012.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0013.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0041.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0042.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0043.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0044.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0046.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS004F.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0112.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0115.json
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-din.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-plug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0121.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0201.json
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0202.json
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0203.json
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0205.json
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0207-extender.json
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0211.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0222.json
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0302.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0502A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0505A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0505B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-SmartAir.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_chyvmhay.json
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV.json
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-motion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-radar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-smoke.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS1001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TY0202.json
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/fvq6avy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/ivfvd7h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/kud7u2l.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.140987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Woolley/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Woolley/SA-029-1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ynoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-SW01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Zehnder/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.144987 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Zemismart/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 09:59:13.000000 z4d-certified-devices-2.50/z4d_certified_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 09:59:26.036986 z4d-certified-devices-2.50/z4d_certified_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-04-22 09:59:25.000000 z4d-certified-devices-2.50/z4d_certified_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-04-22 09:59:26.000000 z4d-certified-devices-2.50/z4d_certified_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:59:25.000000 z4d-certified-devices-2.50/z4d_certified_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 09:59:25.000000 z4d-certified-devices-2.50/z4d_certified_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 09:59:25.000000 z4d-certified-devices-2.50/z4d_certified_devices.egg-info/zip-safe
```

### Comparing `z4d-certified-devices-2.49/LICENSE.txt` & `z4d-certified-devices-2.50/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/PKG-INFO` & `z4d-certified-devices-2.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z4d-certified-devices
-Version: 2.49
+Version: 2.50
 Summary: "Certified devices for Zigbee for Domoticz plugin"
 Home-page: https://github.com/zigbeefordomoticz/z4d-certified-devices
 Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me"
 License: "GPL-3.0"
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `z4d-certified-devices-2.49/README.md` & `z4d-certified-devices-2.50/README.md`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/setup.cfg` & `z4d-certified-devices-2.50/setup.cfg`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LDSENK02F.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LDSENK02F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LDSENK10.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LDSENK10.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LXEK-1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LXEK-1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LXEK-2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LXEK-2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/LXEK-7.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/LXEK-7.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/ZBEK-14.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/ZBEK-14.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Adeo/ZBEK-3.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Adeo/ZBEK-3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Aotec/WG001-Z01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Aotec/WG001-Z01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/90201021A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/90201021A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/AV201024A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/AV201024A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Bitron/AV201029A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Bitron/AV201029A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/ZHUM.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/ZHUM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/ZMOVE.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/ZMOVE.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/CLEODE/ZPLUG.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/CLEODE/ZPLUG.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CAC221.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CAC221.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CCB432.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CCB432.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CDWS312.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CDWS312.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CKF205.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CKF205.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CMS323.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CMS323.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPC321.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPC321.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CPR412.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CPR412.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CSP403.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CSP403.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danalock/V3-BTZB.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danalock/V3-BTZB.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/RV001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/RV001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/eT093WRG.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/eT093WRG.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/eT093WRO.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/eT093WRO.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Danfoss/eTRV0100.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Danfoss/eTRV0100.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/HESZB120.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/HESZB120.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/HMSZB-110.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/HMSZB-110.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/MOSZB-140.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/MOSZB-140.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/SMSZB-120.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/SMSZB-120.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/SPLZB-131.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/SPLZB-131.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/SPLZB-132.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/SPLZB-132.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Develco/ZHEMI101.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Develco/ZHEMI101.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/COSensor-EM.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/COSensor-EM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/RC-EM.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/RC-EM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmartPlug.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmartPlug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/TS0216.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/TS0216.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/WarningDevice.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/WarningDevice.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/OSL 130 C.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/OSL 130 C.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/RB 248 T.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/RB 248 T.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/RB 285 C.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/RB 285 C.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/SP 120.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/SP 120.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/INNR/SP 220.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/INNR/SP 220.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Iluminize/511.201.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Iluminize/511.201.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Iluminize/5120.1200.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Iluminize/5120.1200.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE140103020000.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE140103020000.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE170100510001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE170100510001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE220103020000.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE220103020000.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LIVOLO/TI0001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LIVOLO/TI0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.plug.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.plug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.router.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.router.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sens.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sens.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5454931972789115%*

 * *Differences: {"'ClusterToBind'": "''",*

 * * "'Ep'": "{'01': {'Type': 'Vibration/Strength/Orientation', '0003': '', '0005': '', '0019': '', "*

 * *         "'0101': '', delete: ['0006']}, '02': OrderedDict([('0003', ''), ('0004', ''), ('0005', "*

 * *         "''), ('0012', ''), ('Type', '')])}",*

 * * "'Param'": "OrderedDict([('vibrationAqarasensitivity', 'medium')])",*

 * * "'ReadAttributes'": "{'0101': [], delete: ['0006']}",*

 * * 'delete': "['NoDeviceInterview']"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "ClusterToBind": [],
+    "ClusterToBind": "",
     "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": {
                 "Attributes": {
                     "ff01": {
                         "ActionList": [
@@ -33,21 +33,33 @@
                         "Enabled": true,
                         "ManufRawData": true,
                         "ManufSpecificFunc": "Lumi_fcc0",
                         "Name": "Aqara_0000_fff0"
                     }
                 }
             },
-            "0006": "",
-            "Type": "SwitchAQ2WithOff"
+            "0003": "",
+            "0005": "",
+            "0019": "",
+            "0101": "",
+            "Type": "Vibration/Strength/Orientation"
+        },
+        "02": {
+            "0003": "",
+            "0004": "",
+            "0005": "",
+            "0012": "",
+            "Type": ""
         }
     },
-    "NoDeviceInterview": 1,
+    "Param": {
+        "vibrationAqarasensitivity": "medium"
+    },
     "ReadAttributes": {
         "0000": [
             "0004",
             "0005"
         ],
-        "0006": []
+        "0101": []
     },
     "Type": ""
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5274621212121212%*

 * *Differences: {"'ClusterToBind'": "{insert: [(0, '0000')]}",*

 * * "'ConfigureReporting'": "{replace: OrderedDict([('0006', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('DataType', '10'), ('MinInterval', "*

 * *                         "'0001'), ('MaxInterval', '012c'), ('TimeOut', '0000'), ('Change', "*

 * *                         "'01')]))]))]))])}",*

 * * "'Ep'": "{'01': {'Type': 'Switch', '0003': '', '0004': '', '0005': '', '0006': '', '0019': '', "*

 * *         "'0b05': ''}, 'f2': OrderedDict […]*

```diff
@@ -1,40 +1,70 @@
 {
     "ClusterToBind": [
+        "0000",
         "0006"
     ],
-    "ConfigureReporting": {},
+    "ConfigureReporting": {
+        "0006": {
+            "Attributes": {
+                "0000": {
+                    "Change": "01",
+                    "DataType": "10",
+                    "MaxInterval": "012c",
+                    "MinInterval": "0001",
+                    "TimeOut": "0000"
+                }
+            }
+        }
+    },
     "Ep": {
         "01": {
             "0000": "",
-            "Type": ""
-        },
-        "02": {
+            "0003": "",
+            "0004": "",
+            "0005": "",
             "0006": "",
+            "0019": "",
+            "0b05": "",
             "Type": "Switch"
+        },
+        "f2": {
+            "Type": ""
         }
     },
-    "Param": {},
+    "Identifier": [
+        [
+            "PUCK/SWITCH/1",
+            "Schneider Electric"
+        ],
+        [
+            "PUCKSWITCH1",
+            "Schneider Electric"
+        ]
+    ],
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
             "0006",
-            "0032",
-            "0033",
-            "ff01"
+            "0007",
+            "000a",
+            "000f",
+            "0010",
+            "0015",
+            "f000"
         ],
         "0006": [
             "0000"
         ],
         "0019": []
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Aqara_QBKG21LM.html",
-    "_comment": "D1 Wall Switch (No Neutral, Single Rocker)",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1585#issuecomment-1515294766",
-    "_version": "1.0"
+    "_blakadder": "https://zigbee.blakadder.com/Schneider_Electric_W50110.html",
+    "_comment": "Wiser Micro Module Light Switch",
+    "_source": "https://easydomoticz.com/forum/viewtopic.php?t=13031",
+    "_version": "1.1"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47085648148148146%*

 * *Differences: {"'BatteryDevice'": '1',*

 * * "'BatteryPercentageConverter'": '2',*

 * * "'ClusterToBind'": "['0500']",*

 * * "'Ep'": "{'02': {'Type': 'Motion', '0000': '', '0001': '', '0003': '', '0500': '', delete: "*

 * *         "['0006']}, delete: ['01', '03']}",*

 * * "'NickName'": "'Hue_Motion'",*

 * * "'Param'": "{replace: OrderedDict([('MotionViaIASAlarm1', 1)])}",*

 * * "'ReadAttributes'": "{'0000': {delete: [9, 8, 7, 6, 3, 2, 1, 0]}, '0001': ['0021'], '0500': "*

 * *                     "['0000', '0001', '0002', '0010'], delete: ['0006', '0019']}",*

 * *  […]*

```diff
@@ -1,43 +1,39 @@
 {
+    "BatteryDevice": 1,
+    "BatteryPercentageConverter": 2,
     "ClusterToBind": [
-        "0006"
+        "0500"
     ],
     "ConfigureReporting": {},
     "Ep": {
-        "01": {
-            "0000": "",
-            "Type": ""
-        },
         "02": {
-            "0006": "",
-            "Type": "Switch"
-        },
-        "03": {
-            "0006": "",
-            "Type": "Switch"
+            "0000": "",
+            "0001": "",
+            "0003": "",
+            "0500": "",
+            "Type": "Motion"
         }
     },
-    "Param": {},
+    "NickName": "Hue_Motion",
+    "Param": {
+        "MotionViaIASAlarm1": 1
+    },
     "ReadAttributes": {
         "0000": [
-            "0000",
-            "0001",
-            "0002",
-            "0003",
             "0004",
-            "0005",
-            "0006",
-            "0032",
-            "0033",
-            "ff01"
+            "0005"
         ],
-        "0006": [
-            "0000"
+        "0001": [
+            "0021"
         ],
-        "0019": []
+        "0500": [
+            "0000",
+            "0001",
+            "0002",
+            "0010"
+        ]
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Aqara_QBKG22LM.html",
-    "_comment": "D1 Wall Switch (No Neutral, Double Rocker) ( 2 Gang) ",
+    "_comment": "https://zigbee.blakadder.com/AduroSmart_81823.html",
     "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5473065476190476%*

 * *Differences: {"'ClusterToBind'": "{insert: [(1, '0008'), (2, '0300')]}",*

 * * "'ConfigureReporting'": "{replace: OrderedDict([('0006', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('DataType', '10'), ('MinInterval', "*

 * *                         "'0001'), ('MaxInterval', '012C'), ('TimeOut', '0000'), ('Change', "*

 * *                         "'01')]))]))])), ('0008', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('DataType', '20'), ('MinInte […]*

```diff
@@ -1,54 +1,81 @@
 {
     "ClusterToBind": [
-        "0006"
+        "0006",
+        "0008",
+        "0300"
     ],
-    "ConfigureReporting": {},
+    "ConfigureReporting": {
+        "0006": {
+            "Attributes": {
+                "0000": {
+                    "Change": "01",
+                    "DataType": "10",
+                    "MaxInterval": "012C",
+                    "MinInterval": "0001",
+                    "TimeOut": "0000"
+                }
+            }
+        },
+        "0008": {
+            "Attributes": {
+                "0000": {
+                    "Change": "05",
+                    "DataType": "20",
+                    "MaxInterval": "012C",
+                    "MinInterval": "0005",
+                    "TimeOut": "0000"
+                }
+            }
+        }
+    },
     "Ep": {
         "01": {
             "0000": "",
-            "0002": "",
             "0003": "",
             "0004": "",
             "0005": "",
             "0006": "",
-            "0009": "",
-            "000a": "",
+            "0008": "",
             "0019": "",
-            "Type": "Switch"
+            "0300": "",
+            "1000": "",
+            "Type": "ColorControlWW",
+            "fc82": ""
         },
-        "02": {
+        "f2": {
             "0000": "",
-            "0006": "",
-            "Type": "Switch"
+            "0021": ""
         }
     },
     "Param": {
-        "AqaraOppleMode": 1,
-        "AqaraOpple_aqara_switch_mode_switch": 1,
-        "AqaraOpple_flip_indicator_light": 0,
-        "AqaraOpple_switch_operation_mode_opple": 0,
-        "AqaraOpple_switch_power_outage_memory": 1
+        "PowerOnAfterOffOn": 1,
+        "fadingOff": 0,
+        "moveToColourTemp": 0,
+        "moveToLevel": 0
     },
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
             "0006",
-            "0032",
-            "0033"
+            "0007"
         ],
         "0006": [
-            "0000"
+            "0000",
+            "4001",
+            "4002",
+            "4003"
         ],
-        "0019": []
+        "0008": [
+            "0000"
+        ]
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Aqara_QBKG39LM.html",
-    "_comment": "E1 Wall Switch (No Neutral, Double Rocker)",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1576",
-    "_version": "Initial Version"
+    "_blakadder": "https://zigbee.blakadder.com/Ynoa_LA-GU10-CCT.html",
+    "_comment": "Smart Spot White Tones GU10 CCT",
+    "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.43967803030303027%*

 * *Differences: {"'ClusterToBind'": "['0001', '0003']",*

 * * "'ConfigureReporting'": "{replace: OrderedDict([('0006', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('Change', '01'), ('DataType', '10'), "*

 * *                         "('MaxInterval', '0258'), ('MinInterval', '0000'), ('TimeOut', "*

 * *                         "'0FFF')]))]))])), ('0008', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('DataType', '20'), ('MinInterval', "*

 * *            […]*

```diff
@@ -1,56 +1,72 @@
 {
     "ClusterToBind": [
-        "0006",
-        "0012"
+        "0001",
+        "0003"
     ],
-    "ConfigureReporting": {},
+    "ConfigureReporting": {
+        "0006": {
+            "Attributes": {
+                "0000": {
+                    "Change": "01",
+                    "DataType": "10",
+                    "MaxInterval": "0258",
+                    "MinInterval": "0000",
+                    "TimeOut": "0FFF"
+                }
+            }
+        },
+        "0008": {
+            "Attributes": {
+                "0000": {
+                    "Change": "05",
+                    "DataType": "20",
+                    "MaxInterval": "012C",
+                    "MinInterval": "0005",
+                    "TimeOut": "0000"
+                }
+            }
+        }
+    },
     "Ep": {
         "01": {
             "0000": "",
-            "0002": "",
             "0003": "",
             "0004": "",
+            "0005": "",
             "0006": "",
-            "0009": "",
-            "000a": "",
+            "0008": "",
             "0019": "",
-            "Type": "Switch"
-        },
-        "29": {
-            "0012": "",
-            "Type": ""
+            "0b05": "",
+            "Type": "LvlControl"
         }
     },
-    "Param": {
-        "AqaraOppleMode": 1,
-        "AqaraOpple_aqara_switch_mode_switch": 1,
-        "AqaraOpple_flip_indicator_light": 0,
-        "AqaraOpple_led_disabled_night": 0,
-        "AqaraOpple_switch_operation_mode_opple": 0,
-        "AqaraOpple_switch_power_outage_memory": 1
-    },
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
-            "0006",
-            "0007"
+            "0007",
+            "000a",
+            "4000"
+        ],
+        "0001": [
+            "0020",
+            "0021",
+            "0033"
         ],
         "0006": [
             "0000"
         ],
-        "0012": [
-            "0055"
-        ],
-        "0019": []
+        "0008": [
+            "0000"
+        ]
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Aqara_WS-EUK01.html",
-    "_description": "Aqara smart wall switch H1 EU (no neutral, single rocker)",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1585",
-    "_version": "0.1"
+    "_blakadder": "https://zigbee.blakadder.com/Sunricher_SR-ZG9101SAC-HP.html",
+    "_comment": "AC Phase-Cut Dimmer",
+    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1583",
+    "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6624579124579125%*

 * *Differences: {"'ClusterToBind'": "{insert: [(1, '0012')]}",*

 * * "'Ep'": "{'01': {'0000': {replace: OrderedDict([('Attributes', OrderedDict([('fff0', "*

 * *         "OrderedDict([('Enabled', True), ('Name', 'Aqara_0000_fff0'), ('DataType', '42'), "*

 * *         "('ManufRawData', True), ('ManufSpecificFunc', 'Lumi_fcc0'), ('ActionList', "*

 * *         "['check_store_value'])])), ('ff01', OrderedDict([('Enabled', True), ('Name', "*

 * *         "'Aqara_0000_ff01'), ('DataType', '42'), ('ManufRawData', True), ('ManufSpecificFunc', "*

 * *         " […]*

```diff
@@ -1,28 +1,61 @@
 {
     "ClusterToBind": [
-        "0006"
+        "0006",
+        "0012"
     ],
     "ConfigureReporting": {},
     "Ep": {
         "01": {
-            "0000": "",
+            "0000": {
+                "Attributes": {
+                    "ff01": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff01"
+                    },
+                    "ff02": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "4c",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff02"
+                    },
+                    "fff0": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_fff0"
+                    }
+                }
+            },
             "0002": "",
             "0003": "",
             "0004": "",
             "0006": "",
             "0009": "",
             "000a": "",
             "0019": "",
             "Type": "Switch"
         },
-        "02": {
-            "0000": "",
-            "0006": "",
-            "Type": "Switch"
+        "29": {
+            "0012": "",
+            "Type": ""
         }
     },
     "Param": {
         "AqaraOppleMode": 1,
         "AqaraOpple_aqara_switch_mode_switch": 1,
         "AqaraOpple_flip_indicator_light": 0,
         "AqaraOpple_led_disabled_night": 0,
@@ -39,15 +72,18 @@
             "0005",
             "0006",
             "0007"
         ],
         "0006": [
             "0000"
         ],
+        "0012": [
+            "0055"
+        ],
         "0019": []
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Aqara_WS-EUK02.html",
-    "_comment": "Aqara smart wall switch H1 EU (no neutral, double rocker)",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1503",
+    "_blakadder": "https://zigbee.blakadder.com/Aqara_WS-EUK01.html",
+    "_description": "Aqara smart wall switch H1 EU (no neutral, single rocker)",
+    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1585",
     "_version": "0.1"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/LUMI/lumi.weather.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.weather.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Cable outlet.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Cable outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Connected outlet.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Connected outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Micromodule switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Micromodule switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Mobile outlet.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Mobile outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Legrand/Teleruptor.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Legrand/Teleruptor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Lixee/Zigate-Router.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Lixee/Zigate-Router.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Plug 01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Plug 01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/OSRAM/Plug Z3.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/OSRAM/Plug Z3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/BDP3001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/BDP3001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/Dimmablelight.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/Dimmablelight.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/Lamp_01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/Lamp_01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0202.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6116071428571429%*

 * *Differences: {"'ClusterToBind'": "{insert: [(0, '0001')]}",*

 * * "'Ep'": "{replace: OrderedDict([('01', OrderedDict([('0000', ''), ('0001', ''), ('0500', ''), "*

 * *         "('Type', 'Motion/Tamper')]))])}",*

 * * "'Param'": "{'TuyaPIRKeepTime': 1, 'IASsensitivity': 1}",*

 * * "'ReadAttributes'": "{'0001': {insert: [(0, '0020')]}, '0500': {insert: [(4, '0011'), (5, "*

 * *                     "'0013'), (6, 'f001')]}}",*

 * * "'_blakadder'": "'https://zigbee.blakadder.com/Tuya_ZM-35ZH-Q.html'",*

 * * "'_comment'": "'Tuya Motion Sensor IH012-RT01'",*

 * * 'd […]*

```diff
@@ -1,39 +1,44 @@
 {
     "BatteryDevice": 1,
     "BatteryPercentageConverter": 2,
     "ClusterToBind": [
+        "0001",
         "0500"
     ],
     "ConfigureReporting": {},
     "Ep": {
-        "02": {
+        "01": {
             "0000": "",
             "0001": "",
-            "0003": "",
             "0500": "",
-            "Type": "Motion"
+            "Type": "Motion/Tamper"
         }
     },
-    "NickName": "Hue_Motion",
     "Param": {
-        "MotionViaIASAlarm1": 1
+        "IASsensitivity": 1,
+        "MotionViaIASAlarm1": 1,
+        "TuyaPIRKeepTime": 1
     },
     "ReadAttributes": {
         "0000": [
             "0004",
             "0005"
         ],
         "0001": [
+            "0020",
             "0021"
         ],
         "0500": [
             "0000",
             "0001",
             "0002",
-            "0010"
+            "0010",
+            "0011",
+            "0013",
+            "f001"
         ]
     },
     "Type": "",
-    "_comment": "https://zigbee.blakadder.com/AduroSmart_81823.html",
-    "_version": "1.0"
+    "_blakadder": "https://zigbee.blakadder.com/Tuya_ZM-35ZH-Q.html",
+    "_comment": "Tuya Motion Sensor IH012-RT01"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-CL01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-CL01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-CT01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-CT01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Others/ZB-SW02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Others/ZB-SW02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/AC201A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/AC201A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/AC211.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/AC211.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/AC221.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/AC221.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/CB432.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/CB432.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/DWS312-E.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/DWS312-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/KF205.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/KF205.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PC321.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PC321.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PIR323-A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PIR323-A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PIR323.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PIR323.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/PR412.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/PR412.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/THS317-ET.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/THS317-ET.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Owon/WSP402.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Owon/WSP402.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/440400982841.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/440400982841.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/440400982842.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/440400982842.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003052501_01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003052501_01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003052501_02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003052501_02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003053301_01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003053301_01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/929003053301_02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/929003053301_02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCA001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCA001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT003.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT003.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT007.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT007.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT010.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT010.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT015.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT015.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LCT024.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LCT024.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LLC010.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LLC010.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LOM008.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LOM008.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LST002.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LST002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTA001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTA001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTC001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTC001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTG002.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTG002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTW001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTW001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTW004.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTW004.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LTW013.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LTW013.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWA001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWA001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWA009.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWA009.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWB006.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWB006.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/LWB010.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/LWB010.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/ROM001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/ROM001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/RWL021.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/RWL021.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML002.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML003.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML003.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Philips/SML004.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Philips/SML004.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/README.md` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/README.md`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/SALUS/SPE600.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/SALUS/SPE600.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Samotech/SM309.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Samotech/SM309.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0042.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.40946969696969693%*

 * *Differences: {"'ClusterToBind'": "{insert: [(1, '0001')], delete: [0]}",*

 * * "'ConfigureReporting'": '{replace: OrderedDict()}',*

 * * "'Ep'": "{'01': {'Type': 'Button_3', '0001': '', '000a': '', delete: ['0003', '0b05']}, '02': "*

 * *         "OrderedDict([('0000', ''), ('0001', ''), ('0004', ''), ('0005', ''), ('0006', ''), "*

 * *         "('000a', ''), ('0019', ''), ('Type', 'Button_3')]), delete: ['f2']}",*

 * * "'ReadAttributes'": "{'0000': {insert: [(6, '0007'), (9, 'ffe2'), (10, 'ffdf')], delete: [12, 11, "*

 * *                     "10,  […]*

```diff
@@ -1,70 +1,49 @@
 {
     "ClusterToBind": [
-        "0000",
-        "0006"
+        "0006",
+        "0001"
     ],
-    "ConfigureReporting": {
-        "0006": {
-            "Attributes": {
-                "0000": {
-                    "Change": "01",
-                    "DataType": "10",
-                    "MaxInterval": "012c",
-                    "MinInterval": "0001",
-                    "TimeOut": "0000"
-                }
-            }
-        }
-    },
+    "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
-            "0003": "",
+            "0001": "",
             "0004": "",
             "0005": "",
             "0006": "",
+            "000a": "",
             "0019": "",
-            "0b05": "",
-            "Type": "Switch"
+            "Type": "Button_3"
         },
-        "f2": {
-            "Type": ""
+        "02": {
+            "0000": "",
+            "0001": "",
+            "0004": "",
+            "0005": "",
+            "0006": "",
+            "000a": "",
+            "0019": "",
+            "Type": "Button_3"
         }
     },
-    "Identifier": [
-        [
-            "PUCK/SWITCH/1",
-            "Schneider Electric"
-        ],
-        [
-            "PUCKSWITCH1",
-            "Schneider Electric"
-        ]
-    ],
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
+            "0007",
             "0006",
             "0007",
-            "000a",
-            "000f",
-            "0010",
-            "0015",
-            "f000"
-        ],
-        "0006": [
-            "0000"
+            "ffe2",
+            "ffdf"
         ],
-        "0019": []
+        "0006": []
     },
+    "TUYA_REMOTE": true,
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Schneider_Electric_W50110.html",
-    "_comment": "Wiser Micro Module Light Switch",
-    "_source": "https://easydomoticz.com/forum/viewtopic.php?t=13031",
-    "_version": "1.1"
+    "_comment": "2 Gang Wireless Switch",
+    "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Schneider/iTRV.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Schneider/iTRV.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/SmartThings/outletv4.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/SmartThings/outletv4.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/01MINIZB.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/01MINIZB.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/66666.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/66666.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/TH01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/TH01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/ZG2858A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/ZG2858A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48665123456790127%*

 * *Differences: {"'ClusterToBind'": "['0000', '0005']",*

 * * "'ConfigureReporting'": '{replace: OrderedDict()}',*

 * * "'Ep'": "{'01': {'Type': 'ColorControlFull', delete: ['0003', '0004', '0006', '0008', '0019', "*

 * *         "'0b05']}, '02': OrderedDict([('0000', ''), ('0001', ''), ('0003', ''), ('0004', ''), "*

 * *         "('0005', ''), ('0006', ''), ('0008', ''), ('0019', ''), ('0300', ''), ('0b05', ''), "*

 * *         "('Type', 'ColorControlFull')]), '03': OrderedDict([('0000', ''), ('Type', "*

 * *         "'ColorControlFull')]), '04': Orde […]*

```diff
@@ -1,47 +1,39 @@
 {
     "ClusterToBind": [
-        "0001",
-        "0003"
+        "0000",
+        "0005"
     ],
-    "ConfigureReporting": {
-        "0006": {
-            "Attributes": {
-                "0000": {
-                    "Change": "01",
-                    "DataType": "10",
-                    "MaxInterval": "0258",
-                    "MinInterval": "0000",
-                    "TimeOut": "0FFF"
-                }
-            }
-        },
-        "0008": {
-            "Attributes": {
-                "0000": {
-                    "Change": "05",
-                    "DataType": "20",
-                    "MaxInterval": "012C",
-                    "MinInterval": "0005",
-                    "TimeOut": "0000"
-                }
-            }
-        }
-    },
+    "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
+            "0005": "",
+            "Type": "ColorControlFull"
+        },
+        "02": {
+            "0000": "",
+            "0001": "",
             "0003": "",
             "0004": "",
             "0005": "",
             "0006": "",
             "0008": "",
             "0019": "",
+            "0300": "",
             "0b05": "",
-            "Type": "LvlControl"
+            "Type": "ColorControlFull"
+        },
+        "03": {
+            "0000": "",
+            "Type": "ColorControlFull"
+        },
+        "04": {
+            "0000": "",
+            "Type": "ColorControlFull"
         }
     },
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
@@ -53,20 +45,15 @@
             "4000"
         ],
         "0001": [
             "0020",
             "0021",
             "0033"
         ],
-        "0006": [
-            "0000"
-        ],
-        "0008": [
-            "0000"
-        ]
+        "0006": [],
+        "0008": [],
+        "0300": []
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Sunricher_SR-ZG9101SAC-HP.html",
-    "_comment": "AC Phase-Cut Dimmer",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1583",
-    "_version": "1.0"
+    "_comment": "Single Color 4 Groups ZigBee Key Remote Controller",
+    "_version": "0.1"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0302.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.32977891156462585%*

 * *Differences: {"'ClusterToBind'": "{insert: [(1, '0102')], delete: [1]}",*

 * * "'ConfigureReporting'": "{replace: OrderedDict([('0102', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0008', OrderedDict([('DataType', '20'), ('MinInterval', "*

 * *                         "'0001'), ('MaxInterval', '0384'), ('TimeOut', '0000'), ('Change', "*

 * *                         "'01')]))]))]))])}",*

 * * "'Ep'": "{'01': {'Type': 'Venetian', '0102': '', '0019': ''}, 'f2': OrderedDict([('Type', '')]), "*

 * *         "delete: ['02',  […]*

```diff
@@ -1,59 +1,56 @@
 {
     "ClusterToBind": [
         "0000",
-        "0005"
+        "0102"
     ],
-    "ConfigureReporting": {},
+    "ConfigureReporting": {
+        "0102": {
+            "Attributes": {
+                "0008": {
+                    "Change": "01",
+                    "DataType": "20",
+                    "MaxInterval": "0384",
+                    "MinInterval": "0001",
+                    "TimeOut": "0000"
+                }
+            }
+        }
+    },
     "Ep": {
         "01": {
             "0000": "",
             "0005": "",
-            "Type": "ColorControlFull"
-        },
-        "02": {
-            "0000": "",
-            "0001": "",
-            "0003": "",
-            "0004": "",
-            "0005": "",
-            "0006": "",
-            "0008": "",
             "0019": "",
-            "0300": "",
-            "0b05": "",
-            "Type": "ColorControlFull"
+            "0102": "",
+            "Type": "Venetian"
         },
-        "03": {
-            "0000": "",
-            "Type": "ColorControlFull"
-        },
-        "04": {
-            "0000": "",
-            "Type": "ColorControlFull"
+        "f2": {
+            "Type": ""
         }
     },
+    "IgnoreWindowsCoverringValue50": 1,
+    "Param": {},
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
+            "0006",
             "0007",
             "000a",
-            "4000"
-        ],
-        "0001": [
-            "0020",
-            "0021",
-            "0033"
+            "000f",
+            "0010",
+            "0015",
+            "f000"
         ],
-        "0006": [],
-        "0008": [],
-        "0300": []
+        "0019": [],
+        "0102": [
+            "0008"
+        ]
     },
     "Type": "",
-    "_comment": "Single Color 4 Groups ZigBee Key Remote Controller",
-    "_version": "0.1"
+    "WindowsCoverringInverted": 1
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/TUYATEC/RH3040.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/TUYATEC/RH3040.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0002.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0003.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0003.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0011.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0011.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0012.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0012.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0013.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0013.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0041.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0041.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0042.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0044.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.512224517906336%*

 * *Differences: {"'BatteryDevice'": '1',*

 * * "'BatteryPercentageConverter'": '2',*

 * * "'ClusterToBind'": "{insert: [(1, '0006')], delete: [0]}",*

 * * "'ConfigureReporting'": "{replace: OrderedDict([('0006', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('DataType', '10'), ('MinInterval', "*

 * *                         "'0001'), ('MaxInterval', '012C'), ('TimeOut', '0258'), ('Change', "*

 * *                         "'01')]))]))]))])}",*

 * * "'Ep'": "{'01': {delete: ['0004', '0005']}, '02': {delete: [' […]*

```diff
@@ -1,49 +1,63 @@
 {
+    "BatteryDevice": 1,
+    "BatteryPercentageConverter": 2,
     "ClusterToBind": [
-        "0006",
-        "0001"
+        "0001",
+        "0006"
     ],
-    "ConfigureReporting": {},
+    "ConfigureReporting": {
+        "0006": {
+            "Attributes": {
+                "0000": {
+                    "Change": "01",
+                    "DataType": "10",
+                    "MaxInterval": "012C",
+                    "MinInterval": "0001",
+                    "TimeOut": "0258"
+                }
+            }
+        }
+    },
     "Ep": {
         "01": {
             "0000": "",
             "0001": "",
-            "0004": "",
-            "0005": "",
             "0006": "",
             "000a": "",
             "0019": "",
             "Type": "Button_3"
         },
         "02": {
-            "0000": "",
-            "0001": "",
-            "0004": "",
-            "0005": "",
             "0006": "",
-            "000a": "",
-            "0019": "",
+            "Type": "Button_3"
+        },
+        "03": {
+            "0006": "",
+            "Type": "Button_3"
+        },
+        "04": {
+            "0006": "",
             "Type": "Button_3"
         }
     },
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
-            "0002",
-            "0003",
             "0004",
-            "0005",
-            "0007",
-            "0006",
-            "0007",
-            "ffe2",
-            "ffdf"
+            "0005"
+        ],
+        "0001": [
+            "0020",
+            "0021"
         ],
         "0006": []
     },
+    "ReadAttributesEp": [
+        "01"
+    ],
     "TUYA_REMOTE": true,
     "Type": "",
-    "_comment": "2 Gang Wireless Switch",
-    "_version": "1.0"
+    "_comment": "Tuya 4 switch remote (Single, Double,Long press)",
+    "_version": "Initial Version"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0043.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0043.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0044.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8302083333333333%*

 * *Differences: {"'ClusterToBind'": '{delete: [0]}',*

 * * "'ConfigureReporting'": '{replace: OrderedDict()}',*

 * * "'Param'": "OrderedDict([('TS004FMode', 'Scene')])",*

 * * "'ReadAttributes'": "{'0000': {insert: [(2, '0000'), (3, '0001'), (4, '0007'), (5, 'fffe')], "*

 * *                     "delete: [1, 0]}, '0006': ['0000', '8004'], '0019': [], 'e001': ['d011']}"}*

```diff
@@ -1,27 +1,14 @@
 {
     "BatteryDevice": 1,
     "BatteryPercentageConverter": 2,
     "ClusterToBind": [
-        "0001",
         "0006"
     ],
-    "ConfigureReporting": {
-        "0006": {
-            "Attributes": {
-                "0000": {
-                    "Change": "01",
-                    "DataType": "10",
-                    "MaxInterval": "012C",
-                    "MinInterval": "0001",
-                    "TimeOut": "0258"
-                }
-            }
-        }
-    },
+    "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
             "0001": "",
             "0006": "",
             "000a": "",
             "0019": "",
@@ -36,26 +23,38 @@
             "Type": "Button_3"
         },
         "04": {
             "0006": "",
             "Type": "Button_3"
         }
     },
+    "Param": {
+        "TS004FMode": "Scene"
+    },
     "ReadAttributes": {
         "0000": [
+            "0004",
+            "0005",
             "0000",
             "0001",
-            "0004",
-            "0005"
+            "0007",
+            "fffe"
         ],
         "0001": [
             "0020",
             "0021"
         ],
-        "0006": []
+        "0006": [
+            "0000",
+            "8004"
+        ],
+        "0019": [],
+        "e001": [
+            "d011"
+        ]
     },
     "ReadAttributesEp": [
         "01"
     ],
     "TUYA_REMOTE": true,
     "Type": "",
     "_comment": "Tuya 4 switch remote (Single, Double,Long press)",
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0046.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0046.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS004F.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992559523809524%*

 * *Differences: {"'Ep'": "{'01': {'e001': ''}}"}*

```diff
@@ -8,15 +8,16 @@
     "Ep": {
         "01": {
             "0000": "",
             "0001": "",
             "0006": "",
             "000a": "",
             "0019": "",
-            "Type": "Button_3"
+            "Type": "Button_3",
+            "e001": ""
         },
         "02": {
             "0006": "",
             "Type": "Button_3"
         },
         "03": {
             "0006": "",
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS004F.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.43116865773115776%*

 * *Differences: {"'ClusterToBind'": '[]',*

 * * "'Ep'": "{'01': {'Type': 'Vanne', '0004': '', '0005': '', '0102': OrderedDict([('Attributes', "*

 * *         "OrderedDict([('f002', OrderedDict([('Enabled', True), ('Name', 'Tuya_0102_f002'), "*

 * *         "('DataType', '20'), ('ActionList', ['check_store_value'])])), ('f003', "*

 * *         "OrderedDict([('Enabled', True), ('Name', 'Tuya_0102_f002'), ('DataType', '21'), "*

 * *         "('ActionList', ['check_store_value'])]))]))]), 'ee00': '', 'f001': '', 'f002': '', "*

 * *         "delete: ['0001' […]*

```diff
@@ -1,63 +1,71 @@
 {
-    "BatteryDevice": 1,
-    "BatteryPercentageConverter": 2,
-    "ClusterToBind": [
-        "0006"
-    ],
+    "ClusterToBind": [],
     "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
-            "0001": "",
+            "0004": "",
+            "0005": "",
             "0006": "",
-            "000a": "",
             "0019": "",
-            "Type": "Button_3",
-            "e001": ""
-        },
-        "02": {
-            "0006": "",
-            "Type": "Button_3"
-        },
-        "03": {
-            "0006": "",
-            "Type": "Button_3"
-        },
-        "04": {
-            "0006": "",
-            "Type": "Button_3"
+            "0102": {
+                "Attributes": {
+                    "f002": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "20",
+                        "Enabled": true,
+                        "Name": "Tuya_0102_f002"
+                    },
+                    "f003": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "21",
+                        "Enabled": true,
+                        "Name": "Tuya_0102_f002"
+                    }
+                }
+            },
+            "Type": "Vanne",
+            "ee00": "",
+            "f001": "",
+            "f002": ""
         }
     },
     "Param": {
-        "TS004FMode": "Scene"
+        "TuyaBackLight": 1,
+        "TuyaMotoReversal": 0,
+        "moesCalibrationTime": 200
     },
     "ReadAttributes": {
         "0000": [
-            "0004",
-            "0005",
             "0000",
             "0001",
+            "0002",
+            "0003",
+            "0004",
+            "0005",
             "0007",
-            "fffe"
-        ],
-        "0001": [
-            "0020",
-            "0021"
+            "ffe2"
         ],
         "0006": [
-            "0000",
-            "8004"
+            "8001",
+            "5000"
         ],
-        "0019": [],
-        "e001": [
-            "d011"
+        "0102": [
+            "0008",
+            "0017",
+            "f000",
+            "f001",
+            "f002",
+            "f003",
+            "8000",
+            "8001"
         ]
     },
-    "ReadAttributesEp": [
-        "01"
-    ],
-    "TUYA_REMOTE": true,
     "Type": "",
-    "_comment": "Tuya 4 switch remote (Single, Double,Long press)",
-    "_version": "Initial Version"
+    "_comment": "MOES Smart Curtain Switch Module",
+    "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0112.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0112.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0115.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0115.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-din.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-din.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F-plug.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F-plug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS011F.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS011F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0121.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0121.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0202.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4094618055555556%*

 * *Differences: {"'ClusterToBind'": "['0000', 'ef00']",*

 * * "'Ep'": "{'01': {'Type': 'LvlControl', '0004': '', 'ef00': '', '000a': '', '0019': '', delete: "*

 * *         "['0001', '0500']}}",*

 * * "'Identifier'": "[['TS0601', '_TZE200_whpb9yts'], ['TS0601', '_TZE200_ebwgzdqq'], ['TS0601', "*

 * *                 "'_TZE200_ctq0k47x'], ['TS0601', '_TZE200_9i9dt8is'], ['TS0601', "*

 * *                 "'_TZE200_dfxkcots'], ['TS0601', '_TZE200_w4cryh2i'], ['TS0601', "*

 * *                 "'_TZE200_ojzhk75b'], ['TS0601', '_TZE200_swaamsoy'], ['TS0601 […]*

```diff
@@ -1,44 +1,68 @@
 {
-    "BatteryDevice": 1,
-    "BatteryPercentageConverter": 2,
     "ClusterToBind": [
-        "0001",
-        "0500"
+        "0000",
+        "ef00"
     ],
     "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
-            "0001": "",
-            "0500": "",
-            "Type": "Motion/Tamper"
+            "0004": "",
+            "000a": "",
+            "0019": "",
+            "Type": "LvlControl",
+            "ef00": ""
         }
     },
-    "Param": {
-        "IASsensitivity": 1,
-        "MotionViaIASAlarm1": 1,
-        "TuyaPIRKeepTime": 1
-    },
+    "Identifier": [
+        [
+            "TS0601",
+            "_TZE200_whpb9yts"
+        ],
+        [
+            "TS0601",
+            "_TZE200_ebwgzdqq"
+        ],
+        [
+            "TS0601",
+            "_TZE200_ctq0k47x"
+        ],
+        [
+            "TS0601",
+            "_TZE200_9i9dt8is"
+        ],
+        [
+            "TS0601",
+            "_TZE200_dfxkcots"
+        ],
+        [
+            "TS0601",
+            "_TZE200_w4cryh2i"
+        ],
+        [
+            "TS0601",
+            "_TZE200_ojzhk75b"
+        ],
+        [
+            "TS0601",
+            "_TZE200_swaamsoy"
+        ],
+        [
+            "TS0601",
+            "_TZE200_3p5ydos3"
+        ]
+    ],
     "ReadAttributes": {
         "0000": [
             "0004",
-            "0005"
-        ],
-        "0001": [
-            "0020",
-            "0021"
-        ],
-        "0500": [
             "0000",
             "0001",
-            "0002",
-            "0010",
-            "0011",
-            "0013",
-            "f001"
+            "0005",
+            "0007"
         ]
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Tuya_ZM-35ZH-Q.html",
-    "_comment": "Tuya Motion Sensor IH012-RT01"
+    "_blakadder": "https://zigbee.blakadder.com/Eardatek_EDM-1ZBB-EU.html",
+    "_comment": "Tuya Smart Dimmer Switch",
+    "_version": "0.10"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0222.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0222.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0302.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3899857954545455%*

 * *Differences: {"'ClusterToBind'": "['0006']",*

 * * "'ConfigureReporting'": '{replace: OrderedDict()}',*

 * * "'Ep'": "{'01': {'0000': {replace: OrderedDict([('Attributes', OrderedDict([('fff0', "*

 * *         "OrderedDict([('Enabled', True), ('Name', 'Aqara_0000_fff0'), ('DataType', '42'), "*

 * *         "('ManufRawData', True), ('ManufSpecificFunc', 'Lumi_fcc0'), ('ActionList', "*

 * *         "['check_store_value'])])), ('ff01', OrderedDict([('Enabled', True), ('Name', "*

 * *         "'Aqara_0000_ff01'), ('DataType', '42'), ('ManufRawData', Tru […]*

```diff
@@ -1,56 +1,76 @@
 {
     "ClusterToBind": [
-        "0000",
-        "0102"
+        "0006"
     ],
-    "ConfigureReporting": {
-        "0102": {
-            "Attributes": {
-                "0008": {
-                    "Change": "01",
-                    "DataType": "20",
-                    "MaxInterval": "0384",
-                    "MinInterval": "0001",
-                    "TimeOut": "0000"
-                }
-            }
-        }
-    },
+    "ConfigureReporting": {},
     "Ep": {
         "01": {
-            "0000": "",
-            "0005": "",
-            "0019": "",
-            "0102": "",
-            "Type": "Venetian"
-        },
-        "f2": {
+            "0000": {
+                "Attributes": {
+                    "ff01": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff01"
+                    },
+                    "ff02": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "4c",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff02"
+                    },
+                    "fff0": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_fff0"
+                    }
+                }
+            },
             "Type": ""
+        },
+        "02": {
+            "0006": "",
+            "Type": "Switch"
+        },
+        "03": {
+            "0006": "",
+            "Type": "Switch"
         }
     },
-    "IgnoreWindowsCoverringValue50": 1,
     "Param": {},
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
             "0006",
-            "0007",
-            "000a",
-            "000f",
-            "0010",
-            "0015",
-            "f000"
+            "0032",
+            "0033",
+            "ff01"
+        ],
+        "0006": [
+            "0000"
         ],
-        "0019": [],
-        "0102": [
-            "0008"
-        ]
+        "0019": []
     },
     "Type": "",
-    "WindowsCoverringInverted": 1
+    "_blakadder": "https://zigbee.blakadder.com/Aqara_QBKG22LM.html",
+    "_comment": "D1 Wall Switch (No Neutral, Double Rocker) ( 2 Gang) ",
+    "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0502A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0502A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0505A.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0505A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0505B.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0505B.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-motion.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4198206018518518%*

 * *Differences: {"'BatteryDevice'": '1',*

 * * "'ClusterToBind'": '[]',*

 * * "'Ep'": "{'01': {'Type': 'Motion/Lux', '0005': '', '0500': '', delete: ['ef00']}}",*

 * * "'Identifier'": "{0: {insert: [(1, '_TZE200_bh3n6gk8')], delete: [1]}, 1: {insert: [(1, "*

 * *                 "'_TZE200_3towulqd')], delete: [1]}, 2: {insert: [(1, '_TZE200_1ibpyhdc')], "*

 * *                 'delete: [1]}, delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'Param'": "OrderedDict([('ZG204Z_MotionSensivity', 2), ('ZG204Z_MotionOccupancyTime', 0), "*

 * *            "('ForceIASRegistratio […]*

```diff
@@ -1,68 +1,76 @@
 {
-    "ClusterToBind": [
-        "0000",
-        "ef00"
-    ],
+    "BatteryDevice": 1,
+    "ClusterToBind": [],
     "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
             "0004": "",
+            "0005": "",
             "000a": "",
             "0019": "",
-            "Type": "LvlControl",
-            "ef00": ""
+            "0500": "",
+            "Type": "Motion/Lux"
         }
     },
     "Identifier": [
         [
             "TS0601",
-            "_TZE200_whpb9yts"
-        ],
-        [
-            "TS0601",
-            "_TZE200_ebwgzdqq"
-        ],
-        [
-            "TS0601",
-            "_TZE200_ctq0k47x"
-        ],
-        [
-            "TS0601",
-            "_TZE200_9i9dt8is"
-        ],
-        [
-            "TS0601",
-            "_TZE200_dfxkcots"
-        ],
-        [
-            "TS0601",
-            "_TZE200_w4cryh2i"
+            "_TZE200_bh3n6gk8"
         ],
         [
             "TS0601",
-            "_TZE200_ojzhk75b"
+            "_TZE200_3towulqd"
         ],
         [
             "TS0601",
-            "_TZE200_swaamsoy"
-        ],
-        [
-            "TS0601",
-            "_TZE200_3p5ydos3"
+            "_TZE200_1ibpyhdc"
         ]
     ],
+    "Param": {
+        "ForceIASRegistrationEp": "01",
+        "ZG204Z_MotionOccupancyTime": 0,
+        "ZG204Z_MotionSensivity": 2
+    },
     "ReadAttributes": {
         "0000": [
             "0004",
             "0000",
             "0001",
             "0005",
-            "0007"
-        ]
+            "0007",
+            "fffe"
+        ],
+        "0001": [],
+        "0019": [],
+        "0500": [
+            "0000",
+            "0001",
+            "0002",
+            "0010",
+            "0011"
+        ],
+        "ef00": []
+    },
+    "TS0601_DP": {
+        "01": {
+            "DomoDeviceFormat": "str",
+            "EvalExp": "int(value == 0)",
+            "sensor_type": "motion"
+        },
+        "04": {
+            "sensor_type": "battery"
+        },
+        "09": {
+            "store_tuya_attribute": "Sensitivity"
+        },
+        "0a": {
+            "store_tuya_attribute": "KeepTime"
+        },
+        "0c": {
+            "sensor_type": "illuminance"
+        }
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Eardatek_EDM-1ZBB-EU.html",
-    "_comment": "Tuya Smart Dimmer Switch",
-    "_version": "0.10"
+    "_comment": "Tuya Motion"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-motion.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.623983134920635%*

 * *Differences: {"'ClusterToBind'": "['0000']",*

 * * "'Ep'": "{'01': {'Type': 'Temp/Humi', delete: ['0500', '000a']}}",*

 * * "'Identifier'": "{0: {insert: [(1, '_TZE200_qoy0ekbd')], delete: [1]}, 1: {insert: [(1, "*

 * *                 "'_TZE200_znbl8dj5')], delete: [1]}, 2: {insert: [(1, '_TZE200_a8sdabtg')], "*

 * *                 'delete: [1]}}',*

 * * "'Param'": '{replace: OrderedDict()}',*

 * * "'ReadAttributes'": "{'0000': {insert: [(1, '0005'), (5, 'ffe2'), (6, 'ffe4'), (7, 'ffdf')], "*

 * *                     "delete: [3]}, delete: ['0001', '05 […]*

```diff
@@ -1,76 +1,73 @@
 {
     "BatteryDevice": 1,
-    "ClusterToBind": [],
+    "ClusterToBind": [
+        "0000"
+    ],
     "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
             "0004": "",
             "0005": "",
-            "000a": "",
             "0019": "",
-            "0500": "",
-            "Type": "Motion/Lux"
+            "Type": "Temp/Humi"
         }
     },
     "Identifier": [
         [
             "TS0601",
-            "_TZE200_bh3n6gk8"
+            "_TZE200_qoy0ekbd"
         ],
         [
             "TS0601",
-            "_TZE200_3towulqd"
+            "_TZE200_znbl8dj5"
         ],
         [
             "TS0601",
-            "_TZE200_1ibpyhdc"
+            "_TZE200_a8sdabtg"
         ]
     ],
-    "Param": {
-        "ForceIASRegistrationEp": "01",
-        "ZG204Z_MotionOccupancyTime": 0,
-        "ZG204Z_MotionSensivity": 2
-    },
+    "Param": {},
     "ReadAttributes": {
         "0000": [
             "0004",
+            "0005",
             "0000",
             "0001",
-            "0005",
             "0007",
+            "ffe2",
+            "ffe4",
+            "ffdf",
             "fffe"
         ],
-        "0001": [],
         "0019": [],
-        "0500": [
-            "0000",
-            "0001",
-            "0002",
-            "0010",
-            "0011"
-        ],
         "ef00": []
     },
     "TS0601_DP": {
         "01": {
-            "DomoDeviceFormat": "str",
-            "EvalExp": "int(value == 0)",
-            "sensor_type": "motion"
+            "EvalExp": "round(value/10,1)",
+            "sensor_type": "temperature"
+        },
+        "02": {
+            "sensor_type": "humidity"
         },
         "04": {
+            "EvalExp": "int(value/10)",
             "sensor_type": "battery"
         },
         "09": {
-            "store_tuya_attribute": "Sensitivity"
+            "store_tuya_attribute": "temperature_unit"
         },
-        "0a": {
-            "store_tuya_attribute": "KeepTime"
+        "17": {
+            "EvalExp": "int(value/10)",
+            "store_tuya_attribute": "temperature_calibration"
         },
-        "0c": {
-            "sensor_type": "illuminance"
+        "18": {
+            "store_tuya_attribute": "humidity_calibration"
         }
     },
     "Type": "",
-    "_comment": "Tuya Motion"
+    "_blakadder": "https://zigbee.blakadder.com/Tuya_ZG-227ZL.html",
+    "_comment": "Tuya Temp/Humi sensor with LCD",
+    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1561"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-radar.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-radar.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48806561085972855%*

 * *Differences: {"'ClusterToBind'": "['0006']",*

 * * "'Ep'": "{'01': {'0000': {replace: OrderedDict([('Attributes', OrderedDict([('fff0', "*

 * *         "OrderedDict([('Enabled', True), ('Name', 'Aqara_0000_fff0'), ('DataType', '42'), "*

 * *         "('ManufRawData', True), ('ManufSpecificFunc', 'Lumi_fcc0'), ('ActionList', "*

 * *         "['check_store_value'])])), ('ff01', OrderedDict([('Enabled', True), ('Name', "*

 * *         "'Aqara_0000_ff01'), ('DataType', '42'), ('ManufRawData', True), ('ManufSpecificFunc', "*

 * *         "'Lumi_fcc0'), ( […]*

```diff
@@ -1,73 +1,73 @@
 {
-    "BatteryDevice": 1,
     "ClusterToBind": [
-        "0000"
+        "0006"
     ],
     "ConfigureReporting": {},
     "Ep": {
         "01": {
-            "0000": "",
-            "0004": "",
-            "0005": "",
-            "0019": "",
-            "Type": "Temp/Humi"
+            "0000": {
+                "Attributes": {
+                    "ff01": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff01"
+                    },
+                    "ff02": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "4c",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff02"
+                    },
+                    "fff0": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_fff0"
+                    }
+                }
+            },
+            "Type": ""
+        },
+        "02": {
+            "0006": "",
+            "Type": "Switch"
         }
     },
-    "Identifier": [
-        [
-            "TS0601",
-            "_TZE200_qoy0ekbd"
-        ],
-        [
-            "TS0601",
-            "_TZE200_znbl8dj5"
-        ],
-        [
-            "TS0601",
-            "_TZE200_a8sdabtg"
-        ]
-    ],
     "Param": {},
     "ReadAttributes": {
         "0000": [
-            "0004",
-            "0005",
             "0000",
             "0001",
-            "0007",
-            "ffe2",
-            "ffe4",
-            "ffdf",
-            "fffe"
+            "0002",
+            "0003",
+            "0004",
+            "0005",
+            "0006",
+            "0032",
+            "0033",
+            "ff01"
         ],
-        "0019": [],
-        "ef00": []
-    },
-    "TS0601_DP": {
-        "01": {
-            "EvalExp": "round(value/10,1)",
-            "sensor_type": "temperature"
-        },
-        "02": {
-            "sensor_type": "humidity"
-        },
-        "04": {
-            "EvalExp": "int(value/10)",
-            "sensor_type": "battery"
-        },
-        "09": {
-            "store_tuya_attribute": "temperature_unit"
-        },
-        "17": {
-            "EvalExp": "int(value/10)",
-            "store_tuya_attribute": "temperature_calibration"
-        },
-        "18": {
-            "store_tuya_attribute": "humidity_calibration"
-        }
+        "0006": [
+            "0000"
+        ],
+        "0019": []
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Tuya_ZG-227ZL.html",
-    "_comment": "Tuya Temp/Humi sensor with LCD",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1561"
+    "_blakadder": "https://zigbee.blakadder.com/Aqara_QBKG21LM.html",
+    "_comment": "D1 Wall Switch (No Neutral, Single Rocker)",
+    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1585#issuecomment-1515294766",
+    "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS1001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS1001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'Ep'": "{'01': {'Type': 'Curtain'}}"}*

```diff
@@ -24,15 +24,15 @@
                         ],
                         "DataType": "21",
                         "Enabled": true,
                         "Name": "Tuya_0102_f002"
                     }
                 }
             },
-            "Type": "Vanne",
+            "Type": "Curtain",
             "ee00": "",
             "f001": "",
             "f002": ""
         }
     },
     "Param": {
         "TuyaBackLight": 1,
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7505050505050506%*

 * *Differences: {"'Ep'": "{'01': {'000a': '', delete: ['ee00', 'f001', 'f002']}, 'f2': OrderedDict([('0021', ''), "*

 * *         "('Type', '')])}",*

 * * "'Param'": "{'TuyaCurtainMode': 0, 'TuyaCalibrationTime': 600, delete: ['TuyaBackLight', "*

 * *            "'moesCalibrationTime']}",*

 * * "'ReadAttributes'": "{'0000': {insert: [(0, '0004'), (5, 'fffe')], delete: [7, 4, 3, 2]}}",*

 * * "'_comment'": "'Zigbee Curtain Module QS-Zigbee-CP03'",*

 * * "'_sponsorship'": "'Thanks to pacofrancisco'"}*

```diff
@@ -3,14 +3,15 @@
     "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
             "0004": "",
             "0005": "",
             "0006": "",
+            "000a": "",
             "0019": "",
             "0102": {
                 "Attributes": {
                     "f002": {
                         "ActionList": [
                             "check_store_value"
                         ],
@@ -24,35 +25,34 @@
                         ],
                         "DataType": "21",
                         "Enabled": true,
                         "Name": "Tuya_0102_f002"
                     }
                 }
             },
-            "Type": "Curtain",
-            "ee00": "",
-            "f001": "",
-            "f002": ""
+            "Type": "Curtain"
+        },
+        "f2": {
+            "0021": "",
+            "Type": ""
         }
     },
     "Param": {
-        "TuyaBackLight": 1,
-        "TuyaMotoReversal": 0,
-        "moesCalibrationTime": 200
+        "TuyaCalibrationTime": 600,
+        "TuyaCurtainMode": 0,
+        "TuyaMotoReversal": 0
     },
     "ReadAttributes": {
         "0000": [
+            "0004",
             "0000",
             "0001",
-            "0002",
-            "0003",
-            "0004",
             "0005",
             "0007",
-            "ffe2"
+            "fffe"
         ],
         "0006": [
             "8001",
             "5000"
         ],
         "0102": [
             "0008",
@@ -62,10 +62,11 @@
             "f002",
             "f003",
             "8000",
             "8001"
         ]
     },
     "Type": "",
-    "_comment": "MOES Smart Curtain Switch Module",
+    "_comment": "Zigbee Curtain Module QS-Zigbee-CP03",
+    "_sponsorship": "Thanks to pacofrancisco",
     "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Woolley/SA-029-1.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46654040404040403%*

 * *Differences: {"'ClusterToBind'": "['0006']",*

 * * "'ConfigureReporting'": "{replace: OrderedDict([('0006', OrderedDict([('Attributes', "*

 * *                         "OrderedDict([('0000', OrderedDict([('DataType', '10'), ('MinInterval', "*

 * *                         "'0001'), ('MaxInterval', '012C'), ('TimeOut', '0000'), ('Change', "*

 * *                         "'01')]))]))]))])}",*

 * * "'Ep'": "{'01': {'Type': 'Plug', '0003': '', 'fca0': '', 'fc57': '', delete: ['000a', '0102']}}",*

 * * "'ReadAttributes'": "{'0000': {insert: [(2, '0002'),  […]*

```diff
@@ -1,72 +1,60 @@
 {
-    "ClusterToBind": [],
-    "ConfigureReporting": {},
+    "ClusterToBind": [
+        "0006"
+    ],
+    "ConfigureReporting": {
+        "0006": {
+            "Attributes": {
+                "0000": {
+                    "Change": "01",
+                    "DataType": "10",
+                    "MaxInterval": "012C",
+                    "MinInterval": "0001",
+                    "TimeOut": "0000"
+                }
+            }
+        }
+    },
     "Ep": {
         "01": {
             "0000": "",
+            "0003": "",
             "0004": "",
             "0005": "",
             "0006": "",
-            "000a": "",
             "0019": "",
-            "0102": {
-                "Attributes": {
-                    "f002": {
-                        "ActionList": [
-                            "check_store_value"
-                        ],
-                        "DataType": "20",
-                        "Enabled": true,
-                        "Name": "Tuya_0102_f002"
-                    },
-                    "f003": {
-                        "ActionList": [
-                            "check_store_value"
-                        ],
-                        "DataType": "21",
-                        "Enabled": true,
-                        "Name": "Tuya_0102_f002"
-                    }
-                }
-            },
-            "Type": "Curtain"
+            "Type": "Plug",
+            "fc57": "",
+            "fca0": ""
         },
         "f2": {
             "0021": "",
             "Type": ""
         }
     },
-    "Param": {
-        "TuyaCalibrationTime": 600,
-        "TuyaCurtainMode": 0,
-        "TuyaMotoReversal": 0
-    },
     "ReadAttributes": {
         "0000": [
-            "0004",
             "0000",
             "0001",
+            "0002",
+            "0003",
+            "0004",
             "0005",
+            "0006",
             "0007",
-            "fffe"
+            "000a",
+            "4000"
         ],
         "0006": [
-            "8001",
-            "5000"
-        ],
-        "0102": [
-            "0008",
-            "0017",
-            "f000",
-            "f001",
-            "f002",
-            "f003",
-            "8000",
-            "8001"
+            "0000",
+            "4001",
+            "4002",
+            "4003"
         ]
     },
     "Type": "",
-    "_comment": "Zigbee Curtain Module QS-Zigbee-CP03",
-    "_sponsorship": "Thanks to pacofrancisco",
+    "_blakadder": "https://zigbee.blakadder.com/Wooley_SA-029.html",
+    "_comment": "Wooley Plug Smart Plug",
+    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1558",
     "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Tuya/TY0202.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Tuya/TY0202.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Woolley/SA-029-1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5460833333333334%*

 * *Differences: {"'ClusterToBind'": "{insert: [(1, '0008'), (2, '0300')]}",*

 * * "'ConfigureReporting'": "{'0008': OrderedDict([('Attributes', OrderedDict([('0000', "*

 * *                         "OrderedDict([('DataType', '20'), ('MinInterval', '0005'), "*

 * *                         "('MaxInterval', '012C'), ('TimeOut', '0000'), ('Change', '05')]))]))])}",*

 * * "'Ep'": "{'01': {'Type': 'ColorControlWW', '0008': '', '0300': '', '1000': '', 'fc82': '', "*

 * *         "delete: ['fca0', 'fc57']}, 'f2': {'0000': '', delete: ['Type']}}",*

 * * "'Param […]*

```diff
@@ -1,60 +1,88 @@
 {
     "ClusterToBind": [
-        "0006"
+        "0006",
+        "0008",
+        "0300"
     ],
     "ConfigureReporting": {
         "0006": {
             "Attributes": {
                 "0000": {
                     "Change": "01",
                     "DataType": "10",
                     "MaxInterval": "012C",
                     "MinInterval": "0001",
                     "TimeOut": "0000"
                 }
             }
+        },
+        "0008": {
+            "Attributes": {
+                "0000": {
+                    "Change": "05",
+                    "DataType": "20",
+                    "MaxInterval": "012C",
+                    "MinInterval": "0005",
+                    "TimeOut": "0000"
+                }
+            }
         }
     },
     "Ep": {
         "01": {
             "0000": "",
             "0003": "",
             "0004": "",
             "0005": "",
             "0006": "",
+            "0008": "",
             "0019": "",
-            "Type": "Plug",
-            "fc57": "",
-            "fca0": ""
+            "0300": "",
+            "1000": "",
+            "Type": "ColorControlWW",
+            "fc82": ""
         },
         "f2": {
-            "0021": "",
-            "Type": ""
+            "0000": "",
+            "0021": ""
         }
     },
+    "Param": {
+        "PowerOnAfterOffOn": 1,
+        "fadingOff": 0,
+        "moveToColourTemp": 0,
+        "moveToLevel": 0
+    },
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
             "0003",
             "0004",
             "0005",
             "0006",
-            "0007",
-            "000a",
-            "4000"
+            "0007"
         ],
         "0006": [
             "0000",
             "4001",
             "4002",
             "4003"
+        ],
+        "0008": [
+            "0000"
+        ],
+        "0019": [],
+        "0300": [
+            "0003",
+            "0004",
+            "0007",
+            "0008",
+            "400a"
         ]
     },
     "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Wooley_SA-029.html",
-    "_comment": "Wooley Plug Smart Plug",
-    "_source": "https://github.com/zigbeefordomoticz/Domoticz-Zigbee/issues/1558",
+    "_comment": "Smart Spot White Tones GU10 CCT",
     "_version": "1.0"
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.33352272727272725%*

 * *Differences: {"'ClusterToBind'": '[]',*

 * * "'ConfigureReporting'": '{replace: OrderedDict()}',*

 * * "'Ep'": "{'01': {'0000': {replace: OrderedDict([('Attributes', OrderedDict([('fff0', "*

 * *         "OrderedDict([('Enabled', True), ('Name', 'Aqara_0000_fff0'), ('DataType', '42'), "*

 * *         "('ManufRawData', True), ('ManufSpecificFunc', 'Lumi_fcc0'), ('ActionList', "*

 * *         "['check_store_value'])])), ('ff01', OrderedDict([('Enabled', True), ('Name', "*

 * *         "'Aqara_0000_ff01'), ('DataType', '42'), ('ManufRawData', True), (' […]*

```diff
@@ -1,81 +1,53 @@
 {
-    "ClusterToBind": [
-        "0006",
-        "0008",
-        "0300"
-    ],
-    "ConfigureReporting": {
-        "0006": {
-            "Attributes": {
-                "0000": {
-                    "Change": "01",
-                    "DataType": "10",
-                    "MaxInterval": "012C",
-                    "MinInterval": "0001",
-                    "TimeOut": "0000"
-                }
-            }
-        },
-        "0008": {
-            "Attributes": {
-                "0000": {
-                    "Change": "05",
-                    "DataType": "20",
-                    "MaxInterval": "012C",
-                    "MinInterval": "0005",
-                    "TimeOut": "0000"
-                }
-            }
-        }
-    },
+    "ClusterToBind": [],
+    "ConfigureReporting": {},
     "Ep": {
         "01": {
-            "0000": "",
-            "0003": "",
-            "0004": "",
-            "0005": "",
+            "0000": {
+                "Attributes": {
+                    "ff01": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff01"
+                    },
+                    "ff02": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "4c",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_ff02"
+                    },
+                    "fff0": {
+                        "ActionList": [
+                            "check_store_value"
+                        ],
+                        "DataType": "42",
+                        "Enabled": true,
+                        "ManufRawData": true,
+                        "ManufSpecificFunc": "Lumi_fcc0",
+                        "Name": "Aqara_0000_fff0"
+                    }
+                }
+            },
             "0006": "",
-            "0008": "",
-            "0019": "",
-            "0300": "",
-            "1000": "",
-            "Type": "ColorControlWW",
-            "fc82": ""
-        },
-        "f2": {
-            "0000": "",
-            "0021": ""
+            "Type": "SwitchAQ2WithOff"
         }
     },
-    "Param": {
-        "PowerOnAfterOffOn": 1,
-        "fadingOff": 0,
-        "moveToColourTemp": 0,
-        "moveToLevel": 0
-    },
+    "NoDeviceInterview": 1,
     "ReadAttributes": {
         "0000": [
-            "0000",
-            "0001",
-            "0002",
-            "0003",
             "0004",
-            "0005",
-            "0006",
-            "0007"
-        ],
-        "0006": [
-            "0000",
-            "4001",
-            "4002",
-            "4003"
+            "0005"
         ],
-        "0008": [
-            "0000"
-        ]
+        "0006": []
     },
-    "Type": "",
-    "_blakadder": "https://zigbee.blakadder.com/Ynoa_LA-GU10-CCT.html",
-    "_comment": "Smart Spot White Tones GU10 CCT",
-    "_version": "1.0"
+    "Type": ""
 }
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json` & `z4d-certified-devices-2.50/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices/__init__.py` & `z4d-certified-devices-2.50/z4d_certified_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices.egg-info/PKG-INFO` & `z4d-certified-devices-2.50/z4d_certified_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z4d-certified-devices
-Version: 2.49
+Version: 2.50
 Summary: "Certified devices for Zigbee for Domoticz plugin"
 Home-page: https://github.com/zigbeefordomoticz/z4d-certified-devices
 Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me"
 License: "GPL-3.0"
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `z4d-certified-devices-2.49/z4d_certified_devices.egg-info/SOURCES.txt` & `z4d-certified-devices-2.50/z4d_certified_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

