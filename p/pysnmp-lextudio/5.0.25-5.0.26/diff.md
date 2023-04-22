# Comparing `tmp/pysnmp_lextudio-5.0.25.tar.gz` & `tmp/pysnmp_lextudio-5.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnmp_lextudio-5.0.25.tar", max compression
+gzip compressed data, was "pysnmp_lextudio-5.0.26.tar", max compression
```

## Comparing `pysnmp_lextudio-5.0.25.tar` & `pysnmp_lextudio-5.0.26.tar`

### file list

```diff
@@ -1,322 +1,326 @@
--rw-r--r--   0        0        0     1386 2023-01-21 20:50:50.830634 pysnmp_lextudio-5.0.25/LICENSE.rst
--rw-r--r--   0        0        0     6508 2023-01-23 04:32:28.373749 pysnmp_lextudio-5.0.25/README.md
--rw-r--r--   0        0        0     7418 2022-11-10 07:54:24.451176 pysnmp_lextudio-5.0.25/docs/Makefile
--rw-r--r--   0        0        0      226 2022-11-10 07:54:24.451245 pysnmp_lextudio-5.0.25/docs/README.txt
--rw-r--r--   0        0        0     1670 2023-01-21 20:50:50.833766 pysnmp_lextudio-5.0.25/docs/mibs/PYSNMP-MIB.txt
--rw-r--r--   0        0        0     2774 2023-01-21 20:50:50.834272 pysnmp_lextudio-5.0.25/docs/mibs/PYSNMP-SOURCE-MIB.txt
--rw-r--r--   0        0        0     7084 2023-01-21 20:50:50.834777 pysnmp_lextudio-5.0.25/docs/mibs/PYSNMP-USM-MIB.txt
--rw-r--r--   0        0        0     1738 2022-11-10 07:54:24.451628 pysnmp_lextudio-5.0.25/docs/net-snmpd.conf
--rw-r--r--   0        0        0     2141 2022-11-10 07:54:24.451741 pysnmp_lextudio-5.0.25/docs/net-snmptrapd.conf
--rw-r--r--   0        0        0      232 2022-11-10 07:54:24.451936 pysnmp_lextudio-5.0.25/docs/source/.static/css/rtdimproved.css
--rw-r--r--   0        0        0     4030 2022-11-10 07:54:24.452014 pysnmp_lextudio-5.0.25/docs/source/.static/favicon.ico
--rw-r--r--   0        0        0    13811 2022-11-10 07:54:24.452123 pysnmp_lextudio-5.0.25/docs/source/.static/logo.svg
--rw-r--r--   0        0        0      557 2023-01-21 20:50:50.835204 pysnmp_lextudio-5.0.25/docs/source/.templates/layout.html
--rw-r--r--   0        0        0       54 2022-11-10 07:54:24.452185 pysnmp_lextudio-5.0.25/docs/source/changelog.rst
--rw-r--r--   0        0        0    10691 2023-01-27 01:01:10.253480 pysnmp_lextudio-5.0.25/docs/source/conf.py
--rw-r--r--   0        0        0     5167 2023-01-21 20:50:50.836511 pysnmp_lextudio-5.0.25/docs/source/development.rst
--rw-r--r--   0        0        0    10384 2023-01-21 20:50:50.837019 pysnmp_lextudio-5.0.25/docs/source/docs/api-reference.rst
--rw-r--r--   0        0        0      138 2022-11-10 08:01:10.001761 pysnmp_lextudio-5.0.25/docs/source/docs/hlapi/asyncio/agent/ntforg/notification.rst
--rw-r--r--   0        0        0      111 2022-11-10 08:01:10.001888 pysnmp_lextudio-5.0.25/docs/source/docs/hlapi/asyncio/manager/cmdgen/bulkcmd.rst
--rw-r--r--   0        0        0      102 2022-11-10 08:01:10.001957 pysnmp_lextudio-5.0.25/docs/source/docs/hlapi/asyncio/manager/cmdgen/getcmd.rst
--rw-r--r--   0        0        0      111 2022-11-10 08:01:10.002015 pysnmp_lextudio-5.0.25/docs/source/docs/hlapi/asyncio/manager/cmdgen/nextcmd.rst
--rw-r--r--   0        0        0      102 2022-11-10 08:01:10.002070 pysnmp_lextudio-5.0.25/docs/source/docs/hlapi/asyncio/manager/cmdgen/setcmd.rst
--rw-r--r--   0        0        0    28148 2022-11-10 07:54:24.456435 pysnmp_lextudio-5.0.25/docs/source/docs/mib-object-instances.svg
--rw-r--r--   0        0        0   134409 2022-11-10 07:54:24.457060 pysnmp_lextudio-5.0.25/docs/source/docs/nms-components.svg
--rw-r--r--   0        0        0    25840 2022-11-10 07:54:24.457265 pysnmp_lextudio-5.0.25/docs/source/docs/oid-tree-mibs.svg
--rw-r--r--   0        0        0    17023 2022-11-10 07:54:24.457488 pysnmp_lextudio-5.0.25/docs/source/docs/oid-tree.svg
--rw-r--r--   0        0        0     4749 2022-11-10 08:01:10.002236 pysnmp_lextudio-5.0.25/docs/source/docs/pysnmp-architecture.rst
--rw-r--r--   0        0        0    35260 2023-01-21 20:50:50.837684 pysnmp_lextudio-5.0.25/docs/source/docs/pysnmp-design.svg
--rw-r--r--   0        0        0    22937 2023-01-21 20:50:50.839506 pysnmp_lextudio-5.0.25/docs/source/docs/pysnmp-hlapi-tutorial.rst
--rw-r--r--   0        0        0    11023 2022-11-10 07:54:24.458530 pysnmp_lextudio-5.0.25/docs/source/docs/snmp-apps.svg
--rw-r--r--   0        0        0    10594 2023-01-21 20:50:50.840073 pysnmp_lextudio-5.0.25/docs/source/docs/snmp-design.rst
--rw-r--r--   0        0        0    19939 2022-11-10 07:54:24.458826 pysnmp_lextudio-5.0.25/docs/source/docs/snmp-engine.svg
--rw-r--r--   0        0        0     4748 2022-11-10 07:54:24.458954 pysnmp_lextudio-5.0.25/docs/source/docs/snmp-history.rst
--rw-r--r--   0        0        0      164 2022-11-10 08:01:10.003361 pysnmp_lextudio-5.0.25/docs/source/docs/tutorial.rst
--rw-r--r--   0        0        0     2292 2023-01-21 20:50:50.840602 pysnmp_lextudio-5.0.25/docs/source/download.rst
--rw-r--r--   0        0        0      537 2022-11-10 08:01:10.003968 pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst
--rw-r--r--   0        0        0      468 2022-11-10 08:01:10.004053 pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/agent/ntforg/common-notifications.rst
--rw-r--r--   0        0        0     2423 2023-01-21 20:50:50.840702 pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/index.rst
--rw-r--r--   0        0        0      960 2022-11-10 08:01:10.004282 pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst
--rw-r--r--   0        0        0      792 2022-11-10 08:01:10.004363 pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst
--rw-r--r--   0        0        0      467 2022-11-10 08:01:10.004435 pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/manager/cmdgen/walking-operations.rst
--rw-r--r--   0        0        0     4719 2023-01-21 20:50:50.841164 pysnmp_lextudio-5.0.25/docs/source/examples/index.rst
--rw-r--r--   0        0        0      745 2022-11-10 07:54:24.466971 pysnmp_lextudio-5.0.25/docs/source/examples/smi/agent/implementing-mib-objects.rst
--rw-r--r--   0        0        0     1184 2022-11-10 07:54:24.467088 pysnmp_lextudio-5.0.25/docs/source/examples/smi/manager/browsing-mib-tree.rst
--rw-r--r--   0        0        0      600 2022-11-10 07:54:24.467402 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst
--rw-r--r--   0        0        0      895 2022-11-10 07:54:24.467540 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst
--rw-r--r--   0        0        0      486 2022-11-10 07:54:24.467743 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/cmdgen/fetching-variables.rst
--rw-r--r--   0        0        0      455 2022-11-10 07:54:24.467818 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/cmdgen/modifying-variables.rst
--rw-r--r--   0        0        0      868 2022-11-10 07:54:24.467899 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst
--rw-r--r--   0        0        0      877 2022-11-10 07:54:24.468040 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst
--rw-r--r--   0        0        0      530 2022-11-10 07:54:24.468366 pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst
--rw-r--r--   0        0        0      483 2022-11-10 07:54:24.468931 pysnmp_lextudio-5.0.25/docs/source/examples/v3arch/asyncio/agent/cmdrsp/snmp-versions.rst
--rw-r--r--   0        0        0     1531 2023-01-21 20:50:50.841628 pysnmp_lextudio-5.0.25/docs/source/examples/v3arch/asyncio/index.rst
--rw-r--r--   0        0        0      482 2022-11-10 07:54:24.469199 pysnmp_lextudio-5.0.25/docs/source/examples/v3arch/asyncio/manager/ntfrcv/transport-tweaks.rst
--rw-r--r--   0        0        0     1410 2022-11-10 07:54:24.472768 pysnmp_lextudio-5.0.25/docs/source/faq/getting-peer-information.rst
--rw-r--r--   0        0        0     3823 2022-11-10 07:54:24.472856 pysnmp_lextudio-5.0.25/docs/source/faq/how-to-implement-agent-mib.rst
--rw-r--r--   0        0        0     3139 2023-01-23 07:07:30.039469 pysnmp_lextudio-5.0.25/docs/source/faq/ignored-snmp-packets.rst
--rw-r--r--   0        0        0     1224 2022-11-10 07:54:24.473003 pysnmp_lextudio-5.0.25/docs/source/faq/listening-on-multiple-interfaces.rst
--rw-r--r--   0        0        0     1016 2023-01-21 20:50:50.843902 pysnmp_lextudio-5.0.25/docs/source/faq/non-printable-snmp-values-apps.rst
--rw-r--r--   0        0        0     1538 2022-11-10 07:54:24.473152 pysnmp_lextudio-5.0.25/docs/source/faq/non-printable-snmp-values-tools.rst
--rw-r--r--   0        0        0     2004 2023-01-21 20:50:50.844674 pysnmp_lextudio-5.0.25/docs/source/faq/oids-not-increasing.rst
--rw-r--r--   0        0        0     1983 2023-01-21 20:50:50.845230 pysnmp_lextudio-5.0.25/docs/source/faq/pass-custom-mib-to-manager.rst
--rw-r--r--   0        0        0     1237 2022-11-10 07:54:24.473460 pysnmp_lextudio-5.0.25/docs/source/faq/py2exe-throws-error.rst
--rw-r--r--   0        0        0     1726 2022-11-10 07:54:24.473561 pysnmp_lextudio-5.0.25/docs/source/faq/response-values-mib-resolution.rst
--rw-r--r--   0        0        0     1596 2022-11-10 07:54:24.473654 pysnmp_lextudio-5.0.25/docs/source/faq/snmp-data-constraints-verification-failure.rst
--rw-r--r--   0        0        0      839 2022-11-10 07:54:24.473727 pysnmp_lextudio-5.0.25/docs/source/faq/walk-whole-mib.rst
--rw-r--r--   0        0        0      389 2023-01-21 20:50:50.843361 pysnmp_lextudio-5.0.25/docs/source/faq.rst
--rw-r--r--   0        0        0     3207 2023-01-21 20:50:50.849633 pysnmp_lextudio-5.0.25/docs/source/index.rst
--rw-r--r--   0        0        0       49 2022-11-10 07:54:24.473797 pysnmp_lextudio-5.0.25/docs/source/license.rst
--rw-r--r--   0        0        0      330 2023-01-21 20:50:50.850267 pysnmp_lextudio-5.0.25/docs/source/oldsite.rst
--rw-r--r--   0        0        0     1870 2023-01-21 20:50:50.852462 pysnmp_lextudio-5.0.25/docs/source/quick-start.rst
--rw-r--r--   0        0        0      363 2023-01-21 20:50:50.852549 pysnmp_lextudio-5.0.25/examples/README.md
--rw-r--r--   0        0        0     1338 2023-01-21 20:50:50.853342 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py
--rw-r--r--   0        0        0     1943 2023-01-21 20:50:50.855652 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py
--rw-r--r--   0        0        0     1304 2023-01-21 20:50:50.858767 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py
--rw-r--r--   0        0        0     1650 2023-01-24 18:28:40.573385 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py
--rw-r--r--   0        0        0     1558 2023-01-21 20:50:50.859916 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     1561 2023-01-24 18:28:33.036293 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py
--rw-r--r--   0        0        0     1728 2023-01-22 20:04:44.081851 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py
--rw-r--r--   0        0        0     1122 2023-01-27 00:57:26.068575 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v1-get.py
--rw-r--r--   0        0        0     1127 2023-01-27 00:58:39.314623 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v1-next.py
--rw-r--r--   0        0        0     1136 2023-01-27 00:58:46.679772 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v1-set.py
--rw-r--r--   0        0        0     1150 2023-01-27 00:59:31.743434 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-bulk.py
--rw-r--r--   0        0        0     1122 2023-01-25 01:17:53.010687 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-get.py
--rw-r--r--   0        0        0     1127 2023-01-25 01:38:53.802174 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-next.py
--rw-r--r--   0        0        0     1135 2023-01-25 01:38:31.015249 pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-set.py
--rw-r--r--   0        0        0     1603 2023-01-21 20:50:50.864540 pysnmp_lextudio-5.0.25/examples/smi/agent/custom-managed-object.py
--rw-r--r--   0        0        0     1747 2023-01-21 20:50:50.865413 pysnmp_lextudio-5.0.25/examples/smi/agent/operations-on-managed-objects.py
--rw-r--r--   0        0        0    17033 2023-01-21 20:50:50.867580 pysnmp_lextudio-5.0.25/examples/smi/manager/builder.py
--rw-r--r--   0        0        0     1340 2023-01-21 20:50:50.870440 pysnmp_lextudio-5.0.25/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py
--rw-r--r--   0        0        0     3811 2023-01-21 20:50:50.871036 pysnmp_lextudio-5.0.25/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py
--rw-r--r--   0        0        0     2619 2023-01-21 20:50:50.871359 pysnmp_lextudio-5.0.25/examples/smi/manager/mib-tree-inspection.py
--rw-r--r--   0        0        0     5171 2023-01-22 04:48:48.689957 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     2851 2023-01-21 20:50:50.873484 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     2408 2023-01-21 20:50:50.875755 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     3237 2023-01-21 20:50:50.875980 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py
--rw-r--r--   0        0        0     3228 2023-01-21 20:50:50.880172 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py
--rw-r--r--   0        0        0     3921 2023-01-21 20:50:50.884314 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py
--rw-r--r--   0        0        0     3473 2023-01-24 04:40:21.414174 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py
--rw-r--r--   0        0        0     3903 2023-01-22 20:28:04.985015 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py
--rw-r--r--   0        0        0     2766 2023-01-21 20:50:50.888466 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py
--rw-r--r--   0        0        0     3470 2023-01-21 20:50:50.888714 pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py
--rw-r--r--   0        0        0     2679 2023-01-21 20:50:50.888939 pysnmp_lextudio-5.0.25/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py
--rw-r--r--   0        0        0     2157 2023-01-21 20:50:50.889191 pysnmp_lextudio-5.0.25/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py
--rw-r--r--   0        0        0     2521 2023-01-21 20:50:50.889674 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py
--rw-r--r--   0        0        0     2466 2023-01-21 20:50:50.890099 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py
--rw-r--r--   0        0        0     1997 2023-01-21 20:50:50.890243 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py
--rw-r--r--   0        0        0     3605 2023-01-21 20:50:50.890416 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py
--rw-r--r--   0        0        0     2460 2023-01-21 20:50:50.890753 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py
--rw-r--r--   0        0        0     4321 2023-01-21 20:50:50.891063 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py
--rw-r--r--   0        0        0     2067 2023-01-21 20:50:50.891254 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py
--rw-r--r--   0        0        0     2092 2023-01-21 20:50:50.891466 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py
--rw-r--r--   0        0        0     3169 2023-01-21 20:50:50.891666 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py
--rw-r--r--   0        0        0     2201 2023-01-21 20:50:50.891850 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py
--rw-r--r--   0        0        0     3354 2023-01-21 20:50:50.892162 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py
--rw-r--r--   0        0        0     2716 2023-01-21 20:50:50.892315 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py
--rw-r--r--   0        0        0     3316 2023-01-21 20:50:50.892530 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py
--rw-r--r--   0        0        0     3885 2023-01-22 20:28:23.335266 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py
--rw-r--r--   0        0        0     2618 2023-01-22 20:28:24.764600 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py
--rw-r--r--   0        0        0     3569 2023-01-22 20:28:32.176159 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py
--rw-r--r--   0        0        0     3395 2023-01-22 20:28:34.071758 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     2654 2023-01-22 20:28:36.889141 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py
--rw-r--r--   0        0        0     3525 2023-01-22 20:28:42.553777 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py
--rw-r--r--   0        0        0     3030 2023-01-22 20:28:43.222139 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py
--rw-r--r--   0        0        0     3335 2023-01-22 20:28:50.206258 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v1-trap.py
--rw-r--r--   0        0        0     3317 2023-01-22 20:28:52.798993 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py
--rw-r--r--   0        0        0     3362 2023-01-22 20:28:55.662992 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py
--rw-r--r--   0        0        0     3225 2023-01-22 20:28:58.213864 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py
--rw-r--r--   0        0        0     2963 2023-01-22 20:29:00.009610 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v3-trap.py
--rw-r--r--   0        0        0     2510 2023-01-22 20:29:00.722369 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py
--rw-r--r--   0        0        0     2164 2023-01-22 20:29:01.530820 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py
--rw-r--r--   0        0        0     2300 2023-01-21 20:50:50.905007 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py
--rw-r--r--   0        0        0     2574 2023-01-22 20:29:02.196820 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py
--rw-r--r--   0        0        0     2370 2023-01-22 20:29:02.778380 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py
--rw-r--r--   0        0        0     3226 2023-01-22 20:29:03.553618 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py
--rw-r--r--   0        0        0     2423 2023-01-22 20:29:05.517253 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py
--rw-r--r--   0        0        0     3633 2023-01-22 20:29:09.200698 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py
--rw-r--r--   0        0        0     2443 2023-01-22 20:29:11.136296 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py
--rw-r--r--   0        0        0     2439 2023-01-22 20:29:12.968351 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py
--rw-r--r--   0        0        0     2438 2023-01-22 20:29:14.602400 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py
--rw-r--r--   0        0        0     3104 2023-01-22 20:29:15.912688 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py
--rw-r--r--   0        0        0     2232 2023-01-22 20:29:17.596770 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py
--rw-r--r--   0        0        0     2193 2023-01-22 20:29:19.130047 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py
--rw-r--r--   0        0        0     2089 2023-01-22 20:29:20.779591 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/v1-get.py
--rw-r--r--   0        0        0     2108 2023-01-22 20:29:22.210634 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py
--rw-r--r--   0        0        0     2217 2023-01-21 20:50:50.907479 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py
--rw-r--r--   0        0        0     2133 2023-01-21 20:50:50.907615 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py
--rw-r--r--   0        0        0     2131 2023-01-21 20:50:50.907763 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     3730 2023-01-21 20:50:50.907904 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py
--rw-r--r--   0        0        0     3315 2023-01-21 20:50:50.908143 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     3293 2023-01-21 20:50:50.908314 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py
--rw-r--r--   0        0        0     4030 2023-01-22 20:29:23.557359 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py
--rw-r--r--   0        0        0     3999 2023-01-22 20:29:25.197652 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py
--rw-r--r--   0        0        0     3982 2023-01-22 20:29:26.842129 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py
--rw-r--r--   0        0        0     4123 2023-01-22 20:29:28.426844 pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py
--rw-r--r--   0        0        0     1181 2023-01-27 01:01:05.722788 pysnmp_lextudio-5.0.25/pyproject.toml
--rw-r--r--   0        0        0      471 2023-01-27 01:01:14.523700 pysnmp_lextudio-5.0.25/pysnmp/__init__.py
--rw-r--r--   0        0        0     1252 2023-01-21 20:50:50.911870 pysnmp_lextudio-5.0.25/pysnmp/cache.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.495155 pysnmp_lextudio-5.0.25/pysnmp/carrier/__init__.py
--rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495252 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/__init__.py
--rw-r--r--   0        0        0     1857 2023-01-21 20:50:50.912293 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/base.py
--rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495435 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/__init__.py
--rw-r--r--   0        0        0     5316 2023-01-21 20:50:50.912624 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/base.py
--rw-r--r--   0        0        0     1994 2023-01-21 20:50:50.914278 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/udp.py
--rw-r--r--   0        0        0     1101 2023-01-21 20:50:50.914731 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/udp6.py
--rw-r--r--   0        0        0     3443 2023-01-21 20:50:50.916499 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dispatch.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.495867 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/__init__.py
--rw-r--r--   0        0        0     3335 2023-01-21 20:50:50.917864 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/base.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.496059 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/__init__.py
--rw-r--r--   0        0        0     7379 2023-01-21 20:50:50.919311 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/base.py
--rw-r--r--   0        0        0      584 2023-01-21 20:50:50.919596 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/udp.py
--rw-r--r--   0        0        0     1389 2023-01-21 20:50:50.919865 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/udp6.py
--rw-r--r--   0        0        0     1621 2023-01-21 20:50:50.920132 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/unix.py
--rw-r--r--   0        0        0     1734 2023-01-21 20:50:50.920446 pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dispatch.py
--rw-r--r--   0        0        0       59 2022-11-10 08:01:10.019074 pysnmp_lextudio-5.0.25/pysnmp/carrier/asynsock/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 08:01:10.019179 pysnmp_lextudio-5.0.25/pysnmp/carrier/asynsock/dgram/__init__.py
--rw-r--r--   0        0        0      208 2023-01-21 20:50:50.920759 pysnmp_lextudio-5.0.25/pysnmp/carrier/asynsock/dgram/udp.py
--rw-r--r--   0        0        0      209 2023-01-21 20:50:50.921023 pysnmp_lextudio-5.0.25/pysnmp/carrier/asynsock/dgram/udp6.py
--rw-r--r--   0        0        0      209 2023-01-21 20:50:50.921303 pysnmp_lextudio-5.0.25/pysnmp/carrier/asynsock/dgram/unix.py
--rw-r--r--   0        0        0      248 2023-01-21 20:50:50.921561 pysnmp_lextudio-5.0.25/pysnmp/carrier/asynsock/dispatch.py
--rw-r--r--   0        0        0     8140 2023-01-21 20:50:50.921848 pysnmp_lextudio-5.0.25/pysnmp/carrier/base.py
--rw-r--r--   0        0        0      235 2023-01-21 20:50:50.922097 pysnmp_lextudio-5.0.25/pysnmp/carrier/error.py
--rw-r--r--   0        0        0      676 2023-01-21 20:50:50.922367 pysnmp_lextudio-5.0.25/pysnmp/carrier/sockfix.py
--rw-r--r--   0        0        0     3558 2023-01-21 20:50:50.922632 pysnmp_lextudio-5.0.25/pysnmp/carrier/sockmsg.py
--rw-r--r--   0        0        0     3501 2023-01-21 20:50:50.922909 pysnmp_lextudio-5.0.25/pysnmp/debug.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.497717 pysnmp_lextudio-5.0.25/pysnmp/entity/__init__.py
--rw-r--r--   0        0        0    34968 2023-01-21 20:50:50.925478 pysnmp_lextudio-5.0.25/pysnmp/entity/config.py
--rw-r--r--   0        0        0     8176 2023-01-21 20:50:50.925875 pysnmp_lextudio-5.0.25/pysnmp/entity/engine.py
--rw-r--r--   0        0        0     2561 2023-01-21 20:50:50.927273 pysnmp_lextudio-5.0.25/pysnmp/entity/observer.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.498303 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/__init__.py
--rw-r--r--   0        0        0    18591 2023-01-21 20:50:50.927634 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/cmdgen.py
--rw-r--r--   0        0        0    14980 2023-01-21 20:50:50.927946 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/cmdrsp.py
--rw-r--r--   0        0        0    10212 2023-01-21 20:50:50.930359 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/config.py
--rw-r--r--   0        0        0     2623 2023-01-21 20:50:50.930748 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/context.py
--rw-r--r--   0        0        0     2855 2023-01-21 20:50:50.931078 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/mibvar.py
--rw-r--r--   0        0        0    17749 2023-01-21 20:50:50.931536 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/ntforg.py
--rw-r--r--   0        0        0     4532 2023-01-21 20:50:50.931830 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/ntfrcv.py
--rw-r--r--   0        0        0       59 2022-11-10 08:01:10.022472 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/oneliner/__init__.py
--rw-r--r--   0        0        0    10016 2023-01-21 20:50:50.932126 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/oneliner/cmdgen.py
--rw-r--r--   0        0        0     6644 2023-01-21 20:50:50.932396 pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/oneliner/ntforg.py
--rw-r--r--   0        0        0      501 2023-01-21 20:50:50.932669 pysnmp_lextudio-5.0.25/pysnmp/error.py
--rw-r--r--   0        0        0     3321 2023-01-21 20:50:50.932947 pysnmp_lextudio-5.0.25/pysnmp/hlapi/__init__.py
--rw-r--r--   0        0        0      459 2023-01-21 20:50:50.933233 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/__init__.py
--rw-r--r--   0        0        0    19830 2023-01-23 06:09:42.855989 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/cmdgen.py
--rw-r--r--   0        0        0     5525 2023-01-23 06:09:50.177751 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/ntforg.py
--rw-r--r--   0        0        0    13211 2023-01-25 01:36:58.327193 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/slim.py
--rw-r--r--   0        0        0     4976 2023-01-23 20:11:38.568253 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/transport.py
--rw-r--r--   0        0        0      462 2023-01-21 20:50:50.935912 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/__init__.py
--rw-r--r--   0        0        0    20298 2023-01-24 04:31:59.666586 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/cmdgen.py
--rw-r--r--   0        0        0     5202 2023-01-23 06:07:37.714838 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/ntforg.py
--rw-r--r--   0        0        0      624 2023-01-21 20:50:50.936686 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/__init__.py
--rw-r--r--   0        0        0    24567 2023-01-24 04:40:02.622854 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/cmdgen.py
--rw-r--r--   0        0        0       59 2022-11-10 08:01:10.023965 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/compat/__init__.py
--rw-r--r--   0        0        0     9212 2023-01-21 20:50:50.937282 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py
--rw-r--r--   0        0        0     1572 2023-01-21 20:50:50.937531 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/compat/ntforg.py
--rw-r--r--   0        0        0     4573 2023-01-23 06:09:47.723087 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/ntforg.py
--rw-r--r--   0        0        0     5124 2023-01-21 20:50:50.938011 pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/transport.py
--rw-r--r--   0        0        0    18218 2023-01-21 20:50:50.938431 pysnmp_lextudio-5.0.25/pysnmp/hlapi/auth.py
--rw-r--r--   0        0        0     2050 2023-01-21 20:50:50.938693 pysnmp_lextudio-5.0.25/pysnmp/hlapi/context.py
--rw-r--r--   0        0        0    11790 2023-01-21 20:50:50.938949 pysnmp_lextudio-5.0.25/pysnmp/hlapi/lcd.py
--rw-r--r--   0        0        0     1922 2023-01-21 20:50:50.939218 pysnmp_lextudio-5.0.25/pysnmp/hlapi/transport.py
--rw-r--r--   0        0        0     2920 2023-01-21 20:50:50.939457 pysnmp_lextudio-5.0.25/pysnmp/hlapi/varbinds.py
--rw-r--r--   0        0        0     1197 2023-01-21 20:50:50.939677 pysnmp_lextudio-5.0.25/pysnmp/nextid.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504675 pysnmp_lextudio-5.0.25/pysnmp/proto/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504925 pysnmp_lextudio-5.0.25/pysnmp/proto/acmod/__init__.py
--rw-r--r--   0        0        0    12323 2023-01-21 20:50:50.939958 pysnmp_lextudio-5.0.25/pysnmp/proto/acmod/rfc3415.py
--rw-r--r--   0        0        0      889 2023-01-21 20:50:50.940198 pysnmp_lextudio-5.0.25/pysnmp/proto/acmod/void.py
--rw-r--r--   0        0        0      371 2023-01-21 20:50:50.940472 pysnmp_lextudio-5.0.25/pysnmp/proto/api/__init__.py
--rw-r--r--   0        0        0     9391 2023-01-21 20:50:50.940745 pysnmp_lextudio-5.0.25/pysnmp/proto/api/v1.py
--rw-r--r--   0        0        0     5599 2023-01-21 20:50:50.940989 pysnmp_lextudio-5.0.25/pysnmp/proto/api/v2c.py
--rw-r--r--   0        0        0      926 2023-01-21 20:50:50.941214 pysnmp_lextudio-5.0.25/pysnmp/proto/api/verdec.py
--rw-r--r--   0        0        0     1151 2023-01-21 20:50:50.941430 pysnmp_lextudio-5.0.25/pysnmp/proto/cache.py
--rw-r--r--   0        0        0     5975 2023-01-21 20:50:50.941660 pysnmp_lextudio-5.0.25/pysnmp/proto/errind.py
--rw-r--r--   0        0        0     1191 2023-01-21 20:50:50.941881 pysnmp_lextudio-5.0.25/pysnmp/proto/error.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.507349 pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/__init__.py
--rw-r--r--   0        0        0     1754 2023-01-21 20:50:50.942134 pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/base.py
--rw-r--r--   0        0        0     3910 2023-01-21 20:50:50.942358 pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/cache.py
--rw-r--r--   0        0        0    20350 2023-01-21 20:50:50.942628 pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/rfc2576.py
--rw-r--r--   0        0        0    35109 2023-01-22 07:40:10.590039 pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/rfc3412.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.508803 pysnmp_lextudio-5.0.25/pysnmp/proto/proxy/__init__.py
--rw-r--r--   0        0        0     9874 2023-01-21 20:50:50.943242 pysnmp_lextudio-5.0.25/pysnmp/proto/proxy/rfc2576.py
--rw-r--r--   0        0        0     6085 2023-01-21 20:50:50.943486 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1155.py
--rw-r--r--   0        0        0     3323 2023-01-21 20:50:50.943726 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1157.py
--rw-r--r--   0        0        0      563 2023-01-21 20:50:50.943981 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1901.py
--rw-r--r--   0        0        0    21296 2023-01-21 20:50:50.944278 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1902.py
--rw-r--r--   0        0        0     5671 2023-01-21 20:50:50.944541 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1905.py
--rw-r--r--   0        0        0     1374 2023-01-21 20:50:50.944781 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc3411.py
--rw-r--r--   0        0        0    21759 2023-01-21 20:50:50.945141 pysnmp_lextudio-5.0.25/pysnmp/proto/rfc3412.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510738 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/__init__.py
--rw-r--r--   0        0        0     1485 2023-01-21 20:50:50.945499 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/base.py
--rw-r--r--   0        0        0      881 2023-01-21 20:50:50.945778 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/cache.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510991 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511096 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/__init__.py
--rw-r--r--   0        0        0     1030 2023-01-21 20:50:50.946099 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/aes192.py
--rw-r--r--   0        0        0      999 2023-01-21 20:50:50.946416 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/aes256.py
--rw-r--r--   0        0        0     3203 2023-01-21 20:50:50.946711 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/aesbase.py
--rw-r--r--   0        0        0     5231 2023-01-21 20:50:50.946982 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/des3.py
--rw-r--r--   0        0        0    21657 2023-01-22 01:10:54.940825 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc2576.py
--rw-r--r--   0        0        0      261 2023-01-21 20:50:50.947549 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511982 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/__init__.py
--rw-r--r--   0        0        0      850 2023-01-21 20:50:50.947795 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/base.py
--rw-r--r--   0        0        0     3709 2023-01-21 20:50:50.948046 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py
--rw-r--r--   0        0        0     3468 2023-01-21 20:50:50.948325 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py
--rw-r--r--   0        0        0      733 2023-01-22 19:49:47.441260 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/noauth.py
--rw-r--r--   0        0        0     2098 2023-01-21 20:50:50.949099 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/localkey.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.512518 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/__init__.py
--rw-r--r--   0        0        0      728 2023-01-21 20:50:50.951254 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/base.py
--rw-r--r--   0        0        0     4710 2023-01-21 20:50:50.951503 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/des.py
--rw-r--r--   0        0        0      807 2023-01-21 20:50:50.951774 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/nopriv.py
--rw-r--r--   0        0        0    56002 2023-01-22 20:02:41.908685 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/service.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513200 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3826/__init__.py
--rw-r--r--   0        0        0       59 2022-12-02 02:52:14.601095 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3826/priv/__init__.py
--rw-r--r--   0        0        0     4759 2023-01-21 20:50:50.953359 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3826/priv/aes.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513516 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc7860/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513622 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc7860/auth/__init__.py
--rw-r--r--   0        0        0     4037 2023-01-21 20:50:50.953621 pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513825 pysnmp_lextudio-5.0.25/pysnmp/smi/__init__.py
--rw-r--r--   0        0        0    16487 2023-01-21 20:50:50.953912 pysnmp_lextudio-5.0.25/pysnmp/smi/builder.py
--rw-r--r--   0        0        0     2326 2023-01-21 20:50:50.954158 pysnmp_lextudio-5.0.25/pysnmp/smi/compiler.py
--rw-r--r--   0        0        0     2351 2023-01-21 20:50:50.954423 pysnmp_lextudio-5.0.25/pysnmp/smi/error.py
--rw-r--r--   0        0        0      317 2023-01-21 20:50:50.954638 pysnmp_lextudio-5.0.25/pysnmp/smi/exval.py
--rw-r--r--   0        0        0     3084 2023-01-21 20:50:50.954871 pysnmp_lextudio-5.0.25/pysnmp/smi/indices.py
--rw-r--r--   0        0        0     9227 2023-01-21 20:50:50.955119 pysnmp_lextudio-5.0.25/pysnmp/smi/instrum.py
--rw-r--r--   0        0        0      283 2023-01-21 20:50:50.955343 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/ASN1-ENUMERATION.py
--rw-r--r--   0        0        0      534 2023-01-21 20:50:50.955553 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/ASN1-REFINEMENT.py
--rw-r--r--   0        0        0      505 2023-01-21 20:50:50.955778 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/ASN1.py
--rw-r--r--   0        0        0    17614 2023-01-21 20:50:50.957301 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/INET-ADDRESS-MIB.py
--rw-r--r--   0        0        0     3591 2023-01-21 20:50:50.957643 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/PYSNMP-MIB.py
--rw-r--r--   0        0        0     4620 2023-01-21 20:50:50.957971 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py
--rw-r--r--   0        0        0     9922 2023-01-21 20:50:50.958209 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/PYSNMP-USM-MIB.py
--rw-r--r--   0        0        0     1318 2023-01-21 20:50:50.958608 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/RFC1158-MIB.py
--rw-r--r--   0        0        0    56809 2023-01-21 20:50:50.959093 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/RFC1213-MIB.py
--rw-r--r--   0        0        0    17437 2023-01-21 20:50:50.959514 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py
--rw-r--r--   0        0        0    18836 2023-01-21 20:50:50.961309 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py
--rw-r--r--   0        0        0     5882 2023-01-21 20:50:50.961679 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-MPD-MIB.py
--rw-r--r--   0        0        0    19031 2023-01-21 20:50:50.962008 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py
--rw-r--r--   0        0        0    10138 2023-01-21 20:50:50.962396 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-PROXY-MIB.py
--rw-r--r--   0        0        0    24833 2023-01-21 20:50:50.962836 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-TARGET-MIB.py
--rw-r--r--   0        0        0     3913 2023-01-21 20:50:50.963197 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py
--rw-r--r--   0        0        0    33731 2023-01-21 20:50:50.963774 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py
--rw-r--r--   0        0        0     3572 2023-01-21 20:50:50.964077 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py
--rw-r--r--   0        0        0     5841 2023-01-21 20:50:50.964367 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py
--rw-r--r--   0        0        0    30173 2023-01-21 20:50:50.964903 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py
--rw-r--r--   0        0        0     4096 2023-01-21 20:50:50.965255 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-CONF.py
--rw-r--r--   0        0        0    31135 2023-01-21 20:50:50.965742 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-MIB.py
--rw-r--r--   0        0        0    46776 2023-01-21 20:50:50.966284 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-SMI.py
--rw-r--r--   0        0        0    28986 2023-01-21 20:50:50.966685 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-TC.py
--rw-r--r--   0        0        0     6921 2023-01-21 20:50:50.967022 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-TM.py
--rw-r--r--   0        0        0    24370 2023-01-21 20:50:50.967422 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.522800 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/__init__.py
--rw-r--r--   0        0        0      926 2023-01-21 20:50:50.967752 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py
--rw-r--r--   0        0        0     1174 2023-01-21 20:50:50.968042 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py
--rw-r--r--   0        0        0     1047 2023-01-21 20:50:50.968298 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py
--rw-r--r--   0        0        0     1046 2023-01-21 20:50:50.968546 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py
--rw-r--r--   0        0        0     2232 2023-01-21 20:50:50.968782 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py
--rw-r--r--   0        0        0      530 2023-01-21 20:50:50.969033 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py
--rw-r--r--   0        0        0     7605 2023-01-21 20:50:50.969323 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.523596 pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__init__.py
--rw-r--r--   0        0        0    44735 2023-01-21 20:50:50.971471 pysnmp_lextudio-5.0.25/pysnmp/smi/rfc1902.py
--rw-r--r--   0        0        0    12218 2023-01-21 20:50:50.971883 pysnmp_lextudio-5.0.25/pysnmp/smi/view.py
--rw-r--r--   0        0        0     8273 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.25/setup.py
--rw-r--r--   0        0        0     7809 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.25/PKG-INFO
+-rw-r--r--   0        0        0     1386 2023-01-21 20:50:50.830634 pysnmp_lextudio-5.0.26/LICENSE.rst
+-rw-r--r--   0        0        0     6508 2023-04-21 00:52:22.285829 pysnmp_lextudio-5.0.26/README.md
+-rw-r--r--   0        0        0     7418 2022-11-10 07:54:24.451176 pysnmp_lextudio-5.0.26/docs/Makefile
+-rw-r--r--   0        0        0      226 2022-11-10 07:54:24.451245 pysnmp_lextudio-5.0.26/docs/README.txt
+-rw-r--r--   0        0        0     1670 2023-01-21 20:50:50.833766 pysnmp_lextudio-5.0.26/docs/mibs/PYSNMP-MIB.txt
+-rw-r--r--   0        0        0     2774 2023-01-21 20:50:50.834272 pysnmp_lextudio-5.0.26/docs/mibs/PYSNMP-SOURCE-MIB.txt
+-rw-r--r--   0        0        0     7084 2023-02-26 23:53:14.445656 pysnmp_lextudio-5.0.26/docs/mibs/PYSNMP-USM-MIB.txt
+-rw-r--r--   0        0        0     1738 2022-11-10 07:54:24.451628 pysnmp_lextudio-5.0.26/docs/net-snmpd.conf
+-rw-r--r--   0        0        0     2141 2022-11-10 07:54:24.451741 pysnmp_lextudio-5.0.26/docs/net-snmptrapd.conf
+-rw-r--r--   0        0        0      232 2022-11-10 07:54:24.451936 pysnmp_lextudio-5.0.26/docs/source/.static/css/rtdimproved.css
+-rw-r--r--   0        0        0     4030 2022-11-10 07:54:24.452014 pysnmp_lextudio-5.0.26/docs/source/.static/favicon.ico
+-rw-r--r--   0        0        0      143 2023-01-29 09:26:05.471724 pysnmp_lextudio-5.0.26/docs/source/.static/google_analytics_tracker.js
+-rw-r--r--   0        0        0    13811 2022-11-10 07:54:24.452123 pysnmp_lextudio-5.0.26/docs/source/.static/logo.svg
+-rw-r--r--   0        0        0      557 2023-01-21 20:50:50.835204 pysnmp_lextudio-5.0.26/docs/source/.templates/layout.html
+-rw-r--r--   0        0        0      558 2023-01-29 09:29:30.479143 pysnmp_lextudio-5.0.26/docs/source/.templates/sourcelink.html
+-rw-r--r--   0        0        0       54 2022-11-10 07:54:24.452185 pysnmp_lextudio-5.0.26/docs/source/changelog.rst
+-rw-r--r--   0        0        0    10773 2023-04-22 01:39:38.248895 pysnmp_lextudio-5.0.26/docs/source/conf.py
+-rw-r--r--   0        0        0     5167 2023-01-21 20:50:50.836511 pysnmp_lextudio-5.0.26/docs/source/development.rst
+-rw-r--r--   0        0        0     9568 2023-01-28 08:01:44.614630 pysnmp_lextudio-5.0.26/docs/source/docs/api-reference.rst
+-rw-r--r--   0        0        0      138 2022-11-10 08:01:10.001761 pysnmp_lextudio-5.0.26/docs/source/docs/hlapi/asyncio/agent/ntforg/notification.rst
+-rw-r--r--   0        0        0      111 2022-11-10 08:01:10.001888 pysnmp_lextudio-5.0.26/docs/source/docs/hlapi/asyncio/manager/cmdgen/bulkcmd.rst
+-rw-r--r--   0        0        0      102 2022-11-10 08:01:10.001957 pysnmp_lextudio-5.0.26/docs/source/docs/hlapi/asyncio/manager/cmdgen/getcmd.rst
+-rw-r--r--   0        0        0      111 2022-11-10 08:01:10.002015 pysnmp_lextudio-5.0.26/docs/source/docs/hlapi/asyncio/manager/cmdgen/nextcmd.rst
+-rw-r--r--   0        0        0      102 2022-11-10 08:01:10.002070 pysnmp_lextudio-5.0.26/docs/source/docs/hlapi/asyncio/manager/cmdgen/setcmd.rst
+-rw-r--r--   0        0        0    28148 2022-11-10 07:54:24.456435 pysnmp_lextudio-5.0.26/docs/source/docs/mib-object-instances.svg
+-rw-r--r--   0        0        0   134409 2022-11-10 07:54:24.457060 pysnmp_lextudio-5.0.26/docs/source/docs/nms-components.svg
+-rw-r--r--   0        0        0    25840 2022-11-10 07:54:24.457265 pysnmp_lextudio-5.0.26/docs/source/docs/oid-tree-mibs.svg
+-rw-r--r--   0        0        0    17023 2022-11-10 07:54:24.457488 pysnmp_lextudio-5.0.26/docs/source/docs/oid-tree.svg
+-rw-r--r--   0        0        0     4749 2022-11-10 08:01:10.002236 pysnmp_lextudio-5.0.26/docs/source/docs/pysnmp-architecture.rst
+-rw-r--r--   0        0        0    35260 2023-01-21 20:50:50.837684 pysnmp_lextudio-5.0.26/docs/source/docs/pysnmp-design.svg
+-rw-r--r--   0        0        0    22937 2023-04-21 00:52:22.286522 pysnmp_lextudio-5.0.26/docs/source/docs/pysnmp-hlapi-tutorial.rst
+-rw-r--r--   0        0        0    11023 2022-11-10 07:54:24.458530 pysnmp_lextudio-5.0.26/docs/source/docs/snmp-apps.svg
+-rw-r--r--   0        0        0    10594 2023-01-21 20:50:50.840073 pysnmp_lextudio-5.0.26/docs/source/docs/snmp-design.rst
+-rw-r--r--   0        0        0    19939 2022-11-10 07:54:24.458826 pysnmp_lextudio-5.0.26/docs/source/docs/snmp-engine.svg
+-rw-r--r--   0        0        0     4748 2022-11-10 07:54:24.458954 pysnmp_lextudio-5.0.26/docs/source/docs/snmp-history.rst
+-rw-r--r--   0        0        0      164 2022-11-10 08:01:10.003361 pysnmp_lextudio-5.0.26/docs/source/docs/tutorial.rst
+-rw-r--r--   0        0        0     2292 2023-01-21 20:50:50.840602 pysnmp_lextudio-5.0.26/docs/source/download.rst
+-rw-r--r--   0        0        0      537 2022-11-10 08:01:10.003968 pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst
+-rw-r--r--   0        0        0      468 2022-11-10 08:01:10.004053 pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/agent/ntforg/common-notifications.rst
+-rw-r--r--   0        0        0     2423 2023-04-21 00:52:22.286962 pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/index.rst
+-rw-r--r--   0        0        0      960 2022-11-10 08:01:10.004282 pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst
+-rw-r--r--   0        0        0      792 2022-11-10 08:01:10.004363 pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst
+-rw-r--r--   0        0        0      467 2022-11-10 08:01:10.004435 pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/manager/cmdgen/walking-operations.rst
+-rw-r--r--   0        0        0     4719 2023-04-21 00:52:22.288740 pysnmp_lextudio-5.0.26/docs/source/examples/index.rst
+-rw-r--r--   0        0        0      745 2022-11-10 07:54:24.466971 pysnmp_lextudio-5.0.26/docs/source/examples/smi/agent/implementing-mib-objects.rst
+-rw-r--r--   0        0        0     1184 2022-11-10 07:54:24.467088 pysnmp_lextudio-5.0.26/docs/source/examples/smi/manager/browsing-mib-tree.rst
+-rw-r--r--   0        0        0      600 2023-04-21 00:52:22.289077 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst
+-rw-r--r--   0        0        0      895 2023-04-21 00:52:22.289192 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst
+-rw-r--r--   0        0        0      486 2023-04-21 00:52:22.289317 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/cmdgen/fetching-variables.rst
+-rw-r--r--   0        0        0      455 2023-04-21 00:52:22.289376 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/cmdgen/modifying-variables.rst
+-rw-r--r--   0        0        0      868 2023-04-21 00:52:22.289431 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst
+-rw-r--r--   0        0        0      877 2023-04-21 00:52:22.289507 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst
+-rw-r--r--   0        0        0      530 2023-04-21 00:52:22.289594 pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst
+-rw-r--r--   0        0        0      483 2022-11-10 07:54:24.468931 pysnmp_lextudio-5.0.26/docs/source/examples/v3arch/asyncio/agent/cmdrsp/snmp-versions.rst
+-rw-r--r--   0        0        0     1531 2023-01-21 20:50:50.841628 pysnmp_lextudio-5.0.26/docs/source/examples/v3arch/asyncio/index.rst
+-rw-r--r--   0        0        0      482 2022-11-10 07:54:24.469199 pysnmp_lextudio-5.0.26/docs/source/examples/v3arch/asyncio/manager/ntfrcv/transport-tweaks.rst
+-rw-r--r--   0        0        0     1410 2022-11-10 07:54:24.472768 pysnmp_lextudio-5.0.26/docs/source/faq/getting-peer-information.rst
+-rw-r--r--   0        0        0     3823 2022-11-10 07:54:24.472856 pysnmp_lextudio-5.0.26/docs/source/faq/how-to-implement-agent-mib.rst
+-rw-r--r--   0        0        0     3139 2023-01-23 07:07:30.039469 pysnmp_lextudio-5.0.26/docs/source/faq/ignored-snmp-packets.rst
+-rw-r--r--   0        0        0     1224 2022-11-10 07:54:24.473003 pysnmp_lextudio-5.0.26/docs/source/faq/listening-on-multiple-interfaces.rst
+-rw-r--r--   0        0        0     1016 2023-01-21 20:50:50.843902 pysnmp_lextudio-5.0.26/docs/source/faq/non-printable-snmp-values-apps.rst
+-rw-r--r--   0        0        0     1538 2022-11-10 07:54:24.473152 pysnmp_lextudio-5.0.26/docs/source/faq/non-printable-snmp-values-tools.rst
+-rw-r--r--   0        0        0     2004 2023-01-21 20:50:50.844674 pysnmp_lextudio-5.0.26/docs/source/faq/oids-not-increasing.rst
+-rw-r--r--   0        0        0     1983 2023-01-21 20:50:50.845230 pysnmp_lextudio-5.0.26/docs/source/faq/pass-custom-mib-to-manager.rst
+-rw-r--r--   0        0        0     1237 2022-11-10 07:54:24.473460 pysnmp_lextudio-5.0.26/docs/source/faq/py2exe-throws-error.rst
+-rw-r--r--   0        0        0     1726 2022-11-10 07:54:24.473561 pysnmp_lextudio-5.0.26/docs/source/faq/response-values-mib-resolution.rst
+-rw-r--r--   0        0        0     1596 2022-11-10 07:54:24.473654 pysnmp_lextudio-5.0.26/docs/source/faq/snmp-data-constraints-verification-failure.rst
+-rw-r--r--   0        0        0      839 2022-11-10 07:54:24.473727 pysnmp_lextudio-5.0.26/docs/source/faq/walk-whole-mib.rst
+-rw-r--r--   0        0        0      389 2023-01-21 20:50:50.843361 pysnmp_lextudio-5.0.26/docs/source/faq.rst
+-rw-r--r--   0        0        0     3207 2023-01-21 20:50:50.849633 pysnmp_lextudio-5.0.26/docs/source/index.rst
+-rw-r--r--   0        0        0       49 2022-11-10 07:54:24.473797 pysnmp_lextudio-5.0.26/docs/source/license.rst
+-rw-r--r--   0        0        0      330 2023-01-21 20:50:50.850267 pysnmp_lextudio-5.0.26/docs/source/oldsite.rst
+-rw-r--r--   0        0        0     1871 2023-01-28 05:36:25.676602 pysnmp_lextudio-5.0.26/docs/source/quick-start.rst
+-rw-r--r--   0        0        0      363 2023-01-21 20:50:50.852549 pysnmp_lextudio-5.0.26/examples/README.md
+-rw-r--r--   0        0        0     1336 2023-01-28 02:10:04.207146 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py
+-rw-r--r--   0        0        0     1941 2023-01-28 02:10:04.207497 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py
+-rw-r--r--   0        0        0     1581 2023-01-28 08:09:49.565481 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/agent/ntforg/v3-inform.py
+-rw-r--r--   0        0        0     1304 2023-01-21 20:50:50.858767 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py
+-rw-r--r--   0        0        0     1648 2023-01-28 02:10:04.207259 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py
+-rw-r--r--   0        0        0     1556 2023-01-28 02:10:04.207201 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     1559 2023-01-28 02:10:04.207244 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py
+-rw-r--r--   0        0        0     1728 2023-04-21 00:52:22.290304 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py
+-rw-r--r--   0        0        0     1120 2023-01-28 02:10:04.207716 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v1-get.py
+-rw-r--r--   0        0        0     1125 2023-01-28 02:10:04.207214 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v1-next.py
+-rw-r--r--   0        0        0     1134 2023-01-28 02:10:04.207668 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v1-set.py
+-rw-r--r--   0        0        0     1148 2023-01-28 02:10:04.207230 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-bulk.py
+-rw-r--r--   0        0        0     1120 2023-04-21 00:52:22.290743 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-get.py
+-rw-r--r--   0        0        0     1119 2023-01-28 20:02:25.533801 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-next.py
+-rw-r--r--   0        0        0     1133 2023-01-28 02:10:04.207177 pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-set.py
+-rw-r--r--   0        0        0     1601 2023-01-28 02:10:04.201800 pysnmp_lextudio-5.0.26/examples/smi/agent/custom-managed-object.py
+-rw-r--r--   0        0        0     1745 2023-01-28 02:10:04.093856 pysnmp_lextudio-5.0.26/examples/smi/agent/operations-on-managed-objects.py
+-rw-r--r--   0        0        0    17033 2023-01-21 20:50:50.867580 pysnmp_lextudio-5.0.26/examples/smi/manager/builder.py
+-rw-r--r--   0        0        0     1338 2023-04-21 00:52:22.291317 pysnmp_lextudio-5.0.26/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py
+-rw-r--r--   0        0        0     3809 2023-01-28 02:10:04.201814 pysnmp_lextudio-5.0.26/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py
+-rw-r--r--   0        0        0     2617 2023-01-28 02:10:04.111797 pysnmp_lextudio-5.0.26/examples/smi/manager/mib-tree-inspection.py
+-rw-r--r--   0        0        0     1045 2023-04-21 00:52:22.291835 pysnmp_lextudio-5.0.26/examples/smi/manager/print-oid-description.py
+-rw-r--r--   0        0        0     5169 2023-04-21 00:52:22.292532 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     2849 2023-04-21 00:52:22.292945 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     2406 2023-04-21 00:52:22.293292 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     3235 2023-04-21 00:52:22.295613 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py
+-rw-r--r--   0        0        0     3226 2023-04-21 00:52:22.295979 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py
+-rw-r--r--   0        0        0     3919 2023-04-21 00:52:22.296288 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py
+-rw-r--r--   0        0        0     3471 2023-04-21 00:52:22.296592 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py
+-rw-r--r--   0        0        0     3901 2023-04-21 00:52:22.296931 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py
+-rw-r--r--   0        0        0     2764 2023-04-21 00:52:22.297258 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py
+-rw-r--r--   0        0        0     3468 2023-04-21 00:52:22.297618 pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py
+-rw-r--r--   0        0        0     2677 2023-01-28 02:10:04.337349 pysnmp_lextudio-5.0.26/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py
+-rw-r--r--   0        0        0     2155 2023-01-28 02:10:04.345263 pysnmp_lextudio-5.0.26/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py
+-rw-r--r--   0        0        0     2519 2023-04-21 00:52:22.298051 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py
+-rw-r--r--   0        0        0     2464 2023-04-21 00:52:22.298392 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py
+-rw-r--r--   0        0        0     1995 2023-04-21 00:52:22.300650 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py
+-rw-r--r--   0        0        0     3603 2023-04-21 00:52:22.301465 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py
+-rw-r--r--   0        0        0     2458 2023-04-21 00:52:22.301890 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py
+-rw-r--r--   0        0        0     4319 2023-04-21 00:52:22.302623 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py
+-rw-r--r--   0        0        0     2065 2023-04-21 00:52:22.303159 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py
+-rw-r--r--   0        0        0     2090 2023-04-21 00:52:22.303511 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py
+-rw-r--r--   0        0        0     3167 2023-04-21 00:52:22.304156 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py
+-rw-r--r--   0        0        0     2199 2023-04-21 00:52:22.304446 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py
+-rw-r--r--   0        0        0     3352 2023-04-21 00:52:22.304775 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py
+-rw-r--r--   0        0        0     2714 2023-04-21 00:52:22.305142 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py
+-rw-r--r--   0        0        0     3314 2023-04-21 00:52:22.305471 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py
+-rw-r--r--   0        0        0     3883 2023-04-21 00:52:22.305829 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py
+-rw-r--r--   0        0        0     2616 2023-04-21 00:52:22.306131 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py
+-rw-r--r--   0        0        0     3567 2023-04-21 00:52:22.306448 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py
+-rw-r--r--   0        0        0     3393 2023-04-21 00:52:22.308732 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     2652 2023-04-21 00:52:22.309070 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py
+-rw-r--r--   0        0        0     3523 2023-04-21 00:52:22.309442 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py
+-rw-r--r--   0        0        0     3028 2023-04-21 00:52:22.309745 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py
+-rw-r--r--   0        0        0     3333 2023-04-21 00:52:22.310190 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v1-trap.py
+-rw-r--r--   0        0        0     3315 2023-04-21 00:52:22.310647 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py
+-rw-r--r--   0        0        0     3360 2023-04-21 00:52:22.310987 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py
+-rw-r--r--   0        0        0     3223 2023-04-21 00:52:22.311434 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py
+-rw-r--r--   0        0        0     2961 2023-04-21 00:52:22.313615 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v3-trap.py
+-rw-r--r--   0        0        0     2508 2023-04-21 00:52:22.314329 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py
+-rw-r--r--   0        0        0     2162 2023-04-21 00:52:22.314850 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py
+-rw-r--r--   0        0        0     2298 2023-04-21 00:52:22.315285 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py
+-rw-r--r--   0        0        0     2572 2023-04-21 00:52:22.315750 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py
+-rw-r--r--   0        0        0     2368 2023-04-21 00:52:22.316195 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py
+-rw-r--r--   0        0        0     3224 2023-04-21 00:52:22.316656 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py
+-rw-r--r--   0        0        0     2421 2023-04-21 00:52:22.317102 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py
+-rw-r--r--   0        0        0     3631 2023-04-21 00:52:22.317652 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py
+-rw-r--r--   0        0        0     2441 2023-04-21 00:52:22.318154 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py
+-rw-r--r--   0        0        0     2437 2023-04-21 00:52:22.320606 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py
+-rw-r--r--   0        0        0     2436 2023-04-21 00:52:22.320980 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py
+-rw-r--r--   0        0        0     3102 2023-04-21 00:52:22.321321 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py
+-rw-r--r--   0        0        0     2230 2023-04-21 00:52:22.321632 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py
+-rw-r--r--   0        0        0     2191 2023-04-21 00:52:22.321947 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py
+-rw-r--r--   0        0        0     2087 2023-04-21 00:52:22.322265 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/v1-get.py
+-rw-r--r--   0        0        0     2106 2023-04-21 00:52:22.322723 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py
+-rw-r--r--   0        0        0     2215 2023-04-21 00:52:22.325388 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py
+-rw-r--r--   0        0        0     2131 2023-04-21 00:52:22.326374 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py
+-rw-r--r--   0        0        0     2129 2023-04-21 00:52:22.326737 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     3728 2023-04-21 00:52:22.327858 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py
+-rw-r--r--   0        0        0     3313 2023-04-21 00:52:22.328342 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     3291 2023-04-21 00:52:22.328688 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py
+-rw-r--r--   0        0        0     4028 2023-04-21 00:52:22.329088 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py
+-rw-r--r--   0        0        0     3997 2023-04-21 00:52:22.330152 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py
+-rw-r--r--   0        0        0     3980 2023-04-21 00:52:22.330836 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py
+-rw-r--r--   0        0        0     4121 2023-04-21 00:52:22.331364 pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py
+-rw-r--r--   0        0        0     1189 2023-04-22 01:39:36.220888 pysnmp_lextudio-5.0.26/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-04-22 01:39:39.792551 pysnmp_lextudio-5.0.26/pysnmp/__init__.py
+-rw-r--r--   0        0        0     1252 2023-01-21 20:50:50.911870 pysnmp_lextudio-5.0.26/pysnmp/cache.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.495155 pysnmp_lextudio-5.0.26/pysnmp/carrier/__init__.py
+-rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495252 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/__init__.py
+-rw-r--r--   0        0        0     1857 2023-01-21 20:50:50.912293 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/base.py
+-rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495435 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/__init__.py
+-rw-r--r--   0        0        0     5316 2023-04-21 00:52:22.331968 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/base.py
+-rw-r--r--   0        0        0     1994 2023-01-21 20:50:50.914278 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/udp.py
+-rw-r--r--   0        0        0     1101 2023-01-21 20:50:50.914731 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/udp6.py
+-rw-r--r--   0        0        0     3443 2023-01-21 20:50:50.916499 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dispatch.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.332205 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/__init__.py
+-rw-r--r--   0        0        0     3335 2023-04-21 00:52:22.333698 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/base.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.333778 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/__init__.py
+-rw-r--r--   0        0        0     7379 2023-04-21 00:52:22.334421 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/base.py
+-rw-r--r--   0        0        0      584 2023-04-21 00:52:22.335041 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/udp.py
+-rw-r--r--   0        0        0     1389 2023-04-21 00:52:22.335816 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/udp6.py
+-rw-r--r--   0        0        0     1621 2023-04-21 00:52:22.336644 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/unix.py
+-rw-r--r--   0        0        0     1734 2023-04-21 00:52:22.337494 pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dispatch.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.337591 pysnmp_lextudio-5.0.26/pysnmp/carrier/asynsock/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.337679 pysnmp_lextudio-5.0.26/pysnmp/carrier/asynsock/dgram/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-21 00:52:22.346381 pysnmp_lextudio-5.0.26/pysnmp/carrier/asynsock/dgram/udp.py
+-rw-r--r--   0        0        0      209 2023-04-21 00:52:22.346875 pysnmp_lextudio-5.0.26/pysnmp/carrier/asynsock/dgram/udp6.py
+-rw-r--r--   0        0        0      209 2023-04-21 00:52:22.347793 pysnmp_lextudio-5.0.26/pysnmp/carrier/asynsock/dgram/unix.py
+-rw-r--r--   0        0        0      248 2023-04-21 00:52:22.348394 pysnmp_lextudio-5.0.26/pysnmp/carrier/asynsock/dispatch.py
+-rw-r--r--   0        0        0     8140 2023-04-21 00:52:22.349103 pysnmp_lextudio-5.0.26/pysnmp/carrier/base.py
+-rw-r--r--   0        0        0      235 2023-01-21 20:50:50.922097 pysnmp_lextudio-5.0.26/pysnmp/carrier/error.py
+-rw-r--r--   0        0        0      676 2023-01-21 20:50:50.922367 pysnmp_lextudio-5.0.26/pysnmp/carrier/sockfix.py
+-rw-r--r--   0        0        0     3558 2023-01-21 20:50:50.922632 pysnmp_lextudio-5.0.26/pysnmp/carrier/sockmsg.py
+-rw-r--r--   0        0        0     3501 2023-01-21 20:50:50.922909 pysnmp_lextudio-5.0.26/pysnmp/debug.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.497717 pysnmp_lextudio-5.0.26/pysnmp/entity/__init__.py
+-rw-r--r--   0        0        0    34968 2023-04-21 00:52:22.353135 pysnmp_lextudio-5.0.26/pysnmp/entity/config.py
+-rw-r--r--   0        0        0     8176 2023-01-21 20:50:50.925875 pysnmp_lextudio-5.0.26/pysnmp/entity/engine.py
+-rw-r--r--   0        0        0     2561 2023-01-21 20:50:50.927273 pysnmp_lextudio-5.0.26/pysnmp/entity/observer.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.498303 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/__init__.py
+-rw-r--r--   0        0        0    18591 2023-01-21 20:50:50.927634 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/cmdgen.py
+-rw-r--r--   0        0        0    14980 2023-01-21 20:50:50.927946 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/cmdrsp.py
+-rw-r--r--   0        0        0    10212 2023-01-21 20:50:50.930359 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/config.py
+-rw-r--r--   0        0        0     2623 2023-01-21 20:50:50.930748 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/context.py
+-rw-r--r--   0        0        0     2855 2023-01-21 20:50:50.931078 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/mibvar.py
+-rw-r--r--   0        0        0    17749 2023-01-21 20:50:50.931536 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/ntforg.py
+-rw-r--r--   0        0        0     4532 2023-01-21 20:50:50.931830 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/ntfrcv.py
+-rw-r--r--   0        0        0       59 2022-11-10 08:01:10.022472 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/oneliner/__init__.py
+-rw-r--r--   0        0        0    10016 2023-04-21 00:52:22.354201 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/oneliner/cmdgen.py
+-rw-r--r--   0        0        0     6644 2023-04-21 00:52:22.356701 pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/oneliner/ntforg.py
+-rw-r--r--   0        0        0      501 2023-01-21 20:50:50.932669 pysnmp_lextudio-5.0.26/pysnmp/error.py
+-rw-r--r--   0        0        0     3321 2023-04-21 00:52:22.357264 pysnmp_lextudio-5.0.26/pysnmp/hlapi/__init__.py
+-rw-r--r--   0        0        0      459 2023-01-21 20:50:50.933233 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/__init__.py
+-rw-r--r--   0        0        0    19830 2023-01-31 07:58:06.498827 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/cmdgen.py
+-rw-r--r--   0        0        0     5525 2023-01-23 06:09:50.177751 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/ntforg.py
+-rw-r--r--   0        0        0    13211 2023-01-25 01:36:58.327193 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/slim.py
+-rw-r--r--   0        0        0     4976 2023-01-23 20:11:38.568253 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/transport.py
+-rw-r--r--   0        0        0      462 2023-04-21 00:52:22.358928 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/__init__.py
+-rw-r--r--   0        0        0    20298 2023-04-21 00:52:22.362071 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/cmdgen.py
+-rw-r--r--   0        0        0     5202 2023-04-21 00:52:22.363199 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/ntforg.py
+-rw-r--r--   0        0        0      624 2023-04-21 00:52:22.363767 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/__init__.py
+-rw-r--r--   0        0        0    24567 2023-04-21 00:52:22.364659 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/cmdgen.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.364765 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/compat/__init__.py
+-rw-r--r--   0        0        0     9212 2023-04-21 00:52:22.365599 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py
+-rw-r--r--   0        0        0     1572 2023-04-21 00:52:22.365784 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/compat/ntforg.py
+-rw-r--r--   0        0        0     4573 2023-04-21 00:52:22.366001 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/ntforg.py
+-rw-r--r--   0        0        0     5124 2023-04-21 00:52:22.366195 pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/transport.py
+-rw-r--r--   0        0        0    18218 2023-04-21 00:52:22.366583 pysnmp_lextudio-5.0.26/pysnmp/hlapi/auth.py
+-rw-r--r--   0        0        0     2050 2023-04-21 00:52:22.366871 pysnmp_lextudio-5.0.26/pysnmp/hlapi/context.py
+-rw-r--r--   0        0        0    11790 2023-01-21 20:50:50.938949 pysnmp_lextudio-5.0.26/pysnmp/hlapi/lcd.py
+-rw-r--r--   0        0        0     1922 2023-04-21 00:52:22.367114 pysnmp_lextudio-5.0.26/pysnmp/hlapi/transport.py
+-rw-r--r--   0        0        0     2920 2023-01-21 20:50:50.939457 pysnmp_lextudio-5.0.26/pysnmp/hlapi/varbinds.py
+-rw-r--r--   0        0        0     1197 2023-01-21 20:50:50.939677 pysnmp_lextudio-5.0.26/pysnmp/nextid.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504675 pysnmp_lextudio-5.0.26/pysnmp/proto/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504925 pysnmp_lextudio-5.0.26/pysnmp/proto/acmod/__init__.py
+-rw-r--r--   0        0        0    12323 2023-01-21 20:50:50.939958 pysnmp_lextudio-5.0.26/pysnmp/proto/acmod/rfc3415.py
+-rw-r--r--   0        0        0      889 2023-01-21 20:50:50.940198 pysnmp_lextudio-5.0.26/pysnmp/proto/acmod/void.py
+-rw-r--r--   0        0        0      371 2023-01-21 20:50:50.940472 pysnmp_lextudio-5.0.26/pysnmp/proto/api/__init__.py
+-rw-r--r--   0        0        0     9391 2023-01-21 20:50:50.940745 pysnmp_lextudio-5.0.26/pysnmp/proto/api/v1.py
+-rw-r--r--   0        0        0     5599 2023-01-21 20:50:50.940989 pysnmp_lextudio-5.0.26/pysnmp/proto/api/v2c.py
+-rw-r--r--   0        0        0      926 2023-04-22 01:36:13.197204 pysnmp_lextudio-5.0.26/pysnmp/proto/api/verdec.py
+-rw-r--r--   0        0        0     1151 2023-04-21 00:52:22.367350 pysnmp_lextudio-5.0.26/pysnmp/proto/cache.py
+-rw-r--r--   0        0        0     5975 2023-04-21 00:52:22.367613 pysnmp_lextudio-5.0.26/pysnmp/proto/errind.py
+-rw-r--r--   0        0        0     1191 2023-01-21 20:50:50.941881 pysnmp_lextudio-5.0.26/pysnmp/proto/error.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.507349 pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/__init__.py
+-rw-r--r--   0        0        0     1754 2023-01-21 20:50:50.942134 pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/base.py
+-rw-r--r--   0        0        0     3910 2023-01-21 20:50:50.942358 pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/cache.py
+-rw-r--r--   0        0        0    20350 2023-01-21 20:50:50.942628 pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/rfc2576.py
+-rw-r--r--   0        0        0    35109 2023-01-22 07:40:10.590039 pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/rfc3412.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.508803 pysnmp_lextudio-5.0.26/pysnmp/proto/proxy/__init__.py
+-rw-r--r--   0        0        0     9874 2023-01-21 20:50:50.943242 pysnmp_lextudio-5.0.26/pysnmp/proto/proxy/rfc2576.py
+-rw-r--r--   0        0        0     6085 2023-04-21 00:52:22.367846 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1155.py
+-rw-r--r--   0        0        0     3323 2023-01-21 20:50:50.943726 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1157.py
+-rw-r--r--   0        0        0      563 2023-01-21 20:50:50.943981 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1901.py
+-rw-r--r--   0        0        0    21296 2023-04-21 00:52:22.368250 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1902.py
+-rw-r--r--   0        0        0     5671 2023-01-21 20:50:50.944541 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1905.py
+-rw-r--r--   0        0        0     1374 2023-01-21 20:50:50.944781 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc3411.py
+-rw-r--r--   0        0        0    21759 2023-01-21 20:50:50.945141 pysnmp_lextudio-5.0.26/pysnmp/proto/rfc3412.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510738 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/__init__.py
+-rw-r--r--   0        0        0     1485 2023-01-21 20:50:50.945499 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/base.py
+-rw-r--r--   0        0        0      881 2023-01-21 20:50:50.945778 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/cache.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510991 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511096 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/__init__.py
+-rw-r--r--   0        0        0     1030 2023-01-21 20:50:50.946099 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/aes192.py
+-rw-r--r--   0        0        0      999 2023-01-21 20:50:50.946416 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/aes256.py
+-rw-r--r--   0        0        0     3203 2023-01-21 20:50:50.946711 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/aesbase.py
+-rw-r--r--   0        0        0     5231 2023-01-21 20:50:50.946982 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/des3.py
+-rw-r--r--   0        0        0    21657 2023-04-21 00:52:22.368591 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc2576.py
+-rw-r--r--   0        0        0      261 2023-01-21 20:50:50.947549 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511982 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/__init__.py
+-rw-r--r--   0        0        0      850 2023-01-21 20:50:50.947795 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/base.py
+-rw-r--r--   0        0        0     3709 2023-01-21 20:50:50.948046 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py
+-rw-r--r--   0        0        0     3468 2023-01-21 20:50:50.948325 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py
+-rw-r--r--   0        0        0      733 2023-01-22 19:49:47.441260 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/noauth.py
+-rw-r--r--   0        0        0     2098 2023-01-21 20:50:50.949099 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/localkey.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.512518 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/__init__.py
+-rw-r--r--   0        0        0      728 2023-01-21 20:50:50.951254 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/base.py
+-rw-r--r--   0        0        0     4710 2023-01-21 20:50:50.951503 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/des.py
+-rw-r--r--   0        0        0      807 2023-01-21 20:50:50.951774 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/nopriv.py
+-rw-r--r--   0        0        0    56002 2023-01-22 20:02:41.908685 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/service.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513200 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3826/__init__.py
+-rw-r--r--   0        0        0       59 2022-12-02 02:52:14.601095 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3826/priv/__init__.py
+-rw-r--r--   0        0        0     4759 2023-01-21 20:50:50.953359 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3826/priv/aes.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513516 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc7860/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513622 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc7860/auth/__init__.py
+-rw-r--r--   0        0        0     4037 2023-01-21 20:50:50.953621 pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513825 pysnmp_lextudio-5.0.26/pysnmp/smi/__init__.py
+-rw-r--r--   0        0        0    16487 2023-01-21 20:50:50.953912 pysnmp_lextudio-5.0.26/pysnmp/smi/builder.py
+-rw-r--r--   0        0        0     2326 2023-04-04 18:56:40.326682 pysnmp_lextudio-5.0.26/pysnmp/smi/compiler.py
+-rw-r--r--   0        0        0     2351 2023-01-21 20:50:50.954423 pysnmp_lextudio-5.0.26/pysnmp/smi/error.py
+-rw-r--r--   0        0        0      317 2023-01-21 20:50:50.954638 pysnmp_lextudio-5.0.26/pysnmp/smi/exval.py
+-rw-r--r--   0        0        0     3084 2023-01-21 20:50:50.954871 pysnmp_lextudio-5.0.26/pysnmp/smi/indices.py
+-rw-r--r--   0        0        0     9227 2023-01-21 20:50:50.955119 pysnmp_lextudio-5.0.26/pysnmp/smi/instrum.py
+-rw-r--r--   0        0        0      283 2023-01-21 20:50:50.955343 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/ASN1-ENUMERATION.py
+-rw-r--r--   0        0        0      534 2023-01-21 20:50:50.955553 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/ASN1-REFINEMENT.py
+-rw-r--r--   0        0        0      505 2023-01-21 20:50:50.955778 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/ASN1.py
+-rw-r--r--   0        0        0    17614 2023-01-21 20:50:50.957301 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/INET-ADDRESS-MIB.py
+-rw-r--r--   0        0        0     3591 2023-01-21 20:50:50.957643 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/PYSNMP-MIB.py
+-rw-r--r--   0        0        0     4620 2023-01-21 20:50:50.957971 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py
+-rw-r--r--   0        0        0     9922 2023-01-21 20:50:50.958209 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/PYSNMP-USM-MIB.py
+-rw-r--r--   0        0        0     1318 2023-01-21 20:50:50.958608 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/RFC1158-MIB.py
+-rw-r--r--   0        0        0    56809 2023-01-21 20:50:50.959093 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/RFC1213-MIB.py
+-rw-r--r--   0        0        0    17437 2023-01-21 20:50:50.959514 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py
+-rw-r--r--   0        0        0    18836 2023-01-21 20:50:50.961309 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py
+-rw-r--r--   0        0        0     5882 2023-01-21 20:50:50.961679 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-MPD-MIB.py
+-rw-r--r--   0        0        0    19031 2023-01-21 20:50:50.962008 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py
+-rw-r--r--   0        0        0    10138 2023-01-21 20:50:50.962396 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-PROXY-MIB.py
+-rw-r--r--   0        0        0    24833 2023-01-21 20:50:50.962836 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-TARGET-MIB.py
+-rw-r--r--   0        0        0     3913 2023-01-21 20:50:50.963197 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py
+-rw-r--r--   0        0        0    33731 2023-01-21 20:50:50.963774 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py
+-rw-r--r--   0        0        0     3572 2023-01-21 20:50:50.964077 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py
+-rw-r--r--   0        0        0     5841 2023-01-21 20:50:50.964367 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py
+-rw-r--r--   0        0        0    30173 2023-01-21 20:50:50.964903 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py
+-rw-r--r--   0        0        0     4096 2023-01-21 20:50:50.965255 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-CONF.py
+-rw-r--r--   0        0        0    31135 2023-01-21 20:50:50.965742 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-MIB.py
+-rw-r--r--   0        0        0    46776 2023-01-21 20:50:50.966284 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-SMI.py
+-rw-r--r--   0        0        0    28986 2023-01-21 20:50:50.966685 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-TC.py
+-rw-r--r--   0        0        0     6921 2023-01-21 20:50:50.967022 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-TM.py
+-rw-r--r--   0        0        0    24370 2023-01-21 20:50:50.967422 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.522800 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/__init__.py
+-rw-r--r--   0        0        0      926 2023-01-21 20:50:50.967752 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py
+-rw-r--r--   0        0        0     1174 2023-01-21 20:50:50.968042 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py
+-rw-r--r--   0        0        0     1047 2023-01-21 20:50:50.968298 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py
+-rw-r--r--   0        0        0     1046 2023-01-21 20:50:50.968546 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py
+-rw-r--r--   0        0        0     2232 2023-01-21 20:50:50.968782 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py
+-rw-r--r--   0        0        0      530 2023-01-21 20:50:50.969033 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py
+-rw-r--r--   0        0        0     7605 2023-01-21 20:50:50.969323 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.523596 pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__init__.py
+-rw-r--r--   0        0        0    44735 2023-04-21 00:52:22.370798 pysnmp_lextudio-5.0.26/pysnmp/smi/rfc1902.py
+-rw-r--r--   0        0        0    12218 2023-01-21 20:50:50.971883 pysnmp_lextudio-5.0.26/pysnmp/smi/view.py
+-rw-r--r--   0        0        0     8280 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.26/setup.py
+-rw-r--r--   0        0        0     7816 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.26/PKG-INFO
```

### Comparing `pysnmp_lextudio-5.0.25/LICENSE.rst` & `pysnmp_lextudio-5.0.26/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/README.md` & `pysnmp_lextudio-5.0.26/README.md`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/Makefile` & `pysnmp_lextudio-5.0.26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/mibs/PYSNMP-MIB.txt` & `pysnmp_lextudio-5.0.26/docs/mibs/PYSNMP-MIB.txt`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/mibs/PYSNMP-SOURCE-MIB.txt` & `pysnmp_lextudio-5.0.26/docs/mibs/PYSNMP-SOURCE-MIB.txt`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/mibs/PYSNMP-USM-MIB.txt` & `pysnmp_lextudio-5.0.26/docs/mibs/PYSNMP-USM-MIB.txt`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/net-snmpd.conf` & `pysnmp_lextudio-5.0.26/docs/net-snmpd.conf`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/net-snmptrapd.conf` & `pysnmp_lextudio-5.0.26/docs/net-snmptrapd.conf`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/.static/favicon.ico` & `pysnmp_lextudio-5.0.26/docs/source/.static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/.static/logo.svg` & `pysnmp_lextudio-5.0.26/docs/source/.static/logo.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/.templates/layout.html` & `pysnmp_lextudio-5.0.26/docs/source/.templates/layout.html`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/conf.py` & `pysnmp_lextudio-5.0.26/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
     'sphinx.ext.intersphinx',
-    'sphinx_sitemap'
+    'sphinx_sitemap',
+    'sphinx_copybutton',
 ]
 
-html_baseurl = 'https://www.pysnmp.com/pysnmp'
+html_baseurl = 'https://www.pysnmp.com/pysnmp/'
 sitemap_url_scheme = '{link}'
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['.templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -50,32 +51,32 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'SNMP library for Python'
-copyright = '2005-2019, Ilya Etingof <etingof@gmail.com>;2022-2023, LeXtudio Inc. <support@lextudio.com>'
+copyright = '2005-2019, Ilya Etingof. © Copyright 2022-2023, LeXtudio Inc.'
 author = 'LeXtudio Inc. <support@lextudio.com>'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '5.0'
 # The full version, including alpha/beta/rc tags.
-release = '5.0.25'
+release = '5.0.26'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
 
@@ -109,40 +110,28 @@
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 #todo_include_todos = True
 
 
 # -- Options for HTML output ----------------------------------------------
 
+html_context = {
+    'display_github': True,
+    'github_user': 'lextudio',
+    'github_repo': 'pysnmp',
+    'github_version': 'main/docs/source/',
+}
+
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
-#html_theme = 'sphinx_rtd_theme'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    'logo': 'logo.svg',
-    'description': '<p align=left><i><b>Brewing free software for the communities</i></b></p>',
-    'show_powered_by': False,
-    'github_user': 'lextudio',
-    'github_repo': 'pysnmp',
-    'fixed_sidebar': True,
-}
-
-html_sidebars = {
-    '**': [
-        'about.html',
-        'navigation.html',
-        'relations.html',
-        'searchbox.html',
-        'donate.html',
-    ]
-}
 
 # Add any paths that contain custom themes here, relative to this directory.
 #html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 #html_title = None
@@ -191,18 +180,18 @@
 # If false, no index is generated.
 #html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
 #html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-html_show_sourcelink = False
+#html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-html_show_sphinx = False
+#html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
 #html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
@@ -308,16 +297,16 @@
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 
 
 # Configuration for Intersphinx
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3.4/', None),
-    'pyasn1': ('https://pyasn1.readthedocs.io/', None),
+    'python': ('https://docs.python.org/3.7/', None),
+    'pyasn1': ('https://pyasn1.readthedocs.io/en/latest/', None),
     'pysmi': ('https://www.pysnmp.com/pysmi/', None),
 }
 
 # this merges constructor docstring with class docstring
 autoclass_content = 'both'
 # Sort members by type
 autodoc_member_order = 'bysource'
@@ -329,7 +318,16 @@
 napoleon_include_special_with_doc = True
 napoleon_use_admonition_for_examples = False
 napoleon_use_admonition_for_notes = False
 napoleon_use_admonition_for_references = False
 napoleon_use_ivar = False
 napoleon_use_param = False
 napoleon_use_rtype = False
+
+def setup(app):
+    on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
+    if not on_rtd:
+        """Insert Google Analytics tracker
+        Based on this Stackoverflow suggestion: https://stackoverflow.com/a/41885884
+        """
+        app.add_js_file("https://www.googletagmanager.com/gtag/js?id=G-DYQGY4MKR3")
+        app.add_js_file("google_analytics_tracker.js")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysnmp_lextudio-5.0.25/docs/source/development.rst` & `pysnmp_lextudio-5.0.26/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/api-reference.rst` & `pysnmp_lextudio-5.0.26/docs/source/docs/api-reference.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 is shipped with a set of bindings to popular asynchronous Python I/O
 frameworks that let you run PySNMP in parallel with other tasks your
 application may perform.
 
 Synchronous SNMP
 ----------------
 
-Most simple and strightforward way to use PySNMP is by employing its
+Most simple and straightforward way to use PySNMP is by employing its
 Synchronous, blocking API. It's also the default API offered by
 users on *pysnmp.hlapi* sub-package import.
 
 Command Generator
 
 .. toctree::
    :maxdepth: 2
@@ -55,57 +55,21 @@
 
 .. autoclass:: pysnmp.hlapi.UdpTransportTarget
    :members: setLocalAddress
 
 .. autoclass:: pysnmp.hlapi.Udp6TransportTarget
    :members: setLocalAddress
 
-Asynchronous: asyncore
-----------------------
-
-The :mod:`asyncore` module is in Python standard library since ancient
-times. Main loop is built around :mod:`select` dispatcher, user
-code is invoked through callback callables.
-
-Command Generator
-
-.. toctree::
-   :maxdepth: 2
-
-   /docs/hlapi/asyncio/manager/cmdgen/getcmd
-   /docs/hlapi/asyncio/manager/cmdgen/setcmd
-   /docs/hlapi/asyncio/manager/cmdgen/nextcmd
-   /docs/hlapi/asyncio/manager/cmdgen/bulkcmd
-
-Notification Originator
-
-.. toctree::
-   :maxdepth: 2
-
-   /docs/hlapi/asyncio/agent/ntforg/notification 
-
-Transport configuration
-+++++++++++++++++++++++
-
-.. toctree::
-   :maxdepth: 2
-
-.. autoclass:: pysnmp.hlapi.asyncore.UdpTransportTarget
-   :members: setLocalAddress
-
-.. autoclass:: pysnmp.hlapi.asyncore.Udp6TransportTarget
-   :members: setLocalAddress
-
 Asynchronous: asyncio
 ---------------------
 
 The :mod:`asyncio` module first appeared in standard library since
 Python 3.3 (in provisional basis). Its main design feature is that
-it makes asynchronous code looking like synchronous one. That greately
-simplifies development and maintanence.
+it makes asynchronous code looking like synchronous one. That greatly
+simplifies development and maintenance.
 
 Command Generator
 
 .. toctree::
    :maxdepth: 2
 
    /docs/hlapi/asyncio/manager/cmdgen/getcmd
@@ -133,15 +97,15 @@
    :members: setLocalAddress
 
 
 SNMP Engine
 -----------
 
 SNMP Engine is a central, stateful object used by all SNMP v3
-substsems.  Calls to high-level Applications API also consume SNMP
+subsystems.  Calls to high-level Applications API also consume SNMP
 Engine object on input.
 
 .. toctree::
    :maxdepth: 2
 
 .. autoclass:: pysnmp.hlapi.SnmpEngine(snmpEngineID=None)
 
@@ -253,15 +217,15 @@
 +++++++++++++
 
 SNMP MIB variable is identified by an OBJECT IDENTIFIER (OID) and is 
 accompanied by a value belonging to one of SNMP types (:RFC:`1902#section-2`).
 This pair is collectively called a variable-binding in SNMP parlance.
 
 The :py:mod:`~pysnmp.smi.rfc1902` module implements :RFC:`1902#section-2`
