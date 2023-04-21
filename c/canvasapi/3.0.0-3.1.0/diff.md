# Comparing `tmp/canvasapi-3.0.0.tar.gz` & `tmp/canvasapi-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvasapi-3.0.0.tar", last modified: Wed Sep 21 21:59:58 2022, max compression
+gzip compressed data, was "canvasapi-3.1.0.tar", last modified: Fri Apr 21 23:07:46 2023, max compression
```

## Comparing `canvasapi-3.0.0.tar` & `canvasapi-3.1.0.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:59:58.266841 canvasapi-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-09-21 21:59:56.000000 canvasapi-3.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-21 21:59:56.000000 canvasapi-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8504 2022-09-21 21:59:58.266841 canvasapi-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7552 2022-09-21 21:59:56.000000 canvasapi-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:59:58.262841 canvasapi-3.0.0/canvasapi/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    68508 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/appointment_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    21529 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/authentication_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/authentication_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/avatar.py
--rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/calendar_event.py
--rw-r--r--   0 runner    (1001) docker     (121)    50165 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/canvas_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/comm_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     7596 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/communication_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/content_export.py
--rw-r--r--   0 runner    (1001) docker     (121)    12170 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/content_migration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/conversation.py
--rw-r--r--   0 runner    (1001) docker     (121)    95996 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/course.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/course_epub_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/current_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     4777 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/custom_gradebook_columns.py
--rw-r--r--   0 runner    (1001) docker     (121)    22480 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/discussion_topic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/enrollment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/enrollment_term.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/eportfolio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/external_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)     4445 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/external_tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/favorite.py
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/feature.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/folder.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/grade_change_log.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/gradebook_history.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/grading_period.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/grading_standard.py
--rw-r--r--   0 runner    (1001) docker     (121)    40868 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/group.py
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/license.py
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     8462 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/module.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/notification_preference.py
--rw-r--r--   0 runner    (1001) docker     (121)    13736 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/outcome.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/outcome_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     8649 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/page.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/page_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/pairing_code.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/peer_review.py
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/planner.py
--rw-r--r--   0 runner    (1001) docker     (121)     6947 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/poll.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/poll_choice.py
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/poll_session.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/poll_submission.py
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)    32609 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/quiz.py
--rw-r--r--   0 runner    (1001) docker     (121)     4094 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/quiz_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     9261 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/requester.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/rubric.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)     6988 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/section.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/sis_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     7300 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/submission.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/tab.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/todo.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/usage_rights.py
--rw-r--r--   0 runner    (1001) docker     (121)    38136 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     7866 2022-09-21 21:59:56.000000 canvasapi-3.0.0/canvasapi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 21:59:58.266841 canvasapi-3.0.0/canvasapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8504 2022-09-21 21:59:58.000000 canvasapi-3.0.0/canvasapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-09-21 21:59:58.000000 canvasapi-3.0.0/canvasapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:59:58.000000 canvasapi-3.0.0/canvasapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 21:59:58.000000 canvasapi-3.0.0/canvasapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-21 21:59:58.000000 canvasapi-3.0.0/canvasapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-21 21:59:58.000000 canvasapi-3.0.0/canvasapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-21 21:59:58.266841 canvasapi-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1650 2022-09-21 21:59:56.000000 canvasapi-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:07:46.250545 canvasapi-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-21 23:07:43.000000 canvasapi-3.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-21 23:07:43.000000 canvasapi-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-21 23:07:46.250545 canvasapi-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-21 23:07:43.000000 canvasapi-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:07:46.250545 canvasapi-3.1.0/canvasapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70346 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/account_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/appointment_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/authentication_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/authentication_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/avatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/calendar_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50761 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/canvas_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/comm_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/communication_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/content_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/content_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96214 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/course.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/course_epub_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/course_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/custom_gradebook_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22480 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/discussion_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/enrollment_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/eportfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/external_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/external_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/grade_change_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/gradebook_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/grading_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/grading_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40859 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/notification_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14174 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/outcome_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/pairing_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/peer_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/poll_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/quiz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/quiz_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/rubric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/sis_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/todo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/usage_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38451 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-21 23:07:43.000000 canvasapi-3.1.0/canvasapi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 23:07:46.250545 canvasapi-3.1.0/canvasapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 23:07:46.000000 canvasapi-3.1.0/canvasapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-21 23:07:46.250545 canvasapi-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-21 23:07:43.000000 canvasapi-3.1.0/setup.py
```

### Comparing `canvasapi-3.0.0/AUTHORS.md` & `canvasapi-3.1.0/AUTHORS.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 - Catherine Abbruzzese [@cat0698](https://github.com/cat0698))
 - Cameron Cuff [@ctcuff](https://github.com/ctcuff)
 - Craig Thompson [@craigdsthompson](https://github.com/craigdsthompson)
 - Dalton Durst [@UniversalSuperBox](https://github.com/UniversalSuperBox)
 - Damian Sweeney [@damianfs](https://github.com/damianfs)
 - Daniel Brinkman [@DanBrink91](https://github.com/DanBrink91)
 - Daniel Grobani [@dgrobani](https://github.com/dgrobani)
+- Daniel Molares [@dmols](https://github.com/dmols)
 - David Warden [@dfwarden](https://github.com/dfwarden)
 - Davis Goff [@Goff-Davis](https://github.com/Goff-Davis)
 - Deundre Williams [@deundrewilliams](https://github.com/deundrewilliams)
 - Devin Singh [@devints47](https://github.com/devints47)
 - Dmitry Savransky [@dsavransky](https://github.com/dsavransky)
 - Elise Heron [@thedarkestknight](https://github.com/thedarkestknight)
 - Elli Howard [@qwertynerd97](https://github.com/qwertynerd97)
@@ -56,33 +57,37 @@
 - Jose Silveti [@jrsilveti](https://github.com/jrsilveti)
 - Joshua Salzedo [@theunkn0wn1](https://github.com/theunkn0wn1)
 - [@kailukaitisBrendan](https://github.com/kailukaitisBrendan)
 - Keegan Berry [@keeeeeegan](https://github.com/keeeeeegan)
 - Kenny Perez [@kennygperez](https://github.com/kennygperez)
 - [@kensler](https://github.com/kensler)
 - Lawrence Oks [@ljoks](https://github.com/ljoks)
+- Lee Fent [@lafent](https://github.com/lafent)
 - Leonard Camacho [@lcamacho](https://github.com/lcamacho)
+- Lucas Salas [@lucas-salas](https://github.com/lucas-salas)
 - Mark Lalor [@MarkLalor](https://github.com/MarkLalor)
 - Markus [@elec3647](https://github.com/elec3647)
 - Matthew Fedder [@matthewf-ucsd](https://github.com/matthewf-ucsd)
 - Matthew Jones [@jonespm](https://github.com/jonespm)
 - Michael Phelps [@nottheswimmer](https://github.com/nottheswimmer)
 - Mike Nahmias [@Mike-Nahmias](https://github.com/Mike-Nahmias)
+- Mike Suhan [@mikesuhan](https://github.com/mikesuhan)
 - Nathan Dabu [@nathaned](https://github.com/nathaned)
 - Petar Nikolovski [@petarGitNik](https://github.com/petarGitNik)
 - Philip Austin [@phaustin](https://github.com/phaustin)
 - Philip Carter [@phillyc](https://github.com/phillyc)
 - Ralph Baird [@rmanbaird](https://github.com/rmanbaird)
 - [@Screeeech](https://github.com/Screeeech)
 - Shane Rosenkrantz [@shaneros](https://github.com/shaneros)
 - Sigurður Baldursson [@sigurdurb](https://github.com/sigurdurb)
 - Spencer Rogers [@spencer1248](https://github.com/spencer1248)
 - Stephen Woosley [@stephenwoosley](https://github.com/stephenwoosley)
 - Steven Bell [@stevenbell](https://github.com/stevenbell)
 - Steven Williams [@onomou](https://github.com/onomou)
+- [@svanderwulp](https://github.com/svanderwulp)
 - Tinson Lai [@laitingsheng](https://github.com/laitingsheng)
 - Toan Vu [@vutoan1245](https://github.com/vutoan1245)
 - [@Tobiaqs](https://github.com/Tobiaqs)
 - Tuan Pham [@tuanvpham](https://github.com/tuanvpham)
 - Tyler Wallace [@wallacetyler](https://github.com/wallacetyler)
 - [@us91](https://github.com/us91)
 - Vishvak Seenichamy [@Vishvak365](https://github.com/Vishvak365)
```

### Comparing `canvasapi-3.0.0/LICENSE` & `canvasapi-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/PKG-INFO` & `canvasapi-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvasapi
-Version: 3.0.0
+Version: 3.1.0
 Summary: API wrapper for the Canvas LMS
 Home-page: https://github.com/ucfopen/canvasapi
 Author: University of Central Florida - Center for Distributed Learning
 Author-email: techrangers@ucf.edu
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `canvasapi-3.0.0/README.md` & `canvasapi-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/account.py` & `canvasapi-3.1.0/canvasapi/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,30 @@
+from canvasapi.account_calendar import AccountCalendar
+from canvasapi.authentication_event import AuthenticationEvent
+from canvasapi.authentication_provider import AuthenticationProvider
 from canvasapi.canvas_object import CanvasObject
+from canvasapi.content_migration import ContentMigration, Migrator
+from canvasapi.course import Course
+from canvasapi.course_event import CourseEvent
+from canvasapi.enrollment import Enrollment
+from canvasapi.enrollment_term import EnrollmentTerm
 from canvasapi.exceptions import CanvasException, RequiredFieldMissing
+from canvasapi.external_tool import ExternalTool
 from canvasapi.feature import Feature, FeatureFlag
 from canvasapi.grading_period import GradingPeriod
 from canvasapi.grading_standard import GradingStandard
+from canvasapi.group import Group, GroupCategory
+from canvasapi.login import Login
+from canvasapi.outcome import OutcomeGroup, OutcomeLink
 from canvasapi.outcome_import import OutcomeImport
 from canvasapi.paginated_list import PaginatedList
 from canvasapi.rubric import Rubric
+from canvasapi.scope import Scope
 from canvasapi.sis_import import SisImport
+from canvasapi.user import User
 from canvasapi.util import combine_kwargs, file_or_path, obj_or_id, obj_or_str
 
 
 class Account(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.name, self.id)
 
@@ -58,16 +72,14 @@
         Add external authentication providers for the account
 
         :calls: `POST /api/v1/accounts/:account_id/authentication_providers \
         <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.create>`_
 
         :rtype: :class:`canvasapi.authentication_provider.AuthenticationProvider`
         """
-        from canvasapi.authentication_provider import AuthenticationProvider
-
         response = self._requester.request(
             "POST",
             "accounts/{}/authentication_providers".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         authentication_providers_json = response.json()
         authentication_providers_json.update({"account_id": self.id})
@@ -119,16 +131,14 @@
         :param user: The user object or ID to close the notificaton for.
         :type user: :class:`canvasapi.user.User` or int
         :param notification: The notification object or ID to close.
         :type notification: :class:`canvasapi.account.AccountNotification` or int
 
         :rtype: :class:`canvasapi.account.AccountNotification`
         """
-        from canvasapi.user import User
-
         user_id = obj_or_id(user, "user", (User,))
         notif_id = obj_or_id(notification, "notification", (AccountNotification,))
 
         response = self._requester.request(
             "DELETE",
             "accounts/{}/users/{}/account_notifications/{}".format(
                 self.id, user_id, notif_id
@@ -161,16 +171,14 @@
         <https://canvas.instructure.com/doc/api/admins.html#method.admins.create>`_
 
         :param user: The user object or ID to promote to admin.
         :type user: :class:`canvasapi.user.User` or int
 
         :rtype: :class:`canvasapi.account.Admin`
         """
-        from canvasapi.user import User
-
         user_id = obj_or_id(user, "user", (User,))
         kwargs["user_id"] = user_id
 
         response = self._requester.request(
             "POST",
             "accounts/{}/admins".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
@@ -185,16 +193,14 @@
         <https://canvas.instructure.com/doc/api/content_migrations.html#method.content_migrations.create>`_
 
         :param migration_type: The migrator type to use in this migration
         :type migration_type: str or :class:`canvasapi.content_migration.Migrator`
 
         :rtype: :class:`canvasapi.content_migration.ContentMigration`
         """
-        from canvasapi.content_migration import ContentMigration, Migrator
-
         if isinstance(migration_type, Migrator):
             kwargs["migration_type"] = migration_type.type
         elif isinstance(migration_type, str):
             kwargs["migration_type"] = migration_type
         else:
             raise TypeError("Parameter migration_type must be of type Migrator or str")
 
@@ -214,16 +220,14 @@
         Create a course.
 
         :calls: `POST /api/v1/accounts/:account_id/courses \
         <https://canvas.instructure.com/doc/api/courses.html#method.courses.create>`_
 
         :rtype: :class:`canvasapi.course.Course`
         """
-        from canvasapi.course import Course
-
         response = self._requester.request(
             "POST",
             "accounts/{}/courses".format(self.id),
             account_id=self.id,
             _kwargs=combine_kwargs(**kwargs),
         )
         return Course(self._requester, response.json())
@@ -233,16 +237,14 @@
         Create an enrollment term.
 
         :calls: `POST /api/v1/accounts/:account_id/terms \
         <https://canvas.instructure.com/doc/api/enrollment_terms.html#method.terms.create>`_
 
         :rtype: :class:`canvasapi.enrollment_term.EnrollmentTerm`
         """
-        from canvasapi.enrollment_term import EnrollmentTerm
-
         response = self._requester.request(
             "POST",
             "accounts/{}/terms".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         enrollment_term_json = response.json()
         enrollment_term_json.update({"account_id": self.id})
@@ -265,16 +267,14 @@
         :type privacy_level: str
         :param consumer_key: The consumer key for the external tool
         :type consumer_key: str
         :param shared_secret: The shared secret with the external tool
         :type shared_secret: str
         :rtype: :class:`canvasapi.external_tool.ExternalTool`
         """
-        from canvasapi.external_tool import ExternalTool
-
         response = self._requester.request(
             "POST",
             "accounts/{}/external_tools".format(self.id),
             name=name,
             privacy_level=privacy_level,
             consumer_key=consumer_key,
             shared_secret=shared_secret,
@@ -292,16 +292,14 @@
         :calls: `POST /api/v1/accounts/:account_id/group_categories \
         <https://canvas.instructure.com/doc/api/group_categories.html#method.group_categories.create>`_
 
         :param name: Name of group category.
         :type name: str
         :rtype: :class:`canvasapi.group.GroupCategory`
         """
-        from canvasapi.group import GroupCategory
-
         response = self._requester.request(
             "POST",
             "accounts/{}/group_categories".format(self.id),
             name=name,
             _kwargs=combine_kwargs(**kwargs),
         )
         return GroupCategory(self._requester, response.json())
@@ -322,18 +320,16 @@
             (x in account_notification for x in required_key_list)
         )
 
         if isinstance(account_notification, dict) and required_keys_present:
             kwargs["account_notification"] = account_notification
         else:
             raise RequiredFieldMissing(
-                (
-                    "account_notification must be a dictionary with keys "
-                    "'subject', 'message', 'start_at', and 'end_at'."
-                )
+                "account_notification must be a dictionary with keys "
+                "'subject', 'message', 'start_at', and 'end_at'."
             )
 
         response = self._requester.request(
             "POST",
             "accounts/{}/account_notifications".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -351,15 +347,14 @@
         <https://canvas.instructure.com/doc/api/account_reports.html#method.account_reports.create>`_
 
         :param report_type: The type of report.
         :type report_type: str
 
         :rtype: :class:`canvasapi.account.AccountReport`
         """
-
         response = self._requester.request(
             "POST",
             "accounts/{}/reports/{}".format(self.id, report_type),
             _kwargs=combine_kwargs(**kwargs),
         )
 
         response_json = response.json()
@@ -394,15 +389,14 @@
         <https://canvas.instructure.com/doc/api/sis_imports.html#method.sis_imports_api.create>`_
 
         :param attachment: A file handler or path of the file to import.
         :type attachment: file or str
 
         :rtype: :class:`canvasapi.sis_import.SisImport`
         """
-
         attachment, is_path = file_or_path(attachment)
 
         try:
             response = self._requester.request(
                 "POST",
                 "accounts/{}/sis_imports".format(self.id),
                 file={"attachment": attachment},
@@ -448,16 +442,14 @@
         :calls: `POST /api/v1/accounts/:account_id/users \
         <https://canvas.instructure.com/doc/api/users.html#method.users.create>`_
 
         :param pseudonym: The pseudonym of the account.
         :type pseudonym: dict
         :rtype: :class:`canvasapi.user.User`
         """
-        from canvasapi.user import User
-
         if isinstance(pseudonym, dict) and "unique_id" in pseudonym:
             kwargs["pseudonym"] = pseudonym
         else:
             raise RequiredFieldMissing("Dictionary with key 'unique_id' is required.")
 
         response = self._requester.request(
             "POST",
@@ -475,26 +467,24 @@
 
         :param user: The attributes of the user to create a login for
         :type user: `dict`
         :param login: The attributes of the login to create
         :type login: `dict`
         :rtype: :class:`canvasapi.login.Login`
         """
-        from canvasapi.login import Login
-
         if isinstance(user, dict) and "id" in user:
             kwargs["user"] = user
         else:
-            raise RequiredFieldMissing(("user must be a dictionary with keys " "'id'."))
+            raise RequiredFieldMissing("user must be a dictionary with keys 'id'.")
 
         if isinstance(login, dict) and "unique_id" in login:
             kwargs["login"] = login
         else:
             raise RequiredFieldMissing(
-                ("login must be a dictionary with keys " "'unique_id'.")
+                "login must be a dictionary with keys 'unique_id'."
             )
 
         response = self._requester.request(
             "POST",
             "accounts/{}/logins".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -553,16 +543,14 @@
         <https://canvas.instructure.com/doc/api/admins.html#method.admins.destroy>`_
 
         :param user: The user object or ID to remove as admin.
         :type user: :class:`canvasapi.user.User` or int
 
         :rtype: :class:`canvasapi.account.Admin`
         """
-        from canvasapi.user import User
-
         user_id = obj_or_id(user, "user", (User,))
         kwargs["user_id"] = user_id
 
         response = self._requester.request(
             "DELETE",
             "accounts/{}/admins/{}".format(self.id, user_id),
             _kwargs=combine_kwargs(**kwargs),
@@ -612,25 +600,41 @@
         <https://canvas.instructure.com/doc/api/accounts.html#method.accounts.remove_user>`_
 
         :param user: The user object or ID to delete.
         :type user: :class:`canvasapi.user.User` or int
 
         :rtype: :class:`canvasapi.user.User`
         """
-        from canvasapi.user import User
-
         user_id = obj_or_id(user, "user", (User,))
 
         response = self._requester.request(
             "DELETE",
             "accounts/{}/users/{}".format(self.id, user_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return User(self._requester, response.json())
 
+    def get_account_calendar(self, **kwargs):
+        """
+        Returns information about a single account calendar.
+
+        :calls: `GET /api/v1/account_calendars/:account_id \
+        <https://canvas.instructure.com/doc/api/account_calendars.html#method.account_calendars_api.show>`_
+
+        :rtype: :class:`canvasapi.account_calendar.AccountCalendar`
+        """
+
+        response = self._requester.request(
+            "GET",
+            "account_calendars/{}".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        return AccountCalendar(self._requester, response.json())
+
     def get_admins(self, **kwargs):
         """
         Get the paginated list of admins for the current account.
 
         :calls: `GET /api/v1/accounts/:account_id/admins \
         <https://canvas.instructure.com/doc/api/admins.html#method.admins.index>`_
 
@@ -641,27 +645,44 @@
             Admin,
             self._requester,
             "GET",
             "accounts/{}/admins".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
+    def get_all_account_calendars(self, **kwargs):
+        """
+        Lists all account calendars available to the account given.
+
+        :calls: `GET /api/v1/accounts/:account_id/account_calendars \
+        <https://canvas.instructure.com/doc/api/account_calendars.html#method.account_calendars_api.all_calendars>`_
+
+        :returns: Paginated list of all account calendars for the provided account.
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.account_calendar.AccountCalendar`
+        """
+        return PaginatedList(
+            AccountCalendar,
+            self._requester,
+            "GET",
+            "accounts/{}/account_calendars".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def get_all_outcome_links_in_context(self, **kwargs):
         """
         Get all outcome links for context - BETA
 
         :calls: `GET /api/v1/accounts/:account_id/outcome_group_links \
         <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.link_index>`_
 
         :returns: Paginated List of OutcomesLinks in the context.
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.outcome.OutcomeLink`
         """
-        from canvasapi.outcome import OutcomeLink
-
         return PaginatedList(
             OutcomeLink,
             self._requester,
             "GET",
             "accounts/{}/outcome_group_links".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -672,16 +693,14 @@
 
         :calls: `GET /api/v1/audit/authentication/accounts/:account_id \
         <https://canvas.instructure.com/doc/api/authentications_log.html#method.authentication_audit_api.for_account>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
                 :class:`canvasapi.authentication_event.AuthenticationEvent`
         """
-        from canvasapi.authentication_event import AuthenticationEvent
-
         return PaginatedList(
             AuthenticationEvent,
             self._requester,
             "GET",
             "audit/authentication/accounts/{}".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -695,16 +714,14 @@
 
         :param authentication_provider: The object or ID of the authentication provider
         :type authentication_provider:
             :class:`canvasapi.authentication_provider.AuthenticationProvider` or int
 
         :rtype: :class:`canvasapi.authentication_provider.AuthenticationProvider`
         """
-        from canvasapi.authentication_provider import AuthenticationProvider
-
         authentication_providers_id = obj_or_id(
             authentication_provider,
             "authentication provider",
             (AuthenticationProvider,),
         )
 
         response = self._requester.request(
@@ -723,16 +740,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/authentication_providers \
         <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.authentication_provider.AuthenticationProvider`
         """
-        from canvasapi.authentication_provider import AuthenticationProvider
-
         return PaginatedList(
             AuthenticationProvider,
             self._requester,
             "GET",
             "accounts/{}/authentication_providers".format(self.id),
             {"account_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
@@ -746,16 +761,14 @@
         <https://canvas.instructure.com/doc/api/content_migrations.html#method.content_migrations.show>`_
 
         :param content_migration: The object or ID of the content migration to retrieve.
         :type contnet_migration: int, str or :class:`canvasapi.content_migration.ContentMigration`
 
         :rtype: :class:`canvasapi.content_migration.ContentMigration`
         """
-        from canvasapi.content_migration import ContentMigration
-
         migration_id = obj_or_id(
             content_migration, "content_migration", (ContentMigration,)
         )
 
         response = self._requester.request(
             "GET",
             "accounts/{}/content_migrations/{}".format(self.id, migration_id),
@@ -773,16 +786,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/content_migrations/ \
         <https://canvas.instructure.com/doc/api/content_migrations.html#method.content_migrations.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.content_migration.ContentMigration`
         """
-        from canvasapi.content_migration import ContentMigration
-
         return PaginatedList(
             ContentMigration,
             self._requester,
             "GET",
             "accounts/{}/content_migrations".format(self.id),
             {"account_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
@@ -794,16 +805,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/courses \
         <https://canvas.instructure.com/doc/api/accounts.html#method.accounts.courses_api>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.course.Course`
         """
-        from canvasapi.course import Course
-
         return PaginatedList(
             Course,
             self._requester,
             "GET",
             "accounts/{}/courses".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -813,15 +822,14 @@
         Return the distribution of all concluded grades in the default term
 
         :calls: `GET /api/v1/accounts/:account_id/analytics/completed/grades \
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_grades>`_
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/completed/grades".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -830,15 +838,14 @@
         Return the distribution of all available grades in the default term
 
         :calls: `GET /api/v1/accounts/:account_id/analytics/current/grades \
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_grades>`_
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/current/grades".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -850,15 +857,14 @@
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_grades>`_
 
         :param term_id: The ID of the term, or the strings "current" or "completed"
         :type term_id: int or str
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/terms/{}/grades".format(self.id, term_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -867,15 +873,14 @@
         Return page view hits all concluded courses in the default term
 
         :calls: `GET /api/v1/accounts/:account_id/analytics/completed/activity \
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_participation>`_
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/completed/activity".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -884,15 +889,14 @@
         Return page view hits all available courses in the default term
 
         :calls: `GET /api/v1/accounts/:account_id/analytics/current/activity \
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_participation>`_
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/current/activity".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -906,15 +910,14 @@
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_participation>`_
 
         :param term_id: The ID of the term, or the strings "current" or "completed"
         :type term_id: int or str
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/terms/{}/activity".format(self.id, term_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -923,15 +926,14 @@
         Return all available numeric statistics about the department in the default term
 
         :calls: `GET /api/v1/accounts/:account_id/analytics/current/statistics \
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_statistics>`_
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/completed/statistics".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -940,15 +942,14 @@
         Return all available numeric statistics about the department in the default term
 
         :calls: `GET /api/v1/accounts/:account_id/analytics/current/statistics \
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_statistics>`_
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/current/statistics".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
@@ -960,55 +961,50 @@
         <https://canvas.instructure.com/doc/api/analytics.html#method.analytics_api.department_statistics>`_
 
         :param term_id: The ID of the term, or the strings "current" or "completed"
         :type term_id: int or str
 
         :rtype: dict
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/analytics/terms/{}/statistics".format(self.id, term_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
     def get_enabled_features(self, **kwargs):
         """
         Lists all enabled features in an account.
 
         :calls: `GET /api/v1/accounts/:account_id/features/enabled \
         <https://canvas.instructure.com/doc/api/feature_flags.html#method.feature_flags.enabled_features>`_
 
-        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
-            :class:`canvasapi.feature.Feature`
+        :rtype: `list` of `str`
         """
-        return PaginatedList(
-            Feature,
-            self._requester,
+        response = self._requester.request(
             "GET",
             "accounts/{}/features/enabled".format(self.id),
-            {"account_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
         )
 
+        return response.json()
+
     def get_enrollment(self, enrollment, **kwargs):
         """
         Get an enrollment object by ID.
 
         :calls: `GET /api/v1/accounts/:account_id/enrollments/:id \
         <https://canvas.instructure.com/doc/api/enrollments.html#method.enrollments_api.show>`_
 
         :param enrollment: The object or ID of the enrollment to retrieve.
         :type enrollment: :class:`canvasapi.enrollment.Enrollment` or int
 
         :rtype: :class:`canvasapi.enrollment.Enrollment`
         """
-        from canvasapi.enrollment import Enrollment
-
         enrollment_id = obj_or_id(enrollment, "enrollment", (Enrollment,))
 
         response = self._requester.request(
             "GET",
             "accounts/{}/enrollments/{}".format(self.id, enrollment_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1022,16 +1018,14 @@
         <https://canvas.instructure.com/doc/api/enrollment_terms.html#method.terms_api.show>`_
 
         :param term: The object or ID of the enrollment term to retrieve.
         :type term: :class:`canvasapi.enrollment_term.EnrollmentTerm` or int
 
         :rtype: :class:`canvasapi.enrollment_term.EnrollmentTerm`
         """
-        from canvasapi.enrollment_term import EnrollmentTerm
-
         term_id = obj_or_id(term, "term", (EnrollmentTerm,))
 
         response = self._requester.request(
             "GET", "accounts/{}/terms/{}".format(self.id, term_id)
         )
         return EnrollmentTerm(self._requester, response.json())
 
@@ -1041,16 +1035,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/terms \
         <https://canvas.instructure.com/doc/api/enrollment_terms.html#method.terms_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.enrollment_term.EnrollmentTerm`
         """
-        from canvasapi.enrollment_term import EnrollmentTerm
-
         return PaginatedList(
             EnrollmentTerm,
             self._requester,
             "GET",
             "accounts/{}/terms".format(self.id),
             {"account_id": self.id},
             _root="enrollment_terms",
@@ -1063,16 +1055,14 @@
         <https://canvas.instructure.com/doc/api/external_tools.html#method.external_tools.show>`_
 
         :param tool: The object or ID of the tool
         :type tool: :class:`canvasapi.external_tool.ExternalTool` or int
 
         :rtype: :class:`canvasapi.external_tool.ExternalTool`
         """
-        from canvasapi.external_tool import ExternalTool
-
         tool_id = obj_or_id(tool, "tool", (ExternalTool,))
 
         response = self._requester.request(
             "GET",
             "accounts/{}/external_tools/{}".format(self.id, tool_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1085,16 +1075,14 @@
         """
         :calls: `GET /api/v1/accounts/:account_id/external_tools \
         <https://canvas.instructure.com/doc/api/external_tools.html#method.external_tools.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.external_tool.ExternalTool`
         """
-        from canvasapi.external_tool import ExternalTool
-
         return PaginatedList(
             ExternalTool,
             self._requester,
             "GET",
             "accounts/{}/external_tools".format(self.id),
             {"account_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
@@ -1148,15 +1136,14 @@
         <https://canvas.instructure.com/doc/api/account_notifications.html#method.account_notifications.show>`_
 
         :param notification_id: The notification ID of the desired notification.
         :type notification_id: `int`
 
         :rtype: :class:`canvasapi.account.AccountNotification`
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/account_notifications/{}".format(self.id, notification_id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
         response_json = response.json()
@@ -1170,15 +1157,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/grading_periods \
         <https://canvas.instructure.com/doc/api/grading_periods.html#method.grading_periods.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.grading_period.GradingPeriod`
         """
-
         return PaginatedList(
             GradingPeriod,
             self._requester,
             "GET",
             "accounts/{}/grading_periods".format(self.id),
             {"account_id": self.id},
             _root="grading_periods",
@@ -1191,15 +1177,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/grading_standards \
         <https://canvas.instructure.com/doc/api/grading_standards.html#method.grading_standards_api.context_index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.grading_standards.GradingStandard`
         """
-
         return PaginatedList(
             GradingStandard,
             self._requester,
             "GET",
             "accounts/%s/grading_standards" % (self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1210,16 +1195,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/group_categories \
         <https://canvas.instructure.com/doc/api/group_categories.html#method.group_categories.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.group.GroupCategory`
         """
-        from canvasapi.group import GroupCategory
-
         return PaginatedList(
             GroupCategory,
             self._requester,
             "GET",
             "accounts/{}/group_categories".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1229,16 +1212,14 @@
         Return a list of active groups for the specified account.
 
         :calls: `GET /api/v1/accounts/:account_id/groups \
         <https://canvas.instructure.com/doc/api/groups.html#method.groups.context_index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of :class:`canvasapi.group.Group`
         """
-        from canvasapi.group import Group
-
         return PaginatedList(
             Group,
             self._requester,
             "GET",
             "accounts/{}/groups".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1270,16 +1251,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/content_migrations/migrators \
         <https://canvas.instructure.com/doc/api/content_migrations.html#method.content_migrations.available_migrators>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.content_migration.Migrator`
         """
-        from canvasapi.content_migration import Migrator
-
         return PaginatedList(
             Migrator,
             self._requester,
             "GET",
             "accounts/{}/content_migrations/migrators".format(self.id),
             {"account_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
@@ -1294,16 +1273,14 @@
 
         :param group: The outcome group object or ID to return.
         :type group: :class:`canvasapi.outcome.OutcomeGroup` or int
 
         :returns: An outcome group object.
         :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
-        from canvasapi.outcome import OutcomeGroup
-
         outcome_group_id = obj_or_id(group, "outcome group", (OutcomeGroup,))
         response = self._requester.request(
             "GET",
             "accounts/{}/outcome_groups/{}".format(self.id, outcome_group_id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
@@ -1316,16 +1293,14 @@
         :calls: `GET /api/v1/accounts/:account_id/outcome_groups \
         <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.index>`_
 
         :returns: Paginated List of OutcomesGroups in the context.
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.outcome.OutcomeGroups`
         """
-        from canvasapi.outcome import OutcomeGroup
-
         return PaginatedList(
             OutcomeGroup,
             self._requester,
             "GET",
             "accounts/{}/outcome_groups".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1434,15 +1409,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/roles \
         <https://canvas.instructure.com/doc/api/roles.html#method.role_overrides.api_index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.account.Role`
         """
-
         return PaginatedList(
             Role,
             self._requester,
             "GET",
             "accounts/{}/roles".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1453,16 +1427,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/root_outcome_group \
         <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.redirect>`_
 
         :returns: The OutcomeGroup of the context.
         :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
-        from canvasapi.outcome import OutcomeGroup
-
         response = self._requester.request(
             "GET",
             "accounts/{}/root_outcome_group".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return OutcomeGroup(self._requester, response.json())
 
@@ -1508,16 +1480,14 @@
         Retrieve a paginated list of scopes.
 
         :calls: `GET /api/v1/accounts/:account_id/scopes \
         <https://canvas.instructure.com/doc/api/api_token_scopes.html#method.scopes_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of :class:`canvasapi.scope.Scope`
         """
-        from canvasapi.scope import Scope
-
         return PaginatedList(
             Scope,
             self._requester,
             "GET",
             "accounts/{}/scopes".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1529,15 +1499,14 @@
         :calls: `GET /api/v1/accounts/:account_id/grading_standards/:grading_standard_id \
         <https://canvas.instructure.com/doc/api/grading_standards.html#method.grading_standards_api.context_show>`_
 
         :param grading_standard_id: The grading standard id
         :type grading_standard_id: int
         :rtype: :class:`canvasapi.grading_standards.GradingStandard`
         """
-
         response = self._requester.request(
             "GET",
             "accounts/%s/grading_standards/%d" % (self.id, grading_standard_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return GradingStandard(self._requester, response.json())
 
@@ -1572,15 +1541,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/sis_imports \
         <https://canvas.instructure.com/doc/api/sis_imports.html#method.sis_imports_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.sis_import.SisImport`
         """
-
         return PaginatedList(
             SisImport,
             self._requester,
             "GET",
             "accounts/{}/sis_imports".format(self.id),
             {"account_id": self.id},
             _root="sis_imports",
@@ -1593,15 +1561,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/sis_imports/importing \
         <https://canvas.instructure.com/doc/api/sis_imports.html#method.sis_imports_api.importing>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList`
             of :class:`canvasapi.sis_import.SisImport`
         """
-
         return PaginatedList(
             SisImport,
             self._requester,
             "GET",
             "accounts/{}/sis_imports/importing".format(self.id),
             {"account_id": self.id},
             _root="sis_imports",
@@ -1636,16 +1603,14 @@
 
         :calls: `GET /api/v1/accounts/:account_id/logins \
         <https://canvas.instructure.com/doc/api/logins.html#method.pseudonyms.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.login.Login`
         """
-        from canvasapi.login import Login
-
         return PaginatedList(
             Login,
             self._requester,
             "GET",
             "accounts/{}/logins".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1661,16 +1626,14 @@
 
         :param user: The user object or ID to retrieve notifications for.
         :type user: :class:`canvasapi.user.User` or int
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.account.AccountNotification`
         """
-        from canvasapi.user import User
-
         user_id = obj_or_id(user, "user", (User,))
 
         return PaginatedList(
             AccountNotification,
             self._requester,
             "GET",
             "accounts/{}/users/{}/account_notifications".format(self.id, user_id),
@@ -1682,16 +1645,14 @@
         Retrieve a list of users associated with this account.
 
         :calls: `GET /api/v1/accounts/:account_id/users \
         <https://canvas.instructure.com/doc/api/users.html#method.users.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of :class:`canvasapi.user.User`
         """
-        from canvasapi.user import User
-
         return PaginatedList(
             User,
             self._requester,
             "GET",
             "accounts/{}/users".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1704,15 +1665,14 @@
         <https://canvas.instructure.com/doc/api/outcome_imports.html#method.outcome_imports_api.create>`_
 
         :param attachment: A file handler or path of the file to import.
         :type attachment: file or str
 
         :rtype: :class:`canvasapi.outcome_import.OutcomeImport`
         """
-
         attachment, is_path = file_or_path(attachment)
 
         try:
             response = self._requester.request(
                 "POST",
                 "accounts/{}/outcome_imports".format(self.id),
                 file={"attachment": attachment},
@@ -1723,24 +1683,41 @@
             response_json.update({"account_id": self.id})
 
             return OutcomeImport(self._requester, response_json)
         finally:
             if is_path:
                 attachment.close()
 
+    def query_audit_by_account(self, **kwargs):
+        """
+        List course change events for a specific account.
+
+        :calls: `GET /api/v1/audit/course/accounts/:account_id \
+        <https://canvas.instructure.com/doc/api/course_audit_log.html#method.course_audit_api.for_account>`_
+
+        :rtype: list of :class:`canvasapi.course_event.CourseEvent`
+        """
+
+        return PaginatedList(
+            CourseEvent,
+            self._requester,
+            "GET",
+            "audit/course/accounts/{}".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def show_account_auth_settings(self, **kwargs):
         """
         Return the current state of each account level setting
 
         :calls: `GET /api/v1/accounts/:account_id/sso_settings \
         <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.show_sso_settings>`_
 
         :rtype: :class:`canvasapi.account.SSOSettings`
         """
-
         response = self._requester.request(
             "GET",
             "accounts/{}/sso_settings".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
         return SSOSettings(self._requester, response.json())
@@ -1770,23 +1747,56 @@
         Return the current state of account level after updated
 
         :calls: `PUT /api/v1/accounts/:account_id/sso_settings \
         <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.update_sso_settings>`_
 
         :rtype: :class:`canvasapi.account.SSOSettings`
         """
-
         response = self._requester.request(
             "PUT",
             "accounts/{}/sso_settings".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
         return SSOSettings(self._requester, response.json())
 
+    def update_account_calendar_visibility(self, **kwargs):
+        """
+        Update one account calendar's visibility.
+
+        :calls: `PUT /api/v1/account_calendars/:account_id \
+        <https://canvas.instructure.com/doc/api/account_calendars.html#method.account_calendars_api.update>`_
+
+        :rtype: :class:`canvasapi.account_calendar.AccountCalendar`
+        """
+        response = self._requester.request(
+            "PUT",
+            "account_calendars/{}".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        return AccountCalendar(self._requester, response.json())
+
+    def update_many_account_calendars_visibility(self, **kwargs):
+        """
+        Update many account calendars visibility at once.
+
+        :calls: `PUT /api/v1/accounts/:account_id/account_calendars \
+        <https://canvas.instructure.com/doc/api/account_calendars.html#method.account_calendars_api.bulk_update>`_
+
+        :rtype: :class:`canvasapi.account_calendar.AccountCalendar`
+        """
+        response = self._requester.request(
+            "PUT",
+            "accounts/{}/account_calendars".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        return AccountCalendar(self._requester, response.json())
+
     def update_role(self, role, **kwargs):
         """
         Update permissions for an existing role.
 
         :calls: `PUT /api/v1/accounts/:account_id/roles/:id \
         <https://canvas.instructure.com/doc/api/roles.html#method.role_overrides.update>`_
 
@@ -1826,18 +1836,16 @@
             x in account_notification for x in required_key_list
         )
 
         if isinstance(account_notification, dict) and required_keys_present:
             kwargs["account_notification"] = account_notification
         else:
             raise RequiredFieldMissing(
-                (
-                    "account_notification must be a dictionary with keys "
-                    "'subject', 'message', 'start_at', and 'end_at'."
-                )
+                "account_notification must be a dictionary with keys "
+                "'subject', 'message', 'start_at', and 'end_at'."
             )
 
         response = self._requester.request(
             "PUT",
             "accounts/{}/account_notifications/{}".format(self.account_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
```

### Comparing `canvasapi-3.0.0/canvasapi/appointment_group.py` & `canvasapi-3.1.0/canvasapi/appointment_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         :rtype: :class:`canvasapi.appointment_group.AppointmentGroup`
         """
         if isinstance(appointment_group, dict) and "context_codes" in appointment_group:
             kwargs["appointment_group"] = appointment_group
         else:
             raise RequiredFieldMissing(
-                "Dictionary with key 'context_codes' is required."
+                "Dictionary with key 'context_code' is required."
             )
 
         response = self._requester.request(
             "PUT",
             "appointment_groups/{}".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
```

### Comparing `canvasapi-3.0.0/canvasapi/assignment.py` & `canvasapi-3.1.0/canvasapi/assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,34 @@
             _kwargs=combine_kwargs(**kwargs),
         )
 
         request_json = request.json()
 
         return request_json.get("needs_provisional_grade")
 
+    def get_students_selected_for_moderation(self, **kwargs):
+        """
+        Get a list of students selected for moderation.
+
+        :calls: `GET /api/v1/courses/:course_id/assignments/:assignment_id/moderated_students \
+        <https://canvas.instructure.com/doc/api/moderated_grading.html#method.moderation_set.index>`_
+
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.user.User`
+        """
+        return PaginatedList(
+            User,
+            self._requester,
+            "GET",
+            "courses/{}/assignments/{}/moderated_students".format(
+                self.course_id, self.id
+            ),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def get_submission(self, user, **kwargs):
         """
         Get a single submission, based on user id.
 
         :calls: `GET /api/v1/courses/:course_id/assignments/:assignment_id/submissions/:user_id \
         <https://canvas.instructure.com/doc/api/submissions.html#method.submissions_api.show>`_
 
@@ -273,14 +293,35 @@
             "courses/{}/assignments/{}/provisional_grades/publish".format(
                 self.course_id, self.id
             ),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
 
+    def select_students_for_moderation(self, **kwargs):
+        """
+        Select student(s) for moderation.
+
+        :calls: `POST /api/v1/courses/:course_id/assignments/:assignment_id/moderated_students \
+        <https://canvas.instructure.com/doc/api/moderated_grading.html#method.moderation_set.create>`_
+
+        :returns: The list of users that were selected
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.user.User`
+        """
+        return PaginatedList(
+            User,
+            self._requester,
+            "POST",
+            "courses/{}/assignments/{}/moderated_students".format(
+                self.course_id, self.id
+            ),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def selected_provisional_grade(self, provisional_grade_id, **kwargs):
         """
         Choose which provisional grade the student should receive for a submission.
         The caller must be the final grader for the assignment
         or an admin with :select_final_grade rights.
 
         :calls: `PUT /api/v1/courses/:course_id/assignments/:assignment_id/provisional_grades/
@@ -518,15 +559,15 @@
     def __str__(self):
         return "{} ({})".format(self.title, self.id)
 
     def delete(self, **kwargs):
         """
         Delete this assignment override.
 
-        :calls: `DELETE /api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
+        :calls: `DELETE /api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id \
         <https://canvas.instructure.com/doc/api/assignments.html#method.assignment_overrides.destroy>`_
 
         :returns: The previous content of the now-deleted assignment override.
         :rtype: :class:`canvasapi.assignment.AssignmentGroup`
         """
         response = self._requester.request(
             "DELETE",
@@ -543,15 +584,15 @@
 
     def edit(self, **kwargs):
         """
         Update this assignment override.
 
         Note: All current overridden values must be supplied if they are to be retained.
 
-        :calls: `PUT /api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id
+        :calls: `PUT /api/v1/courses/:course_id/assignments/:assignment_id/overrides/:id \
         <https://canvas.instructure.com/doc/api/assignments.html#method.assignment_overrides.update>`_
 
         :rtype: :class:`canvasapi.assignment.AssignmentOverride`
         """
         response = self._requester.request(
             "PUT",
             "courses/{}/assignments/{}/overrides/{}".format(
```

### Comparing `canvasapi-3.0.0/canvasapi/authentication_provider.py` & `canvasapi-3.1.0/canvasapi/authentication_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,30 @@
 from canvasapi.util import combine_kwargs
 
 
 class AuthenticationProvider(CanvasObject):
     def __str__(self):  # pragma: no cover
         return "{} ({})".format(self.auth_type, self.position)
 
+    def delete(self, **kwargs):
+        """
+        Delete the config
+
+        :calls: `DELETE /api/v1/accounts/:account_id/authentication_providers/:id \
+        <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.destroy>`_
+
+        :rtype: :class:`canvasapi.authentication_provider.AuthenticationProvider`
+        """
+        response = self._requester.request(
+            "DELETE",
+            "accounts/{}/authentication_providers/{}".format(self.account_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return AuthenticationProvider(self._requester, response.json())
+
     def update(self, **kwargs):
         """
         Update an authentication provider using the same options as the create endpoint
 
         :calls: `PUT /api/v1/accounts/:account_id/authentication_providers/:id \
         <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.update>`_
 
@@ -21,22 +37,7 @@
             _kwargs=combine_kwargs(**kwargs),
         )
 
         if response.json().get("auth_type"):
             super(AuthenticationProvider, self).set_attributes(response.json())
 
         return response.json().get("auth_type")
-
-    def delete(self):
-        """
-        Delete the config
-
-        :calls: `DELETE /api/v1/accounts/:account_id/authentication_providers/:id \
-        <https://canvas.instructure.com/doc/api/authentication_providers.html#method.account_authorization_configs.destroy>`_
-
-        :rtype: :class:`canvasapi.authentication_provider.AuthenticationProvider`
-        """
-        response = self._requester.request(
-            "DELETE",
-            "accounts/{}/authentication_providers/{}".format(self.account_id, self.id),
-        )
-        return AuthenticationProvider(self._requester, response.json())
```

### Comparing `canvasapi-3.0.0/canvasapi/blueprint.py` & `canvasapi-3.1.0/canvasapi/blueprint.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/bookmark.py` & `canvasapi-3.1.0/canvasapi/bookmark.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/calendar_event.py` & `canvasapi-3.1.0/canvasapi/calendar_event.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/canvas.py` & `canvasapi-3.1.0/canvasapi/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import warnings
 
 from canvasapi.account import Account
+from canvasapi.account_calendar import AccountCalendar
+from canvasapi.appointment_group import AppointmentGroup
+from canvasapi.calendar_event import CalendarEvent
 from canvasapi.comm_message import CommMessage
-from canvasapi.course import Course
+from canvasapi.conversation import Conversation
+from canvasapi.course import Course, CourseNickname
 from canvasapi.course_epub_export import CourseEpubExport
 from canvasapi.current_user import CurrentUser
+from canvasapi.discussion_topic import DiscussionTopic
 from canvasapi.eportfolio import EPortfolio
 from canvasapi.exceptions import RequiredFieldMissing
 from canvasapi.file import File
 from canvasapi.folder import Folder
 from canvasapi.group import Group, GroupCategory
+from canvasapi.jwt import JWT
+from canvasapi.outcome import Outcome, OutcomeGroup
 from canvasapi.paginated_list import PaginatedList
+from canvasapi.planner import PlannerNote, PlannerOverride
+from canvasapi.poll import Poll
+from canvasapi.progress import Progress
 from canvasapi.requester import Requester
 from canvasapi.section import Section
 from canvasapi.todo import Todo
 from canvasapi.user import User
 from canvasapi.util import combine_kwargs, get_institution_url, obj_or_id
 
 
@@ -89,17 +99,14 @@
 
         :param conversation_ids: List of conversations to update. Limited to 500 conversations.
         :type conversation_ids: `list` of `str`
         :param event: The action to take on each conversation.
         :type event: `str`
         :rtype: :class:`canvasapi.progress.Progress`
         """
-
-        from canvasapi.progress import Progress
-
         ALLOWED_EVENTS = [
             "mark_as_read",
             "mark_as_unread",
             "star",
             "unstar",
             "archive",
             "destroy",
@@ -202,16 +209,14 @@
 
         :param appointment_group: The attributes of the appointment group.
         :type appointment_group: `dict`
         :param title: The title of the appointment group.
         :type title: `str`
         :rtype: :class:`canvasapi.appointment_group.AppointmentGroup`
         """
-        from canvasapi.appointment_group import AppointmentGroup
-
         if (
             isinstance(appointment_group, dict)
             and "context_codes" in appointment_group
             and "title" in appointment_group
         ):
             kwargs["appointment_group"] = appointment_group
 
@@ -239,21 +244,19 @@
         :calls: `POST /api/v1/calendar_events \
         <https://canvas.instructure.com/doc/api/calendar_events.html#method.calendar_events_api.create>`_
 
         :param calendar_event: The attributes of the calendar event.
         :type calendar_event: `dict`
         :rtype: :class:`canvasapi.calendar_event.CalendarEvent`
         """
-        from canvasapi.calendar_event import CalendarEvent
-
         if isinstance(calendar_event, dict) and "context_code" in calendar_event:
             kwargs["calendar_event"] = calendar_event
         else:
             raise RequiredFieldMissing(
-                "Dictionary with key 'context_codes' is required."
+                "Dictionary with key 'context_code' is required."
             )
 
         response = self.__requester.request(
             "POST", "calendar_events", _kwargs=combine_kwargs(**kwargs)
         )
 
         return CalendarEvent(self.__requester, response.json())
@@ -270,16 +273,14 @@
             with 'course\\_' or 'group\\_' respectively,
             e.g. recipients=['1', '2', 'course_3']
         :type recipients: `list` of `str`
         :param body: The body of the message being added.
         :type body: `str`
         :rtype: list of :class:`canvasapi.conversation.Conversation`
         """
-        from canvasapi.conversation import Conversation
-
         kwargs["recipients"] = recipients
         kwargs["body"] = body
 
         response = self.__requester.request(
             "POST", "conversations", _kwargs=combine_kwargs(**kwargs)
         )
         return [Conversation(self.__requester, convo) for convo in response.json()]
@@ -294,25 +295,38 @@
         :rtype: :class:`canvasapi.group.Group`
         """
         response = self.__requester.request(
             "POST", "groups", _kwargs=combine_kwargs(**kwargs)
         )
         return Group(self.__requester, response.json())
 
+    def create_jwt(self, **kwargs):
+        """
+        Creates a unique JWT to use with other Canvas services.
+
+        :calls: `POST /api/v1/jwts \
+        <https://canvas.instructure.com/doc/api/jw_ts.html#method.jwts.create>`_
+
+        :rtype: list of :class:`canvasapi.jwt.JWT`
+        """
+        response = self.__requester.request(
+            "POST", "jwts", _kwargs=combine_kwargs(**kwargs)
+        )
+
+        return JWT(self.__requester, response.json())
+
     def create_planner_note(self, **kwargs):
         """
         Create a planner note for the current user
 
         :calls: `POST /api/v1/planner_notes \
         <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.create>`_
 
         :rtype: :class:`canvasapi.planner.PlannerNote`
         """
-        from canvasapi.planner import PlannerNote
-
         response = self.__requester.request(
             "POST", "planner_notes", _kwargs=combine_kwargs(**kwargs)
         )
         return PlannerNote(self.__requester, response.json())
 
     def create_planner_override(self, plannable_type, plannable_id, **kwargs):
         """
@@ -325,16 +339,14 @@
         :type plannable_type: str
 
         :param plannable_id: ID of the item that you are overriding in the planner
         :type plannable_id: int or :class:`canvasapi.planner.PlannerOverride`
 
         :rtype: :class:`canvasapi.planner.PlannerOverride`
         """
-        from canvasapi.planner import PlannerOverride
-
         if isinstance(plannable_type, str):
             kwargs["plannable_type"] = plannable_type
         else:
             raise RequiredFieldMissing("plannable_type is required as a str.")
         if isinstance(plannable_id, int):
             kwargs["plannable_id"] = plannable_id
         else:
@@ -352,16 +364,14 @@
         :calls: `POST /api/v1/polls \
         <https://canvas.instructure.com/doc/api/polls.html#method.polling/polls.create>`_
 
         :param polls: List of polls to create. `'question'` key is required.
         :type polls: list of dict
         :rtype: :class:`canvasapi.poll.Poll`
         """
-        from canvasapi.poll import Poll
-
         if (
             isinstance(polls, list)
             and isinstance(polls[0], dict)
             and "question" in polls[0]
         ):
             kwargs["polls"] = polls
         else:
@@ -397,14 +407,32 @@
             uri_str = "accounts/{}"
 
         response = self.__requester.request(
             "GET", uri_str.format(account_id), _kwargs=combine_kwargs(**kwargs)
         )
         return Account(self.__requester, response.json())
 
+    def get_account_calendars(self, **kwargs):
+        """
+        Returns a paginated list of account calendars available to the user.
+
+        :calls: `GET /api/v1/account_calendars \
+        <https://canvas.instructure.com/doc/api/account_calendars.html#method.account_calendars_api.index>`_
+
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.account_calendar.AccountCalendar`
+        """
+        return PaginatedList(
+            AccountCalendar,
+            self.__requester,
+            "GET",
+            "account_calendars",
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def get_accounts(self, **kwargs):
         """
         List accounts that the current user can view or manage.
 
         Typically, students and teachers will get an empty list in
         response. Only account admins can view the accounts that they
         are in.
@@ -448,16 +476,14 @@
 
         :param context_codes: Course ID(s) or <Course> objects to request announcements from.
         :type context_codes: list
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
                 :class:`canvasapi.discussion_topic.DiscussionTopic`
         """
-        from canvasapi.discussion_topic import DiscussionTopic
-
         if type(context_codes) is not list or len(context_codes) == 0:
             raise RequiredFieldMissing("context_codes need to be passed as a list")
 
         if isinstance(context_codes[0], str) and "course_" in context_codes[0]:
             # Legacy support for context codes passed as list of `course_123`-style strings
             kwargs["context_codes"] = context_codes
         else:
@@ -489,16 +515,14 @@
         <https://canvas.instructure.com/doc/api/appointment_groups.html#method.appointment_groups.show>`_
 
         :param appointment_group: The ID of the appointment group.
         :type appointment_group: :class:`canvasapi.appointment_group.AppointmentGroup` or int
 
         :rtype: :class:`canvasapi.appointment_group.AppointmentGroup`
         """
-        from canvasapi.appointment_group import AppointmentGroup
-
         appointment_group_id = obj_or_id(
             appointment_group, "appointment_group", (AppointmentGroup,)
         )
 
         response = self.__requester.request(
             "GET",
             "appointment_groups/{}".format(appointment_group_id),
@@ -512,16 +536,14 @@
 
         :calls: `GET /api/v1/appointment_groups \
         <https://canvas.instructure.com/doc/api/appointment_groups.html#method.appointment_groups.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.appointment_group.AppointmentGroup`
         """
-        from canvasapi.appointment_group import AppointmentGroup
-
         return PaginatedList(
             AppointmentGroup,
             self.__requester,
             "GET",
             "appointment_groups",
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -549,16 +571,14 @@
         <https://canvas.instructure.com/doc/api/calendar_events.html#method.calendar_events_api.show>`_
 
         :param calendar_event: The object or ID of the calendar event.
         :type calendar_event: :class:`canvasapi.calendar_event.CalendarEvent` or int
 
         :rtype: :class:`canvasapi.calendar_event.CalendarEvent`
         """
-        from canvasapi.calendar_event import CalendarEvent
-
         calendar_event_id = obj_or_id(
             calendar_event, "calendar_event", (CalendarEvent,)
         )
 
         response = self.__requester.request(
             "GET",
             "calendar_events/{}".format(calendar_event_id),
@@ -572,16 +592,14 @@
 
         :calls: `GET /api/v1/calendar_events \
         <https://canvas.instructure.com/doc/api/calendar_events.html#method.calendar_events_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.calendar_event.CalendarEvent`
         """
-        from canvasapi.calendar_event import CalendarEvent
-
         return PaginatedList(
             CalendarEvent,
             self.__requester,
             "GET",
             "calendar_events",
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -620,16 +638,14 @@
         <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.show>`_
 
         :param conversation: The object or ID of the conversation.
         :type conversation: :class:`canvasapi.conversation.Conversation` or int
 
         :rtype: :class:`canvasapi.conversation.Conversation`
         """
-        from canvasapi.conversation import Conversation
-
         conversation_id = obj_or_id(conversation, "conversation", (Conversation,))
 
         response = self.__requester.request(
             "GET",
             "conversations/{}".format(conversation_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -641,16 +657,14 @@
 
         :calls: `GET /api/v1/conversations \
         <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of \
         :class:`canvasapi.conversation.Conversation`
         """
-        from canvasapi.conversation import Conversation
-
         return PaginatedList(
             Conversation,
             self.__requester,
             "GET",
             "conversations",
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -712,16 +726,14 @@
         <https://canvas.instructure.com/doc/api/users.html#method.course_nicknames.show>`_
 
         :param course: The object or ID of the course.
         :type course: :class:`canvasapi.course.Course` or int
 
         :rtype: :class:`canvasapi.course.CourseNickname`
         """
-        from canvasapi.course import CourseNickname
-
         course_id = obj_or_id(course, "course", (Course,))
 
         response = self.__requester.request(
             "GET",
             "users/self/course_nicknames/{}".format(course_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -733,16 +745,14 @@
 
         :calls: `GET /api/v1/users/self/course_nicknames \
         <https://canvas.instructure.com/doc/api/users.html#method.course_nicknames.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.course.CourseNickname`
         """
-        from canvasapi.course import CourseNickname
-
         return PaginatedList(
             CourseNickname,
             self.__requester,
             "GET",
             "users/self/course_nicknames",
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -910,17 +920,14 @@
         <https://canvas.instructure.com/doc/api/appointment_groups.html#method.appointment_groups.groups>`_
 
         :param appointment_group: The object or ID of the appointment group.
         :type appointment_group: :class:`canvasapi.appointment_group.AppointmentGroup` or int
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of :class:`canvasapi.group.Group`
         """
-        from canvasapi.appointment_group import AppointmentGroup
-        from canvasapi.group import Group
-
         appointment_group_id = obj_or_id(
             appointment_group, "appointment_group", (AppointmentGroup,)
         )
 
         return PaginatedList(
             Group,
             self.__requester,
@@ -938,16 +945,14 @@
 
         :param outcome: The outcome object or ID to return.
         :type outcome: :class:`canvasapi.outcome.Outcome` or int
 
         :returns: An Outcome object.
         :rtype: :class:`canvasapi.outcome.Outcome`
         """
-        from canvasapi.outcome import Outcome
-
         outcome_id = obj_or_id(outcome, "outcome", (Outcome,))
         response = self.__requester.request(
             "GET", "outcomes/{}".format(outcome_id), _kwargs=combine_kwargs(**kwargs)
         )
         return Outcome(self.__requester, response.json())
 
     def get_outcome_group(self, group, **kwargs):
@@ -959,16 +964,14 @@
 
         :param group: The outcome group object or ID to return.
         :type group: :class:`canvasapi.outcome.OutcomeGroup` or int
 
         :returns: An outcome group object.
         :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
-        from canvasapi.outcome import OutcomeGroup
-
         outcome_group_id = obj_or_id(group, "group", (OutcomeGroup,))
 
         response = self.__requester.request(
             "GET",
             "global/outcome_groups/{}".format(outcome_group_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -983,16 +986,14 @@
         <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.show>`_
 
         :param planner_note: The ID of the planner note to retrieve.
         :type planner_note: int or :class:`canvasapi.planner.PlannerNote`
 
         :rtype: :class:`canvasapi.planner.PlannerNote`
         """
-        from canvasapi.planner import PlannerNote
-
         if isinstance(planner_note, int) or isinstance(planner_note, PlannerNote):
             planner_note_id = obj_or_id(planner_note, "planner_note", (PlannerNote,))
         else:
             raise RequiredFieldMissing(
                 "planner_note is required as an object or as an int."
             )
 
@@ -1010,16 +1011,14 @@
 
         :calls: `GET /api/v1/planner_notes \
         <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.planner.PlannerNote`
         """
-        from canvasapi.planner import PlannerNote
-
         return PaginatedList(
             PlannerNote,
             self.__requester,
             "GET",
             "planner_notes",
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1032,16 +1031,14 @@
         <https://canvas.instructure.com/doc/api/planner.html#method.planner_overrides.show>`_
 
         :param planner_override: The override or the ID of the planner override to retrieve.
         :type planner_override: int or :class:`canvasapi.planner.PlannerOverride`
 
         :rtype: :class:`canvasapi.planner.PlannerOverride`
         """
-        from canvasapi.planner import PlannerOverride
-
         if isinstance(planner_override, int) or isinstance(
             planner_override, PlannerOverride
         ):
             planner_override_id = obj_or_id(
                 planner_override, "planner_override", (PlannerOverride,)
             )
         else:
@@ -1063,16 +1060,14 @@
 
         :calls: `GET /api/v1/planner/overrides \
         <https://canvas.instructure.com/doc/api/planner.html#method.planner_overrides.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.planner.PlannerOverride`
         """
-        from canvasapi.planner import PlannerOverride
-
         return PaginatedList(
             PlannerOverride,
             self.__requester,
             "GET",
             "planner/overrides",
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1084,16 +1079,14 @@
         :calls: `GET /api/v1/polls/:id \
         <https://canvas.instructure.com/doc/api/polls.html#method.polling/polls.show>`_
 
         :param poll: The ID of the poll or the poll to change.
         :type poll: int
         :rtype: :class:`canvasapi.poll.Poll`
         """
-        from canvasapi.poll import Poll
-
         poll_id = obj_or_id(poll, "poll", (Poll,))
 
         response = self.__requester.request(
             "GET", "polls/{}".format(poll_id), _kwargs=combine_kwargs(**kwargs)
         )
         return Poll(self.__requester, response.json()["polls"][0])
 
@@ -1103,16 +1096,14 @@
 
         :calls: `GET /api/1/polls \
         <https://canvas.instructure.com/doc/api/polls.html#method.polling/polls.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.poll.Poll`
         """
-        from canvasapi.poll import Poll
-
         return PaginatedList(
             Poll,
             self.__requester,
             "GET",
             "polls",
             _root="polls",
             _kwargs=combine_kwargs(**kwargs),
@@ -1126,17 +1117,14 @@
             <https://canvas.instructure.com/doc/api/progress.html#method.progress.show>`_
 
         :param progress: The object or ID of the progress to retrieve.
         :type progress: int, str or :class:`canvasapi.progress.Progress`
 
         :rtype: :class:`canvasapi.progress.Progress`
         """
-
-        from canvasapi.progress import Progress
-
         progress_id = obj_or_id(progress, "progress", (Progress,))
 
         response = self.__requester.request(
             "GET", "progress/{}".format(progress_id), _kwargs=combine_kwargs(**kwargs)
         )
         return Progress(self.__requester, response.json())
 
@@ -1146,16 +1134,14 @@
 
         :calls: `GET /api/v1/global/root_outcome_group \
         <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.redirect>`_
 
         :returns: The OutcomeGroup of the context.
         :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
-        from canvasapi.outcome import OutcomeGroup
-
         response = self.__requester.request(
             "GET", "global/root_outcome_group", _kwargs=combine_kwargs(**kwargs)
         )
         return OutcomeGroup(self.__requester, response.json())
 
     def get_section(self, section, use_sis_id=False, **kwargs):
         """
@@ -1256,17 +1242,14 @@
         <https://canvas.instructure.com/doc/api/appointment_groups.html#method.appointment_groups.users>`_
 
         :param appointment_group: The object or ID of the appointment group.
         :type appointment_group: :class:`canvasapi.appointment_group.AppointmentGroup` or int
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of :class:`canvasapi.user.User`
         """
-        from canvasapi.appointment_group import AppointmentGroup
-        from canvasapi.user import User
-
         appointment_group_id = obj_or_id(
             appointment_group, "appointment_group", (AppointmentGroup,)
         )
 
         return PaginatedList(
             User,
             self.__requester,
@@ -1298,14 +1281,35 @@
             # Needs to call special endpoint without api/v1
             _url=self.__requester.original_url + "/api/graphql",
             json=True,
         )
 
         return response.json()
 
+    def refresh_jwt(self, jwt, **kwargs):
+        """
+        Refreshes a JWT for reuse with other canvas services. It generates a
+        different JWT each time it's called; expires after one hour.
+
+        :calls: `POST /api/v1/jwts/refresh \
+        <https://canvas.instructure.com/doc/api/jw_ts.html#method.jwts.refresh>`_
+
+        :param jwt: An existing JWT to refresh.
+        :type jwt: str or :class:`canvasapi.jwt.JWT`
+        :rtype: :class:`canvasapi.jwt.JWT`
+        """
+        if isinstance(jwt, JWT):
+            jwt = jwt.token
+
+        response = self.__requester.request(
+            "POST", "jwts/refresh", jwt=jwt, _kwargs=combine_kwargs(**kwargs)
+        )
+
+        return JWT(self.__requester, response.json())
+
     def reserve_time_slot(self, calendar_event, participant_id=None, **kwargs):
         """
         Return single Calendar Event by id
 
         :calls: `POST /api/v1/calendar_events/:id/reservations \
         <https://canvas.instructure.com/doc/api/calendar_events.html#method.calendar_events_api.reserve>`_
 
@@ -1313,16 +1317,14 @@
         :type calendar_event: :class:`canvasapi.calendar_event.CalendarEvent` or int
 
         :param participant_id: The ID of the participant, if given.
         :type participant_id: str
 
         :rtype: :class:`canvasapi.calendar_event.CalendarEvent`
         """
-        from canvasapi.calendar_event import CalendarEvent
-
         calendar_event_id = obj_or_id(
             calendar_event, "calendar_event", (CalendarEvent,)
         )
 
         if participant_id:
             uri = "calendar_events/{}/reservations/{}".format(
                 calendar_event_id, participant_id
@@ -1396,16 +1398,14 @@
         :param course: The ID of the course.
         :type course: :class:`canvasapi.course.Course` or int
         :param nickname: The nickname for the course.
         :type nickname: str
 
         :rtype: :class:`canvasapi.course.CourseNickname`
         """
-        from canvasapi.course import CourseNickname
-
         course_id = obj_or_id(course, "course", (Course,))
 
         kwargs["nickname"] = nickname
 
         response = self.__requester.request(
             "PUT",
             "users/self/course_nicknames/{}".format(course_id),
```

### Comparing `canvasapi-3.0.0/canvasapi/canvas_object.py` & `canvasapi-3.1.0/canvasapi/canvas_object.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/collaboration.py` & `canvasapi-3.1.0/canvasapi/collaboration.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/communication_channel.py` & `canvasapi-3.1.0/canvasapi/communication_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         :param notification_preferences: Dict that indicates the frequency for \
             different notification types.
         :type notification: dict
 
         :rtype: :class:`canvasapi.notification_preference.NotificationPreference`
         """
         if isinstance(notification_preferences, dict) and notification_preferences:
-
             for key, value in notification_preferences.items():
                 try:
                     if not value["frequency"]:
                         return False
                 except KeyError:
                     return False
```

### Comparing `canvasapi-3.0.0/canvasapi/content_migration.py` & `canvasapi-3.1.0/canvasapi/content_migration.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/conversation.py` & `canvasapi-3.1.0/canvasapi/conversation.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,51 +2,35 @@
 from canvasapi.util import combine_kwargs
 
 
 class Conversation(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.subject, self.id)
 
-    def edit(self, **kwargs):
+    def add_message(self, body, **kwargs):
         """
-        Update a conversation.
+        Add a message to a conversation.
 
-        :calls: `PUT /api/v1/conversations/:id \
-        <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.update>`_
+        :calls: `POST /api/v1/conversations/:id/add_message \
+        <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.add_message>`_
 
-        :rtype: `bool`
+        :param body: The body of the conversation.
+        :type body: str
+        :returns: A conversation with only the most recent message.
+        :rtype: :class:`canvasapi.account.Conversation`
         """
         response = self._requester.request(
-            "PUT", "conversations/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
+            "POST",
+            "conversations/{}/add_message".format(self.id),
+            body=body,
+            _kwargs=combine_kwargs(**kwargs),
         )
+        return Conversation(self._requester, response.json())
 
-        if response.json().get("id"):
-            super(Conversation, self).set_attributes(response.json())
-            return True
-        else:
-            return False
-
-    def delete(self):
-        """
-        Delete a conversation.
-
-        :calls: `DELETE /api/v1/conversations/:id \
-        <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.destroy>`_
-
-        :rtype: `bool`
-        """
-        response = self._requester.request("DELETE", "conversations/{}".format(self.id))
-
-        if response.json().get("id"):
-            super(Conversation, self).set_attributes(response.json())
-            return True
-        else:
-            return False
-
-    def add_recipients(self, recipients):
+    def add_recipients(self, recipients, **kwargs):
         """
         Add a recipient to a conversation.
 
         :calls: `POST /api/v1/conversations/:id/add_recipients \
         <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.add_recipients>`_
 
         :param recipients: A list of string format recipient ids.
@@ -56,48 +40,72 @@
         :type recipients:  `list` of `str`
         :rtype: :class:`canvasapi.account.Conversation`
         """
         response = self._requester.request(
             "POST",
             "conversations/{}/add_recipients".format(self.id),
             recipients=recipients,
+            _kwargs=combine_kwargs(**kwargs),
         )
         return Conversation(self._requester, response.json())
 
-    def add_message(self, body, **kwargs):
+    def delete(self, **kwargs):
         """
-        Add a message to a conversation.
+        Delete a conversation.
 
-        :calls: `POST /api/v1/conversations/:id/add_message \
-        <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.add_message>`_
+        :calls: `DELETE /api/v1/conversations/:id \
+        <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.destroy>`_
 
-        :param body: The body of the conversation.
-        :type body: str
-        :returns: A conversation with only the most recent message.
-        :rtype: :class:`canvasapi.account.Conversation`
+        :rtype: `bool`
         """
         response = self._requester.request(
-            "POST",
-            "conversations/{}/add_message".format(self.id),
-            body=body,
+            "DELETE",
+            "conversations/{}".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
-        return Conversation(self._requester, response.json())
 
-    def delete_messages(self, remove):
+        if response.json().get("id"):
+            super(Conversation, self).set_attributes(response.json())
+            return True
+        else:
+            return False
+
+    def delete_messages(self, remove, **kwargs):
         """
         Delete messages from this conversation.
 
         Note that this only affects this user's view of the conversation.
         If all messages are deleted, the conversation will be as well.
 
         :calls: `POST /api/v1/conversations/:id/remove_messages \
         <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.remove_messages>`_
 
         :param remove: List of message ids to be removed.
         :type remove: `list` of `str`
         :rtype: `dict`
         """
         response = self._requester.request(
-            "POST", "conversations/{}/remove_messages".format(self.id), remove=remove
+            "POST",
+            "conversations/{}/remove_messages".format(self.id),
+            remove=remove,
+            _kwargs=combine_kwargs(**kwargs),
         )
         return response.json()
+
+    def edit(self, **kwargs):
+        """
+        Update a conversation.
+
+        :calls: `PUT /api/v1/conversations/:id \
+        <https://canvas.instructure.com/doc/api/conversations.html#method.conversations.update>`_
+
+        :rtype: `bool`
+        """
+        response = self._requester.request(
+            "PUT", "conversations/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
+        )
+
+        if response.json().get("id"):
+            super(Conversation, self).set_attributes(response.json())
+            return True
+        else:
+            return False
```

### Comparing `canvasapi-3.0.0/canvasapi/course.py` & `canvasapi-3.1.0/canvasapi/course.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import warnings
 
 from canvasapi.assignment import Assignment, AssignmentGroup
 from canvasapi.blueprint import BlueprintSubscription
 from canvasapi.canvas_object import CanvasObject
 from canvasapi.collaboration import Collaboration
+from canvasapi.content_export import ContentExport
 from canvasapi.course_epub_export import CourseEpubExport
+from canvasapi.course_event import CourseEvent
 from canvasapi.custom_gradebook_columns import CustomGradebookColumn
 from canvasapi.discussion_topic import DiscussionTopic
 from canvasapi.exceptions import RequiredFieldMissing
+from canvasapi.external_feed import ExternalFeed
 from canvasapi.feature import Feature, FeatureFlag
 from canvasapi.folder import Folder
 from canvasapi.grade_change_log import GradeChangeEvent
 from canvasapi.gradebook_history import (
     Day,
     Grader,
     SubmissionHistory,
     SubmissionVersion,
 )
 from canvasapi.grading_period import GradingPeriod
 from canvasapi.grading_standard import GradingStandard
 from canvasapi.license import License
+from canvasapi.module import Module
 from canvasapi.outcome_import import OutcomeImport
 from canvasapi.page import Page
 from canvasapi.paginated_list import PaginatedList
 from canvasapi.progress import Progress
 from canvasapi.quiz import QuizExtension
 from canvasapi.rubric import Rubric, RubricAssociation
 from canvasapi.submission import GroupedSubmission, Submission
@@ -318,16 +322,14 @@
         :calls: `POST /api/v1/courses/:course_id/external_feeds \
         <https://canvas.instructure.com/doc/api/announcement_external_feeds.html#method.external_feeds.create>`_
 
         :param url: The url of the external rss or atom feed
         :type url: str
         :rtype: :class:`canvasapi.external_feed.ExternalFeed`
         """
-        from canvasapi.external_feed import ExternalFeed
-
         response = self._requester.request(
             "POST",
             "courses/{}/external_feeds".format(self.id),
             url=url,
             _kwargs=combine_kwargs(**kwargs),
         )
         return ExternalFeed(self._requester, response.json())
@@ -431,16 +433,14 @@
         <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.create>`_
 
         :param module: The attributes for the module.
         :type module: dict
         :returns: The created module.
         :rtype: :class:`canvasapi.module.Module`
         """
-        from canvasapi.module import Module
-
         if isinstance(module, dict) and "name" in module:
             kwargs["module"] = module
         else:
             raise RequiredFieldMissing("Dictionary with key 'name' is required.")
 
         response = self._requester.request(
             "POST",
@@ -592,16 +592,14 @@
         <https://canvas.instructure.com/doc/api/announcement_external_feeds.html#method.external_feeds.destroy>`_
 
         :param feed: The object or ID of the feed to be deleted.
         :type feed: :class:`canvasapi.external_feed.ExternalFeed` or int
 
         :rtype: :class:`canvasapi.external_feed.ExternalFeed`
         """
-        from canvasapi.external_feed import ExternalFeed
-
         feed_id = obj_or_id(feed, "feed", (ExternalFeed,))
 
         response = self._requester.request(
             "DELETE",
             "courses/{}/external_feeds/{}".format(self.id, feed_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -691,16 +689,14 @@
         <https://canvas.instructure.com/doc/api/content_exports.html#method.content_exports_api.create>`_
 
         :param export_type: The type of content to export.
         :type export_type: str
 
         :rtype: :class:`canvasapi.content_export.ContentExport`
         """
-        from canvasapi.content_export import ContentExport
-
         kwargs["export_type"] = export_type
 
         response = self._requester.request(
             "POST",
             "courses/{}/content_exports".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -923,16 +919,14 @@
         <https://canvas.instructure.com/doc/api/content_exports.html#method.content_exports_api.show>`_
 
         :param content_export: The object or ID of the content export to show.
         :type content_export: int or :class:`canvasapi.content_export.ContentExport`
 
         :rtype: :class:`canvasapi.content_export.ContentExport`
         """
-        from canvasapi.content_export import ContentExport
-
         export_id = obj_or_id(content_export, "content_export", (ContentExport,))
 
         response = self._requester.request(
             "GET",
             "courses/{}/content_exports/{}".format(self.id, export_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -945,16 +939,14 @@
 
         :calls: `GET /api/v1/courses/:course_id/content_exports\
         <https://canvas.instructure.com/doc/api/content_exports.html#method.content_exports_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.content_export.ContentExport`
         """
-        from canvasapi.content_export import ContentExport
-
         return PaginatedList(
             ContentExport,
             self._requester,
             "GET",
             "courses/{}/content_exports".format(self.id),
             kwargs=combine_kwargs(**kwargs),
         )
@@ -1131,26 +1123,24 @@
     def get_enabled_features(self, **kwargs):
         """
         Lists all enabled features in a course.
 
         :calls: `GET /api/v1/courses/:course_id/features/enabled \
         <https://canvas.instructure.com/doc/api/feature_flags.html#method.feature_flags.enabled_features>`_
 
-        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
-            :class:`canvasapi.feature.Feature`
+        :rtype: `list` of `str`
         """
-        return PaginatedList(
-            Feature,
-            self._requester,
+        response = self._requester.request(
             "GET",
             "courses/{}/features/enabled".format(self.id),
-            {"course_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
         )
 
+        return response.json()
+
     def get_enrollments(self, **kwargs):
         """
         List all of the enrollments in this course.
 
         :calls: `GET /api/v1/courses/:course_id/enrollments \
         <https://canvas.instructure.com/doc/api/enrollments.html#method.enrollments_api.index>`_
 
@@ -1196,16 +1186,14 @@
 
         :calls: `GET /api/v1/courses/:course_id/external_feeds \
         <https://canvas.instructure.com/doc/api/announcement_external_feeds.html#method.external_feeds.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.external_feed.ExternalFeed`
         """
-        from canvasapi.external_feed import ExternalFeed
-
         return PaginatedList(
             ExternalFeed,
             self._requester,
             "GET",
             "courses/{}/external_feeds".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1649,21 +1637,22 @@
         <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.show>`_
 
         :param module: The object or ID of the module to retrieve.
         :type module: :class:`canvasapi.module.Module` or int
 
         :rtype: :class:`canvasapi.module.Module`
         """
-        from canvasapi.module import Module
-
         module_id = obj_or_id(module, "module", (Module,))
 
         response = self._requester.request(
-            "GET", "courses/{}/modules/{}".format(self.id, module_id)
+            "GET",
+            "courses/{}/modules/{}".format(self.id, module_id),
+            _kwargs=combine_kwargs(**kwargs),
         )
+
         module_json = response.json()
         module_json.update({"course_id": self.id})
 
         return Module(self._requester, module_json)
 
     def get_modules(self, **kwargs):
         """
@@ -1671,16 +1660,14 @@
 
         :calls: `GET /api/v1/courses/:course_id/modules \
         <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.module.Module`
         """
-        from canvasapi.module import Module
-
         return PaginatedList(
             Module,
             self._requester,
             "GET",
             "courses/{}/modules".format(self.id),
             {"course_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
@@ -2378,14 +2365,32 @@
         response = self._requester.request(
             "POST",
             "courses/{}/preview_html".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.json().get("html", "")
 
+    def query_audit_by_course(self, **kwargs):
+        """
+        Lists course change events for a specific course.
+
+        :calls: `GET /api/v1/audit/course/courses/:course_id \
+        <https://canvas.instructure.com/doc/api/course_audit_log.html#method.course_audit_api.for_course>`_
+
+        :rtype: list of :class:`canvasapi.course_event.CourseEvent`
+        """
+
+        return PaginatedList(
+            CourseEvent,
+            self._requester,
+            "GET",
+            "audit/course/courses/{}".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
     def remove_usage_rights(self, **kwargs):
         """
         Removes the usage rights for specified files that are under the current course scope
 
         :calls: `DELETE /api/v1/courses/:course_id/usage_rights \
         <https://canvas.instructure.com/doc/api/files.html#method.usage_rights.remove_usage_rights>`_
```

### Comparing `canvasapi-3.0.0/canvasapi/current_user.py` & `canvasapi-3.1.0/canvasapi/current_user.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/custom_gradebook_columns.py` & `canvasapi-3.1.0/canvasapi/custom_gradebook_columns.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/discussion_topic.py` & `canvasapi-3.1.0/canvasapi/discussion_topic.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/enrollment.py` & `canvasapi-3.1.0/canvasapi/enrollment.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,31 @@
 from canvasapi.util import combine_kwargs
 
 
 class Enrollment(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.type, self.id)
 
+    def accept(self, **kwargs):
+        """
+        Accept a pending course invitation.
+
+        :calls: `POST /api/v1/courses/:course_id/enrollments/:id/accept \
+        <https://canvas.instructure.com/doc/api/enrollments.html#method.enrollments_api.accept>`_
+
+        :returns: True if the course invitation was accepted.
+        :rtype: bool
+        """
+        response = self._requester.request(
+            "POST",
+            "courses/{}/enrollments/{}/accept".format(self.course_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return response.json().get("success", False)
+
     def deactivate(self, task, **kwargs):
         """
         Delete, conclude, or deactivate an enrollment.
 
         The following tasks can be performed on an enrollment: conclude, delete, \
         inactivate, deactivate.
 
@@ -49,7 +66,24 @@
         """
         response = self._requester.request(
             "PUT",
             "courses/{}/enrollments/{}/reactivate".format(self.course_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return Enrollment(self._requester, response.json())
+
+    def reject(self, **kwargs):
+        """
+        Reject a pending course invitation.
+
+        :calls: `POST /api/v1/courses/:course_id/enrollments/:id/reject \
+        <https://canvas.instructure.com/doc/api/enrollments.html#method.enrollments_api.reject>`_
+
+        :returns: True if the course invitation was rejected.
+        :rtype: bool
+        """
+        response = self._requester.request(
+            "POST",
+            "courses/{}/enrollments/{}/reject".format(self.course_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return response.json().get("success", False)
```

### Comparing `canvasapi-3.0.0/canvasapi/enrollment_term.py` & `canvasapi-3.1.0/canvasapi/enrollment_term.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from canvasapi.util import combine_kwargs
 
 
 class EnrollmentTerm(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.name, self.id)
 
-    def delete(self):
+    def delete(self, **kwargs):
         """
         Delete this Enrollment Term.
 
         :calls: `DELETE /api/v1/accounts/:account_id/terms/:id \
         <https://canvas.instructure.com/doc/api/enrollment_terms.html#method.terms.destroy>`_
 
         :rtype: :class:`canvasapi.enrollment_term.EnrollmentTerm`
         """
         response = self._requester.request(
-            "DELETE", "accounts/{}/terms/{}".format(self.account_id, self.id)
+            "DELETE",
+            "accounts/{}/terms/{}".format(self.account_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
         return EnrollmentTerm(self._requester, response.json())
 
     def edit(self, **kwargs):
         """
         Modify this Enrollment Term.
```

### Comparing `canvasapi-3.0.0/canvasapi/eportfolio.py` & `canvasapi-3.1.0/canvasapi/eportfolio.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/exceptions.py` & `canvasapi-3.1.0/canvasapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/external_tool.py` & `canvasapi-3.1.0/canvasapi/external_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,33 +31,15 @@
         if hasattr(self, "course_id"):
             return "course"
         elif hasattr(self, "account_id"):
             return "account"
         else:
             raise ValueError("ExternalTool does not have a course_id or account_id")
 
-    def get_parent(self):
-        """
-        Return the object that spawned this tool.
-
-        :rtype: :class:`canvasapi.account.Account` or :class:`canvasapi.account.Course`
-        """
-        from canvasapi.account import Account
-        from canvasapi.course import Course
-
-        response = self._requester.request(
-            "GET", "{}s/{}".format(self.parent_type, self.parent_id)
-        )
-
-        if self.parent_type == "account":
-            return Account(self._requester, response.json())
-        elif self.parent_type == "course":
-            return Course(self._requester, response.json())
-
-    def delete(self):
+    def delete(self, **kwargs):
         """
         Remove the specified external tool.
 
         :calls: `DELETE /api/v1/courses/:course_id/external_tools/:external_tool_id
             <https://canvas.instructure.com/doc/api/external_tools.html#method.external_tools.destroy>`_
             or `DELETE /api/v1/accounts/:account_id/external_tools/:external_tool_id
             <https://canvas.instructure.com/doc/api/external_tools.html#method.external_tools.destroy>`_
@@ -65,14 +47,15 @@
         :rtype: :class:`canvasapi.external_tool.ExternalTool`
         """
         response = self._requester.request(
             "DELETE",
             "{}s/{}/external_tools/{}".format(
                 self.parent_type, self.parent_id, self.id
             ),
+            _kwargs=combine_kwargs(**kwargs),
         )
 
         return ExternalTool(self._requester, response.json())
 
     def edit(self, **kwargs):
         """
         Update the specified external tool.
@@ -94,14 +77,34 @@
         response_json = response.json()
 
         if "name" in response_json:
             super(ExternalTool, self).set_attributes(response_json)
 
         return ExternalTool(self._requester, response_json)
 
+    def get_parent(self, **kwargs):
+        """
+        Return the object that spawned this tool.
+
+        :rtype: :class:`canvasapi.account.Account` or :class:`canvasapi.account.Course`
+        """
+        from canvasapi.account import Account
+        from canvasapi.course import Course
+
+        response = self._requester.request(
+            "GET",
+            "{}s/{}".format(self.parent_type, self.parent_id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        if self.parent_type == "account":
+            return Account(self._requester, response.json())
+        elif self.parent_type == "course":
+            return Course(self._requester, response.json())
+
     def get_sessionless_launch_url(self, **kwargs):
         """
         Return a sessionless launch url for an external tool.
 
         :calls: `GET /api/v1/courses/:course_id/external_tools/sessionless_launch
             <https://canvas.instructure.com/doc/api/external_tools.html#method.external_tools.generate_sessionless_launch>`_
             or `GET /api/v1/accounts/:account_id/external_tools/sessionless_launch \
```

### Comparing `canvasapi-3.0.0/canvasapi/favorite.py` & `canvasapi-3.1.0/canvasapi/favorite.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/feature.py` & `canvasapi-3.1.0/canvasapi/feature.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/file.py` & `canvasapi-3.1.0/canvasapi/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,21 @@
         :rtype: str or bytes
         """
         response = self._requester.request("GET", _url=self.url)
         if binary:
             return response.content
         else:
             return response.text
+
+    def update(self, **kwargs):
+        """
+        Update some settings on the specified file.
+
+        :calls: `PUT /api/v1/files/:id \
+        <https://canvas.instructure.com/doc/api/files.html#method.files.api_update>`_
+
+        :rtype: :class:`canvasapi.file.File`
+        """
+        response = self._requester.request(
+            "PUT", "files/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
+        )
+        return File(self._requester, response.json())
```

### Comparing `canvasapi-3.0.0/canvasapi/folder.py` & `canvasapi-3.1.0/canvasapi/folder.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/grading_period.py` & `canvasapi-3.1.0/canvasapi/grading_period.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/group.py` & `canvasapi-3.1.0/canvasapi/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from canvasapi.canvas_object import CanvasObject
 from canvasapi.collaboration import Collaboration
 from canvasapi.discussion_topic import DiscussionTopic
 from canvasapi.exceptions import RequiredFieldMissing
+from canvasapi.external_feed import ExternalFeed
 from canvasapi.folder import Folder
 from canvasapi.license import License
 from canvasapi.paginated_list import PaginatedList
 from canvasapi.tab import Tab
 from canvasapi.upload import FileOrPathLike, Uploader
 from canvasapi.usage_rights import UsageRights
 from canvasapi.util import combine_kwargs, is_multivalued, obj_or_id
@@ -74,16 +75,14 @@
         :calls: `POST /api/v1/groups/:group_id/external_feeds \
         <https://canvas.instructure.com/doc/api/announcement_external_feeds.html#method.external_feeds.create>`_
 
         :param url: The urlof the external rss or atom feed
         :type url: str
         :rtype: :class:`canvasapi.external_feed.ExternalFeed`
         """
-        from canvasapi.external_feed import ExternalFeed
-
         response = self._requester.request(
             "POST",
             "groups/{}/external_feeds".format(self.id),
             url=url,
             _kwargs=combine_kwargs(**kwargs),
         )
         return ExternalFeed(self._requester, response.json())
```

### Comparing `canvasapi-3.0.0/canvasapi/login.py` & `canvasapi-3.1.0/canvasapi/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from canvasapi.util import combine_kwargs
 
 
 class Login(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.id, self.unique_id)
 
-    def delete(self):
+    def delete(self, **kwargs):
         """
         Delete an existing login.
 
         :calls: `DELETE /api/v1/users/:user_id/logins/:id \
         <https://canvas.instructure.com/doc/api/logins.html#method.pseudonyms.destroy>`_
 
         :rtype: :class:`canvasapi.login.Login`
         """
         response = self._requester.request(
-            "DELETE", "users/{}/logins/{}".format(self.user_id, self.id)
+            "DELETE",
+            "users/{}/logins/{}".format(self.user_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
         return Login(self._requester, response.json())
 
     def edit(self, **kwargs):
         """
         Update an existing login for a user in the given account.
```

### Comparing `canvasapi-3.0.0/canvasapi/module.py` & `canvasapi-3.1.0/canvasapi/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,90 +4,88 @@
 from canvasapi.util import combine_kwargs, obj_or_id
 
 
 class Module(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.name, self.id)
 
-    def edit(self, **kwargs):
+    def create_module_item(self, module_item, **kwargs):
         """
-        Update this module.
+        Create a module item.
 
-        :calls: `PUT /api/v1/courses/:course_id/modules/:id \
-        <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.update>`_
+        :calls: `POST /api/v1/courses/:course_id/modules/:module_id/items \
+        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.create>`_
 
-        :rtype: :class:`canvasapi.module.Module`
+        :param module_item: The attributes to create the module item with.
+        :type module_item: dict
+        :returns: The created module item.
+        :rtype: :class:`canvasapi.module.ModuleItem`
         """
+
+        unrequired_types = ["ExternalUrl", "Page", "SubHeader"]
+
+        if isinstance(module_item, dict) and "type" in module_item:
+            # content_id is not required for unrequired_types
+            if module_item["type"] in unrequired_types or "content_id" in module_item:
+                kwargs["module_item"] = module_item
+            else:
+                raise RequiredFieldMissing(
+                    "Dictionary with key 'content_id' is required."
+                )
+        else:
+            raise RequiredFieldMissing("Dictionary with key 'type' is required.")
+
         response = self._requester.request(
-            "PUT",
-            "courses/{}/modules/{}".format(self.course_id, self.id),
+            "POST",
+            "courses/{}/modules/{}/items".format(self.course_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
-        module_json = response.json()
-        module_json.update({"course_id": self.course_id})
+        module_item_json = response.json()
+        module_item_json.update({"course_id": self.course_id})
 
-        return Module(self._requester, module_json)
+        return ModuleItem(self._requester, module_item_json)
 
-    def delete(self):
+    def delete(self, **kwargs):
         """
         Delete this module.
 
         :calls: `DELETE /api/v1/courses/:course_id/modules/:id \
         <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.destroy>`_
 
         :rtype: :class:`canvasapi.module.Module`
         """
         response = self._requester.request(
-            "DELETE", "courses/{}/modules/{}".format(self.course_id, self.id)
+            "DELETE",
+            "courses/{}/modules/{}".format(self.course_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
         module_json = response.json()
         module_json.update({"course_id": self.course_id})
 
         return Module(self._requester, module_json)
 
-    def relock(self):
+    def edit(self, **kwargs):
         """
-        Reset module progressions to their default locked state and recalculates
-        them based on the current requirements.
-
-        Adding progression requirements to an active course will not lock students
-        out of modules they have already unlocked unless this action is called.
+        Update this module.
 
-        :calls: `PUT /api/v1/courses/:course_id/modules/:id/relock \
-        <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.relock>`_
+        :calls: `PUT /api/v1/courses/:course_id/modules/:id \
+        <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.update>`_
 
         :rtype: :class:`canvasapi.module.Module`
         """
         response = self._requester.request(
-            "PUT", "courses/{}/modules/{}/relock".format(self.course_id, self.id)
+            "PUT",
+            "courses/{}/modules/{}".format(self.course_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
         module_json = response.json()
         module_json.update({"course_id": self.course_id})
 
         return Module(self._requester, module_json)
 
-    def get_module_items(self, **kwargs):
-        """
-        List all of the items in this module.
-
-        :calls: `GET /api/v1/courses/:course_id/modules/:module_id/items \
-        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.index>`_
-
-        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
-            :class:`canvasapi.module.ModuleItem`
-        """
-        return PaginatedList(
-            ModuleItem,
-            self._requester,
-            "GET",
-            "courses/{}/modules/{}/items".format(self.course_id, self.id),
-            {"course_id": self.course_id},
-            _kwargs=combine_kwargs(**kwargs),
-        )
-
     def get_module_item(self, module_item, **kwargs):
         """
         Retrieve a module item by ID.
 
         :calls: `GET /api/v1/courses/:course_id/modules/:module_id/items/:id \
         <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.show>`_
 
@@ -106,129 +104,138 @@
             _kwargs=combine_kwargs(**kwargs),
         )
         module_item_json = response.json()
         module_item_json.update({"course_id": self.course_id})
 
         return ModuleItem(self._requester, module_item_json)
 
-    def create_module_item(self, module_item, **kwargs):
+    def get_module_items(self, **kwargs):
         """
-        Create a module item.
+        List all of the items in this module.
 
-        :calls: `POST /api/v1/courses/:course_id/modules/:module_id/items \
-        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.create>`_
+        :calls: `GET /api/v1/courses/:course_id/modules/:module_id/items \
+        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.index>`_
 
-        :param module_item: The attributes to create the module item with.
-        :type module_item: dict
-        :returns: The created module item.
-        :rtype: :class:`canvasapi.module.ModuleItem`
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.module.ModuleItem`
         """
+        return PaginatedList(
+            ModuleItem,
+            self._requester,
+            "GET",
+            "courses/{}/modules/{}/items".format(self.course_id, self.id),
+            {"course_id": self.course_id},
+            _kwargs=combine_kwargs(**kwargs),
+        )
 
-        unrequired_types = ["ExternalUrl", "Page", "SubHeader"]
+    def relock(self, **kwargs):
+        """
+        Reset module progressions to their default locked state and recalculates
+        them based on the current requirements.
 
-        if isinstance(module_item, dict) and "type" in module_item:
-            # content_id is not required for unrequired_types
-            if module_item["type"] in unrequired_types or "content_id" in module_item:
-                kwargs["module_item"] = module_item
-            else:
-                raise RequiredFieldMissing(
-                    "Dictionary with key 'content_id' is required."
-                )
-        else:
-            raise RequiredFieldMissing("Dictionary with key 'type' is required.")
+        Adding progression requirements to an active course will not lock students
+        out of modules they have already unlocked unless this action is called.
 
+        :calls: `PUT /api/v1/courses/:course_id/modules/:id/relock \
+        <https://canvas.instructure.com/doc/api/modules.html#method.context_modules_api.relock>`_
+
+        :rtype: :class:`canvasapi.module.Module`
+        """
         response = self._requester.request(
-            "POST",
-            "courses/{}/modules/{}/items".format(self.course_id, self.id),
+            "PUT",
+            "courses/{}/modules/{}/relock".format(self.course_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
-        module_item_json = response.json()
-        module_item_json.update({"course_id": self.course_id})
+        module_json = response.json()
+        module_json.update({"course_id": self.course_id})
 
-        return ModuleItem(self._requester, module_item_json)
+        return Module(self._requester, module_json)
 
 
 class ModuleItem(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.title, self.id)
 
-    def edit(self, **kwargs):
+    def complete(self, **kwargs):
         """
-        Update this module item.
+        Mark this module item as done.
 
-        :calls: `PUT /api/v1/courses/:course_id/modules/:module_id/items/:id \
-        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.update>`_
+        :calls: `PUT /api/v1/courses/:course_id/modules/:module_id/items/:id/done \
+        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.mark_as_done>`_
 
-        :returns: The updated module item.
         :rtype: :class:`canvasapi.module.ModuleItem`
         """
         response = self._requester.request(
             "PUT",
-            "courses/{}/modules/{}/items/{}".format(
+            "courses/{}/modules/{}/items/{}/done".format(
                 self.course_id, self.module_id, self.id
             ),
             _kwargs=combine_kwargs(**kwargs),
         )
         module_item_json = response.json()
         module_item_json.update({"course_id": self.course_id})
 
         return ModuleItem(self._requester, module_item_json)
 
-    def delete(self):
+    def delete(self, **kwargs):
         """
         Delete this module item.
 
         :calls: `DELETE /api/v1/courses/:course_id/modules/:module_id/items/:id \
         <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.destroy>`_
 
         :rtype: :class:`canvasapi.module.ModuleItem`
         """
         response = self._requester.request(
             "DELETE",
             "courses/{}/modules/{}/items/{}".format(
                 self.course_id, self.module_id, self.id
             ),
+            _kwargs=combine_kwargs(**kwargs),
         )
         module_item_json = response.json()
         module_item_json.update({"course_id": self.course_id})
 
         return ModuleItem(self._requester, module_item_json)
 
-    def complete(self):
+    def edit(self, **kwargs):
         """
-        Mark this module item as done.
+        Update this module item.
 
-        :calls: `PUT /api/v1/courses/:course_id/modules/:module_id/items/:id/done \
-        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.mark_as_done>`_
+        :calls: `PUT /api/v1/courses/:course_id/modules/:module_id/items/:id \
+        <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.update>`_
 
+        :returns: The updated module item.
         :rtype: :class:`canvasapi.module.ModuleItem`
         """
         response = self._requester.request(
             "PUT",
-            "courses/{}/modules/{}/items/{}/done".format(
+            "courses/{}/modules/{}/items/{}".format(
                 self.course_id, self.module_id, self.id
             ),
+            _kwargs=combine_kwargs(**kwargs),
         )
         module_item_json = response.json()
         module_item_json.update({"course_id": self.course_id})
 
         return ModuleItem(self._requester, module_item_json)
 
-    def uncomplete(self):
+    def uncomplete(self, **kwargs):
         """
         Mark this module item as not done.
 
         :calls: `DELETE /api/v1/courses/:course_id/modules/:module_id/items/:id/done \
         <https://canvas.instructure.com/doc/api/modules.html#method.context_module_items_api.mark_as_done>`_
 
         :rtype: :class:`canvasapi.module.ModuleItem`
         """
         response = self._requester.request(
             "DELETE",
             "courses/{}/modules/{}/items/{}/done".format(
                 self.course_id, self.module_id, self.id
             ),
+            _kwargs=combine_kwargs(**kwargs),
         )
         module_item_json = response.json()
         module_item_json.update({"course_id": self.course_id})
 
         return ModuleItem(self._requester, module_item_json)
```

### Comparing `canvasapi-3.0.0/canvasapi/outcome.py` & `canvasapi-3.1.0/canvasapi/outcome.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,30 +35,32 @@
 
     def context_ref(self):
         if self.context_type == "Course":
             return "courses/{}".format(self.context_id)
         elif self.context_type == "Account":
             return "accounts/{}".format(self.context_id)
 
-    def get_outcome(self):
+    def get_outcome(self, **kwargs):
         """
         Return the linked outcome
 
         :calls: `GET /api/v1/outcomes/:id \
         <https://canvas.instructure.com/doc/api/outcomes.html#method.outcomes_api.show>`_
 
         :returns: Outcome object that was in the OutcomeLink
         :rtype: :class:`canvasapi.outcome.Outcome`
         """
         oid = self.outcome["id"]
-        response = self._requester.request("GET", "outcomes/{}".format(oid))
+        response = self._requester.request(
+            "GET", "outcomes/{}".format(oid), _kwargs=combine_kwargs(**kwargs)
+        )
 
         return Outcome(self._requester, response.json())
 
-    def get_outcome_group(self):
+    def get_outcome_group(self, **kwargs):
         """
         Return the linked outcome group
 
         :calls: `GET /api/v1/global/outcome_groups/:id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.show>`_
             or `GET /api/v1/accounts/:account_id/outcome_groups/:id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.show>`_
@@ -66,15 +68,17 @@
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.show>`_
 
         :returns: Linked outcome group object.
         :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
         ogid = self.outcome_group["id"]
         response = self._requester.request(
-            "GET", "{}/outcome_groups/{}".format(self.context_ref(), ogid)
+            "GET",
+            "{}/outcome_groups/{}".format(self.context_ref(), ogid),
+            _kwargs=combine_kwargs(**kwargs),
         )
 
         return OutcomeGroup(self._requester, response.json())
 
 
 class OutcomeGroup(CanvasObject):
     def __str__(self):
@@ -84,55 +88,58 @@
         if self.context_type == "Course":
             return "courses/{}".format(self.context_id)
         elif self.context_type == "Account":
             return "accounts/{}".format(self.context_id)
         elif self.context_type is None:
             return "global"
 
-    def update(self, **kwargs):
+    def create_subgroup(self, title, **kwargs):
         """
-        Update an outcome group.
+        Create a subgroup of the current group
 
-        :calls: `PUT /api/v1/global/outcome_groups/:id \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.update>`_
-            or `PUT /api/v1/accounts/:account_id/outcome_groups/:id \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.update>`_
-            or `PUT /api/v1/courses/:course_id/outcome_groups/:id \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.update>`_
+        :calls: `POST /api/v1/global/outcome_groups/:id/subgroups \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.create>`_
+            or `POST /api/v1/accounts/:account_id/outcome_groups/:id/subgroups \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.create>`_
+            or `POST /api/v1/courses/:course_id/outcome_groups/:id/subgroups \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.create>`_
 
-        :returns: True if updated, False otherwise.
-        :rtype: bool
+        :param title: The title of the subgroup.
+        :type title: str
+
+        :returns: Itself as an OutcomeGroup object.
+        :rtype: :class:`canvasapi.outcome.OutcomeGroup`
         """
         response = self._requester.request(
-            "PUT",
-            "{}/outcome_groups/{}".format(self.context_ref(), self.id),
+            "POST",
+            "{}/outcome_groups/{}/subgroups".format(self.context_ref(), self.id),
+            title=title,
             _kwargs=combine_kwargs(**kwargs),
         )
 
-        if "id" in response.json():
-            super(OutcomeGroup, self).set_attributes(response.json())
-
-        return "id" in response.json()
+        return OutcomeGroup(self._requester, response.json())
 
-    def delete(self):
+    def delete(self, **kwargs):
         """
         Delete an outcome group.
 
         :calls: `DELETE /api/v1/global/outcome_groups/:id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.destroy>`_
             or `DELETE /api/v1/accounts/:account_id/outcome_groups/:id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.destroy>`_
             or `DELETE /api/v1/courses/:course_id/outcome_groups/:id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.destroy>`_
 
         :returns: True if successful, false if failed.
         :rtype: bool
         """
         response = self._requester.request(
-            "DELETE", "{}/outcome_groups/{}".format(self.context_ref(), self.id)
+            "DELETE",
+            "{}/outcome_groups/{}".format(self.context_ref(), self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
 
         if "id" in response.json():
             super(OutcomeGroup, self).set_attributes(response.json())
 
         return "id" in response.json()
 
@@ -155,15 +162,69 @@
             OutcomeLink,
             self._requester,
             "GET",
             "{}/outcome_groups/{}/outcomes".format(self.context_ref(), self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
-    def link_existing(self, outcome):
+    def get_subgroups(self, **kwargs):
+        """
+        List subgroups.
+
+        :calls: `GET /api/v1/global/outcome_groups/:id/subgroups \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.subgroups>`_
+            or `GET /api/v1/accounts/:account_id/outcome_groups/:id/subgroups \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.subgroups>`_
+            or `GET /api/v1/courses/:course_id/outcome_groups/:id/subgroups \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.subgroups>`_
+
+        :returns: Paginated List of OutcomeGroups linked to the current group.
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.outcome.OutcomeGroup`
+        """
+        return PaginatedList(
+            OutcomeGroup,
+            self._requester,
+            "GET",
+            "{}/outcome_groups/{}/subgroups".format(self.context_ref(), self.id),
+            {"context_type": self.context_type, "context_id": self.context_id},
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+    def import_outcome_group(self, outcome_group, **kwargs):
+        """
+        Import an outcome group as a subgroup into the current outcome group
+
+        :calls: `POST /api/v1/global/outcome_groups/:id/import \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.import>`_
+            or `POST /api/v1/accounts/:account_id/outcome_groups/:id/import \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.import>`_
+            or `POST /api/v1/courses/:course_id/outcome_groups/:id/import \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.import>`_
+
+        :param outcome: The object or ID of the outcome group to import.
+        :type outcome: :class:`canvasapi.outcome.OutcomeGroup` or int
+
+        :returns: Itself as an OutcomeGroup object.
+        :rtype: :class:`canvasapi.outcome.OutcomeGroup`
+        """
+        source_outcome_group_id = obj_or_id(
+            outcome_group, "outcome_group", (OutcomeGroup,)
+        )
+
+        response = self._requester.request(
+            "POST",
+            "{}/outcome_groups/{}/import".format(self.context_ref(), self.id),
+            source_outcome_group_id=source_outcome_group_id,
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        return OutcomeGroup(self._requester, response.json())
+
+    def link_existing(self, outcome, **kwargs):
         """
         Link to an existing Outcome.
 
         :calls: `PUT /api/v1/global/outcome_groups/:id/outcomes/:outcome_id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.link>`_
             or `PUT /api/v1/accounts/:account_id/outcome_groups/:id/outcomes/:outcome_id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.link>`_
@@ -177,16 +238,19 @@
         :rtype: :class:`canvasapi.outcome.OutcomeLink`
         """
         outcome_id = obj_or_id(outcome, "outcome", (Outcome,))
 
         response = self._requester.request(
             "PUT",
             "{}/outcome_groups/{}/outcomes/{}".format(
-                self.context_ref(), self.id, outcome_id
+                self.context_ref(),
+                self.id,
+                outcome_id,
             ),
+            _kwargs=combine_kwargs(**kwargs),
         )
 
         return OutcomeLink(self._requester, response.json())
 
     def link_new(self, title, **kwargs):
         """
         Create a new Outcome and link it to this OutcomeGroup
@@ -209,15 +273,15 @@
             "{}/outcome_groups/{}/outcomes".format(self.context_ref(), self.id),
             title=title,
             _kwargs=combine_kwargs(**kwargs),
         )
 
         return OutcomeLink(self._requester, response.json())
 
-    def unlink_outcome(self, outcome):
+    def unlink_outcome(self, outcome, **kwargs):
         """
         Remove an Outcome from and OutcomeLink
 
         :calls: `DELETE /api/v1/global/outcome_groups/:id/outcomes/:outcome_id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.unlink>`_
             or `DELETE /api/v1/accounts/:account_id/outcome_groups/:id/outcomes/:outcome_id \
             <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.unlink>`_
@@ -231,99 +295,48 @@
         :rtype: bool
         """
         outcome_id = obj_or_id(outcome, "outcome", (Outcome,))
 
         response = self._requester.request(
             "DELETE",
             "{}/outcome_groups/{}/outcomes/{}".format(
-                self.context_ref(), self.id, outcome_id
+                self.context_ref(),
+                self.id,
+                outcome_id,
             ),
+            _kwargs=combine_kwargs(**kwargs),
         )
 
         if "context_id" in response.json():
             super(OutcomeGroup, self).set_attributes(response.json())
 
         return "context_id" in response.json()
 
-    def get_subgroups(self, **kwargs):
-        """
-        List subgroups.
-
-        :calls: `GET /api/v1/global/outcome_groups/:id/subgroups \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.subgroups>`_
-            or `GET /api/v1/accounts/:account_id/outcome_groups/:id/subgroups \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.subgroups>`_
-            or `GET /api/v1/courses/:course_id/outcome_groups/:id/subgroups \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.subgroups>`_
-
-        :returns: Paginated List of OutcomeGroups linked to the current group.
-        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
-            :class:`canvasapi.outcome.OutcomeGroup`
-        """
-        return PaginatedList(
-            OutcomeGroup,
-            self._requester,
-            "GET",
-            "{}/outcome_groups/{}/subgroups".format(self.context_ref(), self.id),
-            {"context_type": self.context_type, "context_id": self.context_id},
-            _kwargs=combine_kwargs(**kwargs),
-        )
-
-    def create_subgroup(self, title, **kwargs):
+    def update(self, **kwargs):
         """
-        Create a subgroup of the current group
-
-        :calls: `POST /api/v1/global/outcome_groups/:id/subgroups \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.create>`_
-            or `POST /api/v1/accounts/:account_id/outcome_groups/:id/subgroups \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.create>`_
-            or `POST /api/v1/courses/:course_id/outcome_groups/:id/subgroups \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.create>`_
+        Update an outcome group.
 
-        :param title: The title of the subgroup.
-        :type title: str
+        :calls: `PUT /api/v1/global/outcome_groups/:id \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.update>`_
+            or `PUT /api/v1/accounts/:account_id/outcome_groups/:id \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.update>`_
+            or `PUT /api/v1/courses/:course_id/outcome_groups/:id \
+            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.update>`_
 
-        :returns: Itself as an OutcomeGroup object.
-        :rtype: :class:`canvasapi.outcome.OutcomeGroup`
+        :returns: True if updated, False otherwise.
+        :rtype: bool
         """
         response = self._requester.request(
-            "POST",
-            "{}/outcome_groups/{}/subgroups".format(self.context_ref(), self.id),
-            title=title,
+            "PUT",
+            "{}/outcome_groups/{}".format(self.context_ref(), self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
-        return OutcomeGroup(self._requester, response.json())
-
-    def import_outcome_group(self, outcome_group):
-        """
-        Import an outcome group as a subgroup into the current outcome group
-
-        :calls: `POST /api/v1/global/outcome_groups/:id/import \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.import>`_
-            or `POST /api/v1/accounts/:account_id/outcome_groups/:id/import \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.import>`_
-            or `POST /api/v1/courses/:course_id/outcome_groups/:id/import \
-            <https://canvas.instructure.com/doc/api/outcome_groups.html#method.outcome_groups_api.import>`_
-
-        :param outcome: The object or ID of the outcome group to import.
-        :type outcome: :class:`canvasapi.outcome.OutcomeGroup` or int
-
-        :returns: Itself as an OutcomeGroup object.
-        :rtype: :class:`canvasapi.outcome.OutcomeGroup`
-        """
-        source_outcome_group_id = obj_or_id(
-            outcome_group, "outcome_group", (OutcomeGroup,)
-        )
-
-        response = self._requester.request(
-            "POST",
-            "{}/outcome_groups/{}/import".format(self.context_ref(), self.id),
-            source_outcome_group_id=source_outcome_group_id,
-        )
+        if "id" in response.json():
+            super(OutcomeGroup, self).set_attributes(response.json())
 
-        return OutcomeGroup(self._requester, response.json())
+        return "id" in response.json()
 
 
 class OutcomeResult(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.id, self.score)
```

### Comparing `canvasapi-3.0.0/canvasapi/page.py` & `canvasapi-3.1.0/canvasapi/page.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/paginated_list.py` & `canvasapi-3.1.0/canvasapi/paginated_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         requester,
         request_method,
         first_url,
         extra_attribs=None,
         _root=None,
         **kwargs
     ):
-
         self._elements = list()
 
         self._requester = requester
         self._content_class = content_class
         self._first_url = first_url
         self._first_params = kwargs or {}
         self._first_params["per_page"] = kwargs.get("per_page", 100)
```

### Comparing `canvasapi-3.0.0/canvasapi/planner.py` & `canvasapi-3.1.0/canvasapi/planner.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,77 +2,77 @@
 from canvasapi.util import combine_kwargs
 
 
 class PlannerNote(CanvasObject):
     def __str__(self):
         return "{} {} ({})".format(self.title, self.todo_date, self.id)
 
-    def update(self, **kwargs):
+    def delete(self, **kwargs):
         """
-        Update a planner note for the current user
+        Delete a planner note for the current user
 
-        :calls: `PUT /api/v1/planner_notes/:id \
-        <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.update>`_
+        :calls: `DELETE /api/v1/planner_notes/:id \
+        <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.destroy>`_
 
         :rtype: :class:`canvasapi.planner.PlannerNote`
         """
-
         response = self._requester.request(
-            "PUT", "planner_notes/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
+            "DELETE",
+            "planner_notes/{}".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
+
         return PlannerNote(self._requester, response.json())
 
-    def delete(self, **kwargs):
+    def update(self, **kwargs):
         """
-        Delete a planner note for the current user
+        Update a planner note for the current user
 
-        :calls: `DELETE /api/v1/planner_notes/:id \
-        <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.destroy>`_
+        :calls: `PUT /api/v1/planner_notes/:id \
+        <https://canvas.instructure.com/doc/api/planner.html#method.planner_notes.update>`_
 
         :rtype: :class:`canvasapi.planner.PlannerNote`
         """
+
         response = self._requester.request(
-            "DELETE",
-            "planner_notes/{}".format(self.id),
-            _kwargs=combine_kwargs(**kwargs),
+            "PUT", "planner_notes/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
         )
-
         return PlannerNote(self._requester, response.json())
 
 
 class PlannerOverride(CanvasObject):
     def __str__(self):
         return "{} {} ({})".format(self.plannable_id, self.marked_complete, self.id)
 
-    def update(self, **kwargs):
+    def delete(self, **kwargs):
         """
-        Update a planner override's visibilty for the current user
+        Delete a planner override for the current user
 
-        :calls: `PUT /api/v1/planner/overrides/:id \
-        <https://canvas.instructure.com/doc/api/planner.html#method.planner_overrides.update>`_
+        :calls: `DELETE /api/v1/planner/overrides/:id \
+        <https://canvas.instructure.com/doc/api/planner.html#method.planner_overrides.destroy>`_
 
         :rtype: :class:`canvasapi.planner.PlannerOverride`
         """
-
         response = self._requester.request(
-            "PUT",
+            "DELETE",
             "planner/overrides/{}".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
+
         return PlannerOverride(self._requester, response.json())
 
-    def delete(self, **kwargs):
+    def update(self, **kwargs):
         """
-        Delete a planner override for the current user
+        Update a planner override's visibilty for the current user
 
-        :calls: `DELETE /api/v1/planner/overrides/:id \
-        <https://canvas.instructure.com/doc/api/planner.html#method.planner_overrides.destroy>`_
+        :calls: `PUT /api/v1/planner/overrides/:id \
+        <https://canvas.instructure.com/doc/api/planner.html#method.planner_overrides.update>`_
 
         :rtype: :class:`canvasapi.planner.PlannerOverride`
         """
+
         response = self._requester.request(
-            "DELETE",
+            "PUT",
             "planner/overrides/{}".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
-
         return PlannerOverride(self._requester, response.json())
```

### Comparing `canvasapi-3.0.0/canvasapi/poll.py` & `canvasapi-3.1.0/canvasapi/poll.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,38 +6,70 @@
 from canvasapi.util import combine_kwargs, obj_or_id
 
 
 class Poll(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.question, self.id)
 
-    def update(self, poll, **kwargs):
+    def create_choice(self, poll_choice, **kwargs):
         """
-        Update an existing poll belonging to the current user.
+        Create a new choice for the current poll.
 
-        :calls: `PUT /api/v1/polls/:id \
-        <https://canvas.instructure.com/doc/api/polls.html#method.polling/polls.update>`_
+        :calls: `POST /api/v1/polls/:poll_id/poll_choices \
+        <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.create>`_
 
-        :param poll: List of arguments. 'Question' is required and 'Description' is optional
-        :type poll: list
-        :rtype: :class:`canvasapi.poll.Poll`
+        :param poll_choice: 'text' is required, 'is_correct' and 'position' are optional.
+        :type poll_choice: list
+        :rtype: :class:`canvasapi.poll_choice.PollChoice`
         """
         if (
-            isinstance(poll, list)
-            and isinstance(poll[0], dict)
-            and "question" in poll[0]
+            isinstance(poll_choice, list)
+            and isinstance(poll_choice[0], dict)
+            and "text" in poll_choice[0]
         ):
-            kwargs["poll"] = poll
+            kwargs["poll_choice"] = poll_choice
         else:
-            raise RequiredFieldMissing("Dictionary with key 'question' is required.")
+            raise RequiredFieldMissing("Dictionary with key 'text' is required.")
 
         response = self._requester.request(
-            "PUT", "polls/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
+            "POST",
+            "polls/{}/poll_choices".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
         )
-        return Poll(self._requester, response.json()["polls"][0])
+        return PollChoice(self._requester, response.json()["poll_choices"][0])
+
+    def create_session(self, poll_session, **kwargs):
+        """
+        Create a new poll session for this poll
+
+        :calls: `POST /api/v1/polls/:poll_id/poll_sessions \
+        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.create>`_
+
+        :param poll_session: List of arguments. course_id (required): id of the course for the
+            session, course_section_id (optional): id of the course section for this session,
+            has_public_results (optional): whether the results are viewable by students.
+        :type poll_session: list
+
+        :rtype: :class:`canvasapi.poll_session.PollSession`
+        """
+        if (
+            isinstance(poll_session, list)
+            and isinstance(poll_session[0], dict)
+            and "course_id" in poll_session[0]
+        ):
+            kwargs["poll_session"] = poll_session
+        else:
+            raise RequiredFieldMissing("Dictionary with key 'course_id' is required.")
+
+        response = self._requester.request(
+            "POST",
+            "polls/{}/poll_sessions".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return PollSession(self._requester, response.json()["poll_sessions"][0])
 
     def delete(self, **kwargs):
         """
         Delete a single poll, based on the poll id.
 
         :calls: `DELETE /api/v1/polls/:id \
         <https://canvas.instructure.com/doc/api/polls.html#method.polling/polls.destroy>`_
@@ -47,33 +79,14 @@
         :rtype: bool
         """
         response = self._requester.request(
             "DELETE", "polls/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
         )
         return response.status_code == 204
 
-    def get_choices(self, **kwargs):
-        """
-        Returns a paginated list of PollChoices of a poll, based on poll id.
-
-        :calls: `GET /api/v1/polls/:poll_id/poll_choices \
-        <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.index>`_
-
-        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
-            :class:`canvasapi.poll_choice.PollChoice`
-        """
-        return PaginatedList(
-            PollChoice,
-            self._requester,
-            "GET",
-            "polls/{}/poll_choices".format(self.id),
-            _root="poll_choices",
-            _kwargs=combine_kwargs(**kwargs),
-        )
-
     def get_choice(self, poll_choice, **kwargs):
         """
         Returns the poll choice with the given id.
 
         :calls: `GET /api/v1/polls/:poll_id/poll_choices/:id \
         <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.show>`_
 
@@ -84,57 +97,30 @@
         response = self._requester.request(
             "GET",
             "polls/{}/poll_choices/{}".format(self.id, poll_choice_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return PollChoice(self._requester, response.json()["poll_choices"][0])
 
-    def create_choice(self, poll_choice, **kwargs):
-        """
-        Create a new choice for the current poll.
-
-        :calls: `POST /api/v1/polls/:poll_id/poll_choices \
-        <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.create>`_
-
-        :param poll_choice: 'text' is required, 'is_correct' and 'position' are optional.
-        :type poll_choice: list
-        :rtype: :class:`canvasapi.poll_choice.PollChoice`
-        """
-        if (
-            isinstance(poll_choice, list)
-            and isinstance(poll_choice[0], dict)
-            and "text" in poll_choice[0]
-        ):
-            kwargs["poll_choice"] = poll_choice
-        else:
-            raise RequiredFieldMissing("Dictionary with key 'text' is required.")
-
-        response = self._requester.request(
-            "POST",
-            "polls/{}/poll_choices".format(self.id),
-            _kwargs=combine_kwargs(**kwargs),
-        )
-        return PollChoice(self._requester, response.json()["poll_choices"][0])
-
-    def get_sessions(self, **kwargs):
+    def get_choices(self, **kwargs):
         """
-        Returns the paginated list of PollSessions in a poll.
+        Returns a paginated list of PollChoices of a poll, based on poll id.
 
-        :calls: `GET /api/v1/polls/:poll_id/poll_sessions \
-        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.index>`_
+        :calls: `GET /api/v1/polls/:poll_id/poll_choices \
+        <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.index>`_
 
-        :rtype: :class:`canvasapi.paginated_lsit.Paginated List` of
-            :class:`canvasapi.poll_session.PollSession`
+        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
+            :class:`canvasapi.poll_choice.PollChoice`
         """
         return PaginatedList(
-            PollSession,
+            PollChoice,
             self._requester,
             "GET",
-            "polls/{}/poll_sessions".format(self.id),
-            _root="poll_sessions",
+            "polls/{}/poll_choices".format(self.id),
+            _root="poll_choices",
             _kwargs=combine_kwargs(**kwargs),
         )
 
     def get_session(self, poll_session, **kwargs):
         """
         Returns the poll session with the given id.
 
@@ -151,36 +137,50 @@
         response = self._requester.request(
             "GET",
             "polls/{}/poll_sessions/{}".format(self.id, poll_session_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return PollSession(self._requester, response.json()["poll_sessions"][0])
 
-    def create_session(self, poll_session, **kwargs):
+    def get_sessions(self, **kwargs):
         """
-        Create a new poll session for this poll
+        Returns the paginated list of PollSessions in a poll.
 
-        :calls: `POST /api/v1/polls/:poll_id/poll_sessions \
-        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.create>`_
+        :calls: `GET /api/v1/polls/:poll_id/poll_sessions \
+        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.index>`_
 
-        :param poll_session: List of arguments. course_id (required): id of the course for the
-            session, course_section_id (optional): id of the course section for this session,
-            has_public_results (optional): whether the results are viewable by students.
-        :type poll_session: list
+        :rtype: :class:`canvasapi.paginated_lsit.Paginated List` of
+            :class:`canvasapi.poll_session.PollSession`
+        """
+        return PaginatedList(
+            PollSession,
+            self._requester,
+            "GET",
+            "polls/{}/poll_sessions".format(self.id),
+            _root="poll_sessions",
+            _kwargs=combine_kwargs(**kwargs),
+        )
 
-        :rtype: :class:`canvasapi.poll_session.PollSession`
+    def update(self, poll, **kwargs):
+        """
+        Update an existing poll belonging to the current user.
+
+        :calls: `PUT /api/v1/polls/:id \
+        <https://canvas.instructure.com/doc/api/polls.html#method.polling/polls.update>`_
+
+        :param poll: List of arguments. 'Question' is required and 'Description' is optional
+        :type poll: list
+        :rtype: :class:`canvasapi.poll.Poll`
         """
         if (
-            isinstance(poll_session, list)
-            and isinstance(poll_session[0], dict)
-            and "course_id" in poll_session[0]
+            isinstance(poll, list)
+            and isinstance(poll[0], dict)
+            and "question" in poll[0]
         ):
-            kwargs["poll_session"] = poll_session
+            kwargs["poll"] = poll
         else:
-            raise RequiredFieldMissing("Dictionary with key 'course_id' is required.")
+            raise RequiredFieldMissing("Dictionary with key 'question' is required.")
 
         response = self._requester.request(
-            "POST",
-            "polls/{}/poll_sessions".format(self.id),
-            _kwargs=combine_kwargs(**kwargs),
+            "PUT", "polls/{}".format(self.id), _kwargs=combine_kwargs(**kwargs)
         )
-        return PollSession(self._requester, response.json()["poll_sessions"][0])
+        return Poll(self._requester, response.json()["polls"][0])
```

### Comparing `canvasapi-3.0.0/canvasapi/poll_choice.py` & `canvasapi-3.1.0/canvasapi/poll_choice.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 from canvasapi.util import combine_kwargs
 
 
 class PollChoice(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.text, self.id)
 
+    def delete(self, **kwargs):
+        """
+        Delete a single poll, based on the poll id.
+
+        :calls: `DELETE /api/v1/polls/:poll_id/poll_choices/:id \
+        <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.destroy>`_
+
+        :returns: True if the deletion was successful, false otherwise.
+
+        :rtype: bool
+        """
+        response = self._requester.request(
+            "DELETE",
+            "polls/{}/poll_choices/{}".format(self.poll_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return response.status_code == 204
+
     def update(self, poll_choice, **kwargs):
         """
         Update an existing choice for this poll.
 
         :calls: `PUT /api/v1/polls/:poll_id/poll_choices/:id \
         <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.update>`_
 
@@ -30,25 +48,7 @@
 
         response = self._requester.request(
             "PUT",
             "polls/{}/poll_choices/{}".format(self.poll_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return PollChoice(self._requester, response.json()["poll_choices"][0])
-
-    def delete(self, **kwargs):
-        """
-        Delete a single poll, based on the poll id.
-
-        :calls: `DELETE /api/v1/polls/:poll_id/poll_choices/:id \
-        <https://canvas.instructure.com/doc/api/poll_choices.html#method.polling/poll_choices.destroy>`_
-
-        :returns: True if the deletion was successful, false otherwise.
-
-        :rtype: bool
-        """
-        response = self._requester.request(
-            "DELETE",
-            "polls/{}/poll_choices/{}".format(self.poll_id, self.id),
-            _kwargs=combine_kwargs(**kwargs),
-        )
-        return response.status_code == 204
```

### Comparing `canvasapi-3.0.0/canvasapi/poll_session.py` & `canvasapi-3.1.0/canvasapi/poll_session.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,43 +4,60 @@
 from canvasapi.util import combine_kwargs, obj_or_id
 
 
 class PollSession(CanvasObject):
     def __str__(self):
         return "{} ({})".format(self.poll_id, self.id)
 
-    def update(self, poll_session, **kwargs):
+    def close(self, **kwargs):
         """
-        Update an existing poll session for a poll based on poll id.
+        Close a poll session to answers based on the poll id.
 
-        :calls: `PUT /api/v1/polls/:poll_id/poll_sessions/:id \
-        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.update>`_
+        :calls: `GET /api/v1/polls/:poll_id/poll_sessions/:id/close \
+        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.close>`_
 
-        :param poll_session: List of arguments. course_id (required): id of the course for the
-            session, course_section_id (optional): id of the course section for this session,
-            has_public_results (optional): whether the results are viewable by students.
-        :type poll_session: list
+        :returns: :class:`canvasapi.poll_session.PollSession`
+        """
+        response = self._requester.request(
+            "GET",
+            "polls/{}/poll_sessions/{}/close".format(self.poll_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return PollSession(self._requester, response.json()["poll_sessions"][0])
 
-        :rtype: :class:`canvasapi.poll_session.PollSession`
+    def create_submission(self, poll_submissions, **kwargs):
+        """
+        Create a new poll submission for this poll session.
+
+        :calls: `POST /api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions \
+        <https://canvas.instructure.com/doc/api/poll_submissions.html#method.polling/poll_submissions.create>`_
+
+        :param poll_submissions: List of arguments. poll_choice_id (required int): Chosen poll \
+        choice for this submission.
+        :type poll_submissions: list
+
+        :rtype: :class:`canvasapi.poll_submission.PollSubmission`
         """
         if (
-            isinstance(poll_session, list)
-            and isinstance(poll_session[0], dict)
-            and "course_id" in poll_session[0]
+            isinstance(poll_submissions, list)
+            and isinstance(poll_submissions[0], dict)
+            and "poll_choice_id" in poll_submissions[0]
         ):
-            kwargs["poll_session"] = poll_session
+            kwargs["poll_submissions"] = poll_submissions
         else:
-            raise RequiredFieldMissing("Dictionary with key 'course_id' is required.")
+            raise RequiredFieldMissing(
+                "Dictionary with key 'poll_choice_id is required."
+            )
 
         response = self._requester.request(
-            "PUT",
-            "polls/{}/poll_sessions/{}".format(self.poll_id, self.id),
+            "POST",
+            "polls/{}/poll_sessions/{}/poll_submissions".format(self.poll_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
-        return PollSession(self._requester, response.json()["poll_sessions"][0])
+        return PollSubmission(self._requester, response.json()["poll_submissions"][0])
 
     def delete(self, **kwargs):
         """
         Delete a single poll session, based on the session id.
 
         :calls: `DELETE /api/v1/polls/:poll_id/poll_sessions/:id \
         <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.destroy>`_
@@ -52,46 +69,14 @@
         response = self._requester.request(
             "DELETE",
             "polls/{}/poll_sessions/{}".format(self.poll_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return response.status_code == 204
 
-    def open(self, **kwargs):
-        """
-        Open a poll session to answers based on the poll id.
-
-        :calls: `GET /api/v1/polls/:poll_id/poll_sessions/:id/open \
-        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.open>`_
-
-        :returns: :class:`canvasapi.poll_session.PollSession`
-        """
-        response = self._requester.request(
-            "GET",
-            "polls/{}/poll_sessions/{}/open".format(self.poll_id, self.id),
-            _kwargs=combine_kwargs(**kwargs),
-        )
-        return PollSession(self._requester, response.json()["poll_sessions"][0])
-
-    def close(self, **kwargs):
-        """
-        Close a poll session to answers based on the poll id.
-
-        :calls: `GET /api/v1/polls/:poll_id/poll_sessions/:id/close \
-        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.close>`_
-
-        :returns: :class:`canvasapi.poll_session.PollSession`
-        """
-        response = self._requester.request(
-            "GET",
-            "polls/{}/poll_sessions/{}/close".format(self.poll_id, self.id),
-            _kwargs=combine_kwargs(**kwargs),
-        )
-        return PollSession(self._requester, response.json()["poll_sessions"][0])
-
     def get_submission(self, poll_submission, **kwargs):
         """
         Returns the poll submission with the given id.
 
         :calls: `GET /api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions/:id \
         <https://canvas.instructure.com/doc/api/poll_submissions.html#method.polling/poll_submissions.show>`_
 
@@ -109,37 +94,52 @@
             "polls/{}/poll_sessions/{}/poll_submissions/{}".format(
                 self.poll_id, self.id, poll_submission_id
             ),
             _kwargs=combine_kwargs(**kwargs),
         )
         return PollSubmission(self._requester, response.json()["poll_submissions"][0])
 
-    def create_submission(self, poll_submissions, **kwargs):
+    def open(self, **kwargs):
         """
-        Create a new poll submission for this poll session.
+        Open a poll session to answers based on the poll id.
 
-        :calls: `POST /api/v1/polls/:poll_id/poll_sessions/:poll_session_id/poll_submissions \
-        <https://canvas.instructure.com/doc/api/poll_submissions.html#method.polling/poll_submissions.create>`_
+        :calls: `GET /api/v1/polls/:poll_id/poll_sessions/:id/open \
+        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.open>`_
 
-        :param poll_submissions: List of arguments. poll_choice_id (required int): Chosen poll \
-        choice for this submission.
-        :type poll_submissions: list
+        :returns: :class:`canvasapi.poll_session.PollSession`
+        """
+        response = self._requester.request(
+            "GET",
+            "polls/{}/poll_sessions/{}/open".format(self.poll_id, self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return PollSession(self._requester, response.json()["poll_sessions"][0])
 
-        :rtype: :class:`canvasapi.poll_submission.PollSubmission`
+    def update(self, poll_session, **kwargs):
+        """
+        Update an existing poll session for a poll based on poll id.
+
+        :calls: `PUT /api/v1/polls/:poll_id/poll_sessions/:id \
+        <https://canvas.instructure.com/doc/api/poll_sessions.html#method.polling/poll_sessions.update>`_
+
+        :param poll_session: List of arguments. course_id (required): id of the course for the
+            session, course_section_id (optional): id of the course section for this session,
+            has_public_results (optional): whether the results are viewable by students.
+        :type poll_session: list
+
+        :rtype: :class:`canvasapi.poll_session.PollSession`
         """
         if (
-            isinstance(poll_submissions, list)
-            and isinstance(poll_submissions[0], dict)
-            and "poll_choice_id" in poll_submissions[0]
+            isinstance(poll_session, list)
+            and isinstance(poll_session[0], dict)
+            and "course_id" in poll_session[0]
         ):
-            kwargs["poll_submissions"] = poll_submissions
+            kwargs["poll_session"] = poll_session
         else:
-            raise RequiredFieldMissing(
-                "Dictionary with key 'poll_choice_id is required."
-            )
+            raise RequiredFieldMissing("Dictionary with key 'course_id' is required.")
 
         response = self._requester.request(
-            "POST",
-            "polls/{}/poll_sessions/{}/poll_submissions".format(self.poll_id, self.id),
+            "PUT",
+            "polls/{}/poll_sessions/{}".format(self.poll_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
-        return PollSubmission(self._requester, response.json()["poll_submissions"][0])
+        return PollSession(self._requester, response.json()["poll_sessions"][0])
```

### Comparing `canvasapi-3.0.0/canvasapi/progress.py` & `canvasapi-3.1.0/canvasapi/progress.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/quiz.py` & `canvasapi-3.1.0/canvasapi/quiz.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/quiz_group.py` & `canvasapi-3.1.0/canvasapi/quiz_group.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/requester.py` & `canvasapi-3.1.0/canvasapi/requester.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/rubric.py` & `canvasapi-3.1.0/canvasapi/rubric.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,18 +22,92 @@
             "courses/{}/rubrics/{}".format(self.course_id, self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
 
         return Rubric(self._requester, response.json())
 
 
+class RubricAssessment(CanvasObject):
+    def __str__(self):
+        return "{}, {}".format(self.id, self.artifact_type)
+
+    def delete(self, **kwargs):
+        """
+        Delete a single RubricAssessment.
+
+        :calls: `DELETE /api/v1/courses/:course_id/rubric_associations\
+        /:rubric_association_id/rubric_assessments/:id \
+        <https://canvas.instructure.com/doc/api/rubrics.html#method.rubric_assessments.destroy>`_
+
+        :rtype: :class:`canvasapi.rubric.RubricAssessment`
+        """
+        from canvasapi.rubric import RubricAssessment
+
+        response = self._requester.request(
+            "DELETE",
+            "courses/{}/rubric_associations/{}/rubric_assessments/{}".format(
+                self.course_id, self.rubric_association_id, self.id
+            ),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        return RubricAssessment(self._requester, response.json())
+
+    def update(self, **kwargs):
+        """
+        Update a single RubricAssessment.
+
+        :calls: `PUT /api/v1/courses/:course_id/rubric_associations\
+        /:rubric_association_id/rubric_assessments/:id \
+        <https://canvas.instructure.com/doc/api/rubrics.html#method.rubric_assessments.update>`_
+
+        :rtype: :class:`canvasapi.rubric.RubricAssessment`
+        """
+        from canvasapi.rubric import RubricAssessment
+
+        response = self._requester.request(
+            "PUT",
+            "courses/{}/rubric_associations/{}/rubric_assessments/{}".format(
+                self.course_id, self.rubric_association_id, self.id
+            ),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        return RubricAssessment(self._requester, response.json())
+
+
 class RubricAssociation(CanvasObject):
     def __str__(self):
         return "{}, {}".format(self.id, self.association_type)
 
+    def create_rubric_assessment(self, **kwargs):
+        """
+        Create a single RubricAssessment.
+
+        :calls: `POST /api/v1/courses/:course_id/rubric_associations\
+        /:rubric_association_id/rubric_assessments \
+        <https://canvas.instructure.com/doc/api/rubrics.html#method.rubric_assessments.create>`_
+
+        :rtype: :class:`canvasapi.rubric.RubricAssessment`
+        """
+        from canvasapi.rubric import RubricAssessment
+
+        response = self._requester.request(
+            "POST",
+            "courses/{}/rubric_associations/{}/rubric_assessments".format(
+                self.course_id, self.id
+            ),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+
+        assessment_json = response.json()
+        assessment_json.update({"course_id": self.id})
+
+        return RubricAssessment(self._requester, assessment_json)
+
     def delete(self, **kwargs):
         """
         Delete a RubricAssociation.
 
         :calls: `DELETE /api/v1/courses/:course_id/rubric_associations/:id \
         <https://canvas.instructure.com/doc/api/rubrics.html#method.rubric_associations.destroy>`_
```

### Comparing `canvasapi-3.0.0/canvasapi/section.py` & `canvasapi-3.1.0/canvasapi/section.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/sis_import.py` & `canvasapi-3.1.0/canvasapi/sis_import.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/submission.py` & `canvasapi-3.1.0/canvasapi/submission.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/tab.py` & `canvasapi-3.1.0/canvasapi/tab.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/upload.py` & `canvasapi-3.1.0/canvasapi/upload.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi/user.py` & `canvasapi-3.1.0/canvasapi/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from canvasapi.authentication_event import AuthenticationEvent
+from canvasapi.avatar import Avatar
 from canvasapi.calendar_event import CalendarEvent
 from canvasapi.canvas_object import CanvasObject
 from canvasapi.communication_channel import CommunicationChannel
+from canvasapi.content_export import ContentExport
+from canvasapi.content_migration import ContentMigration, Migrator
 from canvasapi.feature import Feature, FeatureFlag
 from canvasapi.folder import Folder
 from canvasapi.grade_change_log import GradeChangeEvent
 from canvasapi.license import License
+from canvasapi.page_view import PageView
 from canvasapi.paginated_list import PaginatedList
 from canvasapi.pairing_code import PairingCode
 from canvasapi.upload import FileOrPathLike, Uploader
 from canvasapi.usage_rights import UsageRights
 from canvasapi.util import combine_kwargs, obj_or_id, obj_or_str
 
 
@@ -77,16 +82,14 @@
         <https://canvas.instructure.com/doc/api/content_migrations.html#method.content_migrations.create>`_
 
         :param migration_type: The migrator type to use in this migration
         :type migration_type: str or :class:`canvasapi.content_migration.Migrator`
 
         :rtype: :class:`canvasapi.content_migration.ContentMigration`
         """
-        from canvasapi.content_migration import ContentMigration, Migrator
-
         if isinstance(migration_type, Migrator):
             kwargs["migration_type"] = migration_type.type
         elif isinstance(migration_type, str):
             kwargs["migration_type"] = migration_type
         else:
             raise TypeError("Parameter migration_type must be of type Migrator or str")
 
@@ -161,16 +164,14 @@
         <https://canvas.instructure.com/doc/api/content_exports.html#method.content_exports_api.create>`_
 
         :param export_type: The type of content to export.
         :type export_type: str
 
         :rtype: :class:`canvasapi.content_export.ContentExport`
         """
-        from canvasapi.content_export import ContentExport
-
         kwargs["export_type"] = export_type
 
         response = self._requester.request(
             "POST",
             "users/{}/content_exports".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -209,16 +210,14 @@
 
         :calls: `GET /api/v1/audit/authentication/users/:user_id \
         <https://canvas.instructure.com/doc/api/authentications_log.html#method.authentication_audit_api.for_user>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
                 :class:`canvasapi.authentication_event.AuthenticationEvent`
         """
-        from canvasapi.authentication_event import AuthenticationEvent
-
         return PaginatedList(
             AuthenticationEvent,
             self._requester,
             "GET",
             "audit/authentication/users/{}".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -229,16 +228,14 @@
 
         :calls: `GET /api/v1/users/:user_id/avatars \
         <https://canvas.instructure.com/doc/api/users.html#method.profile.profile_pics>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.avatar.Avatar`
         """
-        from canvasapi.avatar import Avatar
-
         return PaginatedList(
             Avatar,
             self._requester,
             "GET",
             "users/{}/avatars".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -345,16 +342,14 @@
         <https://canvas.instructure.com/doc/api/content_exports.html#method.content_exports_api.show>`_
 
         :param content_export: The object or ID of the content export to show.
         :type content_export: int or :class:`canvasapi.content_export.ContentExport`
 
         :rtype: :class:`canvasapi.content_export.ContentExport`
         """
-        from canvasapi.content_export import ContentExport
-
         export_id = obj_or_id(content_export, "content_export", (ContentExport,))
 
         response = self._requester.request(
             "GET",
             "users/{}/content_exports/{}".format(self.id, export_id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -367,16 +362,14 @@
 
         :calls: `GET /api/v1/users/:user_id/content_exports\
         <https://canvas.instructure.com/doc/api/content_exports.html#method.content_exports_api.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.content_export.ContentExport`
         """
-        from canvasapi.content_export import ContentExport
-
         return PaginatedList(
             ContentExport,
             self._requester,
             "GET",
             "users/{}/content_exports".format(self.id),
             kwargs=combine_kwargs(**kwargs),
         )
@@ -454,26 +447,24 @@
     def get_enabled_features(self, **kwargs):
         """
         Lists all of the enabled features for a user.
 
         :calls: `GET /api/v1/users/:user_id/features/enabled \
         <https://canvas.instructure.com/doc/api/feature_flags.html#method.feature_flags.enabled_features>`_
 
-        :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
-            :class:`canvasapi.feature.Feature`
+        :rtype: `list` of `str`
         """
-        return PaginatedList(
-            Feature,
-            self._requester,
+        response = self._requester.request(
             "GET",
             "users/{}/features/enabled".format(self.id),
-            {"user_id": self.id},
             _kwargs=combine_kwargs(**kwargs),
         )
 
+        return response.json()
+
     def get_enrollments(self, **kwargs):
         """
         List all of the enrollments for this user.
 
         :calls: `GET /api/v1/users/:user_id/enrollments \
         <https://canvas.instructure.com/doc/api/enrollments.html#method.enrollments_api.index>`_
 
@@ -817,16 +808,14 @@
 
         :calls: `GET /api/v1/users/:user_id/page_views \
         <https://canvas.instructure.com/doc/api/users.html#method.page_views.index>`_
 
         :rtype: :class:`canvasapi.paginated_list.PaginatedList` of
             :class:`canvasapi.course.PageView`
         """
-        from canvasapi.page_view import PageView
-
         return PaginatedList(
             PageView,
             self._requester,
             "GET",
             "users/{}/page_views".format(self.id),
             _kwargs=combine_kwargs(**kwargs),
         )
@@ -1015,14 +1004,34 @@
         response = self._requester.request(
             "GET",
             "users/{}/observees/{}".format(self.id, observee_id),
             _kwargs=combine_kwargs(**kwargs),
         )
         return User(self._requester, response.json())
 
+    def terminate_sessions(self, **kwargs):
+        """
+        Terminate all sessions for a user.
+
+        This includes all browser-based sessions and all access tokens,
+        including manually generated ones.
+
+        :calls: `DELETE /api/v1/users/:id/sessions \
+        <https://canvas.instructure.com/doc/api/users.html#method.users.terminate_sessions>`_
+
+        :rtype: str
+        """
+
+        response = self._requester.request(
+            "DELETE",
+            "users/{}/sessions".format(self.id),
+            _kwargs=combine_kwargs(**kwargs),
+        )
+        return response.json()
+
     def update_color(self, asset_string, hexcode, **kwargs):
         """
         Update a custom color for this user for a given context.
 
         This allows colors for the calendar and elsewhere to be customized on a user basis.
 
         The `asset_string` parameter should be in the format 'context_id', for example 'course_42'.
```

### Comparing `canvasapi-3.0.0/canvasapi/util.py` & `canvasapi-3.1.0/canvasapi/util.py`

 * *Files identical despite different names*

### Comparing `canvasapi-3.0.0/canvasapi.egg-info/PKG-INFO` & `canvasapi-3.1.0/canvasapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvasapi
-Version: 3.0.0
+Version: 3.1.0
 Summary: API wrapper for the Canvas LMS
 Home-page: https://github.com/ucfopen/canvasapi
 Author: University of Central Florida - Center for Distributed Learning
 Author-email: techrangers@ucf.edu
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `canvasapi-3.0.0/canvasapi.egg-info/SOURCES.txt` & `canvasapi-3.1.0/canvasapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHORS.md
 LICENSE
 README.md
 setup.cfg
 setup.py
 canvasapi/__init__.py
 canvasapi/account.py
+canvasapi/account_calendar.py
 canvasapi/appointment_group.py
 canvasapi/assignment.py
 canvasapi/authentication_event.py
 canvasapi/authentication_provider.py
 canvasapi/avatar.py
 canvasapi/blueprint.py
 canvasapi/bookmark.py
@@ -19,14 +20,15 @@
 canvasapi/comm_message.py
 canvasapi/communication_channel.py
 canvasapi/content_export.py
 canvasapi/content_migration.py
 canvasapi/conversation.py
 canvasapi/course.py
 canvasapi/course_epub_export.py
+canvasapi/course_event.py
 canvasapi/current_user.py
 canvasapi/custom_gradebook_columns.py
 canvasapi/discussion_topic.py
 canvasapi/enrollment.py
 canvasapi/enrollment_term.py
 canvasapi/eportfolio.py
 canvasapi/exceptions.py
@@ -37,14 +39,15 @@
 canvasapi/file.py
 canvasapi/folder.py
 canvasapi/grade_change_log.py
 canvasapi/gradebook_history.py
 canvasapi/grading_period.py
 canvasapi/grading_standard.py
 canvasapi/group.py
+canvasapi/jwt.py
 canvasapi/license.py
 canvasapi/login.py
 canvasapi/module.py
 canvasapi/notification_preference.py
 canvasapi/outcome.py
 canvasapi/outcome_import.py
 canvasapi/page.py
```

### Comparing `canvasapi-3.0.0/setup.py` & `canvasapi-3.1.0/setup.py`

 * *Files identical despite different names*

