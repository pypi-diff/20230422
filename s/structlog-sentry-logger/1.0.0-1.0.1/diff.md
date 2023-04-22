# Comparing `tmp/structlog_sentry_logger-1.0.0-cp39-cp39-win_amd64.whl.zip` & `tmp/structlog_sentry_logger-1.0.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 93469 bytes, number of entries: 14
+Zip file size: 93466 bytes, number of entries: 14
 -rw-r--r--  2.0 fat      454 b- defN 80-Jan-01 00:00 structlog_sentry_logger/__init__.py
 -rw-r--r--  2.0 fat    15788 b- defN 80-Jan-01 00:00 structlog_sentry_logger/_config.py
 -rw-r--r--  2.0 fat     3434 b- defN 80-Jan-01 00:00 structlog_sentry_logger/_feature_flags.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 structlog_sentry_logger/py.typed
 -rw-r--r--  2.0 fat     9632 b- defN 80-Jan-01 00:00 structlog_sentry_logger/structlog_sentry.py
 -rw-r--r--  2.0 fat   119296 b- defN 80-Jan-01 00:00 d4a104d1b860d1fab654__mypyc.cp38-win_amd64.pyd
 -rw-r--r--  2.0 fat    10752 b- defN 80-Jan-01 00:00 structlog_sentry_logger/__init__.cp38-win_amd64.pyd
 -rw-r--r--  2.0 fat    10752 b- defN 80-Jan-01 00:00 structlog_sentry_logger/_config.cp38-win_amd64.pyd
 -rw-r--r--  2.0 fat    10752 b- defN 80-Jan-01 00:00 structlog_sentry_logger/_feature_flags.cp38-win_amd64.pyd
 -rw-r--r--  2.0 fat    10752 b- defN 80-Jan-01 00:00 structlog_sentry_logger/structlog_sentry.cp38-win_amd64.pyd
--rw-r--r--  2.0 fat    11558 b- defN 80-Jan-01 00:00 structlog_sentry_logger-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 fat    20809 b- defN 80-Jan-01 00:00 structlog_sentry_logger-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 structlog_sentry_logger-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1381 b- defN 16-Jan-01 00:00 structlog_sentry_logger-1.0.0.dist-info/RECORD
-14 files, 225456 bytes uncompressed, 91115 bytes compressed:  59.6%
+-rw-r--r--  2.0 fat    11558 b- defN 80-Jan-01 00:00 structlog_sentry_logger-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 fat    20809 b- defN 80-Jan-01 00:00 structlog_sentry_logger-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 structlog_sentry_logger-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1381 b- defN 16-Jan-01 00:00 structlog_sentry_logger-1.0.1.dist-info/RECORD
+14 files, 225456 bytes uncompressed, 91112 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: structlog_sentry_logger/_feature_flags.cp38-win_amd64.pyd
 Comment: 
 
 Filename: structlog_sentry_logger/structlog_sentry.cp38-win_amd64.pyd
 Comment: 
 
-Filename: structlog_sentry_logger-1.0.0.dist-info/LICENSE
+Filename: structlog_sentry_logger-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: structlog_sentry_logger-1.0.0.dist-info/METADATA
+Filename: structlog_sentry_logger-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: structlog_sentry_logger-1.0.0.dist-info/WHEEL
+Filename: structlog_sentry_logger-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: structlog_sentry_logger-1.0.0.dist-info/RECORD
+Filename: structlog_sentry_logger-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `structlog_sentry_logger-1.0.0.dist-info/LICENSE` & `structlog_sentry_logger-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `structlog_sentry_logger-1.0.0.dist-info/METADATA` & `structlog_sentry_logger-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structlog-sentry-logger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Log without the setup via a pre-configured structlog logger with optional Sentry integration
 Home-page: https://github.com/TeoZosa/structlog-sentry-logger
 License: Apache-2.0
 Keywords: logging,structured,structure,log,structured logging,sentry,structlog,structlog-sentry
 Author: Teo Zosa
 Author-email: erinzosa@ucla.com
 Requires-Python: >=3.8,<3.12
@@ -28,15 +28,15 @@
 Provides-Extra: sentry
 Requires-Dist: colorama (>=0.4.3,<0.5.0) ; platform_system == "Windows"
 Requires-Dist: gitpython (>=3.1.7,<4.0.0)
 Requires-Dist: orjson (>=3.6.4,<4.0.0)
 Requires-Dist: python-dotenv (>=0.19)
 Requires-Dist: rich (>=10.12,<14.0)
 Requires-Dist: sentry-sdk (>0.17.0) ; extra == "sentry"
