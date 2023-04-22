# Comparing `tmp/fullctl-1.2.0.tar.gz` & `tmp/fullctl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullctl-1.2.0.tar", max compression
+gzip compressed data, was "fullctl-1.3.0.tar", max compression
```

## Comparing `fullctl-1.2.0.tar` & `fullctl-1.3.0.tar`

### file list

```diff
@@ -1,292 +1,301 @@
--rw-r--r--   0        0        0    11357 2021-04-22 13:27:52.952758 fullctl-1.2.0/LICENSE
--rw-r--r--   0        0        0     1203 2023-04-15 17:47:54.744256 fullctl-1.2.0/README.md
--rw-r--r--   0        0        0     2223 2023-04-15 17:47:45.806100 fullctl-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.2.0/src/fullctl/__init__.py
--rwxr-xr-x   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.2.0/src/fullctl/django/__init__.py
--rw-r--r--   0        0        0     5587 2023-04-15 16:24:16.029446 fullctl-1.2.0/src/fullctl/django/admin.py
--rw-r--r--   0        0        0      259 2021-10-21 03:49:59.920722 fullctl-1.2.0/src/fullctl/django/apps.py
--rw-r--r--   0        0        0     7188 2023-02-27 05:27:02.246818 fullctl-1.2.0/src/fullctl/django/auditlog.py
--rw-r--r--   0        0        0     4863 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/auth.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.2.0/src/fullctl/django/autocomplete/__init__.py
--rw-r--r--   0        0        0      954 2023-02-27 05:27:02.247818 fullctl-1.2.0/src/fullctl/django/autocomplete/pdb.py
--rw-r--r--   0        0        0     2518 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/context.py
--rw-r--r--   0        0        0     3402 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/context_processors.py
--rw-r--r--   0        0        0     3102 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/decorators.py
--rw-r--r--   0        0        0      233 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/enum.py
--rw-r--r--   0        0        0      283 2022-10-14 13:57:25.205745 fullctl-1.2.0/src/fullctl/django/exceptions.py
--rw-r--r--   0        0        0      650 2022-10-14 13:57:25.205745 fullctl-1.2.0/src/fullctl/django/fields/__init__.py
--rw-r--r--   0        0        0     4351 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/fields/service_bridge/__init__.py
--rw-r--r--   0        0        0      317 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/fields/service_bridge/prefixctl.py
--rw-r--r--   0        0        0       79 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/forms.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.2.0/src/fullctl/django/inet/__init__.py
--rw-r--r--   0        0        0      325 2021-04-22 13:27:52.954758 fullctl-1.2.0/src/fullctl/django/inet/const.py
--rw-r--r--   0        0        0      186 2021-04-22 13:27:52.955758 fullctl-1.2.0/src/fullctl/django/inet/exceptions.py
--rw-r--r--   0        0        0      761 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/inet/fields.py
--rw-r--r--   0        0        0      519 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/inet/util.py
--rw-r--r--   0        0        0     3738 2021-06-15 13:03:05.246145 fullctl-1.2.0/src/fullctl/django/inet/validators.py
--rw-r--r--   0        0        0      307 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/mail.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.2.0/src/fullctl/django/management/__init__.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.2.0/src/fullctl/django/management/commands/__init__.py
--rw-r--r--   0        0        0     4128 2021-10-29 12:45:46.921418 fullctl-1.2.0/src/fullctl/django/management/commands/base.py
--rw-r--r--   0        0        0     1867 2023-02-27 05:27:02.248818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
--rw-r--r--   0        0        0     4750 2023-02-27 05:27:02.249818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py
--rw-r--r--   0        0        0      620 2023-02-27 05:27:02.249818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_promote_user.py
--rw-r--r--   0        0        0      763 2023-02-27 05:27:02.249818 fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_work_task.py
--rw-r--r--   0        0        0     3040 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/middleware.py
--rw-r--r--   0        0        0     8661 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0001_initial.py
--rw-r--r--   0        0        0      291 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0002_delete_apikey.py
--rw-r--r--   0        0        0     2216 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0003_auditlog.py
--rw-r--r--   0        0        0     1081 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py
--rw-r--r--   0        0        0      625 2023-02-27 05:27:02.250818 fullctl-1.2.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py
--rw-r--r--   0        0        0     1374 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py
--rw-r--r--   0        0        0      485 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0007_auditlog_ip_address.py
--rw-r--r--   0        0        0     4435 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0008_managementtask.py
--rw-r--r--   0        0        0     2341 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0009_taskclaim.py
--rw-r--r--   0        0        0      557 2023-02-27 05:27:02.251818 fullctl-1.2.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
--rw-r--r--   0        0        0      749 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py
--rw-r--r--   0        0        0     5399 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py
--rw-r--r--   0        0        0      723 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py
--rw-r--r--   0        0        0      516 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
--rw-r--r--   0        0        0      625 2023-02-27 05:27:02.252818 fullctl-1.2.0/src/fullctl/django/migrations/0015_alter_task_parent.py
--rw-r--r--   0        0        0      414 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0016_task_limit_id.py
--rw-r--r--   0        0        0      463 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
--rw-r--r--   0        0        0     4271 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0018_task_schedule.py
--rw-r--r--   0        0        0      402 2023-02-27 05:27:02.253818 fullctl-1.2.0/src/fullctl/django/migrations/0019_default_org.py
--rw-r--r--   0        0        0      389 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0020_auditlog_action_length.py
--rw-r--r--   0        0        0     3330 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0021_servicebridgeaction.py
--rw-r--r--   0        0        0     1077 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py
--rw-r--r--   0        0        0     1050 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py
--rw-r--r--   0        0        0     2539 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py
--rw-r--r--   0        0        0      900 2023-02-27 05:27:02.254818 fullctl-1.2.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py
--rw-r--r--   0        0        0      837 2023-02-27 05:27:02.255818 fullctl-1.2.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py
--rw-r--r--   0        0        0     4518 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0027_request_response.py
--rw-r--r--   0        0        0      457 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0028_request_identifier.py
--rw-r--r--   0        0        0      427 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0029_response_content.py
--rw-r--r--   0        0        0      550 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0030_alter_response_content.py
--rw-r--r--   0        0        0     2496 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.2.0/src/fullctl/django/migrations/__init__.py
--rw-r--r--   0        0        0      218 2021-10-21 03:49:59.989723 fullctl-1.2.0/src/fullctl/django/models/__init__.py
--rw-r--r--   0        0        0      150 2022-10-14 13:57:25.208745 fullctl-1.2.0/src/fullctl/django/models/abstract/__init__.py
--rw-r--r--   0        0        0     3282 2022-06-14 21:13:57.268730 fullctl-1.2.0/src/fullctl/django/models/abstract/alert.py
--rw-r--r--   0        0        0     3337 2022-10-14 13:57:25.209745 fullctl-1.2.0/src/fullctl/django/models/abstract/base.py
--rw-r--r--   0        0        0    13540 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/models/abstract/meta.py
--rw-r--r--   0        0        0     7822 2023-02-27 05:27:02.255818 fullctl-1.2.0/src/fullctl/django/models/abstract/service_bridge.py
--rw-r--r--   0        0        0     2682 2023-02-27 05:27:02.256818 fullctl-1.2.0/src/fullctl/django/models/abstract/template.py
--rw-r--r--   0        0        0      288 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/models/concrete/__init__.py
--rw-r--r--   0        0        0     7437 2023-02-27 05:27:02.256818 fullctl-1.2.0/src/fullctl/django/models/concrete/account.py
--rw-r--r--   0        0        0     1884 2023-02-27 05:27:02.256818 fullctl-1.2.0/src/fullctl/django/models/concrete/auditlog.py
--rw-r--r--   0        0        0     1808 2023-04-15 16:24:16.030446 fullctl-1.2.0/src/fullctl/django/models/concrete/meta.py
--rw-r--r--   0        0        0     7811 2023-02-27 05:27:02.257818 fullctl-1.2.0/src/fullctl/django/models/concrete/service_bridge.py
--rw-r--r--   0        0        0    16238 2023-04-15 16:24:16.031446 fullctl-1.2.0/src/fullctl/django/models/concrete/tasks.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.2.0/src/fullctl/django/rest/__init__.py
--rw-r--r--   0        0        0     8217 2023-02-27 05:27:02.257818 fullctl-1.2.0/src/fullctl/django/rest/api_schema.py
--rw-r--r--   0        0        0     1143 2021-10-29 12:45:46.966419 fullctl-1.2.0/src/fullctl/django/rest/authentication.py
--rw-r--r--   0        0        0     1831 2021-06-15 13:03:05.250145 fullctl-1.2.0/src/fullctl/django/rest/core.py
--rw-r--r--   0        0        0     8517 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/decorators.py
--rw-r--r--   0        0        0      328 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/fields.py
--rw-r--r--   0        0        0     1074 2021-10-21 03:50:00.023724 fullctl-1.2.0/src/fullctl/django/rest/filters.py
--rw-r--r--   0        0        0     1486 2022-10-14 13:57:25.257745 fullctl-1.2.0/src/fullctl/django/rest/mixins.py
--rw-r--r--   0        0        0     2148 2021-10-29 12:45:46.983419 fullctl-1.2.0/src/fullctl/django/rest/renderers.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.957758 fullctl-1.2.0/src/fullctl/django/rest/route/__init__.py
--rw-r--r--   0        0        0      352 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/route/aaactl_sync.py
--rw-r--r--   0        0        0      298 2021-10-21 03:50:00.070725 fullctl-1.2.0/src/fullctl/django/rest/route/account.py
--rw-r--r--   0        0        0      426 2023-02-27 05:27:02.258818 fullctl-1.2.0/src/fullctl/django/rest/route/service_bridge.py
--rw-r--r--   0        0        0      342 2023-02-27 05:27:02.259818 fullctl-1.2.0/src/fullctl/django/rest/route/usage.py
--rw-r--r--   0        0        0     1558 2023-02-27 05:27:02.259818 fullctl-1.2.0/src/fullctl/django/rest/serializers/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-15 16:24:16.031446 fullctl-1.2.0/src/fullctl/django/rest/serializers/aaactl_sync.py
--rw-r--r--   0        0        0     2523 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/serializers/account.py
--rw-r--r--   0        0        0      518 2023-04-15 16:24:16.032446 fullctl-1.2.0/src/fullctl/django/rest/serializers/meta.py
--rw-r--r--   0        0        0      807 2022-10-14 13:57:25.258745 fullctl-1.2.0/src/fullctl/django/rest/serializers/org.py
--rw-r--r--   0        0        0      233 2023-02-27 05:27:02.260818 fullctl-1.2.0/src/fullctl/django/rest/serializers/service_bridge.py
--rw-r--r--   0        0        0      688 2022-10-14 13:57:25.258745 fullctl-1.2.0/src/fullctl/django/rest/serializers/template.py
--rw-r--r--   0        0        0      440 2023-02-27 05:27:02.260818 fullctl-1.2.0/src/fullctl/django/rest/serializers/usage.py
--rw-r--r--   0        0        0      395 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/throttle.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0/src/fullctl/django/rest/urls/__init__.py
--rw-r--r--   0        0        0      222 2021-10-21 03:50:00.135727 fullctl-1.2.0/src/fullctl/django/rest/urls/aaactl_sync.py
--rw-r--r--   0        0        0      210 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/urls/account.py
--rw-r--r--   0        0        0      491 2021-10-29 12:45:46.983419 fullctl-1.2.0/src/fullctl/django/rest/urls/service_bridge.py
--rw-r--r--   0        0        0     2084 2023-02-27 05:27:02.260818 fullctl-1.2.0/src/fullctl/django/rest/urls/service_bridge_proxy.py
--rw-r--r--   0        0        0      204 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/urls/usage.py
--rw-r--r--   0        0        0      419 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/usage.py
--rw-r--r--   0        0        0        0 2021-06-15 13:03:05.251145 fullctl-1.2.0/src/fullctl/django/rest/views/__init__.py
--rw-r--r--   0        0        0     3258 2022-10-14 13:57:25.258745 fullctl-1.2.0/src/fullctl/django/rest/views/aaactl_sync.py
--rw-r--r--   0        0        0     2576 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/views/account.py
--rw-r--r--   0        0        0     7159 2023-04-15 17:32:55.630524 fullctl-1.2.0/src/fullctl/django/rest/views/service_bridge.py
--rw-r--r--   0        0        0      994 2023-02-27 05:27:02.261818 fullctl-1.2.0/src/fullctl/django/rest/views/template.py
--rw-r--r--   0        0        0     1410 2023-02-27 05:27:02.261818 fullctl-1.2.0/src/fullctl/django/rest/views/usage.py
--rw-r--r--   0        0        0    16282 2023-04-15 17:32:55.631524 fullctl-1.2.0/src/fullctl/django/settings/__init__.py
--rw-r--r--   0        0        0     2655 2023-02-27 05:27:02.262818 fullctl-1.2.0/src/fullctl/django/settings/default.py
--rw-r--r--   0        0        0     1215 2023-02-27 05:27:02.262818 fullctl-1.2.0/src/fullctl/django/signals.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0/src/fullctl/django/social/__init__.py
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0/src/fullctl/django/social/backends/__init__.py
--rw-r--r--   0        0        0     1206 2021-06-15 13:03:05.252145 fullctl-1.2.0/src/fullctl/django/social/backends/peeringdb.py
--rw-r--r--   0        0        0     1589 2021-10-21 03:50:00.137727 fullctl-1.2.0/src/fullctl/django/social/backends/twentyc.py
--rw-r--r--   0        0        0      388 2021-06-15 13:03:05.252145 fullctl-1.2.0/src/fullctl/django/social/pipelines/__init__.py
--rw-r--r--   0        0        0     4237 2021-04-22 13:27:52.959758 fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
--rw-r--r--   0        0        0    56503 2023-04-15 17:32:55.631524 fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.rest.js
--rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.959758 fullctl-1.2.0/src/fullctl/django/static/common/20c-logo-filled.svg
--rw-r--r--   0        0        0    21299 2023-02-27 05:27:02.264818 fullctl-1.2.0/src/fullctl/django/static/common/app.css
--rw-r--r--   0        0        0    19449 2023-02-27 05:27:02.265818 fullctl-1.2.0/src/fullctl/django/static/common/app.js
--rwxr-xr-x   0        0        0   372526 2021-10-29 12:45:47.007420 fullctl-1.2.0/src/fullctl/django/static/common/favicon.ico
--rw-r--r--   0        0        0     3380 2021-04-22 13:27:52.960758 fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
--rw-r--r--   0        0        0     3657 2021-04-22 13:27:52.960758 fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
--rw-r--r--   0        0        0     3430 2021-04-22 13:27:52.960758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/add.svg
--rw-r--r--   0        0        0     3819 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/alerts.svg
--rw-r--r--   0        0        0     2838 2022-06-14 21:13:57.362731 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/api.svg
--rw-r--r--   0        0        0     1303 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
--rw-r--r--   0        0        0     2681 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/delete.svg
--rw-r--r--   0        0        0     5490 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/edit.svg
--rwxr-xr-x   0        0        0     1172 2021-10-29 12:45:47.024420 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/launch.svg
--rw-r--r--   0        0        0     1601 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
--rw-r--r--   0        0        0     3357 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/list.svg
--rwxr-xr-x   0        0        0     1721 2022-06-14 21:13:57.362731 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/location.svg
--rw-r--r--   0        0        0     2617 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/logout.svg
--rwxr-xr-x   0        0        0      726 2021-10-29 12:45:47.026420 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/mail.svg
--rw-r--r--   0        0        0     2761 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/org.svg
--rw-r--r--   0        0        0     1597 2022-06-14 21:13:57.599734 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/refresh.svg
--rw-r--r--   0        0        0     1515 2022-06-14 21:13:57.623735 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/report.svg
--rw-r--r--   0        0        0     8263 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/settings.svg
--rw-r--r--   0        0        0     4138 2021-04-22 13:27:52.961758 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/user.svg
--rwxr-xr-x   0        0        0     2782 2021-10-29 12:45:47.035421 fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/view.svg
--rw-r--r--   0        0        0     3689 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      169 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-add.svg
--rw-r--r--   0        0        0      275 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-create.svg
--rw-r--r--   0        0        0      272 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-list-box.svg
--rw-r--r--   0        0        0      240 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/md-trash.svg
--rw-r--r--   0        0        0     5957 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      954 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
--rw-r--r--   0        0        0      818 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-close.svg
--rwxr-xr-x   0        0        0     2427 2023-02-27 05:27:02.266818 fullctl-1.2.0/src/fullctl/django/static/common/logos/aclctl-dark.svg
--rwxr-xr-x   0        0        0    36084 2023-04-15 16:24:16.033446 fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png
--rwxr-xr-x   0        0        0    36307 2023-04-15 16:24:16.033446 fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-light.png
--rwxr-xr-x   0        0        0     4680 2022-10-14 13:57:25.295745 fullctl-1.2.0/src/fullctl/django/static/common/logos/devicectl-dark.svg
--rwxr-xr-x   0        0        0     2579 2021-10-29 12:45:47.035421 fullctl-1.2.0/src/fullctl/django/static/common/logos/ixctl-dark.svg
--rwxr-xr-x   0        0        0     3857 2021-10-29 12:45:47.035421 fullctl-1.2.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg
--rwxr-xr-x   0        0        0     4166 2021-10-29 12:45:47.036420 fullctl-1.2.0/src/fullctl/django/static/common/logos/peerctl-dark.svg
--rwxr-xr-x   0        0        0     4336 2022-06-14 21:13:57.623735 fullctl-1.2.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg
--rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.962758 fullctl-1.2.0/src/fullctl/django/static/common/oauth/20c.svg
--rw-r--r--   0        0        0      689 2021-04-22 13:27:52.963758 fullctl-1.2.0/src/fullctl/django/static/common/oauth/google.svg
--rw-r--r--   0        0        0     5222 2023-04-15 16:24:16.033446 fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png
--rw-r--r--   0        0        0     9186 2021-04-22 13:27:52.963758 fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb.png
--rw-r--r--   0        0        0     4323 2021-10-21 03:50:00.180728 fullctl-1.2.0/src/fullctl/django/static/common/service_bridge.js
--rw-r--r--   0        0        0    11545 2023-02-27 05:27:02.266818 fullctl-1.2.0/src/fullctl/django/static/common/themes/dark.css
--rw-r--r--   0        0        0        0 2021-04-22 13:27:52.963758 fullctl-1.2.0/src/fullctl/django/static/common/themes/light.css
--rw-r--r--   0        0        0    25412 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/static/common/v2/app.css
--rw-r--r--   0        0        0    32037 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/static/common/v2/app.js
--rw-r--r--   0        0        0      644 2023-02-27 05:27:02.268818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/add.svg
--rw-r--r--   0        0        0     4812 2023-02-27 05:27:02.268818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/api.svg
--rw-r--r--   0        0        0      352 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
--rw-r--r--   0        0        0      232 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/arrow.svg
--rw-r--r--   0        0        0      532 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
--rw-r--r--   0        0        0      423 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/cancel.svg
--rw-r--r--   0        0        0      274 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/close.svg
--rw-r--r--   0        0        0     1229 2023-04-15 16:24:16.034446 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/database.svg
--rw-r--r--   0        0        0      427 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/download.svg
--rw-r--r--   0        0        0      438 2023-02-27 05:27:02.269818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/envelope.svg
--rw-r--r--   0        0        0      569 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/eye.svg
--rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
--rw-r--r--   0        0        0     1530 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/gear.svg
--rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/geo-alt.svg
--rw-r--r--   0        0        0     1975 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/help.svg
--rw-r--r--   0        0        0      582 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/delete.svg
--rw-r--r--   0        0        0      438 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/edit.svg
--rw-r--r--   0        0        0      818 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/options.svg
--rw-r--r--   0        0        0      447 2023-02-27 05:27:02.270818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list-ul.svg
--rw-r--r--   0        0        0      553 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/logout.svg
--rw-r--r--   0        0        0      749 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/org.svg
--rw-r--r--   0        0        0      331 2023-02-27 05:27:02.271818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/search.svg
--rw-r--r--   0        0        0     1465 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
--rw-r--r--   0        0        0      465 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
--rw-r--r--   0        0        0      190 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
--rw-r--r--   0        0        0     4138 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/user.svg
--rw-r--r--   0        0        0     3986 2023-02-27 05:27:02.272818 fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/view-settings.svg
--rw-r--r--   0        0        0    61189 2023-02-27 05:27:02.273818 fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/help.png
--rw-r--r--   0        0        0   426086 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png
--rw-r--r--   0        0        0    14637 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/static/common/v2/themes/dark.css
--rw-r--r--   0        0        0        0 2023-02-27 05:27:02.273818 fullctl-1.2.0/src/fullctl/django/static/common/v2/themes/light.css
--rw-r--r--   0        0        0      921 2023-02-27 05:27:02.274818 fullctl-1.2.0/src/fullctl/django/tasks/__init__.py
--rw-r--r--   0        0        0      740 2021-10-21 03:50:00.186728 fullctl-1.2.0/src/fullctl/django/tasks/celery.py
--rw-r--r--   0        0        0     2351 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/tasks/orm.py
--rw-r--r--   0        0        0     2220 2023-04-15 16:24:16.037446 fullctl-1.2.0/src/fullctl/django/tasks/qualifiers.py
--rw-r--r--   0        0        0      374 2023-02-27 05:27:02.274818 fullctl-1.2.0/src/fullctl/django/tasks/util.py
--rw-r--r--   0        0        0      658 2022-10-14 13:57:25.296744 fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/redoc.html
--rw-r--r--   0        0        0      856 2022-10-14 13:57:25.296744 fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/swagger.html
--rw-r--r--   0        0        0     8871 2022-10-14 13:57:25.296744 fullctl-1.2.0/src/fullctl/django/templates/common/app/base.html
--rw-r--r--   0        0        0      211 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/checkbox.html
--rw-r--r--   0        0        0     1935 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      726 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/invite.html
--rw-r--r--   0        0        0      792 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
--rw-r--r--   0        0        0      355 2021-06-15 13:03:05.254145 fullctl-1.2.0/src/fullctl/django/templates/common/app/index.html
--rw-r--r--   0        0        0     1974 2021-04-22 13:27:52.964758 fullctl-1.2.0/src/fullctl/django/templates/common/app/manage/permissions.html
--rw-r--r--   0        0        0     4752 2022-10-14 13:57:25.297744 fullctl-1.2.0/src/fullctl/django/templates/common/app/modal.html
--rw-r--r--   0        0        0     2668 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/app/navbar.html
--rw-r--r--   0        0        0      371 2023-02-27 05:27:02.275818 fullctl-1.2.0/src/fullctl/django/templates/common/app/templates.html
--rw-r--r--   0        0        0     3101 2022-10-14 13:57:25.297744 fullctl-1.2.0/src/fullctl/django/templates/common/auth/login.html
--rw-r--r--   0        0        0      880 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth-badge.html
--rw-r--r--   0        0        0     1110 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth.html
--rw-r--r--   0        0        0     1996 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/base.html
--rw-r--r--   0        0        0      333 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/400.html
--rw-r--r--   0        0        0      367 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/401.html
--rw-r--r--   0        0        0      375 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/403.html
--rw-r--r--   0        0        0      377 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/404.html
--rw-r--r--   0        0        0      456 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/500.html
--rw-r--r--   0        0        0      565 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/base.html
--rw-r--r--   0        0        0      351 2021-06-15 13:03:05.255145 fullctl-1.2.0/src/fullctl/django/templates/common/errors/details.html
--rw-r--r--   0        0        0     1229 2022-06-14 21:13:57.992740 fullctl-1.2.0/src/fullctl/django/templates/common/snippets.html
--rw-r--r--   0        0        0      234 2021-04-22 13:27:52.965758 fullctl-1.2.0/src/fullctl/django/templates/common/tool_base.html
--rw-r--r--   0        0        0      658 2023-02-27 05:27:02.276818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html
--rw-r--r--   0        0        0      856 2023-02-27 05:27:02.276818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html
--rw-r--r--   0        0        0    12217 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/base.html
--rw-r--r--   0        0        0      211 2023-02-27 05:27:02.277818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/checkbox.html
--rw-r--r--   0        0        0     2092 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
--rw-r--r--   0        0        0      357 2023-02-27 05:27:02.277818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/delete_selected.html
--rw-r--r--   0        0        0     1775 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/footer.html
--rw-r--r--   0        0        0     1935 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      430 2023-04-15 17:32:55.632524 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
--rw-r--r--   0        0        0      726 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/invite.html
--rw-r--r--   0        0        0      792 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2023-02-27 05:27:02.278818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
--rw-r--r--   0        0        0      358 2023-02-27 05:27:02.279818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/index.html
--rw-r--r--   0        0        0     1974 2023-02-27 05:27:02.279818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html
--rw-r--r--   0        0        0     6317 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/modal.html
--rw-r--r--   0        0        0     2668 2023-02-27 05:27:02.280818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/navbar.html
--rw-r--r--   0        0        0      413 2023-02-27 05:27:02.280818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/templates.html
--rw-r--r--   0        0        0     3048 2023-02-27 05:27:02.280818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/login.html
--rw-r--r--   0        0        0     1109 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
--rw-r--r--   0        0        0     1339 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth.html
--rw-r--r--   0        0        0     1977 2023-04-15 16:24:16.038446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/base.html
--rw-r--r--   0        0        0      339 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/400.html
--rw-r--r--   0        0        0      373 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/401.html
--rw-r--r--   0        0        0      381 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/403.html
--rw-r--r--   0        0        0      383 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/404.html
--rw-r--r--   0        0        0      462 2023-02-27 05:27:02.281818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/500.html
--rw-r--r--   0        0        0      568 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/base.html
--rw-r--r--   0        0        0      351 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/details.html
--rw-r--r--   0        0        0     1661 2023-04-15 16:24:16.039446 fullctl-1.2.0/src/fullctl/django/templates/common/v2/snippets.html
--rw-r--r--   0        0        0      234 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/tool_base.html
--rw-r--r--   0        0        0      249 2023-02-27 05:27:02.282818 fullctl-1.2.0/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
--rw-r--r--   0        0        0        0 2022-06-14 21:13:57.992740 fullctl-1.2.0/src/fullctl/django/templatetags/__init__.py
--rw-r--r--   0        0        0     3398 2023-04-15 16:24:16.039446 fullctl-1.2.0/src/fullctl/django/templatetags/fullctl_util.py
--rw-r--r--   0        0        0     3152 2023-02-27 05:27:02.283818 fullctl-1.2.0/src/fullctl/django/testutil.py
--rw-r--r--   0        0        0     3266 2023-04-15 17:32:55.633525 fullctl-1.2.0/src/fullctl/django/urls.py
--rw-r--r--   0        0        0     1171 2023-02-27 05:27:02.283818 fullctl-1.2.0/src/fullctl/django/util.py
--rw-r--r--   0        0        0     1193 2022-10-14 13:57:25.299744 fullctl-1.2.0/src/fullctl/django/validators.py
--rw-r--r--   0        0        0     2304 2023-02-27 05:27:02.284818 fullctl-1.2.0/src/fullctl/django/views/__init__.py
--rw-r--r--   0        0        0      199 2022-10-14 13:57:25.300744 fullctl-1.2.0/src/fullctl/django/views/api_schema.py
--rw-r--r--   0        0        0      927 2023-04-15 17:32:55.633525 fullctl-1.2.0/src/fullctl/django/views/template.py
--rw-r--r--   0        0        0        0 2021-06-15 13:03:05.256145 fullctl-1.2.0/src/fullctl/service_bridge/__init__.py
--rw-r--r--   0        0        0     2604 2023-04-15 17:32:55.633525 fullctl-1.2.0/src/fullctl/service_bridge/aaactl.py
--rw-r--r--   0        0        0     8510 2023-04-15 16:24:16.052446 fullctl-1.2.0/src/fullctl/service_bridge/client.py
--rw-r--r--   0        0        0     3419 2023-02-27 05:27:02.285818 fullctl-1.2.0/src/fullctl/service_bridge/data.py
--rw-r--r--   0        0        0     2180 2023-04-15 16:24:16.053446 fullctl-1.2.0/src/fullctl/service_bridge/devicectl.py
--rw-r--r--   0        0        0     2577 2023-04-15 16:24:16.053446 fullctl-1.2.0/src/fullctl/service_bridge/ixctl.py
--rw-r--r--   0        0        0     2651 2023-02-27 05:27:02.286818 fullctl-1.2.0/src/fullctl/service_bridge/nautobot.py
--rw-r--r--   0        0        0     1699 2023-04-15 16:24:16.054446 fullctl-1.2.0/src/fullctl/service_bridge/pdbctl.py
--rw-r--r--   0        0        0     1037 2023-04-15 16:24:16.063447 fullctl-1.2.0/src/fullctl/service_bridge/peerctl.py
--rw-r--r--   0        0        0     1076 2023-04-15 16:24:16.097447 fullctl-1.2.0/src/fullctl/service_bridge/prefixctl.py
--rw-r--r--   0        0        0     6952 2023-04-15 16:24:16.097447 fullctl-1.2.0/src/fullctl/service_bridge/sot.py
--rw-r--r--   0        0        0      323 2022-10-14 13:57:25.408743 fullctl-1.2.0/src/fullctl/utils/__init__.py
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 fullctl-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-04-22 13:27:52.952758 fullctl-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1203 2023-04-18 23:41:07.569197 fullctl-1.3.0/README.md
+-rw-r--r--   0        0        0     2223 2023-04-22 03:43:30.100693 fullctl-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.3.0/src/fullctl/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.3.0/src/fullctl/django/__init__.py
+-rw-r--r--   0        0        0     5587 2023-04-15 16:24:16.029446 fullctl-1.3.0/src/fullctl/django/admin.py
+-rw-r--r--   0        0        0      259 2021-10-21 03:49:59.920722 fullctl-1.3.0/src/fullctl/django/apps.py
+-rw-r--r--   0        0        0     7188 2023-02-27 05:27:02.246818 fullctl-1.3.0/src/fullctl/django/auditlog.py
+-rw-r--r--   0        0        0     4863 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/auth.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.3.0/src/fullctl/django/autocomplete/__init__.py
+-rw-r--r--   0        0        0      954 2023-02-27 05:27:02.247818 fullctl-1.3.0/src/fullctl/django/autocomplete/pdb.py
+-rw-r--r--   0        0        0     2518 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/context.py
+-rw-r--r--   0        0        0     3402 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/context_processors.py
+-rw-r--r--   0        0        0     3102 2023-04-15 17:32:55.630524 fullctl-1.3.0/src/fullctl/django/decorators.py
+-rw-r--r--   0        0        0      233 2023-04-15 17:32:55.630524 fullctl-1.3.0/src/fullctl/django/enum.py
+-rw-r--r--   0        0        0      283 2022-10-14 13:57:25.205745 fullctl-1.3.0/src/fullctl/django/exceptions.py
+-rw-r--r--   0        0        0      650 2022-10-14 13:57:25.205745 fullctl-1.3.0/src/fullctl/django/fields/__init__.py
+-rw-r--r--   0        0        0     4351 2023-02-27 05:27:02.248818 fullctl-1.3.0/src/fullctl/django/fields/service_bridge/__init__.py
+-rw-r--r--   0        0        0      317 2023-02-27 05:27:02.248818 fullctl-1.3.0/src/fullctl/django/fields/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0       79 2021-06-15 13:03:05.246145 fullctl-1.3.0/src/fullctl/django/forms.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.3.0/src/fullctl/django/inet/__init__.py
+-rw-r--r--   0        0        0      325 2021-04-22 13:27:52.954758 fullctl-1.3.0/src/fullctl/django/inet/const.py
+-rw-r--r--   0        0        0      186 2021-04-22 13:27:52.955758 fullctl-1.3.0/src/fullctl/django/inet/exceptions.py
+-rw-r--r--   0        0        0      761 2021-06-15 13:03:05.246145 fullctl-1.3.0/src/fullctl/django/inet/fields.py
+-rw-r--r--   0        0        0      519 2021-06-15 13:03:05.246145 fullctl-1.3.0/src/fullctl/django/inet/util.py
+-rw-r--r--   0        0        0     3738 2021-06-15 13:03:05.246145 fullctl-1.3.0/src/fullctl/django/inet/validators.py
+-rw-r--r--   0        0        0      307 2023-02-27 05:27:02.248818 fullctl-1.3.0/src/fullctl/django/mail.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.3.0/src/fullctl/django/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.3.0/src/fullctl/django/management/commands/__init__.py
+-rw-r--r--   0        0        0     4128 2021-10-29 12:45:46.921418 fullctl-1.3.0/src/fullctl/django/management/commands/base.py
+-rw-r--r--   0        0        0     1867 2023-02-27 05:27:02.248818 fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
+-rw-r--r--   0        0        0     4750 2023-02-27 05:27:02.249818 fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py
+-rw-r--r--   0        0        0      620 2023-02-27 05:27:02.249818 fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_promote_user.py
+-rw-r--r--   0        0        0      763 2023-02-27 05:27:02.249818 fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_work_task.py
+-rw-r--r--   0        0        0     3040 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/middleware.py
+-rw-r--r--   0        0        0     8661 2023-02-27 05:27:02.250818 fullctl-1.3.0/src/fullctl/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0      291 2023-02-27 05:27:02.250818 fullctl-1.3.0/src/fullctl/django/migrations/0002_delete_apikey.py
+-rw-r--r--   0        0        0     2216 2023-02-27 05:27:02.250818 fullctl-1.3.0/src/fullctl/django/migrations/0003_auditlog.py
+-rw-r--r--   0        0        0     1081 2023-02-27 05:27:02.250818 fullctl-1.3.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py
+-rw-r--r--   0        0        0      625 2023-02-27 05:27:02.250818 fullctl-1.3.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py
+-rw-r--r--   0        0        0     1374 2023-02-27 05:27:02.251818 fullctl-1.3.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py
+-rw-r--r--   0        0        0      485 2023-02-27 05:27:02.251818 fullctl-1.3.0/src/fullctl/django/migrations/0007_auditlog_ip_address.py
+-rw-r--r--   0        0        0     4435 2023-02-27 05:27:02.251818 fullctl-1.3.0/src/fullctl/django/migrations/0008_managementtask.py
+-rw-r--r--   0        0        0     2341 2023-02-27 05:27:02.251818 fullctl-1.3.0/src/fullctl/django/migrations/0009_taskclaim.py
+-rw-r--r--   0        0        0      557 2023-02-27 05:27:02.251818 fullctl-1.3.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
+-rw-r--r--   0        0        0      749 2023-02-27 05:27:02.252818 fullctl-1.3.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py
+-rw-r--r--   0        0        0     5399 2023-02-27 05:27:02.252818 fullctl-1.3.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py
+-rw-r--r--   0        0        0      723 2023-02-27 05:27:02.252818 fullctl-1.3.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py
+-rw-r--r--   0        0        0      516 2023-02-27 05:27:02.252818 fullctl-1.3.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
+-rw-r--r--   0        0        0      625 2023-02-27 05:27:02.252818 fullctl-1.3.0/src/fullctl/django/migrations/0015_alter_task_parent.py
+-rw-r--r--   0        0        0      414 2023-02-27 05:27:02.253818 fullctl-1.3.0/src/fullctl/django/migrations/0016_task_limit_id.py
+-rw-r--r--   0        0        0      463 2023-02-27 05:27:02.253818 fullctl-1.3.0/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
+-rw-r--r--   0        0        0     4271 2023-02-27 05:27:02.253818 fullctl-1.3.0/src/fullctl/django/migrations/0018_task_schedule.py
+-rw-r--r--   0        0        0      402 2023-02-27 05:27:02.253818 fullctl-1.3.0/src/fullctl/django/migrations/0019_default_org.py
+-rw-r--r--   0        0        0      389 2023-02-27 05:27:02.254818 fullctl-1.3.0/src/fullctl/django/migrations/0020_auditlog_action_length.py
+-rw-r--r--   0        0        0     3330 2023-02-27 05:27:02.254818 fullctl-1.3.0/src/fullctl/django/migrations/0021_servicebridgeaction.py
+-rw-r--r--   0        0        0     1077 2023-02-27 05:27:02.254818 fullctl-1.3.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py
+-rw-r--r--   0        0        0     1050 2023-02-27 05:27:02.254818 fullctl-1.3.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py
+-rw-r--r--   0        0        0     2539 2023-02-27 05:27:02.254818 fullctl-1.3.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py
+-rw-r--r--   0        0        0      900 2023-02-27 05:27:02.254818 fullctl-1.3.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py
+-rw-r--r--   0        0        0      837 2023-02-27 05:27:02.255818 fullctl-1.3.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py
+-rw-r--r--   0        0        0     4518 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/migrations/0027_request_response.py
+-rw-r--r--   0        0        0      457 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/migrations/0028_request_identifier.py
+-rw-r--r--   0        0        0      427 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/migrations/0029_response_content.py
+-rw-r--r--   0        0        0      550 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/migrations/0030_alter_response_content.py
+-rw-r--r--   0        0        0     2496 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.3.0/src/fullctl/django/migrations/__init__.py
+-rw-r--r--   0        0        0      218 2021-10-21 03:49:59.989723 fullctl-1.3.0/src/fullctl/django/models/__init__.py
+-rw-r--r--   0        0        0      150 2022-10-14 13:57:25.208745 fullctl-1.3.0/src/fullctl/django/models/abstract/__init__.py
+-rw-r--r--   0        0        0     3282 2022-06-14 21:13:57.268730 fullctl-1.3.0/src/fullctl/django/models/abstract/alert.py
+-rw-r--r--   0        0        0     3337 2022-10-14 13:57:25.209745 fullctl-1.3.0/src/fullctl/django/models/abstract/base.py
+-rw-r--r--   0        0        0    13813 2023-04-22 03:42:18.731445 fullctl-1.3.0/src/fullctl/django/models/abstract/meta.py
+-rw-r--r--   0        0        0     7822 2023-02-27 05:27:02.255818 fullctl-1.3.0/src/fullctl/django/models/abstract/service_bridge.py
+-rw-r--r--   0        0        0     2682 2023-02-27 05:27:02.256818 fullctl-1.3.0/src/fullctl/django/models/abstract/template.py
+-rw-r--r--   0        0        0      288 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/models/concrete/__init__.py
+-rw-r--r--   0        0        0     7437 2023-02-27 05:27:02.256818 fullctl-1.3.0/src/fullctl/django/models/concrete/account.py
+-rw-r--r--   0        0        0     1884 2023-02-27 05:27:02.256818 fullctl-1.3.0/src/fullctl/django/models/concrete/auditlog.py
+-rw-r--r--   0        0        0     1808 2023-04-15 16:24:16.030446 fullctl-1.3.0/src/fullctl/django/models/concrete/meta.py
+-rw-r--r--   0        0        0     7811 2023-02-27 05:27:02.257818 fullctl-1.3.0/src/fullctl/django/models/concrete/service_bridge.py
+-rw-r--r--   0        0        0    16238 2023-04-15 16:24:16.031446 fullctl-1.3.0/src/fullctl/django/models/concrete/tasks.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.3.0/src/fullctl/django/rest/__init__.py
+-rw-r--r--   0        0        0     8217 2023-02-27 05:27:02.257818 fullctl-1.3.0/src/fullctl/django/rest/api_schema.py
+-rw-r--r--   0        0        0     1143 2021-10-29 12:45:46.966419 fullctl-1.3.0/src/fullctl/django/rest/authentication.py
+-rw-r--r--   0        0        0     1831 2021-06-15 13:03:05.250145 fullctl-1.3.0/src/fullctl/django/rest/core.py
+-rw-r--r--   0        0        0     8517 2023-02-27 05:27:02.258818 fullctl-1.3.0/src/fullctl/django/rest/decorators.py
+-rw-r--r--   0        0        0      328 2023-02-27 05:27:02.258818 fullctl-1.3.0/src/fullctl/django/rest/fields.py
+-rw-r--r--   0        0        0     1074 2021-10-21 03:50:00.023724 fullctl-1.3.0/src/fullctl/django/rest/filters.py
+-rw-r--r--   0        0        0     1486 2022-10-14 13:57:25.257745 fullctl-1.3.0/src/fullctl/django/rest/mixins.py
+-rw-r--r--   0        0        0     2148 2021-10-29 12:45:46.983419 fullctl-1.3.0/src/fullctl/django/rest/renderers.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.957758 fullctl-1.3.0/src/fullctl/django/rest/route/__init__.py
+-rw-r--r--   0        0        0      352 2023-02-27 05:27:02.258818 fullctl-1.3.0/src/fullctl/django/rest/route/aaactl_sync.py
+-rw-r--r--   0        0        0      298 2021-10-21 03:50:00.070725 fullctl-1.3.0/src/fullctl/django/rest/route/account.py
+-rw-r--r--   0        0        0      426 2023-02-27 05:27:02.258818 fullctl-1.3.0/src/fullctl/django/rest/route/service_bridge.py
+-rw-r--r--   0        0        0      342 2023-02-27 05:27:02.259818 fullctl-1.3.0/src/fullctl/django/rest/route/usage.py
+-rw-r--r--   0        0        0     1558 2023-02-27 05:27:02.259818 fullctl-1.3.0/src/fullctl/django/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-15 16:24:16.031446 fullctl-1.3.0/src/fullctl/django/rest/serializers/aaactl_sync.py
+-rw-r--r--   0        0        0     2523 2023-04-15 17:32:55.630524 fullctl-1.3.0/src/fullctl/django/rest/serializers/account.py
+-rw-r--r--   0        0        0      518 2023-04-15 16:24:16.032446 fullctl-1.3.0/src/fullctl/django/rest/serializers/meta.py
+-rw-r--r--   0        0        0      807 2022-10-14 13:57:25.258745 fullctl-1.3.0/src/fullctl/django/rest/serializers/org.py
+-rw-r--r--   0        0        0      233 2023-02-27 05:27:02.260818 fullctl-1.3.0/src/fullctl/django/rest/serializers/service_bridge.py
+-rw-r--r--   0        0        0      688 2022-10-14 13:57:25.258745 fullctl-1.3.0/src/fullctl/django/rest/serializers/template.py
+-rw-r--r--   0        0        0      440 2023-02-27 05:27:02.260818 fullctl-1.3.0/src/fullctl/django/rest/serializers/usage.py
+-rw-r--r--   0        0        0      395 2023-04-15 17:32:55.630524 fullctl-1.3.0/src/fullctl/django/rest/throttle.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.3.0/src/fullctl/django/rest/urls/__init__.py
+-rw-r--r--   0        0        0      222 2021-10-21 03:50:00.135727 fullctl-1.3.0/src/fullctl/django/rest/urls/aaactl_sync.py
+-rw-r--r--   0        0        0      210 2021-06-15 13:03:05.251145 fullctl-1.3.0/src/fullctl/django/rest/urls/account.py
+-rw-r--r--   0        0        0      491 2021-10-29 12:45:46.983419 fullctl-1.3.0/src/fullctl/django/rest/urls/service_bridge.py
+-rw-r--r--   0        0        0     2084 2023-02-27 05:27:02.260818 fullctl-1.3.0/src/fullctl/django/rest/urls/service_bridge_proxy.py
+-rw-r--r--   0        0        0      204 2021-06-15 13:03:05.251145 fullctl-1.3.0/src/fullctl/django/rest/urls/usage.py
+-rw-r--r--   0        0        0      419 2021-06-15 13:03:05.251145 fullctl-1.3.0/src/fullctl/django/rest/usage.py
+-rw-r--r--   0        0        0        0 2021-06-15 13:03:05.251145 fullctl-1.3.0/src/fullctl/django/rest/views/__init__.py
+-rw-r--r--   0        0        0     3258 2022-10-14 13:57:25.258745 fullctl-1.3.0/src/fullctl/django/rest/views/aaactl_sync.py
+-rw-r--r--   0        0        0     2576 2023-04-15 17:32:55.630524 fullctl-1.3.0/src/fullctl/django/rest/views/account.py
+-rw-r--r--   0        0        0     7159 2023-04-15 17:32:55.630524 fullctl-1.3.0/src/fullctl/django/rest/views/service_bridge.py
+-rw-r--r--   0        0        0      994 2023-02-27 05:27:02.261818 fullctl-1.3.0/src/fullctl/django/rest/views/template.py
+-rw-r--r--   0        0        0     1410 2023-02-27 05:27:02.261818 fullctl-1.3.0/src/fullctl/django/rest/views/usage.py
+-rw-r--r--   0        0        0    16414 2023-04-22 03:42:18.731445 fullctl-1.3.0/src/fullctl/django/settings/__init__.py
+-rw-r--r--   0        0        0     2655 2023-02-27 05:27:02.262818 fullctl-1.3.0/src/fullctl/django/settings/default.py
+-rw-r--r--   0        0        0     1215 2023-02-27 05:27:02.262818 fullctl-1.3.0/src/fullctl/django/signals.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.3.0/src/fullctl/django/social/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.3.0/src/fullctl/django/social/backends/__init__.py
+-rw-r--r--   0        0        0     1206 2021-06-15 13:03:05.252145 fullctl-1.3.0/src/fullctl/django/social/backends/peeringdb.py
+-rw-r--r--   0        0        0     1589 2021-10-21 03:50:00.137727 fullctl-1.3.0/src/fullctl/django/social/backends/twentyc.py
+-rw-r--r--   0        0        0      388 2021-06-15 13:03:05.252145 fullctl-1.3.0/src/fullctl/django/social/pipelines/__init__.py
+-rw-r--r--   0        0        0     4237 2021-04-22 13:27:52.959758 fullctl-1.3.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
+-rw-r--r--   0        0        0    56535 2023-04-22 03:42:18.731445 fullctl-1.3.0/src/fullctl/django/static/common/20c/twentyc.rest.js
+-rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.959758 fullctl-1.3.0/src/fullctl/django/static/common/20c-logo-filled.svg
+-rw-r--r--   0        0        0    21299 2023-02-27 05:27:02.264818 fullctl-1.3.0/src/fullctl/django/static/common/app.css
+-rw-r--r--   0        0        0    19449 2023-02-27 05:27:02.265818 fullctl-1.3.0/src/fullctl/django/static/common/app.js
+-rwxr-xr-x   0        0        0   372526 2021-10-29 12:45:47.007420 fullctl-1.3.0/src/fullctl/django/static/common/favicon.ico
+-rw-r--r--   0        0        0     3380 2021-04-22 13:27:52.960758 fullctl-1.3.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
+-rw-r--r--   0        0        0     3657 2021-04-22 13:27:52.960758 fullctl-1.3.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
+-rw-r--r--   0        0        0     3430 2021-04-22 13:27:52.960758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/add.svg
+-rw-r--r--   0        0        0     3819 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/alerts.svg
+-rw-r--r--   0        0        0     2838 2022-06-14 21:13:57.362731 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/api.svg
+-rw-r--r--   0        0        0     1303 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
+-rw-r--r--   0        0        0     2681 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/delete.svg
+-rw-r--r--   0        0        0     5490 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/edit.svg
+-rwxr-xr-x   0        0        0     1172 2021-10-29 12:45:47.024420 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/launch.svg
+-rw-r--r--   0        0        0     1601 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
+-rw-r--r--   0        0        0     3357 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/list.svg
+-rwxr-xr-x   0        0        0     1721 2022-06-14 21:13:57.362731 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/location.svg
+-rw-r--r--   0        0        0     2617 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/logout.svg
+-rwxr-xr-x   0        0        0      726 2021-10-29 12:45:47.026420 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/mail.svg
+-rw-r--r--   0        0        0     2761 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/org.svg
+-rw-r--r--   0        0        0     1597 2022-06-14 21:13:57.599734 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/refresh.svg
+-rw-r--r--   0        0        0     1515 2022-06-14 21:13:57.623735 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/report.svg
+-rw-r--r--   0        0        0     8263 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/settings.svg
+-rw-r--r--   0        0        0     4138 2021-04-22 13:27:52.961758 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/user.svg
+-rwxr-xr-x   0        0        0     2782 2021-10-29 12:45:47.035421 fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/view.svg
+-rw-r--r--   0        0        0     3689 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      169 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/md-add.svg
+-rw-r--r--   0        0        0      275 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/md-create.svg
+-rw-r--r--   0        0        0      272 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/md-list-box.svg
+-rw-r--r--   0        0        0      240 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/md-trash.svg
+-rw-r--r--   0        0        0     5957 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      954 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
+-rw-r--r--   0        0        0      818 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/icons/ui-close.svg
+-rwxr-xr-x   0        0        0     2427 2023-02-27 05:27:02.266818 fullctl-1.3.0/src/fullctl/django/static/common/logos/aclctl-dark.svg
+-rw-r--r--   0        0        0     2625 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/aclctl-light.svg
+-rwxr-xr-x   0        0        0     3333 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/auditctl-dark.svg
+-rwxr-xr-x   0        0        0     3333 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/auditctl-light.svg
+-rwxr-xr-x   0        0        0    36084 2023-04-15 16:24:16.033446 fullctl-1.3.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png
+-rwxr-xr-x   0        0        0    36307 2023-04-15 16:24:16.033446 fullctl-1.3.0/src/fullctl/django/static/common/logos/ctl-mark-light.png
+-rwxr-xr-x   0        0        0     4680 2022-10-14 13:57:25.295745 fullctl-1.3.0/src/fullctl/django/static/common/logos/devicectl-dark.svg
+-rw-r--r--   0        0        0     4682 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/devicectl-light.svg
+-rwxr-xr-x   0        0        0     2579 2021-10-29 12:45:47.035421 fullctl-1.3.0/src/fullctl/django/static/common/logos/ixctl-dark.svg
+-rw-r--r--   0        0        0     2581 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/ixctl-light.svg
+-rwxr-xr-x   0        0        0     3857 2021-10-29 12:45:47.035421 fullctl-1.3.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg
+-rw-r--r--   0        0        0     3859 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/pdbctl-light.svg
+-rwxr-xr-x   0        0        0     4166 2021-10-29 12:45:47.036420 fullctl-1.3.0/src/fullctl/django/static/common/logos/peerctl-dark.svg
+-rw-r--r--   0        0        0     4168 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/peerctl-light.svg
+-rwxr-xr-x   0        0        0     4336 2022-06-14 21:13:57.623735 fullctl-1.3.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg
+-rw-r--r--   0        0        0     4338 2023-04-22 03:42:18.732445 fullctl-1.3.0/src/fullctl/django/static/common/logos/prefixctl-light.svg
+-rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.962758 fullctl-1.3.0/src/fullctl/django/static/common/oauth/20c.svg
+-rw-r--r--   0        0        0      689 2021-04-22 13:27:52.963758 fullctl-1.3.0/src/fullctl/django/static/common/oauth/google.svg
+-rw-r--r--   0        0        0     5222 2023-04-15 16:24:16.033446 fullctl-1.3.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png
+-rw-r--r--   0        0        0     9186 2021-04-22 13:27:52.963758 fullctl-1.3.0/src/fullctl/django/static/common/oauth/peeringdb.png
+-rw-r--r--   0        0        0     4323 2021-10-21 03:50:00.180728 fullctl-1.3.0/src/fullctl/django/static/common/service_bridge.js
+-rw-r--r--   0        0        0    11545 2023-02-27 05:27:02.266818 fullctl-1.3.0/src/fullctl/django/static/common/themes/dark.css
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.963758 fullctl-1.3.0/src/fullctl/django/static/common/themes/light.css
+-rw-r--r--   0        0        0    25412 2023-04-15 17:32:55.632524 fullctl-1.3.0/src/fullctl/django/static/common/v2/app.css
+-rw-r--r--   0        0        0    32037 2023-04-15 17:32:55.632524 fullctl-1.3.0/src/fullctl/django/static/common/v2/app.js
+-rw-r--r--   0        0        0      644 2023-02-27 05:27:02.268818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/add.svg
+-rw-r--r--   0        0        0     4812 2023-02-27 05:27:02.268818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/api.svg
+-rw-r--r--   0        0        0      352 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
+-rw-r--r--   0        0        0      232 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/arrow.svg
+-rw-r--r--   0        0        0      532 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
+-rw-r--r--   0        0        0      423 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/cancel.svg
+-rw-r--r--   0        0        0      274 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/close.svg
+-rw-r--r--   0        0        0     1229 2023-04-15 16:24:16.034446 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/database.svg
+-rw-r--r--   0        0        0      427 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/download.svg
+-rw-r--r--   0        0        0      438 2023-02-27 05:27:02.269818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/envelope.svg
+-rw-r--r--   0        0        0      569 2023-02-27 05:27:02.270818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/eye.svg
+-rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
+-rw-r--r--   0        0        0     1530 2023-02-27 05:27:02.270818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/gear.svg
+-rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/geo-alt.svg
+-rw-r--r--   0        0        0     1975 2023-02-27 05:27:02.270818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/help.svg
+-rw-r--r--   0        0        0      582 2023-02-27 05:27:02.271818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/list/delete.svg
+-rw-r--r--   0        0        0      438 2023-02-27 05:27:02.271818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/list/edit.svg
+-rw-r--r--   0        0        0      818 2023-02-27 05:27:02.271818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/list/options.svg
+-rw-r--r--   0        0        0      447 2023-02-27 05:27:02.270818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/list-ul.svg
+-rw-r--r--   0        0        0      553 2023-02-27 05:27:02.271818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/logout.svg
+-rw-r--r--   0        0        0      749 2023-02-27 05:27:02.271818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/org.svg
+-rw-r--r--   0        0        0      331 2023-02-27 05:27:02.271818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/search.svg
+-rw-r--r--   0        0        0     1465 2023-02-27 05:27:02.272818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
+-rw-r--r--   0        0        0      465 2023-02-27 05:27:02.272818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
+-rw-r--r--   0        0        0      190 2023-02-27 05:27:02.272818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
+-rw-r--r--   0        0        0     4138 2023-02-27 05:27:02.272818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/user.svg
+-rw-r--r--   0        0        0     3986 2023-02-27 05:27:02.272818 fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/view-settings.svg
+-rw-r--r--   0        0        0    61189 2023-02-27 05:27:02.273818 fullctl-1.3.0/src/fullctl/django/static/common/v2/imgs/help.png
+-rw-r--r--   0        0        0   426086 2023-04-15 16:24:16.037446 fullctl-1.3.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png
+-rw-r--r--   0        0        0    14637 2023-04-15 16:24:16.037446 fullctl-1.3.0/src/fullctl/django/static/common/v2/themes/dark.css
+-rw-r--r--   0        0        0        0 2023-02-27 05:27:02.273818 fullctl-1.3.0/src/fullctl/django/static/common/v2/themes/light.css
+-rw-r--r--   0        0        0      921 2023-02-27 05:27:02.274818 fullctl-1.3.0/src/fullctl/django/tasks/__init__.py
+-rw-r--r--   0        0        0      740 2021-10-21 03:50:00.186728 fullctl-1.3.0/src/fullctl/django/tasks/celery.py
+-rw-r--r--   0        0        0     2351 2023-04-15 16:24:16.037446 fullctl-1.3.0/src/fullctl/django/tasks/orm.py
+-rw-r--r--   0        0        0     2232 2023-04-22 03:42:18.733445 fullctl-1.3.0/src/fullctl/django/tasks/qualifiers.py
+-rw-r--r--   0        0        0      374 2023-02-27 05:27:02.274818 fullctl-1.3.0/src/fullctl/django/tasks/util.py
+-rw-r--r--   0        0        0      658 2022-10-14 13:57:25.296744 fullctl-1.3.0/src/fullctl/django/templates/common/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2022-10-14 13:57:25.296744 fullctl-1.3.0/src/fullctl/django/templates/common/apidocs/swagger.html
+-rw-r--r--   0        0        0     8871 2022-10-14 13:57:25.296744 fullctl-1.3.0/src/fullctl/django/templates/common/app/base.html
+-rw-r--r--   0        0        0      211 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/checkbox.html
+-rw-r--r--   0        0        0     1935 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      726 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      355 2021-06-15 13:03:05.254145 fullctl-1.3.0/src/fullctl/django/templates/common/app/index.html
+-rw-r--r--   0        0        0     1974 2021-04-22 13:27:52.964758 fullctl-1.3.0/src/fullctl/django/templates/common/app/manage/permissions.html
+-rw-r--r--   0        0        0     4752 2022-10-14 13:57:25.297744 fullctl-1.3.0/src/fullctl/django/templates/common/app/modal.html
+-rw-r--r--   0        0        0     2668 2021-04-22 13:27:52.965758 fullctl-1.3.0/src/fullctl/django/templates/common/app/navbar.html
+-rw-r--r--   0        0        0      371 2023-02-27 05:27:02.275818 fullctl-1.3.0/src/fullctl/django/templates/common/app/templates.html
+-rw-r--r--   0        0        0     3101 2022-10-14 13:57:25.297744 fullctl-1.3.0/src/fullctl/django/templates/common/auth/login.html
+-rw-r--r--   0        0        0      880 2021-04-22 13:27:52.965758 fullctl-1.3.0/src/fullctl/django/templates/common/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1110 2021-04-22 13:27:52.965758 fullctl-1.3.0/src/fullctl/django/templates/common/auth/oauth.html
+-rw-r--r--   0        0        0     1996 2023-04-15 16:24:16.038446 fullctl-1.3.0/src/fullctl/django/templates/common/base.html
+-rw-r--r--   0        0        0      333 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/400.html
+-rw-r--r--   0        0        0      367 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/401.html
+-rw-r--r--   0        0        0      375 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/403.html
+-rw-r--r--   0        0        0      377 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/404.html
+-rw-r--r--   0        0        0      456 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/500.html
+-rw-r--r--   0        0        0      565 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/base.html
+-rw-r--r--   0        0        0      351 2021-06-15 13:03:05.255145 fullctl-1.3.0/src/fullctl/django/templates/common/errors/details.html
+-rw-r--r--   0        0        0     1229 2022-06-14 21:13:57.992740 fullctl-1.3.0/src/fullctl/django/templates/common/snippets.html
+-rw-r--r--   0        0        0      234 2021-04-22 13:27:52.965758 fullctl-1.3.0/src/fullctl/django/templates/common/tool_base.html
+-rw-r--r--   0        0        0      658 2023-02-27 05:27:02.276818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2023-02-27 05:27:02.276818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html
+-rw-r--r--   0        0        0    12217 2023-04-15 17:32:55.632524 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/base.html
+-rw-r--r--   0        0        0      211 2023-02-27 05:27:02.277818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/checkbox.html
+-rw-r--r--   0        0        0     2092 2023-04-15 17:32:55.632524 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
+-rw-r--r--   0        0        0      357 2023-02-27 05:27:02.277818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/delete_selected.html
+-rw-r--r--   0        0        0     1945 2023-04-22 03:42:18.733445 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/footer.html
+-rw-r--r--   0        0        0     1935 2023-02-27 05:27:02.278818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      430 2023-04-15 17:32:55.632524 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
+-rw-r--r--   0        0        0      726 2023-02-27 05:27:02.278818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2023-02-27 05:27:02.278818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2023-02-27 05:27:02.278818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2023-02-27 05:27:02.278818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      358 2023-02-27 05:27:02.279818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/index.html
+-rw-r--r--   0        0        0     1974 2023-02-27 05:27:02.279818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html
+-rw-r--r--   0        0        0     6317 2023-04-15 16:24:16.038446 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/modal.html
+-rw-r--r--   0        0        0     2668 2023-02-27 05:27:02.280818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/navbar.html
+-rw-r--r--   0        0        0      413 2023-02-27 05:27:02.280818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/templates.html
+-rw-r--r--   0        0        0     3048 2023-02-27 05:27:02.280818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/auth/login.html
+-rw-r--r--   0        0        0     1109 2023-04-15 16:24:16.038446 fullctl-1.3.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1339 2023-04-15 16:24:16.038446 fullctl-1.3.0/src/fullctl/django/templates/common/v2/auth/oauth.html
+-rw-r--r--   0        0        0     1977 2023-04-15 16:24:16.038446 fullctl-1.3.0/src/fullctl/django/templates/common/v2/base.html
+-rw-r--r--   0        0        0      339 2023-02-27 05:27:02.281818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/400.html
+-rw-r--r--   0        0        0      373 2023-02-27 05:27:02.281818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/401.html
+-rw-r--r--   0        0        0      381 2023-02-27 05:27:02.281818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/403.html
+-rw-r--r--   0        0        0      383 2023-02-27 05:27:02.281818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/404.html
+-rw-r--r--   0        0        0      462 2023-02-27 05:27:02.281818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/500.html
+-rw-r--r--   0        0        0      568 2023-02-27 05:27:02.282818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/base.html
+-rw-r--r--   0        0        0      351 2023-02-27 05:27:02.282818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/details.html
+-rw-r--r--   0        0        0     1661 2023-04-15 16:24:16.039446 fullctl-1.3.0/src/fullctl/django/templates/common/v2/snippets.html
+-rw-r--r--   0        0        0      234 2023-02-27 05:27:02.282818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/tool_base.html
+-rw-r--r--   0        0        0      249 2023-02-27 05:27:02.282818 fullctl-1.3.0/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
+-rw-r--r--   0        0        0        0 2022-06-14 21:13:57.992740 fullctl-1.3.0/src/fullctl/django/templatetags/__init__.py
+-rw-r--r--   0        0        0     3398 2023-04-15 16:24:16.039446 fullctl-1.3.0/src/fullctl/django/templatetags/fullctl_util.py
+-rw-r--r--   0        0        0     3152 2023-02-27 05:27:02.283818 fullctl-1.3.0/src/fullctl/django/testutil.py
+-rw-r--r--   0        0        0     3321 2023-04-22 03:42:18.733445 fullctl-1.3.0/src/fullctl/django/urls.py
+-rw-r--r--   0        0        0     1171 2023-02-27 05:27:02.283818 fullctl-1.3.0/src/fullctl/django/util.py
+-rw-r--r--   0        0        0     1193 2022-10-14 13:57:25.299744 fullctl-1.3.0/src/fullctl/django/validators.py
+-rw-r--r--   0        0        0     2539 2023-04-22 03:42:18.733445 fullctl-1.3.0/src/fullctl/django/views/__init__.py
+-rw-r--r--   0        0        0      199 2022-10-14 13:57:25.300744 fullctl-1.3.0/src/fullctl/django/views/api_schema.py
+-rw-r--r--   0        0        0      927 2023-04-15 17:32:55.633525 fullctl-1.3.0/src/fullctl/django/views/template.py
+-rw-r--r--   0        0        0        0 2021-06-15 13:03:05.256145 fullctl-1.3.0/src/fullctl/service_bridge/__init__.py
+-rw-r--r--   0        0        0     2604 2023-04-15 17:32:55.633525 fullctl-1.3.0/src/fullctl/service_bridge/aaactl.py
+-rw-r--r--   0        0        0      940 2023-04-22 03:42:18.733445 fullctl-1.3.0/src/fullctl/service_bridge/auditctl.py
+-rw-r--r--   0        0        0     8510 2023-04-15 16:24:16.052446 fullctl-1.3.0/src/fullctl/service_bridge/client.py
+-rw-r--r--   0        0        0     3419 2023-02-27 05:27:02.285818 fullctl-1.3.0/src/fullctl/service_bridge/data.py
+-rw-r--r--   0        0        0     2882 2023-04-22 03:42:18.733445 fullctl-1.3.0/src/fullctl/service_bridge/devicectl.py
+-rw-r--r--   0        0        0     2577 2023-04-15 16:24:16.053446 fullctl-1.3.0/src/fullctl/service_bridge/ixctl.py
+-rw-r--r--   0        0        0     2651 2023-02-27 05:27:02.286818 fullctl-1.3.0/src/fullctl/service_bridge/nautobot.py
+-rw-r--r--   0        0        0     1699 2023-04-15 16:24:16.054446 fullctl-1.3.0/src/fullctl/service_bridge/pdbctl.py
+-rw-r--r--   0        0        0     1037 2023-04-15 16:24:16.063447 fullctl-1.3.0/src/fullctl/service_bridge/peerctl.py
+-rw-r--r--   0        0        0     1076 2023-04-15 16:24:16.097447 fullctl-1.3.0/src/fullctl/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0     6952 2023-04-15 16:24:16.097447 fullctl-1.3.0/src/fullctl/service_bridge/sot.py
+-rw-r--r--   0        0        0      323 2022-10-14 13:57:25.408743 fullctl-1.3.0/src/fullctl/utils/__init__.py
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 fullctl-1.3.0/PKG-INFO
```

### Comparing `fullctl-1.2.0/LICENSE` & `fullctl-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/README.md` & `fullctl-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/pyproject.toml` & `fullctl-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fullctl"
 repository = "https://github.com/fullctl/fullctl"
