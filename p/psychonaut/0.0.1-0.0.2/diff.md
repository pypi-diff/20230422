# Comparing `tmp/psychonaut-0.0.1.tar.gz` & `tmp/psychonaut-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychonaut-0.0.1.tar", max compression
+gzip compressed data, was "psychonaut-0.0.2.tar", max compression
```

## Comparing `psychonaut-0.0.1.tar` & `psychonaut-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,150 @@
--rw-r--r--   0        0        0       36 2023-04-16 16:38:56.445915 psychonaut-0.0.1/README.md
--rw-r--r--   0        0        0       16 2023-04-16 16:40:56.312431 psychonaut-0.0.1/psychonaut/__init__.py
--rw-r--r--   0        0        0      489 2023-04-16 16:46:30.883968 psychonaut-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 psychonaut-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-22 21:21:36.755778 psychonaut-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2325 2023-04-22 21:21:36.759778 psychonaut-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      469 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      721 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      794 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      528 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      793 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      774 2023-04-22 21:21:36.767778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/external.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/images.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/record.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0      875 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1007 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      706 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0     1053 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      784 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      455 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/like.py
+-rw-r--r--   0        0        0      614 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      463 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      525 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      890 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0      872 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      702 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0      894 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      743 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      843 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      460 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      876 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      460 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0      927 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      594 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      491 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0      845 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      891 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1212 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.771778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1140 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1292 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1413 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/defs.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0      774 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      788 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      815 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      631 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      659 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      704 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0     1112 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      762 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      820 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      830 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0     1087 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0      730 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      625 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      523 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/lexicons/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0     3017 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/api/session.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/cli/__init__.py
+-rw-r--r--   0        0        0     1682 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/cli/cli.py
+-rw-r--r--   0        0        0     1219 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/common_web/__init__.py
+-rw-r--r--   0        0        0     2364 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/common_web/ipld.py
+-rw-r--r--   0        0        0      421 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/common_web/ipld_test.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/__init__.py
+-rw-r--r--   0        0        0     1347 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/did.py
+-rw-r--r--   0        0        0     2106 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/did_test.py
+-rw-r--r--   0        0        0     3117 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/handle.py
+-rw-r--r--   0        0        0     6649 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/handle_test.py
+-rw-r--r--   0        0        0    15049 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/reserved.py
+-rw-r--r--   0        0        0      672 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/resolve.py
+-rw-r--r--   0        0        0      467 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/identifier/resolve_test.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/__init__.py
+-rw-r--r--   0        0        0     2003 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/blob_refs.py
+-rw-r--r--   0        0        0     7958 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/codegen.py
+-rw-r--r--   0        0        0        0 2023-04-22 21:21:36.775778 psychonaut-0.0.2/psychonaut/lexicon/codegen_test.py
+-rw-r--r--   0        0        0      212 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/ctx.py
+-rw-r--r--   0        0        0      767 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/defs.py
+-rw-r--r--   0        0        0     6822 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/fields.py
+-rw-r--r--   0        0        0     2921 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/fields_test.py
+-rw-r--r--   0        0        0     1900 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/formats.py
+-rw-r--r--   0        0        0     1919 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/formats_test.py
+-rw-r--r--   0        0        0      939 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/tools.py
+-rw-r--r--   0        0        0     8801 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/types.py
+-rw-r--r--   0        0        0     3785 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/types_test.py
+-rw-r--r--   0        0        0     1909 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/lexicon/util.py
+-rw-r--r--   0        0        0       23 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/nsid/__init__.py
+-rw-r--r--   0        0        0     3003 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/nsid/nsid.py
+-rw-r--r--   0        0        0     3287 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/nsid/nsid_test.py
+-rw-r--r--   0        0        0     3716 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/uri/__init__.py
+-rw-r--r--   0        0        0    17624 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/uri/uri_test.py
+-rw-r--r--   0        0        0     3912 2023-04-22 21:21:36.779778 psychonaut-0.0.2/psychonaut/uri/validation.py
+-rw-r--r--   0        0        0     1025 2023-04-22 21:21:36.779778 psychonaut-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 psychonaut-0.0.2/PKG-INFO
```