-MACRO definiitons.
+MACRO definitions.
 
 .. toctree::
    :maxdepth: 2
 
 .. autoclass:: pysnmp.smi.rfc1902.ObjectIdentity
    :members:
 
@@ -275,15 +239,15 @@
 
 SNMP Notifications are enumerated and imply including certain
 set of MIB variables.
 Notification Originator applications refer to MIBs for MIB notifications
 through *NOTIFICATION-TYPE* ASN.1 macro. It conveys a set of MIB variables to 
 be gathered and reported in SNMP Notification. The
 :py:mod:`~pysnmp.smi.rfc1902` module implements :RFC:`1902#section-2`
-macro definiitons.
+macro definitions.
 
 .. toctree::
    :maxdepth: 2
 
 .. autoclass:: pysnmp.smi.rfc1902.NotificationType
    :members:
```

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/mib-object-instances.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/mib-object-instances.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/nms-components.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/nms-components.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/oid-tree-mibs.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/oid-tree-mibs.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/oid-tree.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/oid-tree.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/pysnmp-architecture.rst` & `pysnmp_lextudio-5.0.26/docs/source/docs/pysnmp-architecture.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/pysnmp-design.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/pysnmp-design.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/pysnmp-hlapi-tutorial.rst` & `pysnmp_lextudio-5.0.26/docs/source/docs/pysnmp-hlapi-tutorial.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/snmp-apps.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/snmp-apps.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/snmp-design.rst` & `pysnmp_lextudio-5.0.26/docs/source/docs/snmp-design.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/snmp-engine.svg` & `pysnmp_lextudio-5.0.26/docs/source/docs/snmp-engine.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/docs/snmp-history.rst` & `pysnmp_lextudio-5.0.26/docs/source/docs/snmp-history.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/download.rst` & `pysnmp_lextudio-5.0.26/docs/source/download.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/index.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/index.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/smi/agent/implementing-mib-objects.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/smi/agent/implementing-mib-objects.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/smi/manager/browsing-mib-tree.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/smi/manager/browsing-mib-tree.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/examples/v3arch/asyncio/index.rst` & `pysnmp_lextudio-5.0.26/docs/source/examples/v3arch/asyncio/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/getting-peer-information.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/getting-peer-information.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/how-to-implement-agent-mib.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/how-to-implement-agent-mib.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/ignored-snmp-packets.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/ignored-snmp-packets.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/listening-on-multiple-interfaces.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/listening-on-multiple-interfaces.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/non-printable-snmp-values-apps.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/non-printable-snmp-values-apps.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/non-printable-snmp-values-tools.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/non-printable-snmp-values-tools.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/oids-not-increasing.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/oids-not-increasing.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/pass-custom-mib-to-manager.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/pass-custom-mib-to-manager.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/py2exe-throws-error.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/py2exe-throws-error.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/response-values-mib-resolution.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/response-values-mib-resolution.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/snmp-data-constraints-verification-failure.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/snmp-data-constraints-verification-failure.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/faq/walk-whole-mib.rst` & `pysnmp_lextudio-5.0.26/docs/source/faq/walk-whole-mib.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/index.rst` & `pysnmp_lextudio-5.0.26/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/docs/source/quick-start.rst` & `pysnmp_lextudio-5.0.26/docs/source/quick-start.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 Quick start
 ===========
 
 .. toctree::
    :maxdepth: 2
 
-Once you downloaded and installed PySNMP library on your Linux/Windows/OS X
+Once you downloaded and installed PySNMP library on your Linux/Windows/macOS
 system, you should be able to solve the very basic SNMP task right from 
 your Python prompt - fetch some data from a remote SNMP Agent (you'd need 
 at least version 4.3.0 to run code from this page).
 
 Fetch SNMP variable
 -------------------
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * with Enterprise OID 1.3.6.1.4.1.20408.4.1.1.2
 * include managed object information '1.3.6.1.2.1.1.1.0' = 'my system'
 
 Functionally similar to:
 
 | $ snmptrap -v1 -c public demo.pysnmp.com 1.3.6.1.4.1.20408.4.1.1.2 0.0.0.0 1 0 0 1.3.6.1.2.1.1.1.0 s "my system"
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio import *
 
 
 async def run():
     snmpEngine = SnmpEngine()
     trap_result = await sendNotification(
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public demo.pysnmp.com 12345 1.3.6.1.6.3.1.1.5.2
 | $ snmpinform -v2c -c public demo.pysnmp.com 12345 1.3.6.1.6.3.1.1.5.2
 | $ snmptrap -v2c -c public demo.pysnmp.com 12345 1.3.6.1.6.3.1.1.5.2
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio import *
 
 
 async def sendone(snmpEngine, hostname, notifyType):
     trap_result = await sendNotification(
         snmpEngine,
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * based on asyncio I/O framework
 
 Functionally similar to:
 
 | $ snmpbulkwalk -v3 -lnoAuthNoPriv -u usr-none-none -Cn0 -Cr50 \
 |                demo.pysnmp.com  SNMPv2-MIB::system
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio import *
 
 
 async def run(varBinds):
     snmpEngine = SnmpEngine()
     while True:
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Functionally similar to:
 
 | $ snmpget -v2c -c public demo.pysnmp.com:1161 SNMPv2-MIB::sysDescr.0
 | $ snmpget -v2c -c public demo.pysnmp.com:2161 SNMPv2-MIB::sysDescr.0
 | $ snmpget -v2c -c public demo.pysnmp.com:3161 SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio import *
 
 
 async def getone(snmpEngine, hostname):
     get_result = await getCmd(
         snmpEngine,
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Functionally similar to:
 
 | $ snmpget -v2c -c public demo.pysnmp.com:1161 SNMPv2-MIB::sysDescr.0
 | $ snmpget -v2c -c public demo.pysnmp.com:2161 SNMPv2-MIB::sysDescr.0
 | $ snmpget -v2c -c public demo.pysnmp.com:3161 SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio import *
 
 
 async def getone(snmpEngine, hostname):
     result_get = await getCmd(
         snmpEngine,
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v1-get.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v1-get.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
 | $ snmpget -v1 -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim(1)
     errorIndication, errorStatus, errorIndex, varBinds = await slim.get(
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v1-next.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v1-next.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
 | $ snmpgetnext -v1 -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim(1)
     errorIndication, errorStatus, errorIndex, varBinds = await slim.next(
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v1-set.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v1-set.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
 | $ snmpget -v1 -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim(1)
     errorIndication, errorStatus, errorIndex, varBinds = await slim.set(
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-bulk.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
 | $ snmpbulkget -v2c -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim()
     errorIndication, errorStatus, errorIndex, varBinds = await slim.bulk(
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-get.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-next.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
   * over IPv4/UDP
   * to an Agent at demo.pysnmp.com:161
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
-| $ snmpget -v2c -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
+| $ snmpgetnext -v2c -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim()
-    errorIndication, errorStatus, errorIndex, varBinds = await slim.get(
+    errorIndication, errorStatus, errorIndex, varBinds = await slim.next(
         'public',
-        'demo.pysnmp.com',
+        'localhost',
         161,
         ObjectType(ObjectIdentity("SNMPv2-MIB", "sysDescr", 0)),
     )
 
     if errorIndication:
         print(errorIndication)
     elif errorStatus:
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-next.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-get.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
   * over IPv4/UDP
   * to an Agent at demo.pysnmp.com:161
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
-| $ snmpgetnext -v2c -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
+| $ snmpget -v2c -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim()
-    errorIndication, errorStatus, errorIndex, varBinds = await slim.next(
+    errorIndication, errorStatus, errorIndex, varBinds = await slim.get(
         'public',
         'demo.pysnmp.com',
         161,
         ObjectType(ObjectIdentity("SNMPv2-MIB", "sysDescr", 0)),
     )
 
     if errorIndication:
```

