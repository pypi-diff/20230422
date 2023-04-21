# Comparing `tmp/cloudshell-snmp-5.0.0.zip` & `tmp/cloudshell-snmp-5.0.1.zip`

## zipinfo {}

```diff
@@ -1,117 +1,117 @@
-Zip file size: 145745 bytes, number of entries: 115
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/.tox/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/
--rw-r--r--  2.0 unx       58 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/MANIFEST.in
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/README.txt
--rw-r--r--  2.0 unx    11560 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/LICENSE
--rw-r--r--  2.0 unx     1068 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tox.ini
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/dev_requirements.txt
--rw-r--r--  2.0 unx      277 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/PKG-INFO
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/test_requirements.txt
--rw-r--r--  2.0 unx      855 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/setup.py
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/version.txt
--rw-r--r--  2.0 unx       52 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/third_party_requirements.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/setup.cfg
--rw-r--r--  2.0 unx       60 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/requirements.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     3574 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      277 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       59 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/top_level.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/configurator/
--rw-r--r--  2.0 unx     6347 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/test_snmp_context_manager.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/__init__.py
--rw-r--r--  2.0 unx     8054 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/test_snmp_parameters.py
--rw-r--r--  2.0 unx     4989 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/test_cloudshell_snmp.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/tools/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/domain/
--rw-r--r--  2.0 unx     3288 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/test_snmp_service.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/__init__.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/tools/__init__.py
--rw-r--r--  2.0 unx     2032 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_transport.py
--rw-r--r--  2.0 unx     2786 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_mib_builder.py
--rw-r--r--  2.0 unx     7478 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_json_mib.py
--rw-r--r--  2.0 unx     6670 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_json_mib_parser.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/domain/__init__.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_snmp_response.py
--rw-r--r--  2.0 unx     1245 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_json_type_record.py
--rw-r--r--  2.0 unx     1809 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_json_record.py
--rw-r--r--  2.0 unx     1614 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_quali_mib_table.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/configurator/__init__.py
--rw-r--r--  2.0 unx     6945 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/tests/snmp/configurator/test_snmp_configurator.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/.tox/build/
--rw-r--r--  2.0 unx      515 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/.tox/build/.tox-info.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/
--rw-r--r--  2.0 unx      778 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/types.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/__init__.py
--rw-r--r--  2.0 unx     5256 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/snmp_configurator.py
--rw-r--r--  2.0 unx     6863 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/snmp_parameters.py
--rw-r--r--  2.0 unx     2623 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/cloudshell_snmp.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/
--rw-r--r--  2.0 unx    14033 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_service.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_engine.py
--rw-r--r--  2.0 unx    12397 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_view_controller.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/__init__.py
--rw-r--r--  2.0 unx      375 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
--rw-r--r--  2.0 unx     1354 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_context_manager.py
--rw-r--r--  2.0 unx      349 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_errors.py
--rw-r--r--  2.0 unx     2549 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_mib_builder.py
--rw-r--r--  2.0 unx     8876 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_response_reader.py
--rw-r--r--  2.0 unx     1947 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/mib_builder_helper.py
--rw-r--r--  2.0 unx     1327 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_context.py
--rw-r--r--  2.0 unx    13419 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_json_mib.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/__init__.py
--rw-r--r--  2.0 unx     1297 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_security.py
--rw-r--r--  2.0 unx     2600 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_trasnport.py
--rw-r--r--  2.0 unx     1997 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_parameters_helper.py
--rw-r--r--  2.0 unx      992 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_constants.py
--rw-r--r--  2.0 unx     1385 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_json_record.py
--rw-r--r--  2.0 unx     2929 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_response.py
--rw-r--r--  2.0 unx     2501 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/quali_mib_table.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/__init__.py
--rw-r--r--  2.0 unx     4281 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_oid.py
--rw-r--r--  2.0 unx    42496 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/LLDP-MIB.json
--rw-r--r--  2.0 unx      611 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
--rw-r--r--  2.0 unx     6501 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
--rw-r--r--  2.0 unx    24494 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ENTITY-MIB.json
--rw-r--r--  2.0 unx   116385 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RMON2-MIB.json
--rw-r--r--  2.0 unx      386 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ASN1.py
--rw-r--r--  2.0 unx     4092 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMPv2-CONF.py
--rw-r--r--  2.0 unx    24807 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__init__.py
--rw-r--r--  2.0 unx    30835 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/EtherLike-MIB.json
--rw-r--r--  2.0 unx     7929 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
--rw-r--r--  2.0 unx     2597 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IPV6-TC.json
--rw-r--r--  2.0 unx    37281 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IF-MIB.json
--rw-r--r--  2.0 unx    90974 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RMON-MIB.json
--rw-r--r--  2.0 unx     3398 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-MIB.py
--rw-r--r--  2.0 unx     4368 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
--rw-r--r--  2.0 unx      162 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
--rw-r--r--  2.0 unx    34416 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IPV6-MIB.json
--rw-r--r--  2.0 unx    32561 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/BRIDGE-MIB.json
--rw-r--r--  2.0 unx    16818 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANA-MAU-MIB.json
--rw-r--r--  2.0 unx      416 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
--rw-r--r--  2.0 unx    59229 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
--rw-r--r--  2.0 unx    33327 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
--rw-r--r--  2.0 unx    42211 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
--rw-r--r--  2.0 unx     6071 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
--rw-r--r--  2.0 unx     7637 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__SNMPv2-MIB.py
--rw-r--r--  2.0 unx   110034 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IP-MIB.json
--rw-r--r--  2.0 unx    21756 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANAifType-MIB.json
--rw-r--r--  2.0 unx    23277 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMPv2-MIB.json
--rw-r--r--  2.0 unx    34783 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/MAU-MIB.json
--rw-r--r--  2.0 unx    67738 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RFC1271-MIB.json
--rw-r--r--  2.0 unx     2920 b- defN 23-Mar-22 21:24 cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
-115 files, 1057763 bytes uncompressed, 124399 bytes compressed:  88.2%
+Zip file size: 145763 bytes, number of entries: 115
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/.tox/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/
+-rw-r--r--  2.0 unx    11560 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/LICENSE
+-rw-r--r--  2.0 unx      277 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/PKG-INFO
+-rw-r--r--  2.0 unx     1068 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tox.ini
+-rw-r--r--  2.0 unx      855 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/setup.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/dev_requirements.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/setup.cfg
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/version.txt
+-rw-r--r--  2.0 unx       58 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/MANIFEST.in
+-rw-r--r--  2.0 unx       74 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/requirements.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/README.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/test_requirements.txt
+-rw-r--r--  2.0 unx       52 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/third_party_requirements.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/
+-rw-r--r--  2.0 unx      778 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/types.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/__init__.py
+-rw-r--r--  2.0 unx     2623 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/cloudshell_snmp.py
+-rw-r--r--  2.0 unx     5256 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_configurator.py
+-rw-r--r--  2.0 unx     6863 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_parameters.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/
+-rw-r--r--  2.0 unx      349 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_errors.py
+-rw-r--r--  2.0 unx      375 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
+-rw-r--r--  2.0 unx    12397 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_view_controller.py
+-rw-r--r--  2.0 unx     2549 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_mib_builder.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/__init__.py
+-rw-r--r--  2.0 unx     8876 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_response_reader.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_engine.py
+-rw-r--r--  2.0 unx     1354 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_context_manager.py
+-rw-r--r--  2.0 unx    14033 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_service.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/__init__.py
+-rw-r--r--  2.0 unx     2501 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/quali_mib_table.py
+-rw-r--r--  2.0 unx     4281 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_oid.py
+-rw-r--r--  2.0 unx     1385 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_json_record.py
+-rw-r--r--  2.0 unx     2929 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_response.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_parameters_helper.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_context.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_constants.py
+-rw-r--r--  2.0 unx     1947 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/mib_builder_helper.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/__init__.py
+-rw-r--r--  2.0 unx     1297 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_security.py
+-rw-r--r--  2.0 unx    13419 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib.py
+-rw-r--r--  2.0 unx     2600 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_trasnport.py
+-rw-r--r--  2.0 unx     1327 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
+-rw-r--r--  2.0 unx     2920 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
+-rw-r--r--  2.0 unx    37281 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IF-MIB.json
+-rw-r--r--  2.0 unx     7637 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__SNMPv2-MIB.py
+-rw-r--r--  2.0 unx     4368 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
+-rw-r--r--  2.0 unx      611 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
+-rw-r--r--  2.0 unx    30835 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/EtherLike-MIB.json
+-rw-r--r--  2.0 unx     2597 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-TC.json
+-rw-r--r--  2.0 unx     6071 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
+-rw-r--r--  2.0 unx      416 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
+-rw-r--r--  2.0 unx    24807 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
+-rw-r--r--  2.0 unx    21756 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANAifType-MIB.json
+-rw-r--r--  2.0 unx     7929 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
+-rw-r--r--  2.0 unx   116385 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON2-MIB.json
+-rw-r--r--  2.0 unx    34416 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-MIB.json
+-rw-r--r--  2.0 unx    32561 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/BRIDGE-MIB.json
+-rw-r--r--  2.0 unx    16818 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-MAU-MIB.json
+-rw-r--r--  2.0 unx    42496 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/LLDP-MIB.json
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__init__.py
+-rw-r--r--  2.0 unx    67738 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RFC1271-MIB.json
+-rw-r--r--  2.0 unx    42211 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
+-rw-r--r--  2.0 unx     3398 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-MIB.py
+-rw-r--r--  2.0 unx     6501 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
+-rw-r--r--  2.0 unx    90974 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON-MIB.json
+-rw-r--r--  2.0 unx    33327 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
+-rw-r--r--  2.0 unx    34783 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/MAU-MIB.json
+-rw-r--r--  2.0 unx     4092 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-CONF.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
+-rw-r--r--  2.0 unx   110034 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IP-MIB.json
+-rw-r--r--  2.0 unx    24494 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ENTITY-MIB.json
+-rw-r--r--  2.0 unx    59229 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
+-rw-r--r--  2.0 unx      386 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1.py
+-rw-r--r--  2.0 unx    23277 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-MIB.json
+-rw-r--r--  2.0 unx       73 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/requires.txt
+-rw-r--r--  2.0 unx      277 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     3574 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/.tox/build/
+-rw-r--r--  2.0 unx      515 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/.tox/build/.tox-info.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/
+-rw-r--r--  2.0 unx     8054 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/test_snmp_parameters.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/__init__.py
+-rw-r--r--  2.0 unx     6347 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/test_snmp_context_manager.py
+-rw-r--r--  2.0 unx     4989 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/test_cloudshell_snmp.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/__init__.py
+-rw-r--r--  2.0 unx     3288 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/test_snmp_service.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_snmp_response.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/__init__.py
+-rw-r--r--  2.0 unx     1809 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_record.py
+-rw-r--r--  2.0 unx     1245 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_type_record.py
+-rw-r--r--  2.0 unx     1614 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_quali_mib_table.py
+-rw-r--r--  2.0 unx     6670 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib_parser.py
+-rw-r--r--  2.0 unx     2786 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_mib_builder.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/__init__.py
+-rw-r--r--  2.0 unx     2032 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_transport.py
+-rw-r--r--  2.0 unx     7478 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib.py
+-rw-r--r--  2.0 unx     6945 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/__init__.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/test_snmp_configurator.py
+115 files, 1057791 bytes uncompressed, 124417 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -1,346 +1,346 @@
-Filename: cloudshell-snmp-5.0.0/
+Filename: cloudshell-snmp-5.0.1/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/
+Filename: cloudshell-snmp-5.0.1/cloudshell/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/
+Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/.tox/
+Filename: cloudshell-snmp-5.0.1/.tox/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/
+Filename: cloudshell-snmp-5.0.1/tests/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/MANIFEST.in
+Filename: cloudshell-snmp-5.0.1/LICENSE
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/README.txt
+Filename: cloudshell-snmp-5.0.1/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/LICENSE
+Filename: cloudshell-snmp-5.0.1/tox.ini
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tox.ini
+Filename: cloudshell-snmp-5.0.1/setup.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/dev_requirements.txt
+Filename: cloudshell-snmp-5.0.1/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/PKG-INFO
+Filename: cloudshell-snmp-5.0.1/setup.cfg
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/test_requirements.txt
+Filename: cloudshell-snmp-5.0.1/version.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/setup.py
+Filename: cloudshell-snmp-5.0.1/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/version.txt
+Filename: cloudshell-snmp-5.0.1/requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/third_party_requirements.txt
+Filename: cloudshell-snmp-5.0.1/README.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/setup.cfg
+Filename: cloudshell-snmp-5.0.1/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/requirements.txt
+Filename: cloudshell-snmp-5.0.1/third_party_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/dependency_links.txt
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/SOURCES.txt
+Filename: cloudshell-snmp-5.0.1/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/PKG-INFO
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/requires.txt
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/top_level.txt
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/types.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/cloudshell_snmp.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_configurator.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/configurator/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_parameters.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/test_snmp_context_manager.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/test_snmp_parameters.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_errors.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/test_cloudshell_snmp.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/tools/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_view_controller.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/domain/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_mib_builder.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/test_snmp_service.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_response_reader.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/tools/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_engine.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_transport.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_context_manager.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_mib_builder.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_service.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_json_mib.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_json_mib_parser.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/quali_mib_table.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/domain/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_oid.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_snmp_response.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_json_record.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_json_type_record.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_response.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_json_record.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_parameters_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_quali_mib_table.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_context.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/configurator/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/mib_builder_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/tests/snmp/configurator/test_snmp_configurator.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/.tox/build/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_security.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/.tox/build/.tox-info.json
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_trasnport.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IF-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/types.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__SNMPv2-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/snmp_configurator.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/snmp_parameters.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/EtherLike-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/cloudshell_snmp.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-TC.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_service.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_engine.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANAifType-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_view_controller.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON2-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_context_manager.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/BRIDGE-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_errors.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-MAU-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_mib_builder.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/LLDP-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_response_reader.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/mib_builder_helper.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RFC1271-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_context.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_json_mib.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_security.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_trasnport.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/MAU-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_parameters_helper.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-CONF.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_constants.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_json_record.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IP-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_response.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ENTITY-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/quali_mib_table.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/__init__.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_oid.py
+Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/LLDP-MIB.json
+Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
+Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
+Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ENTITY-MIB.json
+Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RMON2-MIB.json
+Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ASN1.py
+Filename: cloudshell-snmp-5.0.1/.tox/build/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMPv2-CONF.py
+Filename: cloudshell-snmp-5.0.1/.tox/build/.tox-info.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__init__.py
+Filename: cloudshell-snmp-5.0.1/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/EtherLike-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
+Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IPV6-TC.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/test_snmp_parameters.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IF-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RMON-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/test_snmp_context_manager.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-MIB.py
+Filename: cloudshell-snmp-5.0.1/tests/snmp/test_cloudshell_snmp.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IPV6-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/BRIDGE-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/test_snmp_service.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANA-MAU-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_snmp_response.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_record.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_type_record.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_quali_mib_table.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib_parser.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__SNMPv2-MIB.py
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_mib_builder.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IP-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANAifType-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_transport.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMPv2-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/MAU-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RFC1271-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
+Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/test_snmp_configurator.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-snmp-5.0.0/LICENSE` & `cloudshell-snmp-5.0.1/LICENSE`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tox.ini` & `cloudshell-snmp-5.0.1/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/setup.py` & `cloudshell-snmp-5.0.1/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell_snmp.egg-info/SOURCES.txt` & `cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/test_snmp_context_manager.py` & `cloudshell-snmp-5.0.1/tests/snmp/test_snmp_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/test_snmp_parameters.py` & `cloudshell-snmp-5.0.1/tests/snmp/test_snmp_parameters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/test_cloudshell_snmp.py` & `cloudshell-snmp-5.0.1/tests/snmp/test_cloudshell_snmp.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/test_snmp_service.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/test_snmp_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_transport.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_transport.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_mib_builder.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_mib_builder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_json_mib.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/tools/test_snmp_json_mib_parser.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_snmp_response.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_snmp_response.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_json_type_record.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_type_record.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_json_record.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_record.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/core/domain/test_quali_mib_table.py` & `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_quali_mib_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/configurator/test_enable_disable_snmp_configurator.py` & `cloudshell-snmp-5.0.1/tests/snmp/configurator/test_enable_disable_snmp_configurator.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/tests/snmp/configurator/test_snmp_configurator.py` & `cloudshell-snmp-5.0.1/tests/snmp/configurator/test_snmp_configurator.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/.tox/build/.tox-info.json` & `cloudshell-snmp-5.0.1/.tox/build/.tox-info.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'Python'": "{'virtualenv version': '20.22.0'}"}*