-Requires-Dist: structlog (>=21.1,<23.0)
+Requires-Dist: structlog (>=21.1,<24.0)
 Project-URL: Changelog, https://github.com/TeoZosa/structlog-sentry-logger/releases
 Project-URL: Repository, https://github.com/TeoZosa/structlog-sentry-logger
 Description-Content-Type: text/markdown
 
 Structlog-Sentry-Logger
 ==============================
 ![CI](https://github.com/TeoZosa/structlog-sentry-logger/workflows/CI/badge.svg)
```

## Comparing `structlog_sentry_logger-1.0.0.dist-info/RECORD` & `structlog_sentry_logger-1.0.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 structlog_sentry_logger/__init__.py,sha256=Pf1yBCoRBrn0rdsbdPUjE-yJp4EX6-tU8XO-BY5-YHY,454
 structlog_sentry_logger/_config.py,sha256=obRPzqoQX0urLuiWIq77IjAQJY-StAkk1nCMhEKBGGM,15788
 structlog_sentry_logger/_feature_flags.py,sha256=0aSGUR2oT6wnfTcn09BNggAgfFCgpG079mVGZuEswBk,3434
 structlog_sentry_logger/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 structlog_sentry_logger/structlog_sentry.py,sha256=LK4rVBUsM5BMO-0dUMkV5DjEEy2YmPolb_6ZHY8F9Cc,9632
-d4a104d1b860d1fab654__mypyc.cp38-win_amd64.pyd,sha256=9mWu9iF_2VO6Zais6-BtlhmRH_jr7b99n03mwXsXl24,119296
-structlog_sentry_logger/__init__.cp38-win_amd64.pyd,sha256=QuPzZvLaJKncR-gqSFVQQrouuJnl7gtWwgsoC8fozMA,10752
-structlog_sentry_logger/_config.cp38-win_amd64.pyd,sha256=6Cr2tTDrobcGT5U-gktSPD4tMGLZn1XBczz8dUmJ0Mg,10752
-structlog_sentry_logger/_feature_flags.cp38-win_amd64.pyd,sha256=DTBr6qjOBMXvxE2Qai0Pm8fu50wNvcjtJ_LwV_xQOwU,10752
-structlog_sentry_logger/structlog_sentry.cp38-win_amd64.pyd,sha256=974N7rJdEXLLT9nxY0b9J_Yz1_ngDyRmyrN0zVriXkg,10752
-structlog_sentry_logger-1.0.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-structlog_sentry_logger-1.0.0.dist-info/METADATA,sha256=YvftA4UhcJuQ5VkV-mbi9FdbleVrzQjAZarpuQlikqc,20809
-structlog_sentry_logger-1.0.0.dist-info/WHEEL,sha256=Ud29gZsZT-Ie5I5p1I_pDiLrTJI9uR7-nOCJlWJ3uA0,96
-structlog_sentry_logger-1.0.0.dist-info/RECORD,,
+d4a104d1b860d1fab654__mypyc.cp38-win_amd64.pyd,sha256=UTlGs-cHPcqk6dLUoxP1yKYJv_Ayyoc0ugE40bIsAos,119296
+structlog_sentry_logger/__init__.cp38-win_amd64.pyd,sha256=iPq8_BSPfiz8SScS2MpmSHg9uAmw2lmhJRo9oYkhXTI,10752
+structlog_sentry_logger/_config.cp38-win_amd64.pyd,sha256=daHQdJdcbzvglYwBmnaK_JvKAB4l_j0odxadpLA_bgQ,10752
+structlog_sentry_logger/_feature_flags.cp38-win_amd64.pyd,sha256=iugs8ZzJWN0SS2sYNTCPghi3rs0VD4WxxhhK874ViB4,10752
+structlog_sentry_logger/structlog_sentry.cp38-win_amd64.pyd,sha256=FDNaYDJ32RUwzzROSAUlMabmFgiLz7hXM_ENjKtLy6s,10752
+structlog_sentry_logger-1.0.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+structlog_sentry_logger-1.0.1.dist-info/METADATA,sha256=4err47UeCvf31mIQrJepFd56jnfGGxmogrhDcLF8W9g,20809
+structlog_sentry_logger-1.0.1.dist-info/WHEEL,sha256=Ud29gZsZT-Ie5I5p1I_pDiLrTJI9uR7-nOCJlWJ3uA0,96
+structlog_sentry_logger-1.0.1.dist-info/RECORD,,
```

