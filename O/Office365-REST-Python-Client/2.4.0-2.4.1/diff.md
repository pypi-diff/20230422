# Comparing `tmp/Office365-REST-Python-Client-2.4.0.tar.gz` & `tmp/Office365-REST-Python-Client-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Office365-REST-Python-Client-2.4.0.tar", last modified: Fri Feb 17 17:08:18 2023, max compression
+gzip compressed data, was "Office365-REST-Python-Client-2.4.1.tar", last modified: Sat Apr 22 08:23:37 2023, max compression
```

## Comparing `Office365-REST-Python-Client-2.4.0.tar` & `Office365-REST-Python-Client-2.4.1.tar`

### file list

```diff
@@ -1,1713 +1,1785 @@
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.348641 Office365-REST-Python-Client-2.4.0/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1083 2021-07-11 21:05:58.000000 Office365-REST-Python-Client-2.4.0/LICENSE
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       60 2021-08-09 07:15:24.000000 Office365-REST-Python-Client-2.4.0/MANIFEST.in
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.028643 Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    16247 2023-02-17 17:08:17.000000 Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/PKG-INFO
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    67611 2023-02-17 17:08:17.000000 Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/SOURCES.txt
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        1 2023-02-17 17:08:17.000000 Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/dependency_links.txt
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       49 2023-02-17 17:08:17.000000 Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/requires.txt
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       10 2023-02-17 17:08:17.000000 Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/top_level.txt
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    16247 2023-02-17 17:08:18.348641 Office365-REST-Python-Client-2.4.0/PKG-INFO
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    15045 2023-02-13 18:43:02.000000 Office365-REST-Python-Client-2.4.0/README.md
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.048643 Office365-REST-Python-Client-2.4.0/office365/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2733 2022-05-31 14:42:35.000000 Office365-REST-Python-Client-2.4.0/office365/base_item.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.048643 Office365-REST-Python-Client-2.4.0/office365/communications/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:41:58.000000 Office365-REST-Python-Client-2.4.0/office365/communications/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.048643 Office365-REST-Python-Client-2.4.0/office365/communications/callrecords/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-24 07:16:24.000000 Office365-REST-Python-Client-2.4.0/office365/communications/callrecords/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      630 2021-10-01 15:01:23.000000 Office365-REST-Python-Client-2.4.0/office365/communications/callrecords/call_record.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.052643 Office365-REST-Python-Client-2.4.0/office365/communications/calls/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:45:54.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4292 2022-09-29 16:21:05.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/call.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1671 2022-09-25 17:55:11.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2021-08-24 07:08:22.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/incoming_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      207 2021-09-11 17:07:11.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/invitation_participant_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3023 2022-09-29 16:13:19.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/participant.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      174 2021-08-24 07:12:32.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/participant_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      138 2021-08-24 07:03:15.000000 Office365-REST-Python-Client-2.4.0/office365/communications/calls/route.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2508 2022-09-25 17:36:16.000000 Office365-REST-Python-Client-2.4.0/office365/communications/cloud_communications.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.052643 Office365-REST-Python-Client-2.4.0/office365/communications/meetings/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 21:32:41.000000 Office365-REST-Python-Client-2.4.0/office365/communications/meetings/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.052643 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-24 07:15:35.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2614 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      142 2021-08-24 16:18:09.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/meeting_participant.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      165 2021-09-11 18:49:22.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/meeting_participant_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      789 2021-09-11 18:51:36.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/meeting_participants.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2150 2022-12-04 19:40:44.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/online_meeting.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      208 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/provider_type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.052643 Office365-REST-Python-Client-2.4.0/office365/communications/operations/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:56:10.000000 Office365-REST-Python-Client-2.4.0/office365/communications/operations/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      207 2022-09-29 16:17:04.000000 Office365-REST-Python-Client-2.4.0/office365/communications/operations/cancel_media_processing.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      700 2021-08-06 18:57:58.000000 Office365-REST-Python-Client-2.4.0/office365/communications/operations/comms.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      638 2022-09-29 16:14:05.000000 Office365-REST-Python-Client-2.4.0/office365/communications/operations/invite_participants.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      238 2022-09-28 20:05:15.000000 Office365-REST-Python-Client-2.4.0/office365/communications/operations/start_hold_music.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      235 2022-09-28 20:10:48.000000 Office365-REST-Python-Client-2.4.0/office365/communications/operations/stop_hold_music.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.068643 Office365-REST-Python-Client-2.4.0/office365/communications/presences/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-24 06:54:16.000000 Office365-REST-Python-Client-2.4.0/office365/communications/presences/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4164 2022-09-24 12:11:22.000000 Office365-REST-Python-Client-2.4.0/office365/communications/presences/presence.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      510 2022-07-01 14:03:19.000000 Office365-REST-Python-Client-2.4.0/office365/delta_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.068643 Office365-REST-Python-Client-2.4.0/office365/directory/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/directory/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.072643 Office365-REST-Python-Client-2.4.0/office365/directory/applications/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 11:58:19.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1873 2022-12-17 19:35:18.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/api.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1125 2022-12-17 19:45:10.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/app_identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10243 2022-12-19 15:46:04.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/application.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      673 2022-12-17 19:40:47.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/public_client.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.072643 Office365-REST-Python-Client-2.4.0/office365/directory/applications/roles/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 15:56:05.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/roles/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      717 2022-10-01 08:25:32.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/roles/assignment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      289 2022-12-18 16:07:08.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/roles/role.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9348 2022-12-18 16:03:03.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/service_principal.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      322 2022-12-17 19:52:50.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/spa.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2315 2022-12-17 19:16:43.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/template.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      922 2022-12-17 19:51:21.000000 Office365-REST-Python-Client-2.4.0/office365/directory/applications/web.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.072643 Office365-REST-Python-Client-2.4.0/office365/directory/audit/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 10:06:48.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      853 2022-12-17 20:53:20.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/activity_initiator.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1384 2022-12-17 21:05:32.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/directory.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2740 2022-12-18 11:36:36.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/log_root.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.076643 Office365-REST-Python-Client-2.4.0/office365/directory/audit/provisioning/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 11:25:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/provisioning/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       37 2022-12-18 11:41:51.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/provisioning/action.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      493 2022-12-18 11:33:53.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/provisioning/object_summary.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2022-12-18 11:31:52.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/provisioning/service_principal.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.076643 Office365-REST-Python-Client-2.4.0/office365/directory/audit/signins/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 11:26:01.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/signins/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1164 2022-12-18 11:29:46.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/signins/signin.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      792 2022-12-18 11:25:28.000000 Office365-REST-Python-Client-2.4.0/office365/directory/audit/signins/status.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.076643 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-27 07:44:48.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2744 2022-11-20 20:23:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/authentication.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      773 2022-12-01 15:07:35.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/basic.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      784 2022-12-18 16:28:11.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/client_certificate.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      741 2022-09-29 17:49:23.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/configuration_base.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.080643 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-20 15:58:26.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      253 2022-11-20 20:15:01.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/fido.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2359 2022-09-27 07:55:02.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/method.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      313 2022-11-20 20:18:33.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/password.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2259 2022-11-20 16:05:43.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/phone.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      372 2022-11-20 16:07:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/authentication/password_reset_response.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.080643 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-09 13:59:09.000000 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1314 2022-11-30 22:08:56.000000 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/auth_configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      857 2022-09-19 06:43:19.000000 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/authority.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      157 2022-12-18 16:14:42.000000 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/certification.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      387 2022-12-18 16:28:11.000000 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/pkcs12_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2022-11-30 22:22:23.000000 Office365-REST-Python-Client-2.4.0/office365/directory/certificates/self_signed.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1527 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.0/office365/directory/directory.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.080643 Office365-REST-Python-Client-2.4.0/office365/directory/domains/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 16:50:42.000000 Office365-REST-Python-Client-2.4.0/office365/directory/domains/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      294 2022-12-18 16:55:02.000000 Office365-REST-Python-Client-2.4.0/office365/directory/domains/dns_record.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      484 2022-12-19 11:20:54.000000 Office365-REST-Python-Client-2.4.0/office365/directory/domains/domain.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.080643 Office365-REST-Python-Client-2.4.0/office365/directory/extensions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 13:49:51.000000 Office365-REST-Python-Client-2.4.0/office365/directory/extensions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      488 2022-12-01 20:28:07.000000 Office365-REST-Python-Client-2.4.0/office365/directory/extensions/extended_property.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      152 2021-08-06 13:47:48.000000 Office365-REST-Python-Client-2.4.0/office365/directory/extensions/extension.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1859 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.0/office365/directory/extensions/extension_property.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.084643 Office365-REST-Python-Client-2.4.0/office365/directory/groups/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 11:58:39.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1568 2022-07-02 07:53:52.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10511 2022-12-18 16:03:03.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2466 2023-02-13 18:25:25.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/lifecycle_policy.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      565 2022-04-09 13:48:19.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/profile.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/setting.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      323 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.0/office365/directory/groups/setting_template.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.084643 Office365-REST-Python-Client-2.4.0/office365/directory/identities/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:58:24.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1825 2022-12-01 15:07:35.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/api_connector.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2021-09-11 09:25:41.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/conditional_access_root.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3261 2022-09-19 06:52:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/container.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      808 2022-12-18 11:40:31.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      534 2021-08-06 09:59:26.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/identity_set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1668 2022-09-30 07:43:58.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/object_identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1024 2022-09-19 06:42:22.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1000 2022-12-18 18:52:22.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/provider_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.084643 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-11 09:26:29.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      424 2021-08-09 16:50:30.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/base.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1022 2022-12-18 18:54:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/base_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      531 2022-09-19 06:39:52.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/builtin_identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      461 2022-09-19 06:38:48.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/saml_or_wsfed.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1272 2022-09-19 06:34:14.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/social_identity.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.084643 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 19:29:05.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      661 2021-09-11 09:34:54.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/attribute.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/b2x/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-11 09:31:47.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/b2x/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2719 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/b2x/user_flow.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2114 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/language_configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      362 2022-06-30 19:55:04.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/language_page.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      652 2021-09-11 08:34:50.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/user_attribute_assignment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       79 2021-08-09 16:30:24.000000 Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/user_flow.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/insights/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-05 15:01:40.000000 Office365-REST-Python-Client-2.4.0/office365/directory/insights/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      279 2022-12-05 15:03:30.000000 Office365-REST-Python-Client-2.4.0/office365/directory/insights/office_graph.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-08-05 15:00:14.000000 Office365-REST-Python-Client-2.4.0/office365/directory/internal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/internal/paths/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-08-05 15:00:22.000000 Office365-REST-Python-Client-2.4.0/office365/directory/internal/paths/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-08-05 20:37:22.000000 Office365-REST-Python-Client-2.4.0/office365/directory/internal/paths/me.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      271 2022-05-31 14:51:22.000000 Office365-REST-Python-Client-2.4.0/office365/directory/key_credential.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 13:52:30.000000 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      706 2022-12-18 13:11:23.000000 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/assigned_license.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2021-08-09 14:42:31.000000 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/assigned_plan.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1115 2021-08-06 14:03:08.000000 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/details.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1595 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/service_plan_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      533 2021-08-06 14:03:08.000000 Office365-REST-Python-Client-2.4.0/office365/directory/licenses/subscribed_sku.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3324 2022-12-16 10:43:00.000000 Office365-REST-Python-Client-2.4.0/office365/directory/object.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4205 2022-11-20 16:18:09.000000 Office365-REST-Python-Client-2.4.0/office365/directory/object_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1009 2022-12-17 19:18:30.000000 Office365-REST-Python-Client-2.4.0/office365/directory/password_credential.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 21:27:37.000000 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.088642 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/grants/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 11:54:10.000000 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/grants/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1549 2022-12-18 12:11:52.000000 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/grants/condition_set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      436 2022-12-18 12:01:11.000000 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/grants/oauth2.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/grants/resource_specific.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1220 2022-12-17 20:50:01.000000 Office365-REST-Python-Client-2.4.0/office365/directory/permissions/scope.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.092642 Office365-REST-Python-Client-2.4.0/office365/directory/policies/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 08:25:01.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2022-12-18 13:02:47.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/authentication_methods.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      284 2022-12-17 18:55:42.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/authorization.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      357 2022-10-01 08:21:16.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/base.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2021-08-10 08:27:22.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/conditional_access.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1578 2022-12-18 12:54:15.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/permission_grant.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2991 2022-12-18 13:06:56.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/root.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      926 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.0/office365/directory/policies/sts.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      699 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/directory/profile_photo.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.092642 Office365-REST-Python-Client-2.4.0/office365/directory/rbac/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 17:57:14.000000 Office365-REST-Python-Client-2.4.0/office365/directory/rbac/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      382 2022-11-30 18:00:13.000000 Office365-REST-Python-Client-2.4.0/office365/directory/rbac/application.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.092642 Office365-REST-Python-Client-2.4.0/office365/directory/roles/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 17:53:05.000000 Office365-REST-Python-Client-2.4.0/office365/directory/roles/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      738 2022-11-30 18:02:39.000000 Office365-REST-Python-Client-2.4.0/office365/directory/roles/management.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      639 2022-12-01 20:39:52.000000 Office365-REST-Python-Client-2.4.0/office365/directory/roles/role.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      249 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.0/office365/directory/roles/template.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.092642 Office365-REST-Python-Client-2.4.0/office365/directory/security/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 21:22:03.000000 Office365-REST-Python-Client-2.4.0/office365/directory/security/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      233 2022-07-08 21:24:49.000000 Office365-REST-Python-Client-2.4.0/office365/directory/security/security.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.092642 Office365-REST-Python-Client-2.4.0/office365/directory/users/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 11:58:29.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      908 2022-07-11 13:13:42.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      852 2022-12-17 12:57:10.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      404 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/password_profile.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1370 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/profile.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      807 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    28354 2023-02-12 08:32:53.000000 Office365-REST-Python-Client-2.4.0/office365/directory/users/user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.096642 Office365-REST-Python-Client-2.4.0/office365/education/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 15:54:41.000000 Office365-REST-Python-Client-2.4.0/office365/education/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      436 2022-07-08 15:56:25.000000 Office365-REST-Python-Client-2.4.0/office365/education/class.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      176 2022-07-08 16:00:19.000000 Office365-REST-Python-Client-2.4.0/office365/education/root.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      444 2022-07-08 15:57:47.000000 Office365-REST-Python-Client-2.4.0/office365/education/user.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1934 2022-08-09 07:05:20.000000 Office365-REST-Python-Client-2.4.0/office365/entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1457 2022-12-19 12:52:47.000000 Office365-REST-Python-Client-2.4.0/office365/entity_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.096642 Office365-REST-Python-Client-2.4.0/office365/external/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 21:10:06.000000 Office365-REST-Python-Client-2.4.0/office365/external/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      163 2022-07-08 21:14:47.000000 Office365-REST-Python-Client-2.4.0/office365/external/connection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      658 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/external/external.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11861 2022-12-18 18:48:03.000000 Office365-REST-Python-Client-2.4.0/office365/graph_client.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      241 2022-12-06 09:54:20.000000 Office365-REST-Python-Client-2.4.0/office365/graph_request.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.096642 Office365-REST-Python-Client-2.4.0/office365/intune/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-19 07:01:31.000000 Office365-REST-Python-Client-2.4.0/office365/intune/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.096642 Office365-REST-Python-Client-2.4.0/office365/intune/audit/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-16 09:22:23.000000 Office365-REST-Python-Client-2.4.0/office365/intune/audit/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1117 2022-12-16 09:30:34.000000 Office365-REST-Python-Client-2.4.0/office365/intune/audit/event.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.096642 Office365-REST-Python-Client-2.4.0/office365/intune/devices/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 12:58:14.000000 Office365-REST-Python-Client-2.4.0/office365/intune/devices/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      174 2022-12-16 10:31:30.000000 Office365-REST-Python-Client-2.4.0/office365/intune/devices/app_management.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      105 2022-12-16 09:21:45.000000 Office365-REST-Python-Client-2.4.0/office365/intune/devices/configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2866 2022-12-18 16:40:07.000000 Office365-REST-Python-Client-2.4.0/office365/intune/devices/device.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1043 2022-12-16 09:38:23.000000 Office365-REST-Python-Client-2.4.0/office365/intune/devices/management.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.100642 Office365-REST-Python-Client-2.4.0/office365/intune/organizations/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 14:14:38.000000 Office365-REST-Python-Client-2.4.0/office365/intune/organizations/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2328 2022-12-17 12:28:09.000000 Office365-REST-Python-Client-2.4.0/office365/intune/organizations/contact.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2622 2022-12-01 19:13:35.000000 Office365-REST-Python-Client-2.4.0/office365/intune/organizations/organization.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      351 2022-12-01 19:15:22.000000 Office365-REST-Python-Client-2.4.0/office365/intune/provisioned_plan.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      844 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/logger.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.100642 Office365-REST-Python-Client-2.4.0/office365/onedrive/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.100642 Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 09:59:42.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      196 2022-11-30 17:14:29.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/item_action_stat.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1206 2022-11-30 17:29:27.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/item_activity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      743 2022-03-23 18:27:21.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/item_activity_stat.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      264 2021-07-24 10:41:49.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/item_analytics.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.104642 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:41:50.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      807 2022-03-06 18:26:06.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/calculated.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      871 2022-06-04 19:54:06.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/choice.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2021-08-10 19:10:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/column_link.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      387 2022-03-06 18:46:50.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/currency.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      437 2021-08-06 15:48:48.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/default_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5815 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2641 2022-10-17 18:51:08.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/definition_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-06-23 07:24:46.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/display_name_localization.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      192 2021-08-10 18:54:25.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/geolocation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      388 2022-10-12 06:58:07.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/hyperlink_or_picture.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1110 2022-10-12 06:50:02.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/lookup.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1274 2022-03-07 09:28:10.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/number.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      892 2022-07-08 08:39:21.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/person_or_group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      648 2022-03-07 18:49:02.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/term.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      722 2022-06-23 14:56:54.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/text.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      274 2022-03-07 09:48:54.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/thumbnail.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       66 2022-06-23 19:53:42.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/types.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      832 2022-06-23 07:24:46.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/validation.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.108642 Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:48:29.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3867 2022-12-04 19:19:05.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7288 2022-12-04 19:21:48.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/content_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      405 2022-07-08 08:35:55.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      530 2022-06-05 07:45:32.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/order.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.108642 Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 19:14:21.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      760 2022-09-29 12:41:02.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/content.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1483 2022-07-08 08:33:43.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/document_set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1199 2022-11-21 15:04:57.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/version.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      188 2022-09-29 12:43:01.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/version_item.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.112642 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:40:08.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      375 2021-08-11 09:02:39.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/audio.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/conflict_behavior.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    23308 2023-02-14 07:38:05.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/driveItem.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      799 2022-09-29 14:47:23.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/geo_coordinates.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      388 2021-08-11 09:05:36.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/image.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      242 2022-11-30 17:24:23.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/item_preview_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      203 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/photo.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      647 2022-11-20 21:18:10.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/publication_facet.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      638 2022-11-21 14:54:19.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/remote_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      203 2021-08-11 09:14:40.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/special_folder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2021-08-05 10:00:45.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/system_facet.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      953 2022-07-15 16:07:27.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/thumbnail.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      886 2021-08-10 09:49:49.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/thumbnail_set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      620 2022-09-29 14:38:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/uploadable_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/video.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.112642 Office365-REST-Python-Client-2.4.0/office365/onedrive/drives/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:30:49.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/drives/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4282 2022-11-30 21:21:32.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/drives/drive.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      544 2022-09-29 12:37:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/drives/recipient.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.112642 Office365-REST-Python-Client-2.4.0/office365/onedrive/files/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:44:01.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/files/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      859 2022-09-29 12:37:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/files/file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      587 2022-09-29 12:37:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/files/system_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.112642 Office365-REST-Python-Client-2.4.0/office365/onedrive/folders/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:44:12.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/folders/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      692 2022-09-29 14:38:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/folders/folder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      755 2022-10-12 06:53:21.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/folders/view.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.112642 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-02 10:37:03.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.116642 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 14:30:09.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      562 2022-08-06 12:35:57.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/children.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      504 2022-08-06 09:11:12.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/root.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      473 2022-06-05 19:29:01.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/shared.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      693 2022-08-06 11:59:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/site.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      986 2022-08-06 11:51:43.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/url.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.116642 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 14:29:30.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      995 2022-12-05 14:48:27.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/download_content.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1240 2022-11-21 15:20:10.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/get_activities_by_interval.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1083 2022-11-13 13:20:09.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/resumable_file_upload.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      917 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/upload_content.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.116642 Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:44:49.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      137 2021-08-06 09:57:23.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/field_value_set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1109 2022-03-07 09:51:29.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/item_reference.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3608 2022-11-21 15:20:10.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/list_item.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.116642 Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:39:52.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      738 2022-09-29 12:55:18.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      905 2022-09-29 13:06:17.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3193 2022-12-17 19:22:25.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/list.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.116642 Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:47:57.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4241 2022-09-29 16:26:45.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/permission.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1061 2022-03-07 09:57:00.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/sharing_invitation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      641 2022-06-26 09:35:31.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/sharing_link.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      108 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/root.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      816 2022-09-29 14:34:36.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/sharepoint_ids.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.120642 Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:44:09.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      574 2022-09-29 14:34:37.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2699 2022-11-30 17:50:44.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/drive_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      687 2022-06-05 10:24:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/shared.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.120642 Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:32:09.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8297 2022-11-30 17:17:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/site.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      698 2022-05-31 14:50:54.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/site_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1456 2022-10-11 18:35:34.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/sites_with_root.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.124642 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-03-07 18:46:33.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1332 2022-07-20 16:56:52.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      546 2022-03-08 10:04:08.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/localized_description.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      720 2022-03-14 13:10:47.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/localized_label.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      583 2022-03-14 09:41:47.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/localized_name.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2281 2022-03-23 18:27:21.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/relation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2490 2022-08-06 08:57:41.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1836 2022-07-20 17:06:50.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/set_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2336 2022-11-30 21:53:41.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/store.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1769 2022-08-06 09:01:28.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/term.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1267 2022-07-24 10:17:43.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/term_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      191 2022-03-08 09:51:50.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/term_group_scope.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.124642 Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 09:49:47.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      586 2022-07-06 09:04:57.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/base_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1052 2022-11-20 21:14:39.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/drive_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1206 2022-11-21 15:04:57.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/list_item.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.124642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.124642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/applications/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 18:37:17.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/applications/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      914 2022-11-30 20:37:05.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/applications/application.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.124642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:35:36.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      159 2022-07-08 09:19:09.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/area_format.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      117 2022-07-08 09:15:10.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/axes.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1508 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/chart.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      323 2022-07-08 09:13:58.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      161 2022-07-08 09:16:31.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/data_labels.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2022-07-08 09:18:01.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/legend.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       82 2022-07-08 09:16:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/series.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/comments/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:41:32.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/comments/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      595 2022-12-04 11:53:07.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/comments/comment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      124 2022-12-04 11:53:07.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/comments/reply.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      121 2022-12-04 11:55:39.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/filter.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/functions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:35:56.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/functions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1095 2022-12-04 11:58:03.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/functions/functions.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       85 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/functions/result.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/names/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:40:44.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/names/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1181 2022-07-08 09:28:40.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/names/named_item.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/operations/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:41:07.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/operations/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      140 2022-07-08 12:18:33.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/operations/workbook.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:34:53.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      670 2022-07-08 14:16:15.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/format.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      140 2022-07-08 14:17:07.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/format_protection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1235 2022-12-04 12:52:52.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/range.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      111 2022-11-30 20:26:20.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/reference.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      594 2022-12-04 12:06:00.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/view.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      484 2022-07-08 11:54:29.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/session_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:35:18.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1687 2022-11-19 17:33:51.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/columns/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 20:07:10.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/columns/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1348 2022-12-04 12:36:33.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/columns/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1533 2022-12-04 17:10:46.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/columns/column.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1182 2022-07-08 14:12:51.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/pivot_table.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.128642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/rows/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 20:06:44.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/rows/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1429 2022-11-19 17:53:08.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/rows/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      601 2022-11-10 18:46:16.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/rows/row.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2972 2022-12-04 12:56:34.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/table.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5027 2022-11-20 21:12:48.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/workbook.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.132642 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:36:22.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1300 2022-11-20 20:31:37.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       90 2022-07-08 09:26:08.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/protection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      167 2022-07-08 09:08:32.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/protection_options.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2834 2022-11-10 20:12:39.000000 Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/worksheet.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.132642 Office365-REST-Python-Client-2.4.0/office365/onenote/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      139 2021-08-15 18:22:15.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/entity_base_model.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1340 2021-08-16 12:41:08.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/entity_hierarchy_model.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      570 2021-08-15 18:26:08.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/entity_schema_object_model.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.132642 Office365-REST-Python-Client-2.4.0/office365/onenote/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-10-31 11:48:19.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/internal/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2871 2022-07-21 15:53:56.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/internal/multipart_page_query.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.132642 Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:16.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2343 2022-11-20 15:57:27.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2021-08-16 08:23:29.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/copy_notebook_model.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1511 2022-03-23 18:27:20.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/notebook.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      217 2021-08-16 08:11:16.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/recent.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2852 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/onenote.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.132642 Office365-REST-Python-Client-2.4.0/office365/onenote/operations/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:09:18.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/operations/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      406 2021-08-15 18:18:58.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/operations/onenote.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      423 2021-08-15 18:19:23.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/operations/onenote_operation_error.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       72 2021-08-15 18:16:32.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/operations/operation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-16 07:32:23.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/operations/operation_status.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.132642 Office365-REST-Python-Client-2.4.0/office365/onenote/pages/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:03.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/pages/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2807 2022-12-05 07:56:45.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/pages/page.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      646 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/pages/page_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      541 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/pages/page_links.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.136642 Office365-REST-Python-Client-2.4.0/office365/onenote/resources/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:59.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/resources/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1094 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/resources/resource.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.136642 Office365-REST-Python-Client-2.4.0/office365/onenote/sectiongroups/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:37.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/sectiongroups/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2383 2022-06-16 07:46:41.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/sectiongroups/section_group.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.136642 Office365-REST-Python-Client-2.4.0/office365/onenote/sections/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:14:30.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/sections/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3622 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/onenote/sections/section.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.136642 Office365-REST-Python-Client-2.4.0/office365/outlook/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-02 10:12:23.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.140642 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      923 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/attendee.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      651 2022-06-05 10:01:41.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/attendee_base.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4607 2022-12-04 17:45:40.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/calendar.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      870 2022-02-20 19:56:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/dateTimeTimeZone.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      313 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/email_address.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9163 2022-12-04 19:40:44.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/event.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      966 2022-12-03 18:39:33.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      180 2022-06-05 10:08:53.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/location_constraint.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      279 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/meeting_time_suggestion.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1267 2021-08-02 10:13:28.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/meeting_time_suggestions_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1679 2022-06-05 10:14:49.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/permission.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      594 2021-09-10 06:57:12.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/place.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      446 2022-06-05 10:11:43.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/reminder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      368 2022-06-05 10:19:34.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/role_type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.140642 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/schedule/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-29 21:16:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/schedule/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1881 2022-11-29 21:21:03.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/schedule/information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      299 2022-11-29 21:16:30.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/schedule/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      467 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/time_slot.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       99 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/working_hours.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      304 2022-06-07 12:14:26.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/category.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.140642 Office365-REST-Python-Client-2.4.0/office365/outlook/contacts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-02 10:14:30.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/contacts/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3953 2022-07-17 14:15:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/contacts/contact.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2545 2022-12-03 18:45:01.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/contacts/folder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      189 2022-09-29 21:17:34.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/convert_id_result.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.140642 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-10 06:58:23.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.140642 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/paths/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-16 10:46:01.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/paths/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.140642 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/queries/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-16 10:46:10.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/queries/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1894 2022-11-13 13:35:09.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/internal/queries/attachment_upload.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      603 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      828 2023-02-14 07:22:48.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/locale_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.144642 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.148642 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-10 06:57:10.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2093 2022-12-05 14:50:02.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/attachment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      800 2022-08-04 09:37:01.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/attachment_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/attachment_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2659 2022-08-04 13:55:12.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      962 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      540 2022-12-04 17:35:27.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      306 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/reference.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      347 2023-02-14 07:26:13.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/automatic_replies_setting.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       90 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/body_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      490 2022-12-04 19:31:48.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/conversation_thread.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3348 2022-12-04 17:39:16.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/folder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      114 2022-06-23 14:44:05.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/importance.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      525 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/item_body.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      360 2021-07-19 18:43:54.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/location.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      899 2023-02-14 07:29:06.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/mailbox_settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.148642 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-10 07:21:38.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1396 2022-12-04 19:40:44.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1070 2022-12-01 20:31:54.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/event_message.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9331 2023-02-12 08:32:53.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/message.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      486 2022-12-04 17:39:16.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/message_rule.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      538 2022-12-01 20:30:26.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/patterned_recurrence.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      608 2022-12-04 19:43:14.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/physical_address.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      139 2022-12-04 19:17:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/post.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      759 2022-12-04 17:26:31.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/recipient.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      421 2022-12-04 17:41:44.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/recurrence_pattern.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      427 2022-12-04 19:44:59.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/mail/recurrence_range.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      600 2022-11-20 13:31:00.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/timezone_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2764 2022-11-29 21:42:01.000000 Office365-REST-Python-Client-2.4.0/office365/outlook/user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.148642 Office365-REST-Python-Client-2.4.0/office365/planner/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:42:11.000000 Office365-REST-Python-Client-2.4.0/office365/planner/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.148642 Office365-REST-Python-Client-2.4.0/office365/planner/buckets/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:45:34.000000 Office365-REST-Python-Client-2.4.0/office365/planner/buckets/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       76 2021-08-17 17:00:23.000000 Office365-REST-Python-Client-2.4.0/office365/planner/buckets/bucket.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      620 2022-12-05 09:08:49.000000 Office365-REST-Python-Client-2.4.0/office365/planner/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1655 2022-03-23 18:27:20.000000 Office365-REST-Python-Client-2.4.0/office365/planner/planner.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/planner/plans/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:43:41.000000 Office365-REST-Python-Client-2.4.0/office365/planner/plans/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1343 2022-12-05 09:06:20.000000 Office365-REST-Python-Client-2.4.0/office365/planner/plans/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2444 2022-03-23 18:27:21.000000 Office365-REST-Python-Client-2.4.0/office365/planner/plans/plan.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2021-11-07 08:27:57.000000 Office365-REST-Python-Client-2.4.0/office365/planner/plans/plan_details.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/planner/tasks/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:43:34.000000 Office365-REST-Python-Client-2.4.0/office365/planner/tasks/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      281 2021-08-17 18:57:10.000000 Office365-REST-Python-Client-2.4.0/office365/planner/tasks/check_list_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      587 2021-08-17 19:00:14.000000 Office365-REST-Python-Client-2.4.0/office365/planner/tasks/check_list_items.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      553 2021-11-07 08:42:21.000000 Office365-REST-Python-Client-2.4.0/office365/planner/tasks/task.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      228 2021-08-17 17:02:59.000000 Office365-REST-Python-Client-2.4.0/office365/planner/tasks/task_details.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1098 2022-12-05 09:06:46.000000 Office365-REST-Python-Client-2.4.0/office365/planner/user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/project/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-05 07:58:43.000000 Office365-REST-Python-Client-2.4.0/office365/project/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      163 2022-07-05 08:00:40.000000 Office365-REST-Python-Client-2.4.0/office365/project/project.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/reports/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-11 13:05:47.000000 Office365-REST-Python-Client-2.4.0/office365/reports/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/reports/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-30 09:30:26.000000 Office365-REST-Python-Client-2.4.0/office365/reports/internal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/reports/internal/queries/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-30 09:30:34.000000 Office365-REST-Python-Client-2.4.0/office365/reports/internal/queries/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      868 2022-11-30 17:32:59.000000 Office365-REST-Python-Client-2.4.0/office365/reports/internal/queries/create_report_query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      347 2022-07-08 18:01:57.000000 Office365-REST-Python-Client-2.4.0/office365/reports/report.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8779 2022-11-30 17:43:43.000000 Office365-REST-Python-Client-2.4.0/office365/reports/report_root.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.152642 Office365-REST-Python-Client-2.4.0/office365/runtime/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.156642 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4478 2022-11-13 14:54:20.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/authentication_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      320 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/authentication_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      273 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/client_credential.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      115 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/credential_type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.160642 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3680 2022-07-27 15:21:37.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/acs_token_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      488 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/network_credential_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      974 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/ntlm_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      921 2022-07-27 15:21:37.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/oauth_token_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11495 2022-10-26 18:59:46.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/saml_token_provider.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.160642 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2115 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/FederatedSAML.xml
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1513 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/RST2.xml
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1526 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/SAML.xml
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1232 2022-05-31 14:50:36.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/sts_profile.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      854 2022-07-27 15:21:37.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/token_response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      224 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/user_credential.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      238 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/auth/user_realm_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7979 2022-11-16 20:18:36.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_object.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7010 2022-12-18 13:53:54.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_object_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4469 2022-11-19 10:33:32.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1322 2022-06-07 13:08:17.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_request_exception.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1941 2023-01-11 19:34:00.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7182 2022-12-25 10:01:56.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_runtime_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2036 2022-08-12 13:40:49.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2763 2023-01-08 15:44:58.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/client_value_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1687 2022-07-27 15:29:10.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/compat.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.160642 Office365-REST-Python-Client-2.4.0/office365/runtime/csom/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/csom/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.160642 Office365-REST-Python-Client-2.4.0/office365/runtime/http/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/http/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      148 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/http/http_method.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      830 2021-10-30 19:54:58.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/http/request_options.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.164642 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      881 2022-08-12 13:51:15.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/json_format.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      270 2022-12-25 10:58:06.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/method.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      356 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/model.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      165 2022-12-25 10:58:06.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/parameter.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1908 2022-06-13 19:27:17.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/path_builder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      141 2022-12-25 11:01:56.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/property.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3437 2022-07-05 08:25:47.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/query_options.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2341 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/reader.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6116 2022-12-10 12:24:14.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2771 2022-12-24 11:19:58.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-06-06 20:38:04.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/type_information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.164642 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 12:50:06.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5571 2022-11-13 13:35:10.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/batch_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1108 2022-08-14 08:49:20.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/json_light_format.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      571 2022-02-20 20:24:12.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/metadata_level.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      449 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/metadata_reader.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.164642 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 12:50:14.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2930 2022-11-13 13:37:10.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/batch_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1165 2022-08-12 13:51:15.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/json_format.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      590 2022-08-12 08:53:57.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/metadata_level.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      376 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/metadata_reader.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      458 2022-08-04 13:13:26.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/upload_session.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2346 2022-11-13 13:20:09.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/upload_session_request.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.168642 Office365-REST-Python-Client-2.4.0/office365/runtime/paths/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-11-12 20:47:45.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/paths/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      922 2022-08-09 10:02:18.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/paths/entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      183 2022-12-19 12:52:47.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/paths/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      978 2022-08-09 09:19:07.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/paths/resource_path.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      783 2022-07-21 15:53:56.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/paths/service_operation.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.168642 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1813 2022-11-13 13:35:09.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/batch.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1718 2022-11-15 20:27:51.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/client_query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      827 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/create_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      367 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/delete_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1236 2022-11-29 21:33:12.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/function.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      818 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/read_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1722 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/service_operation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      589 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/update_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      756 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/queries/upload_session.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.168642 Office365-REST-Python-Client-2.4.0/office365/runtime/types/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/types/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      561 2022-06-04 19:54:06.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/types/collections.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      558 2022-08-03 08:58:31.000000 Office365-REST-Python-Client-2.4.0/office365/runtime/types/event_handler.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.172642 Office365-REST-Python-Client-2.4.0/office365/search/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-01 08:39:25.000000 Office365-REST-Python-Client-2.4.0/office365/search/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      652 2022-07-08 11:38:29.000000 Office365-REST-Python-Client-2.4.0/office365/search/aggregation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2022-07-08 11:33:40.000000 Office365-REST-Python-Client-2.4.0/office365/search/alteration_options.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-07-08 11:36:45.000000 Office365-REST-Python-Client-2.4.0/office365/search/bucket.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2066 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/search/entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      283 2022-07-08 11:03:52.000000 Office365-REST-Python-Client-2.4.0/office365/search/entity_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      800 2022-07-08 11:28:30.000000 Office365-REST-Python-Client-2.4.0/office365/search/hit.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1235 2022-07-08 11:32:52.000000 Office365-REST-Python-Client-2.4.0/office365/search/hits_container.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      404 2022-07-08 10:33:47.000000 Office365-REST-Python-Client-2.4.0/office365/search/query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2268 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/search/request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      773 2022-07-08 10:47:57.000000 Office365-REST-Python-Client-2.4.0/office365/search/response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      144 2022-07-08 10:39:04.000000 Office365-REST-Python-Client-2.4.0/office365/search/sort_property.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.176642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.176642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-11 06:54:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      464 2022-11-08 19:15:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/action_facet.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      215 2022-11-08 14:53:55.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/capabilities.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      108 2022-11-08 14:46:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/client_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      373 2022-11-08 19:15:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/entity.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.176642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/facets/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-08 19:00:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/facets/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      214 2022-11-08 19:03:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/facets/rename.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      522 2022-11-08 19:08:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/facets/sharing.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2022-11-08 19:04:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      201 2022-11-08 15:05:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/logger.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      967 2022-11-08 15:15:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/tracked_item_service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      223 2022-11-08 15:15:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/tracked_item_updates_request.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/addtoonedrive/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-19 21:22:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/addtoonedrive/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-12-19 21:24:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/addtoonedrive/mount_service.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/addtoonedrive/requests/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-19 21:22:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/addtoonedrive/requests/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      111 2022-12-19 21:25:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/addtoonedrive/requests/get_remote_item_Info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/analytics/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-15 09:26:38.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/analytics/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1288 2022-09-25 11:22:28.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/analytics/usage_service.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/orgassets/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 10:17:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/orgassets/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/orgassets/library.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      113 2022-07-08 10:25:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/orgassets/library_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      390 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/orgassets/org_assets.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1259 2022-07-11 09:44:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/web_application.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1193 2022-07-11 09:46:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/web_service.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1234 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/alert.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1736 2022-09-26 07:17:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      609 2022-02-03 12:29:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/creation_information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.180642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/analytics/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:40:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/analytics/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2449 2022-09-25 10:11:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/analytics/usage_entry.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-26 06:23:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1836 2022-09-26 06:15:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/credential.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      177 2022-07-06 08:33:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/identity_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      168 2022-09-26 06:26:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      145 2022-09-26 06:23:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/name.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/apps/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-14 07:18:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/apps/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      191 2022-12-06 10:57:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/apps/app_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4084 2022-10-01 12:50:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/attachment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3100 2022-06-18 19:56:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      924 2022-06-11 10:38:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/creation_information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/audit/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-03 10:02:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/audit/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      674 2022-07-03 20:08:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/audit/audit.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authentication/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-13 13:24:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authentication/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      514 2022-09-14 07:26:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authentication/acs_service_principal_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authpolicy/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-15 09:23:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authpolicy/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authpolicy/events/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-15 09:23:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authpolicy/events/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      206 2022-09-15 09:25:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/authpolicy/events/auth_event.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1275 2022-07-28 11:42:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/base_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      289 2022-10-10 20:40:38.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/base_entity_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/businessdata/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:39:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/businessdata/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      100 2022-09-14 07:21:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/businessdata/app_bdc_catalog.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.184642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/campaigns/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-26 07:19:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/campaigns/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      699 2022-09-26 13:49:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/campaigns/campaigns.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-09-26 07:21:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/campaigns/communication_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      101 2022-09-26 13:48:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/campaigns/entity.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.188642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      301 2022-06-06 09:54:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/alert.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      999 2022-06-06 09:47:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/change.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1871 2022-09-26 07:02:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2022-06-06 09:49:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/content_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/field.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      453 2022-06-06 14:16:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      351 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/folder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      404 2022-06-07 14:38:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      817 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/list.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1401 2022-06-06 10:07:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/log_item_query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3672 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      460 2022-12-23 16:57:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/token.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      697 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      172 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/user.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/web.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    21212 2023-02-15 10:22:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/client_context.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/hostedapps/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-01 11:39:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/hostedapps/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      224 2022-10-28 09:08:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/hostedapps/add_response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-10-28 09:13:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/hostedapps/app.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      627 2022-12-20 16:31:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/hostedapps/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      408 2022-09-15 08:26:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/identifier.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      613 2022-12-20 21:43:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/query_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2022-06-09 18:58:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/storage_entity.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/client/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-01 11:45:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/client/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      196 2022-10-01 11:49:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/client/identity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      719 2022-10-01 11:38:20.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1653 2022-10-01 11:38:20.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/comment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      583 2022-10-01 11:49:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-24 08:08:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-10-11 18:23:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/dlp_classification_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2022-10-11 18:23:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/pending_review_items_statistics.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1646 2022-12-06 22:22:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/store_proxy.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      542 2022-12-17 10:46:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/tag.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      208 2022-06-24 08:10:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/tag_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:00:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.192642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:02:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      229 2022-12-17 10:59:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/enabled.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4034 2022-12-17 11:08:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/hub.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.196642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/models/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 10:59:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/models/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      755 2022-12-17 11:00:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/models/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      245 2022-09-22 06:23:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/models/entity_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      225 2022-10-29 11:31:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/models/model.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.196642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/publications/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 11:16:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/publications/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      237 2022-12-06 09:08:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/publications/publication.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.196642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 11:00:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      763 2022-12-17 11:08:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      540 2022-10-29 11:30:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/entity_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      196 2022-12-10 14:42:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/meta.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      229 2022-12-17 11:08:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/sample.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.196642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/workitems/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 11:15:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/workitems/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      419 2022-12-17 11:16:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/workitems/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2022-10-05 19:11:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/workitems/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-12-17 10:35:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/syntex_models_landing_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.196642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4660 2022-12-19 12:59:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6973 2022-12-19 19:27:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/content_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      907 2022-06-18 10:00:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/content_type_id.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      843 2023-01-04 21:16:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      432 2022-12-19 12:31:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/entity_data.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.200642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/fieldlinks/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 20:22:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/fieldlinks/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2755 2022-12-19 14:32:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/fieldlinks/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1184 2022-12-19 13:16:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/fieldlinks/field_link.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.200642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/customactions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/customactions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1463 2022-10-08 08:38:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/customactions/action.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      434 2022-09-09 17:31:20.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/customactions/element.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      490 2022-09-09 17:30:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/customactions/element_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.200642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1284 2023-02-15 10:18:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      419 2022-05-31 14:57:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/group_and_user_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5247 2023-02-15 10:18:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/helper.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      164 2023-02-15 10:15:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/link.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2021-12-06 18:17:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/members_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      188 2023-01-12 22:20:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/membership_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      184 2023-01-12 22:27:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/my_groups_result.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.204642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/provider/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:41:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/provider/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2023-01-04 21:04:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/provider/provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      942 2022-10-08 11:09:28.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/session.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1048 2023-02-15 10:18:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.204642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/documentmanagement/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/documentmanagement/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2175 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/documentmanagement/document_id.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2234 2022-08-18 16:13:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/documentmanagement/document_set.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.204642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      236 2022-07-08 10:10:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      907 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1070 2022-07-06 08:24:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/definition_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.204642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/excel/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/excel/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      613 2021-11-18 20:10:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/excel/excel_rest.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.204642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2319 2022-12-10 12:49:48.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.204642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/definitions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-20 14:55:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/definitions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1081 2022-11-20 15:04:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/definitions/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      343 2022-10-13 06:43:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/definitions/definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      265 2022-06-18 20:25:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/definitions/scope.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      538 2022-06-18 20:21:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/feature.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-12-07 20:38:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/known_list.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.212642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1073 2022-06-12 18:10:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/add_field_options.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      946 2022-12-11 20:56:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/calculated.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      125 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/choice.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7185 2022-07-15 15:43:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      435 2022-02-15 20:37:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/computed.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1666 2022-06-12 18:15:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      745 2022-06-12 18:15:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/currency.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      674 2022-06-14 09:20:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/date_time.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-06-14 09:17:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/date_time_format.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2022-06-18 09:23:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/datetime_field_format_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10458 2022-10-08 08:53:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/field.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      310 2022-02-04 11:01:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/geolocation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      822 2022-02-04 11:41:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/geolocation_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      162 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/guid.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      533 2022-09-15 13:30:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/image_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1570 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/lookup.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      734 2022-08-08 09:53:28.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/lookup_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1001 2022-06-24 20:05:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_choice.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      342 2022-08-08 14:01:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_choice_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1127 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_line_text.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      295 2022-06-12 18:13:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_lookup_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      387 2022-06-14 09:10:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_user_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1424 2022-06-14 08:51:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/number.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      920 2022-06-14 09:10:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/rating_scale.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2081 2022-06-14 13:56:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/related_field.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      682 2022-06-14 13:56:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/related_field_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      294 2022-12-19 09:41:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/string_values.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      581 2022-02-15 20:51:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/text.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       92 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/thumbnail.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2782 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      363 2022-06-24 20:00:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/url.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2022-06-12 18:16:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/urlFieldFormatType.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      740 2022-06-12 18:22:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/url_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1566 2022-06-26 09:33:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/user.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      727 2022-06-12 18:13:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/user_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      644 2022-07-14 09:14:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/xmlSchemaFieldCreationInformation.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.216642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1844 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/checked_out_file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      852 2022-07-10 13:17:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/checked_out_file_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3469 2022-10-28 12:33:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1088 2022-10-19 10:43:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    28717 2023-02-15 10:15:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2022-06-11 10:36:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/move_operations.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      927 2022-10-01 12:45:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/recent_file_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      533 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/system_object_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3504 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/version.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2592 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/version_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1100 2022-12-16 13:25:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/version_event.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.216642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/flows/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-25 18:45:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/flows/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2021-08-25 18:46:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/flows/synchronization_result.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3060 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      454 2022-06-03 14:09:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/delete_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-10-02 09:29:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/download_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    16094 2022-11-19 10:26:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/folder.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/forms/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/forms/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1429 2022-02-04 10:57:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/forms/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      825 2022-06-24 10:38:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/forms/form.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      941 2022-12-25 10:58:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/key_value.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/paths/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-02-17 21:42:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/paths/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      246 2022-08-09 09:25:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/paths/entity.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-11-23 14:55:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      734 2022-10-28 07:17:48.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/create_file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      924 2022-06-21 07:12:48.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/download_file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      632 2022-06-21 07:18:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/upload_file.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2979 2022-10-28 12:44:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/upload_session.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/likes/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/likes/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1534 2022-06-28 17:24:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/likes/liked_by_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      502 2022-09-15 08:23:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/likes/user_entity.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.220642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listhome/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-05 20:03:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listhome/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      172 2022-12-05 20:02:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listhome/favorite_lists.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      197 2022-12-05 20:07:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listhome/item.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.224642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.224642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/caml/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/caml/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4194 2022-11-22 20:35:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/caml/query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1274 2022-10-12 11:29:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-12-19 09:23:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/collection_position.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      596 2022-06-19 07:46:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/compliance_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1007 2022-06-19 07:46:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      987 2022-06-19 11:57:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/creation_information_using_path.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      267 2022-12-19 09:22:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/delete_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1416 2022-06-12 18:13:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/form_update_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       94 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/hashtag.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      208 2022-11-10 19:21:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/listdata_validation_exception_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    23057 2022-12-19 09:43:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/listitem.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      111 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/update_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/user_info_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2585 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/version.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      631 2022-02-04 10:31:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/base_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      663 2022-10-13 16:37:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/bloom_filter.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3086 2022-09-25 11:58:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      327 2022-12-10 14:45:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/collection_position.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      813 2022-06-19 09:48:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/creatable_item_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2253 2022-06-19 09:46:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/creatables_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      802 2022-06-19 09:56:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      944 2022-11-25 18:14:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/currency.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      845 2022-11-25 18:12:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/currency_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      449 2022-11-25 18:06:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/currency_information_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      190 2022-06-19 19:43:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/data_source.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      316 2022-02-04 10:39:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/document_library_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      239 2022-06-19 09:53:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/document_template_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      492 2022-12-10 14:11:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/get_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    35513 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/list.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      601 2022-10-13 06:33:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/render_data_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2022-10-13 06:34:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/render_override_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       97 2021-09-11 20:16:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/rule.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1810 2022-10-01 18:41:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/template.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      763 2022-07-14 08:03:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/template_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1623 2022-06-19 10:03:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/template_type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/logger/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/logger/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/logger/logFileInfo.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      337 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/logger/logFileInfoCollection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1222 2022-09-22 06:44:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/logger/log_export.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-06 10:33:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      815 2022-09-14 14:12:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/app_metadata.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      797 2022-09-14 14:18:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/app_metadata_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:48:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:53:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1162 2022-09-14 14:17:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/accessor.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      188 2022-07-04 09:53:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/allowed_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      513 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/allowed_items.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/tenant/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:48:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/tenant/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.232642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/tenant/appcatalog/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:53:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/tenant/appcatalog/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1745 2022-07-04 09:56:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/tenant/appcatalog/accessor.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.236642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      318 2022-07-10 10:48:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/attachment_store.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      182 2022-07-06 07:17:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2022-06-03 14:04:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      294 2022-07-10 10:50:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-06-03 14:04:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microfeed/post_definition.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.236642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microservice/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microservice/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1058 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/microservice/manager.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.236642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-07 12:03:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.236642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/common/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-31 16:20:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/common/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      275 2022-10-31 16:24:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/common/task.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-10-31 16:26:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/common/task_definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-10-31 16:23:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/common/task_entity_data.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.236642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/service/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-31 16:19:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/migrationcenter/service/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.236642 Office365-REST-Python-Client-2.4.0/office365/sharepoint/multigeo/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-07 12:04:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/multigeo/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      212 2022-12-16 10:50:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/multigeo/unified_group.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.240641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2023-02-15 20:51:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/configured_metadata_items.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      572 2022-11-27 12:05:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/home_site_navigation_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      611 2022-07-14 09:20:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/menu_node.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1784 2022-06-07 12:10:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/menu_state.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1176 2023-02-15 20:50:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/metadata_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1995 2022-05-31 14:55:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/navigation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5888 2022-12-05 15:01:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/navigation_service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3077 2022-10-08 11:18:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/node.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2606 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/node_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1386 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/node_creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1482 2022-06-07 10:59:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/provider_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      171 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/publishing_navigation_provider_type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.240641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/oauth/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-24 10:18:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/oauth/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      186 2022-09-24 12:20:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/oauth/authentication.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      746 2022-06-24 10:24:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/oauth/native_client.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.240641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/orgnewssite/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-06 09:28:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/orgnewssite/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      956 2022-12-06 10:00:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/orgnewssite/api.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      206 2022-12-06 10:00:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/orgnewssite/info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.240641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/packaging/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 21:01:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/packaging/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      194 2022-11-30 21:06:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/packaging/app_details.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.240641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pageinstrumentation/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-24 10:25:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pageinstrumentation/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      191 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pageinstrumentation/click_manager.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.240641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      301 2022-06-13 17:52:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/customized_page_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1147 2022-02-15 20:35:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/page_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      479 2022-02-04 10:28:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/template_file_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      650 2021-10-26 21:43:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/wiki_page_creation_information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.244641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1936 2022-07-10 13:08:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/base_permissions.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.244641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/irm/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:54:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/irm/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2022-07-10 13:08:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/irm/effective_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      463 2022-10-01 18:37:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/irm/file_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      887 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/irm/settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1028 2022-12-19 21:19:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/kind.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.244641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:57:55.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.244641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/assignments/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:52:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/assignments/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2021 2022-12-19 20:18:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/assignments/assignment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2712 2022-07-10 13:11:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/assignments/collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.244641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:50:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3400 2022-12-19 20:43:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      926 2022-12-19 20:43:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2526 2022-12-19 20:50:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7710 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/securable_object.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      212 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/utility.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.244641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/policy/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-12-25 11:10:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/policy/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1683 2022-12-19 10:20:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/policy/dlp_policy_tip.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2022-07-10 13:26:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/policy/evaluation_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.248641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.248641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/channels/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-22 21:59:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/channels/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2022-12-22 22:01:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/channels/info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      455 2022-12-23 16:49:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/channels/info_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-11-26 13:30:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/collaboration_mailbox.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-10-01 12:32:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/community_moderation.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.248641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:12:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-09-08 18:15:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/creation_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      623 2022-09-08 18:16:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      595 2022-09-08 18:16:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/creation_params.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1499 2022-07-11 11:19:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      465 2022-07-11 10:15:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/site_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6936 2022-12-24 10:08:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/site_manager.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.248641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/home/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-11 15:39:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/home/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-11-28 19:02:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/home/page_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      342 2022-09-20 06:28:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/home/service_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      642 2022-11-28 18:57:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/home/service_context_builder.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1063 2022-10-31 14:18:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/hub_sites_utility.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.248641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-29 16:23:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      207 2022-10-29 16:25:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/contract.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      521 2022-10-29 16:27:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/list_contract.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      839 2022-10-29 16:43:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2687 2022-09-20 06:42:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/mysite_recommendations.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      710 2022-12-06 10:47:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/organization_news.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/orglabels/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-29 15:58:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/orglabels/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      203 2022-10-29 16:03:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/orglabels/context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      529 2022-10-29 16:03:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/orglabels/context_list.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      830 2022-11-27 18:46:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/rating_settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:23:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      976 2022-11-27 13:22:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/creation_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      381 2022-11-26 13:27:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/creation_response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1543 2022-06-18 19:56:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/icon_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4645 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      388 2022-02-21 14:37:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      195 2022-10-01 12:33:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/suite_nav_data.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/teams/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-29 16:19:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/teams/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-12-22 22:03:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/teams/recent_and_joined_response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1202 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/theme_manager.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/userprofiles/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-30 14:07:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/userprofiles/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      232 2022-11-01 18:39:38.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/userprofiles/documents_shared_with_group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-10-30 14:11:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/userprofiles/documents_shared_with_me.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/webcontrols/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-20 06:28:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/webcontrols/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.252641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-20 15:20:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3435 2022-12-20 15:35:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      369 2022-12-20 15:39:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3128 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2162 2022-11-29 21:51:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/principal.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      515 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/source.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      216 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.256641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-20 15:20:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2454 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      539 2022-10-06 07:39:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/id_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3468 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.256641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      244 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/client_side_page.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.256641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-10-25 14:25:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1086 2022-10-29 12:08:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/controller.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2022-02-19 16:37:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/page_details.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      499 2022-12-03 11:20:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/page_diagnostics.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      229 2022-12-03 11:20:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/page_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      697 2022-09-13 07:03:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/embed_data_v1.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      900 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/embed_service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      525 2022-12-03 11:28:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/file_picker_options.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.256641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/navigation/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/navigation/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.260641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 08:00:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      201 2022-12-03 12:15:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/campaign_publication.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3270 2022-12-03 10:52:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1203 2021-10-28 06:42:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/fields_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4507 2022-10-06 19:11:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/metadata.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      631 2022-12-03 10:47:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/metadata_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8929 2022-12-03 18:06:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/page.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      284 2022-12-03 18:06:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/page_3d.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      517 2022-07-29 10:06:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/repost.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8005 2022-12-03 10:43:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      287 2022-07-29 08:11:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/topic.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      341 2022-07-29 08:11:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/topic_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      139 2022-07-29 08:11:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/topic_fields_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      262 2022-07-29 08:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/version_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.260641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/personmagazine/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-13 07:05:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/personmagazine/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      101 2022-09-13 07:06:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/personmagazine/person_magazine.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      215 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/portal_health_status.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.260641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/portallaunch/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-22 11:25:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/portallaunch/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-11-22 11:27:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/portallaunch/wave.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      194 2022-11-22 11:28:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/portallaunch/waves_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      597 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/primary_city_time.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1910 2022-09-20 07:00:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/rich_sharing.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2022-10-29 15:18:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/search.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.260641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 07:39:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.260641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 07:41:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1058 2022-11-26 12:39:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/creation_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      239 2022-07-29 07:41:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/creation_response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3468 2022-11-27 13:29:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/site.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      277 2022-07-29 09:40:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/user_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.264641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 08:05:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      550 2022-10-29 15:16:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/channel.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      347 2022-07-29 08:06:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/channel_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1204 2022-10-29 15:10:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      332 2022-07-29 08:06:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/item_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      471 2022-10-29 15:29:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/service_discoverer.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      803 2022-07-29 08:06:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/service_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      173 2022-10-29 15:06:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/view_data.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.264641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pushnotifications/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-02 14:39:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pushnotifications/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      825 2022-12-07 20:09:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pushnotifications/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1215 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/pushnotifications/subscriber.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.264641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/quotamanagement/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-01-08 09:38:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/quotamanagement/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.264641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2536 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2977 2022-10-01 19:43:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/item_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1236 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/query_information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.264641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/reputationmodel/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/reputationmodel/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2943 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/reputationmodel/reputation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-11-28 20:57:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      832 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/request_context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      836 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/request_user_context.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.268641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.272641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1977 2022-11-24 18:00:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/document_crawl_log.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      259 2022-11-30 21:01:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/site_content_processing_info_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      646 2022-11-24 18:09:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/site_me_ta_info_provider.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1173 2023-01-03 14:37:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/tenant_crawl_versions_info_provider.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.272641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/analytics/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-05-29 08:42:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/analytics/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      324 2022-10-07 17:50:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/analytics/action.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-10-07 17:53:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/analytics/signal.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      278 2022-10-07 17:55:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/analytics/signal_store.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      718 2022-12-21 15:20:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/context_condition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1188 2022-11-23 19:58:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/custom_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      493 2022-12-21 20:09:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/endpoints.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      803 2022-12-21 15:32:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/object_owner_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1136 2022-12-21 15:24:54.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/promoted_result_query_rule.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1101 2022-12-21 15:27:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/promoted_results_operations_result.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.276641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1058 2022-12-01 21:19:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/auto_completion.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      406 2022-12-22 21:58:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/auto_completion_match.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1251 2022-07-14 19:16:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/auto_completion_results.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      277 2022-11-27 17:32:48.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/condition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1506 2022-12-21 20:06:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      664 2022-12-21 20:17:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/context.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      305 2022-12-21 19:57:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/expanded_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      964 2022-07-14 17:27:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/personal_result_suggestion.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      627 2022-11-24 17:51:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/personalization_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-12-21 20:37:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/popular_tenant_query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      784 2022-11-23 18:59:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/property.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      354 2022-11-23 18:53:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/property_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      343 2022-11-27 18:05:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/reordering_rule.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      602 2022-12-21 20:13:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/routing_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.276641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/sort/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-07 17:29:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/sort/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2267 2022-10-07 17:48:20.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/sort/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      882 2023-01-08 16:39:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/sort/sort.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1337 2023-01-08 15:38:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/suggestion_results.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-10-06 19:48:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/tenant_custom_query_suggestions.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2058 2022-12-24 10:18:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1913 2022-12-21 19:47:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/ranking_labeling.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1720 2022-12-24 10:18:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/refinement_results.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.276641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/refiner/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-06 19:39:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/refiner/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      464 2022-12-24 10:22:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/refiner/entry.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2022-11-24 18:11:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/refiner/refiner.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2907 2022-12-24 11:30:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/relevant_results.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      304 2022-12-21 19:50:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/reordering_rule_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.276641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/reports/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-05-29 09:26:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/reports/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      338 2022-05-29 09:40:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/reports/abandoned_queries.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2022-11-23 19:22:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/reports/base.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2022-11-23 19:36:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/reports/top_queries.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6857 2022-11-27 18:05:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3019 2022-12-24 10:43:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    13118 2023-01-08 16:48:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4633 2023-01-08 09:51:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/setting.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      471 2022-12-24 11:24:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/simple_data_row.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      548 2022-12-24 11:40:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/simple_data_table.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-12-24 11:37:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/special_term_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      572 2022-12-24 11:40:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/special_term_results.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2263 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/server_settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.284641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      371 2022-12-07 13:49:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/abilities.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      661 2022-12-11 12:01:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/ability_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      428 2022-11-24 19:38:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/access_request_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6916 2022-11-08 21:07:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/document_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      332 2022-06-13 08:08:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/external_site_option.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2433 2022-12-07 13:51:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-11-24 19:38:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/information_request.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.284641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/invitation/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-18 16:00:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/invitation/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      451 2022-11-24 19:15:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/invitation/creation_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1021 2022-11-24 18:49:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/invitation/link.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1001 2022-12-11 16:15:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/link_abilities.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.284641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-18 16:04:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1356 2022-10-18 16:12:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/access_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2022-01-24 09:43:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-11-24 19:20:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/default_template.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      409 2022-11-24 19:24:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/default_templates_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2351 2022-11-24 20:54:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      854 2022-06-01 12:09:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/kind.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2640 2022-06-26 09:35:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/share_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      488 2022-10-18 16:42:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/share_response.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      651 2022-06-01 12:31:13.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/share_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9254 2022-10-18 16:05:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/object_sharing_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1320 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/object_sharing_information_user.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3577 2022-10-18 16:04:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/object_sharing_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1693 2022-06-26 09:35:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/operation_status_code.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1530 2022-12-11 20:53:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/permission_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1053 2022-12-11 21:03:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/personal_web.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1067 2022-11-08 19:42:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/picker_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      247 2022-11-24 18:46:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/principal.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3826 2022-12-20 15:21:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3534 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/role_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      997 2022-12-07 14:02:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/securable_object_extensions.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      190 2022-11-09 20:09:48.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/shared_document_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      117 2022-02-03 10:15:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/shared_object_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      198 2022-06-26 09:35:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/shared_with_user.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1051 2022-10-01 18:58:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/sharepoint_sharing_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1424 2022-11-09 20:21:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/site_sharing_report_helper.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-11-09 20:21:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/site_sharing_report_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      881 2022-09-26 06:32:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/user_directory_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      627 2022-11-08 20:48:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/user_role_assignment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1027 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/user_sharing_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2130 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/utility.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2022-12-11 21:07:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/web_sharing_manager.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.288641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1396 2022-06-04 08:51:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/creation_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/design_package_menu_contents.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      406 2022-06-04 08:28:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/metadata.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      234 2023-01-05 10:37:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/principal.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      324 2023-01-05 10:37:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/run.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      224 2023-01-05 10:26:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/task.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.288641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitehealth/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:56:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitehealth/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      262 2022-09-14 14:05:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitehealth/result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      689 2022-07-04 20:04:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitehealth/summary.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.288641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      125 2022-11-22 15:43:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/azure_container_Info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2022-11-26 15:01:20.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/home_site_reference.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/home_sites_details.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       95 2021-08-25 20:26:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/language.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      800 2022-07-06 09:00:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/language_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    24902 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/site.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      118 2022-02-22 07:45:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/site_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4590 2022-12-06 09:18:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/sph_site.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       99 2022-07-03 20:06:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/team_site_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      155 2022-10-08 08:23:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/upgrade_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      966 2021-09-03 10:18:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/usage_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.292641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-03 12:53:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      450 2023-01-05 10:38:55.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/action_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2023-01-05 17:34:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/action_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      109 2023-01-05 10:39:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/creation_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      339 2022-06-03 16:14:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/metadata.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1123 2023-01-05 17:34:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/serialization_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      383 2023-01-05 17:34:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/serialization_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      274 2023-01-05 10:40:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/update_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11973 2023-02-17 07:31:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/utility.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.292641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      236 2022-07-04 13:45:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/actor.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      554 2022-07-04 13:44:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/actor_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1336 2022-12-07 07:53:28.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/announcement_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      290 2022-07-10 09:47:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/attachment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      222 2022-07-04 13:46:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/attachment_action.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      450 2022-07-09 09:17:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/data_overlay.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.296641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 10:09:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2606 2022-09-08 12:00:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/feed.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3691 2022-12-07 13:41:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      783 2022-09-08 12:05:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/rest.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      976 2022-07-04 14:16:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/rest_manager.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.296641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/following/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 10:11:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/following/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1540 2022-07-10 10:25:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/following/manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1597 2022-07-09 12:35:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/following/rest_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      329 2022-07-10 09:56:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/link.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.296641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/microfeed/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 12:10:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/microfeed/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2022-09-08 12:11:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/microfeed/thread.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2022-09-08 12:12:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/microfeed/thread_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      105 2022-09-08 12:13:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/microfeed/user_posts.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.296641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 10:03:02.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      403 2022-07-10 10:00:39.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/actor_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1720 2022-07-09 12:42:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/creation_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      272 2022-07-10 10:07:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/definition_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      316 2022-07-10 10:08:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/definition_data_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1468 2022-07-10 10:03:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/post.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1532 2022-12-07 13:38:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/reference.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      774 2022-07-04 14:05:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/rest_actor.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2119 2022-07-09 12:02:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/rest_thread.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1325 2022-07-10 08:54:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/switch.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1723 2022-12-07 13:38:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/thread.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.300641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/storagemetrics/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/storagemetrics/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1433 2022-06-24 19:57:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/storagemetrics/storage_metrics.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.300641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.300641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/contenttypesync/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:38:35.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/contenttypesync/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6480 2022-07-15 12:52:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/create_xml_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3202 2022-07-15 13:23:58.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/field.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1415 2022-06-16 20:09:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/field_value.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      833 2022-07-14 12:38:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1743 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      911 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/item_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      318 2022-07-15 12:34:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/metadata.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1103 2022-11-13 13:20:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      645 2022-07-14 12:38:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/set.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1871 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/store.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      171 2022-07-14 12:24:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/term.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.304641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/teams/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-12-27 14:02:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/teams/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2022-02-16 18:22:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/teams/channel.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3071 2022-11-25 20:24:28.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/teams/channel_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      371 2022-12-22 22:15:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/teams/site_owner_response.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.304641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.308641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.308641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/audit/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-13 06:44:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/audit/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-10-13 06:45:55.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/audit/data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-10-13 06:49:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/audit/unified_record.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.308641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/collaboration/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-12 10:33:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/collaboration/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      829 2022-11-22 11:13:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/collaboration/insights_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      172 2022-09-19 20:18:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/deny_add_and_customize_pages_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      409 2022-07-05 08:03:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/endpoints.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.312641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-13 07:24:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1588 2022-10-01 18:33:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1350 2022-06-18 08:50:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/hub_site.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-10-09 18:58:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/permission.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      707 2022-10-09 19:05:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/properties.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.312641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/insights/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-25 18:49:49.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/insights/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      116 2022-11-25 18:57:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/insights/onedrive_site_sharing.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      238 2022-10-07 18:13:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/insights/top_files_sharing.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.312641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-22 06:42:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/internal/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      544 2022-10-09 18:47:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/internal/web_appservice_principal.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      514 2022-11-26 09:55:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/response_message_center.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      234 2022-11-10 18:22:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/response_service_health.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      762 2022-06-04 19:54:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/secondary_administrators_fields_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      474 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/secondary_administrators_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1781 2022-12-10 18:52:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/settings_service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      618 2022-02-19 17:21:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/sharing_capabilities.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      495 2022-10-08 14:13:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_administrators_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1195 2022-11-26 10:14:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_collection_management_service.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      384 2022-11-26 10:19:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_creation_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      254 2022-10-07 18:09:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_creation_default_storage_quota.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      933 2022-07-05 15:18:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_creation_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      537 2022-11-26 10:19:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_creation_source.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4381 2022-10-09 13:47:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1986 2022-12-10 18:51:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_properties_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      951 2022-12-10 18:36:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_properties_enumerable_filter.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      230 2022-12-10 18:44:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_state_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-12-10 18:43:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_user_group_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      309 2022-11-26 11:12:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/siteinfo_for_site_picker.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/smtp_server.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      675 2022-07-04 20:25:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/spo_operation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    18792 2022-12-17 11:45:27.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/tenant.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      218 2022-10-12 10:43:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/theme_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      304 2022-06-23 22:29:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/web_template.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      161 2022-10-08 08:21:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/app_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2022-10-08 08:17:34.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/app_instance.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      408 2022-09-25 07:24:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/cdn_api.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      198 2022-09-25 09:56:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/cdn_url.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.312641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-03 06:29:36.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.312641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-10 19:04:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      671 2022-12-11 11:53:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      212 2022-12-11 16:15:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/external_user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.312641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/results/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-11 11:46:23.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/results/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      853 2022-12-11 16:15:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/results/get.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-12-11 11:53:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/results/remove.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      250 2022-12-11 11:53:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/results/session_revocation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11605 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/office365_tenant.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1252 2022-07-04 10:34:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.316641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-08 08:01:20.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      717 2022-09-28 07:12:08.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/item_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      270 2022-09-28 07:16:40.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/job.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      299 2022-09-28 07:13:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/job_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      491 2022-07-05 07:58:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/job_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      622 2022-09-27 13:32:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/notification_recipient.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      551 2022-09-27 13:32:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/notification_recipient_set_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      565 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/notification_recipient_users.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2022-09-09 18:02:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/requested_translation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2022-12-19 20:00:32.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/resource_entry.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2022-06-24 10:44:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1328 2022-09-28 07:04:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/status_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      348 2022-06-24 10:55:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/status_creation_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      470 2022-09-09 18:10:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/status_set_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2722 2022-09-28 18:26:33.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/sync_translator.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1988 2022-12-19 19:55:43.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/user_resource.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1535 2022-09-28 07:28:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/variations_timer_job.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.316641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/types/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/types/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2022-12-06 22:01:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/types/property_values.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      596 2022-06-16 18:42:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/types/resource_path.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       87 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/types/wopi_action.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.316641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.320641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.320641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-24 17:05:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2022-07-24 17:07:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/entity_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      899 2022-07-24 17:39:25.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/entity_information_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3168 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/query_parameters.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      768 2022-11-27 14:18:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/query_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6186 2022-12-21 15:18:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/web_service_interface.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.320641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/usercustomactions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/usercustomactions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1638 2021-09-13 07:33:07.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/usercustomactions/action.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      925 2022-06-18 19:56:52.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/usercustomactions/collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.324641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      678 2023-01-04 21:05:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/follow_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1637 2023-01-04 21:18:47.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/followed_content.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      416 2023-01-04 21:16:03.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/followed_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1021 2022-10-11 06:16:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/hash_tag.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1737 2022-09-20 17:31:09.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/my_site_links.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11911 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/people_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3123 2022-12-25 10:07:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/person_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1035 2022-11-01 07:25:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/personal_cache.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      299 2022-10-11 06:19:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/personal_cache_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      367 2022-06-07 18:48:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/personal_site_creation_priority.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2081 2022-10-11 06:39:48.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/profile_image_store.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1883 2022-11-01 07:38:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/profile_loader.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2643 2022-11-01 19:00:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/promoted_sites.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1576 2022-09-08 11:42:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/properties_for_user.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.324641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-11 15:32:50.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1201 2022-09-20 17:27:57.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/document.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      312 2022-09-20 07:10:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/document_user.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2022-07-11 15:38:17.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/items.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      339 2022-07-11 15:37:38.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/view_item_removal_result.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4855 2022-11-01 07:43:01.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/user_profile.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.324641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1353 2022-06-24 10:35:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/email_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      688 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/move_copy_options.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4394 2022-07-20 18:16:10.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/move_copy_util.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      242 2022-06-12 07:49:00.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/principal_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      941 2022-06-13 14:02:15.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/upload_status.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8868 2022-12-21 15:10:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/utility.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2022-10-05 19:50:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/wopi_frame_action.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      146 2022-06-18 20:14:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/wopi_properties.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/wopi_web_app_properties.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.328641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1954 2022-12-19 09:54:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1747 2022-12-19 09:54:21.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/create_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2341 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/field_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      506 2022-11-22 21:17:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/scope.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6255 2022-11-22 20:19:18.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/view.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2022-10-06 19:01:12.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/visualization.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.328641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-01 08:39:30.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2022-10-01 12:19:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/app_configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      118 2022-10-26 19:09:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/connections_url_configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1704 2022-11-14 19:06:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/employee_engagement.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-12-05 14:58:11.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/site_request_info.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.328641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1816 2023-01-05 10:17:41.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/subscription.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2165 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/subscription_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1258 2021-10-19 09:23:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/subscription_information.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.328641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.332641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/client/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 10:50:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/client/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      736 2022-07-04 10:52:37.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/client/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      778 2022-12-25 09:51:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/client/webpart.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1604 2022-09-22 06:19:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      893 2022-09-22 06:14:45.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/definition_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1219 2022-07-04 10:59:06.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/limited_manager.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1242 2022-07-04 11:06:55.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/personalization_scope.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      166 2022-07-09 12:46:26.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/tile_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      332 2022-07-04 10:42:24.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/webpart.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.332641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      263 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/calendar_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1230 2022-07-09 08:55:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1187 2022-06-08 07:54:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/context_web_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      371 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      113 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/info_creation_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      144 2022-06-08 17:17:56.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      859 2022-07-09 08:55:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/information_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1227 2022-09-27 13:27:04.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/multilingual_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2723 2022-09-27 13:43:38.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/regional_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1421 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/remote_web.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      528 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/subweb_query.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      525 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/template.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      841 2022-07-09 08:55:05.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/template_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      901 2022-10-06 07:16:44.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/theme_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1783 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/time_zone.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      891 2022-06-02 19:55:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/time_zone_information.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    85514 2023-02-17 13:47:53.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/web.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.336641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workflow/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-02-17 07:31:42.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workflow/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      194 2022-07-04 20:05:46.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workflow/association.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      166 2022-07-04 20:08:22.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workflow/template.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.336641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workflowservices/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-02 20:44:14.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workflowservices/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.336641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workmanagement/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-01-27 20:49:19.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/workmanagement/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.336641 Office365-REST-Python-Client-2.4.0/office365/sharepoint/yammer/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/yammer/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       93 2021-09-03 05:55:31.000000 Office365-REST-Python-Client-2.4.0/office365/sharepoint/yammer/wac_api.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.336641 Office365-REST-Python-Client-2.4.0/office365/subscriptions/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-31 07:27:09.000000 Office365-REST-Python-Client-2.4.0/office365/subscriptions/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1990 2022-12-17 13:19:37.000000 Office365-REST-Python-Client-2.4.0/office365/subscriptions/change_notification.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1362 2022-12-17 13:07:18.000000 Office365-REST-Python-Client-2.4.0/office365/subscriptions/change_notification_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      187 2022-12-17 13:18:22.000000 Office365-REST-Python-Client-2.4.0/office365/subscriptions/encrypted_content.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      278 2022-12-17 13:10:45.000000 Office365-REST-Python-Client-2.4.0/office365/subscriptions/resource_data.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1005 2022-12-17 12:48:31.000000 Office365-REST-Python-Client-2.4.0/office365/subscriptions/subscription.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.340641 Office365-REST-Python-Client-2.4.0/office365/teams/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/teams/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.340641 Office365-REST-Python-Client-2.4.0/office365/teams/apps/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:02:23.000000 Office365-REST-Python-Client-2.4.0/office365/teams/apps/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      971 2022-07-02 08:02:36.000000 Office365-REST-Python-Client-2.4.0/office365/teams/apps/app.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1578 2022-06-26 07:50:16.000000 Office365-REST-Python-Client-2.4.0/office365/teams/apps/definition.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1386 2022-06-25 15:43:00.000000 Office365-REST-Python-Client-2.4.0/office365/teams/apps/installation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      722 2022-09-24 12:25:50.000000 Office365-REST-Python-Client-2.4.0/office365/teams/apps/user_scope_installation.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.340641 Office365-REST-Python-Client-2.4.0/office365/teams/bots/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-09 06:18:01.000000 Office365-REST-Python-Client-2.4.0/office365/teams/bots/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2021-09-09 06:19:05.000000 Office365-REST-Python-Client-2.4.0/office365/teams/bots/teamwork_bot.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.340641 Office365-REST-Python-Client-2.4.0/office365/teams/channels/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:58:03.000000 Office365-REST-Python-Client-2.4.0/office365/teams/channels/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5877 2022-11-29 21:43:59.000000 Office365-REST-Python-Client-2.4.0/office365/teams/channels/channel.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1452 2022-11-29 21:42:00.000000 Office365-REST-Python-Client-2.4.0/office365/teams/channels/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      351 2022-11-29 21:05:33.000000 Office365-REST-Python-Client-2.4.0/office365/teams/channels/membership_type.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      180 2022-11-29 21:43:59.000000 Office365-REST-Python-Client-2.4.0/office365/teams/channels/provision_email_result.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.340641 Office365-REST-Python-Client-2.4.0/office365/teams/chats/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:46:30.000000 Office365-REST-Python-Client-2.4.0/office365/teams/chats/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2544 2022-07-02 08:02:36.000000 Office365-REST-Python-Client-2.4.0/office365/teams/chats/chat.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1115 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/teams/chats/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1449 2022-06-24 20:24:42.000000 Office365-REST-Python-Client-2.4.0/office365/teams/chats/message.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1119 2022-06-24 20:21:37.000000 Office365-REST-Python-Client-2.4.0/office365/teams/chats/message_attachment.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2158 2022-12-25 09:56:18.000000 Office365-REST-Python-Client-2.4.0/office365/teams/collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      276 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.0/office365/teams/fun_settings.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      576 2022-11-20 21:18:10.000000 Office365-REST-Python-Client-2.4.0/office365/teams/guest_settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.344641 Office365-REST-Python-Client-2.4.0/office365/teams/internal/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-04-09 17:22:26.000000 Office365-REST-Python-Client-2.4.0/office365/teams/internal/__init__.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.344641 Office365-REST-Python-Client-2.4.0/office365/teams/internal/paths/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-04-09 17:22:33.000000 Office365-REST-Python-Client-2.4.0/office365/teams/internal/paths/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      293 2022-08-06 09:16:53.000000 Office365-REST-Python-Client-2.4.0/office365/teams/internal/paths/team.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      537 2022-06-26 09:33:00.000000 Office365-REST-Python-Client-2.4.0/office365/teams/member_settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.344641 Office365-REST-Python-Client-2.4.0/office365/teams/members/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-26 08:50:37.000000 Office365-REST-Python-Client-2.4.0/office365/teams/members/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      829 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/teams/members/aad_user_conversation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      373 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.0/office365/teams/members/conversation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.0/office365/teams/members/conversation_collection.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.344641 Office365-REST-Python-Client-2.4.0/office365/teams/messages/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:58:53.000000 Office365-REST-Python-Client-2.4.0/office365/teams/messages/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1273 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/teams/messaging_settings.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.344641 Office365-REST-Python-Client-2.4.0/office365/teams/operations/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:01:17.000000 Office365-REST-Python-Client-2.4.0/office365/teams/operations/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1421 2022-11-29 21:14:51.000000 Office365-REST-Python-Client-2.4.0/office365/teams/operations/async_operation.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      403 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/teams/operations/async_operation_status.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.348641 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:12:57.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      195 2022-06-05 09:35:48.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/availability.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1072 2022-06-05 09:50:47.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/change_tracked_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      217 2021-12-21 19:35:41.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/offer_shift_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      145 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/open_shift_change_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      594 2022-06-05 09:44:02.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/preferences.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1708 2022-10-01 08:34:13.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/schedule.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      651 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/schedule_change_request.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2022-06-06 14:16:09.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/schedule_entity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      147 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/scheduling_group.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      765 2022-06-05 09:34:07.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/shift.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      100 2022-06-05 09:26:17.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/shift_activity.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      776 2022-06-06 14:16:26.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/shift_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      130 2021-09-09 17:41:29.000000 Office365-REST-Python-Client-2.4.0/office365/teams/shifts/time_off_reason.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.348641 Office365-REST-Python-Client-2.4.0/office365/teams/tabs/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:00:53.000000 Office365-REST-Python-Client-2.4.0/office365/teams/tabs/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      384 2022-07-02 07:43:14.000000 Office365-REST-Python-Client-2.4.0/office365/teams/tabs/configuration.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1241 2022-07-02 07:55:46.000000 Office365-REST-Python-Client-2.4.0/office365/teams/tabs/tab.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9805 2022-12-12 19:59:33.000000 Office365-REST-Python-Client-2.4.0/office365/teams/team.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      123 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.0/office365/teams/team_info.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      397 2021-07-27 14:53:28.000000 Office365-REST-Python-Client-2.4.0/office365/teams/template.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2574 2022-09-24 12:28:14.000000 Office365-REST-Python-Client-2.4.0/office365/teams/user_teamwork.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      142 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.0/office365/teams/visibility_type.py
-drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-02-17 17:08:18.348641 Office365-REST-Python-Client-2.4.0/office365/todo/
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-06 07:19:13.000000 Office365-REST-Python-Client-2.4.0/office365/todo/__init__.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-07-08 08:20:03.000000 Office365-REST-Python-Client-2.4.0/office365/todo/checklist_item.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      394 2022-07-08 08:22:33.000000 Office365-REST-Python-Client-2.4.0/office365/todo/linked_resource.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1894 2022-07-08 08:27:42.000000 Office365-REST-Python-Client-2.4.0/office365/todo/task.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1077 2022-08-11 15:15:56.000000 Office365-REST-Python-Client-2.4.0/office365/todo/task_list.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      551 2022-07-08 21:06:29.000000 Office365-REST-Python-Client-2.4.0/office365/todo/task_list_collection.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      500 2022-07-08 20:47:56.000000 Office365-REST-Python-Client-2.4.0/office365/todo/todo.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       36 2022-07-08 18:23:51.000000 Office365-REST-Python-Client-2.4.0/office365/todo/wellknown_list_name.py
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       79 2023-02-17 17:08:18.348641 Office365-REST-Python-Client-2.4.0/setup.cfg
--rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2071 2023-02-17 13:55:22.000000 Office365-REST-Python-Client-2.4.0/setup.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1083 2021-07-11 21:05:58.000000 Office365-REST-Python-Client-2.4.1/LICENSE
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       60 2021-08-09 07:15:24.000000 Office365-REST-Python-Client-2.4.1/MANIFEST.in
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.371856 Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    16132 2023-04-22 08:23:37.000000 Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/PKG-INFO
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    70461 2023-04-22 08:23:37.000000 Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/SOURCES.txt
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        1 2023-04-22 08:23:37.000000 Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/dependency_links.txt
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       49 2023-04-22 08:23:37.000000 Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/requires.txt
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       10 2023-04-22 08:23:37.000000 Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/top_level.txt
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    16132 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/PKG-INFO
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    14930 2023-04-08 10:17:02.000000 Office365-REST-Python-Client-2.4.1/README.md
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.371856 Office365-REST-Python-Client-2.4.1/office365/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2734 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/base_item.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.371856 Office365-REST-Python-Client-2.4.1/office365/communications/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:41:58.000000 Office365-REST-Python-Client-2.4.1/office365/communications/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.371856 Office365-REST-Python-Client-2.4.1/office365/communications/callrecords/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-24 07:16:24.000000 Office365-REST-Python-Client-2.4.1/office365/communications/callrecords/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      631 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/communications/callrecords/call_record.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.375856 Office365-REST-Python-Client-2.4.1/office365/communications/calls/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:45:54.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4292 2022-09-29 16:21:05.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/call.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1671 2022-09-25 17:55:11.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2021-08-24 07:08:22.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/incoming_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      207 2021-09-11 17:07:11.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/invitation_participant_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3023 2022-09-29 16:13:19.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/participant.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      174 2021-08-24 07:12:32.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/participant_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      138 2021-08-24 07:03:15.000000 Office365-REST-Python-Client-2.4.1/office365/communications/calls/route.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2508 2022-09-25 17:36:16.000000 Office365-REST-Python-Client-2.4.1/office365/communications/cloud_communications.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.375856 Office365-REST-Python-Client-2.4.1/office365/communications/meetings/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 21:32:41.000000 Office365-REST-Python-Client-2.4.1/office365/communications/meetings/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.375856 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-24 07:15:35.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2614 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      142 2021-08-24 16:18:09.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/meeting_participant.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      165 2021-09-11 18:49:22.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/meeting_participant_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      789 2021-09-11 18:51:36.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/meeting_participants.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2150 2022-12-04 19:40:44.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/online_meeting.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      208 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/provider_type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.375856 Office365-REST-Python-Client-2.4.1/office365/communications/operations/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:56:10.000000 Office365-REST-Python-Client-2.4.1/office365/communications/operations/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      207 2022-09-29 16:17:04.000000 Office365-REST-Python-Client-2.4.1/office365/communications/operations/cancel_media_processing.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      700 2021-08-06 18:57:58.000000 Office365-REST-Python-Client-2.4.1/office365/communications/operations/comms.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      638 2022-09-29 16:14:05.000000 Office365-REST-Python-Client-2.4.1/office365/communications/operations/invite_participants.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      238 2022-09-28 20:05:15.000000 Office365-REST-Python-Client-2.4.1/office365/communications/operations/start_hold_music.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      235 2022-09-28 20:10:48.000000 Office365-REST-Python-Client-2.4.1/office365/communications/operations/stop_hold_music.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.375856 Office365-REST-Python-Client-2.4.1/office365/communications/presences/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-24 06:54:16.000000 Office365-REST-Python-Client-2.4.1/office365/communications/presences/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4164 2022-09-24 12:11:22.000000 Office365-REST-Python-Client-2.4.1/office365/communications/presences/presence.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      749 2023-02-22 13:42:46.000000 Office365-REST-Python-Client-2.4.1/office365/delta_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2023-02-22 14:09:37.000000 Office365-REST-Python-Client-2.4.1/office365/delta_path.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.375856 Office365-REST-Python-Client-2.4.1/office365/directory/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/directory/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      550 2023-03-12 13:48:02.000000 Office365-REST-Python-Client-2.4.1/office365/directory/administrative_unit.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.379856 Office365-REST-Python-Client-2.4.1/office365/directory/applications/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 11:58:19.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1873 2022-12-17 19:35:18.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/api.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1125 2022-12-17 19:45:10.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/app_identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10243 2022-12-19 15:46:04.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/application.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      673 2022-12-17 19:40:47.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/public_client.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.379856 Office365-REST-Python-Client-2.4.1/office365/directory/applications/roles/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 15:56:05.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/roles/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      717 2022-10-01 08:25:32.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/roles/assignment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      289 2022-12-18 16:07:08.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/roles/role.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9345 2023-03-08 20:01:38.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/service_principal.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      322 2022-12-17 19:52:50.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/spa.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2315 2022-12-17 19:16:43.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/template.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      922 2022-12-17 19:51:21.000000 Office365-REST-Python-Client-2.4.1/office365/directory/applications/web.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.379856 Office365-REST-Python-Client-2.4.1/office365/directory/audit/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 10:06:48.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      853 2022-12-17 20:53:20.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/activity_initiator.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1384 2022-12-17 21:05:32.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/directory.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2740 2022-12-18 11:36:36.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/log_root.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.379856 Office365-REST-Python-Client-2.4.1/office365/directory/audit/provisioning/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 11:25:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/provisioning/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       37 2022-12-18 11:41:51.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/provisioning/action.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      493 2022-12-18 11:33:53.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/provisioning/object_summary.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      176 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/provisioning/service_principal.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.379856 Office365-REST-Python-Client-2.4.1/office365/directory/audit/signins/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 11:26:01.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/signins/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      179 2023-03-08 19:45:40.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/signins/location.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1936 2023-03-11 21:04:51.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/signins/signin.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      792 2022-12-18 11:25:28.000000 Office365-REST-Python-Client-2.4.1/office365/directory/audit/signins/status.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.379856 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-27 07:44:48.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2744 2022-11-20 20:23:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/authentication.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      773 2022-12-01 15:07:35.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/basic.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      872 2023-03-11 15:09:57.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/client_certificate.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      741 2022-09-29 17:49:23.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/configuration_base.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.383856 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-20 15:58:26.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      253 2022-11-20 20:15:01.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/fido.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2359 2022-09-27 07:55:02.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/method.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      313 2022-11-20 20:18:33.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/password.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2259 2022-11-20 16:05:43.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/phone.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      372 2022-11-20 16:07:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/authentication/password_reset_response.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.383856 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-09 13:59:09.000000 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1314 2022-11-30 22:08:56.000000 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/auth_configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      857 2022-09-19 06:43:19.000000 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/authority.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      157 2022-12-18 16:14:42.000000 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/certification.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1061 2023-03-11 15:09:57.000000 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/pkcs12_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2022-11-30 22:22:23.000000 Office365-REST-Python-Client-2.4.1/office365/directory/certificates/self_signed.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2034 2023-03-12 13:49:47.000000 Office365-REST-Python-Client-2.4.1/office365/directory/directory.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.383856 Office365-REST-Python-Client-2.4.1/office365/directory/domains/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 16:50:42.000000 Office365-REST-Python-Client-2.4.1/office365/directory/domains/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      225 2023-03-14 18:55:34.000000 Office365-REST-Python-Client-2.4.1/office365/directory/domains/dns_cname_record.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      294 2022-12-18 16:55:02.000000 Office365-REST-Python-Client-2.4.1/office365/directory/domains/dns_record.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3974 2023-03-08 20:31:02.000000 Office365-REST-Python-Client-2.4.1/office365/directory/domains/domain.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      248 2023-03-14 19:03:48.000000 Office365-REST-Python-Client-2.4.1/office365/directory/domains/verified.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.383856 Office365-REST-Python-Client-2.4.1/office365/directory/extensions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 13:49:51.000000 Office365-REST-Python-Client-2.4.1/office365/directory/extensions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      488 2023-04-13 19:01:28.000000 Office365-REST-Python-Client-2.4.1/office365/directory/extensions/extended_property.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      152 2021-08-06 13:47:48.000000 Office365-REST-Python-Client-2.4.1/office365/directory/extensions/extension.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1859 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.1/office365/directory/extensions/extension_property.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.383856 Office365-REST-Python-Client-2.4.1/office365/directory/groups/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 11:58:39.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1542 2023-03-18 09:38:50.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10027 2023-03-18 09:57:34.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2466 2023-02-13 18:25:25.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/lifecycle_policy.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      565 2022-04-09 13:48:19.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/profile.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/setting.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      323 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.1/office365/directory/groups/setting_template.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/identities/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:58:24.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1825 2022-12-01 15:07:35.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/api_connector.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2021-09-11 09:25:41.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/conditional_access_root.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3261 2022-09-19 06:52:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/container.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      376 2023-03-14 18:27:51.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/governance.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1668 2022-09-30 07:43:58.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/object_identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      177 2023-03-11 15:32:45.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/protection_root.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1024 2022-09-19 06:42:22.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1000 2022-12-18 18:52:22.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/provider_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-11 09:26:29.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      424 2021-08-09 16:50:30.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/base.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1022 2022-12-18 18:54:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/base_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      531 2022-09-19 06:39:52.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/builtin_identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      461 2022-09-19 06:38:48.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/saml_or_wsfed.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1272 2022-09-19 06:34:14.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/social_identity.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 19:29:05.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      661 2021-09-11 09:34:54.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/attribute.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/b2x/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-11 09:31:47.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/b2x/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2719 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/b2x/user_flow.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2114 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/language_configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      362 2022-06-30 19:55:04.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/language_page.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      652 2021-09-11 08:34:50.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/user_attribute_assignment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       79 2021-08-09 16:30:24.000000 Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/user_flow.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/insights/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-05 15:01:40.000000 Office365-REST-Python-Client-2.4.1/office365/directory/insights/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2269 2023-03-11 16:07:39.000000 Office365-REST-Python-Client-2.4.1/office365/directory/insights/office_graph.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      422 2023-03-11 15:57:12.000000 Office365-REST-Python-Client-2.4.1/office365/directory/insights/shared.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      282 2023-03-11 15:54:12.000000 Office365-REST-Python-Client-2.4.1/office365/directory/insights/trending.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2023-03-11 16:07:08.000000 Office365-REST-Python-Client-2.4.1/office365/directory/insights/used.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-08-05 15:00:14.000000 Office365-REST-Python-Client-2.4.1/office365/directory/internal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.387856 Office365-REST-Python-Client-2.4.1/office365/directory/internal/paths/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-08-05 15:00:22.000000 Office365-REST-Python-Client-2.4.1/office365/directory/internal/paths/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-08-05 20:37:22.000000 Office365-REST-Python-Client-2.4.1/office365/directory/internal/paths/me.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1089 2023-03-12 13:55:21.000000 Office365-REST-Python-Client-2.4.1/office365/directory/key_credential.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.391856 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 13:52:30.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      706 2022-12-18 13:11:23.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/assigned_license.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2021-08-09 14:42:31.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/assigned_plan.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      568 2023-03-08 19:51:55.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/assignment_state.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1115 2021-08-06 14:03:08.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/details.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1595 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/service_plan_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      857 2023-03-11 16:12:19.000000 Office365-REST-Python-Client-2.4.1/office365/directory/licenses/subscribed_sku.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4285 2023-03-12 13:39:51.000000 Office365-REST-Python-Client-2.4.1/office365/directory/object.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4205 2022-11-20 16:18:09.000000 Office365-REST-Python-Client-2.4.1/office365/directory/object_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1009 2022-12-17 19:18:30.000000 Office365-REST-Python-Client-2.4.1/office365/directory/password_credential.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.391856 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 21:27:37.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.391856 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/grants/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-18 11:54:10.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/grants/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1549 2022-12-18 12:11:52.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/grants/condition_set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2778 2023-03-15 19:35:03.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/grants/oauth2.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      614 2023-03-16 19:37:00.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/grants/resource_specific.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      808 2022-12-18 11:40:31.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      838 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/identity_set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1220 2022-12-17 20:50:01.000000 Office365-REST-Python-Client-2.4.1/office365/directory/permissions/scope.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.391856 Office365-REST-Python-Client-2.4.1/office365/directory/policies/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 08:25:01.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2022-12-18 13:02:47.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/authentication_methods.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      284 2022-12-17 18:55:42.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/authorization.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      357 2022-10-01 08:21:16.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/base.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2021-08-10 08:27:22.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/conditional_access.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1578 2022-12-18 12:54:15.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/permission_grant.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2991 2022-12-18 13:06:56.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/root.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      926 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.1/office365/directory/policies/sts.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      699 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/directory/profile_photo.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.391856 Office365-REST-Python-Client-2.4.1/office365/directory/rbac/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 17:57:14.000000 Office365-REST-Python-Client-2.4.1/office365/directory/rbac/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      941 2023-03-11 21:13:12.000000 Office365-REST-Python-Client-2.4.1/office365/directory/rbac/application.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      283 2023-03-11 21:08:33.000000 Office365-REST-Python-Client-2.4.1/office365/directory/rbac/unified_role_assignment.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.395856 Office365-REST-Python-Client-2.4.1/office365/directory/roles/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 17:53:05.000000 Office365-REST-Python-Client-2.4.1/office365/directory/roles/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      738 2022-11-30 18:02:39.000000 Office365-REST-Python-Client-2.4.1/office365/directory/roles/management.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      639 2022-12-01 20:39:52.000000 Office365-REST-Python-Client-2.4.1/office365/directory/roles/role.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      249 2022-09-30 07:27:44.000000 Office365-REST-Python-Client-2.4.1/office365/directory/roles/template.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.395856 Office365-REST-Python-Client-2.4.1/office365/directory/security/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 21:22:03.000000 Office365-REST-Python-Client-2.4.1/office365/directory/security/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      233 2022-07-08 21:24:49.000000 Office365-REST-Python-Client-2.4.1/office365/directory/security/security.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.395856 Office365-REST-Python-Client-2.4.1/office365/directory/users/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 11:58:29.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       77 2023-03-15 21:28:50.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/activity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      908 2022-07-11 13:13:42.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      852 2022-12-17 12:57:10.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3101 2023-03-11 14:18:12.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/invitation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1248 2023-03-11 15:05:32.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/invited_user_message_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      404 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/password_profile.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1370 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/profile.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      807 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    30678 2023-04-08 10:18:08.000000 Office365-REST-Python-Client-2.4.1/office365/directory/users/user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.395856 Office365-REST-Python-Client-2.4.1/office365/education/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 15:54:41.000000 Office365-REST-Python-Client-2.4.1/office365/education/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      436 2022-07-08 15:56:25.000000 Office365-REST-Python-Client-2.4.1/office365/education/class.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      176 2022-07-08 16:00:19.000000 Office365-REST-Python-Client-2.4.1/office365/education/root.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      444 2022-07-08 15:57:47.000000 Office365-REST-Python-Client-2.4.1/office365/education/user.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1934 2022-08-09 07:05:20.000000 Office365-REST-Python-Client-2.4.1/office365/entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1457 2022-12-19 12:52:47.000000 Office365-REST-Python-Client-2.4.1/office365/entity_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.395856 Office365-REST-Python-Client-2.4.1/office365/external/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 21:10:06.000000 Office365-REST-Python-Client-2.4.1/office365/external/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      163 2022-07-08 21:14:47.000000 Office365-REST-Python-Client-2.4.1/office365/external/connection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      658 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/external/external.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    12730 2023-03-14 18:32:24.000000 Office365-REST-Python-Client-2.4.1/office365/graph_client.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      241 2023-02-22 14:07:27.000000 Office365-REST-Python-Client-2.4.1/office365/graph_request.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.395856 Office365-REST-Python-Client-2.4.1/office365/intune/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-19 07:01:31.000000 Office365-REST-Python-Client-2.4.1/office365/intune/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.399856 Office365-REST-Python-Client-2.4.1/office365/intune/audit/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-16 09:22:23.000000 Office365-REST-Python-Client-2.4.1/office365/intune/audit/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1117 2022-12-16 09:30:34.000000 Office365-REST-Python-Client-2.4.1/office365/intune/audit/event.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.399856 Office365-REST-Python-Client-2.4.1/office365/intune/devices/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-04 12:58:14.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1070 2023-04-04 09:22:52.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/app_management.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      105 2022-12-16 09:21:45.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      287 2023-03-11 21:02:03.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/detail.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2866 2022-12-18 16:40:07.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/device.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      742 2023-03-11 20:42:09.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/managed.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      144 2023-03-12 08:15:15.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/managed_app_diagnostic_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      343 2023-04-04 09:20:38.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/managed_app_registration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      144 2023-03-11 20:30:09.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/managed_ebook.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1515 2023-03-11 20:50:15.000000 Office365-REST-Python-Client-2.4.1/office365/intune/devices/management.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.399856 Office365-REST-Python-Client-2.4.1/office365/intune/organizations/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 14:14:38.000000 Office365-REST-Python-Client-2.4.1/office365/intune/organizations/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      880 2023-03-14 18:59:26.000000 Office365-REST-Python-Client-2.4.1/office365/intune/organizations/branding_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2328 2022-12-17 12:28:09.000000 Office365-REST-Python-Client-2.4.1/office365/intune/organizations/contact.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2953 2023-03-14 19:05:08.000000 Office365-REST-Python-Client-2.4.1/office365/intune/organizations/organization.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      403 2023-03-11 15:35:53.000000 Office365-REST-Python-Client-2.4.1/office365/intune/provisioned_plan.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      844 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/logger.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.399856 Office365-REST-Python-Client-2.4.1/office365/onedrive/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.403856 Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 09:59:42.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      196 2022-11-30 17:14:29.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/item_action_stat.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1207 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/item_activity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1152 2023-03-13 20:24:05.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/item_activity_stat.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1276 2023-03-13 06:52:40.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/item_analytics.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.407856 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:41:50.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      198 2023-03-13 20:13:37.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/boolean.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      807 2022-03-06 18:26:06.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/calculated.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      871 2022-06-04 19:54:06.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/choice.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2021-08-10 19:10:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/column_link.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      387 2022-03-06 18:46:50.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/currency.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      437 2021-08-06 15:48:48.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/default_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6026 2023-03-13 20:16:19.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2641 2022-10-17 18:51:08.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/definition_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-06-23 07:24:46.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/display_name_localization.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      192 2021-08-10 18:54:25.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/geolocation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      388 2022-10-12 06:58:07.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/hyperlink_or_picture.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1110 2022-10-12 06:50:02.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/lookup.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1274 2022-03-07 09:28:10.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/number.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      892 2022-07-08 08:39:21.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/person_or_group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      648 2022-03-07 18:49:02.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/term.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      722 2022-06-23 14:56:54.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/text.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      274 2022-03-07 09:48:54.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/thumbnail.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       66 2022-06-23 19:53:42.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/types.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      832 2022-06-23 07:24:46.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/validation.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.407856 Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:48:29.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3867 2022-12-04 19:19:05.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7288 2022-12-04 19:21:48.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/content_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      405 2022-07-08 08:35:55.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      530 2022-06-05 07:45:32.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/order.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.407856 Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 19:14:21.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      760 2022-09-29 12:41:02.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/content.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1456 2023-03-13 20:27:43.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/document_set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1200 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/version.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      545 2023-03-13 20:27:43.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/version_item.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.411856 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:40:08.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      375 2021-08-11 09:02:39.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/audio.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/conflict_behavior.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    23307 2023-02-22 14:11:28.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/driveItem.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      799 2022-09-29 14:47:23.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/geo_coordinates.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      388 2021-08-11 09:05:36.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/image.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      242 2022-11-30 17:24:23.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/item_preview_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      203 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/photo.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      647 2022-11-20 21:18:10.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/publication_facet.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      639 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/remote_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      203 2021-08-11 09:14:40.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/special_folder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2021-08-05 10:00:45.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/system_facet.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      953 2022-07-15 16:07:27.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/thumbnail.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      886 2021-08-10 09:49:49.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/thumbnail_set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      620 2022-09-29 14:38:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/uploadable_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/video.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.411856 Office365-REST-Python-Client-2.4.1/office365/onedrive/drives/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:30:49.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/drives/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4354 2023-04-04 20:36:55.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/drives/drive.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      886 2023-03-14 18:19:28.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/drives/recipient.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.411856 Office365-REST-Python-Client-2.4.1/office365/onedrive/files/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:44:01.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/files/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      859 2022-09-29 12:37:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/files/file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      587 2022-09-29 12:37:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/files/system_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.411856 Office365-REST-Python-Client-2.4.1/office365/onedrive/folders/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:44:12.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/folders/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      692 2022-09-29 14:38:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/folders/folder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      755 2022-10-12 06:53:21.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/folders/view.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.411856 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-02 10:37:03.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.415856 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 14:30:09.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      562 2022-08-06 12:35:57.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/children.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      504 2022-08-06 09:11:12.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/root.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      473 2022-06-05 19:29:01.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/shared.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      693 2022-08-06 11:59:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/site.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      986 2022-08-06 11:51:43.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/url.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.415856 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 14:29:30.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      995 2022-12-05 14:48:27.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/download_content.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1007 2023-03-14 15:54:18.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/get_activities_by_interval.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1083 2022-11-13 13:20:09.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/resumable_file_upload.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      917 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/upload_content.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.415856 Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:44:49.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      137 2021-08-06 09:57:23.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/field_value_set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1109 2022-03-07 09:51:29.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/item_reference.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3608 2022-11-21 15:20:10.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/list_item.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.415856 Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:39:52.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      738 2022-09-29 12:55:18.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      905 2022-09-29 13:06:17.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3193 2022-12-17 19:22:25.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/list.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.419856 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:47:57.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4937 2023-03-13 19:59:27.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/permission.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      500 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/sharepoint_identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1169 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/sharepoint_identity_set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1062 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/sharing_invitation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      641 2022-06-26 09:35:31.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/sharing_link.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      108 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/root.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      816 2022-09-29 14:34:36.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/sharepoint_ids.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.419856 Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:44:09.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      574 2022-09-29 14:34:37.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2700 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/drive_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      687 2022-06-05 10:24:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/shared.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.419856 Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 09:32:09.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8297 2022-11-30 17:17:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/site.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      698 2022-05-31 14:50:54.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/site_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1456 2022-10-11 18:35:34.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/sites_with_root.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.423856 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-03-07 18:46:33.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1332 2022-07-20 16:56:52.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      546 2022-03-08 10:04:08.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/localized_description.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      720 2022-03-14 13:10:47.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/localized_label.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      583 2022-03-14 09:41:47.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/localized_name.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2281 2022-03-23 18:27:21.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/relation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2490 2022-08-06 08:57:41.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1836 2022-07-20 17:06:50.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/set_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2336 2022-11-30 21:53:41.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/store.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1769 2022-08-06 09:01:28.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/term.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1267 2022-07-24 10:17:43.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/term_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      191 2022-03-08 09:51:50.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/term_group_scope.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.423856 Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-10 09:49:47.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      586 2022-07-06 09:04:57.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/base_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1052 2022-11-20 21:14:39.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/drive_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1206 2022-11-21 15:04:57.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/list_item.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.423856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.423856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/applications/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 18:37:17.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/applications/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      914 2022-11-30 20:37:05.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/applications/application.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:35:36.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      159 2022-07-08 09:19:09.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/area_format.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      117 2022-07-08 09:15:10.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/axes.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1508 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/chart.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      323 2022-07-08 09:13:58.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      161 2022-07-08 09:16:31.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/data_labels.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2022-07-08 09:18:01.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/legend.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       82 2022-07-08 09:16:59.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/series.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/comments/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:41:32.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/comments/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      595 2022-12-04 11:53:07.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/comments/comment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      124 2022-12-04 11:53:07.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/comments/reply.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      121 2022-12-04 11:55:39.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/filter.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/functions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:35:56.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/functions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2700 2023-04-08 08:04:45.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/functions/functions.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      165 2023-04-08 07:54:34.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/functions/result.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/names/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:40:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/names/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1181 2022-07-08 09:28:40.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/names/named_item.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/operations/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:41:07.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/operations/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      140 2022-07-08 12:18:33.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/operations/workbook.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:34:53.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      670 2022-07-08 14:16:15.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/format.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      140 2022-07-08 14:17:07.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/format_protection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1235 2022-12-04 12:52:52.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/range.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      111 2022-11-30 20:26:20.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/reference.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      594 2022-12-04 12:06:00.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/view.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      484 2022-07-08 11:54:29.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/session_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.427856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:35:18.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1687 2022-11-19 17:33:51.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/columns/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 20:07:10.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/columns/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1348 2022-12-04 12:36:33.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/columns/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1533 2022-12-04 17:10:46.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/columns/column.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1182 2022-07-08 14:12:51.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/pivot_table.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/rows/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 20:06:44.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/rows/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1429 2022-11-19 17:53:08.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/rows/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      601 2022-11-10 18:46:16.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/rows/row.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2972 2022-12-04 12:56:34.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/table.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5951 2023-03-01 09:52:14.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/workbook.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:36:22.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1300 2022-11-20 20:31:37.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       90 2022-07-08 09:26:08.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/protection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      167 2022-07-08 09:08:32.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/protection_options.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2834 2022-11-10 20:12:39.000000 Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/worksheet.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onenote/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      139 2021-08-15 18:22:15.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/entity_base_model.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1341 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/entity_hierarchy_model.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      570 2021-08-15 18:26:08.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/entity_schema_object_model.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onenote/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-10-31 11:48:19.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/internal/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2866 2023-03-12 14:37:50.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/internal/multipart_page_query.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:16.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2578 2023-03-12 15:19:33.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2021-08-16 08:23:29.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/copy_notebook_model.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1511 2022-03-23 18:27:20.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/notebook.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      754 2023-03-12 15:25:12.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/recent.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      476 2023-03-12 15:27:33.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/recent_links.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2847 2023-03-12 14:37:50.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/onenote.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.431856 Office365-REST-Python-Client-2.4.1/office365/onenote/operations/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:09:18.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/operations/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      406 2021-08-15 18:18:58.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/operations/onenote.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      423 2021-08-15 18:19:23.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/operations/onenote_operation_error.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       72 2021-08-15 18:16:32.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/operations/operation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-16 07:32:23.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/operations/operation_status.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.435856 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:03.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      861 2023-03-12 14:46:31.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      337 2023-03-12 14:41:00.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/external_link.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      642 2023-03-12 14:41:00.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/links.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2802 2023-03-12 14:37:50.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/page.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      284 2023-03-12 15:18:36.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/pages/preview_links.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.435856 Office365-REST-Python-Client-2.4.1/office365/onenote/resources/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:59.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/resources/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      762 2023-03-12 15:15:47.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/resources/resource.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.435856 Office365-REST-Python-Client-2.4.1/office365/onenote/sectiongroups/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:29:37.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/sectiongroups/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2383 2022-06-16 07:46:41.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/sectiongroups/section_group.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.435856 Office365-REST-Python-Client-2.4.1/office365/onenote/sections/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-15 18:14:30.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/sections/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3617 2023-03-12 14:37:50.000000 Office365-REST-Python-Client-2.4.1/office365/onenote/sections/section.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.435856 Office365-REST-Python-Client-2.4.1/office365/outlook/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-02 10:12:23.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.439856 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.439856 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-01 13:32:41.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      935 2023-03-01 13:41:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/attendee.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      142 2023-03-01 13:41:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/availability.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      655 2023-03-01 13:41:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/base.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4614 2023-03-01 10:07:30.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/calendar.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      870 2022-02-20 19:56:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/dateTimeTimeZone.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      313 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/email_address.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.439856 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/events/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-01 10:03:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/events/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9228 2023-03-01 13:41:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/events/event.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      446 2022-06-05 10:11:43.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/events/reminder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      966 2022-12-03 18:39:33.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      180 2022-06-05 10:08:53.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/location_constraint.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.439856 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/meetingtimes/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-01 10:24:07.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/meetingtimes/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1459 2023-03-01 13:41:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/meetingtimes/suggestion.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1193 2023-03-01 10:28:11.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/meetingtimes/suggestions_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1679 2022-06-05 10:14:49.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/permission.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      594 2021-09-10 06:57:12.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/place.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      368 2022-06-05 10:19:34.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/role_type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.439856 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/schedule/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-29 21:16:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/schedule/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1881 2022-11-29 21:21:03.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/schedule/information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      299 2022-11-29 21:16:30.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/schedule/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       87 2023-04-13 19:01:28.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/sharing_message.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      576 2023-03-01 10:48:30.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/time_slot.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      415 2023-03-01 10:33:37.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/time_zone_base.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      457 2023-03-01 10:39:45.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/working_hours.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      742 2023-03-13 20:10:36.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/category.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.443856 Office365-REST-Python-Client-2.4.1/office365/outlook/contacts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-02 10:14:30.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/contacts/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3953 2022-07-17 14:15:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/contacts/contact.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2545 2022-12-03 18:45:01.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/contacts/folder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      564 2023-04-09 07:59:04.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/convert_id_result.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.443856 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-10 06:58:23.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.443856 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/paths/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-16 10:46:01.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/paths/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.443856 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/queries/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-16 10:46:10.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/queries/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1894 2022-11-13 13:35:09.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/internal/queries/attachment_upload.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1696 2023-04-09 08:25:48.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      828 2023-02-14 07:22:48.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/locale_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.443856 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.443856 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-10 06:57:10.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2093 2022-12-05 14:50:02.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/attachment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      800 2022-08-04 09:37:01.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/attachment_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/attachment_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3025 2023-04-10 13:43:20.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      962 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      540 2022-12-04 17:35:27.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      297 2023-03-13 20:12:17.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/reference.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      347 2023-02-14 07:26:13.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/automatic_replies_setting.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       90 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/body_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      783 2023-03-16 19:45:47.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/conversation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2120 2023-03-14 18:45:46.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/conversation_thread.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3348 2022-12-04 17:39:16.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/folder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      114 2022-06-23 14:44:05.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/importance.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      525 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/item_body.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      362 2023-03-01 13:27:31.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/location.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      899 2023-02-14 07:29:06.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/mailbox_settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-10 07:21:38.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1396 2022-12-04 19:40:44.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1077 2023-04-13 19:01:28.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/event_message.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10741 2023-04-10 13:43:20.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/message.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      486 2022-12-04 17:39:16.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/message_rule.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      538 2022-12-01 20:30:26.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/patterned_recurrence.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      608 2022-12-04 19:43:14.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/physical_address.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      139 2022-12-04 19:17:59.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/post.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      759 2022-12-04 17:26:31.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/recipient.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      421 2022-12-04 17:41:44.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/recurrence_pattern.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      427 2022-12-04 19:44:59.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/mail/recurrence_range.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      600 2022-11-20 13:31:00.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/timezone_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2764 2022-11-29 21:42:01.000000 Office365-REST-Python-Client-2.4.1/office365/outlook/user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/planner/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:42:11.000000 Office365-REST-Python-Client-2.4.1/office365/planner/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/planner/buckets/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:45:34.000000 Office365-REST-Python-Client-2.4.1/office365/planner/buckets/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      695 2023-03-12 15:12:01.000000 Office365-REST-Python-Client-2.4.1/office365/planner/buckets/bucket.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      620 2022-12-05 09:08:49.000000 Office365-REST-Python-Client-2.4.1/office365/planner/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1655 2022-03-23 18:27:20.000000 Office365-REST-Python-Client-2.4.1/office365/planner/planner.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/planner/plans/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:43:41.000000 Office365-REST-Python-Client-2.4.1/office365/planner/plans/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1343 2022-12-05 09:06:20.000000 Office365-REST-Python-Client-2.4.1/office365/planner/plans/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2445 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/planner/plans/plan.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2021-11-07 08:27:57.000000 Office365-REST-Python-Client-2.4.1/office365/planner/plans/plan_details.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/planner/tasks/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-17 16:43:34.000000 Office365-REST-Python-Client-2.4.1/office365/planner/tasks/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      281 2021-08-17 18:57:10.000000 Office365-REST-Python-Client-2.4.1/office365/planner/tasks/check_list_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      587 2021-08-17 19:00:14.000000 Office365-REST-Python-Client-2.4.1/office365/planner/tasks/check_list_items.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      931 2023-03-13 06:47:15.000000 Office365-REST-Python-Client-2.4.1/office365/planner/tasks/task.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      228 2021-08-17 17:02:59.000000 Office365-REST-Python-Client-2.4.1/office365/planner/tasks/task_details.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1098 2022-12-05 09:06:46.000000 Office365-REST-Python-Client-2.4.1/office365/planner/user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/project/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-05 07:58:43.000000 Office365-REST-Python-Client-2.4.1/office365/project/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      163 2022-07-05 08:00:40.000000 Office365-REST-Python-Client-2.4.1/office365/project/project.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/reports/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-11 13:05:47.000000 Office365-REST-Python-Client-2.4.1/office365/reports/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.447856 Office365-REST-Python-Client-2.4.1/office365/reports/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-30 09:30:26.000000 Office365-REST-Python-Client-2.4.1/office365/reports/internal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.451856 Office365-REST-Python-Client-2.4.1/office365/reports/internal/queries/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-30 09:30:34.000000 Office365-REST-Python-Client-2.4.1/office365/reports/internal/queries/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      868 2022-11-30 17:32:59.000000 Office365-REST-Python-Client-2.4.1/office365/reports/internal/queries/create_report_query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      347 2022-07-08 18:01:57.000000 Office365-REST-Python-Client-2.4.1/office365/reports/report.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8779 2022-11-30 17:43:43.000000 Office365-REST-Python-Client-2.4.1/office365/reports/report_root.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.451856 Office365-REST-Python-Client-2.4.1/office365/runtime/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.451856 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4478 2022-11-13 14:54:20.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/authentication_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      320 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/authentication_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      273 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/client_credential.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      115 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/credential_type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.455856 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4125 2023-04-19 06:11:09.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/acs_token_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      488 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/network_credential_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      974 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/ntlm_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      921 2022-07-27 15:21:37.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/oauth_token_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11495 2022-10-26 18:59:46.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/saml_token_provider.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.455856 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2115 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/FederatedSAML.xml
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1513 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/RST2.xml
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1526 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/SAML.xml
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1232 2022-05-31 14:50:36.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/sts_profile.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      854 2022-07-27 15:21:37.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/token_response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      224 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/user_credential.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      238 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/auth/user_realm_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8011 2023-02-22 09:35:00.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_object.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7010 2022-12-18 13:53:54.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_object_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4469 2022-11-19 10:33:32.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1322 2022-06-07 13:08:17.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_request_exception.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1970 2023-04-22 08:11:33.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7970 2023-03-18 09:57:34.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_runtime_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2036 2022-08-12 13:40:49.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2763 2023-01-08 15:44:58.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/client_value_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1687 2022-07-27 15:29:10.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/compat.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.455856 Office365-REST-Python-Client-2.4.1/office365/runtime/csom/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/csom/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.455856 Office365-REST-Python-Client-2.4.1/office365/runtime/http/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/http/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      148 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/http/http_method.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      830 2021-10-30 19:54:58.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/http/request_options.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.455856 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      881 2022-08-12 13:51:15.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/json_format.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      270 2022-12-25 10:58:06.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/method.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      356 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/model.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      165 2022-12-25 10:58:06.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/parameter.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      141 2022-12-25 11:01:56.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/property.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3718 2023-04-13 19:01:28.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/query_options.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2341 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/reader.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5885 2023-04-17 19:42:18.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2771 2022-12-24 11:19:58.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-06-06 20:38:04.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/type_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1905 2023-04-13 19:01:28.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/url_builder.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.455856 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 12:50:06.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5571 2022-11-13 13:35:10.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/batch_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1108 2022-08-14 08:49:20.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/json_light_format.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      571 2022-02-20 20:24:12.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/metadata_level.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      449 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/metadata_reader.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.459856 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-27 12:50:14.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2930 2022-11-13 13:37:10.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/batch_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1165 2022-08-12 13:51:15.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/json_format.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      590 2022-08-12 08:53:57.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/metadata_level.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      376 2022-07-05 08:22:53.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/metadata_reader.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1426 2023-04-16 08:07:09.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/upload_session.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2346 2023-04-16 08:01:16.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/upload_session_request.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.459856 Office365-REST-Python-Client-2.4.1/office365/runtime/paths/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-11-12 20:47:45.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/paths/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      924 2023-03-16 20:33:34.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/paths/entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      183 2022-12-19 12:52:47.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/paths/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      978 2023-03-05 13:58:19.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/paths/resource_path.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      780 2023-04-15 13:44:42.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/paths/service_operation.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.459856 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1813 2022-11-13 13:35:09.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/batch.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1718 2023-04-15 13:44:42.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/client_query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      827 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/create_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      367 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/delete_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1233 2023-04-17 19:11:23.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/function.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      815 2023-04-15 13:44:42.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/read_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1710 2023-04-17 19:11:23.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/service_operation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      589 2022-11-13 19:59:22.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/update_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      756 2023-04-15 14:00:37.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/queries/upload_session.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.459856 Office365-REST-Python-Client-2.4.1/office365/runtime/types/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/types/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      561 2022-06-04 19:54:06.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/types/collections.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      558 2022-08-03 08:58:31.000000 Office365-REST-Python-Client-2.4.1/office365/runtime/types/event_handler.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.463857 Office365-REST-Python-Client-2.4.1/office365/search/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-01 08:39:25.000000 Office365-REST-Python-Client-2.4.1/office365/search/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      652 2022-07-08 11:38:29.000000 Office365-REST-Python-Client-2.4.1/office365/search/aggregation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2022-07-08 11:33:40.000000 Office365-REST-Python-Client-2.4.1/office365/search/alteration_options.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1045 2023-03-13 06:41:02.000000 Office365-REST-Python-Client-2.4.1/office365/search/bucket.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2327 2023-03-14 19:15:45.000000 Office365-REST-Python-Client-2.4.1/office365/search/entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      283 2022-07-08 11:03:52.000000 Office365-REST-Python-Client-2.4.1/office365/search/entity_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      800 2022-07-08 11:28:30.000000 Office365-REST-Python-Client-2.4.1/office365/search/hit.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1235 2022-07-08 11:32:52.000000 Office365-REST-Python-Client-2.4.1/office365/search/hits_container.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      404 2022-07-08 10:33:47.000000 Office365-REST-Python-Client-2.4.1/office365/search/query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2268 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/search/request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      856 2023-03-14 19:33:07.000000 Office365-REST-Python-Client-2.4.1/office365/search/response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      206 2023-03-13 06:42:07.000000 Office365-REST-Python-Client-2.4.1/office365/search/sharepoint_onedrive_options.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      144 2022-07-08 10:39:04.000000 Office365-REST-Python-Client-2.4.1/office365/search/sort_property.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.463857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.463857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-11 06:54:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      464 2022-11-08 19:15:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/action_facet.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      215 2022-11-08 14:53:55.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/capabilities.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      108 2022-11-08 14:46:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/client_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      373 2022-11-08 19:15:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/entity.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/facets/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-08 19:00:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/facets/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      214 2022-11-08 19:03:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/facets/rename.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      522 2022-11-08 19:08:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/facets/sharing.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2022-11-08 19:04:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      201 2022-11-08 15:05:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/logger.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      967 2022-11-08 15:15:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/tracked_item_service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      442 2023-03-11 13:21:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/tracked_item_updates_request.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/addtoonedrive/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-19 21:22:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/addtoonedrive/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-12-19 21:24:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/addtoonedrive/mount_service.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/addtoonedrive/requests/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-19 21:22:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/addtoonedrive/requests/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      111 2022-12-19 21:25:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/addtoonedrive/requests/get_remote_item_Info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/analytics/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-15 09:26:38.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/analytics/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1288 2022-09-25 11:22:28.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/analytics/usage_service.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/orgassets/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-08 10:17:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/orgassets/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/orgassets/library.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      113 2022-07-08 10:25:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/orgassets/library_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      390 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/orgassets/org_assets.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1239 2023-03-20 18:11:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/web_application.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1193 2023-04-17 19:11:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/web_service.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1234 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/alert.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1736 2022-09-26 07:17:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      609 2022-02-03 12:29:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/creation_information.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/analytics/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:40:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/analytics/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2439 2023-04-17 19:11:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/analytics/usage_entry.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.467857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-26 06:23:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1836 2023-04-17 19:11:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/credential.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      228 2023-03-02 19:10:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/identity_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      168 2022-09-26 06:26:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      145 2022-09-26 06:23:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/name.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-14 07:18:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      191 2022-12-06 10:57:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/app_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      131 2023-03-11 12:53:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/license.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      385 2023-03-11 12:53:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/license_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      702 2023-03-11 12:56:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/license_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2023-03-11 12:53:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2023-03-02 19:55:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/solution_exporter.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       99 2023-03-02 19:14:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/apps/user_solution.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4084 2022-10-01 12:50:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/attachment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3100 2022-06-18 19:56:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      924 2022-06-11 10:38:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/creation_information.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/audit/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-03 10:02:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/audit/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      674 2022-07-03 20:08:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/audit/audit.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authentication/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-13 13:24:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authentication/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      514 2022-09-14 07:26:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authentication/acs_service_principal_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authpolicy/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-15 09:23:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authpolicy/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authpolicy/events/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-15 09:23:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authpolicy/events/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      206 2022-09-15 09:25:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/authpolicy/events/auth_event.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1275 2022-07-28 11:42:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/base_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      289 2022-10-10 20:40:38.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/base_entity_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/businessdata/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:39:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/businessdata/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      954 2023-03-03 16:59:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/businessdata/app_bdc_catalog.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.471856 Office365-REST-Python-Client-2.4.1/office365/sharepoint/campaigns/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-26 07:19:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/campaigns/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      699 2022-09-26 13:49:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/campaigns/campaigns.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-09-26 07:21:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/campaigns/communication_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      101 2022-09-26 13:48:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/campaigns/entity.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.475857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      301 2022-06-06 09:54:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/alert.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      999 2022-06-06 09:47:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/change.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1871 2022-09-26 07:02:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2022-06-06 09:49:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/content_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/field.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      453 2022-06-06 14:16:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      351 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/folder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      404 2022-06-07 14:38:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      817 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/list.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1401 2022-06-06 10:07:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/log_item_query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3672 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      460 2022-12-23 16:57:39.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/token.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3051 2023-02-22 09:09:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      172 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/user.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/web.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    21916 2023-03-20 18:23:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/client_context.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.475857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      336 2023-03-05 09:07:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/component_context_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.475857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/hostedapps/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-01 11:39:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/hostedapps/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      224 2022-10-28 09:08:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/hostedapps/add_response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-10-28 09:13:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/hostedapps/app.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      627 2022-12-20 16:31:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/hostedapps/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      408 2022-09-15 08:26:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/identifier.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      613 2022-12-20 21:43:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/query_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2022-06-09 18:58:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/storage_entity.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.475857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.475857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/client/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-01 11:45:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/client/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      196 2022-10-01 11:49:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/client/identity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      719 2022-10-01 11:38:20.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1653 2022-10-01 11:38:20.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/comment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      583 2022-10-01 11:49:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/information.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-24 08:08:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-10-11 18:23:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/dlp_classification_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2022-10-11 18:23:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/pending_review_items_statistics.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1646 2022-12-06 22:22:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/store_proxy.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      542 2022-12-17 10:46:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/tag.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      208 2022-06-24 08:10:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/tag_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:00:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:02:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      229 2022-12-17 10:59:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/enabled.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4034 2022-12-17 11:08:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/hub.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/models/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 10:59:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/models/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      755 2022-12-17 11:00:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/models/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      245 2022-09-22 06:23:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/models/entity_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      225 2022-10-29 11:31:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/models/model.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/publications/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 11:16:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/publications/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      237 2022-12-06 09:08:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/publications/publication.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 11:00:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      763 2022-12-17 11:08:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      540 2022-10-29 11:30:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/entity_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      196 2022-12-10 14:42:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/meta.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      229 2022-12-17 11:08:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/sample.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.479857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/workitems/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-17 11:15:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/workitems/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      419 2022-12-17 11:16:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/workitems/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2022-10-05 19:11:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/workitems/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-12-17 10:35:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/syntex_models_landing_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.483857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4660 2022-12-19 12:59:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6973 2022-12-19 19:27:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/content_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      907 2022-06-18 10:00:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/content_type_id.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      843 2023-01-04 21:16:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      432 2022-12-19 12:31:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/entity_data.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.483857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/fieldlinks/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-10 20:22:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/fieldlinks/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2755 2022-12-19 14:32:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/fieldlinks/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1184 2022-12-19 13:16:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/fieldlinks/field_link.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.483857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/customactions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/customactions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1463 2022-10-08 08:38:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/customactions/action.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      434 2022-09-09 17:31:20.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/customactions/element.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      490 2022-09-09 17:30:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/customactions/element_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1284 2023-02-15 10:18:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      419 2022-05-31 14:57:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/group_and_user_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5247 2023-02-15 10:18:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/helper.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      164 2023-02-15 10:15:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/link.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2021-12-06 18:17:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/members_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      188 2023-01-12 22:20:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/membership_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      184 2023-01-12 22:27:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/my_groups_result.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/provider/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:41:02.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/provider/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      546 2023-03-01 17:36:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/provider/provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      942 2022-10-08 11:09:28.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/session.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1048 2023-02-15 10:18:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/documentmanagement/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/documentmanagement/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2175 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/documentmanagement/document_id.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2234 2022-08-18 16:13:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/documentmanagement/document_set.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/esign/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-11 13:13:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/esign/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/esign/models/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-11 13:13:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/esign/models/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      822 2023-03-11 13:05:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      907 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1284 2023-03-11 13:08:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/definition_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/excel/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/excel/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      613 2021-11-18 20:10:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/excel/excel_rest.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.487857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2319 2022-12-10 12:49:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.491857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/definitions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-20 14:55:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/definitions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1081 2022-11-20 15:04:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/definitions/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      343 2022-10-13 06:43:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/definitions/definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      265 2022-06-18 20:25:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/definitions/scope.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      538 2022-06-18 20:21:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/feature.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-12-07 20:38:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/known_list.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.495857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1073 2022-06-12 18:10:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/add_field_options.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      946 2022-12-11 20:56:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/calculated.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      125 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/choice.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7185 2022-07-15 15:43:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      435 2022-02-15 20:37:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/computed.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1666 2022-06-12 18:15:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      745 2022-06-12 18:15:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/currency.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      674 2022-06-14 09:20:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/date_time.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-06-14 09:17:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/date_time_format.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2022-06-18 09:23:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/datetime_field_format_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    10458 2022-10-08 08:53:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/field.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      310 2022-02-04 11:01:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/geolocation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      822 2022-02-04 11:41:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/geolocation_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      162 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/guid.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      533 2022-09-15 13:30:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/image_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1570 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/lookup.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      734 2022-08-08 09:53:28.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/lookup_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1001 2022-06-24 20:05:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_choice.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      342 2022-08-08 14:01:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_choice_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1127 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_line_text.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      295 2022-06-12 18:13:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_lookup_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      387 2022-06-14 09:10:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_user_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1424 2022-06-14 08:51:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/number.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      920 2022-06-14 09:10:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/rating_scale.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2081 2022-06-14 13:56:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/related_field.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      682 2022-06-14 13:56:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/related_field_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      294 2022-12-19 09:41:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/string_values.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      581 2022-02-15 20:51:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/text.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       92 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/thumbnail.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2782 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      363 2022-06-24 20:00:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/url.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2022-06-12 18:16:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/urlFieldFormatType.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      740 2022-06-12 18:22:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/url_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1566 2022-06-26 09:33:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/user.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      727 2022-06-12 18:13:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/user_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      644 2022-07-14 09:14:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/xmlSchemaFieldCreationInformation.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.495857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1844 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/checked_out_file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      852 2022-07-10 13:17:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/checked_out_file_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3469 2022-10-28 12:33:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1088 2022-10-19 10:43:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    28999 2023-03-11 13:12:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2022-06-11 10:36:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/move_operations.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      927 2022-10-01 12:45:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/recent_file_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      533 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/system_object_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3504 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/version.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2592 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/version_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1100 2022-12-16 13:25:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/version_event.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.499857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fileservices/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-02 20:05:02.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/fileservices/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.499857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/flows/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-25 18:45:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/flows/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2021-08-25 18:46:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/flows/synchronization_result.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.499857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3060 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      454 2022-06-03 14:09:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/delete_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-10-02 09:29:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/download_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    16094 2022-11-19 10:26:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/folder.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.499857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/forms/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/forms/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1429 2022-02-04 10:57:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/forms/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      825 2022-06-24 10:38:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/forms/form.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.499857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      941 2022-12-25 10:58:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/key_value.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.499857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/paths/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-02-17 21:42:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/paths/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      246 2022-08-09 09:25:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/paths/entity.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.503857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-11-23 14:55:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      734 2022-10-28 07:17:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/create_file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      924 2022-06-21 07:12:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/download_file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      632 2022-06-21 07:18:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/upload_file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3149 2023-03-07 16:47:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/upload_session.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.503857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/largeoperation/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-02 20:01:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/largeoperation/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.503857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/likes/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/likes/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1534 2022-06-28 17:24:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/likes/liked_by_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      502 2022-09-15 08:23:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/likes/user_entity.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.503857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listhome/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-05 20:03:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listhome/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      172 2022-12-05 20:02:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listhome/favorite_lists.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      197 2022-12-05 20:07:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listhome/item.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.503857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.503857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/caml/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/caml/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4284 2023-03-09 20:29:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/caml/query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1274 2022-10-12 11:29:39.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      386 2023-03-09 20:20:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/collection_position.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      596 2022-06-19 07:46:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/compliance_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1007 2022-06-19 07:46:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      987 2022-06-19 11:57:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/creation_information_using_path.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      267 2022-12-19 09:22:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/delete_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1416 2022-06-12 18:13:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/form_update_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       94 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/hashtag.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      208 2022-11-10 19:21:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/listdata_validation_exception_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    23057 2022-12-19 09:43:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/listitem.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      111 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/update_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/user_info_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2585 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/version.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.507857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      631 2022-02-04 10:31:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/base_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      663 2022-10-13 16:37:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/bloom_filter.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3086 2022-09-25 11:58:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      342 2023-03-09 10:45:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/collection_position.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      813 2022-06-19 09:48:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/creatable_item_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2253 2022-06-19 09:46:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/creatables_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      802 2022-06-19 09:56:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      944 2022-11-25 18:14:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/currency.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      845 2022-11-25 18:12:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/currency_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      449 2022-11-25 18:06:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/currency_information_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      190 2022-06-19 19:43:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/data_source.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      822 2023-03-16 07:13:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/document_library_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      239 2022-06-19 09:53:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/document_template_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      493 2023-03-09 10:32:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/get_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    35513 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/list.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      601 2022-10-13 06:33:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/render_data_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      302 2022-10-13 06:34:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/render_override_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       97 2021-09-11 20:16:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/rule.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1825 2023-03-01 20:17:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/template.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      763 2022-07-14 08:03:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/template_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1623 2022-06-19 10:03:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/template_type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.507857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/logger/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/logger/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/logger/logFileInfo.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      337 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/logger/logFileInfoCollection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1222 2022-09-22 06:44:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/logger/log_export.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-06 10:33:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      815 2022-09-14 14:12:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/app_metadata.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      797 2022-09-14 14:18:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/app_metadata_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:48:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:53:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1162 2022-09-14 14:17:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/accessor.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      188 2022-07-04 09:53:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/allowed_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      513 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/allowed_items.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/tenant/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:48:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/tenant/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/tenant/appcatalog/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:53:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/tenant/appcatalog/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1745 2022-07-04 09:56:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/tenant/appcatalog/accessor.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      318 2022-07-10 10:48:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/attachment_store.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      182 2022-07-06 07:17:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2022-06-03 14:04:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      294 2022-07-10 10:50:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-06-03 14:04:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microfeed/post_definition.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microservice/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microservice/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1038 2023-03-20 14:09:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/microservice/manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-07 12:03:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-31 16:20:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/results/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-02 14:13:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/results/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      108 2023-03-02 14:15:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/results/batch_creation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      275 2022-10-31 16:24:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/task.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-10-31 16:26:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/task_definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-10-31 16:23:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/common/task_entity_data.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/service/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-31 16:19:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/migrationcenter/service/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.511857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/multigeo/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-07 12:04:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/multigeo/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      212 2022-12-16 10:50:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/multigeo/unified_group.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.515857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2023-02-15 20:51:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/configured_metadata_items.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      572 2022-11-27 12:05:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/home_site_navigation_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      611 2022-07-14 09:20:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/menu_node.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1784 2022-06-07 12:10:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/menu_state.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1176 2023-02-15 20:50:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/metadata_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1995 2022-05-31 14:55:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/navigation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5888 2022-12-05 15:01:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/navigation_service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3077 2022-10-08 11:18:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/node.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2606 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/node_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1386 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/node_creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1482 2022-06-07 10:59:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/provider_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      171 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/publishing_navigation_provider_type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.515857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/oauth/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-24 10:18:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/oauth/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      186 2022-09-24 12:20:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/oauth/authentication.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      746 2022-06-24 10:24:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/oauth/native_client.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.515857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/orgnewssite/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-06 09:28:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/orgnewssite/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      956 2022-12-06 10:00:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/orgnewssite/api.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      206 2022-12-06 10:00:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/orgnewssite/info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.515857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/packaging/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-30 21:01:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/packaging/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      194 2022-11-30 21:06:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/packaging/app_details.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.515857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pageinstrumentation/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-24 10:25:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pageinstrumentation/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      191 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pageinstrumentation/click_manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.515857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      301 2022-06-13 17:52:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/customized_page_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1147 2022-02-15 20:35:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/page_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      479 2022-02-04 10:28:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/template_file_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      650 2021-10-26 21:43:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/wiki_page_creation_information.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1936 2022-07-10 13:08:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/base_permissions.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/irm/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:54:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/irm/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2022-07-10 13:08:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/irm/effective_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      463 2022-10-01 18:37:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/irm/file_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      887 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/irm/settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1028 2022-12-19 21:19:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/kind.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:57:55.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/assignments/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:52:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/assignments/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2021 2022-12-19 20:18:39.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/assignments/assignment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2712 2022-07-10 13:11:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/assignments/collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 12:50:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3400 2022-12-19 20:43:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      926 2022-12-19 20:43:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2526 2022-12-19 20:50:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7710 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/securable_object.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      212 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/utility.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/policy/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-12-25 11:10:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/policy/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1683 2022-12-19 10:20:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/policy/dlp_policy_tip.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2022-07-10 13:26:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/policy/evaluation_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.519857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/channels/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-22 21:59:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/channels/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2022-12-22 22:01:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/channels/info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      455 2022-12-23 16:49:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/channels/info_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-11-26 13:30:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/collaboration_mailbox.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-10-01 12:32:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/community_moderation.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:12:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-09-08 18:15:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/creation_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      623 2022-09-08 18:16:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      595 2022-09-08 18:16:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/creation_params.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1499 2022-07-11 11:19:02.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      465 2022-07-11 10:15:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/site_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6936 2022-12-24 10:08:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/site_manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/home/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-11 15:39:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/home/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-11-28 19:02:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/home/page_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      342 2022-09-20 06:28:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/home/service_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      642 2022-11-28 18:57:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/home/service_context_builder.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1063 2022-10-31 14:18:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/hub_sites_utility.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-29 16:23:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      207 2022-10-29 16:25:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/contract.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      521 2022-10-29 16:27:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/list_contract.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      839 2022-10-29 16:43:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2687 2022-09-20 06:42:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/mysite_recommendations.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      710 2022-12-06 10:47:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/organization_news.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/orglabels/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-29 15:58:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/orglabels/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      203 2022-10-29 16:03:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/orglabels/context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      529 2022-10-29 16:03:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/orglabels/context_list.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      830 2022-11-27 18:46:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/rating_settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 18:23:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      976 2022-11-27 13:22:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/creation_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      381 2022-11-26 13:27:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/creation_response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1543 2022-06-18 19:56:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/icon_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4645 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      388 2022-02-21 14:37:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      195 2022-10-01 12:33:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/suite_nav_data.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.523857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/teams/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-29 16:19:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/teams/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-12-22 22:03:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/teams/recent_and_joined_response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1202 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/theme_manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/userprofiles/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-30 14:07:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/userprofiles/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      232 2022-11-01 18:39:38.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/userprofiles/documents_shared_with_group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-10-30 14:11:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/userprofiles/documents_shared_with_me.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/webcontrols/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-20 06:28:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/webcontrols/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-20 15:20:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3435 2022-12-20 15:35:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      369 2022-12-20 15:39:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3128 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2162 2022-11-29 21:51:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/principal.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      515 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/source.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      216 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-20 15:20:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2454 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      539 2022-10-06 07:39:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/id_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3468 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      244 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/client_side_page.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.527857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-10-25 14:25:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1086 2022-10-29 12:08:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/controller.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       98 2022-02-19 16:37:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/page_details.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      499 2022-12-03 11:20:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/page_diagnostics.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      229 2022-12-03 11:20:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/page_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      697 2022-09-13 07:03:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/embed_data_v1.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      900 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/embed_service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      525 2022-12-03 11:28:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/file_picker_options.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.531857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/navigation/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/navigation/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.531857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 08:00:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      201 2022-12-03 12:15:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/campaign_publication.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3270 2022-12-03 10:52:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1203 2021-10-28 06:42:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/fields_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4507 2022-10-06 19:11:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/metadata.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      631 2022-12-03 10:47:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/metadata_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8929 2022-12-03 18:06:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/page.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      284 2022-12-03 18:06:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/page_3d.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      517 2022-07-29 10:06:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/repost.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     7985 2023-03-20 14:08:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      287 2022-07-29 08:11:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/topic.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      341 2022-07-29 08:11:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/topic_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      139 2022-07-29 08:11:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/topic_fields_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      262 2022-07-29 08:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/version_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.531857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/personmagazine/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-13 07:05:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/personmagazine/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      101 2022-09-13 07:06:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/personmagazine/person_magazine.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      215 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/portal_health_status.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.531857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/portallaunch/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-22 11:25:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/portallaunch/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      202 2022-11-22 11:27:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/portallaunch/wave.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      194 2022-11-22 11:28:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/portallaunch/waves_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      597 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/primary_city_time.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1910 2022-09-20 07:00:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/rich_sharing.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      169 2022-10-29 15:18:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/search.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.531857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 07:39:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.531857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 07:41:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1058 2022-11-26 12:39:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/creation_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      239 2022-07-29 07:41:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/creation_response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3468 2022-11-27 13:29:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/site.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      277 2022-07-29 09:40:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/user_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.535857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-29 08:05:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      550 2022-10-29 15:16:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/channel.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      347 2022-07-29 08:06:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/channel_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1204 2022-10-29 15:10:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      332 2022-07-29 08:06:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/item_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      471 2022-10-29 15:29:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/service_discoverer.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      803 2022-07-29 08:06:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/service_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      173 2022-10-29 15:06:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/view_data.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.535857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pushnotifications/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-02 14:39:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pushnotifications/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      825 2022-12-07 20:09:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pushnotifications/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1215 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/pushnotifications/subscriber.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.535857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/quotamanagement/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-01-08 09:38:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/quotamanagement/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.535857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2536 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2977 2022-10-01 19:43:39.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/item_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1236 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/query_information.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.535857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/reputationmodel/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/reputationmodel/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2943 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/reputationmodel/reputation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-11-28 20:57:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      832 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/request_context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      836 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/request_user_context.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.539857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.539857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1977 2022-11-24 18:00:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/document_crawl_log.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      259 2022-11-30 21:01:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/site_content_processing_info_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      646 2022-11-24 18:09:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/site_me_ta_info_provider.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1173 2023-01-03 14:37:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/tenant_crawl_versions_info_provider.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.539857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/analytics/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-05-29 08:42:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/analytics/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      324 2022-10-07 17:50:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/analytics/action.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-11 08:13:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/analytics/actor.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-10-07 17:53:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/analytics/signal.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      591 2023-03-11 12:43:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/analytics/signal_store.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      718 2022-12-21 15:20:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/context_condition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1188 2022-11-23 19:58:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/custom_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      493 2022-12-21 20:09:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/endpoints.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      803 2022-12-21 15:32:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/object_owner_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1136 2022-12-21 15:24:54.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/promoted_result_query_rule.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1101 2022-12-21 15:27:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/promoted_results_operations_result.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.543857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1058 2022-12-01 21:19:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/auto_completion.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      406 2022-12-22 21:58:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/auto_completion_match.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1251 2022-07-14 19:16:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/auto_completion_results.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      277 2022-11-27 17:32:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/condition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1506 2022-12-21 20:06:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      664 2022-12-21 20:17:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/context.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      305 2022-12-21 19:57:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/expanded_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      964 2022-07-14 17:27:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/personal_result_suggestion.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      627 2022-11-24 17:51:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/personalization_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      220 2022-12-21 20:37:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/popular_tenant_query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      784 2022-11-23 18:59:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/property.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      354 2022-11-23 18:53:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/property_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      343 2022-11-27 18:05:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/reordering_rule.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      602 2022-12-21 20:13:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/routing_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.543857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/sort/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-07 17:29:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/sort/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2267 2022-10-07 17:48:20.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/sort/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      882 2023-01-08 16:39:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/sort/sort.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1337 2023-01-08 15:38:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/suggestion_results.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-10-06 19:48:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/tenant_custom_query_suggestions.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2058 2022-12-24 10:18:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1913 2022-12-21 19:47:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/ranking_labeling.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1720 2022-12-24 10:18:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/refinement_results.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.543857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/refiner/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-06 19:39:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/refiner/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      464 2022-12-24 10:22:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/refiner/entry.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      269 2022-11-24 18:11:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/refiner/refiner.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2907 2022-12-24 11:30:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/relevant_results.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      304 2022-12-21 19:50:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/reordering_rule_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.543857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/reports/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-05-29 09:26:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/reports/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      338 2022-05-29 09:40:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/reports/abandoned_queries.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      268 2023-03-11 13:22:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/reports/base.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      219 2022-11-23 19:36:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/reports/top_queries.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6857 2022-11-27 18:05:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3019 2023-04-22 07:46:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    13118 2023-01-08 16:48:02.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4633 2023-01-08 09:51:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/setting.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      471 2022-12-24 11:24:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/simple_data_row.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      548 2022-12-24 11:40:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/simple_data_table.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-12-24 11:37:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/special_term_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      572 2022-12-24 11:40:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/special_term_results.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2203 2023-04-04 09:29:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/server_settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.547857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      371 2022-12-07 13:49:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/abilities.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      661 2022-12-11 12:01:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/ability_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      428 2022-11-24 19:38:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/access_request_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6916 2022-11-08 21:07:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/document_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      332 2022-06-13 08:08:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/external_site_option.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2433 2022-12-07 13:51:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-11-24 19:38:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/information_request.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.547857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/invitation/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-18 16:00:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/invitation/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      451 2022-11-24 19:15:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/invitation/creation_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1021 2022-11-24 18:49:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/invitation/link.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1001 2022-12-11 16:15:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/link_abilities.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.551857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-18 16:04:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1356 2022-10-18 16:12:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/access_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2022-01-24 09:43:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      280 2022-11-24 19:20:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/default_template.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      409 2022-11-24 19:24:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/default_templates_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2351 2022-11-24 20:54:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      854 2022-06-01 12:09:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/kind.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2640 2022-06-26 09:35:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/share_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      488 2022-10-18 16:42:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/share_response.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      651 2022-06-01 12:31:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/share_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9254 2022-10-18 16:05:39.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/object_sharing_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1320 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/object_sharing_information_user.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3577 2022-10-18 16:04:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/object_sharing_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1693 2022-06-26 09:35:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/operation_status_code.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1530 2022-12-11 20:53:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/permission_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1053 2022-12-11 21:03:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/personal_web.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1067 2022-11-08 19:42:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/picker_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      247 2022-11-24 18:46:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/principal.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3826 2022-12-20 15:21:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3534 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/role_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      997 2022-12-07 14:02:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/securable_object_extensions.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      190 2022-11-09 20:09:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/shared_document_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      117 2022-02-03 10:15:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/shared_object_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      198 2022-06-26 09:35:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/shared_with_user.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1051 2022-10-01 18:58:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/sharepoint_sharing_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1424 2022-11-09 20:21:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/site_sharing_report_helper.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      110 2022-11-09 20:21:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/site_sharing_report_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      881 2022-09-26 06:32:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/user_directory_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      627 2022-11-08 20:48:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/user_role_assignment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1027 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/user_sharing_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2145 2023-03-10 18:01:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/utility.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2022-12-11 21:07:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/web_sharing_manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.551857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1396 2022-06-04 08:51:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/creation_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/design_package_menu_contents.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      406 2022-06-04 08:28:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/metadata.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      234 2023-01-05 10:37:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/principal.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      324 2023-01-05 10:37:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/run.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      224 2023-01-05 10:26:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/task.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.551857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitehealth/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 09:56:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitehealth/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      262 2022-09-14 14:05:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitehealth/result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      689 2022-07-04 20:04:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitehealth/summary.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.555857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      125 2022-11-22 15:43:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/azure_container_Info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2022-11-26 15:01:20.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/home_site_reference.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      612 2023-03-05 10:22:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/home_sites_details.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       95 2021-08-25 20:26:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/language.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      800 2022-07-06 09:00:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/language_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    24902 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/site.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      118 2022-02-22 07:45:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/site_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4590 2022-12-06 09:18:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/sph_site.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      101 2023-03-10 18:04:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/team_site_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      155 2022-10-08 08:23:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/upgrade_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      966 2021-09-03 10:18:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/usage_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.555857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-03 12:53:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      450 2023-01-05 10:38:55.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/action_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2023-01-05 17:34:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/action_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      109 2023-01-05 10:39:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/creation_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      339 2022-06-03 16:14:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/metadata.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1123 2023-01-05 17:34:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/serialization_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      383 2023-01-05 17:34:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/serialization_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      274 2023-01-05 10:40:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/update_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11973 2023-02-17 07:31:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/utility.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.559857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      236 2022-07-04 13:45:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/actor.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      554 2022-07-04 13:44:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/actor_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1336 2022-12-07 07:53:28.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/announcement_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      290 2022-07-10 09:47:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/attachment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      222 2022-07-04 13:46:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/attachment_action.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      450 2022-07-09 09:17:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/data_overlay.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.559857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 10:09:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2606 2022-09-08 12:00:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/feed.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5091 2023-03-20 18:24:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      783 2022-09-08 12:05:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/rest.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      976 2022-07-04 14:16:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/rest_manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.559857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/following/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 10:11:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/following/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1540 2022-07-10 10:25:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/following/manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1597 2022-07-09 12:35:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/following/rest_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      329 2022-07-10 09:56:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/link.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.559857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/microfeed/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-08 12:10:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/microfeed/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2022-09-08 12:11:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/microfeed/thread.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2022-09-08 12:12:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/microfeed/thread_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      105 2022-09-08 12:13:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/microfeed/user_posts.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.559857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-10 10:03:02.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      403 2022-07-10 10:00:39.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/actor_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1720 2022-07-09 12:42:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/creation_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      272 2022-07-10 10:07:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/definition_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      316 2022-07-10 10:08:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/definition_data_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1468 2022-07-10 10:03:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/post.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1462 2023-03-20 18:27:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/reference.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      774 2022-07-04 14:05:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/rest_actor.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2119 2022-07-09 12:02:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/rest_thread.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1325 2022-07-10 08:54:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/switch.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1723 2022-12-07 13:38:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/thread.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.559857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/storagemetrics/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/storagemetrics/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1433 2022-06-24 19:57:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/storagemetrics/storage_metrics.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.563857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.563857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/contenttypesync/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 13:38:35.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/contenttypesync/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6480 2022-07-15 12:52:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/create_xml_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3202 2022-07-15 13:23:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/field.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1415 2022-06-16 20:09:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/field_value.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      833 2022-07-14 12:38:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1743 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      911 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/item_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      318 2022-07-15 12:34:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/metadata.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1103 2022-11-13 13:20:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      645 2022-07-14 12:38:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/set.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1871 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/store.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      171 2022-07-14 12:24:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/term.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.563857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/teams/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-12-27 14:02:27.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/teams/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      377 2023-03-11 07:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/teams/channel.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3071 2022-11-25 20:24:28.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/teams/channel_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      371 2022-12-22 22:15:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/teams/site_owner_response.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.563857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.567857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.567857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/audit/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-13 06:44:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/audit/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      209 2022-10-13 06:45:55.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/audit/data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      227 2022-10-13 06:49:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/audit/unified_record.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.567857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/collaboration/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-12 10:33:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/collaboration/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      829 2022-11-22 11:13:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/collaboration/insights_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      172 2022-09-19 20:18:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/deny_add_and_customize_pages_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      409 2022-07-05 08:03:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/endpoints.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.571857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-13 07:24:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1588 2022-10-01 18:33:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1350 2022-06-18 08:50:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/hub_site.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-10-09 18:58:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/permission.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      707 2022-10-09 19:05:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/properties.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.571857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/insights/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-25 18:49:49.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/insights/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      116 2022-11-25 18:57:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/insights/onedrive_site_sharing.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      238 2022-10-07 18:13:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/insights/top_files_sharing.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.571857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-09-22 06:42:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/internal/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      903 2023-03-05 09:04:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/internal/web_appservice_principal.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      514 2022-11-26 09:55:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/response_message_center.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      234 2022-11-10 18:22:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/response_service_health.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      762 2022-06-04 19:54:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/secondary_administrators_fields_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      474 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/secondary_administrators_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1781 2022-12-10 18:52:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/settings_service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      618 2022-02-19 17:21:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/sharing_capabilities.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      495 2022-10-08 14:13:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_administrators_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1195 2022-11-26 10:14:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_collection_management_service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      384 2022-11-26 10:19:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_creation_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      254 2022-10-07 18:09:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_creation_default_storage_quota.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      933 2022-07-05 15:18:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_creation_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      537 2022-11-26 10:19:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_creation_source.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4381 2022-10-09 13:47:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1986 2022-12-10 18:51:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_properties_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      951 2022-12-10 18:36:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_properties_enumerable_filter.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      230 2022-12-10 18:44:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_state_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2022-12-10 18:43:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_user_group_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      309 2022-11-26 11:12:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/siteinfo_for_site_picker.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      292 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/smtp_server.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      675 2022-07-04 20:25:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/spo_operation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    18839 2023-03-05 09:45:58.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/tenant.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      218 2022-10-12 10:43:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/theme_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      304 2022-06-23 22:29:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/web_template.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      161 2022-10-08 08:21:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/app_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      175 2022-10-08 08:17:34.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/app_instance.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2023-03-02 19:07:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/app_utility.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      408 2022-09-25 07:24:40.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/cdn_api.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      198 2022-09-25 09:56:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/cdn_url.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.571857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-03 06:29:36.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.571857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-10 19:04:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      671 2022-12-11 11:53:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      212 2022-12-11 16:15:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/external_user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.571857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/results/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-12-11 11:46:23.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/results/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      853 2022-12-11 16:15:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/results/get.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      240 2022-12-11 11:53:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/results/remove.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      250 2022-12-11 11:53:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/results/session_revocation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    11605 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/office365_tenant.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1252 2022-07-04 10:34:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.575857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-08 08:01:20.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      717 2022-09-28 07:12:08.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/item_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1618 2023-03-01 20:07:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/job.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      299 2022-09-28 07:13:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/job_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      491 2022-07-05 07:58:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/job_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      622 2022-09-27 13:32:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/notification_recipient.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      551 2022-09-27 13:32:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/notification_recipient_set_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      565 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/notification_recipient_users.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2022-09-09 18:02:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/requested_translation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      193 2022-12-19 20:00:32.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/resource_entry.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2022-06-24 10:44:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1328 2022-09-28 07:04:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/status_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      348 2022-06-24 10:55:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/status_creation_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      470 2022-09-09 18:10:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/status_set_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2722 2022-09-28 18:26:33.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/sync_translator.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1988 2022-12-19 19:55:43.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/user_resource.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1535 2022-09-28 07:28:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/variations_timer_job.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.575857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/types/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/types/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2022-12-06 22:01:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/types/property_values.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      596 2022-06-16 18:42:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/types/resource_path.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       87 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/types/wopi_action.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.575857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.575857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.575857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-24 17:05:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      178 2022-07-24 17:07:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/entity_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      899 2022-07-24 17:39:25.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/entity_information_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3168 2022-12-20 15:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/query_parameters.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      768 2022-11-27 14:18:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/query_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6091 2023-03-20 14:21:13.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/web_service_interface.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.579857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/usercustomactions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/usercustomactions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1638 2021-09-13 07:33:07.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/usercustomactions/action.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      925 2022-06-18 19:56:52.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/usercustomactions/collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.579857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      678 2023-01-04 21:05:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/follow_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1637 2023-01-04 21:18:47.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/followed_content.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      416 2023-01-04 21:16:03.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/followed_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1021 2022-10-11 06:16:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/hash_tag.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1737 2022-09-20 17:31:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/my_site_links.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    12318 2023-03-20 14:06:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/people_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     3123 2022-12-25 10:07:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/person_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1035 2022-11-01 07:25:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/personal_cache.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      299 2022-10-11 06:19:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/personal_cache_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      367 2022-06-07 18:48:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/personal_site_creation_priority.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2081 2022-10-11 06:39:48.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/profile_image_store.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1863 2023-03-20 14:05:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/profile_loader.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2643 2022-11-01 19:00:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/promoted_sites.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1576 2022-09-08 11:42:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/properties_for_user.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.579857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-11 15:32:50.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1201 2022-09-20 17:27:57.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/document.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      312 2022-09-20 07:10:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/document_user.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      104 2022-07-11 15:38:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/items.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      339 2022-07-11 15:37:38.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/view_item_removal_result.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4855 2022-11-01 07:43:01.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/user_profile.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.583857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1353 2022-06-24 10:35:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/email_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      688 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/move_copy_options.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     4394 2022-07-20 18:16:10.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/move_copy_util.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      242 2022-06-12 07:49:00.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/principal_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      941 2022-06-13 14:02:15.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/upload_status.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     8868 2022-12-21 15:10:11.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/utility.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      251 2022-10-05 19:50:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/wopi_frame_action.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      146 2022-06-18 20:14:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/wopi_properties.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      107 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/wopi_web_app_properties.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.583857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1954 2022-12-19 09:54:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1747 2022-12-19 09:54:21.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/create_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2341 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/field_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      506 2022-11-22 21:17:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/scope.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      231 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     6255 2022-11-22 20:19:18.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/view.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      102 2022-10-06 19:01:12.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/visualization.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.583857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-10-01 08:39:30.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      103 2022-10-01 12:19:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/app_configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      416 2023-03-09 09:18:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/connections_url_configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1698 2023-03-09 09:12:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/employee_engagement.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      115 2023-03-02 20:07:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/employee_experience_controller.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      199 2023-03-09 09:07:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/home.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      226 2023-03-09 09:18:17.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/home_title_region.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      442 2023-03-09 09:06:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/site_request_info.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.587857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1816 2023-01-05 10:17:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/subscription.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2165 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/subscription_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1258 2021-10-19 09:23:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/subscription_information.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.587857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.587857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/client/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-04 10:50:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/client/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      736 2022-07-04 10:52:37.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/client/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      778 2022-12-25 09:51:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/client/webpart.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1604 2022-09-22 06:19:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      893 2022-09-22 06:14:45.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/definition_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1219 2022-07-04 10:59:06.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/limited_manager.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1242 2022-07-04 11:06:55.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/personalization_scope.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      166 2022-07-09 12:46:26.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/tile_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      332 2022-07-04 10:42:24.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/webpart.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.591857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      263 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/calendar_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1234 2023-04-02 12:11:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1187 2022-06-08 07:54:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/context_web_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      371 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      113 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/info_creation_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      144 2022-06-08 17:17:56.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      859 2022-07-09 08:55:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/information_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1227 2022-09-27 13:27:04.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/multilingual_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2723 2022-09-27 13:43:38.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/regional_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1421 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/remote_web.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      528 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/subweb_query.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      525 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/template.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      841 2022-07-09 08:55:05.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/template_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      901 2022-10-06 07:16:44.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/theme_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1783 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/time_zone.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      891 2022-06-02 19:55:53.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/time_zone_information.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)    86343 2023-03-28 10:43:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/web.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.591857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflow/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-02-17 07:31:42.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflow/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      194 2022-07-04 20:05:46.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflow/association.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      166 2022-07-04 20:08:22.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflow/template.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.591857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflowservices/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-11-02 20:44:14.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflowservices/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      237 2023-03-01 13:57:09.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflowservices/instance.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      886 2023-03-01 13:58:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflowservices/instance_service.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1325 2023-03-01 17:26:41.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workflowservices/manager.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.591857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workmanagement/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-01-27 20:49:19.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/workmanagement/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.591857 Office365-REST-Python-Client-2.4.1/office365/sharepoint/yammer/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/yammer/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       93 2021-09-03 05:55:31.000000 Office365-REST-Python-Client-2.4.1/office365/sharepoint/yammer/wac_api.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.591857 Office365-REST-Python-Client-2.4.1/office365/subscriptions/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-31 07:27:09.000000 Office365-REST-Python-Client-2.4.1/office365/subscriptions/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1990 2022-12-17 13:19:37.000000 Office365-REST-Python-Client-2.4.1/office365/subscriptions/change_notification.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1362 2022-12-17 13:07:18.000000 Office365-REST-Python-Client-2.4.1/office365/subscriptions/change_notification_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      187 2022-12-17 13:18:22.000000 Office365-REST-Python-Client-2.4.1/office365/subscriptions/encrypted_content.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      278 2022-12-17 13:10:45.000000 Office365-REST-Python-Client-2.4.1/office365/subscriptions/resource_data.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1005 2022-12-17 12:48:31.000000 Office365-REST-Python-Client-2.4.1/office365/subscriptions/subscription.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.595857 Office365-REST-Python-Client-2.4.1/office365/teams/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/teams/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.595857 Office365-REST-Python-Client-2.4.1/office365/teams/apps/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:02:23.000000 Office365-REST-Python-Client-2.4.1/office365/teams/apps/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      971 2022-07-02 08:02:36.000000 Office365-REST-Python-Client-2.4.1/office365/teams/apps/app.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1579 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/teams/apps/definition.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1386 2022-06-25 15:43:00.000000 Office365-REST-Python-Client-2.4.1/office365/teams/apps/installation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      722 2022-09-24 12:25:50.000000 Office365-REST-Python-Client-2.4.1/office365/teams/apps/user_scope_installation.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.595857 Office365-REST-Python-Client-2.4.1/office365/teams/bots/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-09-09 06:18:01.000000 Office365-REST-Python-Client-2.4.1/office365/teams/bots/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      126 2021-09-09 06:19:05.000000 Office365-REST-Python-Client-2.4.1/office365/teams/bots/teamwork_bot.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.595857 Office365-REST-Python-Client-2.4.1/office365/teams/channels/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:58:03.000000 Office365-REST-Python-Client-2.4.1/office365/teams/channels/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     5877 2022-11-29 21:43:59.000000 Office365-REST-Python-Client-2.4.1/office365/teams/channels/channel.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1452 2022-11-29 21:42:00.000000 Office365-REST-Python-Client-2.4.1/office365/teams/channels/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      351 2022-11-29 21:05:33.000000 Office365-REST-Python-Client-2.4.1/office365/teams/channels/membership_type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      180 2022-11-29 21:43:59.000000 Office365-REST-Python-Client-2.4.1/office365/teams/channels/provision_email_result.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.595857 Office365-REST-Python-Client-2.4.1/office365/teams/chats/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 18:46:30.000000 Office365-REST-Python-Client-2.4.1/office365/teams/chats/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2843 2023-03-16 06:56:50.000000 Office365-REST-Python-Client-2.4.1/office365/teams/chats/chat.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1115 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/teams/chats/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1449 2022-06-24 20:24:42.000000 Office365-REST-Python-Client-2.4.1/office365/teams/chats/message.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1119 2022-06-24 20:21:37.000000 Office365-REST-Python-Client-2.4.1/office365/teams/chats/message_attachment.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2158 2022-12-25 09:56:18.000000 Office365-REST-Python-Client-2.4.1/office365/teams/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      276 2021-07-11 21:05:59.000000 Office365-REST-Python-Client-2.4.1/office365/teams/fun_settings.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      576 2022-11-20 21:18:10.000000 Office365-REST-Python-Client-2.4.1/office365/teams/guest_settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.595857 Office365-REST-Python-Client-2.4.1/office365/teams/internal/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-04-09 17:22:26.000000 Office365-REST-Python-Client-2.4.1/office365/teams/internal/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.599857 Office365-REST-Python-Client-2.4.1/office365/teams/internal/paths/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-04-09 17:22:33.000000 Office365-REST-Python-Client-2.4.1/office365/teams/internal/paths/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      537 2022-06-26 09:33:00.000000 Office365-REST-Python-Client-2.4.1/office365/teams/member_settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.599857 Office365-REST-Python-Client-2.4.1/office365/teams/members/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-06-26 08:50:37.000000 Office365-REST-Python-Client-2.4.1/office365/teams/members/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      829 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.1/office365/teams/members/aad_user_conversation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      373 2022-07-10 12:59:31.000000 Office365-REST-Python-Client-2.4.1/office365/teams/members/conversation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      340 2022-07-31 16:08:16.000000 Office365-REST-Python-Client-2.4.1/office365/teams/members/conversation_collection.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.599857 Office365-REST-Python-Client-2.4.1/office365/teams/messages/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 15:58:53.000000 Office365-REST-Python-Client-2.4.1/office365/teams/messages/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1273 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/teams/messaging_settings.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.599857 Office365-REST-Python-Client-2.4.1/office365/teams/operations/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:01:17.000000 Office365-REST-Python-Client-2.4.1/office365/teams/operations/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1421 2022-11-29 21:14:51.000000 Office365-REST-Python-Client-2.4.1/office365/teams/operations/async_operation.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      403 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/teams/operations/async_operation_status.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.599857 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:12:57.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      195 2022-06-05 09:35:48.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/availability.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1073 2023-03-13 07:20:44.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/change_tracked_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      217 2021-12-21 19:35:41.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/offer_shift_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      145 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/open_shift_change_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      594 2022-06-05 09:44:02.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/preferences.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1708 2022-10-01 08:34:13.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/schedule.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      651 2022-06-18 19:56:51.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/schedule_change_request.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      112 2022-06-06 14:16:09.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/schedule_entity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      649 2023-04-07 13:36:43.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/scheduling_group.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1018 2023-03-16 12:45:56.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/shift.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      145 2023-03-11 15:39:20.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/shift_activity.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      776 2022-06-06 14:16:26.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/shift_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      130 2021-09-09 17:41:29.000000 Office365-REST-Python-Client-2.4.1/office365/teams/shifts/time_off_reason.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/office365/teams/tabs/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2021-08-06 16:00:53.000000 Office365-REST-Python-Client-2.4.1/office365/teams/tabs/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      384 2022-07-02 07:43:14.000000 Office365-REST-Python-Client-2.4.1/office365/teams/tabs/configuration.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1241 2022-07-02 07:55:46.000000 Office365-REST-Python-Client-2.4.1/office365/teams/tabs/tab.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     9805 2022-12-12 19:59:33.000000 Office365-REST-Python-Client-2.4.1/office365/teams/team.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      123 2022-07-17 13:59:29.000000 Office365-REST-Python-Client-2.4.1/office365/teams/team_info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      397 2021-07-27 14:53:28.000000 Office365-REST-Python-Client-2.4.1/office365/teams/template.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2574 2022-09-24 12:28:14.000000 Office365-REST-Python-Client-2.4.1/office365/teams/user_teamwork.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      142 2022-07-01 16:20:27.000000 Office365-REST-Python-Client-2.4.1/office365/teams/visibility_type.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/office365/todo/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2022-07-06 07:19:13.000000 Office365-REST-Python-Client-2.4.1/office365/todo/__init__.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-11 15:39:19.000000 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      334 2023-03-11 21:18:20.000000 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/base.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      368 2023-03-16 19:23:58.000000 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      146 2023-03-16 12:51:31.000000 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/info.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      516 2023-04-07 14:01:36.000000 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/task_file.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       33 2023-03-16 12:52:40.000000 Office365-REST-Python-Client-2.4.1/office365/todo/attachments/type.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      211 2022-07-08 08:20:03.000000 Office365-REST-Python-Client-2.4.1/office365/todo/checklist_item.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      595 2023-03-11 20:22:29.000000 Office365-REST-Python-Client-2.4.1/office365/todo/linked_resource.py
+drwxrwxr-x   0 vgrem     (1000) vgrem     (1000)        0 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/office365/todo/tasks/
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)        0 2023-03-11 20:18:49.000000 Office365-REST-Python-Client-2.4.1/office365/todo/tasks/__init__.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1083 2023-03-11 20:19:34.000000 Office365-REST-Python-Client-2.4.1/office365/todo/tasks/list.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      549 2023-03-11 20:19:34.000000 Office365-REST-Python-Client-2.4.1/office365/todo/tasks/list_collection.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     1894 2022-07-08 08:27:42.000000 Office365-REST-Python-Client-2.4.1/office365/todo/tasks/task.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)      501 2023-03-11 20:19:34.000000 Office365-REST-Python-Client-2.4.1/office365/todo/todo.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       36 2022-07-08 18:23:51.000000 Office365-REST-Python-Client-2.4.1/office365/todo/wellknown_list_name.py
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)       79 2023-04-22 08:23:37.603857 Office365-REST-Python-Client-2.4.1/setup.cfg
+-rw-rw-r--   0 vgrem     (1000) vgrem     (1000)     2071 2023-04-22 08:20:04.000000 Office365-REST-Python-Client-2.4.1/setup.py
```

### Comparing `Office365-REST-Python-Client-2.4.0/LICENSE` & `Office365-REST-Python-Client-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/PKG-INFO` & `Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Office365-REST-Python-Client
-Version: 2.4.0
+Version: 2.4.1
 Summary: Microsoft 365 & Microsoft Graph Library for Python
 Home-page: https://github.com/vgrem/Office365-REST-Python-Client
 Author: Vadim Gremyachev
 Author-email: vvgrem@gmail.com
 Maintainer: Konrad Gądek, Domenico Di Nicola
 Maintainer-email: kgadek@gmail.com, dom.dinicola@gmail.com
 License: MIT
@@ -157,22 +157,22 @@
 print("Web title: {0}".format(web_title))
 ```
 
 
 The list of examples:
 
 - Working with files
-  - [download a file](examples/sharepoint/files/download_file.py) 
-  - [upload a file](examples/sharepoint/files/upload_file.py)
+  - [download a file](examples/sharepoint/files/download.py) 
+  - [upload a file](examples/sharepoint/files/upload.py)
 
 - Working with lists and list items
   -  [create a list item](examples/sharepoint/lists/data_generator.py)
-  -  [read a list item](examples/sharepoint/lists/read_large_list.py)   
-  -  [update a list item](examples/sharepoint/listitems/update_items_batch.py)
-  -  [delete a list item](examples/sharepoint/listitems/delete_list_item.py) 
+  -  [read a list item](examples/sharepoint/lists/read_large.py)   
+  -  [update a list item](examples/sharepoint/listitems/update_batch.py)
+  -  [delete a list item](examples/sharepoint/listitems/delete.py) 
   
 Refer [examples section](examples/sharepoint) for another scenarios
 
 # Working with Outlook API
 
 The list of supported APIs:
 -   [Outlook Contacts REST API](https://msdn.microsoft.com/en-us/office/office365/api/contacts-rest-operations)
@@ -191,15 +191,15 @@
 
 [The Microsoft Authentication Library (MSAL) for Python](https://pypi.org/project/msal/) which comes as a dependency 
 is used as a default library to obtain tokens to call Microsoft Graph API. 
 
 Using [Microsoft Authentication Library (MSAL) for Python](https://pypi.org/project/msal/)
 
 > Note: access token is getting acquired via [Client Credential flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)
-> in the provided examples. Other forms of token aquisition can be found here: https://msal-python.readthedocs.io/en/latest/
+> in the provided examples. Other forms of token acquisition can be found here: https://msal-python.readthedocs.io/en/latest/
 
 ```python
 import msal
 from office365.graph_client import GraphClient
 
 def acquire_token():
     """
@@ -259,25 +259,25 @@
     subject="Meet for lunch?",
     body="The new cafeteria is open.",
     to_recipients=["fannyd@contoso.onmicrosoft.com"]
 ).execute_query()
 
 ```
 
-> How to enable sending emails on behalf of another user in your organization: https://learn.microsoft.com/en-us/microsoft-365/solutions/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide&viewFallbackFrom=o365-worldwide%3FWT.mc_id%3D365AdminCSH_globalsearch
 
-Additional examples:
+Additional examples & scenarios:
+
+-  [download a message](examples/outlook/messages/download.py) 
+-  [list messages](examples/outlook/messages/list_all.py)
+-  [move messages to a different folder](examples/outlook/messages/move.py)
+-  [search messages](examples/outlook/messages/search.py)   
+-  [send messages](examples/outlook/messages/send.py)
+-  [send messages with attachments](examples/outlook/messages/send_with_attachment.py) 
+-  [enable sending emails on behalf of another user in your organization](https://learn.microsoft.com/en-us/microsoft-365/solutions/allow-members-to-send-as-or-send-on-behalf-of-group)
 
--  [download a message](examples/outlook/download_messages.py) 
--  [list messages](examples/outlook/list_message.py)
--  [move messages to a different folder](examples/outlook/move_message.py)
--  [search messages](examples/outlook/search_message.py)   
--  [send messages](examples/outlook/send_message.py)
--  [send messages with attachments](examples/outlook/send_message_with_attachment.py) 
-  
 Refer to [examples section](examples/outlook) for other scenarios
 
 
 # Working with OneDrive API
 
 #### Documentation 
 
@@ -348,15 +348,15 @@
             # download file content
             with open(os.path.join(local_path, drive_item.name), 'wb') as local_file:
                 drive_item.download(local_file).execute_query()
 ```
 
 Additional examples:
 
--  [create list column](examples/onedrive/create_list_column.py) 
+-  [create list column](examples/onedrive/columns/create_text.py) 
 -  [download file](examples/onedrive/download_file_default.py)
 -  [export files](examples/onedrive/export_files.py)
 -  [import files](examples/onedrive/import_files.py)   
 -  [list drives](examples/onedrive/list_drives.py)
 -  [list files](examples/onedrive/list_files.py)
 
 Refer to [OneDrive examples section](examples/onedrive) for more examples.
@@ -381,16 +381,16 @@
 client = GraphClient(acquire_token_func)
 new_team = client.groups["{group_id}"].add_team().execute_query_retry()
 ```
 
 Additional examples:
 
 -  [create a team](examples/teams/create_team.py) 
--  [create team from group](examples/teams/create_team_from_group.py)
--  [list all teams](examples/teams/list_all_teams.py)
+-  [create team from group](examples/teams/create_from_group.py)
+-  [list all teams](examples/teams/list_all.py)
 -  [list my teams](examples/teams/list_my_teams.py)   
 -  [send messages](examples/teams/send_message.py)
   
 Refer to [examples section](examples/teams) for other scenarios
 
 # Working with Microsoft Onenote API
```

### Comparing `Office365-REST-Python-Client-2.4.0/Office365_REST_Python_Client.egg-info/SOURCES.txt` & `Office365-REST-Python-Client-2.4.1/Office365_REST_Python_Client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Office365_REST_Python_Client.egg-info/SOURCES.txt
 Office365_REST_Python_Client.egg-info/dependency_links.txt
 Office365_REST_Python_Client.egg-info/requires.txt
 Office365_REST_Python_Client.egg-info/top_level.txt
 office365/__init__.py
 office365/base_item.py
 office365/delta_collection.py
+office365/delta_path.py
 office365/entity.py
 office365/entity_collection.py
 office365/graph_client.py
 office365/graph_request.py
 office365/logger.py
 office365/communications/__init__.py
 office365/communications/cloud_communications.py
@@ -41,14 +42,15 @@
 office365/communications/operations/comms.py
 office365/communications/operations/invite_participants.py
 office365/communications/operations/start_hold_music.py
 office365/communications/operations/stop_hold_music.py
 office365/communications/presences/__init__.py
 office365/communications/presences/presence.py
 office365/directory/__init__.py
+office365/directory/administrative_unit.py
 office365/directory/directory.py
 office365/directory/key_credential.py
 office365/directory/object.py
 office365/directory/object_collection.py
 office365/directory/password_credential.py
 office365/directory/profile_photo.py
 office365/directory/applications/__init__.py
@@ -68,14 +70,15 @@
 office365/directory/audit/directory.py
 office365/directory/audit/log_root.py
 office365/directory/audit/provisioning/__init__.py
 office365/directory/audit/provisioning/action.py
 office365/directory/audit/provisioning/object_summary.py
 office365/directory/audit/provisioning/service_principal.py
 office365/directory/audit/signins/__init__.py
+office365/directory/audit/signins/location.py
 office365/directory/audit/signins/signin.py
 office365/directory/audit/signins/status.py
 office365/directory/authentication/__init__.py
 office365/directory/authentication/authentication.py
 office365/directory/authentication/basic.py
 office365/directory/authentication/client_certificate.py
 office365/directory/authentication/configuration_base.py
@@ -88,16 +91,18 @@
 office365/directory/certificates/__init__.py
 office365/directory/certificates/auth_configuration.py
 office365/directory/certificates/authority.py
 office365/directory/certificates/certification.py
 office365/directory/certificates/pkcs12_information.py
 office365/directory/certificates/self_signed.py
 office365/directory/domains/__init__.py
+office365/directory/domains/dns_cname_record.py
 office365/directory/domains/dns_record.py
 office365/directory/domains/domain.py
+office365/directory/domains/verified.py
 office365/directory/extensions/__init__.py
 office365/directory/extensions/extended_property.py
 office365/directory/extensions/extension.py
 office365/directory/extensions/extension_property.py
 office365/directory/groups/__init__.py
 office365/directory/groups/collection.py
 office365/directory/groups/group.py
@@ -105,17 +110,17 @@
 office365/directory/groups/profile.py
 office365/directory/groups/setting.py
 office365/directory/groups/setting_template.py
 office365/directory/identities/__init__.py
 office365/directory/identities/api_connector.py
 office365/directory/identities/conditional_access_root.py
 office365/directory/identities/container.py
-office365/directory/identities/identity.py
-office365/directory/identities/identity_set.py
+office365/directory/identities/governance.py
 office365/directory/identities/object_identity.py
+office365/directory/identities/protection_root.py
 office365/directory/identities/provider.py
 office365/directory/identities/provider_collection.py
 office365/directory/identities/providers/__init__.py
 office365/directory/identities/providers/base.py
 office365/directory/identities/providers/base_collection.py
 office365/directory/identities/providers/builtin_identity.py
 office365/directory/identities/providers/saml_or_wsfed.py
@@ -126,24 +131,30 @@
 office365/directory/identities/userflows/language_page.py
 office365/directory/identities/userflows/user_attribute_assignment.py
 office365/directory/identities/userflows/user_flow.py
 office365/directory/identities/userflows/b2x/__init__.py
 office365/directory/identities/userflows/b2x/user_flow.py
 office365/directory/insights/__init__.py
 office365/directory/insights/office_graph.py
+office365/directory/insights/shared.py
+office365/directory/insights/trending.py
+office365/directory/insights/used.py
 office365/directory/internal/__init__.py
 office365/directory/internal/paths/__init__.py
 office365/directory/internal/paths/me.py
 office365/directory/licenses/__init__.py
 office365/directory/licenses/assigned_license.py
 office365/directory/licenses/assigned_plan.py
+office365/directory/licenses/assignment_state.py
 office365/directory/licenses/details.py
 office365/directory/licenses/service_plan_info.py
 office365/directory/licenses/subscribed_sku.py
 office365/directory/permissions/__init__.py
+office365/directory/permissions/identity.py
+office365/directory/permissions/identity_set.py
 office365/directory/permissions/scope.py
 office365/directory/permissions/grants/__init__.py
 office365/directory/permissions/grants/condition_set.py
 office365/directory/permissions/grants/oauth2.py
 office365/directory/permissions/grants/resource_specific.py
 office365/directory/policies/__init__.py
 office365/directory/policies/authentication_methods.py
@@ -151,23 +162,27 @@
 office365/directory/policies/base.py
 office365/directory/policies/conditional_access.py
 office365/directory/policies/permission_grant.py
 office365/directory/policies/root.py
 office365/directory/policies/sts.py
 office365/directory/rbac/__init__.py
 office365/directory/rbac/application.py
+office365/directory/rbac/unified_role_assignment.py
 office365/directory/roles/__init__.py
 office365/directory/roles/management.py
 office365/directory/roles/role.py
 office365/directory/roles/template.py
 office365/directory/security/__init__.py
 office365/directory/security/security.py
 office365/directory/users/__init__.py
+office365/directory/users/activity.py
 office365/directory/users/collection.py
 office365/directory/users/identity.py
+office365/directory/users/invitation.py
+office365/directory/users/invited_user_message_info.py
 office365/directory/users/password_profile.py
 office365/directory/users/profile.py
 office365/directory/users/settings.py
 office365/directory/users/user.py
 office365/education/__init__.py
 office365/education/class.py
 office365/education/root.py
@@ -178,28 +193,35 @@
 office365/intune/__init__.py
 office365/intune/provisioned_plan.py
 office365/intune/audit/__init__.py
 office365/intune/audit/event.py
 office365/intune/devices/__init__.py
 office365/intune/devices/app_management.py
 office365/intune/devices/configuration.py
+office365/intune/devices/detail.py
 office365/intune/devices/device.py
+office365/intune/devices/managed.py
+office365/intune/devices/managed_app_diagnostic_status.py
+office365/intune/devices/managed_app_registration.py
+office365/intune/devices/managed_ebook.py
 office365/intune/devices/management.py
 office365/intune/organizations/__init__.py
+office365/intune/organizations/branding_properties.py
 office365/intune/organizations/contact.py
 office365/intune/organizations/organization.py
 office365/onedrive/__init__.py
 office365/onedrive/root.py
 office365/onedrive/sharepoint_ids.py
 office365/onedrive/analytics/__init__.py
 office365/onedrive/analytics/item_action_stat.py
 office365/onedrive/analytics/item_activity.py
 office365/onedrive/analytics/item_activity_stat.py
 office365/onedrive/analytics/item_analytics.py
 office365/onedrive/columns/__init__.py
+office365/onedrive/columns/boolean.py
 office365/onedrive/columns/calculated.py
 office365/onedrive/columns/choice.py
 office365/onedrive/columns/column_link.py
 office365/onedrive/columns/currency.py
 office365/onedrive/columns/default_value.py
 office365/onedrive/columns/definition.py
 office365/onedrive/columns/definition_collection.py
@@ -267,14 +289,16 @@
 office365/onedrive/listitems/list_item.py
 office365/onedrive/lists/__init__.py
 office365/onedrive/lists/collection.py
 office365/onedrive/lists/info.py
 office365/onedrive/lists/list.py
 office365/onedrive/permissions/__init__.py
 office365/onedrive/permissions/permission.py
+office365/onedrive/permissions/sharepoint_identity.py
+office365/onedrive/permissions/sharepoint_identity_set.py
 office365/onedrive/permissions/sharing_invitation.py
 office365/onedrive/permissions/sharing_link.py
 office365/onedrive/shares/__init__.py
 office365/onedrive/shares/collection.py
 office365/onedrive/shares/drive_item.py
 office365/onedrive/shares/shared.py
 office365/onedrive/sites/__init__.py
@@ -350,66 +374,76 @@
 office365/onenote/internal/__init__.py
 office365/onenote/internal/multipart_page_query.py
 office365/onenote/notebooks/__init__.py
 office365/onenote/notebooks/collection.py
 office365/onenote/notebooks/copy_notebook_model.py
 office365/onenote/notebooks/notebook.py
 office365/onenote/notebooks/recent.py
+office365/onenote/notebooks/recent_links.py
 office365/onenote/operations/__init__.py
 office365/onenote/operations/onenote.py
 office365/onenote/operations/onenote_operation_error.py
 office365/onenote/operations/operation.py
 office365/onenote/operations/operation_status.py
 office365/onenote/pages/__init__.py
+office365/onenote/pages/collection.py
+office365/onenote/pages/external_link.py
+office365/onenote/pages/links.py
 office365/onenote/pages/page.py
-office365/onenote/pages/page_collection.py
-office365/onenote/pages/page_links.py
+office365/onenote/pages/preview_links.py
 office365/onenote/resources/__init__.py
 office365/onenote/resources/resource.py
 office365/onenote/sectiongroups/__init__.py
 office365/onenote/sectiongroups/section_group.py
 office365/onenote/sections/__init__.py
 office365/onenote/sections/section.py
 office365/outlook/__init__.py
 office365/outlook/category.py
 office365/outlook/convert_id_result.py
 office365/outlook/item.py
 office365/outlook/locale_info.py
 office365/outlook/timezone_information.py
 office365/outlook/user.py
 office365/outlook/calendar/__init__.py
-office365/outlook/calendar/attendee.py
-office365/outlook/calendar/attendee_base.py
 office365/outlook/calendar/calendar.py
 office365/outlook/calendar/dateTimeTimeZone.py
 office365/outlook/calendar/email_address.py
-office365/outlook/calendar/event.py
 office365/outlook/calendar/group.py
 office365/outlook/calendar/location_constraint.py
-office365/outlook/calendar/meeting_time_suggestion.py
-office365/outlook/calendar/meeting_time_suggestions_result.py
 office365/outlook/calendar/permission.py
 office365/outlook/calendar/place.py
-office365/outlook/calendar/reminder.py
 office365/outlook/calendar/role_type.py
+office365/outlook/calendar/sharing_message.py
 office365/outlook/calendar/time_slot.py
+office365/outlook/calendar/time_zone_base.py
 office365/outlook/calendar/working_hours.py
+office365/outlook/calendar/attendees/__init__.py
+office365/outlook/calendar/attendees/attendee.py
+office365/outlook/calendar/attendees/availability.py
+office365/outlook/calendar/attendees/base.py
+office365/outlook/calendar/events/__init__.py
+office365/outlook/calendar/events/event.py
+office365/outlook/calendar/events/reminder.py
+office365/outlook/calendar/meetingtimes/__init__.py
+office365/outlook/calendar/meetingtimes/suggestion.py
+office365/outlook/calendar/meetingtimes/suggestions_result.py
 office365/outlook/calendar/schedule/__init__.py
 office365/outlook/calendar/schedule/information.py
 office365/outlook/calendar/schedule/item.py
 office365/outlook/contacts/__init__.py
 office365/outlook/contacts/contact.py
 office365/outlook/contacts/folder.py
 office365/outlook/internal/__init__.py
 office365/outlook/internal/paths/__init__.py
 office365/outlook/internal/queries/__init__.py
 office365/outlook/internal/queries/attachment_upload.py
 office365/outlook/mail/__init__.py
 office365/outlook/mail/automatic_replies_setting.py
 office365/outlook/mail/body_type.py
+office365/outlook/mail/conversation.py
 office365/outlook/mail/conversation_thread.py
 office365/outlook/mail/folder.py
 office365/outlook/mail/importance.py
 office365/outlook/mail/item_body.py
 office365/outlook/mail/location.py
 office365/outlook/mail/mailbox_settings.py
 office365/outlook/mail/patterned_recurrence.py
@@ -488,21 +522,21 @@
 office365/runtime/http/http_method.py
 office365/runtime/http/request_options.py
 office365/runtime/odata/__init__.py
 office365/runtime/odata/json_format.py
 office365/runtime/odata/method.py
 office365/runtime/odata/model.py
 office365/runtime/odata/parameter.py
-office365/runtime/odata/path_builder.py
 office365/runtime/odata/property.py
 office365/runtime/odata/query_options.py
 office365/runtime/odata/reader.py
 office365/runtime/odata/request.py
 office365/runtime/odata/type.py
 office365/runtime/odata/type_information.py
+office365/runtime/odata/url_builder.py
 office365/runtime/odata/v3/__init__.py
 office365/runtime/odata/v3/batch_request.py
 office365/runtime/odata/v3/json_light_format.py
 office365/runtime/odata/v3/metadata_level.py
 office365/runtime/odata/v3/metadata_reader.py
 office365/runtime/odata/v4/__init__.py
 office365/runtime/odata/v4/batch_request.py
@@ -536,14 +570,15 @@
 office365/search/entity.py
 office365/search/entity_type.py
 office365/search/hit.py
 office365/search/hits_container.py
 office365/search/query.py
 office365/search/request.py
 office365/search/response.py
+office365/search/sharepoint_onedrive_options.py
 office365/search/sort_property.py
 office365/sharepoint/__init__.py
 office365/sharepoint/base_entity.py
 office365/sharepoint/base_entity_collection.py
 office365/sharepoint/client_context.py
 office365/sharepoint/request.py
 office365/sharepoint/request_context.py
@@ -583,14 +618,20 @@
 office365/sharepoint/appprincipal/__init__.py
 office365/sharepoint/appprincipal/credential.py
 office365/sharepoint/appprincipal/identity_provider.py
 office365/sharepoint/appprincipal/manager.py
 office365/sharepoint/appprincipal/name.py
 office365/sharepoint/apps/__init__.py
 office365/sharepoint/apps/app_collection.py
+office365/sharepoint/apps/license.py
+office365/sharepoint/apps/license_collection.py
+office365/sharepoint/apps/license_manager.py
+office365/sharepoint/apps/properties.py
+office365/sharepoint/apps/solution_exporter.py
+office365/sharepoint/apps/user_solution.py
 office365/sharepoint/attachments/__init__.py
 office365/sharepoint/attachments/attachment.py
 office365/sharepoint/attachments/collection.py
 office365/sharepoint/attachments/creation_information.py
 office365/sharepoint/audit/__init__.py
 office365/sharepoint/audit/audit.py
 office365/sharepoint/authentication/__init__.py
@@ -618,14 +659,15 @@
 office365/sharepoint/changes/log_item_query.py
 office365/sharepoint/changes/query.py
 office365/sharepoint/changes/token.py
 office365/sharepoint/changes/type.py
 office365/sharepoint/changes/user.py
 office365/sharepoint/changes/web.py
 office365/sharepoint/clientsidecomponent/__init__.py
+office365/sharepoint/clientsidecomponent/component_context_info.py
 office365/sharepoint/clientsidecomponent/identifier.py
 office365/sharepoint/clientsidecomponent/query_result.py
 office365/sharepoint/clientsidecomponent/storage_entity.py
 office365/sharepoint/clientsidecomponent/hostedapps/__init__.py
 office365/sharepoint/clientsidecomponent/hostedapps/add_response.py
 office365/sharepoint/clientsidecomponent/hostedapps/app.py
 office365/sharepoint/clientsidecomponent/hostedapps/manager.py
@@ -684,14 +726,16 @@
 office365/sharepoint/directory/session.py
 office365/sharepoint/directory/user.py
 office365/sharepoint/directory/provider/__init__.py
 office365/sharepoint/directory/provider/provider.py
 office365/sharepoint/documentmanagement/__init__.py
 office365/sharepoint/documentmanagement/document_id.py
 office365/sharepoint/documentmanagement/document_set.py
+office365/sharepoint/esign/__init__.py
+office365/sharepoint/esign/models/__init__.py
 office365/sharepoint/eventreceivers/__init__.py
 office365/sharepoint/eventreceivers/creation_information.py
 office365/sharepoint/eventreceivers/definition.py
 office365/sharepoint/eventreceivers/definition_collection.py
 office365/sharepoint/excel/__init__.py
 office365/sharepoint/excel/excel_rest.py
 office365/sharepoint/features/__init__.py
@@ -747,14 +791,15 @@
 office365/sharepoint/files/file.py
 office365/sharepoint/files/move_operations.py
 office365/sharepoint/files/recent_file_collection.py
 office365/sharepoint/files/system_object_type.py
 office365/sharepoint/files/version.py
 office365/sharepoint/files/version_collection.py
 office365/sharepoint/files/version_event.py
+office365/sharepoint/fileservices/__init__.py
 office365/sharepoint/flows/__init__.py
 office365/sharepoint/flows/synchronization_result.py
 office365/sharepoint/folders/__init__.py
 office365/sharepoint/folders/collection.py
 office365/sharepoint/folders/delete_parameters.py
 office365/sharepoint/folders/download_parameters.py
 office365/sharepoint/folders/folder.py
@@ -766,14 +811,15 @@
 office365/sharepoint/internal/paths/__init__.py
 office365/sharepoint/internal/paths/entity.py
 office365/sharepoint/internal/queries/__init__.py
 office365/sharepoint/internal/queries/create_file.py
 office365/sharepoint/internal/queries/download_file.py
 office365/sharepoint/internal/queries/upload_file.py
 office365/sharepoint/internal/queries/upload_session.py
+office365/sharepoint/largeoperation/__init__.py
 office365/sharepoint/likes/__init__.py
 office365/sharepoint/likes/liked_by_information.py
 office365/sharepoint/likes/user_entity.py
 office365/sharepoint/listhome/__init__.py
 office365/sharepoint/listhome/favorite_lists.py
 office365/sharepoint/listhome/item.py
 office365/sharepoint/listitems/__init__.py
@@ -838,14 +884,16 @@
 office365/sharepoint/microservice/__init__.py
 office365/sharepoint/microservice/manager.py
 office365/sharepoint/migrationcenter/__init__.py
 office365/sharepoint/migrationcenter/common/__init__.py
 office365/sharepoint/migrationcenter/common/task.py
 office365/sharepoint/migrationcenter/common/task_definition.py
 office365/sharepoint/migrationcenter/common/task_entity_data.py
+office365/sharepoint/migrationcenter/common/results/__init__.py
+office365/sharepoint/migrationcenter/common/results/batch_creation.py
 office365/sharepoint/migrationcenter/service/__init__.py
 office365/sharepoint/multigeo/__init__.py
 office365/sharepoint/multigeo/unified_group.py
 office365/sharepoint/navigation/__init__.py
 office365/sharepoint/navigation/configured_metadata_items.py
 office365/sharepoint/navigation/home_site_navigation_settings.py
 office365/sharepoint/navigation/menu_node.py
@@ -1028,14 +1076,15 @@
 office365/sharepoint/search/administration/__init__.py
 office365/sharepoint/search/administration/document_crawl_log.py
 office365/sharepoint/search/administration/site_content_processing_info_provider.py
 office365/sharepoint/search/administration/site_me_ta_info_provider.py
 office365/sharepoint/search/administration/tenant_crawl_versions_info_provider.py
 office365/sharepoint/search/analytics/__init__.py
 office365/sharepoint/search/analytics/action.py
+office365/sharepoint/search/analytics/actor.py
 office365/sharepoint/search/analytics/signal.py
 office365/sharepoint/search/analytics/signal_store.py
 office365/sharepoint/search/query/__init__.py
 office365/sharepoint/search/query/auto_completion.py
 office365/sharepoint/search/query/auto_completion_match.py
 office365/sharepoint/search/query/auto_completion_results.py
 office365/sharepoint/search/query/condition.py
@@ -1185,14 +1234,15 @@
 office365/sharepoint/teams/__init__.py
 office365/sharepoint/teams/channel.py
 office365/sharepoint/teams/channel_manager.py
 office365/sharepoint/teams/site_owner_response.py
 office365/sharepoint/tenant/__init__.py
 office365/sharepoint/tenant/app_information.py
 office365/sharepoint/tenant/app_instance.py
+office365/sharepoint/tenant/app_utility.py
 office365/sharepoint/tenant/cdn_api.py
 office365/sharepoint/tenant/cdn_url.py
 office365/sharepoint/tenant/settings.py
 office365/sharepoint/tenant/administration/__init__.py
 office365/sharepoint/tenant/administration/deny_add_and_customize_pages_status.py
 office365/sharepoint/tenant/administration/endpoints.py
 office365/sharepoint/tenant/administration/response_message_center.py
@@ -1313,14 +1363,17 @@
 office365/sharepoint/views/type.py
 office365/sharepoint/views/view.py
 office365/sharepoint/views/visualization.py
 office365/sharepoint/viva/__init__.py
 office365/sharepoint/viva/app_configuration.py
 office365/sharepoint/viva/connections_url_configuration.py
 office365/sharepoint/viva/employee_engagement.py
+office365/sharepoint/viva/employee_experience_controller.py
+office365/sharepoint/viva/home.py
+office365/sharepoint/viva/home_title_region.py
 office365/sharepoint/viva/site_request_info.py
 office365/sharepoint/webhooks/__init__.py
 office365/sharepoint/webhooks/subscription.py
 office365/sharepoint/webhooks/subscription_collection.py
 office365/sharepoint/webhooks/subscription_information.py
 office365/sharepoint/webparts/__init__.py
 office365/sharepoint/webparts/definition.py
@@ -1350,14 +1403,17 @@
 office365/sharepoint/webs/time_zone.py
 office365/sharepoint/webs/time_zone_information.py
 office365/sharepoint/webs/web.py
 office365/sharepoint/workflow/__init__.py
 office365/sharepoint/workflow/association.py
 office365/sharepoint/workflow/template.py
 office365/sharepoint/workflowservices/__init__.py
+office365/sharepoint/workflowservices/instance.py
+office365/sharepoint/workflowservices/instance_service.py
+office365/sharepoint/workflowservices/manager.py
 office365/sharepoint/workmanagement/__init__.py
 office365/sharepoint/yammer/__init__.py
 office365/sharepoint/yammer/wac_api.py
 office365/subscriptions/__init__.py
 office365/subscriptions/change_notification.py
 office365/subscriptions/change_notification_collection.py
 office365/subscriptions/encrypted_content.py
@@ -1389,15 +1445,14 @@
 office365/teams/chats/__init__.py
 office365/teams/chats/chat.py
 office365/teams/chats/collection.py
 office365/teams/chats/message.py
 office365/teams/chats/message_attachment.py
 office365/teams/internal/__init__.py
 office365/teams/internal/paths/__init__.py
-office365/teams/internal/paths/team.py
 office365/teams/members/__init__.py
 office365/teams/members/aad_user_conversation.py
 office365/teams/members/conversation.py
 office365/teams/members/conversation_collection.py
 office365/teams/messages/__init__.py
 office365/teams/operations/__init__.py
 office365/teams/operations/async_operation.py
@@ -1418,12 +1473,19 @@
 office365/teams/shifts/time_off_reason.py
 office365/teams/tabs/__init__.py
 office365/teams/tabs/configuration.py
 office365/teams/tabs/tab.py
 office365/todo/__init__.py
 office365/todo/checklist_item.py
 office365/todo/linked_resource.py
-office365/todo/task.py
-office365/todo/task_list.py
-office365/todo/task_list_collection.py
 office365/todo/todo.py
-office365/todo/wellknown_list_name.py
+office365/todo/wellknown_list_name.py
+office365/todo/attachments/__init__.py
+office365/todo/attachments/base.py
+office365/todo/attachments/collection.py
+office365/todo/attachments/info.py
+office365/todo/attachments/task_file.py
+office365/todo/attachments/type.py
+office365/todo/tasks/__init__.py
+office365/todo/tasks/list.py
+office365/todo/tasks/list_collection.py
+office365/todo/tasks/task.py
```

### Comparing `Office365-REST-Python-Client-2.4.0/PKG-INFO` & `Office365-REST-Python-Client-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Office365-REST-Python-Client
-Version: 2.4.0
+Version: 2.4.1
 Summary: Microsoft 365 & Microsoft Graph Library for Python
 Home-page: https://github.com/vgrem/Office365-REST-Python-Client
 Author: Vadim Gremyachev
 Author-email: vvgrem@gmail.com
 Maintainer: Konrad Gądek, Domenico Di Nicola
 Maintainer-email: kgadek@gmail.com, dom.dinicola@gmail.com
 License: MIT
@@ -157,22 +157,22 @@
 print("Web title: {0}".format(web_title))
 ```
 
 
 The list of examples:
 
 - Working with files
-  - [download a file](examples/sharepoint/files/download_file.py) 
-  - [upload a file](examples/sharepoint/files/upload_file.py)
+  - [download a file](examples/sharepoint/files/download.py) 
+  - [upload a file](examples/sharepoint/files/upload.py)
 
 - Working with lists and list items
   -  [create a list item](examples/sharepoint/lists/data_generator.py)
-  -  [read a list item](examples/sharepoint/lists/read_large_list.py)   
-  -  [update a list item](examples/sharepoint/listitems/update_items_batch.py)
-  -  [delete a list item](examples/sharepoint/listitems/delete_list_item.py) 
+  -  [read a list item](examples/sharepoint/lists/read_large.py)   
+  -  [update a list item](examples/sharepoint/listitems/update_batch.py)
+  -  [delete a list item](examples/sharepoint/listitems/delete.py) 
   
 Refer [examples section](examples/sharepoint) for another scenarios
 
 # Working with Outlook API
 
 The list of supported APIs:
 -   [Outlook Contacts REST API](https://msdn.microsoft.com/en-us/office/office365/api/contacts-rest-operations)
@@ -191,15 +191,15 @@
 
 [The Microsoft Authentication Library (MSAL) for Python](https://pypi.org/project/msal/) which comes as a dependency 
 is used as a default library to obtain tokens to call Microsoft Graph API. 
 
 Using [Microsoft Authentication Library (MSAL) for Python](https://pypi.org/project/msal/)
 
 > Note: access token is getting acquired via [Client Credential flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)
-> in the provided examples. Other forms of token aquisition can be found here: https://msal-python.readthedocs.io/en/latest/
+> in the provided examples. Other forms of token acquisition can be found here: https://msal-python.readthedocs.io/en/latest/
 
 ```python
 import msal
 from office365.graph_client import GraphClient
 
 def acquire_token():
     """
@@ -259,25 +259,25 @@
     subject="Meet for lunch?",
     body="The new cafeteria is open.",
     to_recipients=["fannyd@contoso.onmicrosoft.com"]
 ).execute_query()
 
 ```
 
-> How to enable sending emails on behalf of another user in your organization: https://learn.microsoft.com/en-us/microsoft-365/solutions/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide&viewFallbackFrom=o365-worldwide%3FWT.mc_id%3D365AdminCSH_globalsearch
 
-Additional examples:
+Additional examples & scenarios:
+
+-  [download a message](examples/outlook/messages/download.py) 
+-  [list messages](examples/outlook/messages/list_all.py)
+-  [move messages to a different folder](examples/outlook/messages/move.py)
+-  [search messages](examples/outlook/messages/search.py)   
+-  [send messages](examples/outlook/messages/send.py)
+-  [send messages with attachments](examples/outlook/messages/send_with_attachment.py) 
+-  [enable sending emails on behalf of another user in your organization](https://learn.microsoft.com/en-us/microsoft-365/solutions/allow-members-to-send-as-or-send-on-behalf-of-group)
 
--  [download a message](examples/outlook/download_messages.py) 
--  [list messages](examples/outlook/list_message.py)
--  [move messages to a different folder](examples/outlook/move_message.py)
--  [search messages](examples/outlook/search_message.py)   
--  [send messages](examples/outlook/send_message.py)
--  [send messages with attachments](examples/outlook/send_message_with_attachment.py) 
-  
 Refer to [examples section](examples/outlook) for other scenarios
 
 
 # Working with OneDrive API
 
 #### Documentation 
 
@@ -348,15 +348,15 @@
             # download file content
             with open(os.path.join(local_path, drive_item.name), 'wb') as local_file:
                 drive_item.download(local_file).execute_query()
 ```
 
 Additional examples:
 
--  [create list column](examples/onedrive/create_list_column.py) 
+-  [create list column](examples/onedrive/columns/create_text.py) 
 -  [download file](examples/onedrive/download_file_default.py)
 -  [export files](examples/onedrive/export_files.py)
 -  [import files](examples/onedrive/import_files.py)   
 -  [list drives](examples/onedrive/list_drives.py)
 -  [list files](examples/onedrive/list_files.py)
 
 Refer to [OneDrive examples section](examples/onedrive) for more examples.
@@ -381,16 +381,16 @@
 client = GraphClient(acquire_token_func)
 new_team = client.groups["{group_id}"].add_team().execute_query_retry()
 ```
 
 Additional examples:
 
 -  [create a team](examples/teams/create_team.py) 
--  [create team from group](examples/teams/create_team_from_group.py)
--  [list all teams](examples/teams/list_all_teams.py)
+-  [create team from group](examples/teams/create_from_group.py)
+-  [list all teams](examples/teams/list_all.py)
 -  [list my teams](examples/teams/list_my_teams.py)   
 -  [send messages](examples/teams/send_message.py)
   
 Refer to [examples section](examples/teams) for other scenarios
 
 # Working with Microsoft Onenote API
```

### Comparing `Office365-REST-Python-Client-2.4.0/README.md` & `Office365-REST-Python-Client-2.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -127,22 +127,22 @@
 print("Web title: {0}".format(web_title))
 ```
 
 
 The list of examples:
 
 - Working with files
-  - [download a file](examples/sharepoint/files/download_file.py) 
-  - [upload a file](examples/sharepoint/files/upload_file.py)
+  - [download a file](examples/sharepoint/files/download.py) 
+  - [upload a file](examples/sharepoint/files/upload.py)
 
 - Working with lists and list items
   -  [create a list item](examples/sharepoint/lists/data_generator.py)
-  -  [read a list item](examples/sharepoint/lists/read_large_list.py)   
-  -  [update a list item](examples/sharepoint/listitems/update_items_batch.py)
-  -  [delete a list item](examples/sharepoint/listitems/delete_list_item.py) 
+  -  [read a list item](examples/sharepoint/lists/read_large.py)   
+  -  [update a list item](examples/sharepoint/listitems/update_batch.py)
+  -  [delete a list item](examples/sharepoint/listitems/delete.py) 
   
 Refer [examples section](examples/sharepoint) for another scenarios
 
 # Working with Outlook API
 
 The list of supported APIs:
 -   [Outlook Contacts REST API](https://msdn.microsoft.com/en-us/office/office365/api/contacts-rest-operations)
@@ -161,15 +161,15 @@
 
 [The Microsoft Authentication Library (MSAL) for Python](https://pypi.org/project/msal/) which comes as a dependency 
 is used as a default library to obtain tokens to call Microsoft Graph API. 
 
 Using [Microsoft Authentication Library (MSAL) for Python](https://pypi.org/project/msal/)
 
 > Note: access token is getting acquired via [Client Credential flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)
-> in the provided examples. Other forms of token aquisition can be found here: https://msal-python.readthedocs.io/en/latest/
+> in the provided examples. Other forms of token acquisition can be found here: https://msal-python.readthedocs.io/en/latest/
 
 ```python
 import msal
 from office365.graph_client import GraphClient
 
 def acquire_token():
     """
@@ -229,25 +229,25 @@
     subject="Meet for lunch?",
     body="The new cafeteria is open.",
     to_recipients=["fannyd@contoso.onmicrosoft.com"]
 ).execute_query()
 
 ```
 
-> How to enable sending emails on behalf of another user in your organization: https://learn.microsoft.com/en-us/microsoft-365/solutions/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide&viewFallbackFrom=o365-worldwide%3FWT.mc_id%3D365AdminCSH_globalsearch
 
-Additional examples:
+Additional examples & scenarios:
+
+-  [download a message](examples/outlook/messages/download.py) 
+-  [list messages](examples/outlook/messages/list_all.py)
+-  [move messages to a different folder](examples/outlook/messages/move.py)
+-  [search messages](examples/outlook/messages/search.py)   
+-  [send messages](examples/outlook/messages/send.py)
+-  [send messages with attachments](examples/outlook/messages/send_with_attachment.py) 
+-  [enable sending emails on behalf of another user in your organization](https://learn.microsoft.com/en-us/microsoft-365/solutions/allow-members-to-send-as-or-send-on-behalf-of-group)
 
--  [download a message](examples/outlook/download_messages.py) 
--  [list messages](examples/outlook/list_message.py)
--  [move messages to a different folder](examples/outlook/move_message.py)
--  [search messages](examples/outlook/search_message.py)   
--  [send messages](examples/outlook/send_message.py)
--  [send messages with attachments](examples/outlook/send_message_with_attachment.py) 
-  
 Refer to [examples section](examples/outlook) for other scenarios
 
 
 # Working with OneDrive API
 
 #### Documentation 
 
@@ -318,15 +318,15 @@
             # download file content
             with open(os.path.join(local_path, drive_item.name), 'wb') as local_file:
                 drive_item.download(local_file).execute_query()
 ```
 
 Additional examples:
 
--  [create list column](examples/onedrive/create_list_column.py) 
+-  [create list column](examples/onedrive/columns/create_text.py) 
 -  [download file](examples/onedrive/download_file_default.py)
 -  [export files](examples/onedrive/export_files.py)
 -  [import files](examples/onedrive/import_files.py)   
 -  [list drives](examples/onedrive/list_drives.py)
 -  [list files](examples/onedrive/list_files.py)
 
 Refer to [OneDrive examples section](examples/onedrive) for more examples.
@@ -351,16 +351,16 @@
 client = GraphClient(acquire_token_func)
 new_team = client.groups["{group_id}"].add_team().execute_query_retry()
 ```
 
 Additional examples:
 
 -  [create a team](examples/teams/create_team.py) 
--  [create team from group](examples/teams/create_team_from_group.py)
--  [list all teams](examples/teams/list_all_teams.py)
+-  [create team from group](examples/teams/create_from_group.py)
+-  [list all teams](examples/teams/list_all.py)
 -  [list my teams](examples/teams/list_my_teams.py)   
 -  [send messages](examples/teams/send_message.py)
   
 Refer to [examples section](examples/teams) for other scenarios
 
 # Working with Microsoft Onenote API
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/base_item.py` & `Office365-REST-Python-Client-2.4.1/office365/base_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 from office365.onedrive.listitems.item_reference import ItemReference
 
 
 class BaseItem(Entity):
     """The baseItem resource is an abstract resource that contains a common set of properties shared among several
     other resources types """
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/callrecords/call_record.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/callrecords/call_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 
 
 class CallRecord(Entity):
     """Represents a single peer-to-peer call or a group call between multiple participants,
     sometimes referred to as an online meeting."""
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/calls/call.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/calls/call.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/calls/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/calls/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/calls/participant.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/calls/participant.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/cloud_communications.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/cloud_communications.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/meeting_participants.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/meeting_participants.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/onlinemeetings/online_meeting.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/onlinemeetings/online_meeting.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/operations/comms.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/operations/comms.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/operations/invite_participants.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/operations/invite_participants.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/communications/presences/presence.py` & `Office365-REST-Python-Client-2.4.1/office365/communications/presences/presence.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/api.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/api.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/app_identity.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/app_identity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/application.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/application.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/public_client.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/public_client.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/roles/assignment.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/roles/assignment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/service_principal.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/service_principal.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         return self.properties.get('ownedObjects',
                                    DirectoryObjectCollection(self.context,
                                                              ResourcePath("ownedObjects", self.resource_path)))
 
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
-                "app_role_assigned_to": self.app_role_assigned_to,
+                "appRoleAssignedTo": self.app_role_assigned_to,
                 "created_objects": self.created_objects,
                 "oauth2PermissionScopes": self.oauth2_permission_scopes,
                 "ownedObjects": self.owned_objects,
                 "oauth2PermissionGrants": self.oauth2_permission_grants
             }
             default_value = property_mapping.get(name, None)
         return super(ServicePrincipal, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/template.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/template.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/applications/web.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/applications/web.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/audit/activity_initiator.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/audit/activity_initiator.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/audit/directory.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/audit/directory.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/audit/log_root.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/audit/log_root.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/audit/signins/signin.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/picker_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from office365.directory.audit.signins.status import SignInStatus
-from office365.entity import Entity
+from office365.sharepoint.base_entity import BaseEntity
+from office365.sharepoint.ui.applicationpages.peoplepicker.query_settings import PeoplePickerQuerySettings
 
 
-class SignIn(Entity):
-    """Details user and application sign-in activity for a tenant (directory).
-    You must have an Azure AD Premium P1 or P2 license to download sign-in logs using the Microsoft Graph API.
+class PickerSettings(BaseEntity):
+    """
+    This class contains configuration settings for the client people picker control hosted
+    by the SharePoint sharing UI.
     """
 
     @property
-    def user_id(self):
+    def allow_email_addresses(self):
         """
-        ID of the user that initiated the sign-in. Supports $filter (eq operator only).
-        :rtype: str or None
+        Boolean value indicating whether the picker control will allow the resolution of arbitrary email addresses.
         """
-        return self.properties.get("userId", None)
+        return self.properties.get("AllowEmailAddresses", None)
 
     @property
-    def user_principal_name(self):
+    def allow_only_email_addresses(self):
         """
-        User principal name of the user that initiated the sign-in. Supports $filter (eq and startsWith operators only).
-        :rtype: str or None
+        Boolean value indicating whether the picker control will only allow the resolution of email addresses.
         """
-        return self.properties.get("userPrincipalName", None)
+        return self.properties.get("AllowOnlyEmailAddresses", None)
 
     @property
-    def status(self):
+    def query_settings(self):
         """
-        Sign-in status. Includes the error code and description of the error (in case of a sign-in failure).
-        Supports $filter (eq operator only) on errorCode property.
-        :rtype: str or None
+        The query settings to be used by the picker control.
         """
-        return self.properties.get("status", SignInStatus())
+        return self.properties.get("QuerySettings", PeoplePickerQuerySettings())
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/audit/signins/status.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/audit/signins/status.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/authentication/authentication.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/authentication/basic.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/authentication/client_certificate.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/authentication/client_certificate.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,9 +7,12 @@
     """
     A type derived from apiAuthenticationConfigurationBase that is used to represent
     a Pkcs12-based client certificate authentication.
     This is used to retrieve the public properties of uploaded certificates.
     """
 
     def __init__(self, certificates=None):
+        """
+        :param list[Pkcs12CertificateInformation] certificates:
+        """
         super(ClientCertificateAuthentication, self).__init__()
         self.certificateList = ClientValueCollection(Pkcs12CertificateInformation, certificates)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/authentication/configuration_base.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/authentication/configuration_base.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/method.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/method.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/authentication/methods/phone.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/authentication/methods/phone.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/certificates/auth_configuration.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/certificates/auth_configuration.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/certificates/authority.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/certificates/authority.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/directory.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/directory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from office365.directory.administrative_unit import AdministrativeUnit
 from office365.directory.object_collection import DirectoryObjectCollection
 from office365.entity import Entity
+from office365.entity_collection import EntityCollection
 from office365.runtime.paths.resource_path import ResourcePath
 
 
 class Directory(Entity):
     """Represents a deleted item in the directory. When an item is deleted, it is added to the deleted items
     "container". Deleted items will remain available to restore for up to 30 days. After 30 days, the items are
     permanently deleted. """
@@ -16,14 +18,21 @@
                                                           ResourcePath("deletedItems", self.resource_path)))
         else:
             return self.properties.get('deletedItems',
                                        DirectoryObjectCollection(self.context,
                                                                  ResourcePath("deletedItems", self.resource_path)))
 
     @property
+    def administrative_units(self):
+        """	Conceptual container for user and group directory objects."""
+        return self.properties.get('administrativeUnits',
+                                   EntityCollection(self.context, AdministrativeUnit,
+                                                    ResourcePath("administrativeUnits", self.resource_path)))
+
+    @property
     def deleted_groups(self):
         """Recently deleted groups"""
         return self.deleted_items("microsoft.graph.group")
 
     @property
     def deleted_users(self):
         """Recently deleted users"""
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/extensions/extension_property.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/extensions/extension_property.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/groups/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/groups/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,15 @@
         """
         grp_properties = GroupProfile(group_name)
         grp_properties.securityEnabled = False
         grp_properties.mailEnabled = True
         grp_properties.groupTypes = ["Unified"]
         return_type = self.context.groups.add(grp_properties)
 
-        def _group_created(resp):
+        def _after_group_created(resp):
             """
             :type resp: requests.Response
             """
-            new_team = return_type.add_team()
-            return_type.set_property("team", new_team, False)
-
-        self.context.after_execute(_group_created)
+            resp.raise_for_status()
+            return_type.add_team()
+        self.context.after_execute(_after_group_created)
         return return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/groups/group.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/groups/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 from office365.directory.licenses.assigned_license import AssignedLicense
 from office365.directory.object import DirectoryObject
 from office365.directory.object_collection import DirectoryObjectCollection
 from office365.directory.permissions.grants.resource_specific import ResourceSpecificPermissionGrant
 from office365.entity_collection import EntityCollection
 from office365.onedrive.drives.drive import Drive
 from office365.onenote.onenote import Onenote
-from office365.outlook.calendar.event import Event
+from office365.outlook.calendar.events.event import Event
+from office365.outlook.mail.conversation import Conversation
 from office365.outlook.mail.conversation_thread import ConversationThread
 from office365.planner.group import PlannerGroup
-from office365.runtime.client_result import ClientResult
 from office365.runtime.client_value_collection import ClientValueCollection
 from office365.runtime.http.http_method import HttpMethod
-from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.runtime.paths.resource_path import ResourcePath
-from office365.teams.internal.paths.team import TeamPath
+from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.teams.team import Team
 
 
 class Group(DirectoryObject):
     """Represents an Azure Active Directory (Azure AD) group, which can be an Office 365 group, or a security group."""
 
     def renew(self):
@@ -73,60 +72,49 @@
     def unsubscribe_by_mail(self):
         """Calling this method will prevent the current user from receiving email notifications for this group
         about new posts, events, and files in that group. Supported for Microsoft 365 groups only."""
         qry = ServiceOperationQuery(self, "unsubscribeByMail")
         self.context.add_query(qry)
         return self
 
-    def check_member_groups(self, group_ids):
-        """Check for membership in the specified list of groups. Returns from the list those groups of which
-        the specified group has a direct or transitive membership.
-
-        You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types
-        of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups.
-        So membership in a Microsoft 365 group is always direct.
-
-        :param list[str] group_ids: A collection that contains the object IDs of the groups in which to
-            check membership. Up to 20 groups may be specified.
-        """
-        result = ClientResult(self.context)
-        qry = ServiceOperationQuery(self, "checkMemberGroups", None, group_ids, None, result)
-        self.context.add_query(qry)
-        return result
-
     def add_team(self):
         """Create a new team under a group."""
-        team = Team(self.context, TeamPath(self.resource_path))
-        team._parent_collection = self.parent_collection
-        qry = ServiceOperationQuery(self, "team", None, team, None, team)
-        self.context.add_query(qry)
+        qry = ServiceOperationQuery(self, "team", None, self.team, None, self.team)
 
         def _construct_create_team_request(request):
-            cur_qry = self.context.pending_request().current_query
-            if cur_qry.id == qry.id:
-                request.method = HttpMethod.Put
-                request.set_header('Content-Type', "application/json")
-                request.data = json.dumps(request.data)
-
-        self.context.before_execute(_construct_create_team_request, False)
-        return team
+            """
+            :type request: office365.runtime.http.request_options.RequestOptions
+            """
+            request.method = HttpMethod.Put
+            request.set_header('Content-Type', "application/json")
+            request.data = json.dumps(request.data)
+        self.context.before_execute_if_query(qry, _construct_create_team_request)
+        self.context.add_query(qry)
+        return self.team
 
     def delete_object(self, permanent_delete=False):
         """
         :param permanent_delete: Permanently deletes the group from directory
         :type permanent_delete: bool
 
         """
         super(Group, self).delete_object()
         if permanent_delete:
             deleted_item = self.context.directory.deleted_groups[self.id]
             deleted_item.delete_object()
         return self
 
     @property
+    def conversations(self):
+        """The group's conversations."""
+        return self.properties.get('conversations',
+                                   EntityCollection(self.context, Conversation,
+                                                    ResourcePath("threads", self.resource_path)))
+
+    @property
     def extensions(self):
         """
         The collection of open extensions defined for the group
         """
         return self.properties.get('extensions',
                                    EntityCollection(self.context, Extension,
                                                     ResourcePath("extensions", self.resource_path)))
@@ -213,14 +201,20 @@
     @property
     def planner(self):
         """The plannerGroup resource provide access to Planner resources for a group."""
         return self.properties.get('planner',
                                    PlannerGroup(self.context, ResourcePath("planner", self.resource_path)))
 
     @property
+    def team(self):
+        """The team associated with this group."""
+        return self.properties.get('team',
+                                   Team(self.context, ResourcePath(self.id, ResourcePath("teams"))))
+
+    @property
     def assigned_licenses(self):
         return self.properties.get('assignedLicenses', ClientValueCollection(AssignedLicense))
 
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
                 "appRoleAssignments": self.app_role_assignments,
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/groups/lifecycle_policy.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/groups/lifecycle_policy.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/groups/profile.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/groups/profile.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/api_connector.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/api_connector.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/container.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/container.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/identity.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/permissions/identity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/identity_set.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/collection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from office365.directory.identities.identity import Identity
-from office365.runtime.client_value import ClientValue
+from office365.runtime.client_result import ClientResult
+from office365.runtime.queries.service_operation import ServiceOperationQuery
+from office365.sharepoint.base_entity_collection import BaseEntityCollection
+from office365.sharepoint.comments.comment import Comment
 
 
-class IdentitySet(ClientValue):
-    """The IdentitySet resource is a keyed collection of identity resources. It is used to represent a set of
-    identities associated with various events for an item, such as created by or last modified by. """
+class CommentCollection(BaseEntityCollection):
 
-    def __init__(self):
-        super(IdentitySet, self).__init__()
-        self.application = Identity()
-        self.device = Identity()
-        self.user = Identity()
+    def __init__(self, context, resource_path=None):
+        super(CommentCollection, self).__init__(context, Comment, resource_path)
+
+    def delete_all(self):
+        """Deletes all the comments."""
+        return_type = ClientResult(self.context)
+        qry = ServiceOperationQuery(self, "DeleteAll", None, None, None, return_type)
+        self.context.add_query(qry)
+        return return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/object_identity.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/object_identity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/provider.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/provider.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/provider_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/provider_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/base_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/base_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/builtin_identity.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/builtin_identity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/providers/social_identity.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/providers/social_identity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/attribute.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/attribute.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/b2x/user_flow.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/b2x/user_flow.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/language_configuration.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/language_configuration.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/identities/userflows/user_attribute_assignment.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/identities/userflows/user_attribute_assignment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/licenses/assigned_license.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/licenses/assigned_license.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/licenses/details.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/licenses/details.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/licenses/service_plan_info.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/licenses/service_plan_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/object.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/object.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,14 +49,31 @@
         payload = {
             "securityEnabledOnly": security_enabled_only
         }
         qry = ServiceOperationQuery(self, "getMemberGroups", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
+    def check_member_groups(self, group_ids=None):
+        """Check for membership in the specified list of groups. Returns from the list those groups of which
+        the specified group has a direct or transitive membership.
+
+        You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types
+        of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups.
+        So membership in a Microsoft 365 group is always direct.
+
+        :param list[str] group_ids: A collection that contains the object IDs of the groups in which to
+            check membership. Up to 20 groups may be specified.
+        """
+        return_type = ClientResult(self.context, StringCollection())
+        payload = {"groupIds" : group_ids}
+        qry = ServiceOperationQuery(self, "checkMemberGroups", None, payload, None, return_type)
+        self.context.add_query(qry)
+        return return_type
+
     def restore(self):
         """
         Restore a recently deleted application, group, servicePrincipal, administrative unit, or user object from
         deleted items. If an item was accidentally deleted, you can fully restore the item. This is not applicable
         to security groups, which are deleted permanently.
 
         A recently deleted item will remain available for up to 30 days. After 30 days, the item is permanently deleted.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/object_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/object_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/password_credential.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/password_credential.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/permissions/grants/condition_set.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/permissions/grants/condition_set.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/permissions/scope.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/permissions/scope.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/policies/permission_grant.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/policies/permission_grant.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/policies/root.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/policies/root.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/policies/sts.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/policies/sts.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/profile_photo.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/profile_photo.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/roles/management.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/roles/management.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/roles/role.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/roles/role.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/users/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/users/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/users/identity.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/users/identity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/users/profile.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/users/profile.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/users/settings.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/users/settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/directory/users/user.py` & `Office365-REST-Python-Client-2.4.1/office365/directory/users/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from office365.communications.onlinemeetings.collection import OnlineMeetingCollection
 from office365.communications.presences.presence import Presence
 from office365.delta_collection import DeltaCollection
 from office365.directory.authentication.authentication import Authentication
 from office365.directory.extensions.extension import Extension
 from office365.directory.insights.office_graph import OfficeGraphInsights
 from office365.directory.licenses.assigned_plan import AssignedPlan
+from office365.directory.licenses.assignment_state import LicenseAssignmentState
 from office365.directory.permissions.grants.oauth2 import OAuth2PermissionGrant
 from office365.directory.users.settings import UserSettings
+from office365.intune.devices.managed import ManagedDevice
+from office365.intune.devices.managed_app_diagnostic_status import ManagedAppDiagnosticStatus
 from office365.onedrive.sites.site import Site
 from office365.onenote.onenote import Onenote
-from office365.outlook.calendar.attendee_base import AttendeeBase
+from office365.outlook.calendar.attendees.base import AttendeeBase
 from office365.outlook.calendar.calendar import Calendar
 from office365.outlook.calendar.group import CalendarGroup
-from office365.outlook.calendar.event import Event
-from office365.outlook.calendar.meeting_time_suggestions_result import MeetingTimeSuggestionsResult
-from office365.outlook.calendar.reminder import Reminder
+from office365.outlook.calendar.events.event import Event
+from office365.outlook.calendar.meetingtimes.suggestions_result import MeetingTimeSuggestionsResult
+from office365.outlook.calendar.events.reminder import Reminder
 from office365.directory.licenses.assigned_license import AssignedLicense
 from office365.directory.object import DirectoryObject
 from office365.directory.object_collection import DirectoryObjectCollection
 from office365.directory.licenses.details import LicenseDetails
 from office365.directory.identities.object_identity import ObjectIdentity
 from office365.directory.profile_photo import ProfilePhoto
 from office365.entity_collection import EntityCollection
@@ -86,28 +89,28 @@
         :param str body: The body of the message. It can be in HTML or text format
         :param list[str] to_recipients: The To: recipients for the message.
         :param list[str] cc_recipients: The CC: recipients for the message.
         :param list[str] bcc_recipients: The BCC: recipients for the message.
         :param bool save_to_sent_items: Indicates whether to save the message in Sent Items. Specify it only if
             the parameter is false; default is true
         """
-        message = Message(self.context)
-        message.subject = subject
-        message.body = body
-        [message.to_recipients.add(Recipient.from_email(email)) for email in to_recipients]
-        [message.bcc_recipients.add(Recipient.from_email(email)) for email in bcc_recipients]
-        [message.cc_recipients.add(Recipient.from_email(email)) for email in cc_recipients]
+        return_type = Message(self.context)
+        return_type.subject = subject
+        return_type.body = body
+        [return_type.to_recipients.add(Recipient.from_email(email)) for email in to_recipients]
+        [return_type.bcc_recipients.add(Recipient.from_email(email)) for email in bcc_recipients]
+        [return_type.cc_recipients.add(Recipient.from_email(email)) for email in cc_recipients]
 
         payload = {
-            "message": message,
+            "message": return_type,
             "saveToSentItems": save_to_sent_items
         }
         qry = ServiceOperationQuery(self, "sendmail", None, payload)
         self.context.add_query(qry)
-        return message
+        return return_type
 
     def export_personal_data(self, storage_location):
         """
         Submit a data policy operation request from a company administrator or an application to
         export an organizational user's data.
 
         If successful, this method returns a 202 Accepted response code.
@@ -118,41 +121,41 @@
         """
         qry = ServiceOperationQuery(self, "exportPersonalData", None, {"storage_location": storage_location})
         self.context.add_query(qry)
         return self
 
     def find_meeting_times(self, attendees=None, location_constraint=None):
         """
-        Suggest meeting times and locations based on organizer and attendee availability, and time or location
+        Suggest meeting times and locations based on organizer and attendees availability, and time or location
         constraints specified as parameters.
 
         If findMeetingTimes cannot return any meeting suggestions, the response would indicate a reason in the
         emptySuggestionsReason property. Based on this value, you can better adjust the parameters
         and call findMeetingTimes again.
 
         The algorithm used to suggest meeting times and locations undergoes fine-tuning from time to time.
         In scenarios like test environments where the input parameters and calendar data remain static, expect
         that the suggested results may differ over time.
 
         :param list[AttendeeBase] or None attendees: A collection of attendees or resources for the meeting.
-            Since findMeetingTimes assumes that any attendee who is a person is always required, specify required
+            Since findMeetingTimes assumes that any attendees who is a person is always required, specify required
             for a person and resource for a resource in the corresponding type property. An empty collection causes
             findMeetingTimes to look for free time slots for only the organizer. Optional.
         :param office365.outlook.calendar.location_constraint.LocationConstraint or None location_constraint:
             The organizer's requirements about the meeting location, such as whether a suggestion for a meeting
             location is required, or there are specific locations only where the meeting can take place. Optional.
         """
         payload = {
             "attendees": ClientValueCollection(AttendeeBase, attendees),
             "locationConstraint": location_constraint
         }
-        result = ClientResult(self.context, MeetingTimeSuggestionsResult())
-        qry = ServiceOperationQuery(self, "findMeetingTimes", None, payload, None, result)
+        return_type = ClientResult(self.context, MeetingTimeSuggestionsResult())
+        qry = ServiceOperationQuery(self, "findMeetingTimes", None, payload, None, return_type)
         self.context.add_query(qry)
-        return result
+        return return_type
 
     def get_calendar_view(self, start_dt, end_dt):
         """Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
            from the user's default calendar, or from some other calendar of the user's.
 
         :param datetime.datetime end_dt: The end date and time of the time range, represented in ISO 8601 format.
              For example, "2019-11-08T20:00:00-08:00".
@@ -188,14 +191,21 @@
             "startDateTime": start_dt.isoformat(),
             "endDateTime": end_dt.isoformat(),
         }
         qry = FunctionQuery(self, "reminderView", params, return_type)
         self.context.add_query(qry)
         return return_type
 
+    def get_managed_app_diagnostic_statuses(self):
+        """Gets diagnostics validation status for a given user."""
+        return_type = ClientResult(self.context, ClientValueCollection(ManagedAppDiagnosticStatus))
+        qry = FunctionQuery(self, "getManagedAppDiagnosticStatuses", None, return_type)
+        self.context.add_query(qry)
+        return return_type
+
     def delete_object(self, permanent_delete=False):
         """
         :param permanent_delete: Permanently deletes the user from directory
         :type permanent_delete: bool
 
         """
         super(User, self).delete_object()
@@ -318,14 +328,22 @@
         """Indicates whether the user account was created as a regular school or work account (null),
         an external account (Invitation), a local account for an Azure Active Directory B2C tenant (LocalAccount)
         or self-service sign-up using email verification (EmailVerified). Read-only.
         """
         return self.properties.get('creationType', None)
 
     @property
+    def license_assignment_states(self):
+        """
+        State of license assignments for this user. Also indicates licenses that are directly-assigned and those
+        that the user has inherited through group memberships.
+        """
+        return self.properties.get('licenseAssignmentStates', ClientValueCollection(LicenseAssignmentState))
+
+    @property
     def mail(self):
         """The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com".
            Returned by default. Supports $filter and endsWith.
         """
         return self.properties.get('mail', None)
 
     @property
@@ -462,28 +480,50 @@
     @property
     def joined_teams(self):
         """Get the teams in Microsoft Teams that the user is a direct member of."""
         return self.properties.get('joinedTeams',
                                    TeamCollection(self.context, ResourcePath("joinedTeams", self.resource_path)))
 
     @property
+    def managed_devices(self):
+        """"""
+        return self.properties.get('managedDevices',
+                                   EntityCollection(self.context, ManagedDevice,
+                                                    ResourcePath("managedDevices", self.resource_path)))
+
+    @property
     def member_of(self):
         """Get groups and directory roles that the user is a direct member of."""
         return self.properties.get('memberOf',
                                    DirectoryObjectCollection(self.context,
                                                              ResourcePath("memberOf", self.resource_path)))
 
     @property
     def oauth2_permission_grants(self):
         """"""
         return self.properties.get('oauth2PermissionGrants',
                                    DeltaCollection(self.context, OAuth2PermissionGrant,
                                                    ResourcePath("oauth2PermissionGrants", self.resource_path)))
 
     @property
+    def owned_devices(self):
+        """Devices that are owned by the user. Read-only. Nullable. Supports $expand and $filter
+        (/$count eq 0, /$count ne 0, /$count eq 1, /$count ne 1). """
+        return self.properties.get('ownedDevices',
+                                   DirectoryObjectCollection(self.context,
+                                                             ResourcePath("ownedDevices", self.resource_path)))
+
+    @property
+    def owned_objects(self):
+        """Directory objects that are owned by the user. Read-only. Nullable. Supports $expand. """
+        return self.properties.get('ownedObjects',
+                                   DirectoryObjectCollection(self.context,
+                                                             ResourcePath("ownedObjects", self.resource_path)))
+
+    @property
     def transitive_member_of(self):
         """Get groups, directory roles that the user is a member of. This API request is transitive, and will also
         return all groups the user is a nested member of. """
         return self.properties.get('transitiveMemberOf',
                                    DirectoryObjectCollection(self.context,
                                                              ResourcePath("transitiveMemberOf", self.resource_path)))
 
@@ -566,23 +606,26 @@
         if default_value is None:
             property_mapping = {
                 "businessPhones": self.business_phones,
                 "calendarGroups": self.calendar_groups,
                 "contactFolders": self.contact_folders,
                 "followedSites": self.followed_sites,
                 "licenseDetails": self.license_details,
+                "managedDevices": self.managed_devices,
                 "memberOf": self.member_of,
                 "transitiveMemberOf": self.transitive_member_of,
                 "joinedTeams": self.joined_teams,
                 "assignedLicenses": self.assigned_licenses,
                 "mailFolders": self.mail_folders,
                 "mailboxSettings": self.mailbox_settings,
                 "directReports": self.direct_reports,
                 "onlineMeetings": self.online_meetings,
-                "oauth2PermissionGrants": self.oauth2_permission_grants
+                "oauth2PermissionGrants": self.oauth2_permission_grants,
+                "ownedDevices": self.owned_devices,
+                "ownedObjects": self.owned_objects
             }
             default_value = property_mapping.get(name, None)
         return super(User, self).get_property(name, default_value)
 
     def set_property(self, name, value, persist_changes=True):
         super(User, self).set_property(name, value, persist_changes)
         # fallback: create a new resource path
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/entity.py` & `Office365-REST-Python-Client-2.4.1/office365/entity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/entity_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/entity_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/external/external.py` & `Office365-REST-Python-Client-2.4.1/office365/external/external.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/graph_client.py` & `Office365-REST-Python-Client-2.4.1/office365/graph_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from office365.communications.cloud_communications import CloudCommunications
 from office365.delta_collection import DeltaCollection
 from office365.directory.applications.application import Application
 from office365.directory.applications.template import ApplicationTemplate
 from office365.directory.applications.service_principal import ServicePrincipal
 from office365.directory.audit.log_root import AuditLogRoot
 from office365.directory.directory import Directory
+from office365.directory.domains.domain import Domain
+from office365.directory.identities.governance import IdentityGovernance
+from office365.directory.identities.protection_root import IdentityProtectionRoot
 from office365.directory.object_collection import DirectoryObjectCollection
 from office365.directory.groups.collection import GroupCollection
 from office365.directory.groups.lifecycle_policy import GroupLifecyclePolicy
 from office365.directory.groups.setting_template import GroupSettingTemplate
 from office365.directory.identities.container import IdentityContainer
 from office365.directory.identities.provider import IdentityProvider
 from office365.directory.internal.paths.me import MePath
 from office365.directory.licenses.subscribed_sku import SubscribedSku
 from office365.directory.permissions.grants.resource_specific import ResourceSpecificPermissionGrant
 from office365.directory.roles.management import RoleManagement
 from office365.directory.roles.role import DirectoryRole
+from office365.directory.users.invitation import InvitationCollection
 from office365.intune.devices.app_management import DeviceAppManagement
 from office365.intune.devices.management import DeviceManagement
 from office365.intune.organizations.contact import OrgContact
 from office365.intune.organizations.organization import Organization
 from office365.directory.policies.root import PolicyRoot
 from office365.directory.users.user import User
 from office365.directory.users.collection import UserCollection
@@ -127,19 +131,32 @@
 
     @property
     def users(self):
         """Get users"""
         return UserCollection(self, ResourcePath("users"))
 
     @property
+    def domains(self):
+        """Alias to domains"""
+        return EntityCollection(self, Domain, ResourcePath("domains"))
+
+    @property
     def groups(self):
         """Get groups"""
         return GroupCollection(self, ResourcePath("groups"))
 
     @property
+    def invitations(self):
+        """Get invitations"""
+        return InvitationCollection(self, ResourcePath("invitations"))
+
+    def identity_protection(self):
+        return IdentityProtectionRoot(self, ResourcePath("identityProtection"))
+
+    @property
     def sites(self):
         """Get sites"""
         return SitesWithRoot(self, ResourcePath("sites"))
 
     @property
     def shares(self):
         """Get shares"""
@@ -222,14 +239,21 @@
     def communications(self):
         """
         Cloud communications API endpoint
         """
         return CloudCommunications(self, ResourcePath("communications"))
 
     @property
+    def identity_governance(self):
+        """
+        The identity governance singleton
+        """
+        return IdentityGovernance(self, ResourcePath("identityGovernance"))
+
+    @property
     def subscriptions(self):
         """
         Retrieve the properties and relationships of webhook subscriptions,
         based on the app ID, the user, and the user's role with a tenant.
         """
         return EntityCollection(self, Subscription, ResourcePath("subscriptions"))
 
@@ -297,15 +321,15 @@
     @property
     def policies(self):
         """Resource type exposing navigation properties for the policies singleton."""
         return PolicyRoot(self, ResourcePath("policies"))
 
     @property
     def external(self):
-        """A logical container  for external sources."""
+        """A logical container for external sources."""
         return External(self, ResourcePath("external"))
 
     @property
     def security(self):
         """The security resource is the entry point for the Security object model.
         It returns a singleton security resource. It doesn't contain any usable properties."""
         return Security(self, ResourcePath("security"))
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/intune/audit/event.py` & `Office365-REST-Python-Client-2.4.1/office365/intune/audit/event.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/intune/devices/device.py` & `Office365-REST-Python-Client-2.4.1/office365/intune/devices/device.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/intune/devices/management.py` & `Office365-REST-Python-Client-2.4.1/office365/intune/devices/management.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from office365.entity import Entity
+from office365.entity_collection import EntityCollection
 from office365.intune.audit.event import AuditEventCollection
+from office365.intune.devices.managed import ManagedDevice
 from office365.runtime.paths.resource_path import ResourcePath
 
 
 class DeviceManagement(Entity):
     """
     The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in
     Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment
@@ -12,14 +14,22 @@
 
     @property
     def audit_events(self):
         """"""
         return self.properties.get("auditEvents", AuditEventCollection(self.context,
                                                                        ResourcePath("auditEvents", self.resource_path)))
 
+    @property
+    def managed_devices(self):
+        """"""
+        return self.properties.get('managedDevices',
+                                   EntityCollection(self.context, ManagedDevice,
+                                                    ResourcePath("managedDevices", self.resource_path)))
+
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
-                "auditEvents": self.audit_events
+                "auditEvents": self.audit_events,
+                "managedDevices": self.managed_devices
             }
             default_value = property_mapping.get(name, None)
         return super(DeviceManagement, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/intune/organizations/contact.py` & `Office365-REST-Python-Client-2.4.1/office365/intune/organizations/contact.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/intune/organizations/organization.py` & `Office365-REST-Python-Client-2.4.1/office365/intune/organizations/organization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from office365.directory.certificates.auth_configuration import CertificateBasedAuthConfiguration
+from office365.directory.domains.verified import VerifiedDomain
 from office365.directory.object import DirectoryObject
 from office365.directory.extensions.extension import Extension
 from office365.entity_collection import EntityCollection
 from office365.intune.provisioned_plan import ProvisionedPlan
 from office365.runtime.client_value_collection import ClientValueCollection
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.runtime.types.collections import StringCollection
@@ -38,16 +39,22 @@
                                                     ResourcePath("certificateBasedAuthConfiguration",
                                                                  self.resource_path)))
 
     @property
     def provisioned_plans(self):
         return self.properties.get("provisionedPlans", ClientValueCollection(ProvisionedPlan))
 
+    @property
+    def verified_domains(self):
+        """The collection of domains associated with this tenant."""
+        return self.properties.get("verifiedDomains", ClientValueCollection(VerifiedDomain))
+
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
                 "certificateBasedAuthConfiguration": self.certificate_based_auth_configuration,
                 "businessPhones": self.business_phones,
-                "provisionedPlans": self.provisioned_plans
+                "provisionedPlans": self.provisioned_plans,
+                "verifiedDomains": self.verified_domains
             }
             default_value = property_mapping.get(name, None)
         return super(Organization, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/logger.py` & `Office365-REST-Python-Client-2.4.1/office365/logger.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/item_activity.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/analytics/item_activity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 from office365.runtime.paths.resource_path import ResourcePath
 
 
 class ItemActivity(Entity):
     """
     The itemActivity resource provides information about activities that took place on an item or within a container.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/analytics/item_activity_stat.py` & `Office365-REST-Python-Client-2.4.1/office365/todo/tasks/list.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+from office365.directory.extensions.extension import Extension
 from office365.entity import Entity
 from office365.entity_collection import EntityCollection
-from office365.onedrive.analytics.item_activity import ItemActivity
 from office365.runtime.paths.resource_path import ResourcePath
+from office365.todo.tasks.task import TodoTask
 
 
-class ItemActivityStat(Entity):
-    """The itemActivityStat resource provides information about activities that took place
-    within an interval of time."""
+class TodoTaskList(Entity):
+    """A list in Microsoft To Do that contains one or more todoTask resources."""
 
     @property
-    def activities(self):
-        """Exposes the itemActivities represented in this itemActivityStat resource."""
-        return self.properties.get('activities',
-                                   EntityCollection(self.context, ItemActivity,
-                                                    ResourcePath("activities", self.resource_path)))
+    def extensions(self):
+        """The collection of open extensions defined for the task list."""
+        return self.properties.get('extensions',
+                                   EntityCollection(self.context, Extension,
+                                                    ResourcePath("extensions", self.resource_path)))
+
+    @property
+    def tasks(self):
+        """The tasks in this task list."""
+        return self.properties.get('tasks',
+                                   EntityCollection(self.context, TodoTask,
+                                                    ResourcePath("tasks", self.resource_path)))
+
+    @property
+    def entity_type_name(self):
+        return None
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/calculated.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/calculated.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/choice.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/choice.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/definition.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from office365.base_item import BaseItem
+from office365.onedrive.columns.boolean import BooleanColumn
 from office365.onedrive.columns.calculated import CalculatedColumn
 from office365.onedrive.columns.choice import ChoiceColumn
 from office365.onedrive.columns.default_value import DefaultColumnValue
 from office365.onedrive.columns.geolocation import GeolocationColumn
 from office365.onedrive.columns.hyperlink_or_picture import HyperlinkOrPictureColumn
 from office365.onedrive.columns.lookup import LookupColumn
 from office365.onedrive.columns.number import NumberColumn
@@ -48,14 +49,19 @@
 
     @property
     def column_group(self):
         """For site columns, the name of the group this column belongs to. Helps organize related columns."""
         return self.properties.get('columnGroup', None)
 
     @property
+    def boolean(self):
+        """This column stores boolean values."""
+        return self.properties.get('boolean', BooleanColumn())
+
+    @property
     def geolocation(self):
         """This column stores a geolocation."""
         return self.properties.get('geolocation', GeolocationColumn())
 
     @property
     def calculated(self):
         """This column's data is calculated based on other columns."""
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/definition_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/definition_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/lookup.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/lookup.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/number.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/number.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/person_or_group.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/person_or_group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/term.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/term.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/text.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/text.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/columns/validation.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/columns/validation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/content_type.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/content_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/contenttypes/order.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/contenttypes/order.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/content.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/content.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/document_set.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/document_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,12 @@
         :param str welcome_page_url:  Welcome page absolute URL.
         :param list[ContentTypeInfo] allowed_content_types:  Content types allowed in document set.
         :param list[DocumentSetContent] default_contents:  Default contents of document set.
         :param bool propagate_welcome_page_changes:  Specifies whether to push welcome page changes to inherited
             content types.
         :param bool should_prefix_name_to_file:  Indicates whether to add the name of the document set to each file name.
         """
-        super().__init__()
         self.welcomePageUrl = welcome_page_url
         self.allowedContentTypes = ClientValueCollection(ContentTypeInfo, allowed_content_types)
         self.defaultContents = ClientValueCollection(DocumentSetContent, default_contents)
         self.propagateWelcomePageChanges = propagate_welcome_page_changes
         self.shouldPrefixNameToFile = should_prefix_name_to_file
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/documentsets/version.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/documentsets/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.onedrive.documentsets.version_item import DocumentSetVersionItem
 from office365.onedrive.versions.list_item import ListItemVersion
 from office365.runtime.client_value_collection import ClientValueCollection
 
 
 class DocumentSetVersion(ListItemVersion):
     """Represents the version of a document set item in a list."""
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/driveItem.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/driveItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from office365.delta_path import DeltaPath
 from office365.onedrive.driveitems.audio import Audio
 from office365.onedrive.driveitems.geo_coordinates import GeoCoordinates
 from office365.onedrive.driveitems.image import Image
 from office365.onedrive.driveitems.item_preview_info import ItemPreviewInfo
 from office365.onedrive.driveitems.photo import Photo
 from office365.onedrive.driveitems.special_folder import SpecialFolder
 from office365.onedrive.internal.queries.resumable_file_upload import create_resumable_file_upload_query
@@ -476,18 +477,16 @@
         """
         return self.properties.get("webDavUrl", None)
 
     @property
     def children(self):
         """Collection containing Item objects for the immediate children of Item. Only items representing folders
         have children.
-
-        :rtype: EntityCollection
         """
-        return self.get_property('children',
+        return self.properties.get('children',
                                  EntityCollection(self.context, DriveItem, ChildrenPath(self.resource_path)))
 
     @property
     def listItem(self):
         """For drives in SharePoint, the associated document library list item."""
         return self.properties.get('listItem', ListItem(self.context, ResourcePath("listItem", self.resource_path)))
 
@@ -536,15 +535,15 @@
         return self.properties.get('analytics',
                                    ItemAnalytics(self.context, ResourcePath("analytics", self.resource_path)))
 
     @property
     def delta(self):
         """This method allows your app to track changes to a drive item and its children over time."""
         return self.properties.get('delta',
-                                   EntityCollection(self.context, DriveItem, ResourcePath("delta", self.resource_path)))
+                                   EntityCollection(self.context, DriveItem, DeltaPath(self.resource_path)))
 
     @property
     def subscriptions(self):
         """The set of subscriptions on the driveItem.
         """
         return self.properties.get('subscriptions',
                                    EntityCollection(self.context, Subscription,
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/geo_coordinates.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/geo_coordinates.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/publication_facet.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/publication_facet.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/remote_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/remote_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.runtime.client_value import ClientValue
 
 
 class RemoteItem(ClientValue):
     """
     The remoteItem resource indicates that a driveItem references an item that exists in another drive.
     This resource provides the unique IDs of the source drive and target item.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/thumbnail.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/thumbnail.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/thumbnail_set.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/thumbnail_set.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/driveitems/uploadable_properties.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/driveitems/uploadable_properties.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/drives/drive.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/drives/drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from office365.base_item import BaseItem
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity_collection import EntityCollection
 from office365.onedrive.driveitems.driveItem import DriveItem
 from office365.onedrive.driveitems.system_facet import SystemFacet
 from office365.onedrive.internal.paths.root import RootPath
 from office365.onedrive.lists.list import List
+from office365.onedrive.sharepoint_ids import SharePointIds
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.runtime.queries.function import FunctionQuery
 
 
 class Drive(BaseItem):
     """The drive resource is the top level object representing a user's OneDrive or a document library in
     SharePoint. """
@@ -51,15 +52,15 @@
         :rtype: str or None
         """
         return self.properties.get("driveType", None)
 
     @property
     def sharepoint_ids(self):
         """Returns identifiers useful for SharePoint REST compatibility."""
-        return self.properties.get('sharepointIds', None)
+        return self.properties.get('sharepointIds', SharePointIds())
 
     @property
     def system(self):
         """Optional. The user account that owns the drive. Read-only."""
         return self.properties.get('system', SystemFacet())
 
     @property
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/files/file.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/files/file.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/files/system_info.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/files/system_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/folders/folder.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/folders/folder.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/folders/view.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/folders/view.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/children.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/children.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/site.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/site.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/paths/url.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/paths/url.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/download_content.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/download_content.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/get_activities_by_interval.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/get_activities_by_interval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from office365.entity_collection import EntityCollection
 from office365.onedrive.analytics.item_activity_stat import ItemActivityStat
-from office365.runtime.http.http_method import HttpMethod
-from office365.runtime.queries.service_operation import ServiceOperationQuery
+from office365.runtime.queries.function import FunctionQuery
 
 
 def build_get_activities_by_interval_query(binding_type, start_dt=None, end_dt=None, interval=None):
     """
     :param office365.entity.Entity binding_type: Binding type
     :param datetime.datetime start_dt: The start time over which to aggregate activities.
     :param datetime.datetime end_dt: The end time over which to aggregate activities.
@@ -13,13 +12,9 @@
     """
     params = {
         "startDateTime": start_dt.strftime('%m-%d-%Y') if start_dt else None,
         "endDateTime": end_dt.strftime('%m-%d-%Y') if end_dt else None,
         "interval": interval
     }
     return_type = EntityCollection(binding_type.context, ItemActivityStat, binding_type.resource_path)
-    qry = ServiceOperationQuery(binding_type, "getActivitiesByInterval", params, None, None, return_type)
-
-    def _construct_request(request):
-        request.method = HttpMethod.Get
-    binding_type.context.before_execute(_construct_request)
+    qry = FunctionQuery(binding_type, "getActivitiesByInterval", params, return_type)
     return qry
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/resumable_file_upload.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/resumable_file_upload.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/internal/queries/upload_content.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/internal/queries/upload_content.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/item_reference.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/item_reference.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/listitems/list_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/listitems/list_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/info.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/lists/list.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/lists/list.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/permission.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/permission.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 from office365.entity_collection import EntityCollection
 from office365.onedrive.drives.recipient import DriveRecipient
 from office365.onedrive.listitems.item_reference import ItemReference
+from office365.onedrive.permissions.sharepoint_identity_set import SharePointIdentitySet
 from office365.onedrive.permissions.sharing_invitation import SharingInvitation
 from office365.onedrive.permissions.sharing_link import SharingLink
 from office365.runtime.client_value_collection import ClientValueCollection
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.runtime.types.collections import StringCollection
 
@@ -38,19 +39,29 @@
 
     @property
     def granted_to(self):
         """For user type permissions, the details of the users & applications for this permission."""
         return self.properties.get('grantedTo', IdentitySet())
 
     @property
+    def granted_to_v2(self):
+        """For user type permissions, the details of the users and applications for this permission."""
+        return self.properties.get('grantedToV2', SharePointIdentitySet())
+
+    @property
     def granted_to_identities(self):
         """For link type permissions, the details of the users to whom permission was granted. Read-only."""
         return self.properties.get('grantedToIdentities', ClientValueCollection(IdentitySet))
 
     @property
+    def granted_to_identities_v2(self):
+        """For link type permissions, the details of the users to whom permission was granted. """
+        return self.properties.get('grantedToIdentitiesV2', ClientValueCollection(SharePointIdentitySet))
+
+    @property
     def link(self):
         """Provides the link details of the current permission, if it is a link type permissions. Read-only."""
         return self.properties.get('link', SharingLink())
 
     @property
     def roles(self):
         """The type of permission, e.g. read. See below for the full list of roles. Read-only."""
@@ -91,11 +102,13 @@
         return self.properties.get("inheritedFrom", ItemReference())
 
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
                 "inheritedFrom": self.inherited_from,
                 "grantedTo": self.granted_to,
-                "grantedToIdentities": self.granted_to_identities
+                "grantedToV2": self.granted_to_v2,
+                "grantedToIdentities": self.granted_to_identities,
+                "grantedToIdentitiesV2": self.granted_to_identities_v2
             }
             default_value = property_mapping.get(name, None)
         return super(Permission, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/sharing_invitation.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/sharing_invitation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.runtime.client_value import ClientValue
 
 
 class SharingInvitation(ClientValue):
     """The SharingInvitation resource groups invitation-related data items into a single structure."""
 
     def __init__(self, email=None, invited_by=IdentitySet(), redeemed_by=None, signin_required=None):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/permissions/sharing_link.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/permissions/sharing_link.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/sharepoint_ids.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/sharepoint_ids.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/drive_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/drive_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from office365.base_item import BaseItem
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.onedrive.permissions.permission import Permission
 from office365.onedrive.driveitems.driveItem import DriveItem
 from office365.onedrive.lists.list import List
 from office365.onedrive.listitems.list_item import ListItem
 from office365.onedrive.internal.paths.root import RootPath
 from office365.onedrive.sites.site import Site
 from office365.runtime.paths.resource_path import ResourcePath
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/shares/shared.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/shares/shared.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/site.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/site.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/site_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/site_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/sites/sites_with_root.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/sites/sites_with_root.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/group.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/localized_description.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/localized_description.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/localized_label.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/localized_label.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/localized_name.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/localized_name.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/relation.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/relation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/set.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/set.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/set_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/set_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/store.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/store.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/term.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/term.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/termstore/term_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/termstore/term_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/base_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/base_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/drive_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/drive_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/versions/list_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/versions/list_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/applications/application.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/applications/application.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/charts/chart.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/charts/chart.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/comments/comment.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/comments/comment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/functions/functions.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/tenant_crawl_versions_info_provider.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-from office365.entity import Entity
-from office365.onedrive.workbooks.functions.result import WorkbookFunctionResult
+from office365.runtime.client_result import ClientResult
 from office365.runtime.queries.service_operation import ServiceOperationQuery
+from office365.sharepoint.base_entity import BaseEntity
 
 
-class WorkbookFunctions(Entity):
-    """Used as a container for Microsoft Excel worksheet function"""
+class TenantCrawlVersionsInfoProvider(BaseEntity):
+    """
 
-    def abs(self, number):
-        """"""
-        return_type = WorkbookFunctionResult(self.context)
+    """
+
+    def disable_crawl_versions(self, site_id):
+        """
+        :param str site_id:
+        """
+        return_type = ClientResult(self.context, bool())
         payload = {
-            "number": number,
+            "siteId": site_id
         }
-        qry = ServiceOperationQuery(self, "abs", None, payload, None, return_type)
+        qry = ServiceOperationQuery(self, "DisableCrawlVersions", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
-    def days(self, start_date, end_date):
-        """Returns the number of days between two dates.
 
-        :param datetime start_date:
-        :param datetime end_date:
+    def is_crawl_versions_enabled(self, site_id):
         """
-        return_type = WorkbookFunctionResult(self.context)
+        :param str site_id:
+        """
+        return_type = ClientResult(self.context, bool())
         payload = {
-            "startDate": start_date,
-            "endDate": end_date
+            "siteId": site_id
         }
-        qry = ServiceOperationQuery(self, "days", None, payload, None, return_type)
+        qry = ServiceOperationQuery(self, "IsCrawlVersionsEnabled", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
+
+    @property
+    def entity_type_name(self):
+        return "Microsoft.SharePoint.Client.Search.Administration.TenantCrawlVersionsInfoProvider"
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/names/named_item.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/names/named_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/format.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/format.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/range.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/range.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/ranges/view.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/ranges/view.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/columns/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/columns/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/columns/column.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/columns/column.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/pivot_table.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/pivot_table.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/rows/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/rows/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/rows/row.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/rows/row.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/tables/table.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/tables/table.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/workbook.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/workbook.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,53 +6,78 @@
 from office365.onedrive.workbooks.names.named_item import WorkbookNamedItem
 from office365.onedrive.workbooks.operations.workbook import WorkbookOperation
 from office365.onedrive.workbooks.session_info import WorkbookSessionInfo
 from office365.onedrive.workbooks.tables.collection import WorkbookTableCollection
 from office365.onedrive.workbooks.worksheets.collection import WorkbookWorksheetCollection
 from office365.runtime.client_result import ClientResult
 from office365.runtime.paths.resource_path import ResourcePath
+from office365.runtime.queries.function import FunctionQuery
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 
 
 class Workbook(Entity):
     """The top-level object that contains related workbook objects such as worksheets, tables, and ranges."""
 
     def session_info_resource(self):
         return_type = ClientResult(self.context, WorkbookSessionInfo())
-        qry = ServiceOperationQuery(self, "sessionInfoResource", None, None, None, return_type)
+        qry = FunctionQuery(self, "sessionInfoResource", None, return_type)
         self.context.add_query(qry)
         return return_type
 
-    def create_session(self):
+    def create_session(self, persist_changes=None):
         """
         Create a new workbook session.
 
         Excel APIs can be called in one of two modes:
             Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of
                 operation.
             Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel
                 backend server keeps a temporary copy of the file that reflects the changes made during that particular
                 API session. When the Excel session expires, the changes are lost. This mode is useful for apps that
                 need to do analysis or obtain the results of a calculation or a chart image, but not affect the
                 document state.
+
+        :param bool persist_changes: Determines whether persist changes
         """
+        payload = {"persistChanges": persist_changes}
         return_type = ClientResult(self.context, WorkbookSessionInfo())
-        qry = ServiceOperationQuery(self, "createSession", None, None, None, return_type)
+        qry = ServiceOperationQuery(self, "createSession", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
-    def refresh_session(self):
-        """Use this API to refresh an existing workbook session."""
+    def refresh_session(self, session_id):
+        """Use this API to refresh an existing workbook session.
+
+        :param str session_id: Identifier of the workbook session
+        """
         qry = ServiceOperationQuery(self, "refreshSession")
         self.context.add_query(qry)
+        def _construct_request(request):
+            """
+            :type request: office365.runtime.http.request_options.RequestOptions
+            """
+            request.set_header("workbook-session-id", session_id)
+
+        self.context.before_execute(_construct_request)
         return self
 
-    def close_session(self):
-        """Use this API to close an existing workbook session."""
+    def close_session(self, session_id):
+        """Use this API to close an existing workbook session.
+
+        :param str session_id: Identifier of the workbook session
+        """
         qry = ServiceOperationQuery(self, "closeSession")
+
+        def _construct_request(request):
+            """
+            :type request: office365.runtime.http.request_options.RequestOptions
+            """
+            request.set_header("workbook-session-id", session_id)
+
+        self.context.before_execute(_construct_request)
         self.context.add_query(qry)
         return self
 
     @property
     def application(self):
         """"""
         return self.properties.get('application',
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onedrive/workbooks/worksheets/worksheet.py` & `Office365-REST-Python-Client-2.4.1/office365/onedrive/workbooks/worksheets/worksheet.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/entity_hierarchy_model.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/entity_hierarchy_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.onenote.entity_schema_object_model import OnenoteEntitySchemaObjectModel
 
 
 class OnenoteEntityHierarchyModel(OnenoteEntitySchemaObjectModel):
 
     @property
     def display_name(self):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/entity_schema_object_model.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/entity_schema_object_model.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/internal/multipart_page_query.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/internal/multipart_page_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     return payload
 
 
 class OneNotePageCreateQuery(ClientQuery):
 
     def __init__(self, pages, presentation_file, attachment_files=None):
         """
-        :type pages: office365.onenote.pages.page_collection.OnenotePageCollection
+        :type pages: office365.onenote.pages.collection.OnenotePageCollection
         :type presentation_file: typing.IO
         :type attachment_files: dict or None
         """
         super(OneNotePageCreateQuery, self).__init__(pages.context, pages)
         pages.context.before_execute(self._construct_multipart_request)
         self._presentation = presentation_file
         if attachment_files is None:
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 from office365.entity_collection import EntityCollection
 from office365.onenote.notebooks.copy_notebook_model import CopyNotebookModel
 from office365.onenote.notebooks.notebook import Notebook
 from office365.onenote.notebooks.recent import RecentNotebook
 from office365.runtime.client_result import ClientResult
 from office365.runtime.client_value_collection import ClientValueCollection
-from office365.runtime.http.http_method import HttpMethod
+from office365.runtime.queries.function import FunctionQuery
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 
 
 class NotebookCollection(EntityCollection):
 
     def __init__(self, context, resource_path=None):
         super(NotebookCollection, self).__init__(context, Notebook, resource_path)
 
+    def add(self, display_name):
+        """
+        Create a new OneNote notebook.
+
+        :param str display_name: Name for the notebook. Notebook names must be unique. The name cannot contain more
+            than 128 characters or contain the following characters: ?*/:<>|'"
+        :rtype: Notebook
+        """
+        return super(NotebookCollection, self).add(displayName=display_name)
+
     def get_notebook_from_web_url(self, web_url):
         """
         Retrieve the properties and relationships of a notebook object by using its URL path.
         The location can be user notebooks on Microsoft 365, group notebooks,
         or SharePoint site-hosted team notebooks on Microsoft 365.
 
         :param str web_url: The URL path of the notebook to retrieve. It can also contain a "onenote:" prefix.
@@ -33,15 +43,10 @@
         :param bool include_personal_notebooks: Include notebooks owned by the user. Set to true to include notebooks
             owned by the user; otherwise, set to false. If you don't include the includePersonalNotebooks parameter,
             your request will return a 400 error response.
         """
 
         return_type = ClientResult(self.context, ClientValueCollection(RecentNotebook))
         params = {"includePersonalNotebooks": include_personal_notebooks}
-        qry = ServiceOperationQuery(self, "getRecentNotebooks", params, None, None, return_type)
+        qry = FunctionQuery(self, "getRecentNotebooks", params, return_type)
         self.context.add_query(qry)
-
-        def _construct_request(request):
-            request.method = HttpMethod.Get
-
-        self.context.before_execute(_construct_request)
         return return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/notebooks/notebook.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/notebooks/notebook.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/onenote.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/onenote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from office365.entity import Entity
 from office365.entity_collection import EntityCollection
 from office365.onenote.notebooks.collection import NotebookCollection
 from office365.onenote.operations.onenote import OnenoteOperation
-from office365.onenote.pages.page_collection import OnenotePageCollection
+from office365.onenote.pages.collection import OnenotePageCollection
 from office365.onenote.resources.resource import OnenoteResource
 from office365.onenote.sectiongroups.section_group import SectionGroup
 from office365.onenote.sections.section import OnenoteSection
 from office365.runtime.paths.resource_path import ResourcePath
 
 
 class Onenote(Entity):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/pages/page.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/pages/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from office365.onenote.entity_schema_object_model import OnenoteEntitySchemaObjectModel
 from office365.onenote.notebooks.notebook import Notebook
-from office365.onenote.pages.page_links import PageLinks
+from office365.onenote.pages.links import PageLinks
 from office365.onenote.sections.section import OnenoteSection
 from office365.runtime.client_result import ClientResult
 from office365.runtime.queries.function import FunctionQuery
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.runtime.types.collections import StringCollection
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/pages/page_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/pages/collection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from office365.entity_collection import EntityCollection
 from office365.onenote.internal.multipart_page_query import OneNotePageCreateQuery
 from office365.onenote.pages.page import OnenotePage
 
 
 class OnenotePageCollection(EntityCollection):
+    """A collection of pages in a OneNote notebook"""
 
     def __init__(self, context, resource_path=None):
         super(OnenotePageCollection, self).__init__(context, OnenotePage, resource_path)
 
     def add(self, presentation_file, attachment_files=None):
         """
+        Create a new OneNote page.
+
+        :param typing.IO presentation_file: Presentation file
+        :param dict or None attachment_files: Attachment files
         :rtype: OnenotePage
         """
         qry = OneNotePageCreateQuery(self, presentation_file, attachment_files)
         self.context.add_query(qry)
         return qry.return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/resources/resource.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/base_entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-from office365.onenote.entity_base_model import OnenoteEntityBaseModel
-from office365.runtime.client_result import ClientResult
-from office365.runtime.http.http_method import HttpMethod
-from office365.runtime.queries.service_operation import ServiceOperationQuery
-
-
-class OnenoteResource(OnenoteEntityBaseModel):
-    """An image or other file resource on a OneNote page."""
-
-    def get_content(self):
-        """Retrieve the binary data of a file or image resource object."""
-        result = ClientResult(self.context)
-        qry = ServiceOperationQuery(self, "content", None, None, None, result)
-
-        def _construct_query(request):
-            """
-            :type request: office365.runtime.http.request_options.RequestOptions
-            """
-            request.method = HttpMethod.Get
-        self.context.before_execute(_construct_query)
+from office365.runtime.client_object import ClientObject
+from office365.runtime.queries.delete_entity import DeleteEntityQuery
+from office365.runtime.queries.update_entity import UpdateEntityQuery
+
+
+class BaseEntity(ClientObject):
+    """SharePoint specific entity"""
+
+    def with_credentials(self, credentials):
+        """
+        :type self: T
+        :type credentials:  UserCredential or ClientCredential
+        """
+        self.context.with_credentials(credentials)
+        return self
+
+    def delete_object(self):
+        """The recommended way to delete a SharePoint entity"""
+        qry = DeleteEntityQuery(self)
         self.context.add_query(qry)
-        return result
+        self.remove_from_parent_collection()
+        return self
 
-    @property
-    def content_url(self):
-        """The URL for downloading the content
+    def update(self, *args):
+        """The recommended way to update a SharePoint entity"""
+        qry = UpdateEntityQuery(self)
+        self.context.add_query(qry)
+        return self
 
-        :rtype: str or None
+    @property
+    def context(self):
         """
-        return self.properties.get("contentUrl", None)
+        :rtype: office365.sharepoint.client_context.ClientContext
+        """
+        return self._context
+
+    @property
+    def entity_type_name(self):
+        if self._entity_type_name is None:
+            self._entity_type_name = ".".join(["SP", type(self).__name__])
+        return self._entity_type_name
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/sectiongroups/section_group.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/sectiongroups/section_group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/onenote/sections/section.py` & `Office365-REST-Python-Client-2.4.1/office365/onenote/sections/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from office365.entity_collection import EntityCollection
 from office365.onenote.entity_hierarchy_model import OnenoteEntityHierarchyModel
 from office365.onenote.operations.onenote import OnenoteOperation
-from office365.onenote.pages.page_links import PageLinks
+from office365.onenote.pages.links import PageLinks
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.runtime.paths.resource_path import ResourcePath
 
 
 class OnenoteSection(OnenoteEntityHierarchyModel):
     """A section in a OneNote notebook. Sections can contain pages."""
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/attendee.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/attendee.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from office365.outlook.calendar.attendee_base import AttendeeBase
+from office365.outlook.calendar.attendees.base import AttendeeBase
 from office365.outlook.calendar.email_address import EmailAddress
 
 
 class Attendee(AttendeeBase):
-    """An event attendee. This can be a person or resource such as a meeting room or equipment,
+    """An event attendees. This can be a person or resource such as a meeting room or equipment,
     that has been set up as a resource on the Exchange server for the tenant."""
 
-    def __init__(self, emailAddress=EmailAddress(), attendee_type=None, proposedNewTime=None, status=None):
+    def __init__(self, email_address=EmailAddress(), attendee_type=None, proposed_new_time=None, status=None):
         """
 
-        :param office365.mail.emailAddress.EmailAddress emailAddress emailAddress:
-        :param office365.calendar.timeSlot.TimeSlot proposedNewTime:
-        :param str status: The attendee's response (none, accepted, declined, etc.) for the event and date-time
+        :param office365.mail.emailAddress.EmailAddress emailAddress email_address:
+        :param office365.calendar.timeSlot.TimeSlot proposed_new_time:
+        :param str status: The attendees's response (none, accepted, declined, etc.) for the event and date-time
             that the response was sent.
         """
-        super(Attendee, self).__init__(emailAddress, attendee_type)
-        self.proposedNewTime = proposedNewTime
+        super(Attendee, self).__init__(email_address, attendee_type)
+        self.proposedNewTime = proposed_new_time
         self.status = status
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/attendee_base.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/attendees/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from office365.outlook.mail.recipient import Recipient
 
 
 class AttendeeBase(Recipient):
-    """The type of attendee."""
+    """The type of attendees."""
 
     def __init__(self, email_address, attendee_type=None):
         """
 
-        :param office365.mail.emailAddress.EmailAddress email_address: Includes the name and SMTP address of the attendee
-        :param str attendee_type: The type of attendee. The possible values are: required, optional, resource.
-            Currently if the attendee is a person, findMeetingTimes always considers the person is of the Required type.
+        :param office365.mail.emailAddress.EmailAddress email_address: Includes the name and SMTP address of the attendees
+        :param str attendee_type: The type of attendees. The possible values are: required, optional, resource.
+            Currently if the attendees is a person, findMeetingTimes always considers the person is of the Required type.
         """
         super(AttendeeBase, self).__init__(email_address)
         self.type = attendee_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/calendar.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from office365.outlook.calendar.permission import CalendarPermission
 from office365.outlook.calendar.dateTimeTimeZone import DateTimeTimeZone
 from office365.outlook.calendar.email_address import EmailAddress
-from office365.outlook.calendar.event import Event
+from office365.outlook.calendar.events.event import Event
 from office365.outlook.calendar.schedule.information import ScheduleInformation
 from office365.entity import Entity
 from office365.entity_collection import EntityCollection
 from office365.runtime.client_result import ClientResult
 from office365.runtime.client_value_collection import ClientValueCollection
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.runtime.paths.resource_path import ResourcePath
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/dateTimeTimeZone.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/dateTimeTimeZone.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/event.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/events/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from office365.delta_collection import DeltaCollection
 from office365.directory.extensions.extended_property import SingleValueLegacyExtendedProperty
 from office365.entity_collection import EntityCollection
-from office365.outlook.calendar.attendee import Attendee
 from office365.directory.extensions.extension import Extension
+from office365.outlook.calendar.attendees.attendee import Attendee
 from office365.outlook.calendar.dateTimeTimeZone import DateTimeTimeZone
 from office365.outlook.calendar.email_address import EmailAddress
 from office365.outlook.item import OutlookItem
 from office365.outlook.mail.attachments.collection import AttachmentCollection
 from office365.outlook.mail.item_body import ItemBody
 from office365.outlook.mail.location import Location
 from office365.runtime.client_value_collection import ClientValueCollection
@@ -33,15 +34,15 @@
 
     def cancel(self, comment=None):
         """
         This action allows the organizer of a meeting to send a cancellation message and cancel the event.
 
         The action moves the event to the Deleted Items folder. The organizer can also cancel an occurrence
         of a recurring meeting by providing the occurrence event ID.
-        An attendee calling this action gets an error (HTTP 400 Bad Request), with the following error message:
+        An attendees calling this action gets an error (HTTP 400 Bad Request), with the following error message:
             Your request can't be completed. You need to be an organizer to cancel a meeting.
 
         :param str comment: Text included in the response.
         """
         payload = {
             "Comment": comment
         }
@@ -220,15 +221,15 @@
                                    EntityCollection(self.context, Extension,
                                                     ResourcePath("extensions", self.resource_path)))
 
     @property
     def instances(self):
         """The collection of open extensions defined for the event. Nullable."""
         return self.properties.get('instances',
-                                   EntityCollection(self.context, Event, ResourcePath("instances", self.resource_path)))
+                                   DeltaCollection(self.context, Event, ResourcePath("instances", self.resource_path)))
 
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
                 "singleValueExtendedProperties": self.single_value_extended_properties
             }
             default_value = property_mapping.get(name, None)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/group.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/meeting_time_suggestions_result.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/meetingtimes/suggestions_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from office365.outlook.calendar.meeting_time_suggestion import MeetingTimeSuggestion
+from office365.outlook.calendar.meetingtimes.suggestion import MeetingTimeSuggestion
 from office365.runtime.client_value import ClientValue
 from office365.runtime.client_value_collection import ClientValueCollection
 
 
 class MeetingTimeSuggestionsResult(ClientValue):
     """
     A collection of meeting suggestions if there is any, or the reason if there isn't.
     """
-    def __init__(self, meetingTimeSuggestions=None,
-                 emptySuggestionsReason=None):
+    def __init__(self, meeting_time_suggestions=None, empty_suggestions_reason=None):
         """
 
-        :param ClientValueCollection(MeetingTimeSuggestion) meetingTimeSuggestions: An array of meeting suggestions.
-        :param str emptySuggestionsReason: A reason for not returning any meeting suggestions.
+        :param list[MeetingTimeSuggestion] meeting_time_suggestions: An array of meeting suggestions.
+        :param str empty_suggestions_reason: A reason for not returning any meeting suggestions.
             The possible values are: attendeesUnavailable, attendeesUnavailableOrUnknown, locationsUnavailable,
             organizerUnavailable, or unknown. This property is an empty string if the meetingTimeSuggestions property
             does include any meeting suggestions.
         """
         super(MeetingTimeSuggestionsResult, self).__init__()
-        self.meetingTimeSuggestions = ClientValueCollection(MeetingTimeSuggestion) if meetingTimeSuggestions is None \
-            else meetingTimeSuggestions
-        self.emptySuggestionsReason = emptySuggestionsReason
+        self.meetingTimeSuggestions = ClientValueCollection(MeetingTimeSuggestion, meeting_time_suggestions)
+        self.emptySuggestionsReason = empty_suggestions_reason
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/permission.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/permission.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/place.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/place.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/calendar/schedule/information.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/calendar/schedule/information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/contacts/contact.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/contacts/contact.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/contacts/folder.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/contacts/folder.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/internal/queries/attachment_upload.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/internal/queries/attachment_upload.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/locale_info.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/locale_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/attachment.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/attachment_item.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/attachment_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,35 @@
 
 class AttachmentCollection(EntityCollection):
     """Attachment collection"""
 
     def __init__(self, context, resource_path=None):
         super(AttachmentCollection, self).__init__(context, Attachment, resource_path)
 
-    def add_file(self, name, content, content_type=None):
+    def add_file(self, name, content=None, content_type=None, base64_content=None):
         """
         Attach a file to message
 
         :param str name: The name representing the text that is displayed below the icon representing the
              embedded attachment
-        :param str content: The contents of the file
+        :param str or None content: The contents of the file
         :param str or None content_type: The content type of the attachment.
+        :param str or None base64_content: The contents of the file in the form of a base64 string.
         """
+        if not content and not base64_content:
+            raise TypeError("Either content or base64_content is required")
         from office365.outlook.mail.attachments.file import FileAttachment
+
         return_type = FileAttachment(self.context)
         return_type.name = name
-        return_type.content_bytes = base64.b64encode(content.encode("utf-8")).decode("utf-8")
+        if base64_content:
+            content = base64_content
+        else:
+            content = base64.b64encode(content.encode("utf-8")).decode("utf-8")
+        return_type.content_bytes = content
         return_type.content_type = content_type
         self.add_child(return_type)
         return self
 
     def resumable_upload(self, source_path, chunk_size=1000000, chunk_uploaded=None):
         """
         Create an upload session to allow your app to upload files up to the maximum file size.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/file.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/file.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/attachments/item.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/attachments/item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/folder.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/folder.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/item_body.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/item_body.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/mailbox_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/mailbox_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/event_message.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/event_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     acceptance, tentative acceptance, or decline)."""
 
     @property
     def event(self):
         """The event associated with the event message. The assumption for attendees or room resources is that
         the Calendar Attendant is set to automatically update the calendar with an event when meeting request event
         messages arrive. Navigation property. Read-only."""
-        from office365.outlook.calendar.event import Event
+        from office365.outlook.calendar.events.event import Event
         return self.properties.get('event',
                                    Event(self.context, ResourcePath("event", self.resource_path)))
 
     @property
     def patterned_recurrence(self):
         """"""
         return self.properties.get("patternedRecurrence", PatternedRecurrence())
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/messages/message.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/messages/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,24 +56,29 @@
         Get MIME content of a message
         """
         return_type = ClientResult(self.context)
         qry = FunctionQuery(self, "$value", None, return_type)
         self.context.add_query(qry)
         return return_type
 
-    def add_file_attachment(self, name, content, content_type=None):
+    def add_file_attachment(
+        self, name, content=None, content_type=None, base64_content=None
+    ):
         """
         Attach a file to message
 
         :param str name: The name representing the text that is displayed below the icon representing the
              embedded attachment
-        :param str content: The contents of the file
+        :param str or None content: The contents of the file
         :param str or None content_type: The content type of the attachment.
+        :param str or None base64_content: The contents of the file in the form of a base64 string.
         """
-        self.attachments.add_file(name, content, content_type)
+        if not content and not base64_content:
+            raise TypeError("Either content or base64_content is required")
+        self.attachments.add_file(name, content, content_type, base64_content)
         return self
 
     def upload_attachment(self, file_path, chunk_uploaded=None):
         """
         This approach is used to attach a file if the file size is between 3 MB and 150 MB, otherwise
         if a file that's smaller than 3 MB, then add_file_attachment method is utilized
 
@@ -119,20 +124,33 @@
 
     def reply_all(self):
         """Reply to all recipients of a message. The message is then saved in the Sent Items folder. """
         qry = ServiceOperationQuery(self, "replyAll")
         self.context.add_query(qry)
         return self
 
+    def create_reply(self, comment=None):
+        """
+        Create a draft to reply to the sender of a message in either JSON or MIME format.
+
+        :param str comment:
+        """
+        return_type = Message(self.context)
+        payload = {
+            "comment" : comment
+        }
+        qry = ServiceOperationQuery(self, "createReply", None, payload, None, return_type)
+        self.context.add_query(qry)
+        return self
+
     def create_reply_all(self):
         """
         Create a draft to reply to the sender and all the recipients of the specified message.
         You can then update the draft to add reply content to the body or change other message properties, or,
         simply send the draft.
-        :return:
         """
         qry = ServiceOperationQuery(self, "createReplyAll")
         self.context.add_query(qry)
         return self
 
     def move(self, destination_id):
         """
@@ -231,14 +249,27 @@
         return self.get_property('bccRecipients', ClientValueCollection(Recipient), True)
 
     @property
     def cc_recipients(self):
         """The CC: recipients for the message."""
         return self.get_property('ccRecipients', ClientValueCollection(Recipient), True)
 
+    @property
+    def sender(self):
+        """The account that is actually used to generate the message. In most cases, this value is the same as the
+        from property. You can set this property to a different value when sending a message from a shared mailbox,
+        for a shared calendar, or as a delegate. In any case, the value must correspond to the actual mailbox used.
+        Find out more about setting the from and sender properties of a message."""
+        return self.get_property('sender', Recipient())
+
+    @property
+    def parent_folder_id(self):
+        """The unique identifier for the message's parent mailFolder."""
+        return self.get_property('parentFolderId', None)
+
     def get_property(self, name, default_value=None, track_changes=False):
         if default_value is None:
             property_type_mapping = {
                 "toRecipients": self.to_recipients
             }
             default_value = property_type_mapping.get(name, None)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/patterned_recurrence.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/patterned_recurrence.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/physical_address.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/physical_address.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/mail/recipient.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/mail/recipient.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/timezone_information.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/timezone_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/outlook/user.py` & `Office365-REST-Python-Client-2.4.1/office365/outlook/user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/planner/group.py` & `Office365-REST-Python-Client-2.4.1/office365/planner/group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/planner/planner.py` & `Office365-REST-Python-Client-2.4.1/office365/planner/planner.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/planner/plans/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/planner/plans/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/planner/plans/plan.py` & `Office365-REST-Python-Client-2.4.1/office365/planner/plans/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 from office365.entity_collection import EntityCollection
 from office365.planner.buckets.bucket import PlannerBucket
 from office365.planner.plans.plan_details import PlannerPlanDetails
 from office365.planner.tasks.task import PlannerTask
 from office365.runtime.paths.resource_path import ResourcePath
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/planner/tasks/check_list_items.py` & `Office365-REST-Python-Client-2.4.1/office365/planner/tasks/check_list_items.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/planner/user.py` & `Office365-REST-Python-Client-2.4.1/office365/planner/user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/reports/internal/queries/create_report_query.py` & `Office365-REST-Python-Client-2.4.1/office365/reports/internal/queries/create_report_query.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/reports/report_root.py` & `Office365-REST-Python-Client-2.4.1/office365/reports/report_root.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/authentication_context.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/authentication_context.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/acs_token_provider.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/acs_token_provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,22 +38,24 @@
 
     def get_app_only_access_token(self):
         try:
             realm = self._get_realm_from_target_url()
             url_info = urlparse(self.url)
             return self._get_app_only_access_token(url_info.hostname, realm)
         except requests.exceptions.RequestException as e:
-            self.error = e.response.text
-            raise ValueError(e.response.text)
+            self.error = e.response.text if e.response is not None else "Acquire app-only access token failed."
+            raise ValueError(self.error)
 
     def _get_app_only_access_token(self, target_host, target_realm):
         """
+        Retrieves an app-only access token from ACS to call the specified principal
+        at the specified targetHost. The targetHost must be registered for target principal.
 
-        :type target_host: str
-        :type target_realm: str
+        :param str target_host: Url authority of the target principal
+        :param str target_realm: Realm to use for the access token's nameid and audience
         """
         resource = self.get_formatted_principal(self.SharePointPrincipal, target_host, target_realm)
         principal_id = self.get_formatted_principal(self._client_id, None, target_realm)
         sts_url = self.get_security_token_service_url(target_realm)
         oauth2_request = {
             'grant_type': 'client_credentials',
             'client_id': principal_id,
@@ -63,19 +65,23 @@
         }
         response = requests.post(url=sts_url, headers={'Content-Type': 'application/x-www-form-urlencoded'},
                                  data=oauth2_request)
         response.raise_for_status()
         return TokenResponse.from_json(response.json())
 
     def _get_realm_from_target_url(self):
+        """Get the realm for the URL"""
         response = requests.head(url=self.url, headers={'Authorization': 'Bearer'})
         return self.process_realm_response(response)
 
     @staticmethod
     def process_realm_response(response):
+        """
+        :type response: requests.Response
+        """
         header_key = "WWW-Authenticate"
         if header_key in response.headers:
             auth_values = response.headers[header_key].split(",")
             bearer = auth_values[0].split("=")
             return bearer[1].replace('"', '')
         return None
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/ntlm_provider.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/ntlm_provider.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/oauth_token_provider.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/oauth_token_provider.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/saml_token_provider.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/saml_token_provider.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/FederatedSAML.xml` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/FederatedSAML.xml`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/RST2.xml` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/RST2.xml`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/providers/templates/SAML.xml` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/providers/templates/SAML.xml`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/sts_profile.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/sts_profile.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/auth/token_response.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/auth/token_response.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_object.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
     @property
     def properties(self):
         return self._properties
 
     @property
     def parent_collection(self):
+        """Parent collection"""
         return self._parent_collection
 
     def to_json(self, json_format=None):
         """
         Serializes client object
 
         :type json_format: office365.runtime.odata.json_format.ODataJsonFormat or None
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_object_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_object_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_request.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_request_exception.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_request_exception.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_result.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 from typing import TypeVar
 
 from office365.runtime.client_value import ClientValue
 
 T = TypeVar("T", int, str, bytes, bool, ClientValue)
 
 
@@ -12,15 +13,15 @@
         """
         Client result
 
         :type context: office365.runtime.client_runtime_context.ClientRuntimeContext
         :type default_value: T
         """
         self._context = context
-        self._value = default_value
+        self._value = copy.deepcopy(default_value)
 
     def after_execute(self, action, *args, **kwargs):
 
         def _process_response(resp):
             """
             :type resp: requests.Response
             """
@@ -33,16 +34,16 @@
     def set_property(self, key, value, persist_changes=False):
         """
         :type key: str
         :type value: T
         :type persist_changes: bool
         """
         from office365.runtime.client_value import ClientValue
-        if isinstance(self.value, ClientValue):
-            self.value.set_property(key, value, persist_changes)
+        if isinstance(self._value, ClientValue):
+            self._value.set_property(key, value, persist_changes)
         else:
             self._value = value
 
     @property
     def value(self):
         return self._value
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_runtime_context.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_runtime_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,34 @@
             self.before_execute(before_loaded)
         if callable(after_loaded):
             def _action():
                 after_loaded(client_object)
             self.after_query_execute(qry, _action)
         return self
 
+    def before_execute_if_query(self, query, action, *args, **kwargs):
+        """
+        Attach an event handler which is triggered before query is submitted to server
+
+        :type query: office365.runtime.queries.client_query.ClientQuery
+        :type action: (office365.runtime.http.request_options.RequestOptions, *args, **kwargs) -> None
+        """
+
+        def _prepare_request(request):
+            """
+            :type request: office365.runtime.http.request_options.RequestOptions
+            """
+            if self.current_query.id == query.id:
+                action(request, *args, **kwargs)
+            else:
+                self.pending_request().beforeExecute -= _prepare_request
+
+        self.pending_request().beforeExecute += _prepare_request
+        return self
+
     def before_execute(self, action, once=True, *args, **kwargs):
         """
         Attach an event handler which is triggered before request is submitted to server
 
         :param (office365.runtime.http.request_options.RequestOptions, any) -> None action:
         :param bool once: Flag which determines whether action is executed once or multiple times
         """
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_value.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/client_value_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/client_value_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/compat.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/compat.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/http/request_options.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/http/request_options.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/json_format.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/json_format.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/path_builder.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/url_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 from office365.runtime.client_value import ClientValue
 from office365.runtime.compat import is_string_type
 
 
-class ODataPathBuilder(object):
+class ODataUrlBuilder(object):
 
     @staticmethod
     def build(name, parameters=None):
         """
         Constructs path segment from operation name and parameters
 
         :type parameters: list or dict or ClientValue
@@ -16,18 +16,18 @@
         """
         url = name or ""
         if isinstance(parameters, ClientValue):
             url += "(@v)?@v={0}".format(json.dumps(parameters.to_json()))
         elif parameters is not None:
             url += "("
             if isinstance(parameters, dict):
-                url += ','.join(['%s=%s' % (key, ODataPathBuilder.encode_method_value(value)) for (key, value) in
+                url += ','.join(['%s=%s' % (key, ODataUrlBuilder.encode_method_value(value)) for (key, value) in
                                  parameters.items() if value is not None])
             else:
-                url += ','.join(['%s' % (ODataPathBuilder.encode_method_value(value)) for (i, value) in
+                url += ','.join(['%s' % (ODataUrlBuilder.encode_method_value(value)) for (i, value) in
                                  enumerate(parameters) if value is not None])
             url += ")"
         return url
 
     @staticmethod
     def encode_method_value(value):
         if is_string_type(value):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/query_options.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/query_options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import copy
 
 
-def _normalize(key, value):
-    if key == "select" or key == "expand":
-        return ",".join(value)
-    return value
-
-
 class QueryOptions(object):
 
-    def __init__(self, select=None, expand=None, filter_expr=None, order_by=None, top=None, skip=None):
+    def __init__(self, select=None, expand=None, filter_expr=None, order_by=None, top=None, skip=None, custom=None):
         """
         A query option is a set of query string parameters applied to a resource that can help control the amount
         of data being returned for the resource in the URL
 
         :param list[str] select: The $select system query option allows the clients to requests a limited set of
         properties for each entity or complex type.
         :param list[str] expand: The $expand system query option specifies the related resources to be included in
@@ -22,25 +16,29 @@
         that are addressed by a request URL.
         :param str order_by: The $orderby system query option allows clients to request resources in either ascending
         order using asc or descending order using desc
         :param int top: The $top system query option requests the number of items in the queried collection to
         be included in the result.
         :param int skip: The $skip query option requests the number of items in the queried collection that
         are to be skipped and not included in the result.
+        :param dict custom: A custom query options
         """
         if expand is None:
             expand = []
         if select is None:
             select = []
         self.select = select
         self.expand = expand
         self.filter = filter_expr
         self.orderBy = order_by
         self.skip = skip
         self.top = top
+        if custom is None:
+            custom = {}
+        self.custom = custom
 
     @staticmethod
     def build(client_object, properties_to_include=None):
         """
         :param office365.runtime.client_object.ClientObject client_object: Client object
         :param list[str] or None properties_to_include: The list of properties to include
         """
@@ -65,24 +63,35 @@
         return self.to_url()
 
     def __str__(self):
         return self.to_url()
 
     @property
     def is_empty(self):
-        result = {k: v for (k, v) in self.__dict__.items() if v is not None and v}
+        result = {k: v for (k, v) in self}
         return not result
 
     def reset(self):
         self.select = []
         self.expand = []
         self.filter = None
         self.orderBy = None
         self.skip = None
         self.top = None
+        self.custom = {}
 
     def to_url(self):
         """Convert query options to url
         :return: str
         """
-        return '&'.join(['$%s=%s' % (key, _normalize(key, value))
-                         for (key, value) in self.__dict__.items() if value is not None and value])
+        return '&'.join(['$%s=%s' % (key, value) for (key, value) in self])
+
+    def __iter__(self):
+        for k, v in self.__dict__.items():
+            if v:
+                if k == "select" or k == "expand":
+                    yield k, ",".join(v)
+                elif k == "custom":
+                    for c_k, c_v in self.custom.items():
+                        yield c_k, c_v
+                else:
+                    yield k, v
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/reader.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/reader.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/request.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from office365.runtime.client_object import ClientObject
 from office365.runtime.client_request import ClientRequest
 from office365.runtime.client_result import ClientResult
 from office365.runtime.client_value import ClientValue
 from office365.runtime.http.http_method import HttpMethod
 from office365.runtime.http.request_options import RequestOptions
 from office365.runtime.odata.v3.json_light_format import JsonLightFormat
-from office365.runtime.paths.service_operation import ServiceOperationPath
 from office365.runtime.queries.create_entity import CreateEntityQuery
 from office365.runtime.queries.delete_entity import DeleteEntityQuery
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.runtime.queries.update_entity import UpdateEntityQuery
 
 
 class ODataRequest(ClientRequest):
@@ -61,16 +60,14 @@
         if response.headers.get('Content-Type', '').lower().split(';')[0] != 'application/json':
             if isinstance(return_type, ClientResult):
                 return_type.set_property("__value", response.content)
         else:
             if isinstance(json_format, JsonLightFormat):
                 if isinstance(query, ServiceOperationQuery):
                     json_format.function = query.method_name
-                elif isinstance(return_type.resource_path, ServiceOperationPath):
-                    json_format.function = return_type.resource_path.name
 
             self.map_json(response.json(), return_type, json_format)
 
     def map_json(self, json, return_type, json_format=None):
         """
         :type json: any
         :type return_type: ClientValue or ClientResult or ClientObject
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/type.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/batch_request.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/batch_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/json_light_format.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/json_light_format.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v3/metadata_level.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v3/metadata_level.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/batch_request.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/batch_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/json_format.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/json_format.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/metadata_level.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/metadata_level.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/odata/v4/upload_session_request.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/odata/v4/upload_session_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/paths/entity.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/paths/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     @property
     def collection(self):
         return self._collection
 
     @property
     def segments(self):
-        return [self.delimiter, str(self.name or '<id>')]
+        return [self.delimiter, str(self.name or '<null>')]
 
     def normalize(self, name, inplace=False):
         """
         Normalizes entity path
 
         :type name: str or None
         :type inplace: bool
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/paths/resource_path.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/paths/resource_path.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/paths/service_operation.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/paths/service_operation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from office365.runtime.paths.resource_path import ResourcePath
-from office365.runtime.odata.path_builder import ODataPathBuilder
+from office365.runtime.odata.url_builder import ODataUrlBuilder
 
 
 class ServiceOperationPath(ResourcePath):
     """Path to address Service Operations which represents simple functions exposed by an OData service"""
 
     def __init__(self, name, parameters=None, parent=None):
         """
@@ -12,8 +12,8 @@
         :type parent: office365.runtime.paths.resource_path.ResourcePath
         """
         super(ServiceOperationPath, self).__init__(name, parent)
         self._parameters = parameters
 
     @property
     def segments(self):
-        return [self.delimiter, ODataPathBuilder.build(self._name, self._parameters)]
+        return [self.delimiter, ODataUrlBuilder.build(self._name, self._parameters)]
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/batch.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/batch.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/client_query.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/client_query.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/create_entity.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/create_entity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/function.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.runtime.odata.path_builder import ODataPathBuilder
+from office365.runtime.odata.url_builder import ODataUrlBuilder
 from office365.runtime.queries.client_query import ClientQuery
 
 
 class FunctionQuery(ClientQuery):
     """"Service operation query"""
 
     def __init__(self, binding_type,
@@ -22,15 +22,15 @@
                                             return_type)
         self._method_name = method_name
         self._method_params = method_params
 
     @property
     def url(self):
         orig_url = super(FunctionQuery, self).url
-        return "/".join([orig_url, ODataPathBuilder.build(self._method_name, self._method_params)])
+        return "/".join([orig_url, ODataUrlBuilder.build(self._method_name, self._method_params)])
 
     @property
     def method_name(self):
         return self._method_name
 
     @property
     def method_parameters(self):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/read_entity.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/read_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,10 +11,10 @@
         :type entity: office365.runtime.client_object.ClientObject
         """
         super(ReadEntityQuery, self).__init__(entity.context, entity, None, None, entity)
         self._properties_to_include = properties_to_include
 
     @property
     def url(self):
-        query_url = super(ReadEntityQuery, self).url
+        orig_url = super(ReadEntityQuery, self).url
         query_options = QueryOptions.build(self.binding_type, self._properties_to_include)
-        return query_url if query_options.is_empty else query_url + "?" + str(query_options)
+        return orig_url if query_options.is_empty else orig_url + "?" + str(query_options)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/service_operation.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/service_operation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.runtime.odata.path_builder import ODataPathBuilder
+from office365.runtime.odata.url_builder import ODataUrlBuilder
 from office365.runtime.queries.client_query import ClientQuery
 
 
 class ServiceOperationQuery(ClientQuery):
     """"Service operation query"""
 
     def __init__(self, binding_type,
@@ -26,19 +26,19 @@
         self._method_params = method_params
         self.static = is_static
 
     @property
     def url(self):
         orig_url = super(ServiceOperationQuery, self).url
         if self.static:
-            normalized_name = ".".join([self.binding_type.entity_type_name, self.method_name])
+            static_name = ".".join([self.binding_type.entity_type_name, self.method_name])
             return "/".join([self.context.service_root_url(),
-                             ODataPathBuilder.build(normalized_name, self._method_params)])
+                             ODataUrlBuilder.build(static_name, self._method_params)])
         else:
-            return "/".join([orig_url, ODataPathBuilder.build(self._method_name, self._method_params)])
+            return "/".join([orig_url, ODataUrlBuilder.build(self._method_name, self._method_params)])
 
     @property
     def method_name(self):
         return self._method_name
 
     @property
     def method_parameters(self):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/update_entity.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/update_entity.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/queries/upload_session.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/queries/upload_session.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/types/collections.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/types/collections.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/runtime/types/event_handler.py` & `Office365-REST-Python-Client-2.4.1/office365/runtime/types/event_handler.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/search/aggregation.py` & `Office365-REST-Python-Client-2.4.1/office365/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/search/entity.py` & `Office365-REST-Python-Client-2.4.1/office365/search/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,9 +42,15 @@
     def query_events(self, query_string):
         """Searches Outlook calendar events. Alias to query method
 
         :param str query_string: Contains the query terms.
         """
         return self.query(query_string, entity_types=[EntityType.event])
 
+    def query_drive_items(self, query_string):
+        """Searches OneDrive items.
+        Alias to query method
 
+        :param str query_string: Contains the query terms.
+        """
+        return self.query(query_string, entity_types=[EntityType.driveItem])
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/search/hit.py` & `Office365-REST-Python-Client-2.4.1/office365/search/hit.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/search/hits_container.py` & `Office365-REST-Python-Client-2.4.1/office365/search/hits_container.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/search/request.py` & `Office365-REST-Python-Client-2.4.1/office365/search/request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/search/response.py` & `Office365-REST-Python-Client-2.4.1/office365/search/response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from office365.runtime.client_value import ClientValue
 from office365.runtime.client_value_collection import ClientValueCollection
+from office365.runtime.types.collections import StringCollection
 from office365.search.hits_container import SearchHitsContainer
 
 
 class SearchResponse(ClientValue):
     """Represents results from a search query, and the terms used for the query."""
 
     def __init__(self, search_terms=None, hits_containers=None):
         """
         :param list[str] search_terms: Contains the search terms sent in the initial search query.
         :param list[SearchHitsContainer] hits_containers: A collection of search results.
 
         """
         super(SearchResponse, self).__init__()
-        self.searchTerms = search_terms
+        self.searchTerms = StringCollection(search_terms)
         self.hitsContainers = ClientValueCollection(SearchHitsContainer, hits_containers)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/facets/sharing.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/facets/sharing.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/activities/tracked_item_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/activities/tracked_item_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/analytics/usage_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/analytics/usage_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/web_application.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/web_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     def lookup(context, request_uri):
         """
         :type context
         :type request_uri str
         """
         return_type = WebApplication(context)
         payload = {"requestUri": request_uri}
-        qry = ServiceOperationQuery(return_type, "Lookup", None, payload, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(return_type, "Lookup", None, payload, None, return_type, True)
         context.add_query(qry)
         return return_type
 
     @property
     def outbound_mail_sender_address(self):
         """
         :rtype: str or None
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/administration/web_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/administration/web_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/alert.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/alert.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/alerts/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/alerts/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/analytics/usage_entry.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/analytics/usage_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,15 @@
         :param str item_id: The identifier of the item for which the event is being logged.
         """
         payload = {
             "eventTypeId": event_type_id,
             "itemId": item_id,
         }
         binding_type = AnalyticsUsageEntry(context)
-        qry = ServiceOperationQuery(binding_type, "LogAnalyticsEvent", None, payload)
-        qry.static = True
+        qry = ServiceOperationQuery(binding_type, "LogAnalyticsEvent", None, payload, is_static=True)
         context.add_query(qry)
         return binding_type
 
     @staticmethod
     def log_analytics_app_event2(context, app_event_type_id, item_id, rollup_scope_id, site_id, user_id):
         """
         Creates and logs an analytics event into the analytics pipeline with additional parameters.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/appprincipal/credential.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/appprincipal/credential.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/attachment.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/attachments/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/attachments/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/audit/audit.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/audit/audit.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/authentication/acs_service_principal_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/authentication/acs_service_principal_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/base_entity.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/businessdata/app_bdc_catalog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,24 @@
-from office365.runtime.client_object import ClientObject
-from office365.runtime.queries.delete_entity import DeleteEntityQuery
-from office365.runtime.queries.update_entity import UpdateEntityQuery
+from office365.runtime.client_result import ClientResult
+from office365.runtime.queries.service_operation import ServiceOperationQuery
+from office365.runtime.types.collections import StringCollection
+from office365.sharepoint.base_entity import BaseEntity
 
 
-class BaseEntity(ClientObject):
-    """SharePoint specific entity"""
+class AppBdcCatalog(BaseEntity):
+    """
+    Represents the Business Data Connectivity (BDC) MetadataCatalog for an application that contains external content
+    types provisioned by the application.
+    """
 
-    def with_credentials(self, credentials):
+    def get_permissible_connections(self):
         """
-        :type self: T
-        :type credentials:  UserCredential or ClientCredential
+        Gets the list of external connections that the application has permissions to use.
         """
-        self.context.with_credentials(credentials)
-        return self
-
-    def delete_object(self):
-        """The recommended way to delete a SharePoint entity"""
-        qry = DeleteEntityQuery(self)
-        self.context.add_query(qry)
-        self.remove_from_parent_collection()
-        return self
-
-    def update(self, *args):
-        """The recommended way to update a SharePoint entity"""
-        qry = UpdateEntityQuery(self)
+        return_type = ClientResult(self.context, StringCollection())
+        qry = ServiceOperationQuery(self, "GetPermissibleConnections", None, None, None, return_type)
         self.context.add_query(qry)
-        return self
-
-    @property
-    def context(self):
-        """
-        :rtype: office365.sharepoint.client_context.ClientContext
-        """
-        return self._context
+        return return_type
 
     @property
     def entity_type_name(self):
-        if self._entity_type_name is None:
-            self._entity_type_name = ".".join(["SP", type(self).__name__])
-        return self._entity_type_name
+        return "SP.BusinessData.AppBdcCatalog"
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/campaigns/campaigns.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/campaigns/campaigns.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/change.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/change.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/list.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/list.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/log_item_query.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/log_item_query.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/changes/query.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/changes/query.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/client_context.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/client_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -335,14 +335,20 @@
     @property
     def ee(self):
         """Alias to EmployeeEngagement"""
         from office365.sharepoint.viva.employee_engagement import EmployeeEngagement
         return EmployeeEngagement(self)
 
     @property
+    def employee_experience(self):
+        """Alias to EmployeeExperience"""
+        from office365.sharepoint.viva.employee_experience_controller import EmployeeExperienceController
+        return EmployeeExperienceController(self)
+
+    @property
     def micro_service_manager(self):
         """Alias to MicroServiceManager"""
         from office365.sharepoint.microservice.manager import MicroServiceManager
         return MicroServiceManager(self, ResourcePath("microServiceManager"))
 
     @property
     def directory_session(self):
@@ -453,14 +459,20 @@
     @property
     def site_manager(self):
         """Alias to SPSiteManager. Represents methods for creating and managing SharePoint sites"""
         from office365.sharepoint.portal.sites.manager import SPSiteManager
         return SPSiteManager(self, ResourcePath("spSiteManager"))
 
     @property
+    def social_feed_manager(self):
+        """Alias to SocialFeedManager."""
+        from office365.sharepoint.social.feed.manager import SocialFeedManager
+        return SocialFeedManager(self)
+
+    @property
     def home_service(self):
         """Alias to SharePointHomeServiceContextBuilder."""
         from office365.sharepoint.portal.home.service_context_builder import SharePointHomeServiceContextBuilder
         return SharePointHomeServiceContextBuilder(self, ResourcePath("sphomeservice"))
 
     @property
     def home_site(self):
@@ -500,14 +512,20 @@
     @property
     def tenant_settings(self):
         """Alias to TenantSettings"""
         from office365.sharepoint.tenant.settings import TenantSettings
         return TenantSettings.current(self)
 
     @property
+    def workflow_services_manager(self):
+        """Alias to WorkflowServicesManager"""
+        from office365.sharepoint.workflowservices.manager import WorkflowServicesManager
+        return WorkflowServicesManager.current(self)
+
+    @property
     def work_items(self):
         from office365.sharepoint.contentcenter.machinelearning.workitems.collection import \
             SPMachineLearningWorkItemCollection
         return SPMachineLearningWorkItemCollection(self, ResourcePath("workitems"))
 
     @property
     def tenant(self):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/hostedapps/manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/hostedapps/manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/clientsidecomponent/query_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/clientsidecomponent/query_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/service_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from office365.runtime.client_result import ClientResult
 from office365.runtime.queries.service_operation import ServiceOperationQuery
-from office365.sharepoint.base_entity_collection import BaseEntityCollection
-from office365.sharepoint.comments.comment import Comment
+from office365.runtime.paths.resource_path import ResourcePath
+from office365.sharepoint.base_entity import BaseEntity
+from office365.sharepoint.publishing.video.channel_collection import VideoChannelCollection
 
 
-class CommentCollection(BaseEntityCollection):
+class VideoServiceManager(BaseEntity):
 
-    def __init__(self, context, resource_path=None):
-        super(CommentCollection, self).__init__(context, Comment, resource_path)
+    def __init__(self, context):
+        super(VideoServiceManager, self).__init__(context, ResourcePath("SP.Publishing.VideoServiceManager"))
 
-    def delete_all(self):
-        """Deletes all the comments."""
-        return_type = ClientResult(self.context)
-        qry = ServiceOperationQuery(self, "DeleteAll", None, None, None, return_type)
+    def get_channels(self, start_index=0, limit=None):
+        return_type = VideoChannelCollection(self.context)
+        params = {"startIndex": start_index, "limit": limit}
+        qry = ServiceOperationQuery(self, "GetChannels", params, None, None, return_type)
         self.context.add_query(qry)
         return return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/comment.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/comment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/comments/information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/comments/information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/store_proxy.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/store_proxy.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/compliance/tag.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/compliance/tag.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/hub.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/hub.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/models/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/models/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contentcenter/machinelearning/samples/entity_data.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contentcenter/machinelearning/samples/entity_data.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/content_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/content_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/content_type_id.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/content_type_id.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/fieldlinks/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/fieldlinks/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/contenttypes/fieldlinks/field_link.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/contenttypes/fieldlinks/field_link.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/customactions/action.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/customactions/action.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/group.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/helper.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/helper.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/session.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/session.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/directory/user.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/directory/user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/documentmanagement/document_id.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/documentmanagement/document_id.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/documentmanagement/document_set.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/documentmanagement/document_set.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/definition.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/definition.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/eventreceivers/definition_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/eventreceivers/definition_collection.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from office365.runtime.paths.service_operation import ServiceOperationPath
 from office365.sharepoint.base_entity_collection import BaseEntityCollection
 from office365.sharepoint.eventreceivers.definition import EventReceiverDefinition
 
 
 class EventReceiverDefinitionCollection(BaseEntityCollection):
+    """
+    Represents a collection of SP.EventReceiverDefinition objects that are used to enumerate the list of
+    registered event receivers for Windows SharePoint Services objects that can have events.
+    """
 
     def __init__(self, context, resource_path=None, parent=None):
         """Represents a collection of SP.EventReceiverDefinition objects that are used to enumerate the list of
         registered event receivers for Windows SharePoint Services objects that can have events."""
         super(EventReceiverDefinitionCollection, self).__init__(context, EventReceiverDefinition, resource_path, parent)
 
     def get_by_id(self, event_receiver_id):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/excel/excel_rest.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/excel/excel_rest.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/definitions/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/definitions/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/features/feature.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/features/feature.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/add_field_options.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/add_field_options.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/calculated.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/calculated.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/currency.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/currency.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/date_time.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/date_time.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/field.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/field.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/geolocation_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/geolocation_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/image_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/image_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/lookup.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/lookup.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/lookup_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/lookup_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_choice.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_choice.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/multi_line_text.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/multi_line_text.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/number.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/number.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/rating_scale.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/rating_scale.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/related_field.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/related_field.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/related_field_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/related_field_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/text.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/text.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/url_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/url_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/user.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/user_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/user_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/fields/xmlSchemaFieldCreationInformation.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/fields/xmlSchemaFieldCreationInformation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/checked_out_file.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/checked_out_file.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/checked_out_file_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/checked_out_file_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/file.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,20 @@
         """Removes the file from content approval or unpublish a major version.
 
         :type comment: str
         """
         qry = ServiceOperationQuery(self, "unpublish", {"comment": comment})
         self.context.add_query(qry)
         return self
+    
+    def check_access_and_post_view_audit_event(self):
+        return_type = ClientResult(self.context, bool())
+        qry = ServiceOperationQuery(self, "CheckAccessAndPostViewAuditEvent", return_type=return_type)
+        self.context.add_query(qry)
+        return return_type
 
     def checkout(self):
         """Checks out the file from a document library based on the check-out type."""
         qry = ServiceOperationQuery(self, "checkout")
         self.context.add_query(qry)
         return self
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/recent_file_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/recent_file_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/system_object_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/system_object_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/version.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/version.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/version_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/version_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/files/version_event.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/files/version_event.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/folders/folder.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/folders/folder.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/forms/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/forms/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/forms/form.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/forms/form.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/key_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/key_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/create_file.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/create_file.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/download_file.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/download_file.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/upload_file.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/upload_file.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/internal/queries/upload_session.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/internal/queries/upload_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,26 +16,29 @@
     if hasattr(path_or_file, 'read'):
         return create_upload_session_query(binding_type, path_or_file, chunk_size, chunk_uploaded, **kwargs)
     else:
         f = open(path_or_file, 'rb')
         return create_upload_session_query(binding_type, f, chunk_size, chunk_uploaded, True, **kwargs)
 
 
-def create_upload_session_query(binding_type, file_object, chunk_size, chunk_uploaded, force_close=False, **kwargs):
+def create_upload_session_query(binding_type, file_object, chunk_size, chunk_uploaded, force_close=False,
+                                file_size=None, file_name=None, **kwargs):
     """
     :type binding_type: office365.sharepoint.files.collection.FileCollection
     :type file_object: typing.IO
     :type chunk_size: int
     :type force_close: bool
     :type chunk_uploaded: (int, *)->None
+    :type file_size: int
+    :type file_name: str
     """
 
     upload_id = str(uuid.uuid4())
-    file_size = os.fstat(file_object.fileno()).st_size
-    file_name = os.path.basename(file_object.name)
+    file_size = file_size if file_size else os.fstat(file_object.fileno()).st_size
+    file_name = file_name if file_name else os.path.basename(file_object.name)
 
     def _read_next():
         return file_object.read(chunk_size)
 
     def _has_pending_read():
         bytes_read = file_object.tell()
         return bytes_read < file_size
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/likes/liked_by_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/likes/liked_by_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/caml/query.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/caml/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from office365.runtime.client_value import ClientValue
+from office365.sharepoint.listitems.collection_position import ListItemCollectionPosition
 from office365.sharepoint.views.scope import ViewScope
 
 
 class WhereElement(object):
     """Used within the context of a query to specify a filter."""
 
     def __str__(self):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/compliance_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/compliance_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/creation_information_using_path.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/creation_information_using_path.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/form_update_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/form_update_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/listitem.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/listitem.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/listitems/version.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/listitems/version.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/base_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/base_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/bloom_filter.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/creatable_item_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/creatable_item_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/creatables_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/creatables_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/currency.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/currency.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/currency_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/currency_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/list.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/list.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/render_data_parameters.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/render_data_parameters.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/template.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     Use the Web.ListTemplates property (section 3.2.5.143.1.2.13) to return a ListTemplateCollection
     (section 3.2.5.92) for a site collection. Use an indexer to return a single list definition or
     list template from the collection.
     """
 
     def get_global_schema_xml(self):
         """Retrieves the global schema.xml file."""
-        result = ClientResult(self.context)
-        qry = ServiceOperationQuery(self, "GetGlobalSchemaXml", None, None, None, result)
+        return_type = ClientResult(self.context)
+        qry = ServiceOperationQuery(self, "GetGlobalSchemaXml", None, None, None, return_type)
         self.context.add_query(qry)
-        return result
+        return return_type
 
     @property
     def internal_name(self):
         """Gets a value that specifies the identifier for the list template.
 
         :rtype: str or None
         """
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/template_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/template_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/lists/template_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/lists/template_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/logger/log_export.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/logger/log_export.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/app_metadata.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/app_metadata.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/app_metadata_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/app_metadata_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/accessor.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/accessor.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/sitecollection/appcatalog/allowed_items.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/sitecollection/appcatalog/allowed_items.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/marketplace/tenant/appcatalog/accessor.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/marketplace/tenant/appcatalog/accessor.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/microservice/manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/microservice/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         return_type = ClientResult(context)
         payload = {
             "payLoad": payload,
             "minutes": minutes,
             "properties": properties
         }
         manager = MicroServiceManager(context)
-        qry = ServiceOperationQuery(manager, "AddMicroserviceWorkItem", None, payload, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(manager, "AddMicroserviceWorkItem", None, payload, None, return_type, True)
         context.add_query(qry)
         return return_type
 
     @property
     def entity_type_name(self):
         return "SP.MicroService.MicroServiceManager"
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/home_site_navigation_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/home_site_navigation_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/menu_node.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/menu_node.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/menu_state.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/menu_state.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/metadata_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/metadata_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/navigation.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/navigation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/navigation_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/navigation_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/node.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/node.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/node_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/node_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/node_creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/node_creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/navigation/provider_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/navigation/provider_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/oauth/native_client.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/oauth/native_client.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/orgnewssite/api.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/orgnewssite/api.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/page_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/page_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/pages/wiki_page_creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/pages/wiki_page_creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/base_permissions.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/base_permissions.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/irm/settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/irm/settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/kind.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/kind.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/assignments/assignment.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/assignments/assignment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/assignments/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/assignments/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/roles/definitions/definition.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/roles/definitions/definition.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/permissions/securable_object.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/permissions/securable_object.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/policy/dlp_policy_tip.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/policy/dlp_policy_tip.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/creation_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/creation_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/creation_params.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/creation_params.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/groups/site_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/groups/site_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/home/service_context_builder.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/home/service_context_builder.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/hub_sites_utility.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/hub_sites_utility.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/list_contract.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/list_contract.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/linkedsites/manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/linkedsites/manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/mysite_recommendations.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/mysite_recommendations.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/organization_news.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/organization_news.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/orglabels/context_list.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/orglabels/context_list.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/rating_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/rating_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/creation_request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/creation_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/icon_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/icon_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/sites/manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/sites/manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/portal/theme_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/portal/theme_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/groups/group.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/groups/group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/principal.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/principal.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/source.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/source.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/id_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/id_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/principal/users/user.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/principal/users/user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/diagnostics/controller.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/diagnostics/controller.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/embed_data_v1.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/embed_data_v1.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/embed_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/embed_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/file_picker_options.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/file_picker_options.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/fields_data.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/fields_data.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/metadata.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/metadata.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/metadata_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/metadata_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/page.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/page.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/repost.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/repost.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/pages/service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/pages/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,15 @@
     def get_current_user_memberships(context, scenario=None):
         """
         :param office365.sharepoint.client_context.ClientContext context: Client context
         :param str scenario:
         """
         return_type = ClientResult(context, StringCollection())
         svc = SitePageService(context)
-        qry = ServiceOperationQuery(svc, "GetCurrentUserMemberships", None, None, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(svc, "GetCurrentUserMemberships", None, None, None, return_type, True)
         context.add_query(qry)
         return return_type
 
     @staticmethod
     def get_time_zone(context, city_name):
         """
         Gets time zone data for specified city.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/primary_city_time.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/primary_city_time.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/rich_sharing.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/rich_sharing.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/creation_request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/creation_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/sites/communication/site.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/sites/communication/site.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/channel.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/channel.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/item.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/publishing/video/item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/publishing/video/service_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/site_me_ta_info_provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from office365.runtime.client_result import ClientResult
 from office365.runtime.queries.service_operation import ServiceOperationQuery
-from office365.runtime.paths.resource_path import ResourcePath
 from office365.sharepoint.base_entity import BaseEntity
-from office365.sharepoint.publishing.video.channel_collection import VideoChannelCollection
 
 
-class VideoServiceManager(BaseEntity):
+class SiteMeTAInfoProvider(BaseEntity):
+    """"""
 
-    def __init__(self, context):
-        super(VideoServiceManager, self).__init__(context, ResourcePath("SP.Publishing.VideoServiceManager"))
-
-    def get_channels(self, start_index=0, limit=None):
-        return_type = VideoChannelCollection(self.context)
-        params = {"startIndex": start_index, "limit": limit}
-        qry = ServiceOperationQuery(self, "GetChannels", params, None, None, return_type)
+    def get_azure_container_sas_token(self):
+        return_type = ClientResult(self.context, str())
+        qry = ServiceOperationQuery(self, "GetAzureContainerSASToken", None, None, None, return_type)
         self.context.add_query(qry)
         return return_type
+
+    @property
+    def entity_type_name(self):
+        return "Microsoft.SharePoint.Client.Search.Administration.SiteMeTAInfoProvider"
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/pushnotifications/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/pushnotifications/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/pushnotifications/subscriber.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/pushnotifications/subscriber.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/item.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/item_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/item_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/recyclebin/query_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/recyclebin/query_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/reputationmodel/reputation.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/reputationmodel/reputation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/request_context.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/request_context.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/request_user_context.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/request_user_context.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/administration/document_crawl_log.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/administration/document_crawl_log.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/context_condition.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/context_condition.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/custom_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/custom_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/object_owner_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/object_owner_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/promoted_result_query_rule.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/promoted_result_query_rule.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/promoted_results_operations_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/promoted_results_operations_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/auto_completion.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/auto_completion.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/auto_completion_results.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/auto_completion_results.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/configuration.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/configuration.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/context.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/context.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/personal_result_suggestion.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/personal_result_suggestion.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/personalization_data.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/personalization_data.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/property.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/property.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/routing_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/routing_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/sort/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/sort/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/sort/sort.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/sort/sort.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query/suggestion_results.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query/suggestion_results.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/query_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/query_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/ranking_labeling.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/ranking_labeling.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/refinement_results.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/refinement_results.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/relevant_results.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/relevant_results.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/setting.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/setting.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/simple_data_table.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/simple_data_table.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/search/special_term_results.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/search/special_term_results.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/server_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/server_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,39 +15,36 @@
     @staticmethod
     def is_sharepoint_online(context):
         """
         :type context: office365.sharepoint.client_context.ClientContext
         """
         binding_type = ServerSettings(context)
         return_type = ClientResult(context)
-        qry = ServiceOperationQuery(binding_type, "IsSharePointOnline", None, None, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(binding_type, "IsSharePointOnline", None, None, None, return_type, True)
         context.add_query(qry)
         return return_type
 
     @staticmethod
     def get_blocked_file_extensions(context):
         """
         :type context: office365.sharepoint.client_context.ClientContext
         """
         binding_type = ServerSettings(context)
         return_type = ClientResult(context, StringCollection())
-        qry = ServiceOperationQuery(binding_type, "GetBlockedFileExtensions", None, None, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(binding_type, "GetBlockedFileExtensions", None, None, None, return_type, True)
         context.add_query(qry)
         return return_type
 
     @staticmethod
     def get_global_installed_languages(context, compatibility_level):
         """
         Gets a list of installed languages that are compatible with a given version of SharePoint.
 
         :type context: office365.sharepoint.client_context.ClientContext
         :param int compatibility_level: The value of the major SharePoint version to query for installed languages.
         """
         binding_type = ServerSettings(context)
         return_type = LanguageCollection(context)
         qry = ServiceOperationQuery(binding_type, "GetGlobalInstalledLanguages", [compatibility_level],
-                                    None, None, return_type)
-        qry.static = True
+                                    None, None, return_type, True)
         context.add_query(qry)
         return return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/ability_status.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/ability_status.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/document_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/document_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/invitation/link.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/invitation/link.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/link_abilities.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/link_abilities.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/access_request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/access_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/kind.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/kind.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/share_request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/share_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/links/share_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/links/share_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/object_sharing_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/object_sharing_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/object_sharing_information_user.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/object_sharing_information_user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/object_sharing_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/object_sharing_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/operation_status_code.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/operation_status_code.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/permission_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/permission_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/personal_web.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/personal_web.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/picker_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/sharepoint_sharing_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,22 @@
+from office365.runtime.paths.resource_path import ResourcePath
 from office365.sharepoint.base_entity import BaseEntity
-from office365.sharepoint.ui.applicationpages.peoplepicker.query_settings import PeoplePickerQuerySettings
+from office365.sharepoint.sharing.picker_settings import PickerSettings
 
 
-class PickerSettings(BaseEntity):
-    """
-    This class contains configuration settings for the client people picker control hosted
-    by the SharePoint sharing UI.
-    """
+class SharePointSharingSettings(BaseEntity):
+    """This class contains the SharePoint UI-specific sharing settings."""
 
     @property
-    def allow_email_addresses(self):
-        """
-        Boolean value indicating whether the picker control will allow the resolution of arbitrary email addresses.
-        """
-        return self.properties.get("AllowEmailAddresses", None)
+    def picker_properties(self):
+        """An object containing the necessary information to initialize a client people picker control used
+        to search for and resolve desired users and groups."""
+        return self.properties.get('PickerProperties',
+                                   PickerSettings(self.context, ResourcePath("PickerProperties", self.resource_path)))
 
-    @property
-    def allow_only_email_addresses(self):
-        """
-        Boolean value indicating whether the picker control will only allow the resolution of email addresses.
-        """
-        return self.properties.get("AllowOnlyEmailAddresses", None)
-
-    @property
-    def query_settings(self):
-        """
-        The query settings to be used by the picker control.
-        """
-        return self.properties.get("QuerySettings", PeoplePickerQuerySettings())
+    def get_property(self, name, default_value=None):
+        if default_value is None:
+            property_mapping = {
+                "PickerProperties": self.picker_properties,
+            }
+            default_value = property_mapping.get(name, None)
+        return super(SharePointSharingSettings, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/role_type.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/role_type.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/securable_object_extensions.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/securable_object_extensions.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/site_sharing_report_helper.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/site_sharing_report_helper.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/user_directory_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/user_directory_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/user_role_assignment.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/user_role_assignment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/user_sharing_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/user_sharing_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sharing/utility.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sharing/utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     def get_user_directory_info_by_email(context, email):
         """
         Get user information by the user’s email address in directory.
 
         :param str email: The email address of a user.
         :param office365.sharepoint.client_context.ClientContext context: SharePoint client context
         """
-        result = ClientResult(context, UserDirectoryInfo())
+        return_type = ClientResult(context, UserDirectoryInfo())
         payload = {
             "email": email
         }
         utility = SharingUtility(context)
-        qry = ServiceOperationQuery(utility, "GetUserDirectoryInfoByEmail", None, payload, None, result)
+        qry = ServiceOperationQuery(utility, "GetUserDirectoryInfoByEmail", None, payload, None, return_type)
         qry.static = True
         context.add_query(qry)
-        return result
+        return return_type
 
     @staticmethod
     def validate_same_user_emails(context, primary_email, other_email, principal_name):
         """
         Validate the primary email/principal name and other email are of the same user.
 
         :param str primary_email: User’s primary email address
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitedesigns/creation_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitedesigns/creation_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitehealth/summary.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitehealth/summary.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/language_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/language_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/site.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/site.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/sph_site.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/sph_site.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sites/usage_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sites/usage_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/serialization_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/serialization_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/sitescripts/utility.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/sitescripts/utility.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/actor_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/actor_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/announcement_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/announcement_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/feed.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/feed.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from office365.runtime.client_result import ClientResult
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.sharepoint.base_entity import BaseEntity
 from office365.sharepoint.social.actor import SocialActor
 from office365.sharepoint.social.attachment import SocialAttachment
+from office365.sharepoint.social.feed.feed import SocialFeed
 from office365.sharepoint.social.thread import SocialThread
 
 
 class SocialFeedManager(BaseEntity):
     """The SocialFeedManager class provides access to social feeds. It provides methods to create posts,
     delete posts, read posts, and perform other operations on posts."""
 
@@ -59,14 +60,34 @@
         """
         return_type = ClientResult(self.context, SocialAttachment())
         payload = {"name": name, "description": description, "fileData": file_data}
         qry = ServiceOperationQuery(self, "CreateFileAttachment", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
+    def get_feed(self, feed_type=None, options=None):
+        """
+        The GetFeed method returns a feed for the current user. The feed consists of an array of message threads.
+        Each thread consists of a root post and an array of reply posts. See section 3.1.5.17 for details on
+        the SocialFeed type. The server selects a set of posts to return in the feed based on the type
+        and options parameters, but this protocol does require any specific algorithm to select the set of posts
+        from all posts that meet the specified type and options.
+
+        :param int feed_type: Specifies the type of feed to be returned. Feeds can be viewed using a personal view, news
+            view, timeline view, or likes view. If the type is not specified, GetFeed returns the news view.
+        :param SocialFeedOptions options: Specifies the maximum number of threads to get in the feed, the sort order
+            of the threads, and how the threads are to be selected based on the date and time that the threads were
+            created.
+        """
+        return_type = ClientResult(self.context, SocialFeed())
+        payload = {"type": feed_type, "options": options}
+        qry = ServiceOperationQuery(self, "GetFeed", None, payload, None, return_type)
+        self.context.add_query(qry)
+        return return_type
+
     @property
     def owner(self):
         """The Owner property returns the current user."""
         return self.properties.get("Owner", SocialActor())
 
     @property
     def personal_site_portal_uri(self):
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/rest.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/rest.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/feed/rest_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/feed/rest_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/following/manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/following/manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/following/rest_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/following/rest_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/creation_data.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/creation_data.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/post.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/post.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/posts/reference.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/posts/reference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from office365.runtime.client_value import ClientValue
 from office365.sharepoint.social.posts.post import SocialPost
-from office365.sharepoint.social.thread import SocialThread
 
 
 class SocialPostReference(ClientValue):
     """The SocialPostReference class specifies a reference to a post in another thread.  The referenced post can be a
     post with a tag, a post that is liked, a post that mentions a user, or a post that is a reply. Threads that contain
     a SocialPostReference in the PostReference property (see section 3.1.5.42.1.1.6) are threads with root posts that
     are generated on the server and not created by a client."""
 
-    def __init__(self, digest=SocialThread(), post=SocialPost(), thread_id=None, thread_owner_index=None):
+    def __init__(self, digest=None, post=SocialPost(), thread_id=None, thread_owner_index=None):
         """
         :param SocialThread digest: The Digest property provides a digest of the thread containing the referenced post.
         :param SocialPost post: The Post property provides access to the post being referenced
         :param str thread_id: The ThreadId property specifies the unique identifier of the thread containing the
             referenced post.
         :param int thread_owner_index: The ThreadOwnerIndex property specifies the current owner of the thread as an
             index into the SocialThread Actors array
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/rest_actor.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/rest_actor.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/rest_thread.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/rest_thread.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/switch.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/switch.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/social/thread.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/social/thread.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/storagemetrics/storage_metrics.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/storagemetrics/storage_metrics.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/create_xml_parameters.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/create_xml_parameters.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/field.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/field.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/field_value.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/field_value.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/group.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/group.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/item.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/item_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/item_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/set.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/set.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/taxonomy/store.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/taxonomy/store.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/teams/channel_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/teams/channel_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/collaboration/insights_data.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/collaboration/insights_data.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/hub_site.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/hub_site.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/hubsites/properties.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/hubsites/properties.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/response_message_center.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/response_message_center.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/secondary_administrators_fields_data.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/secondary_administrators_fields_data.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/settings_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/settings_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/sharing_capabilities.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/sharing_capabilities.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_collection_management_service.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_collection_management_service.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_creation_properties.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_creation_properties.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_creation_source.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_creation_source.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_properties.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_properties.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_properties_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_properties_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/site_properties_enumerable_filter.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/site_properties_enumerable_filter.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/spo_operation.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/spo_operation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/administration/tenant.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/administration/tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,25 @@
 
     def get_home_sites_details(self):
         return_type = ClientResult(self.context, ClientValueCollection(HomeSitesDetails))
         qry = ServiceOperationQuery(self, "GetHomeSitesDetails", None, None, None, return_type)
         self.context.add_query(qry)
         return return_type
 
-    def remove_home_site(self):
+    def remove_home_site(self, home_site_url):
         """
+        Remove home site
+
+        :param str home_site_url:
         """
-        return_type = ClientResult(self.context, str())
-        qry = ServiceOperationQuery(self, "RemoveSPHSite", None, None, None, return_type)
+        payload = {"homeSiteUrl": home_site_url}
+        qry = ServiceOperationQuery(self, "RemoveHomeSite", None, payload)
         self.context.add_query(qry)
-        return return_type
+        return self
+
 
     def has_valid_education_license(self):
         """"""
         return_type = ClientResult(self.context, bool())
         qry = ServiceOperationQuery(self, "HasValidEducationLicense", None, None, None, return_type)
         self.context.add_query(qry)
         return return_type
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/externalusers/results/get.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/externalusers/results/get.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/management/office365_tenant.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/management/office365_tenant.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/tenant/settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/tenant/settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/item_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/item_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/notification_recipient.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/notification_recipient.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/notification_recipient_set_request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/notification_recipient_set_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/notification_recipient_users.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/notification_recipient_users.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/status_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/status_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/sync_translator.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/sync_translator.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/user_resource.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/user_resource.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/translation/variations_timer_job.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/translation/variations_timer_job.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/types/resource_path.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/types/resource_path.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/entity_information_request.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/entity_information_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/query_parameters.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/query_parameters.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/query_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/query_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/ui/applicationpages/peoplepicker/web_service_interface.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/ui/applicationpages/peoplepicker/web_service_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,14 @@
     PickerEntityInformationRequest
 from office365.sharepoint.ui.applicationpages.peoplepicker.query_parameters import ClientPeoplePickerQueryParameters
 
 
 class ClientPeoplePickerWebServiceInterface(BaseEntity):
     """Specifies an interface that can be used to query principals."""
 
-    def __init__(self, context):
-        super(ClientPeoplePickerWebServiceInterface, self).__init__(context)
-
     @staticmethod
     def get_search_results(context, search_pattern, provider_id=None, hierarchy_node_id=None, entity_types=None):
         """
         Specifies a JSON formatted CSOM String of principals found in the search.
 
         :type context: office365.sharepoint.client_context.ClientContext
         :param str search_pattern: Specifies a pattern used to search for principals.
@@ -111,15 +108,15 @@
         request = PickerEntityInformationRequest(email_address=email_address)
         return_type = PickerEntityInformation(context)
         svc = ClientPeoplePickerWebServiceInterface(context)
         qry = ServiceOperationQuery(svc, "GetPickerEntityInformation",
                                     None,
                                     request,
                                     "entityInformationRequest",
-                                    return_type)
-        qry.static = True
+                                    return_type,
+                                    True)
         context.add_query(qry)
         return return_type
 
     @property
     def entity_type_name(self):
         return "SP.UI.ApplicationPages.ClientPeoplePickerWebServiceInterface"
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/usercustomactions/action.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/usercustomactions/action.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/usercustomactions/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/usercustomactions/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/follow_result.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/follow_result.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/followed_content.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/followed_content.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/hash_tag.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/hash_tag.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/my_site_links.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/my_site_links.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/people_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/people_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,28 @@
         """Gets a collection of the 20 (or fewer) most popular hash tags over the past week.
         The returned collection is sorted in descending order of frequency of use.
 
         :type context: office365.sharepoint.client_context.ClientContext
         """
         return_type = HashTagCollection(context)
         manager = PeopleManager(context)
-        qry = ServiceOperationQuery(manager, "GetTrendingTags", None, None, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(manager, "GetTrendingTags", None, None, None, return_type, True)
         context.add_query(qry)
         return return_type
 
+    def get_user_onedrive_quota_max(self, account_name):
+        """
+        :param str account_name: Account name of the specified user.
+        """
+        return_type = ClientResult(self.context, int())
+        params = {"accountName": account_name}
+        qry = ServiceOperationQuery(self, "GetUserOneDriveQuotaMax", params, None, None, return_type)
+        self.context.add_query(qry)
+        return return_type
+
     def am_i_following(self, account_name):
         """
         Checks whether the current user is following the specified user.
 
         :param str account_name: Account name of the specified user.
         :return:
         """
@@ -71,15 +80,15 @@
         return return_type
 
     def get_user_information(self, account_name, site_id):
         """
         :param str account_name: Account name of the specified user.
         :param str site_id: Site Identifier.
         """
-        return_type = ClientResult(self.context)
+        return_type = ClientResult(self.context, dict())
         params = {"accountName": account_name, "siteId": site_id}
         qry = ServiceOperationQuery(self, "GetSPUserInformation", params, None, None, return_type)
         self.context.add_query(qry)
         return return_type
 
     def follow(self, account_name):
         """
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/person_properties.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/person_properties.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/personal_cache.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/personal_cache.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/profile_image_store.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/profile_image_store.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/profile_loader.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/profile_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     def get_profile_loader(context):
         """
         The GetProfileLoader method returns a profile loader.
 
         :type: office365.sharepoint.client_context.ClientContext context
         """
         return_type = ProfileLoader(context)
-        qry = ServiceOperationQuery(return_type, "GetProfileLoader", None, None, None, return_type)
-        qry.static = True
+        qry = ServiceOperationQuery(return_type, "GetProfileLoader", None, None, None, return_type, True)
         context.add_query(qry)
         return return_type
 
     @staticmethod
     def get_owner_user_profile(context):
         """
         Gets the user profile for the Site owner.
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/promoted_sites.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/promoted_sites.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/properties_for_user.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/properties_for_user.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/sharedwithme/document.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/sharedwithme/document.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/userprofiles/user_profile.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/userprofiles/user_profile.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/email_properties.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/email_properties.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/move_copy_options.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/move_copy_options.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/move_copy_util.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/move_copy_util.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/upload_status.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/upload_status.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/utilities/utility.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/utilities/utility.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/create_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/create_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/field_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/field_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/views/view.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/views/view.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/viva/employee_engagement.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/viva/employee_engagement.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from office365.runtime.client_result import ClientResult
-from office365.runtime.http.http_method import HttpMethod
 from office365.runtime.paths.resource_path import ResourcePath
+from office365.runtime.queries.function import FunctionQuery
 from office365.runtime.queries.service_operation import ServiceOperationQuery
 from office365.sharepoint.base_entity import BaseEntity
 from office365.sharepoint.viva.app_configuration import AppConfiguration
+from office365.sharepoint.viva.home import VivaHome
 
 
 class EmployeeEngagement(BaseEntity):
 
     def __init__(self, context):
         super(EmployeeEngagement, self).__init__(context, ResourcePath("SP.EmployeeEngagement"))
 
@@ -19,23 +20,22 @@
         payload = {"return return_type": override_language_code}
         qry = ServiceOperationQuery(self, "DashboardContent", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
     def viva_home_configuration(self):
         return_type = ClientResult(self.context, dict())
-        qry = ServiceOperationQuery(self, "VivaHomeConfiguration", None, None, None, return_type)
+        qry = FunctionQuery(self, "VivaHomeConfiguration", None, return_type)
         self.context.add_query(qry)
+        return return_type
 
-        def _construct_request(request):
-            """
-            :type request: office365.runtime.http.request_options.RequestOptions
-            """
-            request.method = HttpMethod.Get
-        self.context.before_execute(_construct_request)
+    def viva_home(self):
+        return_type = VivaHome(self.context)
+        qry = ServiceOperationQuery(self, "VivaHome",  return_type=return_type)
+        self.context.add_query(qry)
         return return_type
 
     @property
     def app_configuration(self):
         return self.properties.get("AppConfiguration",
                                    AppConfiguration(self.context, ResourcePath("AppConfiguration", self.resource_path)))
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/subscription.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/subscription.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/subscription_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/subscription_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webhooks/subscription_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webhooks/subscription_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/client/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/client/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/client/webpart.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/client/webpart.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/definition.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/definition.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/definition_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/definition_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/limited_manager.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/limited_manager.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webparts/personalization_scope.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webparts/personalization_scope.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
     def add(self, web_creation_information):
         """
         Create WebSite
 
         :type web_creation_information: office365.sharepoint.webs.creation_information.WebCreationInformation
         """
-        target_web = Web(self.context)
-        self.add_child(target_web)
-        qry = ServiceOperationQuery(self, "add", None, web_creation_information, "parameters", target_web)
+        return_type = Web(self.context)
+        self.add_child(return_type)
+        qry = ServiceOperationQuery(self, "add", None, web_creation_information, "parameters", return_type)
         self.context.add_query(qry)
-        return target_web
+        return return_type
 
     @property
     def resource_url(self):
         val = super(WebCollection, self).resource_url
         parent_web_url = self._parent.get_property("Url")
         if parent_web_url is not None:
             val = val.replace(self.context.service_root_url(), parent_web_url + '/_api')
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/context_web_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/context_web_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/information_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/information_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/multilingual_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/multilingual_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/regional_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/regional_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/remote_web.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/remote_web.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/subweb_query.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/subweb_query.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/template.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/template.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/template_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/template_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/theme_info.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/theme_info.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/time_zone.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/time_zone.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/time_zone_information.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/time_zone_information.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/sharepoint/webs/web.py` & `Office365-REST-Python-Client-2.4.1/office365/sharepoint/webs/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from office365.sharepoint.pushnotifications.subscriber import PushNotificationSubscriber
 from office365.sharepoint.recyclebin.item_collection import RecycleBinItemCollection
 from office365.sharepoint.sharing.external_site_option import ExternalSharingSiteOption
 from office365.sharepoint.sharing.links.access_request import SharingLinkAccessRequest
 from office365.sharepoint.sharing.object_sharing_settings import ObjectSharingSettings
 from office365.sharepoint.sharing.links.data import SharingLinkData
 from office365.sharepoint.sharing.result import SharingResult
+from office365.sharepoint.sharing.shared_document_info import SharedDocumentInfo
 from office365.sharepoint.sitescripts.utility import SiteScriptUtility
 from office365.sharepoint.marketplace.sitecollection.appcatalog.accessor import SiteCollectionCorporateCatalogAccessor
 from office365.sharepoint.marketplace.tenant.appcatalog.accessor import TenantCorporateCatalogAccessor
 from office365.sharepoint.translation.user_resource import UserResource
 from office365.sharepoint.ui.applicationpages.peoplepicker.web_service_interface import (
     ClientPeoplePickerWebServiceInterface
 )
@@ -183,24 +184,24 @@
             user.ensure_property("LoginName", _user_loaded)
         else:
             qry = _create_query(user)
             self.context.add_query(qry)
         return return_type
 
     @staticmethod
-    def create_organization_sharing_link(context, url, is_edit_link):
+    def create_organization_sharing_link(context, url, is_edit_link=False):
         """ Creates and returns an organization-internal link that can be used to access a document and gain permissions
            to it.
 
         :param office365.sharepoint.client_context.ClientContext context:
         :param str url: he URL of the site, with the path of the object in SharePoint that is represented as query
             string parameters, forSharing set to 1 if sharing, and bypass set to 1 to bypass any mobile logic.
         :param bool is_edit_link: If true, the link will allow the logged in user to edit privileges on the item.
         """
-        return_type = ClientResult(context)
+        return_type = ClientResult(context, str())
         params = {"url": url, "isEditLink": is_edit_link}
         qry = ServiceOperationQuery(context.web, "CreateOrganizationSharingLink", None, params, None, return_type)
         qry.static = True
         context.add_query(qry)
         return return_type
 
     @staticmethod
@@ -314,14 +315,15 @@
         return_type = FlowSynchronizationResult(self.context)
         payload = {"category": category}
         qry = ServiceOperationQuery(self, "SyncFlowTemplates", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
     def get_all_client_side_components(self):
+        """"""
         return_type = ClientResult(self.context, str())
         qry = ServiceOperationQuery(self, "GetAllClientSideComponents", None, None, None, return_type)
         self.context.add_query(qry)
         return return_type
 
     def get_app_bdc_catalog(self):
         """
@@ -358,18 +360,21 @@
 
         :param int lcid: Specifies the language identifier to be added.
         """
         qry = ServiceOperationQuery(self, "AddSupportedUILanguage", {"lcid": lcid})
         self.context.add_query(qry)
         return self
 
-    def get_lists(self):
+    def get_lists(self, row_limit=100):
+        """
+        :param int row_limit: Specifies a limit for the number of lists in the query that are returned per page
+        """
         return_type = ListCollection(self.context)
         payload = {
-            "getListsParams": GetListsParameters()
+            "getListsParams": GetListsParameters(row_limit=row_limit)
         }
         qry = ServiceOperationQuery(self, "GetLists", None, payload, None, return_type)
         self.context.add_query(qry)
         return return_type
 
     def get_sub_webs_filtered_for_current_user(self, query):
         """Returns a collection of objects that contain metadata about subsites of the current site (2) in which the
@@ -1323,14 +1328,20 @@
         :param str source:
         """
         payload = {"title": title, "source": source}
         qry = ServiceOperationQuery(self, "SetGlobalNavSettings", None, payload)
         self.context.add_query(qry)
         return self
 
+    def sync_hub_site_theme(self):
+        """"""
+        qry = ServiceOperationQuery(self, "SyncHubSiteTheme")
+        self.context.add_query(qry)
+        return self
+
     def assign_document_id(self, site_prefix, enabled=True):
         """
         Assign Document IDs
 
         :param str site_prefix: Specify whether IDs will be automatically assigned to all documents in the
             Site Collection. Additionally, you can specify a set of 4-12 characters that will be used at the beginning
             of all IDs assigned for documents in this Site Collection, to help ensure that items in different
@@ -1468,14 +1479,20 @@
     def lists(self):
         """Specifies the collection of lists that are contained in the site available to the current user based on the
         current user's permissions."""
         return self.properties.get('Lists',
                                    ListCollection(self.context, ResourcePath("lists", self.resource_path)))
 
     @property
+    def onedrive_shared_items(self):
+        return self.properties.get('OneDriveSharedItems',
+                                   BaseEntityCollection(self.context, SharedDocumentInfo,
+                                                        ResourcePath("OneDriveSharedItems", self.resource_path)))
+
+    @property
     def site_users(self):
         """
         Specifies the collection of users in the site collection that contains the site
         """
         return self.properties.get('SiteUsers',
                                    UserCollection(self.context, ResourcePath("siteUsers", self.resource_path)))
 
@@ -1816,14 +1833,15 @@
                 "CurrentUser": self.current_user,
                 "DescriptionResource": self.description_resource,
                 "EffectiveBasePermissions": self.effective_base_permissions,
                 "EventReceivers": self.event_receivers,
                 "HostedApps": self.hosted_apps,
                 "ListTemplates": self.list_templates,
                 "MultilingualSettings": self.multilingual_settings,
+                "OneDriveSharedItems": self.onedrive_shared_items,
                 "ParentWeb": self.parent_web,
                 "PushNotificationSubscribers": self.push_notification_subscribers,
                 "RootFolder": self.root_folder,
                 "RegionalSettings": self.regional_settings,
                 "RoleDefinitions": self.role_definitions,
                 "RecycleBin": self.recycle_bin,
                 "SiteCollectionAppCatalog": self.site_collection_app_catalog,
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/subscriptions/change_notification.py` & `Office365-REST-Python-Client-2.4.1/office365/subscriptions/change_notification.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/subscriptions/change_notification_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/subscriptions/change_notification_collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/subscriptions/subscription.py` & `Office365-REST-Python-Client-2.4.1/office365/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/apps/app.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/apps/app.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/apps/definition.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/apps/definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.teams.bots.teamwork_bot import TeamworkBot
 
 
 class TeamsAppDefinition(Entity):
     """Represents the details of a version of a teamsApp."""
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/apps/installation.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/apps/installation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/apps/user_scope_installation.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/apps/user_scope_installation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/channels/channel.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/channels/channel.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/channels/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/channels/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/chats/chat.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/chats/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from office365.entity import Entity
 from office365.entity_collection import EntityCollection
 from office365.runtime.paths.resource_path import ResourcePath
 from office365.teams.apps.installation import TeamsAppInstallation
 from office365.teams.members.conversation import ConversationMember
 from office365.teams.chats.message import ChatMessage
 from office365.teams.operations.async_operation import TeamsAsyncOperation
+from office365.teams.tabs.tab import TeamsTab
 
 
 class Chat(Entity):
     """A chat is a collection of chatMessages between one or more participants. Participants can be users or apps."""
 
     @property
     def topic(self):
@@ -46,14 +47,20 @@
         """
         A collection of all the Teams async operations that ran or are running on the chat. Nullable.
         """
         return self.properties.get('operations',
                                    EntityCollection(self.context, TeamsAsyncOperation,
                                                     ResourcePath("operations", self.resource_path)))
 
+    @property
+    def tabs(self):
+        """A collection of all the tabs in the chat."""
+        return self.properties.get('tabs',
+                                   EntityCollection(self.context, TeamsTab, ResourcePath("tabs", self.resource_path)))
+
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
                 "installedApps": self.installed_apps
             }
             default_value = property_mapping.get(name, None)
         return super(Chat, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/chats/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/chats/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/chats/message.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/chats/message.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/chats/message_attachment.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/chats/message_attachment.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/collection.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/collection.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/guest_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/guest_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/member_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/member_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/members/aad_user_conversation.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/members/aad_user_conversation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/messaging_settings.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/messaging_settings.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/operations/async_operation.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/operations/async_operation.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/shifts/change_tracked_entity.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/shifts/change_tracked_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from office365.directory.identities.identity_set import IdentitySet
+from office365.directory.permissions.identity_set import IdentitySet
 from office365.entity import Entity
 
 
 class ChangeTrackedEntity(Entity):
     """Represents an entity to track changes made to any supported schedule and associated resource."""
 
     @property
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/shifts/preferences.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/shifts/preferences.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/shifts/schedule.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/shifts/schedule.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/shifts/schedule_change_request.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/shifts/schedule_change_request.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/shifts/shift.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/shifts/shift.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 class Shift(ChangeTrackedEntity):
     """
     Represents a unit of scheduled work in a shifts.
     """
 
     @property
     def draft_shift(self):
-        """The draft version of this shift that is viewable by managers.
+        """
+        The draft version of this shift that is viewable by managers.
+        """
+        return self.properties.get('draftShift', ShiftItem())
 
-        :rtype: ShiftItem
+    @property
+    def shared_shift(self):
+        """
+        The shared version of this shift that is viewable by both employees and managers.
         """
-        return self.get_property('draftShift', ShiftItem())
+        return self.properties.get('sharedShift', ShiftItem())
 
     def get_property(self, name, default_value=None):
         if default_value is None:
             property_mapping = {
                 "draftShift": self.draft_shift,
+                "sharedShift": self.shared_shift
             }
             default_value = property_mapping.get(name, None)
         return super(Shift, self).get_property(name, default_value)
```

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/shifts/shift_item.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/shifts/shift_item.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/tabs/tab.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/tabs/tab.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/team.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/team.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/teams/user_teamwork.py` & `Office365-REST-Python-Client-2.4.1/office365/teams/user_teamwork.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/todo/task.py` & `Office365-REST-Python-Client-2.4.1/office365/todo/tasks/task.py`

 * *Files identical despite different names*

### Comparing `Office365-REST-Python-Client-2.4.0/office365/todo/task_list_collection.py` & `Office365-REST-Python-Client-2.4.1/office365/todo/tasks/list_collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from office365.entity_collection import EntityCollection
-from office365.todo.task_list import TodoTaskList
+from office365.delta_collection import DeltaCollection
+from office365.todo.tasks.list import TodoTaskList
 
 
-class TodoTaskListCollection(EntityCollection):
+class TodoTaskListCollection(DeltaCollection):
 
     def __init__(self, context, resource_path=None):
         super(TodoTaskListCollection, self).__init__(context, TodoTaskList, resource_path)
 
     def add(self, display_name):
         """
         Create a new lists object.
```

### Comparing `Office365-REST-Python-Client-2.4.0/setup.py` & `Office365-REST-Python-Client-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with io.open("README.md", mode='r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="Office365-REST-Python-Client",
-    version="2.4.0",
+    version="2.4.1",
     author="Vadim Gremyachev",
     author_email="vvgrem@gmail.com",
     maintainer="Konrad Gądek, Domenico Di Nicola",
     maintainer_email="kgadek@gmail.com, dom.dinicola@gmail.com",
     description="Microsoft 365 & Microsoft Graph Library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