```diff
@@ -4,15 +4,15 @@
         "version_info": [
             3,
             9,
             16,
             "final",
             0
         ],
-        "virtualenv version": "20.21.0"
+        "virtualenv version": "20.22.0"
     },
     "PythonRun": {
         "deps": {
             "constraint_options": {
                 "constrain_package_deps": false,
                 "use_frozen_constraints": false
             },
```

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/types.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/types.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/snmp_configurator.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_configurator.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/snmp_parameters.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_parameters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/cloudshell_snmp.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/cloudshell_snmp.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_service.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_engine.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_engine.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_view_controller.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_view_controller.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_context_manager.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_mib_builder.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_mib_builder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/snmp_response_reader.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_response_reader.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/mib_builder_helper.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/mib_builder_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_json_mib_parser.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_context.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_context.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_json_mib.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_security.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_security.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_trasnport.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_trasnport.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_parameters_helper.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_parameters_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/tools/snmp_constants.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_constants.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_json_record.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_json_record.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_response.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_response.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/quali_mib_table.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/quali_mib_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/core/domain/snmp_oid.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_oid.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/LLDP-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/LLDP-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/ENTITY-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ENTITY-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RMON2-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON2-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMPv2-CONF.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-CONF.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/P-BRIDGE-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/P-BRIDGE-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/EtherLike-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/EtherLike-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IPV6-TC.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-TC.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IF-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IF-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RMON-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-MIB.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IPV6-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/BRIDGE-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/BRIDGE-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANA-MAU-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-MAU-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/__SNMPv2-MIB.py` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__SNMPv2-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IP-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IP-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANAifType-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANAifType-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/SNMPv2-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/MAU-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/MAU-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/RFC1271-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RFC1271-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.0/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json` & `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json`

 * *Files identical despite different names*