-version = "1.2.0"
+version = "1.3.0"
 description = "Core classes and functions for service applications"
 authors = ["FullCtl <code@fullctl.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
```

### Comparing `fullctl-1.2.0/src/fullctl/django/admin.py` & `fullctl-1.3.0/src/fullctl/django/admin.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/auditlog.py` & `fullctl-1.3.0/src/fullctl/django/auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/auth.py` & `fullctl-1.3.0/src/fullctl/django/auth.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/autocomplete/pdb.py` & `fullctl-1.3.0/src/fullctl/django/autocomplete/pdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/context.py` & `fullctl-1.3.0/src/fullctl/django/context.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/context_processors.py` & `fullctl-1.3.0/src/fullctl/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/decorators.py` & `fullctl-1.3.0/src/fullctl/django/decorators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/fields/__init__.py` & `fullctl-1.3.0/src/fullctl/django/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/fields/service_bridge/__init__.py` & `fullctl-1.3.0/src/fullctl/django/fields/service_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/inet/fields.py` & `fullctl-1.3.0/src/fullctl/django/inet/fields.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/inet/util.py` & `fullctl-1.3.0/src/fullctl/django/inet/util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/inet/validators.py` & `fullctl-1.3.0/src/fullctl/django/inet/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/base.py` & `fullctl-1.3.0/src/fullctl/django/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py` & `fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py` & `fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_poll_tasks.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_promote_user.py` & `fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_promote_user.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/management/commands/fullctl_work_task.py` & `fullctl-1.3.0/src/fullctl/django/management/commands/fullctl_work_task.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/middleware.py` & `fullctl-1.3.0/src/fullctl/django/middleware.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0001_initial.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0003_auditlog.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0003_auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0004_auto_20210528_1247.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0005_auto_20210528_1252.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0006_auto_20210603_0542.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0008_managementtask.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0008_managementtask.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0009_taskclaim.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0009_taskclaim.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0011_alter_managementtask_status.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0012_auto_20210805_1153.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0013_auto_20210805_1200.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0014_alter_taskclaim_task.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0015_alter_task_parent.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0015_alter_task_parent.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0018_task_schedule.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0018_task_schedule.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0021_servicebridgeaction.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0021_servicebridgeaction.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0022_auto_20220907_1253.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0023_auto_20220907_1354.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0024_auto_20221012_1227.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0025_auto_20221025_1215.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0026_auto_20230131_1405.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0027_request_response.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0027_request_response.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0030_alter_response_content.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0030_alter_response_content.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py` & `fullctl-1.3.0/src/fullctl/django/migrations/0031_auto_20230310_2152.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/alert.py` & `fullctl-1.3.0/src/fullctl/django/models/abstract/alert.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/base.py` & `fullctl-1.3.0/src/fullctl/django/models/abstract/base.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/meta.py` & `fullctl-1.3.0/src/fullctl/django/models/abstract/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,19 +419,28 @@
             raise NoMetaClassDefined()
 
     def write_meta_data(self, req):
         target_field = self.config("target_field", req.config("target_field"))
         source_name = req.config("source_name")
         target = getattr(req, target_field)
 
+        had_entries = False
+
         for date, _target, data in req.process_response(self, target, timezone.now()):
+            had_entries = True
             self._write_meta_data(
                 req, date, req.prepare_data(data), _target, target_field, source_name
             )
 
+        if not had_entries:
+            # no entries were written, write an empty entry
+            self._write_meta_data(
+                req, timezone.now(), {}, target, target_field, source_name
+            )
+
     def _write_meta_data(self, request, date, data, target, target_field, source_name):
         meta_data_cls = self.meta_data_cls
 
         meta_data_type = meta_data_cls.config("type")
         period = meta_data_cls.config("period")
         start = date - timedelta(seconds=period)
         end = date + timedelta(seconds=period)
```

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/service_bridge.py` & `fullctl-1.3.0/src/fullctl/django/models/abstract/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/abstract/template.py` & `fullctl-1.3.0/src/fullctl/django/models/abstract/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/account.py` & `fullctl-1.3.0/src/fullctl/django/models/concrete/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/auditlog.py` & `fullctl-1.3.0/src/fullctl/django/models/concrete/auditlog.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/meta.py` & `fullctl-1.3.0/src/fullctl/django/models/concrete/meta.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/service_bridge.py` & `fullctl-1.3.0/src/fullctl/django/models/concrete/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/models/concrete/tasks.py` & `fullctl-1.3.0/src/fullctl/django/models/concrete/tasks.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/api_schema.py` & `fullctl-1.3.0/src/fullctl/django/rest/api_schema.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/authentication.py` & `fullctl-1.3.0/src/fullctl/django/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/core.py` & `fullctl-1.3.0/src/fullctl/django/rest/core.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/decorators.py` & `fullctl-1.3.0/src/fullctl/django/rest/decorators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/filters.py` & `fullctl-1.3.0/src/fullctl/django/rest/filters.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/mixins.py` & `fullctl-1.3.0/src/fullctl/django/rest/mixins.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/renderers.py` & `fullctl-1.3.0/src/fullctl/django/rest/renderers.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/__init__.py` & `fullctl-1.3.0/src/fullctl/django/rest/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/aaactl_sync.py` & `fullctl-1.3.0/src/fullctl/django/rest/serializers/aaactl_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/account.py` & `fullctl-1.3.0/src/fullctl/django/rest/serializers/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/meta.py` & `fullctl-1.3.0/src/fullctl/django/rest/serializers/meta.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/org.py` & `fullctl-1.3.0/src/fullctl/django/rest/serializers/org.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/serializers/template.py` & `fullctl-1.3.0/src/fullctl/django/rest/serializers/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/urls/service_bridge_proxy.py` & `fullctl-1.3.0/src/fullctl/django/rest/urls/service_bridge_proxy.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/aaactl_sync.py` & `fullctl-1.3.0/src/fullctl/django/rest/views/aaactl_sync.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/account.py` & `fullctl-1.3.0/src/fullctl/django/rest/views/account.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/service_bridge.py` & `fullctl-1.3.0/src/fullctl/django/rest/views/service_bridge.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/template.py` & `fullctl-1.3.0/src/fullctl/django/rest/views/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/rest/views/usage.py` & `fullctl-1.3.0/src/fullctl/django/rest/views/usage.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/settings/__init__.py` & `fullctl-1.3.0/src/fullctl/django/settings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
         # TODO EMAIL_SUBJECT_PREFIX = "[{}] ".format(RELEASE_ENV)
 
         self.set_from_env("EMAIL_HOST")
         self.set_from_env("EMAIL_PORT")
         self.set_from_env("EMAIL_HOST_USER")
         self.set_from_env("EMAIL_HOST_PASSWORD")
         self.set_bool("EMAIL_USE_TLS", True)
+        self.set_option("EMAIL_BACKEND", "django.core.mail.backends.smtp.EmailBackend")
 
         # Application definition
 
         INSTALLED_APPS = [
             "django.contrib.admin",
             "django.contrib.auth",
             "django.contrib.contenttypes",
@@ -311,14 +312,15 @@
         # no default so we error sooner
         self.set_option("AAACTL_URL", "")
         self.set_option("PDBCTL_URL", "")
         self.set_option("PEERCTL_URL", "")
         self.set_option("PREFIXCTL_URL", "")
         self.set_option("IXCTL_URL", "")
         self.set_option("DEVICECTL_URL", "")
+        self.set_option("AUDITCTL_URL", "")
 
     def set_twentyc_social_oauth(self, AAACTL_URL=None):
         """
         This function sets the variables required to OAuth against aaactl using
         django-social-auth. It does not set the SOCIAL_AUTH_PIPELINE or
         AUTHENTICATION_BACKENDS.
         """
```

### Comparing `fullctl-1.2.0/src/fullctl/django/settings/default.py` & `fullctl-1.3.0/src/fullctl/django/settings/default.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/signals.py` & `fullctl-1.3.0/src/fullctl/django/signals.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/social/backends/peeringdb.py` & `fullctl-1.3.0/src/fullctl/django/social/backends/peeringdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/social/backends/twentyc.py` & `fullctl-1.3.0/src/fullctl/django/social/backends/twentyc.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.core.min.js` & `fullctl-1.3.0/src/fullctl/django/static/common/20c/twentyc.core.min.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/20c/twentyc.rest.js` & `fullctl-1.3.0/src/fullctl/django/static/common/20c/twentyc.rest.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -93,31 +93,31 @@
             },
 
             /**
              * Joins URL parts, removing extra slashes at the edges of the parts.
              *
              * @method url_join
              * @param {String} left - The leftmost URL part.
-             * @param {...String} args - The remaining URL parts.
+             * @param {...(String|Number)} args - The remaining URL parts.
              * @return {String} The joined URL string with removed extra slashes.
              */
             url_join: function(left, ...args) {
                 // Simplified urljoin that gets rid of extra / at the edges
                 // of parts
 
                 let right = [];
                 let trailing_slash = !twentyc.rest.no_end_slash;
 
                 // trim left
-
                 left = left.replace(/\/+$/g, "");
 
                 for (const parts of args) {
                     right = right.concat(
                         parts
+                        .toString()
                         .split("/")
                         .filter((part) => part)
                         .map((part) => this.trim_endpoint(part))
                     );
                 }
 
                 if (!right.length)
```

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/20c-logo-filled.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/20c-logo-filled.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/app.css` & `fullctl-1.3.0/src/fullctl/django/static/common/app.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/app.js` & `fullctl-1.3.0/src/fullctl/django/static/common/app.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/favicon.ico` & `fullctl-1.3.0/src/fullctl/django/static/common/favicon.ico`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/add.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/alerts.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/alerts.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/api.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/api.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/delete.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/edit.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/edit.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/launch.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/launch.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/light-mode.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/light-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/list.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/list.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/location.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/location.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/logout.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/mail.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/mail.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/org.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/refresh.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/refresh.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/report.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/report.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/settings.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/user.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/icon/view.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/icon/view.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/icons/ui-close.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/icons/ui-close.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/aclctl-dark.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/aclctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/ctl-mark-dark.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/ctl-mark-light.png` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/ctl-mark-light.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/devicectl-dark.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/devicectl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/ixctl-dark.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/ixctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/pdbctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/peerctl-dark.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/peerctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/logos/prefixctl-dark.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/20c.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/oauth/20c.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/google.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/oauth/google.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png` & `fullctl-1.3.0/src/fullctl/django/static/common/oauth/peeringdb-dark.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/oauth/peeringdb.png` & `fullctl-1.3.0/src/fullctl/django/static/common/oauth/peeringdb.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/service_bridge.js` & `fullctl-1.3.0/src/fullctl/django/static/common/service_bridge.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/themes/dark.css` & `fullctl-1.3.0/src/fullctl/django/static/common/themes/dark.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/app.css` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/app.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/app.js` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/app.js`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/add.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/api.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/api.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/database.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/database.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/eye.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/eye.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/gear.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/gear.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/help.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/help.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/delete.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/list/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/list/options.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/list/options.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/logout.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/org.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/theme-switcher.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/user.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/icons/view-settings.svg` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/icons/view-settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/help.png` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/imgs/help.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/imgs/loading-shim.png`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/static/common/v2/themes/dark.css` & `fullctl-1.3.0/src/fullctl/django/static/common/v2/themes/dark.css`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/__init__.py` & `fullctl-1.3.0/src/fullctl/django/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/celery.py` & `fullctl-1.3.0/src/fullctl/django/tasks/celery.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/orm.py` & `fullctl-1.3.0/src/fullctl/django/tasks/orm.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/tasks/qualifiers.py` & `fullctl-1.3.0/src/fullctl/django/tasks/qualifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,11 +95,11 @@
 
     def __str__(self):
         return f"{self.__class__.__name__} {self.limit}"
 
     def check(self, task):
         return (
             task.__class__.objects.filter(
-                status="pending", queue_id__isnull=False
+                status="pending", queue_id__isnull=False, op=task.op
             ).count()
             < self.limit
         )
```

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/redoc.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/apidocs/redoc.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/apidocs/swagger.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/apidocs/swagger.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/base.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/import-org.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-create.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/forms/org-prefs.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/manage/permissions.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/modal.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/modal.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/app/navbar.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/auth/login.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/auth/login.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth-badge.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/auth/oauth.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/base.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/errors/base.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/errors/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/snippets.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/snippets.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/apidocs/redoc.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/apidocs/swagger.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/base.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/footer.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/footer.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 {% load i18n static %}
 <div class="container-fluid">
   <div class="row align-items-center">
     <div class="col footer-left">
+      {% block footer_left %}
       <div class="row align-items-center">
         <div class="col-sm-auto theme-switcher" type="button">
           <span class="icon icon-lg icon-theme-switcher"></span>
         </div>
         <div class="col-auto">
           <a title="Contact support" data-message-type="support" {% if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else %}data-element="feature_request_btn"{% endif %}>Contact Us</a> |
           <a title="Feature request" data-message-type="feature-request" {% if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else %}data-element="feature_request_btn"{% endif %} type="button">
             Feature Request
           </a>
         </div>
       </div>
+      {% endblock %}
     </div>
     <div class="col-auto footer-center">
-      Copyright © 2014 - {{ current_year }} FullCtl, LLC
+      {% block footer_center %}
+        Copyright © 2014 - {{ current_year }} FullCtl, LLC
+      {% endblock %}
     </div>
     <div class="col footer-right">
-      <div class="row align-items-center">
-        <div class="ms-auto col-auto">{{ version }}</div>
+      {% block footer_right %}
+      <div class="row align-items-center justify-content-end">
+        <div class="col-auto">{{ version }}</div>
         <div class="help-box js-hide">
           <div class="banner-img">
             <img src="{% static "common/v2/imgs/help.png" %}" alt="">
           </div>
           <a href="{{ docs_url }}" target="_blank">Help Center</a>
           <a title="Contact support" data-message-type="support" {% if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else %}data-element="feature_request_btn"{% endif %}>Contact Support</a>
           <a href="{{ legal_url }}">Legal Notes</a>
         </div>
         <div class="col-sm-auto help-btn" type="button">
           <span class="icon icon-lg icon-help"></span>
         </div>
       </div>
+      {% endblock %}
     </div>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,13 +1,18 @@
 {% load i18n static %}
+{% block footer_left %}
 % if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else
 %}data-element="feature_request_btn"{% endif %}>Contact Us
  |
 % if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else
 %}data-element="feature_request_btn"{% endif %} type="button"> Feature Request
-Copyright Â© 2014 - {{ current_year }} FullCtl, LLC
+{% endblock %}
+{% block footer_center %} Copyright Â© 2014 - {{ current_year }} FullCtl, LLC
+{% endblock %}
+{% block footer_right %}
 {{ version }}
 2/imgs/help.png" %}" alt="">
 Help_Center
 % if post_feature_request_url == "" %}href="mailto:{{ support_email }}" {% else
 %}data-element="feature_request_btn"{% endif %}>Contact Support
  Legal_Notes
+{% endblock %}
```

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/modal.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/modal.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/app/navbar.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/login.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/auth/login.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/auth/oauth.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/base.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/errors/base.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/errors/base.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templates/common/v2/snippets.html` & `fullctl-1.3.0/src/fullctl/django/templates/common/v2/snippets.html`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/templatetags/fullctl_util.py` & `fullctl-1.3.0/src/fullctl/django/templatetags/fullctl_util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/testutil.py` & `fullctl-1.3.0/src/fullctl/django/testutil.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/urls.py` & `fullctl-1.3.0/src/fullctl/django/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 
 for import_path, namespace in getattr(settings, "FULLCTL_ADDON_URLS", []):
     urlpatterns += [path("", include((import_path, namespace), namespace=namespace))]
 
 urlpatterns += [
     path("_diag", fullctl.django.views.diag),
+    path("health/", fullctl.django.views.healthcheck),
     path("apidocs/schema.json", api_schema, name="api_schema"),
     path(
         "api/account/",
         include(
             ("fullctl.django.rest.urls.account", "fullctl_account_api"),
             namespace="fullctl_account_api",
         ),
```

### Comparing `fullctl-1.2.0/src/fullctl/django/util.py` & `fullctl-1.3.0/src/fullctl/django/util.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/validators.py` & `fullctl-1.3.0/src/fullctl/django/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/django/views/__init__.py` & `fullctl-1.3.0/src/fullctl/django/views/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import re
 import sys
 
 from django.conf import settings
+from django.db import connection
 
 # from django.conf import settings
 from django.http import Http404, HttpResponse
 from django.shortcuts import redirect, render
 from django.utils.html import escape
 from django.utils.safestring import mark_safe
 
@@ -29,14 +30,25 @@
             continue
         # if k.startswith("HTTP"):
         txt += f"{k}: {v}\n"
 
     return HttpResponse(mark_safe(f"<div><pre>Meta:\n{escape(txt)}</pre></div>"))
 
 
+def healthcheck(request):
+    """
+    Performs a simple database version query
+    """
+
+    with connection.cursor() as cursor:
+        cursor.execute("SELECT version()")
+
+    return HttpResponse("")
+
+
 @require_auth()
 def login(request):
     return redirect("/")
 
 
 def logout(request):
     response = redirect(f"{settings.AAACTL_URL}/account/auth/logout/")
```

### Comparing `fullctl-1.2.0/src/fullctl/django/views/template.py` & `fullctl-1.3.0/src/fullctl/django/views/template.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/aaactl.py` & `fullctl-1.3.0/src/fullctl/service_bridge/aaactl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/client.py` & `fullctl-1.3.0/src/fullctl/service_bridge/client.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/data.py` & `fullctl-1.3.0/src/fullctl/service_bridge/data.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/ixctl.py` & `fullctl-1.3.0/src/fullctl/service_bridge/ixctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/nautobot.py` & `fullctl-1.3.0/src/fullctl/service_bridge/nautobot.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/pdbctl.py` & `fullctl-1.3.0/src/fullctl/service_bridge/pdbctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/peerctl.py` & `fullctl-1.3.0/src/fullctl/service_bridge/peerctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/prefixctl.py` & `fullctl-1.3.0/src/fullctl/service_bridge/prefixctl.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/src/fullctl/service_bridge/sot.py` & `fullctl-1.3.0/src/fullctl/service_bridge/sot.py`

 * *Files identical despite different names*

### Comparing `fullctl-1.2.0/PKG-INFO` & `fullctl-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fullctl
-Version: 1.2.0
+Version: 1.3.0
 Summary: Core classes and functions for service applications
 Home-page: https://github.com/fullctl/fullctl
 License: Apache-2.0
 Author: FullCtl
 Author-email: code@fullctl.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