### Comparing `pysnmp_lextudio-5.0.25/examples/hlapi/asyncio/manager/cmdgen/v2-set.py` & `pysnmp_lextudio-5.0.26/examples/hlapi/asyncio/manager/cmdgen/v2c-set.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   * for an instance of SNMPv2-MIB::sysDescr.0 MIB object
   * Based on asyncio I/O framework
 
 Functionally similar to:
 
 | $ snmpget -v2c -c public demo.pysnmp.com SNMPv2-MIB::sysDescr.0
 
-"""  #
+"""#
 import asyncio
 from pysnmp.hlapi.asyncio.slim import Slim
 from pysnmp.smi.rfc1902 import ObjectIdentity, ObjectType
 
 async def run():
     slim = Slim()
     errorIndication, errorStatus, errorIndex, varBinds = await slim.set(
```

### Comparing `pysnmp_lextudio-5.0.25/examples/smi/agent/custom-managed-object.py` & `pysnmp_lextudio-5.0.26/examples/smi/agent/custom-managed-object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Implementing MIB objects
 ++++++++++++++++++++++++
 
 This script explains how SNMP Agent application could model
 real-world data as Managed Objects defined in MIB.
 
-"""  #
+"""#
 from pysnmp.smi import builder
 
 # MIB Builder is normally pre-created by SNMP engine
 mibBuilder = builder.MibBuilder()
 
 #
 # This may be done in a stand-alone file and then loaded up
```

### Comparing `pysnmp_lextudio-5.0.25/examples/smi/agent/operations-on-managed-objects.py` & `pysnmp_lextudio-5.0.26/examples/smi/agent/operations-on-managed-objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Agent operations on MIB
 +++++++++++++++++++++++
 
 This script explains how SNMP Agent application manipulates
 its MIB possibly triggered by SNMP Manager's commands.
 
-"""  #
+"""#
 # SNMP agent backend e.g. Agent access to Managed Objects
 from pysnmp.smi import builder, instrum, exval
 
 print("Loading MIB modules..."),
 mibBuilder = builder.MibBuilder().loadModules(
     "SNMPv2-MIB", "SNMP-FRAMEWORK-MIB", "SNMP-COMMUNITY-MIB"
 )
```

### Comparing `pysnmp_lextudio-5.0.25/examples/smi/manager/builder.py` & `pysnmp_lextudio-5.0.26/examples/smi/manager/builder.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py` & `pysnmp_lextudio-5.0.26/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ++++++++++++++++++++++++++++
 
 This script explains how Python application could turn SNMP PDU
 variable-bindings into MIB objects or the other way around.
 
 The code that configures MIB compiler is similar to what
 happens inside the pysnmp.hlapi API.
-"""  #
+"""#
 from pysnmp.smi import builder, view, compiler, rfc1902
 
 # Assemble MIB browser
 mibBuilder = builder.MibBuilder()
 mibViewController = view.MibViewController(mibBuilder)
 compiler.addMibCompiler(mibBuilder, sources=['file:///usr/share/snmp/mibs',
                                              'https://mibs.pysnmp.com/asn1/@mib@'])
```

### Comparing `pysnmp_lextudio-5.0.25/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py` & `pysnmp_lextudio-5.0.26/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This script explains how Python application (typically pysnmp-based
 SNMP Manager) could turn SNMP PDU variable-bindings into MIB objects
 or the other way around.
 
 The code below does not explicitly add MIB compiler - that happens
 behind the scenes. Examples below try to demo different kinds
 of MIB objects to work with.
-"""  #
+"""#
 from pysnmp.smi import builder, view, rfc1902, error
 
 # MIB Builder manages pysnmp MIBs
 mibBuilder = builder.MibBuilder()
 
 # MIB View Controller implements various queries to loaded MIBs
 mibView = view.MibViewController(mibBuilder)
```

### Comparing `pysnmp_lextudio-5.0.25/examples/smi/manager/mib-tree-inspection.py` & `pysnmp_lextudio-5.0.26/examples/smi/manager/mib-tree-inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 SNMP MIB browser
 ++++++++++++++++
 
 This script explains how Python application (typically SNMP Manager)
 could load SNMP MIB modules into memory and introspect Managed Objects
 defined in MIB.
 
-"""  #
+"""#
 from pysnmp.smi import builder, view, compiler, error
 
 # Create MIB loader/builder
 mibBuilder = builder.MibBuilder()
 
 # Optionally attach PySMI MIB compiler (if installed)
 # print('Attaching MIB compiler...'),
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 | $ snmpwalk -v2c -c public 127.0.0.1 .1.3.6
 | $ snmpwalk -v2c -c public udp6:[::1] .1.3.6
 
 The Command Receiver below uses two distinct transports for communication 
 with Command Generators - UDP over IPv4 and UDP over IPv6.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp, udp6, unix
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto import api
 import time, bisect
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * with TRAP ID 'coldStart' specified as an OID
 
 The following Net-SNMP command will produce similar SNMP notification:
 
 | $ snmpinform -v2c -c public udp:demo.pysnmp.com 0 1.3.6.1.6.3.1.1.5.1
 | $ snmpinform -v2c -c public udp6:[::1] 0 1.3.6.1.6.3.1.1.5.1
 
-"""  #
+"""#
 from time import time
 from pysnmp.carrier.asynsock.dispatch import AsynsockDispatcher
 from pysnmp.carrier.asynsock.dgram import udp, udp6
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto.api import v2c as pMod
 
 # Build PDU
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 * overriding Enterprise OID with 1.3.6.1.4.1.20408.4.1.1.2
 
 The following Net-SNMP commands will produce similar SNMP notification:
 
 | $ snmptrap -v1 -c public udp:demo.pysnmp.com 1.3.6.1.4.1.20408.4.1.1.2 127.0.0.1 1 0 12345
 | $ snmptrap -v1 -c public udp6:[::1] 1.3.6.1.4.1.20408.4.1.1.2 127.0.0.1 1 0 12345
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp, udp6, unix
 from pyasn1.codec.ber import encoder
 from pysnmp.proto import api
 
 # Protocol version to use
 pMod = api.protoModules[api.protoVersion1]
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 just waits for arbitrary time for collecting all responses. This technology
 is also known as SNMP-based discovery.
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v2c -c public -ObentU 255.255.255.255 1.3.6.1.2.1.1.1.0 1.3.6.1.2.1.1.3.0
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto import api
 from time import time
 
 # Broadcast manager settings
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * to an Agent at demo.pysnmp.com:161
 * for OIDs in tuple form
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v1 -c public -ObentU demo.pysnmp.com 1.3.6.1.2.1.1.1.0 1.3.6.1.2.1.1.3.0
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp, udp6, unix
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto import api
 from time import time
 
 # Protocol version to use
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * for OID in tuple form
 * with non-repeaters=0 and max-repeaters=25
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpbulkwalk -v2c -c public -ObentU -Cn0 -Cr25 demo.pysnmp.com 1.3.6
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto.api import v2c
 from time import time
 
 # SNMP table header
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * to an Agent at demo.pysnmp.com:161
 * for OID in tuple form
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpwalk -v1 -c public -ObentU demo.pysnmp.com 1.3.6
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto import api
 from time import time
 
 # Protocol version to use
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 sending from local interface could also be achieved by binding to 
 it (via openClientMode() parameter).
 
 Agent would respond to the IP address you used as a source. So this script 
 could only get a response if that source address is somehow routed to the 
 host this script is running on. Otherwise it just times out.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.proto import api
 from pyasn1.codec.ber import encoder, decoder
 from time import time
 
 # Send request message to this address
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * to an Agent at demo.pysnmp.com:161
 * for OIDs in string form and values in form of pyasn1 objects
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpset -v2c -c public -ObentU demo.pysnmp.com 1.3.6.1.2.1.1.9.1.3.1 s 'New description' 1.3.6.1.2.1.1.9.1.4.1 t 12
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp
 from pyasn1.codec.ber import encoder, decoder
 from pysnmp.proto import api
 from time import time
 
 # Protocol version to use
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py` & `pysnmp_lextudio-5.0.26/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 | $ snmptrap -v1 -c public 127.0.0.1 1.3.6.1.4.1.20408.4.1.1.2 127.0.0.1 1 1 123 1.3.6.1.2.1.1.1.0 s test
 | $ snmptrap -v2c -c public udp6:[::1] 123 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 s test
 
 Notification Receiver below uses two different transports for communication 
 with Notification Originators - UDP over IPv4 and UDP over IPv6.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp, udp6, unix
 from pyasn1.codec.ber import decoder
 from pysnmp.proto import api
 
 
 # noinspection PyUnusedLocal
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 | $ snmpwalk -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 localhost .1.3.6
 | $ snmpwalk -v3 -u usr-sha-none -l authNoPriv -a SHA -A authkey1 localhost .1.3.6
 | $ snmpwalk -v3 -u usr-sha-aes128 -l authPriv -a SHA -A authkey1 -x AES -X privkey1 localhost .1.3.6
 
 Requires Python 3.4 and later!
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncio.dgram import udp
 import asyncio
 
 # Get the event loop for this thread
 loop = asyncio.get_event_loop()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 receiver:
 
 | $ snmptrap -v2c -c public 127.0.0.1:162 123 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 s test
 | $ snmpinform -v2c -c public 127.0.0.1:2162 123 1.3.6.1.6.3.1.1.5.1
 
 Requires Python 3.4 and later!
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncio.dgram import udp
 from pysnmp.entity.rfc3413 import ntfrcv
 import asyncio
 
 # Get the event loop for this thread
 loop = asyncio.get_event_loop()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 * over IPv4/UDP, listening at 127.0.0.1:161
 
 Either of the following Net-SNMP commands will walk this Agent:
 
 | $ snmpwalk -v3 -u usr-md5-none -l authNoPriv -A authkey1 -E 8000000001020304 -n my-context 127.0.0.1 .1.3.6
 | $ snmpwalk -v3 -u usr-md5-none -l authNoPriv -A authkey1 -E 8000000001020304 127.0.0.1 .1.3.6
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.smi import instrum, builder
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * allow access to SNMPv2-MIB objects (1.3.6.1.2.1)
 * over IPv4/UDP, listening at 127.0.0.1:161
 
 The following Net-SNMP command will send GET request to this Agent:
 
 | $ snmpget -v3 -u usr-none-none -l noAuthNoPriv -n my-context -Ir 127.0.0.1 sysDescr.0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.smi import instrum
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * allow access to SNMPv2-MIB objects (1.3.6.1.2.1)
 * over IPv4/UDP, listening at 127.0.0.1:161
 
 The following Net-SNMP command will walk this Agent:
 
 | $ snmpwalk -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 -e 8000000004030201 localhost .1.3.6
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.proto import rfc1902
 
 # Create SNMP engine
 snmpEngine = engine.SnmpEngine(rfc1902.OctetString(hexValue="8000000004030201"))
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 However this command will fail:
 
 | $ snmpget -v2c -c public 127.0.0.1 SNMPv2-MIB::sysUpTime.0
 
 This command will not reveal `SNMPv2-MIB::sysUpTime.0` among other objects:
 
 | $ snmpwalk -v2c -c public 127.0.0.1 SNMPv2-MIB::system
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * allow read access only to the subtree where the custom MIB object resides
 * over IPv4/UDP, listening at 127.0.0.1:161
 
 The following Net-SNMP commands will walk this Agent:
 
 | $ snmpwalk -v2c -c public 127.0.0.1 .1.3.6
 
-"""  #
+"""#
 import sys
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 | $ snmpwalk -v2c -c public 127.0.0.1 1.3.6
 
 ...while the following command will destroy the same row
 
 | $ snmpset -v2c -c public 127.0.0.1 1.3.6.6.1.5.4.97.98.99 i 6
 | $ snmpwalk -v2c -c public 127.0.0.1 1.3.6
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   over IPv6/UDP, listening at [::1]:161
 
 Either of the following Net-SNMP commands will walk this Agent:
 
 | $ snmpwalk -v2c -c public 127.0.0.1 .1.3.6
 | $ snmpwalk -v2c -c public udp6:[::1] .1.3.6
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp, udp6
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * over IPv4/UDP, listening at 127.0.0.1:161 and 127.0.0.2:161 interfaces
 
 Either of the following Net-SNMP commands will walk this Agent:
 
 | $ snmpwalk -v2c -c public 127.0.0.1 .1.3.6
 | $ snmpwalk -v2c -c public 127.0.0.2 .1.3.6
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 The following script solves this problem by preserving original request
 destination IP address and put it back into response IP packet's source
 address field.
 
 To respond from a non-local (e.g. spoofed) IP address, uncomment the
 .enableTransparent() method call and run this script as root.
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Allow read/write access to all objects in the same MIB subtree.
 
 The following Net-SNMP's commands will GET/SET a value at this Agent:
 
 | $ snmpget -v1 -c public 127.0.0.1 SNMPv2-MIB::sysLocation.0
 | $ snmpset -v1 -c private 127.0.0.1 SNMPv2-MIB::sysLocation.0 s "far away"
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 Agent respectively:
 
 | $ snmpwalk -Ob -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 127.0.0.1 usmUserEntry
 | $ snmpwalk -Ob -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 127.0.0.2 usmUserEntry
 
 Notice differently configured snmpEngineId's in usmUserEntry columns.
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.proto import rfc1902
 from pysnmp.carrier.asyncore.dispatch import AsyncoreDispatcher
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Configuration parameters for each of SNMP Engines
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 Either of the following Net-SNMP commands will walk this Agent:
 
 | $ snmpwalk -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 localhost .1.3.6
 | $ snmpwalk -v3 -u usr-sha-none -l authNoPriv -a SHA -A authkey1 localhost .1.3.6
 | $ snmpwalk -v3 -u usr-sha-aes128 -l authPriv -a SHA -A authkey1 -x AES -X privkey1 localhost .1.3.6
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 | $ snmpwalk -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 localhost .1.3.6
 
 This script will report some details on request processing as seen
 by rfc3412.receiveMessage() and rfc3412.returnResponsePdu()
 abstract interfaces.
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, context
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   1.3.6.1.2.1.1.1.0 = 'Example Notificator'
 
 Functionally similar to:
 
 | $ snmpinform -v3 -l authPriv -u usr-md5-none -A authkey1 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification'
 | $ snmpinform -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   1.3.6.1.2.1.1.3.0 = 123
   1.3.6.1.6.3.1.1.4.1.0 = 1.3.6.1.6.3.1.1.5.1
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public demo.pysnmp.com 0 1.3.6.1.6.3.1.1.5.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   1.3.6.1.2.1.1.5.0 = 'Notificator Example'
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public udp:127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 | $ snmptrap -v2c -c public udp6:[::1] 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp, udp6
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * send TRAP notification
 * with TRAP ID 'coldStart' specified as an OID
 
 Functionally similar to:
 
 | $ snmptrap -v1 -c public 127.0.0.1 1.3.6.1.6.3.1.1.5.1 0.0.0.0 1 0 0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example notification' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * with TRAP ID 'warmStart' specified as an OID
 * include managed object information 1.3.6.1.2.1.1.5.0 = 'system name'
 
 Functionally similar to:
 
 | $ snmpinform -v3 -l authNoPriv -u usr-md5-none -A authkey1 demo.pysnmp.com  0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 = 'system name'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v1-trap.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v1-trap.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * overriding Enterprise OID with 1.3.6.1.4.1.20408.4.1.1.2
 * include managed object information '1.3.6.1.2.1.1.1.0' = 'my system'
 
 Functionally similar to:
 
 | $ snmptrap -v1 -c public demo.pysnmp.com 1.3.6.1.4.1.20408.4.1.1.2 127.0.0.1 6 432 12345 1.3.6.1.2.1.1.1.0 s "my system"
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   1.3.6.1.2.1.1.1.0 = 'Example Notificator'
   1.3.6.1.2.1.1.5.0 = 'Notificator Example'
 
 Functionally similar to:
 
 | $ snmpinform -v2c -c public 127.0.0.1 12345 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s 'Example Notificator' 1.3.6.1.2.1.1.5.0 s 'Notificator Example'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 Where "x" is MIB table index (instance index).
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public 127.0.0.1 0 1.3.6.1.6.3.1.1.5.3 IF-MIB::ifIndex."1" IF-MIB::ifAdminStatus."1" IF-MIB::ifOperStatus."1" IF-MIB::ifDescr."1"
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.smi import rfc1902, view
 
 #
 # Here we fill in some values for Managed Objects Instances (invoked
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   1.3.6.1.2.1.1.1.0 = 'Example Notificator'
   1.3.6.1.2.1.1.5.0 = 'Notificator Example'
 
 Functionally similar to:
 
 | $ snmptrap -v2c -c public 127.0.0.1 12345 1.3.6.1.4.1.20408.4.1.1.2
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/agent/ntforg/v3-trap.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/agent/ntforg/v3-trap.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * with TRAP ID 'warmStart' specified as an OID
 * include managed object information 1.3.6.1.2.1.1.5.0 = 'system name'
 
 Functionally similar to:
 
 | $ snmptrap -v3 -l authPriv -u usr-md5-des -A authkey1 -X privkey1 -e 8000000001020304 demo.pysnmp.com 0 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.1.0 s "my system"
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntforg
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine instance with specific (and locally unique)
 # SnmpEngineId -- it must also be known to the receiving party
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * to an Agent at 127.0.0.1:161
 * for an OID in tuple form
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v3 -l authNoPriv -u usr-md5-none -A authkey1 -E 80004fb805636c6f75644dab22cc -n da761cfc8c94d3aceef4f60f049105ba -ObentU 127.0.0.1:161  1.3.6.1.2.1.1.1.0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.proto import rfc1902
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * wait 3 seconds for response, retry 5 times (plus one initial attempt)
 * for an OID in tuple form
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v2c -c public -ObentU -r 5 -t 1 127.0.0.1 1.3.6.1.2.1.1.1.0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * for two OIDs in tuple form
 * stop on end-of-mib condition for both OIDs
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpwalk -v3 -l authNoPriv -u usr-md5-none -A authkey1 -ObentU udp6:[::1]:161 1.3.6.1.2.1.1 1.3.6.1.4.1.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp6
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * for two OIDs in tuple form (first OID is non-repeating)
 * stop on end-of-mib condition for both OIDs
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpbulkwalk -v3 -l authPriv -u usr-md5-des -A authkey1 -X privkey1 -C n1 -C r25 -ObentU 127.0.0.1 1.3.6.1.2.1.1 1.3.6.1.4.1.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * for two OIDs in tuple form
 * stop on end-of-mib condition for both OIDs
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpbulkwalk -v2c -c public -C n0 -C r25 -ObentU 127.0.0.1 1.3.6.1.2.1.1 1.3.6.1.4.1.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.carrier.asyncore.dgram import udp
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * for two OIDs in tuple form
 * stop on end-of-mib condition for both OIDs
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpwalk -v1 -c public -ObentU 127.0.0.1 1.3.6.1.2.1.1 1.3.6.1.4.1.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.smi import compiler, view, rfc1902
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * for two OIDs in tuple form
 * stop on end-of-mib condition for both OIDs
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpwalk -v1 -c public -ObentU 127.0.0.1 1.3.6.1.2.1.1 1.3.6.1.4.1.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 While execution, this script will report some details on request processing 
 as seen by rfc3412.sendPdu() and rfc3412.receiveMessage() abstract interfaces.
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v3 -l authPriv -u usr-sha-aes -a SHA -A authkey1 -x AES -X privkey1 -ObentU 127.0.0.1:161  1.3.6.1.2.1.1.1.0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * for an OID in string form
 * stop whenever received OID goes out of initial prefix (it may be a table)
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpwalk -v3 -l noAuthNoPriv -u usr-none-none -ObentU 127.0.0.1:161  1.3.6.1.2.1.1 
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.proto import rfc1902
 
 # Initial OID prefix
 initialOID = rfc1902.ObjectName("1.3.6.1.2.1.1")
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * for two OIDs in tuple form
 * stop on end-of-mib condition for both OIDs
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpwalk -v2c -c public -ObentU 127.0.0.1 1.3.6.1.2.1.1 1.3.6.1.4.1.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * to an Agent at 127.0.0.1:161
 * for OIDs in tuple form and an integer and string-typed values
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpset -v1 -c private -ObentU 127.0.0.1:161 1.3.6.1.2.1.1.9.1.3.1 s 'my value'  1.3.6.1.2.1.1.9.1.4.1 t 123 
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.proto import rfc1902
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 It is indeed possible to originate SNMP traffic from any valid local
 IP addresses. It could be a secondary IP interface, for instance. 
 Superuser privileges are only required to send spoofed packets. 
 Alternatively, sending from local interface could also be achieved by
 binding to it (via openClientMode() parameter).
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 * to an Agent at 127.0.0.1:161
 * for an OID in tuple form
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v3 -l authPriv -u usr-sha-aes -a SHA -A authkey1 -x AES -X privkey1 -ObentU 127.0.0.1:161  1.3.6.1.2.1.1.1.0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * to an Agent at 127.0.0.1:161
 * for an OID in tuple form and a string-typed value
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpset -v3 -l authNoPriv -u usr-sha-none -a SHA -A authkey1 -ObentU 127.0.0.1:161 1.3.6.1.2.1.1.9.1.3.1 s 'my new value'
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.proto import rfc1902
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/v1-get.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/v1-get.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 * to an Agent at 127.0.0.1:161
 * for an OID in tuple form
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpget -v1 -c public -ObentU 127.0.0.1 1.3.6.1.2.1.1.1.0
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 * to an Agent at 127.0.0.1:161
 * for an OID in tuple form and an integer-typed value
 
 This script performs similar to the following Net-SNMP command:
 
 | $ snmpset -v2c -c private -ObentU 127.0.0.1:161 1.3.6.1.2.1.1.9.1.4.1 t 123
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import cmdgen
 from pysnmp.proto import rfc1902
 
 # Create SNMP engine instance
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * print received data on stdout
 
 Either of the following Net-SNMP commands will send notifications to this
 receiver:
 
 | $ snmptrap -v2c -c public 127.0.0.1:162 123 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 s test
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntfrcv
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Either of the following Net-SNMP commands will send notifications to this
 receiver:
 
 | $ snmptrap -v2c -c public 127.0.0.1:162 123 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 s test
 | $ snmpinform -v2c -c public 127.0.0.1:2162 123 1.3.6.1.6.3.1.1.5.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntfrcv
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Either of the following Net-SNMP commands will send notifications to this
 receiver:
 
 | $ snmptrap -v1 -c public 127.0.0.1 1.3.6.1.4.1.20408.4.1.1.2 127.0.0.1 1 1 123 1.3.6.1.2.1.1.1.0 s test
 | $ snmptrap -v2c -c public udp6:[::1]:162 123 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 s test
 | $ snmpinform -v2c -c public 127.0.0.1 123 1.3.6.1.6.3.1.1.5.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp, udp6
 from pysnmp.entity.rfc3413 import ntfrcv
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Either of the following Net-SNMP commands will send notifications to this
 receiver:
 
 | $ snmptrap -v3 -u usr-md5-des -l authPriv -A authkey1 -X privkey1 -e 8000000001020304 127.0.0.1 123 1.3.6.1.6.3.1.1.5.1
 | $ snmptrap -v3 -u usr-md5-none -l authNoPriv -A authkey1 -e 8000000001020304 127.0.0.1 123 1.3.6.1.6.3.1.1.5.1
 | $ snmpinform -v3 -u usr-sha-aes128 -l authPriv -a SHA -A authkey1 -x AES -X privkey1 127.0.0.1 123 1.3.6.1.6.3.1.1.5.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntfrcv
 from pysnmp.proto.api import v2c
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Either of the following Net-SNMP commands will send notifications to this
 receiver:
 
 | $ snmptrap -v1 -c public 127.0.0.1 1.3.6.1.4.1.20408.4.1.1.2 127.0.0.1 1 1 123 1.3.6.1.2.1.1.1.0 s test
 | $ snmptrap -v2c -c public udp6:[::1]:162 123 1.3.6.1.6.3.1.1.5.1 1.3.6.1.2.1.1.5.0 s test
 | $ snmpinform -v2c -c public 127.0.0.1 123 1.3.6.1.6.3.1.1.5.1
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp, udp6
 from pysnmp.entity.rfc3413 import ntfrcv
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
 snmpEngine = engine.SnmpEngine()
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 the context of user application.
 
 This script examines the value of CommunityName, as it came from peer SNMP
 Engine, and may modify it to match the only locally configured CommunityName
 'public'. This effectively makes NotificationReceiver accepting messages with
 CommunityName's, not explicitly configured to local SNMP Engine.
 
-"""  #
+"""#
 from pysnmp.entity import engine, config
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity.rfc3413 import ntfrcv
 import re
 
 # Create SNMP engine with autogenernated engineID and pre-bound
 # to socket transport dispatcher
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 | $ snmpget -v2c -c public 127.0.0.1:161 sysDescr.0
 
 Warning: for production operation you would need to modify this script
 so that it will re-map possible duplicate request-ID values, coming in
 initial request PDUs from different Managers, into unique values to
 avoid sending duplicate request-IDs to Agents.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dgram import udp, udp6
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, cmdgen, context
 from pysnmp.proto.api import v2c
 from pysnmp import error
 
 # Create SNMP engine with autogenernated engineID and pre-bound
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 | $ snmpwalk -v1 -c public 127.0.0.1:161 system
 
 Warning: for production operation you would need to modify this script
 so that it will re-map possible duplicate request-ID values, coming in
 initial request PDUs from different Managers, into unique values to
 avoid sending duplicate request-IDs to Agents.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, cmdgen, context
 from pysnmp.proto.api import v2c
 from pysnmp import error
 
 # Create SNMP engine with autogenernated engineID and pre-bound
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 | $ snmpget -v3 -l authNoPriv -u usr-md5-none -A authkey1 -ObentU 127.0.0.1:161  1.3.6.1.2.1.1.1.0
 
 Warning: for production operation you would need to modify this script
 so that it will re-map possible duplicate request-ID values, coming in
 initial request PDUs from different Managers, into unique values to
 avoid sending duplicate request-IDs to Agents.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, cmdgen, context
 from pysnmp.proto.api import v2c
 from pysnmp import error
 
 # Create SNMP engine with autogenernated engineID and pre-bound
```

### Comparing `pysnmp_lextudio-5.0.25/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py` & `pysnmp_lextudio-5.0.26/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 | $ snmpget -v2c -c public 127.0.0.1:161 1.3.6.1.2.1.1.1.0
 
 Warning: for production operation you would need to modify this script
 so that it will re-map possible duplicate request-ID values, coming in
 initial request PDUs from different Managers, into unique values to
 avoid sending duplicate request-IDs to Agents.
 
-"""  #
+"""#
 from pysnmp.carrier.asyncore.dgram import udp
 from pysnmp.entity import engine, config
 from pysnmp.entity.rfc3413 import cmdrsp, cmdgen, context
 from pysnmp.proto.api import v2c
 from pysnmp import error
 
 # Create SNMP engine with autogenernated engineID and pre-bound
```

### Comparing `pysnmp_lextudio-5.0.25/pyproject.toml` & `pysnmp_lextudio-5.0.26/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnmp-lextudio"
-version = "5.0.25"
+version = "5.0.26"
 description = ""
 authors = ["Ilya Etingof <etingof@gmail.com>", "Lex Li <support@lextudio.com>"]
 license = "BSD-2-Clause"
 repository = "https://github.com/lextudio/pysnmp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -24,15 +24,15 @@
 ]
 include = ["docs", "tests", "examples"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pysmi-lextudio = "^1.0.4"
-pyasn1 = ">=0.4.8"
+pyasn1 = ">=0.4.8, <0.5.0"
 pycryptodomex = "^3.11.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.0"
 pytest = "^6.2.5"
 codecov = "^2.1.12"
 pytest-codecov = "^0.4.0"
```

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/cache.py` & `pysnmp_lextudio-5.0.26/pysnmp/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/udp.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/udp.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dgram/udp6.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dgram/udp6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncio/dispatch.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncio/dispatch.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/udp.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/udp.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/udp6.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/udp6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dgram/unix.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dgram/unix.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/asyncore/dispatch.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/asyncore/dispatch.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/sockfix.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/sockfix.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/carrier/sockmsg.py` & `pysnmp_lextudio-5.0.26/pysnmp/carrier/sockmsg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/debug.py` & `pysnmp_lextudio-5.0.26/pysnmp/debug.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/config.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/config.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/engine.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/engine.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/observer.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/observer.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/cmdgen.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/cmdrsp.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/cmdrsp.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/config.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/config.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/context.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/context.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/mibvar.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/mibvar.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/ntforg.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/ntfrcv.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/ntfrcv.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/oneliner/cmdgen.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/oneliner/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/entity/rfc3413/oneliner/ntforg.py` & `pysnmp_lextudio-5.0.26/pysnmp/entity/rfc3413/oneliner/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/__init__.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/cmdgen.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/ntforg.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/slim.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/slim.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncio/transport.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncio/transport.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/cmdgen.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/ntforg.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/__init__.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/cmdgen.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/compat/ntforg.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/compat/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/sync/ntforg.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/sync/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/asyncore/transport.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/asyncore/transport.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/auth.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/auth.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/context.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/context.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/lcd.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/lcd.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/transport.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/transport.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/hlapi/varbinds.py` & `pysnmp_lextudio-5.0.26/pysnmp/hlapi/varbinds.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/nextid.py` & `pysnmp_lextudio-5.0.26/pysnmp/nextid.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/acmod/rfc3415.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/acmod/rfc3415.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/acmod/void.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/acmod/void.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/api/v1.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/api/v1.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/api/v2c.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/api/v2c.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/api/verdec.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/api/verdec.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/cache.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/errind.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/errind.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/error.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/error.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/cache.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/rfc2576.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/rfc2576.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/mpmod/rfc3412.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/mpmod/rfc3412.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/proxy/rfc2576.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/proxy/rfc2576.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1155.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1155.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1157.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1157.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1901.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1901.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1902.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1902.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc1905.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc1905.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc3411.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc3411.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/rfc3412.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/rfc3412.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/cache.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/aes192.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/aes192.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/aes256.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/aes256.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/aesbase.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/aesbase.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/eso/priv/des3.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/eso/priv/des3.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc2576.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc2576.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/auth/noauth.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/auth/noauth.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/localkey.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/localkey.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/base.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/des.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/des.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/priv/nopriv.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/priv/nopriv.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3414/service.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3414/service.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc3826/priv/aes.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc3826/priv/aes.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py` & `pysnmp_lextudio-5.0.26/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/builder.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/builder.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/compiler.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/compiler.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/error.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/error.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/indices.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/indices.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/instrum.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/instrum.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/ASN1-REFINEMENT.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/ASN1-REFINEMENT.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/INET-ADDRESS-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/INET-ADDRESS-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/PYSNMP-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/PYSNMP-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/PYSNMP-USM-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/RFC1158-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/RFC1158-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/RFC1213-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/RFC1213-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-MPD-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-MPD-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-PROXY-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-PROXY-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-TARGET-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-TARGET-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-CONF.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-CONF.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-SMI.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-SMI.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-TC.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-TC.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/SNMPv2-TM.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/SNMPv2-TM.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/rfc1902.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/rfc1902.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/pysnmp/smi/view.py` & `pysnmp_lextudio-5.0.26/pysnmp/smi/view.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.25/setup.py` & `pysnmp_lextudio-5.0.26/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,21 @@
  'pysnmp.smi.mibs',
  'pysnmp.smi.mibs.instances']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pyasn1>=0.4.8',
+['pyasn1>=0.4.8,<0.5.0',
  'pycryptodomex>=3.11.0,<4.0.0',
  'pysmi-lextudio>=1.0.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysnmp-lextudio',
-    'version': '5.0.25',
+    'version': '5.0.26',
     'description': '',
     'long_description': "\nSNMP Library for Python\n-----------------------\n\n[![PyPI](https://img.shields.io/pypi/v/pysnmp-lextudio.svg)](https://pypi.python.org/pypi/pysnmp-lextudio)\n[![PyPI Downloads](https://img.shields.io/pypi/dd/pysnmp-lextudio)](https://pypi.python.org/pypi/pysnmp-lextudio/)\n[![Python Versions](https://img.shields.io/pypi/pyversions/pysnmp-lextudio.svg)](https://pypi.python.org/pypi/pysnmp-lextudio/)\n[![GitHub license](https://img.shields.io/badge/license-BSD-blue.svg)](https://raw.githubusercontent.com/lextudio/pysnmp/master/LICENSE.rst)\n\nThis is a pure-Python, open source and free implementation of v1/v2c/v3\nSNMP engine distributed under 2-clause [BSD license](https://www.pysnmp.com/pysnmp/license.html).\n\nThe PySNMP project was initially sponsored by a [PSF](http://www.python.org/psf/) grant.\nThank you!\n\nThis version is a fork of Ilya Etingof's project [etingof/pysnmp](https://github.com/etingof/pysnmp). Ilya sadly passed away on 10-Aug-2022. Announcement [here](https://lists.openstack.org/pipermail/openstack-discuss/2022-August/030062.html).  His work is still of great use to the Python community and he will be missed.\n\nFeatures\n--------\n\n* Complete SNMPv1/v2c and SNMPv3 support\n* SMI framework for resolving MIB information and implementing SMI\n  Managed Objects\n* Complete SNMP entity implementation\n* USM Extended Security Options support (3DES, 192/256-bit AES encryption)\n* Extensible network transports framework (UDP/IPv4, UDP/IPv6)\n* Asynchronous socket-based IO API support\n* [Asyncio](https://docs.python.org/3/library/asyncio.html) integration\n* [PySMI](https://www.pysnmp.com/pysmi/) integration for dynamic MIB compilation\n* Built-in instrumentation exposing protocol engine operations\n* Python eggs and py2exe friendly\n* 100% Python, works with Python 3.7+\n* MT-safe (if SnmpEngine is thread-local)\n\nFeatures, specific to SNMPv3 model include:\n\n* USM authentication (MD5/SHA-1/SHA-2) and privacy (DES/AES) protocols (RFC3414, RFC7860)\n* View-based access control to use with any SNMP model (RFC3415)\n* Built-in SNMP proxy PDU converter for building multi-lingual\n  SNMP entities (RFC2576)\n* Remote SNMP engine configuration\n* Optional SNMP engine discovery\n* Shipped with standard SNMP applications (RC3413)\n\n\nDownload & Install\n------------------\n\nThe PySNMP software is freely available for download from [PyPI](https://pypi.python.org/pypi/pysnmp-lextudio)\nand [GitHub](https://github.com/lextudio/pysnmp.git).\n\nJust run:\n\n```bash\n$ pip install pysnmp-lextudio\n```\n\nTo download and install PySNMP along with its dependencies:\n\n<!-- Need to find an alternate location for the links to pysnmp.com -->\n* [PyASN1](https://pyasn1.readthedocs.io)\n* [PyCryptodomex](https://pycryptodome.readthedocs.io) (required only if SNMPv3 encryption is in use)\n* [PySMI](https://www.pysnmp.com/pysmi/) (required for MIB services only)\n\nBesides the library, command-line [SNMP utilities](https://github.com/lextudio/snmpclitools)\nwritten in pure-Python could be installed via:\n\n```bash\n$ pip install snmpclitools-lextudio\n```\n\nand used in the very similar manner as conventional Net-SNMP tools:\n\n```bash\n$ snmpget.py -v3 -l authPriv -u usr-md5-des -A authkey1 -X privkey1 demo.pysnmp.com sysDescr.0\nSNMPv2-MIB::sysDescr.0 = STRING: Linux zeus 4.8.6.5-smp #2 SMP Sun Nov 13 14:58:11 CDT 2016 i686\n```\n\nExamples\n--------\n\nPySNMP is designed in a layered fashion. Top-level and easiest to use API is known as\n*hlapi*. Here's a quick example on how to SNMP GET:\n\n```python\nfrom pysnmp.hlapi import *\n\niterator = getCmd(SnmpEngine(),\n                  CommunityData('public'),\n                  UdpTransportTarget(('demo.pysnmp.com', 161)),\n                  ContextData(),\n                  ObjectType(ObjectIdentity('SNMPv2-MIB', 'sysDescr', 0)))\n\nerrorIndication, errorStatus, errorIndex, varBinds = next(iterator)\n\nif errorIndication:  # SNMP engine errors\n    print(errorIndication)\nelse:\n    if errorStatus:  # SNMP agent errors\n        print('%s at %s' % (errorStatus.prettyPrint(), varBinds[int(errorIndex)-1] if errorIndex else '?'))\n    else:\n        for varBind in varBinds:  # SNMP response contents\n            print(' = '.join([x.prettyPrint() for x in varBind]))\n```\n\nThis is how to send SNMP TRAP:\n\n```python\nfrom pysnmp.hlapi import *\n\nerrorIndication, errorStatus, errorIndex, varBinds = next(\n    sendNotification(\n        SnmpEngine(OctetString(hexValue='8000000001020304')),\n        UsmUserData('usr-sha-aes128', 'authkey1', 'privkey1',\n                    authProtocol=usmHMACSHAAuthProtocol,\n                    privProtocol=usmAesCfb128Protocol),\n        UdpTransportTarget(('demo.pysnmp.com', 162)),\n        ContextData(),\n        'trap',\n        NotificationType(ObjectIdentity('SNMPv2-MIB', 'authenticationFailure'))\n    )\n)\n\nif errorIndication:\n    print(errorIndication)\n```\n\n> We maintain publicly available SNMP Agent and TRAP sink at\n> [demo.pysnmp.com](https://www.pysnmp.com/snmpsim/public-snmp-agent-simulator.html). You are\n> welcome to use it while experimenting with whatever SNMP software you deal with.\n\n```bash\n$ python3 examples/hlapi/asyncore/sync/manager/cmdgen/usm-sha-aes128.py\nSNMPv2-MIB::sysDescr.0 = SunOS zeus.pysnmp.com 4.1.3_U1 1 sun4m\n$\n$ python3 examples//hlapi/asyncore/sync/agent/ntforg/v3-inform.py\nSNMPv2-MIB::sysUpTime.0 = 0\nSNMPv2-MIB::snmpTrapOID.0 = SNMPv2-MIB::warmStart\nSNMPv2-MIB::sysName.0 = system name\n```\n\nOther than that, PySNMP is capable to automatically fetch and use required MIBs from HTTP, FTP sites\nor local directories. You could configure any MIB source available to you (including\n[this one](https://github.com/lextudio/mibs.snmplabs.com/tree/master/asn1)) for that purpose.\n\nFor more example scripts please refer to [examples section](https://www.pysnmp.com/pysnmp/examples/index.html#high-level-snmp)\nat pysnmp web site.\n\nDocumentation\n-------------\n\nLibrary documentation and examples can be found at the [pysnmp project site](https://www.pysnmp.com/pysnmp/).\n\nIf something does not work as expected, please\n[open an issue](https://github.com/lextudio/pysnmp/issues) at GitHub or\npost your question [on Stack Overflow](http://stackoverflow.com/questions/ask) or try browsing pysnmp\n[mailing list archives](https://sourceforge.net/p/pysnmp/mailman/pysnmp-users/).\n\nBug reports and PRs are appreciated! ;-)\n\nCopyright (c) 2005-2019, [Ilya Etingof](https://lists.openstack.org/pipermail/openstack-discuss/2022-August/030062.html).\nCopyright (c) 2022, [LeXtudio Inc](mailto:support@lextudio.com).\nAll rights reserved.\n",
     'author': 'Ilya Etingof',
     'author_email': 'etingof@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lextudio/pysnmp',
```

### Comparing `pysnmp_lextudio-5.0.25/PKG-INFO` & `pysnmp_lextudio-5.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnmp-lextudio
-Version: 5.0.25
+Version: 5.0.26
 Summary: 
 Home-page: https://github.com/lextudio/pysnmp
 License: BSD-2-Clause
 Author: Ilya Etingof
 Author-email: etingof@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pyasn1 (>=0.4.8)
+Requires-Dist: pyasn1 (>=0.4.8,<0.5.0)
 Requires-Dist: pycryptodomex (>=3.11.0,<4.0.0)
 Requires-Dist: pysmi-lextudio (>=1.0.4,<2.0.0)
 Project-URL: Repository, https://github.com/lextudio/pysnmp
 Description-Content-Type: text/markdown
 
 
 SNMP Library for Python
```

