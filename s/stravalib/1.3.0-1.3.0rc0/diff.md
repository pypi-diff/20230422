# Comparing `tmp/stravalib-1.3.0.tar.gz` & `tmp/stravalib-1.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stravalib-1.3.0.tar", last modified: Sat Apr 22 14:09:36 2023, max compression
+gzip compressed data, was "stravalib-1.3.0rc0.tar", last modified: Sat Feb 18 23:59:04 2023, max compression
```

## Comparing `stravalib-1.3.0.tar` & `stravalib-1.3.0rc0.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.711472 stravalib-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-22 14:09:19.000000 stravalib-1.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-22 14:09:19.000000 stravalib-1.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.687471 stravalib-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.687471 stravalib-1.3.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-22 14:09:19.000000 stravalib-1.3.0/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-22 14:09:19.000000 stravalib-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.687471 stravalib-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-22 14:09:19.000000 stravalib-1.3.0/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-22 14:09:19.000000 stravalib-1.3.0/.github/workflows/build-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-22 14:09:19.000000 stravalib-1.3.0/.github/workflows/check-strava-api.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-22 14:09:19.000000 stravalib-1.3.0/.github/workflows/push-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-22 14:09:19.000000 stravalib-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-22 14:09:19.000000 stravalib-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-22 14:09:19.000000 stravalib-1.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-22 14:09:19.000000 stravalib-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-22 14:09:19.000000 stravalib-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 14:09:19.000000 stravalib-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-22 14:09:19.000000 stravalib-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-22 14:09:19.000000 stravalib-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-22 14:09:36.711472 stravalib-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-22 14:09:19.000000 stravalib-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-04-22 14:09:19.000000 stravalib-1.3.0/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.687471 stravalib-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.687471 stravalib-1.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/_static/keepme
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/_static/stravalib.css
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.687471 stravalib-1.3.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/contributing/build-release-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/contributing/development-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/contributing/documentation-changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/contributing/how-to-contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/contributing/resources-for-new-contributors.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.691471 stravalib-1.3.0/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/get-started/activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/get-started/athletes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/get-started/authenticate-with-strava.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/get-started/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/get-started/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.691471 stravalib-1.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/images/stravalib_architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.691471 stravalib-1.3.0/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/docs/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.ActivityUploader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.ActivityUploader.update_from_response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.BatchedResultsIterator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.authorization_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.create_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.create_subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.deauthorize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.delete_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.delete_subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.exchange_code_for_token.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.explore_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity_comments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity_kudos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity_laps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity_photos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_activity_zones.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_athlete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_athlete_clubs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_athlete_koms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_athlete_starred_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_athlete_stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_club_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_club_members.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_effort_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_friend_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_gear.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_related_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_route_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_routes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_segment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_segment_effort.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_segment_efforts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_segment_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.get_starred_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.handle_subscription_callback.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.handle_subscription_update.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.join_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.leave_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.list_subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.refresh_access_token.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.update_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.update_athlete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.client.Client.upload_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.field_conversions.enum_value.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.field_conversions.enum_values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.field_conversions.optional_input.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.field_conversions.time_interval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.field_conversions.timezone.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.unithelper.Quantity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.unithelper.UnitConverter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.unithelper.c2f.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.unithelper.is_quantity_type.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.RateLimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/api/stravalib.util.limiter.total_seconds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/field-conversions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/strava_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/unithelper.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-22 14:09:19.000000 stravalib-1.3.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-22 14:09:19.000000 stravalib-1.3.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.683472 stravalib-1.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/examples/strava-oauth/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/examples/strava-oauth/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/static/ConnectWithStrava.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/examples/strava-oauth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/templates/login_error.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 14:09:19.000000 stravalib-1.3.0/examples/strava-oauth/templates/login_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-22 14:09:19.000000 stravalib-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-22 14:09:19.000000 stravalib-1.3.0/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-22 14:09:19.000000 stravalib-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:09:36.711472 stravalib-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/stravalib/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 14:09:36.000000 stravalib-1.3.0/stravalib/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    69645 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    36042 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/strava_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/stravalib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/auth_responder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.707472 stravalib-1.3.0/stravalib/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/functional/test_client_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/functional/test_client_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/functional/test_result_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.707472 stravalib-1.3.0/stravalib/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/integration/strava_api_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)    24592 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/integration/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.711472 stravalib-1.3.0/stravalib/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/activity-manual.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/activity.3.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/athlete.2.json
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/athlete.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/example_route_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/example_zone_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   451575 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/sample.tcx
--rw-r--r--   0 runner    (1001) docker     (123)   102646 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/resources/strava_swagger.json
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/test.ini-example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.711472 stravalib-1.3.0/stravalib/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/unit/test_client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/unit/test_field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/unit/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/tests/unit/test_unithelper.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/unit_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/unithelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.711472 stravalib-1.3.0/stravalib/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-22 14:09:19.000000 stravalib-1.3.0/stravalib/util/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:09:36.703472 stravalib-1.3.0/stravalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-22 14:09:36.000000 stravalib-1.3.0/stravalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-04-22 14:09:36.000000 stravalib-1.3.0/stravalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:09:36.000000 stravalib-1.3.0/stravalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 14:09:36.000000 stravalib-1.3.0/stravalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 14:09:36.000000 stravalib-1.3.0/stravalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.664811 stravalib-1.3.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.github/workflows/build-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.github/workflows/check-strava-api.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.github/workflows/push-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-02-18 23:59:04.664811 stravalib-1.3.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/_static/keepme
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/_static/stravalib.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/contributing/build-release-guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/contributing/development-guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/contributing/documentation-changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/contributing/how-to-contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/contributing/resources-for-new-contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/get-started/activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/get-started/athletes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/get-started/authenticate-with-strava.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/get-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/get-started/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.644811 stravalib-1.3.0rc0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/images/stravalib_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.648811 stravalib-1.3.0rc0/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.656811 stravalib-1.3.0rc0/docs/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.ActivityUploader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.ActivityUploader.update_from_response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.BatchedResultsIterator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.authorization_url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.create_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.create_subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.deauthorize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.delete_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.delete_subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.exchange_code_for_token.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.explore_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity_comments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity_kudos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity_laps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity_photos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_activity_zones.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_athlete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_athlete_clubs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_athlete_koms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_athlete_starred_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_athlete_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_club_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_club_members.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_effort_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_friend_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_gear.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_related_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_route_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_routes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_segment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_segment_effort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_segment_efforts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_segment_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.get_starred_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.handle_subscription_callback.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.handle_subscription_update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.join_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.leave_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.list_subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.refresh_access_token.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.update_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.update_athlete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.upload_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.field_conversions.enum_value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.field_conversions.enum_values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.field_conversions.optional_input.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.field_conversions.time_interval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.field_conversions.timezone.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.unithelper.Quantity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.unithelper.UnitConverter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.unithelper.c2f.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.unithelper.is_quantity_type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.RateLimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/api/stravalib.util.limiter.total_seconds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/field-conversions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/strava_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/unithelper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.640811 stravalib-1.3.0rc0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.656811 stravalib-1.3.0rc0/examples/strava-oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.656811 stravalib-1.3.0rc0/examples/strava-oauth/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/static/ConnectWithStrava.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.656811 stravalib-1.3.0rc0/examples/strava-oauth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/templates/login_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/examples/strava-oauth/templates/login_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 23:59:04.664811 stravalib-1.3.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.656811 stravalib-1.3.0rc0/stravalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-18 23:59:04.000000 stravalib-1.3.0rc0/stravalib/_version_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67052 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25841 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36014 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/strava_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.660811 stravalib-1.3.0rc0/stravalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/auth_responder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.660811 stravalib-1.3.0rc0/stravalib/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/functional/test_client_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/functional/test_client_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/functional/test_result_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.660811 stravalib-1.3.0rc0/stravalib/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/integration/strava_api_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23792 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/integration/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.660811 stravalib-1.3.0rc0/stravalib/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/activity-manual.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/activity.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/athlete.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/athlete.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/example_route_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/example_zone_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   451575 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/sample.tcx
+-rw-r--r--   0 runner    (1001) docker     (123)   102646 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/resources/strava_swagger.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/test.ini-example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.664811 stravalib-1.3.0rc0/stravalib/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/unit/test_client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/unit/test_field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/unit/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/tests/unit/test_unithelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/unit_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/unithelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.664811 stravalib-1.3.0rc0/stravalib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-02-18 23:58:49.000000 stravalib-1.3.0rc0/stravalib/util/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 23:59:04.660811 stravalib-1.3.0rc0/stravalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-02-18 23:59:04.000000 stravalib-1.3.0rc0/stravalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-02-18 23:59:04.000000 stravalib-1.3.0rc0/stravalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 23:59:04.000000 stravalib-1.3.0rc0/stravalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-18 23:59:04.000000 stravalib-1.3.0rc0/stravalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-18 23:59:04.000000 stravalib-1.3.0rc0/stravalib.egg-info/top_level.txt
```

### Comparing `stravalib-1.3.0/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md` & `stravalib-1.3.0rc0/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `stravalib-1.3.0rc0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/.github/workflows/build-docs.yml` & `stravalib-1.3.0rc0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/.github/workflows/build-test.yml` & `stravalib-1.3.0rc0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/.github/workflows/check-strava-api.yml` & `stravalib-1.3.0rc0/.github/workflows/check-strava-api.yml`

 * *Files 23% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 jobs:
   update-model:
     name: Update Model
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
-      - name: Fetch API
-        run: curl https://developers.strava.com/swagger/swagger.json > stravalib/tests/resources/strava_swagger.json
-      - name: Fetch API Schema
+      - name: Fetch Latest API
         uses: stravalib/strava_swagger2pydantic@v1
         with:
           model_file: 'stravalib/strava_model.py'
       - name: Create Pull Request
         uses: peter-evans/create-pull-request@v4
         with:
           add-paths: |
@@ -25,9 +23,7 @@
           commit-message: Strava API Change
           branch: api-change
           delete-branch: true
           title: '[CHANGE] Strava API Change'
           body: |
             There were changes in the Strava API:
             [Please edit this comment to indicate what has changed]
-
-            - [ ] The changelog is updated (only when necessary)
```

### Comparing `stravalib-1.3.0/.github/workflows/push-pypi.yml` & `stravalib-1.3.0rc0/.github/workflows/push-pypi.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/.pre-commit-config.yaml` & `stravalib-1.3.0rc0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 # Common tasks
 #
 # - Run on all files:   pre-commit run --all-files
 # - Register git hooks: pre-commit install --install-hooks
 
 ci:
     autofix_prs: false
-    skip: [flake8]
-    autofix_commit_msg: |
-      '[pre-commit.ci 🤖] Apply code format tools to PR'
-    autoupdate_commit_msg: "[pre-commit.ci] pre-commit autoupdate"
+    skip: [flake8, end-of-file-fixer]
+    #autofix_commit_msg: |
+        #'[pre-commit.ci 🤖] Apply code format tools to PR'
     # Update hook versions every quarter (so we don't get hit with weekly update pr's)
-    autoupdate_schedule: weekly
-    autoupdate_branch: ""
+    autoupdate_schedule: quarterly
 
-default_stages: [commit]
 repos:
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+        files: \.py$
+
   # Misc commit checks
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     # ref: https://github.com/pre-commit/pre-commit-hooks#hooks-available
     hooks:
       # Autoformat: Makes sure files end in a newline and only a newline.
       - id: end-of-file-fixer
@@ -38,22 +41,12 @@
   # Linting: Python code (see the file .flake8)
   - repo: https://github.com/PyCQA/flake8
     rev: "6.0.0"
     hooks:
       - id: flake8
 
   # Black for auto code formatting
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-      - id: black
-        entry: bash -c 'black "$@"; git add -u' --
-        language_version: python3.10
-        args: ["--line-length=79"]
-
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        entry: bash -c 'isort "$@"; git add -u' --
-        files: \.py$
-        args: ["--profile", "black", "--filter-files"]
+#  - repo: https://github.com/psf/black
+#    rev: 22.12.0
+#    hooks:
+#     - id: black
+#       language_version: python3.8
```

### Comparing `stravalib-1.3.0/CODE_OF_CONDUCT.md` & `stravalib-1.3.0rc0/CODE_OF_CONDUCT.md`

 * *Files 0% similar despite different names*

```diff
@@ -127,7 +127,8 @@
 [https://www.contributor-covenant.org/translations][translations].
 
 [homepage]: https://www.contributor-covenant.org
 [v2.1]: https://www.contributor-covenant.org/version/2/1/code_of_conduct.html
 [Mozilla CoC]: https://github.com/mozilla/diversity
 [FAQ]: https://www.contributor-covenant.org/faq
 [translations]: https://www.contributor-covenant.org/translations
+
```

### Comparing `stravalib-1.3.0/CONTRIBUTING.md` & `stravalib-1.3.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/LICENSE.txt` & `stravalib-1.3.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/Makefile` & `stravalib-1.3.0rc0/Makefile`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/PKG-INFO` & `stravalib-1.3.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stravalib
-Version: 1.3.0
+Version: 1.3.0rc0
 Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
 Author-email: Hans Lellelid <hans@xmpl.org>
 Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong
 License: Apache 2.0 License
 Project-URL: homepage, https://example.com
 Project-URL: documentation, https://stravalib.readthedocs.io
 Project-URL: repository, https://github.com/stravalib/stravalib
```

### Comparing `stravalib-1.3.0/README.md` & `stravalib-1.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/changelog.md` & `stravalib-1.3.0rc0/changelog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,272 +1,209 @@
 # Change Log
 
-## Unreleased
-
-## v1.3.0
-
-### Added
-
-- Add: Adds RPE to activity model (@jsamoocha, #355)
-- Add: support sport_type in client.update_activitiy() (@think-nice-things, #360)
-
-### Fixed
-
-- Fix: Move to numpy style docstrings & add black (@lwasser, #365)
-
-### Deprecated
-
-- The `activity_type` parameter in the client method `update_activity()` is deprecated and should be replaced by `sport_type`.
-
-### Contributors to this release
-
-@jsamoocha, @lwasser, @think-nice-things
-
 ## v1.3.0rc0
 
 ### Added
-
-- Adds Strava API changes, and datamodel-code-generator bug fix (@jsamoocha, #333)
-- Add: Replace full legacy model with extensions from the generated pydantic model (@jsamoocha, #324)
-- Add: Add support for lazy loading related entities (@jsamoocha, #322)
-- Add: Add support for nested model attributes(@jsamoocha, #316)
-- Add: replaces implementations for the classes Club, Gear, ActivityTotals, AthleteStats, and Athlete by the generated Pydantic model & backwards compatibility (@jsamoocha, #315)
-- Add: Workflow for updating strava model when the API changes (@jsamoocha, #302)
-- Add: `pydantic_autodoc` to sphinx build and reconfigure api structure - p1 (@lwasser, #326)
+* Adds Strava API changes, and datamodel-code-generator bug fix (@jsamoocha, #333)
+* Add: Replace full legacy model with extensions from the generated pydantic model (@jsamoocha, #324)
+* Add: Add support for  lazy loading related entities (@jsamoocha, #322)
+* Add: Add support for nested model attributes(@jsamoocha, #316)
+* Add: replaces implementations for the classes Club, Gear, ActivityTotals, AthleteStats, and Athlete by the generated Pydantic model & backwards compatibility (@jsamoocha, #315)
+* Add: Workflow for updating strava model when the API changes (@jsamoocha, #302)
+* Add: `pydantic_autodoc` to sphinx build and reconfigure api structure - p1 (@lwasser, #326)
 
 ### Fixed
-
-- Fix: Corrects attribute lookup for enum values (@jsamoocha,#329)
+* Fix: Corrects attribute lookup for enum values (@jsamoocha,#329)
 
 ### Deprecated
-
-- The `BaseEntity` methods `deserialize()`, `from_dict()`, and `to_dict()` are deprecated and will raise a `DeprecationWarning` when they're used. They should be replaced by the pydantic methods `parse_obj()` and `dict()` or `json()`.
+* The `BaseEntity` methods `deserialize()`, `from_dict()`, and `to_dict()` are deprecated and will raise a `DeprecationWarning` when they're used. They should be replaced by the pydantic methods `parse_obj()` and `dict()` or `json()`.
 
 ### Removed
-
-- The complete `attributes` module
-- All the abstract entity types (e.g. `IdentifiableEntity`, `LoadableEntity`) from the `model` module
-- Constants used for activity types such as `Activity.RIDE`
-- `HeartrateActivityZone`, `PowerActivityZone`, `PaceActivityZone` as subtypes of `BaseActivityZone` (the latter is retained)
-- Everything related to segment leaderboards as this is not supported by Strava anymore
+* The complete `attributes` module
+* All the abstract entity types (e.g. `IdentifiableEntity`, `LoadableEntity`) from the `model` module
+* Constants used for activity types such as `Activity.RIDE`
+* `HeartrateActivityZone`, `PowerActivityZone`, `PaceActivityZone` as subtypes of `BaseActivityZone` (the latter is retained)
+* Everything related to segment leaderboards as this is not supported by Strava anymore
 
 ### Contributors to this release
-
 @jsamoocha, @lwasser, @oliverkurth
 
 ## v1.2.0
 
 ### Added
-
-- Add: Upload photo to activity (@gitexel, #318)
-- Add: Support uploading `activity_file` object with type `bytes` (@gitexel, #308)
-- Add: Pre-commit hook + instructions and configure precommit.ci bot (@lwasser, #293)
+* Add: Upload photo to activity (@gitexel, #318)
+* Add: Support uploading `activity_file` object with type `bytes` (@gitexel, #308)
+* Add: Pre-commit hook + instructions and configure precommit.ci bot (@lwasser, #293)
 
 ### Fixed
-
-- Fix: Internal warnings should be ignored in tests (@jsamoocha, #319)
-- Fix: `setuptools_scm` bug when installing stravalib remotely via GitHub (@lwasser, #331)
-- Fix: fix LatLon unmarshal from string type (@oliverkurth, #334)
-- Fix: allows arithmetic and comparison between multiple quantities (@jsamoocha, #335)
+* Fix: Internal warnings should be ignored in tests (@jsamoocha, #319)
+* Fix: `setuptools_scm` bug when installing stravalib remotely via GitHub (@lwasser, #331)
+* Fix: fix LatLon unmarshal from string type (@oliverkurth, #334)
+* Fix: allows arithmetic and comparison between multiple quantities (@jsamoocha, #335)
 
 ### Contributors to this release
-
 @oliverkurth, @gitexel, @jsamoocha, @lwasser
 
 ## v1.1.0
 
 ### Added
-
-- Add: Development & build/release guide to documentation, edit button to documentation theme, pr template for release (@lwasser, #289)
-- Add: Integration tests for /routes/{id} and /segments/starred (GET) (@jsamoocha, #250 (partial))
-- Add: Add integration tests for all POST/PUT client methods (@jsamoocha, #250 (partial))
-- Add: code cov to test suite (@lwasser, #262)
-- Add: add code of conduct to the repo, update contributing guide + readme badges (@lwasser, #269, #274)
-- Add: pull request templates for regular pr and release (@lwasser, #294)
-- Add: Support for python 3.11
+* Add: Development & build/release guide to documentation, edit button to documentation theme, pr template for release (@lwasser, #289)
+* Add: Integration tests for /routes/{id} and /segments/starred (GET) (@jsamoocha, #250 (partial))
+* Add: Add integration tests for all POST/PUT client methods (@jsamoocha, #250 (partial))
+* Add: code cov to test suite (@lwasser, #262)
+* Add: add code of conduct to the repo, update contributing guide + readme badges (@lwasser, #269, #274)
+* Add: pull request templates for regular pr and release (@lwasser, #294)
+* Add: Support for python 3.11
 
 ### Fixed
-
-- Fix: Move docs to `furo` theme, add `myst` support for markdown, include CONTRIBUTING.md in documentation, enhance intro documentation page and add linkcheck to docs build (@lwasser, #276)
-- Fix: deprecated set-output command in actions build (@yihong0618, #272)
-- Fix: Add readthedocs config file to ensure build installs using pip (@lwasser, #270)
+* Fix: Move docs to `furo` theme, add `myst` support for markdown, include CONTRIBUTING.md in documentation, enhance intro documentation page and add linkcheck to docs build (@lwasser, #276)
+* Fix: deprecated set-output command in actions build (@yihong0618, #272)
+* Fix: Add readthedocs config file to ensure build installs using pip (@lwasser, #270)
 
 ### Changed
-
-- Change: Replace `units` dependency by `pint` (@jsamoocha, #281)
+* Change: Replace `units` dependency by `pint` (@jsamoocha, #281)
 
 ### Removed
-
-- Remove: Support for python 3.7
+* Remove: Support for python 3.7
 
 ### Contributors to this release
-
 @lwasser, @yihong0618, @jsamoocha
 
 ## v1.0.0
 
 ### Added
-
-- Add: Add an option to mute Strava activity on update (@ollyajoke, #227)
-- Add Update make to build and serve docs and also run current tests (@lwasser,#263)
-- Add: Move package to build / `setuptools_scm` for version / remove setup.py and add CI push to pypi (@lwasser, #259)
+* Add: Add an option to mute Strava activity on update (@ollyajoke, #227)
+* Add Update make to build and serve docs and also run current tests (@lwasser,#263)
+* Add: Move package to build / `setuptools_scm` for version / remove setup.py and add CI push to pypi (@lwasser, #259)
 
 ### Fixed
-
-- Fix: add new attributes for bikes according to updates to Strava API to fix warning message (@huaminghuangtw, #239)
-- Fix: Minor bug in PyPI push and also streamlined action build (@lwasser, #265)
-- Fix: `get_athlete` w new attrs for shoes given strava updates to API (@lwasser, #220)
-- Fix: Refactor deprecated unittest aliases for Python 3.11 compatibility (@tirkarthi, #223)
-- Patch: Update readme and fix broken links in docs (@lwasser, #229)
+* Fix: add new attributes for bikes according to updates to Strava API to fix warning message (@huaminghuangtw, #239)
+* Fix: Minor bug in PyPI push and also streamlined action build (@lwasser, #265)
+* Fix: `get_athlete` w new attrs for shoes given strava updates to API (@lwasser, #220)
+* Fix: Refactor deprecated unittest aliases for Python 3.11 compatibility (@tirkarthi, #223)
+* Patch: Update readme and fix broken links in docs (@lwasser, #229)
 
 ### Changed
-
-- Change: Improved unknown time zone handling (@jsamoocha, #242)
-- Change: Refactor test suite and implement Ci for tests (@jsamoocha, #246)
-- Change: Remove support for python 2.x (@yihong0618, #254)
-- Change: Overhaul of documentation, fix links and CI build (@lwasser, #222)
+* Change: Improved unknown time zone handling (@jsamoocha, #242)
+* Change: Refactor test suite and implement Ci for tests (@jsamoocha, #246)
+* Change: Remove support for python 2.x (@yihong0618, #254)
+* Change: Overhaul of documentation, fix links and CI build (@lwasser, #222)
 
 ### Contributors to this release
-
 @jsamoocha, @yihong0618, @tirkarthi, @huaminghuangtw, @ollyajoke, @lwasser
 
 ## 0.10.4
-
-- Fix to unicode regression (@hozn, #217)
+* Fix to unicode regression (@hozn, #217)
 
 ## 0.10.3
-
-- Fixes IndexErrors when deserializing empty lists as GPS locations (@hozn, #216)
-- Fix a few fields in Activity model (@hozn, #201, #214, #207)
-- deal with tzname without offset and timedelta in string format (@hozn, #195)
-- Update to docs and repr (@hozn, #200, #205, #206)
-- Now webhooks use the same domain as the rest of API. (@hozn, #204)
-- Setting rate_limit_requests=False in Client causes error (@hozn, #157)
+* Fixes IndexErrors when deserializing empty lists as GPS locations (@hozn, #216)
+* Fix a few fields in Activity model (@hozn, #201, #214, #207)
+* deal with tzname without offset and timedelta in string format (@hozn, #195)
+* Update to docs and repr (@hozn, #200, #205, #206)
+* Now webhooks use the same domain as the rest of API. (@hozn, #204)
+* Setting rate_limit_requests=False in Client causes error (@hozn, #157)
 
 ## 0.10.2
-
-- More fixes to new new authorization scopes (@hozn, #168)
-- Added an example oauth app and some small docs updates.
-- Changed missing-attribute warnings to be debug-level logs.
+* More fixes to new new authorization scopes (@hozn, #168)
+* Added an example oauth app and some small docs updates.
+* Changed missing-attribute warnings to be debug-level logs.
 
 ## 0.10.1
-
-- Fixes of authorization_url / new scopes for new oauth (@hozn, #163, #165)
+* Fixes of authorization_url / new scopes for new oauth (@hozn, #163, #165)
 
 ## 0.10.0
-
-- Implementation of Strava's new auth. (@hozn, #162, #163)
+* Implementation of Strava's new auth.  (@hozn, #162, #163)
 
 ## 0.9.4
-
-- Version bump for dup file upload to pypi. :-[
+* Version bump for dup file upload to pypi. :-[
 
 ## 0.9.3
-
-- Fix mutable parma defaults in rate-limiter util functions (@hozn, #155)
-- Add the missing subscription_permissions attr to Athlete (@hozn, #156)
+* Fix mutable parma defaults in rate-limiter util functions (@hozn, #155)
+* Add the missing subscription_permissions attr to Athlete (@hozn, #156)
 
 ## 0.9.2
 
-- Fix for pip 0.10.0 (@paulte, #149, #150)
+* Fix for pip 0.10.0 (@paulte, #149, #150)
 
 ## 0.9.1
-
-- Auto-configure the rate limits (not just usage) from response headers. (@hozn, #142)
+* Auto-configure the rate limits (not just usage) from response headers. (@hozn, #142)
 
 ## 0.9.0
-
-- More API changes to reflect the big privacy changes from Strava. (@hozn, #139, #140)
-- Fix to kom_type attribute (@hozn, #138)
+* More API changes to reflect the big privacy changes from Strava. (@hozn, #139, #140)
+* Fix to kom_type attribute (@hozn, #138)
 
 ## 0.8.0
-
-- Fixes to segment leaderboard models for Strava's API BREAKING CHANGE (@hozn, #137)
+* Fixes to segment leaderboard models for Strava's API BREAKING CHANGE (@hozn, #137)
   (See https://groups.google.com/forum/#!topic/strava-api/SsL2ytxtZng)
-- Return ObjectNotFound and AccessUnauthorized HTTPError subclasses for 404 and 401
+* Return ObjectNotFound and AccessUnauthorized HTTPError subclasses for 404 and 401
   errors respectively (@hozn, #134)
-- Return None when there are no activity streams (@hozn, #118)
+* Return None when there are no activity streams (@hozn, #118)
 
 ## 0.7.0
-
-- Updated Activity for new attributes (@hozn, #115, #122)
-- New segment attributes (@JohnnyLChang, #106)
-- Streams for a route (@drixselecta, #101)
-- Activity Uploader improvements (@bwalks, #119)
-- Added to_dict() method to model objects (@hozn, #127)
-- Added get_athlete_starred_segments (@wjazdbitu, #117)
-- Fixed glitches in activity.laps (@hozn, #112)
-- Fixed bug in club.members (@hozn, #110)
+* Updated Activity for new attributes (@hozn, #115, #122)
+* New segment attributes (@JohnnyLChang, #106)
+* Streams for a route (@drixselecta, #101)
+* Activity Uploader improvements (@bwalks, #119)
+* Added to_dict() method to model objects (@hozn, #127)
+* Added get_athlete_starred_segments (@wjazdbitu, #117)
+* Fixed glitches in activity.laps (@hozn, #112)
+* Fixed bug in club.members (@hozn, #110)
 
 ## 0.6.6
-
-- Fix for delete_activity (@jonderwaater, #99)
+* Fix for delete_activity (@jonderwaater, #99)
 
 ## 0.6.5
-
-- Updated ActivityPhoto model to support native photos and reverted get_activity_photos behavior for backwards
+* Updated ActivityPhoto model to support native photos and reverted get_activity_photos behavior for backwards
   compatibility (@hozn, #98)
-- Added missing Club attributes (MMI) (@hozn, #97)
+* Added missing Club attributes (MMI) (@hozn, #97)
 
 ## 0.6.4
-
-- Added support for undocumented inclusion of laps in activity details. (@hozn, #96)
-- Added missing parameter for get_activity_photos (@hozn, #94)
-- Added missing activyt pr_count attribute (@Wilm0r, #95)
-- add "starred" property on SegmentExplorerResult (@mdarmetko, #92)
+* Added support for undocumented inclusion of laps in activity details. (@hozn, #96)
+* Added missing parameter for get_activity_photos (@hozn, #94)
+* Added missing activyt pr_count attribute (@Wilm0r, #95)
+* add "starred" property on SegmentExplorerResult (@mdarmetko, #92)
 
 ## 0.6.3
-
-- Fixed update_activity to include description (@hozn, #91)
+* Fixed update_activity to include description (@hozn, #91)
 
 ## 0.6.2
-
-- More Python3 bugfixes
+* More Python3 bugfixes
 
 ## 0.6.1
-
-- Python3 bugfixes (@Tafkas, @martinogden)
-- Added delete_activity
-- added context_entries parameter to get_segment_leaderboard method (@jedman)
+* Python3 bugfixes (@Tafkas, @martinogden)
+* Added delete_activity
+* added context_entries parameter to get_segment_leaderboard method (@jedman)
 
 ## 0.6.0
-
-- Use (require) more modern pip/setuptools.
-- Full Python 3 support (using Six). (@hozn, #69)
-- Webhooks support (thanks to loisaidasam) (@hozn, #77)
-- explore_segments bugfix (@hozn, #71)
-- General updates to model/attribs (@hozn, #64, #73, etc.)
+* Use (require) more modern pip/setuptools.
+* Full Python 3 support (using Six). (@hozn, #69)
+* Webhooks support (thanks to loisaidasam) (@hozn, #77)
+* explore_segments bugfix (@hozn, #71)
+* General updates to model/attribs (@hozn, #64, #73, etc.)
 
 ## 0.5.0
-
-- Renamed `Activity.photos` property to `full_photos` due to new conflict with Strava API (@hozn, #45)
+* Renamed `Activity.photos` property to `full_photos` due to new conflict with Strava API (@hozn, #45)
 
 ## 0.4.0
-
-- Supporting new/removed attribs in Strava API (@hozn, #41, #42)
-- Added support for joining/leaving clubs (@hozn, #43)
-- Respect time zones in datetime objects being converted to epochs. (@hozn, #44)
+* Supporting new/removed attribs in Strava API (@hozn, #41, #42)
+* Added support for joining/leaving clubs (@hozn, #43)
+* Respect time zones in datetime objects being converted to epochs. (@hozn, #44)
 
 ## 0.3.0
-
-- Activity streams data (Ghis)
-- Friends/followers model attributes (Ghis)
-- Support for photos (Ghis)
-- Updates for new Strava exposed API attributes (@hozn)
+* Activity streams data (Ghis)
+* Friends/followers model attributes (Ghis)
+* Support for photos (Ghis)
+* Updates for new Strava exposed API attributes (@hozn)
 
 ## 0.2.2
-
-- Fixed the \_resolve_url to not assume running on **nix** system.
+* Fixed the _resolve_url to not assume running on **nix** system.
 
 ## 0.2.1
-
-- Changed Activity.gear to be a full entity attribute (Strava API changed)
+* Changed Activity.gear to be a full entity attribute (Strava API changed)
 
 ## 0.2.0
-
-- Added core functionality for Strava API v3.
-- Mostly redesigned codebase based on drastic changes in v3 API.
-- Dropped support for API v1, v2 and the "scrape" module.
+* Added core functionality for Strava API v3.
+* Mostly redesigned codebase based on drastic changes in v3 API.
+* Dropped support for API v1, v2 and the "scrape" module.
 
 ## 0.1.0
-
-- First proof-of-concept (very alpha) release.
+* First proof-of-concept (very alpha) release.
```

### Comparing `stravalib-1.3.0/docs/Makefile` & `stravalib-1.3.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/conf.py` & `stravalib-1.3.0rc0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
     version = stravalib.__version__
 
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    "sphinx.ext.napoleon",  # Numpy style doc support
-    "sphinx_remove_toctrees",  # Remove api generated stubs from doctree
+    "sphinx.ext.napoleon", # Numpy style doc support
+    "sphinx_remove_toctrees", # Remove api generated stubs from doctree
     "sphinxcontrib.autodoc_pydantic",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.ifconfig",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
     "sphinx.ext.autosummary",
@@ -107,27 +107,27 @@
 # Add edit button to furo theme
 
 # Link to our repo for easy PR/ editing
 html_theme_options = {
     "header_links_before_dropdown": 4,
     "use_edit_page_button": True,
     "show_toc_level": 1,
-    # "navbar_align": "left",  # [left, content, right] For testing that the navbar items align properly
+    #"navbar_align": "left",  # [left, content, right] For testing that the navbar items align properly
     "github_url": "https://github.com/stravalib/stravalib",
     "footer_items": ["copyright"],
 }
 
 html_context = {
     "github_user": "stravalib",
     "github_repo": "stravalib",
     "github_version": "master",
 }
 
 html_static_path = ["_static"]
-# html_css_files = ["stravalib.css"]
+#html_css_files = ["stravalib.css"]
 
 # Short title for the navigation bar.
 html_short_title = "Stravalib Python Package Documentation"
 
 # Instagram always throws 429 so ignore it
 linkcheck_ignore = [r"https://www.instagram.com/accounts/login/"]
 # The name of an image file (relative to this directory) to place at the top
```

### Comparing `stravalib-1.3.0/docs/contributing/build-release-guide.md` & `stravalib-1.3.0rc0/docs/contributing/build-release-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/contributing/development-guide.md` & `stravalib-1.3.0rc0/docs/contributing/development-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/contributing/resources-for-new-contributors.md` & `stravalib-1.3.0rc0/docs/contributing/resources-for-new-contributors.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 [La Terminal de Unix](https://swcarpentry.github.io/shell-novice-es/)
 
 ## Additional contribution resources
 For more information on contributing to open source projects, checkout:
 
 *  [GitHub's contribution guide](https://docs.github.com/en)
 is a great starting point if you are new to version control.
-* The [Zen of Scientific Software Maintenance](https://jrleeman.github.io/ScientificSoftwareMaintenance/)
+* The [Zen of Scientific Software Maintenance](https://jrleeman.github.io/ScientificSoftwareMaintenance/)
```

### Comparing `stravalib-1.3.0/docs/get-started/activities.rst` & `stravalib-1.3.0rc0/docs/get-started/activities.rst`

 * *Files 0% similar despite different names*

```diff
@@ -73,7 +73,8 @@
 =============== ================================================
 method           doc
 =============== ================================================
 create_activity  :meth:`stravalib.client.Client.create_activity`
 upload_activity :meth:`stravalib.client.Client.upload_activity`
 update_activity :meth:`stravalib.client.Client.update_activity`
 =============== ================================================
+
```

### Comparing `stravalib-1.3.0/docs/get-started/athletes.rst` & `stravalib-1.3.0rc0/docs/get-started/athletes.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/get-started/authenticate-with-strava.rst` & `stravalib-1.3.0rc0/docs/get-started/authenticate-with-strava.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/get-started/index.md` & `stravalib-1.3.0rc0/docs/get-started/index.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/get-started/overview.rst` & `stravalib-1.3.0rc0/docs/get-started/overview.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/images/stravalib_architecture.png` & `stravalib-1.3.0rc0/docs/images/stravalib_architecture.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/index.md` & `stravalib-1.3.0rc0/docs/index.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/reference/api/stravalib.client.ActivityUploader.rst` & `stravalib-1.3.0rc0/docs/reference/api/stravalib.client.ActivityUploader.rst`

 * *Files 0% similar despite different names*

```diff
@@ -28,7 +28,8 @@
 
    .. autosummary::
 
       ~ActivityUploader.is_complete
       ~ActivityUploader.is_error
       ~ActivityUploader.is_processing
       ~ActivityUploader.photo_metadata
+
```

### Comparing `stravalib-1.3.0/docs/reference/api/stravalib.client.Client.rst` & `stravalib-1.3.0rc0/docs/reference/api/stravalib.client.Client.rst`

 * *Files 0% similar despite different names*

```diff
@@ -65,7 +65,8 @@
 
 
    .. rubric:: Attributes
 
    .. autosummary::
 
       ~Client.access_token
+
```

### Comparing `stravalib-1.3.0/docs/reference/client.rst` & `stravalib-1.3.0rc0/docs/reference/client.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/reference/model.rst` & `stravalib-1.3.0rc0/docs/reference/model.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/reference/utilities.rst` & `stravalib-1.3.0rc0/docs/reference/utilities.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/docs/reference.rst` & `stravalib-1.3.0rc0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/examples/strava-oauth/README.md` & `stravalib-1.3.0rc0/examples/strava-oauth/README.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/examples/strava-oauth/server.py` & `stravalib-1.3.0rc0/examples/strava-oauth/server.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/examples/strava-oauth/static/ConnectWithStrava.png` & `stravalib-1.3.0rc0/examples/strava-oauth/static/ConnectWithStrava.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/examples/strava-oauth/templates/login.html` & `stravalib-1.3.0rc0/examples/strava-oauth/templates/login.html`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/pyproject.toml` & `stravalib-1.3.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/client.py` & `stravalib-1.3.0rc0/stravalib/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 from stravalib import exc, model, unithelper
 from stravalib.exc import (
     ActivityPhotoUploadNotSupported,
     warn_attribute_unofficial,
     warn_method_unofficial,
     warn_param_deprecation,
     warn_param_unofficial,
-    warn_param_unsupported,
 )
 from stravalib.protocol import ApiV3
 from stravalib.unithelper import is_quantity_type
 from stravalib.util import limiter
 
 
 class Client(object):
-    """Main client class for interacting with the exposed Strava v3 API methods.
+    """
+    Main client class for interacting with the exposed Strava v3 API methods.
 
-    This class can be instantiated without an access_token when performing
-    authentication; however, most methods will require a valid access token.
+    This class can be instantiated without an access_token when performing authentication;
+    however, most methods will require a valid access token.
 
     """
 
     def __init__(
         self,
         access_token=None,
         rate_limit_requests=True,
@@ -49,16 +49,16 @@
     ):
         """
         Initialize a new client object.
 
         Parameters
         ----------
         access_token : str
-            The token that provides access to a specific Strava account. If
-            empty, assume that this account is not yet authenticated.
+            The token that provides access to a specific Strava account. If empty, assume that this
+            account is not yet authenticated.
         rate_limit_requests : bool
             Whether to apply a rate limiter to the requests. (default True)
         rate_limiter : callable
             A :class:`stravalib.util.limiter.RateLimiter` object to use.
             If not specified (and rate_limit_requests is True), then
             :class:`stravalib.util.limiter.DefaultRateLimiter` will be used.
         requests_session : requests.Session() object
@@ -70,201 +70,177 @@
         )
 
         if rate_limit_requests:
             if not rate_limiter:
                 rate_limiter = limiter.DefaultRateLimiter()
         elif rate_limiter:
             raise ValueError(
-                "Cannot specify rate_limiter object when rate_limit_requests is"
-                " False"
+                "Cannot specify rate_limiter object when rate_limit_requests is False"
             )
 
         self.protocol = ApiV3(
             access_token=access_token,
             requests_session=requests_session,
             rate_limiter=rate_limiter,
         )
 
     @property
     def access_token(self):
-        """The currently configured authorization token."""
+        """
+        The currently configured authorization token.
+        """
         return self.protocol.access_token
 
     @access_token.setter
-    def access_token(self, token_value):
-        """Set the currently configured authorization token.
-
-        Parameters
-        ----------
-        token_value : int
-             User's access token for authentication.
-
-
-        Returns
-        -------
-
+    def access_token(self, v):
+        """
+        Set the currently configured authorization token.
         """
-        self.protocol.access_token = token_value
+        self.protocol.access_token = v
 
     def authorization_url(
         self,
         client_id,
         redirect_uri,
         approval_prompt="auto",
         scope=None,
         state=None,
     ):
-        """Get the URL needed to authorize your application to access a Strava
-        user's information.
+        """
+        Get the URL needed to authorize your application to access a Strava user's information.
 
         See https://developers.strava.com/docs/authentication/
 
         Parameters
         ----------
         client_id : int
             The numeric developer client id.
         redirect_uri : str
-            The URL that Strava will redirect to after successful (or failed)
-            authorization.
-        approval_prompt : str, default='auto'
-            Whether to prompt for approval even if approval already granted to
-            app.
-            Choices are 'auto' or 'force'.
-        scope : list[str], default = None
+            The URL that Strava will redirect to after successful (or failed) authorization.
+        approval_prompt : str
+            Whether to prompt for approval even if approval already granted to app.
+            Choices are 'auto' or 'force'.  (Default is 'auto')
+        scope : list[str]
             The access scope required.  Omit to imply "read" and "activity:read"
-            Valid values are 'read', 'read_all', 'profile:read_all',
-            'profile:write', 'activity:read', 'activity:read_all',
-            'activity:write'.
-        state : str, default=None
-            An arbitrary variable that will be returned to your application in
-            the redirect URI.
+            Valid values are 'read', 'read_all', 'profile:read_all', 'profile:write', 'activity:read',
+            'activity:read_all', 'activity:write'.
+        state : str
+            An arbitrary variable that will be returned to your application in the redirect URI.
 
         Returns
         -------
-        str:
-            A string containing the url required to authorize with the Strava
-            API.
-
+        string : The URL string to use for authorization link.
         """
         return self.protocol.authorization_url(
             client_id=client_id,
             redirect_uri=redirect_uri,
             approval_prompt=approval_prompt,
             scope=scope,
             state=state,
         )
 
     def exchange_code_for_token(self, client_id, client_secret, code):
-        """Exchange the temporary authorization code (returned with redirect
-        from strava authorization URL)  for a short-lived access token and a
-        refresh token (used to obtain the next access token later on).
+        """
+        Exchange the temporary authorization code (returned with redirect from strava authorization URL)
+        for a short-lived access token and a refresh token (used to obtain the next access token later on).
 
         Parameters
         ----------
         client_id : int
             The numeric developer client id.
         client_secret : str
             The developer client secret
         code : str
             The temporary authorization code
 
         Returns
         -------
-        dict
-            Dictionary containing the access_token, refresh_token and
-            expires_at (number of seconds since Epoch when the provided access
-            token will expire)
-
-
+        Dictionary containing the access_token, refresh_token
+        and expires_at (number of seconds since Epoch when the provided access token will expire)
         """
         return self.protocol.exchange_code_for_token(
             client_id=client_id, client_secret=client_secret, code=code
         )
 
     def refresh_access_token(self, client_id, client_secret, refresh_token):
-        """Exchanges the previous refresh token for a short-lived access token
-        and a new refresh token (used to obtain the next access token later on).
+        """
+        Exchanges the previous refresh token for a short-lived access token and a new
+        refresh token (used to obtain the next access token later on).
 
         Parameters
         ----------
         client_id : int
             The numeric developer client id.
         client_secret : str
             The developer client secret
         refresh_token : str
             The refresh token obtained from a previous authorization request
 
         Returns
         -------
-        dict:
-            Dictionary containing the access_token, refresh_token and expires_at
-            (number of seconds since Epoch when the provided access
-            token will expire)
-
+        Dictionary containing the access_token, refresh_token
+        and expires_at (number of seconds since Epoch when the provided access token will expire)
         """
         return self.protocol.refresh_access_token(
             client_id=client_id,
             client_secret=client_secret,
             refresh_token=refresh_token,
         )
 
     def deauthorize(self):
-        """Deauthorize the application. This causes the application to be
-        removed from the athlete's "My Apps" settings page.
+        """
+        Deauthorize the application. This causes the application to be removed
+        from the athlete's "My Apps" settings page.
 
         https://developers.strava.com/docs/authentication/#deauthorization
-
         """
         self.protocol.post("oauth/deauthorize")
 
     def _utc_datetime_to_epoch(self, activity_datetime):
-        """Convert the specified datetime value to a unix epoch timestamp
-        (seconds since epoch).
+        """
+        Convert the specified datetime value to a unix epoch timestamp (seconds since epoch).
 
         Parameters
         ----------
         activity_datetime : str
-            A string which may contain tzinfo (offset) or a datetime object
-            (naive datetime will be considered to be UTC).
+            A string which may contain tzinfo (offset) or a datetime object (naive datetime will
+            be considered to be UTC).
 
         Returns
         -------
-        datetime value in univ epoch time stamp format (seconds since epoch)
-
-
+        Epoch timestamp in int format.
         """
         if isinstance(activity_datetime, str):
             activity_datetime = arrow.get(activity_datetime).datetime
         assert isinstance(activity_datetime, datetime)
         if activity_datetime.tzinfo:
             activity_datetime = activity_datetime.astimezone(pytz.utc)
 
         return calendar.timegm(activity_datetime.timetuple())
 
     def get_activities(self, before=None, after=None, limit=None):
-        """Get activities for authenticated user sorted by newest first.
+        """
+        Get activities for authenticated user sorted by newest first.
 
         https://developers.strava.com/docs/reference/#api-Activities-getLoggedInAthleteActivities
 
-        Parameters
-        ----------
-        before : datetime.datetime or str or None, default=None
-            Result will start with activities whose start date is
-            before specified date. (UTC)
-        after : datetime.datetime or str or None, default=None
-            Result will start with activities whose start date is after
-            specified value. (UTC)
-        limit : int or None, default=None
-            How many maximum activities to return.
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Activity` objects.
+        :param before: Result will start with activities whose start date is
+                       before specified date. (UTC)
+        :type before: datetime.datetime or str or None
+
+        :param after: Result will start with activities whose start date is after
+                      specified value. (UTC)
+        :type after: datetime.datetime or str or None
+
+        :param limit: How many maximum activities to return.
+        :type limit: int or None
 
+        :return: An iterator of :class:`stravalib.model.Activity` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
 
         if before:
             before = self._utc_datetime_to_epoch(before)
 
         if after:
             after = self._utc_datetime_to_epoch(after)
@@ -278,357 +254,321 @@
             entity=model.Activity,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
     def get_athlete(self):
-        """Gets the specified athlete; if athlete_id is None then retrieves a
+        """
+        Gets the specified athlete; if athlete_id is None then retrieves a
         detail-level representation of currently authenticated athlete;
         otherwise summary-level representation returned of athlete.
 
         https://developers.strava.com/docs/reference/#api-Athletes
 
         https://developers.strava.com/docs/reference/#api-Athletes-getLoggedInAthlete
 
-        Parameters
-        ----------
-
-        Returns
-        -------
-        class:`stravalib.model.Athlete`
-            The athlete model object.
-
+        :return: The athlete model object.
+        :rtype: :class:`stravalib.model.Athlete`
         """
         raw = self.protocol.get("/athlete")
         return model.Athlete.parse_obj({**raw, **{"bound_client": self}})
 
     def update_athlete(
         self, city=None, state=None, country=None, sex=None, weight=None
     ):
-        """Updates the properties of the authorized athlete.
+        """
+        Updates the properties of the authorized athlete.
 
         https://developers.strava.com/docs/reference/#api-Athletes-updateLoggedInAthlete
 
         Parameters
-        ----------
-        city : str, default=None
+        -----------
+        city : str
             City the athlete lives in
+
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
             removed in the future.
-        state : str, default=None
+        state : str
             State the athlete lives in
+
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
             removed in the future.
-        country : str, default=None
+        country : str
             Country the athlete lives in
+
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
-            removed in the future.
-        sex : str, default=None
+             removed in the future.
+        sex : str
             Sex of the athlete
+
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
             removed in the future.
-        weight : float, default=None
+        weight : float
             Weight of the athlete in kg (float)
 
-
+        Returns
+        --------
+        :class:`stravalib.model.Athlete`
+            The updated athlete object
         """
         params = {"city": city, "state": state, "country": country, "sex": sex}
         params = {k: v for (k, v) in params.items() if v is not None}
         for p in params.keys():
             if p != "weight":
-                warn_param_unsupported(p)
+                warn_param_deprecation(p)
         if weight is not None:
             params["weight"] = float(weight)
 
         raw_athlete = self.protocol.put("/athlete", **params)
         return model.Athlete.parse_obj(
             {**raw_athlete, **{"bound_client": self}}
         )
 
+    # TODO: Can't find this in the api documentation either. Does it still work?
     def get_athlete_koms(self, athlete_id, limit=None):
-        """Gets Q/KOMs/CRs for specified athlete.
+        """
+        Gets Q/KOMs/CRs for specified athlete.
 
         KOMs are returned as `stravalib.model.SegmentEffort` objects.
 
-        Parameters
-        ----------
-        athlete_id : int
-            The ID of the athlete.
-        limit : int
-            Maximum number of KOM segment efforts to return (default unlimited).
+        :param athlete_id: The ID of the athlete.
+        :type athlete_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.SegmentEffort` objects.
+        :param limit: Maximum number of KOM segment efforts to return (default unlimited).
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.SegmentEffort` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get, "/athletes/{id}/koms", id=athlete_id
         )
 
         return BatchedResultsIterator(
             entity=model.SegmentEffort,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
     def get_athlete_stats(self, athlete_id=None):
-        """Returns Statistics for the athlete.
+        """
+        Returns Statistics for the athlete.
         athlete_id must be the id of the authenticated athlete or left blank.
         If it is left blank two requests will be made - first to get the
         authenticated athlete's id and second to get the Stats.
 
         https://developers.strava.com/docs/reference/#api-Athletes-getStats
 
         Note that this will return the stats for _public_ activities only,
         regardless of the scopes of the current access token.
 
-        Parameters
-        ----------
-        athlete_id : int, default=None
-            Strava ID value for the athlete.
-
-        Returns
-        -------
-        py:class:`stravalib.model.AthleteStats`
-            A model containing the Stats
-
+        :return: A model containing the Stats
+        :rtype: :py:class:`stravalib.model.AthleteStats`
         """
         if athlete_id is None:
             athlete_id = self.get_athlete().id
 
         raw = self.protocol.get("/athletes/{id}/stats", id=athlete_id)
         # TODO: Better error handling - this will return a 401 if this athlete
         #       is not the authenticated athlete.
 
         return model.AthleteStats.parse_obj(raw)
 
     def get_athlete_clubs(self):
-        """List the clubs for the currently authenticated athlete.
+        """
+        List the clubs for the currently authenticated athlete.
 
         https://developers.strava.com/docs/reference/#api-Clubs-getLoggedInAthleteClubs
 
-
-        Returns
-        -------
-        py:class:`list`
-            A list of :class:`stravalib.model.Club`
-
+        :return: A list of :class:`stravalib.model.Club`
+        :rtype: :py:class:`list`
         """
 
-        # TODO: This should return a BatchedResultsIterator or otherwise at
-        # most 30 clubs are returned!
+        # TODO: This should return a BatchedResultsIterator or otherwise at most 30 clubs are returned!
         club_structs = self.protocol.get("/athlete/clubs")
         return [
             model.Club.parse_obj({**raw, **{"bound_client": self}})
             for raw in club_structs
         ]
 
-    def join_club(self, club_id: int):
-        """Joins the club on behalf of authenticated athlete.
+    def join_club(self, club_id):
+        """
+        Joins the club on behalf of authenticated athlete.
 
         (Access token with write permissions required.)
 
-        Parameters
-        ----------
-        club_id : int
-            The numeric ID of the club to join.
-
-        Returns
-        -------
-        No actual return. This implements a post action that allows the athlete
-        to join a club via an API.
-
+        :param club_id: The numeric ID of the club to join.
         """
         self.protocol.post("clubs/{id}/join", id=club_id)
 
-    def leave_club(self, club_id: int):
-        """Leave club on behalf of authenticated user.
-
-        (Access token with write permissions required.)
-
-        Parameters
-        ----------
-        club_id : int
-
+    def leave_club(self, club_id):
+        """
+        Leave club on behalf of authenticated user.
 
-        Returns
-        -------
-        No actual return. This implements a post action that allows the athlete
-        to leave a club via an API.
+        (Acces token with write permissions required.)
 
+        :param club_id:
         """
         self.protocol.post("clubs/{id}/leave", id=club_id)
 
-    def get_club(self, club_id: int):
-        """Return a specific club object.
+    def get_club(self, club_id):
+        """
+        Return a specific club object.
 
         https://developers.strava.com/docs/reference/#api-Clubs-getClubById
 
-        Parameters
-        ----------
-        club_id : int
-            The ID of the club to fetch.
-
-        Returns
-        -------
-        class: `model.Club` object containing the club data.
+        :param club_id: The ID of the club to fetch.
+        :type club_id: int
 
+        :rtype: :class:`stravalib.model.Club`
         """
         raw = self.protocol.get("/clubs/{id}", id=club_id)
         return model.Club.parse_obj({**raw, **{"bound_client": self}})
 
-    def get_club_members(self, club_id: int, limit=None):
-        """Gets the member objects for specified club ID.
+    def get_club_members(self, club_id, limit=None):
+        """
+        Gets the member objects for specified club ID.
 
         https://developers.strava.com/docs/reference/#api-Clubs-getClubMembersById
 
-        Parameters
-        ----------
-        club_id : int
-            The numeric ID for the club.
-        limit : int
-            Maximum number of athletes to return. (default unlimited)
+        :param club_id: The numeric ID for the club.
+        :type club_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Athlete` objects.
+        :param limit: Maximum number of athletes to return. (default unlimited)
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.Athlete` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get, "/clubs/{id}/members", id=club_id
         )
 
         return BatchedResultsIterator(
             entity=model.Athlete,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
-    def get_club_activities(self, club_id: int, limit=None):
-        """Gets the activities associated with specified club.
+    def get_club_activities(self, club_id, limit=None):
+        """
+        Gets the activities associated with specified club.
 
         https://developers.strava.com/docs/reference/#api-Clubs-getClubActivitiesById
 
-        Parameters
-        ----------
-        club_id : int
-            The numeric ID for the club.
-        limit : int
-            Maximum number of activities to return. (default unlimited)
+        :param club_id: The numeric ID for the club.
+        :type club_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Activity` objects.
+        :param limit: Maximum number of activities to return. (default unlimited)
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.Activity` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get, "/clubs/{id}/activities", id=club_id
         )
 
         return BatchedResultsIterator(
             entity=model.Activity,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
-    def get_activity(
-        self, activity_id: int, include_all_efforts: bool = False
-    ):
-        """Gets specified activity.
+    def get_activity(self, activity_id, include_all_efforts=False):
+        """
+        Gets specified activity.
 
-        Will be detail-level if owned by authenticated user; otherwise
-        summary-level.
+        Will be detail-level if owned by authenticated user; otherwise summary-level.
 
         https://developers.strava.com/docs/reference/#api-Activities-getActivityById
 
-        Parameters
-        ----------
-        activity_id : int
-            The ID of activity to fetch.
-        include_all_efforts : bool, default=False
-            Whether to include segment efforts - only
-            available to the owner of the activity.
-
-        Returns
-        -------
-        class: `model.Activity`
-            An Activity object containing the requested activity data.
+        :param activity_id: The ID of activity to fetch.
+        :type activity_id: int
 
+        :param include_all_efforts: Whether to include segment efforts - only
+                                    available to the owner of the activty.
+        :type include_all_efforts: bool
+
+        :rtype: :class:`stravalib.model.Activity`
+
+        TODO: contrary to the Strava API documentation, this endpoint _always_
+        returns all segment efforts when the include_all_efforts parameter is provided,
+        regardless its value
         """
         raw = self.protocol.get(
             "/activities/{id}",
             id=activity_id,
             include_all_efforts=include_all_efforts,
         )
         return model.Activity.parse_obj({**raw, **{"bound_client": self}})
 
-    # TODO: REMOVE from API altogether given deprecation of end point
-    def get_friend_activities(self, limit: int = None):
-        """DEPRECATED This endpoint was removed by Strava in Jan 2018.
-
-        Parameters
-        ----------
-        limit : int
-            Maximum number of activities to return. (default unlimited)
+    def get_friend_activities(self, limit=None):
+        """
+        DEPRECATED This endpoint was removed by Strava in Jan 2018.
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Activity` objects.
+        :param limit: Maximum number of activities to return. (default unlimited)
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.Activity` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         raise NotImplementedError(
             "The /activities/following endpoint was removed by Strava.  "
             "See https://developers.strava.com/docs/january-2018-update/"
         )
 
+        # result_fetcher = functools.partial(self.protocol.get, '/activities/following')
+        #
+        # return BatchedResultsIterator(entity=model.Activity, bind_client=self,
+        #                               result_fetcher=result_fetcher, limit=limit)
+
     def create_activity(
         self,
         name,
         activity_type,
         start_date_local,
         elapsed_time,
         description=None,
         distance=None,
     ):
-        """Create a new manual activity.
+        """
+        Create a new manual activity.
 
         If you would like to create an activity from an uploaded GPS file, see the
         :meth:`stravalib.client.Client.upload_activity` method instead.
 
-        Parameters
-        ----------
-        name : str
-            The name of the activity.
-        activity_type : str
-            The activity type (case-insensitive).
-            Possible values: ride, run, swim, workout, hike, walk, nordicski,
-            alpineski, backcountryski, iceskate, inlineskate, kitesurf,
-            rollerski, windsurf, workout, snowboard, snowshoe
-        start_date_local : class:`datetime.datetime` or string in ISO8601 format
-            Local date/time of activity start. (TZ info will be ignored)
-        elapsed_time : class:`datetime.timedelta` or int (seconds)
-            The time in seconds or a :class:`datetime.timedelta` object.
-        description : str, default=None
-            The description for the activity.
-        distance : class:`pint.Quantity` or float (meters), default=None
-            The distance in meters (float) or a :class:`pint.Quantity` instance.
+        :param name: The name of the activity.
+        :type name: str
+
+        :param activity_type: The activity type (case-insensitive).
+                              Possible values: ride, run, swim, workout, hike, walk, nordicski,
+                              alpineski, backcountryski, iceskate, inlineskate, kitesurf, rollerski,
+                              windsurf, workout, snowboard, snowshoe
+        :type activity_type: str
+
+        :param start_date_local: Local date/time of activity start. (TZ info will be ignored)
+        :type start_date_local: :class:`datetime.datetime` or string in ISO8601 format.
+
+        :param elapsed_time: The time in seconds or a :class:`datetime.timedelta` object.
+        :type elapsed_time: :class:`datetime.timedelta` or int (seconds)
 
+        :param description: The description for the activity.
+        :type description: str
+
+        :param distance: The distance in meters (float) or a :class:`pint.Quantity` instance.
+        :type distance: :class:`pint.Quantity` or float (meters)
         """
         if isinstance(elapsed_time, timedelta):
             elapsed_time = elapsed_time.seconds
 
         if is_quantity_type(distance):
             distance = float(unithelper.meters(distance))
 
@@ -662,78 +602,65 @@
         )
 
     def update_activity(
         self,
         activity_id,
         name=None,
         activity_type=None,
-        sport_type=None,
         private=None,
         commute=None,
         trainer=None,
         gear_id=None,
         description=None,
         device_name=None,
         hide_from_home=None,
     ):
-        """Updates the properties of a specific activity.
+        """
+        Updates the properties of a specific activity.
 
         https://developers.strava.com/docs/reference/#api-Activities-updateActivityById
 
         Parameters
         ----------
+
         activity_id : int
             The ID of the activity to update.
-        name : str, default=None
+        name : str
             The name of the activity.
-        activity_type : str, default=None
+        activity_type : str
             The activity type (case-insensitive).
-            Deprecated. Prefer to use sport_type. In a request where both type
-            and sport_type are present, this field will be ignored.
-            See https://developers.strava.com/docs/reference/#api-models-UpdatableActivity.
-            Possible values: ride, run, swim, workout, hike, walk, nordicski,
-            alpineski, backcountryski, iceskate, inlineskate, kitesurf,
-            rollerski, windsurf, workout, snowboard, snowshoe
-        sport_type : str, default=None
-            Possible values (case-sensitive): AlpineSki, BackcountrySki,
-            Badminton, Canoeing, Crossfit, EBikeRide, Elliptical,
-            EMountainBikeRide, Golf, GravelRide, Handcycle,
-            HighIntensityIntervalTraining, Hike, IceSkate, InlineSkate,
-            Kayaking, Kitesurf, MountainBikeRide, NordicSki, Pickleball,
-            Pilates, Racquetball, Ride, RockClimbing, RollerSki, Rowing, Run,
-            Sail, Skateboard, Snowboard, Snowshoe, Soccer, Squash,
-            StairStepper, StandUpPaddling, Surfing, Swim, TableTennis, Tennis,
-            TrailRun, Velomobile, VirtualRide, VirtualRow, VirtualRun, Walk,
-            WeightTraining, Wheelchair, Windsurf, Workout, Yoga
-        private : bool, default=None
+            Possible values: ride, run, swim, workout, hike,
+            walk, nordicski, alpineski, backcountryski,
+            iceskate, inlineskate, kitesurf, rollerski,
+            windsurf, workout, snowboard, snowshoe
+        private : bool
             Whether the activity is private.
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
             removed in the future.
-        commute : bool, default=None
+        commute : bool
             Whether the activity is a commute.
-        trainer : bool, default=None
+        trainer : bool
             Whether this is a trainer activity.
-        gear_id : int, default=None
+        gear_id : int
             Alpha-numeric ID of gear (bike, shoes) used on this activity.
-        description : str, default=None
+        description : str
             Description for the activity.
-        device_name : str, default=None
+        device_name : str
             Device name for the activity
             .. deprecated:: 1.0
             This param is not supported by the Strava API and may be
             removed in the future.
-        hide_from_home : bool, default=None
+        hide_from_home : bool
             Whether the activity is muted (hidden from Home and Club feeds).
 
         Returns
         -------
-            Updates the activity in the selected Strava account
-
-
+        stravalib.model.Activity
+            The updated activity
         """
 
         # Convert the kwargs into a params dict
         params = {}
 
         if name is not None:
             params["name"] = name
@@ -742,32 +669,17 @@
             if not activity_type.lower() in [
                 t.lower() for t in model.Activity.TYPES
             ]:
                 raise ValueError(
                     f"Invalid activity type: {activity_type}. Possible values: {model.Activity.TYPES!r}"
                 )
             params["type"] = activity_type.lower()
-            warn_param_deprecation(
-                "activity_type",
-                "sport_type",
-                "https://developers.strava.com/docs/reference/#api-models-UpdatableActivity",
-            )
-
-        if sport_type is not None:
-            if not sport_type in model.Activity.SPORT_TYPES:
-                raise ValueError(
-                    f"Invalid activity type: {sport_type}. Possible values: {model.Activity.SPORT_TYPES!r}"
-                )
-            params["sport_type"] = sport_type
-            params.pop(
-                "type", None
-            )  # Just to be sure we don't confuse the Strava API
 
         if private is not None:
-            warn_param_unsupported("private")
+            warn_param_deprecation("private")
             params["private"] = int(private)
 
         if commute is not None:
             params["commute"] = int(commute)
 
         if trainer is not None:
             params["trainer"] = int(trainer)
@@ -775,15 +687,15 @@
         if gear_id is not None:
             params["gear_id"] = gear_id
 
         if description is not None:
             params["description"] = description
 
         if device_name is not None:
-            warn_param_unsupported("device_name")
+            warn_param_deprecation("device_name")
             params["device_name"] = device_name
 
         if hide_from_home is not None:
             params["hide_from_home"] = int(hide_from_home)
 
         raw_activity = self.protocol.put(
             "/activities/{activity_id}", activity_id=activity_id, **params
@@ -801,56 +713,56 @@
         description=None,
         activity_type=None,
         private=None,
         external_id=None,
         trainer=None,
         commute=None,
     ):
-        """Uploads a GPS file (tcx, gpx) to create a new activity for current
-        athlete.
+        """
+        Uploads a GPS file (tcx, gpx) to create a new activity for current athlete.
 
         https://developers.strava.com/docs/reference/#api-Uploads-createUpload
 
-        Parameters
-        ----------
-        activity_file : TextIOWrapper, str or bytes
-            The file object to upload or file contents.
-        data_type : str
-            File format for upload. Possible values: fit, fit.gz, tcx, tcx.gz,
-            gpx, gpx.gz
-        name : str, optional, default=None
-            If not provided, will be populated using start date and location,
-            if available
-        description : str, optional, default=None
-            The description for the activity
-        activity_type : str, optional
-            case-insensitive type of activity.
-            possible values: ride, run, swim, workout, hike, walk,
-            nordicski, alpineski, backcountryski, iceskate, inlineskate,
-            kitesurf, rollerski, windsurf, workout, snowboard, snowshoe
-            Type detected from file overrides, uses athlete's default type if
-            not specified
-            WARNING - This param is supported (as of 2022-11-15), but not
-            documented and may be removed in the future.
-        private : bool, optional, default=None
-            Set to True to mark the resulting activity as private,
-            'view_private' permissions will be necessary to view the activity.
+        :param activity_file: The file object to upload or file contents.
+        :type activity_file: TextIOWrapper, str or bytes
 
-            .. deprecated:: 1.0
-            This param is not supported by the Strava API and may be
-            removed in the future.
-        external_id : str, optional, default=None
-            An arbitrary unique identifier may be specified which
-            will be included in status responses.
-        trainer : bool, optional, default=None
-            Whether the resulting activity should be marked as having
-            been performed on a trainer.
-        commute : bool, optional, default=None
-            Whether the resulting activity should be tagged as a commute.
+        :param data_type: File format for upload. Possible values: fit, fit.gz, tcx, tcx.gz, gpx, gpx.gz
+        :type data_type: str
+
+        :param name: (optional) if not provided, will be populated using start date and location, if available
+        :type name: str
+
+        :param description: (optional) The description for the activity
+        :type name: str
+
+        :param activity_type: (optional) case-insensitive type of activity.
+                              possible values: ride, run, swim, workout, hike, walk,
+                              nordicski, alpineski, backcountryski, iceskate, inlineskate,
+                              kitesurf, rollerski, windsurf, workout, snowboard, snowshoe
+                              Type detected from file overrides, uses athlete's default type if not specified
+                              WARNING - This param is supported (as of 2022-11-15), but not
+                              documented and may be removed in the future.
+        :type activity_type: str
+
+        :param private: (optional) set to True to mark the resulting activity as private,
+                        'view_private' permissions will be necessary to view the activity.
+
+                        .. deprecated:: 1.0
+                        This param is not supported by the Strava API and may be
+                        removed in the future.
+        :type private: bool
 
+        :param external_id: (optional) An arbitrary unique identifier may be specified which will be included in status responses.
+        :type external_id: str
+
+        :param trainer: (optional) Whether the resulting activity should be marked as having been performed on a trainer.
+        :type trainer: bool
+
+        :param commute: (optional) Whether the resulting activity should be tagged as a commute.
+        :type commute: bool
         """
         if not hasattr(activity_file, "read"):
             if isinstance(activity_file, str):
                 activity_file = BytesIO(activity_file.encode("utf-8"))
             elif isinstance(activity_file, bytes):
                 activity_file = BytesIO(activity_file)
             else:
@@ -877,15 +789,15 @@
             ]:
                 raise ValueError(
                     f"Invalid activity type: {activity_type}. Possible values: {model.Activity.TYPES!r}"
                 )
             warn_param_unofficial("activity_type")
             params["activity_type"] = activity_type.lower()
         if private is not None:
-            warn_param_unsupported("private")
+            warn_param_deprecation("private")
             params["private"] = int(private)
         if external_id is not None:
             params["external_id"] = external_id
         if trainer is not None:
             params["trainer"] = int(trainer)
         if commute is not None:
             params["commute"] = int(commute)
@@ -895,70 +807,63 @@
             files={"file": activity_file},
             check_for_errors=False,
             **params,
         )
 
         return ActivityUploader(self, response=initial_response)
 
+    # TODO: I don't think this is the correct link but can't find it in the docs
     def delete_activity(self, activity_id):
-        """Deletes the specified activity.
+        """
+        Deletes the specified activity.
 
         https://developers.strava.com/docs/reference/#api-Activities
 
-        Parameters
-        ----------
-        activity_id : int
-            The activity to delete.
-
+        :param activity_id: The activity to delete.
+        :type activity_id: int
         """
         self.protocol.delete("/activities/{id}", id=activity_id)
 
     def get_activity_zones(self, activity_id):
-        """Gets zones for activity.
+        """
+        Gets zones for activity.
 
         Requires premium account.
 
         https://developers.strava.com/docs/reference/#api-Activities-getZonesByActivityId
 
-        Parameters
-        ----------
-        activity_id : int
-            The activity for which to get zones.
-
-        Returns
-        -------
-        py:class:`list`
-            A list of :class:`stravalib.model.BaseActivityZone` objects.
+        :param activity_id: The activity for which to get zones.
+        :type activity_id: int
 
+        :return: A list of :class:`stravalib.model.BaseActivityZone` objects.
+        :rtype: :py:class:`list`
         """
         zones = self.protocol.get("/activities/{id}/zones", id=activity_id)
         return [
             model.BaseActivityZone.parse_obj({**z, **{"bound_client": self}})
             for z in zones
         ]
 
     def get_activity_comments(self, activity_id, markdown=False, limit=None):
-        """Gets the comments for an activity.
+        """
+        Gets the comments for an activity.
 
         https://developers.strava.com/docs/reference/#api-Activities-getCommentsByActivityId
 
-        Parameters
-        ----------
-        activity_id : int
-            The activity for which to fetch comments.
-        markdown : bool
-            Whether to include markdown in comments (default is false/filterout)
-        limit : int
-            Max rows to return (default unlimited).
+        :param activity_id: The activity for which to fetch comments.
+        :type activity_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.ActivityComment` objects.
+        :param markdown: Whether to include markdown in comments (default is false/filterout).
+        :type markdown: bool
+
+        :param limit: Max rows to return (default unlimited).
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.ActivityComment` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get,
             "/activities/{id}/comments",
             id=activity_id,
             markdown=int(markdown),
         )
@@ -967,66 +872,60 @@
             entity=model.ActivityComment,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
     def get_activity_kudos(self, activity_id, limit=None):
-        """Gets the kudos for an activity.
+        """
+        Gets the kudos for an activity.
 
         https://developers.strava.com/docs/reference/#api-Activities-getKudoersByActivityId
 
-        Parameters
-        ----------
-        activity_id : int
-            The activity for which to fetch kudos.
-        limit : int
-            Max rows to return (default unlimited).
+        :param activity_id: The activity for which to fetch kudos.
+        :type activity_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.ActivityKudos` objects.
+        :param limit: Max rows to return (default unlimited).
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.ActivityKudos` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get, "/activities/{id}/kudos", id=activity_id
         )
 
         return BatchedResultsIterator(
             entity=model.ActivityKudos,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
+    # TODO not sure this is the correct api doc link - couldn't find "photos"
     def get_activity_photos(
         self, activity_id, size=None, only_instagram=False
     ):
-        """Gets the photos from an activity.
+        """
+        Gets the photos from an activity.
 
         https://developers.strava.com/docs/reference/#api-Activities
 
-        Parameters
-        ----------
-        activity_id : int
-            The activity for which to fetch photos.
-        size : int, default=None
-            the requested size of the activity's photos. URLs for the photos
-            will be returned that best match the requested size. If not
-            included, the smallest size is returned
-        only_instagram : bool, default=False
-            Parameter to preserve legacy behavior of only returning Instagram
-            photos.
+        :param activity_id: The activity for which to fetch photos.
+        :type activity_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.ActivityPhoto` objects.
+        :param size: the requested size of the activity's photos. URLs for the photos will be returned that best match
+                    the requested size. If not included, the smallest size is returned
+        :type size: int
 
+        :param only_instagram: Parameter to preserve legacy behavior of only returning Instagram photos.
+        :type only_instagram: bool
+
+        :return: An iterator of :class:`stravalib.model.ActivityPhoto` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         params = {}
 
         if not only_instagram:
             params["photo_sources"] = "true"
 
         if size is not None:
@@ -1042,140 +941,122 @@
         return BatchedResultsIterator(
             entity=model.ActivityPhoto,
             bind_client=self,
             result_fetcher=result_fetcher,
         )
 
     def get_activity_laps(self, activity_id):
-        """Gets the laps from an activity.
+        """
+        Gets the laps from an activity.
 
         https://developers.strava.com/docs/reference/#api-Activities-getLapsByActivityId
 
-        Parameters
-        ----------
-        activity_id : int
-            The activity for which to fetch laps.
-
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.ActivityLaps` objects.
+        :param activity_id: The activity for which to fetch laps.
+        :type activity_id: int
 
+        :return: An iterator of :class:`stravalib.model.ActivityLaps` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get, "/activities/{id}/laps", id=activity_id
         )
 
         return BatchedResultsIterator(
             entity=model.ActivityLap,
             bind_client=self,
             result_fetcher=result_fetcher,
         )
 
-    # TODO remove this method given deprecation of end point
     def get_related_activities(self, activity_id, limit=None):
-        """Deprecated. This endpoint was removed by strava in Jan 2018.
-
-        Parameters
-        ----------
-        activity_id : int
-            The activity for which to fetch related activities.
-        limit : int, default=None
-             Rate limit value for getting activities
+        """
+        Deprecated. This endpoint was removed by strava in Jan 2018.
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Activity` objects.
+        :param activity_id: The activity for which to fetch related activities.
+        :type activity_id: int
 
+        :return: An iterator of :class:`stravalib.model.Activity` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         raise NotImplementedError(
             "The /activities/{id}/related endpoint was removed by Strava.  "
             "See https://developers.strava.com/docs/january-2018-update/"
         )
 
+        # result_fetcher = functools.partial(self.protocol.get,
+        #                                    '/activities/{id}/related',
+        #                                    id=activity_id)
+        #
+        # return BatchedResultsIterator(entity=model.Activity,
+        #                               bind_client=self,
+        #                               result_fetcher=result_fetcher,
+        #                               limit=limit)
+
     def get_gear(self, gear_id):
-        """Get details for an item of gear.
+        """
+        Get details for an item of gear.
 
         https://developers.strava.com/docs/reference/#api-Gears
 
-        Parameters
-        ----------
-        gear_id : str
-            The gear id.
-
-        Returns
-        -------
-        class:`stravalib.model.Gear`
-            The Bike or Shoe subclass object.
+        :param gear_id: The gear id.
+        :type gear_id: str
 
+        :return: The Bike or Shoe subclass object.
+        :rtype: :class:`stravalib.model.Gear`
         """
         return model.Gear.parse_obj(
             self.protocol.get("/gear/{id}", id=gear_id)
         )
 
     def get_segment_effort(self, effort_id):
-        """Return a specific segment effort by ID.
+        """
+        Return a specific segment effort by ID.
 
         https://developers.strava.com/docs/reference/#api-SegmentEfforts
 
-        Parameters
-        ----------
-        effort_id : int
-            The id of associated effort to fetch.
-
-        Returns
-        -------
-        class:`stravalib.model.SegmentEffort`
-            The specified effort on a segment.
+        :param effort_id: The id of associated effort to fetch.
+        :type effort_id: int
 
+        :return: The specified effort on a segment.
+        :rtype: :class:`stravalib.model.SegmentEffort`
         """
         return model.SegmentEffort.parse_obj(
             self.protocol.get("/segment_efforts/{id}", id=effort_id)
         )
 
     def get_segment(self, segment_id):
-        """Gets a specific segment by ID.
+        """
+        Gets a specific segment by ID.
 
         https://developers.strava.com/docs/reference/#api-SegmentEfforts-getSegmentEffortById
 
-        Parameters
-        ----------
-        segment_id : int
-            The segment to fetch.
-
-        Returns
-        -------
-        class:`stravalib.model.Segment`
-            A segment object.
+        :param segment_id: The segment to fetch.
+        :type segment_id: int
 
+        :return: A segment object.
+        :rtype: :class:`stravalib.model.Segment`
         """
         return model.Segment.parse_obj(
             {
                 **self.protocol.get("/segments/{id}", id=segment_id),
                 **{"bound_client": self},
             }
         )
 
     def get_starred_segments(self, limit=None):
-        """Returns a summary representation of the segments starred by the
+        """
+        Returns a summary representation of the segments starred by the
          authenticated user. Pagination is supported.
 
         https://developers.strava.com/docs/reference/#api-Segments-getLoggedInAthleteStarredSegments
 
-        Parameters
-        ----------
-        limit : int, optional, default=None
-            Limit number of starred segments returned.
-
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Segment` starred by authenticated user.
+        :param limit: (optional), limit number of starred segments returned.
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.Segment` starred by authenticated user.
+        :rtype: :class:`BatchedResultsIterator`
         """
 
         params = {}
         if limit is not None:
             params["limit"] = limit
 
         result_fetcher = functools.partial(
@@ -1185,33 +1066,31 @@
         return BatchedResultsIterator(
             entity=model.Segment,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
+    # TODO: i'm not sure what the diff is between this method and the one above
+    # So i used the SAME API doc link for both. may need to revisit
     def get_athlete_starred_segments(self, athlete_id, limit=None):
-        """Returns a summary representation of the segments starred by the
+        """
+        Returns a summary representation of the segments starred by the
          specified athlete. Pagination is supported.
 
         https://developers.strava.com/docs/reference/#api-Segments-getLoggedInAthleteStarredSegments
 
-        Parameters
-        ----------
-        athlete_id : int
-            The ID of the athlete.
-        limit : int, optional, default=None
-            Limit number of starred segments returned.
+        :param athlete_id: The ID of the athlete.
+        :type athlete_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Segment` starred by
-            authenticated user.
+        :param limit: (optional), limit number of starred segments returned.
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.Segment` starred by authenticated user.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get, "/athletes/{id}/segments/starred", id=athlete_id
         )
 
         return BatchedResultsIterator(
             entity=model.Segment,
@@ -1224,55 +1103,53 @@
         self,
         segment_id,
         athlete_id=None,
         start_date_local=None,
         end_date_local=None,
         limit=None,
     ):
-        """Gets all efforts on a particular segment sorted by start_date_local
+        """
+        Gets all efforts on a particular segment sorted by start_date_local
 
         Returns an array of segment effort summary representations sorted by
         start_date_local ascending or by elapsed_time if an athlete_id is
         provided.
 
         If no filtering parameters is provided all efforts for the segment
         will be returned.
 
-        Date range filtering is accomplished using an inclusive start and end
-        time, thus start_date_local and end_date_local must be sent together.
-        For open ended ranges pick dates significantly in the past or future.
-        The filtering is done over local time for the segment, so there is no
-        need for timezone conversion. For example, all efforts on Jan. 1st, 2014
+        Date range filtering is accomplished using an inclusive start and end time,
+        thus start_date_local and end_date_local must be sent together. For open
+        ended ranges pick dates significantly in the past or future. The
+        filtering is done over local time for the segment, so there is no need
+        for timezone conversion. For example, all efforts on Jan. 1st, 2014
         for a segment in San Francisco, CA can be fetched using
         2014-01-01T00:00:00Z and 2014-01-01T23:59:59Z.
 
         https://developers.strava.com/docs/reference/#api-SegmentEfforts-getEffortsBySegmentId
 
-        Parameters
-        ----------
-        segment_id : int
-            ID for the segment of interest
-        athlete_id: int, optional
-            ID of athlete.
-        start_date_local : datetime.datetime or str, optional, default=None
-            Efforts before this date will be excluded.
-            Either as ISO8601 or datetime object
-        end_date_local : datetime.datetime or str, optional, default=None
-            Efforts after this date will be excluded.
-            Either as ISO8601 or datetime object
-        limit : int, default=None, optional
-            limit number of efforts.
-        athlete_id : int, default=None
-            Strava ID for the athlete
+        :param segment_id: ID of the segment.
+        :type segment_id: param
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.SegmentEffort` efforts on
-            a segment.
+        :int athlete_id: (optional) ID of athlete.
+        :type athlete_id: int
+
+        :param start_date_local: (optional) efforts before this date will be excluded.
+                                            Either as ISO8601 or datetime object
+        :type start_date_local: datetime.datetime or str
+
+        :param end_date_local: (optional) efforts after this date will be excluded.
+                                           Either as ISO8601 or datetime object
+        :type end_date_local: datetime.datetime or str
+
+        :param limit: (optional), limit number of efforts.
+        :type limit: int
+
+        :return: An iterator of :class:`stravalib.model.SegmentEffort` efforts on a segment.
+        :rtype: :class:`BatchedResultsIterator`
 
         """
         params = {"segment_id": segment_id}
 
         if athlete_id is not None:
             params["athlete_id"] = athlete_id
 
@@ -1303,34 +1180,33 @@
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
     def explore_segments(
         self, bounds, activity_type=None, min_cat=None, max_cat=None
     ):
-        """Returns an array of up to 10 segments.
+        """
+        Returns an array of up to 10 segments.
 
         https://developers.strava.com/docs/reference/#api-Segments-exploreSegments
 
-        Parameters
-        ----------
-        bounds : list of 4 floats or list of 2 (lat,lon) tuples
-            list of bounding box corners lat/lon
-            [sw.lat, sw.lng, ne.lat, ne.lng] (south,west,north,east)
-        activity_type : str
-            optional, default is riding)  'running' or 'riding'
-        min_cat : int, optional, default=None
-            Minimum climb category filter
-        max_cat : int, optional, default=None
-            Maximum climb category filter
+        :param bounds: list of bounding box corners lat/lon [sw.lat, sw.lng, ne.lat, ne.lng] (south,west,north,east)
+        :type bounds: list of 4 floats or list of 2 (lat,lon) tuples
 
-        Returns
-        -------
-        py:class:`list`
-            An list of :class:`stravalib.model.Segment`.
+        :param activity_type: (optional, default is riding)  'running' or 'riding'
+        :type activity_type: str
+
+        :param min_cat: (optional) Minimum climb category filter
+        :type min_cat: int
+
+        :param max_cat: (optional) Maximum climb category filter
+        :type max_cat: int
+
+        :return: An list of :class:`stravalib.model.Segment`.
+        :rtype: :py:class:`list`
 
         """
         if len(bounds) == 2:
             bounds = (bounds[0][0], bounds[0][1], bounds[1][0], bounds[1][1])
         elif len(bounds) != 4:
             raise ValueError(
                 "Invalid bounds specified: {0!r}. Must be list of 4 float values or list of 2 (lat,lon) tuples."
@@ -1360,52 +1236,52 @@
             )
             for v in raw["segments"]
         ]
 
     def get_activity_streams(
         self, activity_id, types=None, resolution=None, series_type=None
     ):
-        """Returns a stream for an activity.
+        """
+        Returns a stream for an activity.
 
         https://developers.strava.com/docs/reference/#api-Streams-getActivityStreams
 
         Streams represent the raw spatial data for the uploaded file. External
         applications may only access this information for activities owned
         by the authenticated athlete.
 
         Streams are available in 11 different types. If the stream is not
         available for a particular activity it will be left out of the request
         results.
 
         Streams types are: time, latlng, distance, altitude, velocity_smooth,
                            heartrate, cadence, watts, temp, moving, grade_smooth
 
-        Parameters
-        ----------
-        activity_id : int
-            The ID of activity.
-        types : list, optional, default=None
-            A list of the types of streams to fetch.
-        resolution : str
-            optional, default is 'all') indicates desired number
-            of data points. 'low' (100), 'medium' (1000),
-            'high' (10000) or 'all'.
-        series_type : str, optional, default='distance'
-            Relevant only if using resolution either 'time' or 'distance'.
-            Used to index the streams if the stream is being reduced.
+        :param activity_id: The ID of activity.
+        :type activity_id: int
 
-        Returns
-        -------
-        py:class:`dict`
-            An dictionary of :class:`stravalib.model.Stream` from the activity
-            or None if there are no streams.
+        :param types: (optional) A list of the types of streams to fetch.
+        :type types: list
+
+        :param resolution: (optional, default is 'all') indicates desired number
+                            of data points. 'low' (100), 'medium' (1000),
+                            'high' (10000) or 'all'.
+        :type resolution: str
 
+        :param series_type: (optional, default is 'distance'.  Relevant only if
+                             using resolution either 'time' or 'distance'.
+                             Used to index the streams if the stream is being
+                             reduced.
+        :type series_type: str
+
+        :return: An dictionary of :class:`stravalib.model.Stream` from the activity or None if there are no streams.
+        :rtype: :py:class:`dict`
         """
 
-        # Stream is a comma separated list
+        # stream are comma seperated list
         if types is not None:
             types = ",".join(types)
 
         params = {}
         if resolution is not None:
             params["resolution"] = resolution
 
@@ -1431,50 +1307,53 @@
             return {i.type: i for i in streams}
         except exc.ObjectNotFound:
             return None  # just to be explicit.
 
     def get_effort_streams(
         self, effort_id, types=None, resolution=None, series_type=None
     ):
-        """Returns an streams for an effort.
+        """
+        Returns an streams for an effort.
 
         https://developers.strava.com/docs/reference/#api-Streams-getSegmentEffortStreams
 
         Streams represent the raw data of the uploaded file. External
         applications may only access this information for activities owned
         by the authenticated athlete.
 
         Streams are available in 11 different types. If the stream is not
         available for a particular activity it will be left out of the request
         results.
 
         Streams types are: time, latlng, distance, altitude, velocity_smooth,
                            heartrate, cadence, watts, temp, moving, grade_smooth
 
-        Parameters
-        ----------
-        effort_id : int
-            The ID of effort.
-        types : list, optional, default=None
-            A list of the the types of streams to fetch.
-        resolution : str, optional, default='all'
-            Indicates desired number of data points. 'low' (100), 'medium'
-            (1000), 'high' (10000) or 'all'.
-        series_type : str, optional, default='distance'
-            Relevant only if using resolution either 'time' or 'distance'.
-            Used to index the streams if the stream is being reduced.
+        :param effort_id: The ID of effort.
+        :type effort_id: int
 
-        Returns
-        -------
-        py:class:`dict`
-            An dictionary of :class:`stravalib.model.Stream` from the effort.
+        :param types: (optional) A list of the the types of streams to fetch.
+        :type types: list
+
+        :param resolution: (optional, default is 'all') indicates desired number
+                            of data points. 'low' (100), 'medium' (1000),
+                            'high' (10000) or 'all'.
+        :type resolution: str
+
+        :param series_type: (optional, default is 'distance'.  Relevant only if
+                             using resolution either 'time' or 'distance'.
+                             Used to index the streams if the stream is being
+                             reduced.
+        :type series_type: str
+
+        :return: An dictionary of :class:`stravalib.model.Stream` from the effort.
+        :rtype: :py:class:`dict`
 
         """
 
-        # Stream are comma separated lists
+        # stream are comma seperated list
         if types is not None:
             types = ",".join(types)
 
         params = {}
         if resolution is not None:
             params["resolution"] = resolution
 
@@ -1497,50 +1376,52 @@
 
         # Pack streams into dictionary
         return {i.type: i for i in streams}
 
     def get_segment_streams(
         self, segment_id, types=None, resolution=None, series_type=None
     ):
-        """Returns an streams for a segment.
+        """
+        Returns an streams for a segment.
 
         https://developers.strava.com/docs/reference/#api-Streams-getSegmentStreams
 
         Streams represent the raw data of the uploaded file. External
         applications may only access this information for activities owned
         by the authenticated athlete.
 
         Streams are available in 11 different types. If the stream is not
         available for a particular activity it will be left out of the request
         results.
 
         Streams types are: time, latlng, distance, altitude, velocity_smooth,
                            heartrate, cadence, watts, temp, moving, grade_smooth
 
-        Parameters
-        ----------
-        segment_id : int
-            The ID of segment.
-        types : list, optional, default=None
-            A list of the the types of streams to fetch.
-        resolution : str, optional, default='all'
-            Indicates desired number of data points. 'low' (100), 'medium'
-            (1000), 'high' (10000) or 'all'.
-        series_type : str, optional, default='distance'
-            Relevant only if using resolution either 'time' or 'distance'.
-            Used to index the streams if the stream is being reduced.
+        :param segment_id: The ID of segment.
+        :type segment_id: int
 
-        Returns
-        -------
-        py:class:`dict`
-            An dictionary of :class:`stravalib.model.Stream` from the effort.
+        :param types: (optional) A list of the the types of streams to fetch.
+        :type types: list
+
+        :param resolution: (optional, default is 'all') indicates desired number
+                            of data points. 'low' (100), 'medium' (1000),
+                            'high' (10000) or 'all'.
+        :type resolution: str
+
+        :param series_type: (optional, default is 'distance'.  Relevant only if
+                             using resolution either 'time' or 'distance'.
+                             Used to index the streams if the stream is being
+                             reduced.
+        :type series_type: str
 
+        :return: An dictionary of :class:`stravalib.model.Stream` from the effort.
+        :rtype: :py:class:`dict`
         """
 
-        # Stream are comma separated lists
+        # stream are comma seperated list
         if types is not None:
             types = ",".join(types)
 
         params = {}
         if resolution is not None:
             params["resolution"] = resolution
 
@@ -1561,30 +1442,26 @@
             result_fetcher=result_fetcher,
         )
 
         # Pack streams into dictionary
         return {i.type: i for i in streams}
 
     def get_routes(self, athlete_id=None, limit=None):
-        """Gets the routes list for an authenticated user.
+        """
+        Gets the routes list for an authenticated user.
 
         https://developers.strava.com/docs/reference/#api-Routes-getRoutesByAthleteId
 
-        Parameters
-        ----------
-        athlete_id : int, default=None
-            Strava athlete ID
-        limit : int, default=unlimited
-            Max rows to return.
+        :param athlete_id: id for the
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Route` objects.
+        :param limit: Max rows to return (default unlimited).
+        :type limit: int
 
+        :return: An iterator of :class:`stravalib.model.Route` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         if athlete_id is None:
             athlete_id = self.get_athlete().id
 
         result_fetcher = functools.partial(
             self.protocol.get, "/athletes/{id}/routes".format(id=athlete_id)
         )
@@ -1593,54 +1470,45 @@
             entity=model.Route,
             bind_client=self,
             result_fetcher=result_fetcher,
             limit=limit,
         )
 
     def get_route(self, route_id):
-        """Gets specified route.
+        """
+        Gets specified route.
 
-        Will be detail-level if owned by authenticated user; otherwise
-        summary-level.
+        Will be detail-level if owned by authenticated user; otherwise summary-level.
 
         https://developers.strava.com/docs/reference/#api-Routes-getRouteById
 
-        Parameters
-        ----------
-        route_id : int
-            The ID of route to fetch.
-
-        Returns
-        -------
-        class: `model.Route`
-            A model.Route object containing the route data.
+        :param route_id: The ID of route to fetch.
+        :type route_id: int
 
+        :rtype: :class:`stravalib.model.Route`
         """
         raw = self.protocol.get("/routes/{id}", id=route_id)
         return model.Route.parse_obj({**raw, **{"bound_client": self}})
 
     def get_route_streams(self, route_id):
-        """Returns streams for a route.
+        """
+        Returns streams for a route.
 
         Streams represent the raw data of the saved route. External
         applications may access this information for all public routes and for
         the private routes of the authenticated athlete. The 3 available route
         stream types `distance`, `altitude` and `latlng` are always returned.
 
         See: https://developers.strava.com/docs/reference/#api-Streams-getRouteStreams
 
-        Parameters
-        ----------
-        route_id : int
-            The ID of activity.
+        :param route_id: The ID of activity.
+        :type route_id: int
 
-        Returns
-        -------
-        py:class:`dict`
-            A dictionary of :class:`stravalib.model.Stream` from the route.
+        :return: A dictionary of :class:`stravalib.model.Stream` from the route.
+        :rtype: :py:class:`dict`
 
         """
 
         result_fetcher = functools.partial(
             self.protocol.get, "/routes/{id}/streams/".format(id=route_id)
         )
 
@@ -1658,182 +1526,155 @@
     def create_subscription(
         self,
         client_id,
         client_secret,
         callback_url,
         verify_token=model.Subscription.VERIFY_TOKEN_DEFAULT,
     ):
-        """Creates a webhook event subscription.
+        """
+        Creates a webhook event subscription.
 
-        Parameters
-        ----------
-        client_id : int
-            application's ID, obtained during registration
-        client_secret : str
-            application's secret, obtained during registration
-        callback_url : str
-            callback URL where Strava will first send a GET request to validate,
-            then subsequently send POST requests with updates
-        verify_token : str
-            a token you can use to verify Strava's GET callback request (Default
-            value = model.Subscription.VERIFY_TOKEN_DEFAULT)
+        :param client_id: application's ID, obtained during registration
+        :type client_id: int
 
-        Returns
-        -------
-        class:`stravalib.model.Subscription`
+        :param client_secret: application's secret, obtained during registration
+        :type client_secret: str
+
+        :param callback_url: callback URL where Strava will first send a GET request to validate, then subsequently send POST requests with updates
+        :type callback_url: str
+
+        :param verify_token: a token you can use to verify Strava's GET callback request
+        :type verify_token: str
 
-        Notes
-        -----
+        :return: An instance of :class:`stravalib.model.Subscription`.
+        :rtype: :class:`stravalib.model.Subscription`
 
-        `verify_token` is set to a default in the event that the author
-        doesn't want to specify one.
+        Notes:
 
-        The application must have permission to make use of the webhook API.
-        Access can be requested by contacting developers -at- strava.com.
-        An instance of :class:`stravalib.model.Subscription`.
+        `verify_token` is set to a default in the event that the author doesn't want to specify one.
 
+        The appliction must have permission to make use of the webhook API. Access can be requested by contacting developers -at- strava.com.
         """
         params = dict(
             client_id=client_id,
             client_secret=client_secret,
             callback_url=callback_url,
             verify_token=verify_token,
         )
         raw = self.protocol.post("/push_subscriptions", **params)
         return model.Subscription.parse_obj({**raw, **{"bound_client": self}})
 
-    # TODO: UPDATE - this method uses (de)serialize which is deprecated
     def handle_subscription_callback(
         self, raw, verify_token=model.Subscription.VERIFY_TOKEN_DEFAULT
     ):
-        """Validate callback request and return valid response with challenge.
-
-        Parameters
-        ----------
-        raw : dict
-            The raw JSON response which will be serialized to a Python dict.
-        verify_token : default=model.Subscription.VERIFY_TOKEN_DEFAULT
-
-        Returns
-        -------
-        Dict[str, str]
-            The JSON response expected by Strava to the challenge request.
+        """
+        Validate callback request and return valid response with challenge.
 
+        :return: The JSON response expected by Strava to the challenge request.
+        :rtype: Dict[str, str]
         """
         callback = model.SubscriptionCallback.deserialize(raw)
         callback.validate(verify_token)
         response_raw = {"hub.challenge": callback.hub_challenge}
         return response_raw
 
-    # TODO: i'm not sure what raw's "type" is here
     def handle_subscription_update(self, raw):
-        """Converts a raw subscription update into a model.
-
-        Parameters
-        ----------
-        raw : dict
-            The raw json response deserialized into a dict.
-
-        Returns
-        -------
-        class:`stravalib.model.SubscriptionUpdate`
-            The subscription update model object.
+        """
+        Converts a raw subscription update into a model.
 
+        :return: The subscription update model object.
+        :rtype: :class:`stravalib.model.SubscriptionUpdate`
         """
         return model.SubscriptionUpdate.parse_obj(
             {**raw, **{"bound_client": self}}
         )
 
+    # TODO can't find a api doc link here so just removed old link.
     def list_subscriptions(self, client_id, client_secret):
-        """List current webhook event subscriptions in place for the current
-        application.
+        """
+        List current webhook event subscriptions in place for the current application.
 
-        Parameters
-        ----------
-        client_id : int
-            application's ID, obtained during registration
-        client_secret : str
-            application's secret, obtained during registration
+        :param client_id: application's ID, obtained during registration
+        :type client_id: int
 
-        Returns
-        -------
-        class:`BatchedResultsIterator`
-            An iterator of :class:`stravalib.model.Subscription` objects.
+        :param client_secret: application's secret, obtained during registration
+        :type client_secret: str
 
+        :return: An iterator of :class:`stravalib.model.Subscription` objects.
+        :rtype: :class:`BatchedResultsIterator`
         """
         result_fetcher = functools.partial(
             self.protocol.get,
             "/push_subscriptions",
             client_id=client_id,
             client_secret=client_secret,
         )
 
         return BatchedResultsIterator(
             entity=model.Subscription,
             bind_client=self,
             result_fetcher=result_fetcher,
         )
 
+    # TODO can't find a api doc link here so just removed old link.
     def delete_subscription(self, subscription_id, client_id, client_secret):
-        """Unsubscribe from webhook events for an existing subscription.
+        """
+        Unsubscribe from webhook events for an existing subscription.
 
-        Parameters
-        ----------
-        subscription_id : int
-            ID of subscription to remove.
-        client_id : int
-            application's ID, obtained during registration
-        client_secret : str
-            application's secret, obtained during registration
+        :param subscription_id: ID of subscription to remove.
+        :type subscription_id: int
 
-        Returns
-        -------
-        Deletes the specific subscription using the subscription ID
+        :param client_id: application's ID, obtained during registration
+        :type client_id: int
 
+        :param client_secret: application's secret, obtained during registration
+        :type client_secret: str
         """
         self.protocol.delete(
             "/push_subscriptions/{id}",
             id=subscription_id,
             client_id=client_id,
             client_secret=client_secret,
         )
         # Expects a 204 response if all goes well.
 
 
 class BatchedResultsIterator(object):
-    """An iterator that enables iterating over requests that return
-    paged results."""
+    """
+    An iterator that enables iterating over requests that return paged results.
+    """
 
-    # Number of results returned in a batch. We maximize this to minimize
-    # requests to server (rate limiting)
+    # How many results returned in a batch.  We maximize this to minimize
+    #  requests to server (rate limiting)
     default_per_page = 200
 
     def __init__(
         self,
         entity,
         result_fetcher,
         bind_client=None,
         limit=None,
         per_page=None,
     ):
         """
+        :param entity: The class for the model entity.
+        :type entity: type
 
-        Parameters
-        ----------
-        entity : type
-            The class for the model entity.
-        result_fetcher: callable
-            The callable that will return another batch of results.
-        bind_client: :class:`stravalib.client.Client`
-            The client object to pass to the entities for supporting further
-            fetching of objects.
-        limit: int
-            The maximum number of rides to return.
-        per_page: int
-            How many rows to fetch per page (default is 200).
+        :param result_fetcher: The callable that will return another batch of results.
+        :type result_fetcher: callable
+
+        :param bind_client: The client object to pass to the entities for supporting further
+                             fetching of objects.
+        :type bind_client: :class:`stravalib.client.Client`
+
+        :param limit: The maximum number of rides to return.
+        :type limit: int
+
+        :param per_page: How many rows to fetch per page (default is 200).
+        :type per_page: int
         """
         self.log = logging.getLogger(
             "{0.__module__}.{0.__name__}".format(self.__class__)
         )
         self.entity = entity
         self.bind_client = bind_client
         self.result_fetcher = result_fetcher
@@ -1848,38 +1689,38 @@
 
     def __repr__(self):
         return "<{0} entity={1}>".format(
             self.__class__.__name__, self.entity.__name__
         )
 
     def reset(self):
-        """ """
         self._counter = 0
         self._buffer = None
         self._page = 1
         self._all_results_fetched = False
 
     def _fill_buffer(self):
-        """Fills the internal buffer from Strava API."""
+        """
+        Fills the internal buffer from Strava API.
+        """
         # If we cannot fetch anymore from the server then we're done here.
         if self._all_results_fetched:
             self._eof()
         raw_results = self.result_fetcher(
             page=self._page, per_page=self.per_page
         )
 
         entities = []
         for raw in raw_results:
             try:
                 new_entity = self.entity.parse_obj(
                     {**raw, **{"bound_client": self.bind_client}}
                 )
             except AttributeError:
-                # Entity doesn't have a parse_obj() method, so must be of a
-                # legacy type
+                # entity doesn't have a parse_obj() method, so must be of a legacy type
                 new_entity = self.entity.deserialize(
                     raw, bind_client=self.bind_client
                 )
             entities.append(new_entity)
 
         self._buffer = collections.deque(entities)
 
@@ -1893,23 +1734,21 @@
 
         self._page += 1
 
     def __iter__(self):
         return self
 
     def _eof(self):
-        """ """
         self.reset()
         raise StopIteration
 
     def __next__(self):
         return self.next()
 
     def next(self):
-        """ """
         if self.limit and self._counter >= self.limit:
             self._eof()
         if not self._buffer:
             self._fill_buffer()
         try:
             result = self._buffer.popleft()
         except IndexError:
@@ -1917,207 +1756,160 @@
         else:
             self._counter += 1
             return result
 
 
 class ActivityUploader(object):
     """
-    The "future" object that holds information about an activity file
-    upload and can wait for upload to finish, etc.
-
+    The "future" object that holds information about an activity file upload and can
+    wait for upload to finish, etc.
     """
 
     def __init__(self, client, response, raise_exc=True):
         """
-        client: `stravalib.client.Client`
-            The :class:`stravalib.client.Client` object that is handling the
-            upload.
-        response: Dict[str,Any]
-            The initial upload response.
-        raise_exc: bool
-            Whether to raise an exception if the response
-            indicates an error state. (default True)
+        :param client: The :class:`stravalib.client.Client` object that is handling the upload.
+        :type client: :class:`stravalib.client.Client`
+
+        :param response: The initial upload response.
+        :type response: Dict[str,Any]
+
+        :param raise_exc: Whether to raise an exception if the response
+                  indicates an error state. (default True)
+        :type raise_exc: bool
         """
         self.client = client
         self.response = response
         self.update_from_response(response, raise_exc=raise_exc)
 
     @property
     def photo_metadata(self):
-        """photo metadata for the activity upload response, if any.
+        """
+        photo metadata for the activity upload response, if any.
         it contains a pre-signed uri for uploading the photo.
-
-        Notes
-        -----
-        * This is only available after the upload has completed.
-        * This metadata is only available for partner apps. If you have a
-        regular / non partner related Strava app / account it will not work.
-
+        Note1: This is only available after the upload has completed.
+        Note2: available only for partner apps (not for regular account)
         """
 
         warn_attribute_unofficial("photo_metadata")
 
         return self._photo_metadata
 
     @photo_metadata.setter
     def photo_metadata(self, value):
-        """
-
-        Parameters
-        ----------
-        value : list of dictionaries or none
-            Contains an optional list of dictionaries with photo metadata or a
-            value of `None`.
-
-        Returns
-        -------
-        Updates the `_photo_metadata` value in the object
-
-        """
         self._photo_metadata = value
 
     def update_from_response(self, response, raise_exc=True):
-        """Updates internal state of object.
-
-        Parameters
-        ----------
-        response : py:class:`dict`
-            The response object (dict).
-        raise_exc : bool
-
-        Raises
-        ------
-        stravalib.exc.ActivityUploadFailed
-            If the response indicates an
-            error and raise_exc is True. Whether to raise an exception if the
-            response indicates an error state. (default True)
-
-        Returns
-        -------
+        """
+        Updates internal state of object.
 
+        :param response: The response object (dict).
+        :type response: :py:class:`dict`
+        :param raise_exc: Whether to raise an exception if the response
+                          indicates an error state. (default True)
+        :type raise_exc: bool
+        :raise stravalib.exc.ActivityUploadFailed: If the response indicates an error and raise_exc is True.
         """
         self.upload_id = response.get("id")
         self.external_id = response.get("external_id")
         self.activity_id = response.get("activity_id")
         self.status = response.get("status") or response.get("message")
-        # Undocumented field, it contains pre-signed uri to upload photo to
+        # undocumented field, it contains pre-signed uri to upload photo to
         self._photo_metadata: Optional[List[Dict]] = response.get(
             "photo_metadata"
         )
 
         if response.get("error"):
             self.error = response.get("error")
         elif response.get("errors"):
-            # This appears to be an undocumented API; ths is a bit of a hack
-            # for now.
+            # This appears to be an undocumented API; ths is a bit of a hack for now.
             self.error = str(response.get("errors"))
         else:
             self.error = None
 
         if raise_exc:
             self.raise_for_error()
 
     @property
     def is_processing(self):
-        """ """
         return self.activity_id is None and self.error is None
 
     @property
     def is_error(self):
-        """ """
         return self.error is not None
 
     @property
     def is_complete(self):
-        """ """
         return self.activity_id is not None
 
     def raise_for_error(self):
-        """ """
-        # FIXME: We need better handling of the actual responses, once those are
-        # more accurately documented.
+        # FIXME: We need better handling of the actual responses, once those are more accurately documented.
         if self.error:
             raise exc.ActivityUploadFailed(self.error)
         elif self.status == "The created activity has been deleted.":
             raise exc.CreatedActivityDeleted(self.status)
 
     def poll(self):
-        """Update internal state from polling strava.com.
-
-        Raises
-        -------
-        class: `stravalib.exc.ActivityUploadFailed` If poll returns an error.
+        """
+        Update internal state from polling strava.com.
 
+        :raise stravalib.exc.ActivityUploadFailed: If the poll returns an error.
         """
         response = self.client.protocol.get(
             "/uploads/{upload_id}",
             upload_id=self.upload_id,
             check_for_errors=False,
         )
 
         self.update_from_response(response)
 
     def wait(self, timeout=None, poll_interval=1.0):
-        """Wait for the upload to complete or to err out.
+        """
+        Wait for the upload to complete or to err out.
 
-        Will return the resulting Activity or raise an exception if the
-        upload fails.
+        Will return the resulting Activity or raise an exception if the upload fails.
 
-        Parameters
-        ----------
-        timeout : float, default=None
-            The max seconds to wait. Will raise TimeoutExceeded
-            exception if this time passes without success or error response.
-        poll_interval : float, default=1.0 (seconds)
-            How long to wait between upload checks.  Strava
-            recommends 1s minimum.
+        :param timeout: The max seconds to wait. Will raise TimeoutExceeded
+                        exception if this time passes without success or error response.
+        :type timeout: float
 
-        Returns
-        -------
-        class:`stravalib.model.Activity`
+        :param poll_interval: How long to wait between upload checks.  Strava
+                              recommends 1s minimum. (default 1.0s)
+        :type poll_interval: float
 
-        Raises
-        ------
-        stravalib.exc.TimeoutExceeded
-            If a timeout was specified and activity is still processing
-            after timeout has elapsed.
-        stravalib.exc.ActivityUploadFailed
-            If the poll returns an error.
-            The uploaded Activity object (fetched from server)
+        :return: The uploaded Activity object (fetched from server)
+        :rtype: :class:`stravalib.model.Activity`
 
+        :raise stravalib.exc.TimeoutExceeded: If a timeout was specified and
+                                              activity is still processing after
+                                              timeout has elapsed.
+        :raise stravalib.exc.ActivityUploadFailed: If the poll returns an error.
         """
         start = time.time()
         while self.activity_id is None:
             self.poll()
             time.sleep(poll_interval)
             if timeout and (time.time() - start) > timeout:
                 raise exc.TimeoutExceeded()
         # If we got this far, we must have an activity!
         return self.client.get_activity(self.activity_id)
 
     def upload_photo(self, photo, timeout=None):
-        """Uploads a photo to the activity.
+        """
+        Uploads a photo to the activity.
 
-        Parameters
-        ----------
-        photo : bytes
-            The file-like object to upload.
-        timeout : float, default=None
-            The max seconds to wait. Will raise TimeoutExceeded
-
-        Notes
-        -----
-        In order to upload a photo, the activity must be uploaded and
-        processed.
-
-        The ability to add photos to activity is currently limited to
-        partner apps & devices such as Zwift, Peloton, Tempo Move, etc...
-        Given that the ability isn't in the public API, neither are the docs
+        NOTE1: In order to upload a photo, the activity must be uploaded and processed.
+
+        NOTE2: The ability to add photos to activity is currently limited to partner apps & devices such as Zwift,
+        Peloton, Tempo Move, etc... Given that the ability isn't in the public API, neither are the docs
 
+        :param photo: The file-like object to upload.
+        :type photo: bytes
 
+        :param timeout: The max seconds to wait. Will raise TimeoutExceeded
+        :type timeout: float
         """
 
         warn_method_unofficial("upload_photo")
 
         try:
             if not isinstance(photo, bytes):
                 raise TypeError("Photo must be bytes type")
```

### Comparing `stravalib-1.3.0/stravalib/exc.py` & `stravalib-1.3.0rc0/stravalib/exc.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,61 +118,47 @@
         f'The method "{method_name}" of class "{klass}" is deprecated and will be '
         f'removed in the future. Instead, you can use "{alternative}".{alt_support_msg}',
         DeprecationWarning,
         stacklevel=3,
     )
 
 
-def warn_param_unsupported(param_name: str):
+def warn_param_deprecation(param_name: str):
     warnings.warn(
         f'The "{param_name}" parameter is unsupported by the Strava API. It has no '
         "effect and may lead to errors in the future.",
         DeprecationWarning,
         stacklevel=3,
     )
 
 
-def warn_param_deprecation(
-    param_name: str, alternative: str, alt_url: str = None
-):
-    alt_support_msg = (
-        f" See {alt_url} for more information." if alt_url else ""
-    )
-    warnings.warn(
-        f'The "{param_name}" parameter is deprecated and will be removed'
-        f'in the future. Instead, you can use "{alternative}".{alt_support_msg}',
-        DeprecationWarning,
-        stacklevel=3,
-    )
-
-
 def warn_param_unofficial(param_name: str):
     warnings.warn(
         f'The "{param_name}" parameter is undocumented in the Strava API. Its use '
         "may lead to unexpected behavior or errors in the future.",
         FutureWarning,
         stacklevel=3,
     )
 
 
 def warn_attribute_unofficial(attr_name: str):
     warnings.warn(
         f'The "{attr_name}" parameter is undocumented in the Strava API. Its use '
-        "may lead to unexpected behavior or errors in the future.",
+        'may lead to unexpected behavior or errors in the future.',
         FutureWarning,
-        stacklevel=3,
+        stacklevel=3
     )
 
 
 def warn_method_unofficial(method_name: str):
     warnings.warn(
         f'The "{method_name}" method is undocumented in the Strava API. Its use '
-        "may lead to unexpected behavior or errors in the future.",
+        'may lead to unexpected behavior or errors in the future.',
         FutureWarning,
-        stacklevel=3,
+        stacklevel=3
     )
 
 
 def warn_units_deprecated():
     warnings.warn(
         "You are using a Quantity object or attributes from the units library, which is "
         "deprecated. Support for these types will be removed in the future. Instead, "
```

### Comparing `stravalib-1.3.0/stravalib/field_conversions.py` & `stravalib-1.3.0rc0/stravalib/field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/model.py` & `stravalib-1.3.0rc0/stravalib/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     Lap,
     LatLng,
     PhotosSummary,
     PolylineMap,
     Primary,
     Route,
     Split,
-    SportType,
     SummaryPRSegmentEffort,
     SummarySegmentEffort,
     TimedZoneRange,
 )
 
 LOGGER = logging.getLogger(__name__)
 
@@ -59,80 +58,51 @@
     Should be used to decorate the functions that return a lazily loaded
     entity (collection), e.g., the members of a club.
 
     Assumes that fn (like a regular getter property) has as single
     argument a reference to self, and uses one of the (bound) client
     methods to retrieve an entity (collection) by self.id.
     """
-
     @wraps(fn)
     def wrapper(obj):
         try:
             if obj.bound_client is None:
                 raise exc.UnboundEntity(
                     f"Unable to fetch objects for unbound {obj.__class__} entity."
                 )
             if obj.id is None:
-                LOGGER.warning(
-                    f"Cannot retrieve {obj.__class__}.{fn.__name__}, self.id is None"
-                )
+                LOGGER.warning(f'Cannot retrieve {obj.__class__}.{fn.__name__}, self.id is None')
                 return None
             return fn(obj)
         except AttributeError as e:
             raise exc.UnboundEntity(
                 f"Unable to fetch objects for unbound {obj.__class__} entity: {e}"
             )
 
     return property(wrapper)
 
 
 # Custom validators for some edge cases:
 
-
-def check_valid_location(
-    location: Optional[Union[List[float], str]]
-) -> Optional[List[float]]:
-    """
-    Parameters
-    ----------
-    location : list of float
-        Either a list of x,y floating point values or strings or None
-        (The legacy serialized format is str)
-
-    Returns
-    --------
-    list or None
-        Either returns a list of floating point values representing location
-        x,y data or None if empty list is returned from the API.
-
-    Raises
-    ------
-    AttributeError
-        If empty list is returned, raises AttributeError
-
-    """
-
-    # Legacy serialized form is str, so in case of attempting to de-serialize
-    # from local storage:
+def check_valid_location(location: Optional[Union[List[float], str]]) -> Optional[List[float]]:
+    # legacy serialized form is str, so in case of attempting to de-serialize from local storage:
     try:
-        return [float(l) for l in location.split(",")]
+        return [float(l) for l in location.split(',')]
     except AttributeError:
-        # Location for activities without GPS may be returned as empty list by
-        # Strava
+        # location for activities without GPS may be returned as empty list by Strava
         return location if location else None
 
 
 def naive_datetime(value: Optional[Any]) -> Optional[datetime]:
     if value:
         dt = parse_datetime(value)
         return dt.replace(tzinfo=None)
     else:
         return None
 
-
 class DeprecatedSerializableMixin(BaseModel):
     """
     Provides backward compatibility with legacy BaseEntity
     """
 
     @classmethod
     def deserialize(cls, attribute_value_mapping: Dict):
@@ -181,17 +151,15 @@
     * _field_conversions
     * _deprecated_fields (TODO)
     * _unsupported_fields (TODO)
     """
 
     def __getattribute__(self, attr):
         value = object.__getattribute__(self, attr)
-        if attr in ["_field_conversions", "bound_client"] or attr.startswith(
-            "_"
-        ):
+        if attr in ["_field_conversions", "bound_client"] or attr.startswith('_'):
             return value
         try:
             if attr in self._field_conversions:
                 return self._field_conversions[attr](value)
         except AttributeError:
             # Current model class has no field conversions defined
             pass
@@ -257,15 +225,15 @@
     def activities(self):
         return self.bound_client.get_club_activities(self.id)
 
 
 class Gear(
     DetailedGear, DeprecatedSerializableMixin, BackwardCompatibilityMixin
 ):
-    _field_conversions = {"distance": uh.meters}
+    _field_conversions = {'distance': uh.meters}
 
 
 class Bike(Gear):
     pass
 
 
 class Shoe(Gear):
@@ -275,15 +243,15 @@
 class ActivityTotals(
     ActivityTotal, DeprecatedSerializableMixin, BackwardCompatibilityMixin
 ):
     _field_conversions = {
         "elapsed_time": time_interval,
         "moving_time": time_interval,
         "distance": uh.meters,
-        "elevation_gain": uh.meters,
+        "elevation_gain": uh.meters
     }
 
 
 class AthleteStats(
     ActivityStats, DeprecatedSerializableMixin, BackwardCompatibilityMixin
 ):
     """
@@ -305,18 +273,15 @@
     _field_conversions = {
         "biggest_ride_distance": uh.meters,
         "biggest_climb_elevation_gain": uh.meters,
     }
 
 
 class Athlete(
-    DetailedAthlete,
-    DeprecatedSerializableMixin,
-    BackwardCompatibilityMixin,
-    BoundClientEntity,
+    DetailedAthlete, DeprecatedSerializableMixin, BackwardCompatibilityMixin, BoundClientEntity
 ):
     # field overrides from superclass for type extensions:
     clubs: Optional[List[Club]] = None
     bikes: Optional[List[Bike]] = None
     shoes: Optional[List[Shoe]] = None
 
     # Undocumented attributes:
@@ -354,84 +319,75 @@
     sample_race_distance: Optional[int] = None
     sample_race_time: Optional[int] = None
     membership: Optional[str] = None
     admin: Optional[bool] = None
     owner: Optional[bool] = None
     subscription_permissions: Optional[list] = None
 
-    @validator("athlete_type")
+    @validator('athlete_type')
     def to_str_representation(cls, raw_type):
         # Replaces legacy "ChoicesAttribute" class
         return {0: "cyclist", 1: "runner"}.get(raw_type)
 
     @lazy_property
     def authenticated_athlete(self):
         return self.bound_client.get_athlete()
 
     @lazy_property
     def stats(self):
         """
-        Returns
-        -------
-        Associated :class:`stravalib.model.AthleteStats`
+        :return: Associated :class:`stravalib.model.AthleteStats`
         """
         if not self.is_authenticated_athlete():
-            raise exc.NotAuthenticatedAthlete(
-                "Statistics are only available for the authenticated athlete"
-            )
+            raise exc.NotAuthenticatedAthlete("Statistics are only available for the authenticated athlete")
         return self.bound_client.get_athlete_stats(self.id)
 
+
     def is_authenticated_athlete(self):
         """
-        Returns
-        -------
-        bool
-            Whether the athlete is the authenticated athlete (or not).
+        :return: Boolean as to whether the athlete is the authenticated athlete.
         """
 
         if self.is_authenticated is None:
             if self.resource_state == 3:
                 # If the athlete is in detailed state it must be the authenticated athlete
                 self.is_authenticated = True
             else:
                 # We need to check this athlete's id matches the authenticated athlete's id
                 authenticated_athlete = self.authenticated_athlete
                 self.is_authenticated = authenticated_athlete.id == self.id
 
         return self.is_authenticated
 
-
 class ActivityComment(Comment):
-    # Field overrides from superclass for type extensions:
+    # field overrides from superclass for type extensions:
     athlete: Optional[Athlete] = None
 
 
 class ActivityPhotoPrimary(Primary):
     # Undocumented attributes:
     use_primary_photo: Optional[bool] = None
 
 
 class ActivityPhotoMeta(PhotosSummary):
     """
-    The photos structure returned with the activity, not to be confused with
-    the full loaded photos for an activity.
+    The photos structure returned with the activity, not to be confused with the full loaded photos for an activity.
     """
 
     # field overrides from superclass for type extensions:
     primary: Optional[ActivityPhotoPrimary] = None
 
     # Undocumented attributes:
     use_primary_photo: Optional[bool] = None
 
 
 class ActivityPhoto(BackwardCompatibilityMixin, DeprecatedSerializableMixin):
     """
     A full photo record attached to an activity.
-    Warning: this entity is undocumented by Strava and there is no official
-    endpoint to retrieve it
+    Warning: this entity is undocumented by Strava and there is no official endpoint to retrieve it
     """
 
     athlete_id: Optional[int] = None
     activity_id: Optional[int] = None
     activity_name: Optional[str] = None
     ref: Optional[str] = None
     uid: Optional[str] = None
@@ -444,20 +400,16 @@
     location: Optional[LatLon] = None
     urls: Optional[Dict] = None
     sizes: Optional[Dict] = None
     post_id: Optional[int] = None
     default_photo: Optional[bool] = None
     source: Optional[int] = None
 
-    _naive_local = validator("created_at_local", allow_reuse=True)(
-        naive_datetime
-    )
-    _check_latlng = validator("location", allow_reuse=True, pre=True)(
-        check_valid_location
-    )
+    _naive_local = validator('created_at_local', allow_reuse=True)(naive_datetime)
+    _check_latlng = validator('location', allow_reuse=True, pre=True)(check_valid_location)
 
     def __repr__(self):
         if self.source == 1:
             photo_type = "native"
             idfield = "unique_id"
             idval = self.unique_id
         elif self.source == 2:
@@ -481,42 +433,35 @@
     """
     Activity kudos are a subset of athlete properties.
     """
 
     pass
 
 
-class ActivityLap(
-    Lap,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
-):
-    # Field overrides from superclass for type extensions:
+class ActivityLap(Lap, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
+    # field overrides from superclass for type extensions:
     activity: Optional[Activity] = None
     athlete: Optional[Athlete] = None
 
     # Undocumented attributes:
     average_watts: Optional[float] = None
     average_heartrate: Optional[float] = None
     max_heartrate: Optional[float] = None
     device_watts: Optional[bool] = None
 
     _field_conversions = {
-        "elapsed_time": time_interval,
-        "moving_time": time_interval,
-        "distance": uh.meters,
-        "total_elevation_gain": uh.meters,
-        "average_speed": uh.meters_per_second,
-        "max_speed": uh.meters_per_second,
+        'elapsed_time': time_interval,
+        'moving_time': time_interval,
+        'distance': uh.meters,
+        'total_elevation_gain': uh.meters,
+        'average_speed': uh.meters_per_second,
+        'max_speed': uh.meters_per_second
     }
 
-    _naive_local = validator("start_date_local", allow_reuse=True)(
-        naive_datetime
-    )
+    _naive_local = validator('start_date_local', allow_reuse=True)(naive_datetime)
 
 
 class Map(PolylineMap):
     pass
 
 
 class Split(Split, BackwardCompatibilityMixin, DeprecatedSerializableMixin):
@@ -526,112 +471,93 @@
     """
 
     # Undocumented attributes:
     average_heartrate: Optional[float] = None
     average_grade_adjusted_speed: Optional[float] = None
 
     _field_conversions = {
-        "elapsed_time": time_interval,
-        "moving_time": time_interval,
-        "distance": uh.meters,
-        "elevation_difference": uh.meters,
-        "average_speed": uh.meters_per_second,
-        "average_grade_adjusted_speed": uh.meters_per_second,
+        'elapsed_time': time_interval,
+        'moving_time': time_interval,
+        'distance': uh.meters,
+        'elevation_difference': uh.meters,
+        'average_speed': uh.meters_per_second,
+        'average_grade_adjusted_speed': uh.meters_per_second
     }
 
 
 class SegmentExplorerResult(
-    ExplorerSegment,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
+    ExplorerSegment, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity
 ):
     """
     Represents a segment result from the segment explorer feature.
 
     (These are not full segment objects, but the segment object can be fetched
     via the 'segment' property of this object.)
     """
 
-    # Field overrides from superclass for type extensions:
+    # field overrides from superclass for type extensions:
     start_latlng: Optional[LatLon] = None
     end_latlng: Optional[LatLon] = None
 
     # Undocumented attributes:
     starred: Optional[bool] = None
 
-    _field_conversions = {"elev_difference", uh.meters, "distance", uh.meters}
+    _field_conversions = {
+        'elev_difference', uh.meters,
+        'distance', uh.meters
+    }
 
-    _check_latlng = validator(
-        "start_latlng", "end_latlng", allow_reuse=True, pre=True
-    )(check_valid_location)
+    _check_latlng = validator('start_latlng', 'end_latlng', allow_reuse=True, pre=True)(check_valid_location)
 
     @lazy_property
     def segment(self):
         """Associated (full) :class:`stravalib.model.Segment` object."""
         return self.bound_client.get_segment(self.id)
 
 
-class AthleteSegmentStats(
-    SummarySegmentEffort,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-):
+class AthleteSegmentStats(SummarySegmentEffort, BackwardCompatibilityMixin, DeprecatedSerializableMixin):
     """
     A structure being returned for segment stats for current athlete.
     """
 
     # Undocumented attributes:
     effort_count: Optional[int] = None
     pr_elapsed_time: Optional[int] = None
     pr_date: Optional[date] = None
 
     _field_conversions = {
-        "elapsed_time": time_interval,
-        "pr_elapsed_time": time_interval,
-        "distance": uh.meters,
+        'elapsed_time': time_interval,
+        'pr_elapsed_time': time_interval,
+        'distance': uh.meters
     }
 
-    _naive_local = validator("start_date_local", allow_reuse=True)(
-        naive_datetime
-    )
+    _naive_local = validator('start_date_local', allow_reuse=True)(naive_datetime)
 
 
-class AthletePrEffort(
-    SummaryPRSegmentEffort,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-):
+class AthletePrEffort(SummaryPRSegmentEffort, BackwardCompatibilityMixin, DeprecatedSerializableMixin):
     # Undocumented attributes:
     distance: Optional[float] = None
     start_date: Optional[datetime] = None
     start_date_local: Optional[datetime] = None
     is_kom: Optional[bool] = None
 
     _field_conversions = {
-        "pr_elapsed_time": time_interval,
-        "distance": uh.meters,
+        'pr_elapsed_time': time_interval,
+        'distance': uh.meters
     }
 
-    _naive_local = validator("start_date_local", allow_reuse=True)(
-        naive_datetime
-    )
+    _naive_local = validator('start_date_local', allow_reuse=True)(naive_datetime)
 
     @property
     def elapsed_time(self):
-        # For backward compatibility
+        # for backward compatibility
         return self.pr_elapsed_time
 
 
-class Segment(
-    DetailedSegment,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
-):
+class Segment(DetailedSegment, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Represents a single Strava segment.
     """
 
     # field overrides from superclass for type extensions:
     start_latlng: Optional[LatLon] = None
     end_latlng: Optional[LatLon] = None
@@ -646,24 +572,22 @@
     end_longitude: Optional[float] = None
     starred: Optional[bool] = None
     pr_time: Optional[int] = None
     starred_date: Optional[datetime] = None
     elevation_profile: Optional[str] = None
 
     _field_conversions = {
-        "distance": uh.meters,
-        "elevation_high": uh.meters,
-        "elevation_low": uh.meters,
-        "total_elevation_gain": uh.meters,
-        "pr_time": time_interval,
+        'distance': uh.meters,
+        'elevation_high': uh.meters,
+        'elevation_low': uh.meters,
+        'total_elevation_gain': uh.meters,
+        'pr_time': time_interval
     }
 
-    _latlng_check = validator(
-        "start_latlng", "end_latlng", allow_reuse=True, pre=True
-    )(check_valid_location)
+    _latlng_check = validator('start_latlng', 'end_latlng', allow_reuse=True, pre=True)(check_valid_location)
 
 
 class SegmentEffortAchievement(BaseModel):
     """
     An undocumented structure being returned for segment efforts.
     """
 
@@ -681,38 +605,31 @@
     """
     Numeric ID for type of achievement?  (6 = year_pr, 2 = overall ??? other?)
     """
 
     effort_count: Optional[int] = None
 
 
-class BaseEffort(
-    DetailedSegmentEffort,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
-):
+class BaseEffort(DetailedSegmentEffort, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Base class for a best effort or segment effort.
     """
 
     # field overrides from superclass for type extensions:
     segment: Optional[Segment] = None
     activity: Optional[Activity] = None
     athlete: Optional[Athlete] = None
 
     _field_conversions = {
-        "moving_time": time_interval,
-        "elapsed_time": time_interval,
-        "distance": uh.meters,
+        'moving_time': time_interval,
+        'elapsed_time': time_interval,
+        'distance': uh.meters
     }
 
-    _naive_local = validator("start_date_local", allow_reuse=True)(
-        naive_datetime
-    )
+    _naive_local = validator('start_date_local', allow_reuse=True)(naive_datetime)
 
 
 class BestEffort(BaseEffort):
     """
     Class representing a best effort (e.g. best time for 5k)
     """
 
@@ -721,20 +638,15 @@
     """
     Class representing a best effort on a particular segment.
     """
 
     achievements: Optional[List[SegmentEffortAchievement]] = None
 
 
-class Activity(
-    DetailedActivity,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
-):
+class Activity(DetailedActivity, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Represents an activity (ride, run, etc.).
     """
 
     # field overrides from superclass for type extensions:
     athlete: Optional[Athlete] = None
     start_latlng: Optional[LatLon] = None
@@ -746,21 +658,15 @@
     splits_metric: Optional[List[Split]] = None
     splits_standard: Optional[List[Split]] = None
     photos: Optional[ActivityPhotoMeta] = None
     laps: Optional[List[ActivityLap]] = None
 
     # Added for backward compatibility
     # TODO maybe deprecate?
-    TYPES: ClassVar[Tuple] = get_args(
-        ActivityType.__fields__["__root__"].type_
-    )
-
-    SPORT_TYPES: ClassVar[Tuple] = get_args(
-        SportType.__fields__["__root__"].type_
-    )
+    TYPES: ClassVar[Tuple] = get_args(ActivityType.__fields__['__root__'].type_)
 
     # Undocumented attributes:
     guid: Optional[str] = None
     utc_offset: Optional[float] = None
     location_city: Optional[str] = None
     location_state: Optional[str] = None
     location_country: Optional[str] = None
@@ -774,34 +680,29 @@
     average_cadence: Optional[float] = None
     average_temp: Optional[int] = None
     instagram_primary_photo: Optional[str] = None
     partner_logo_url: Optional[str] = None
     partner_brand_tag: Optional[str] = None
     from_accepted_tag: Optional[bool] = None
     segment_leaderboard_opt_out: Optional[bool] = None
-    perceived_exertion: Optional[int] = None
 
     _field_conversions = {
-        "moving_time": time_interval,
-        "elapsed_time": time_interval,
-        "timezone": timezone,
-        "distance": uh.meters,
-        "total_elevation_gain": uh.meters,
-        "average_speed": uh.meters_per_second,
-        "max_speed": uh.meters_per_second,
-        "type": enum_value,
-        "sport_type": enum_value,
+        'moving_time': time_interval,
+        'elapsed_time': time_interval,
+        'timezone': timezone,
+        'distance': uh.meters,
+        'total_elevation_gain': uh.meters,
+        'average_speed': uh.meters_per_second,
+        'max_speed': uh.meters_per_second,
+        'type': enum_value,
+        'sport_type': enum_value
     }
 
-    _latlng_check = validator(
-        "start_latlng", "end_latlng", allow_reuse=True, pre=True
-    )(check_valid_location)
-    _naive_local = validator("start_date_local", allow_reuse=True)(
-        naive_datetime
-    )
+    _latlng_check = validator('start_latlng', 'end_latlng', allow_reuse=True, pre=True)(check_valid_location)
+    _naive_local = validator('start_date_local', allow_reuse=True)(naive_datetime)
 
     @lazy_property
     def comments(self):
         return self.bound_client.get_activity_comments(self.id)
 
     @lazy_property
     def zones(self):
@@ -819,71 +720,60 @@
 
 
 class DistributionBucket(TimedZoneRange):
     """
     A single distribution bucket object, used for activity zones.
     """
 
-    _field_conversions = {"time": uh.seconds}
+    _field_conversions = {'time': uh.seconds}
 
 
-class BaseActivityZone(
-    ActivityZone,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
-):
+class BaseActivityZone(ActivityZone, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Base class for activity zones.
 
     A collection of :class:`stravalib.model.DistributionBucket` objects.
     """
 
     # field overrides from superclass for type extensions:
     distribution_buckets: Optional[List[DistributionBucket]] = None
 
     # overriding the superclass type: it should also support pace as value
     type: Optional[Literal["heartrate", "power", "pace"]] = None
 
 
-class Stream(
-    BaseStream, BackwardCompatibilityMixin, DeprecatedSerializableMixin
-):
+class Stream(BaseStream, BackwardCompatibilityMixin, DeprecatedSerializableMixin):
     """
     Stream of readings from the activity, effort or segment.
     """
 
     type: Optional[str] = None
 
     # Not using the typed subclasses from the generated model
     # for backward compatibility:
     data: Optional[List[Any]] = None
 
 
-class Route(
-    Route,
-    BackwardCompatibilityMixin,
-    DeprecatedSerializableMixin,
-    BoundClientEntity,
-):
+class Route(Route, BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Represents a Route.
     """
 
     # Superclass field overrides for using extended types
     athlete: Optional[Athlete] = None
     map: Optional[Map] = None
     segments: Optional[List[Segment]]
 
-    _field_conversions = {"distance": uh.meters, "elevation_gain": uh.meters}
+    _field_conversions = {
+        'distance': uh.meters,
+        'elevation_gain': uh.meters
+    }
 
 
-class Subscription(
-    BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity
-):
+class Subscription(BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Represents a Webhook Event Subscription.
     """
 
     OBJECT_TYPE_ACTIVITY: ClassVar[str] = "activity"
     ASPECT_TYPE_CREATE: ClassVar[str] = "create"
     VERIFY_TOKEN_DEFAULT: ClassVar[str] = "STRAVA"
@@ -893,35 +783,31 @@
     object_type: Optional[str] = None
     aspect_type: Optional[str] = None
     callback_url: Optional[str] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
 
 
-class SubscriptionCallback(
-    BackwardCompatibilityMixin, DeprecatedSerializableMixin
-):
+class SubscriptionCallback(BackwardCompatibilityMixin, DeprecatedSerializableMixin):
     """
     Represents a Webhook Event Subscription Callback.
     """
 
     hub_mode: Optional[str] = None
     hub_verify_token: Optional[str] = None
     hub_challenge: Optional[str] = None
 
     class Config:
-        alias_generator = lambda field_name: field_name.replace("hub_", "hub.")
+        alias_generator = lambda field_name: field_name.replace('hub_', 'hub.')
 
     def validate(self, verify_token=Subscription.VERIFY_TOKEN_DEFAULT):
         assert self.hub_verify_token == verify_token
 
 
-class SubscriptionUpdate(
-    BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity
-):
+class SubscriptionUpdate(BackwardCompatibilityMixin, DeprecatedSerializableMixin, BoundClientEntity):
     """
     Represents a Webhook Event Subscription Update.
     """
 
     subscription_id: Optional[int] = None
     owner_id: Optional[int] = None
     object_id: Optional[int] = None
```

### Comparing `stravalib-1.3.0/stravalib/protocol.py` & `stravalib-1.3.0rc0/stravalib/protocol.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/strava_model.py` & `stravalib-1.3.0rc0/stravalib/strava_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,17 +646,15 @@
     """
     Whether the club is private.
     """
     profile_medium: Optional[str] = None
     """
     URL to a 60x60 pixel profile picture.
     """
-    sport_type: Optional[
-        Literal["cycling", "running", "triathlon", "other"]
-    ] = None
+    sport_type: Optional[Literal["cycling", "running", "triathlon", "other"]] = None
     """
     Deprecated. Prefer to use activity_types.
     """
     state: Optional[str] = None
     """
     The club's state or geographical region.
     """
@@ -1040,17 +1038,15 @@
     """
     The segment's average grade, in percents
     """
     climb_category: Optional[conint(ge=0, le=5)] = None
     """
     The category of the climb [0, 5]. Higher is harder ie. 5 is Hors catégorie, 0 is uncategorized in climb_category. If climb_category = 5, climb_category_desc = HC. If climb_category = 2, climb_category_desc = 3.
     """
-    climb_category_desc: Optional[
-        Literal["NC", "4", "3", "2", "1", "HC"]
-    ] = None
+    climb_category_desc: Optional[Literal["NC", "4", "3", "2", "1", "HC"]] = None
     """
     The description for the category of the climb
     """
     distance: Optional[float] = None
     """
     The segment's distance, in meters
     """
```

### Comparing `stravalib-1.3.0/stravalib/tests/__init__.py` & `stravalib-1.3.0rc0/stravalib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/auth_responder.py` & `stravalib-1.3.0rc0/stravalib/tests/auth_responder.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     def serve_forever(self, *args, **kwargs):
         self.listening_event.set()
         return HTTPServer.serve_forever(self, *args, **kwargs)
 
 
 class RequestHandler(BaseHTTPRequestHandler):
     def do_GET(self):
+
         request_path = self.path
 
         parsed_path = urlparse.urlparse(request_path)
 
         client = Client()
 
         if request_path.startswith("/authorization"):
@@ -94,14 +95,15 @@
             self.send_header("Content-type", "text/plain")
             self.send_header(b"Location", bytes(url))
             self.end_headers()
             self.wfile.write(b"Redirect to URL: {}\n".format(url))
 
 
 def main(port, client_id, client_secret):
+
     logging.basicConfig(
         level=logging.INFO, format="%(levelname)-8s %(message)s"
     )
 
     logger = logging.getLogger("auth_responder")
     logger.info("Listening on localhost:%s" % port)
 
@@ -111,14 +113,15 @@
         client_id=client_id,
         client_secret=client_secret,
     )
     server.serve_forever()
 
 
 if __name__ == "__main__":
+
     parser = argparse.ArgumentParser(
         description="Run a local web server to receive authorization responses from Strava."
     )
 
     parser.add_argument(
         "-p",
         "--port",
```

### Comparing `stravalib-1.3.0/stravalib/tests/functional/__init__.py` & `stravalib-1.3.0rc0/stravalib/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/functional/test_client.py` & `stravalib-1.3.0rc0/stravalib/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/functional/test_client_rate_limiter.py` & `stravalib-1.3.0rc0/stravalib/tests/functional/test_client_rate_limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,13 +69,13 @@
         try:
             # waiting until timeout expires
             time.sleep(5)
 
             # this time it should work again
             self.client.get_athlete()
             self.assertTrue("No exception raised")
-        except exc.RateLimitExceeded as e:
+        except (exc.RateLimitExceeded) as e:
             self.fail("limiter raised RateLimitTimeout unexpectedly!")
 
         # continuse other tests with DefaultRateLimiter
         print("setting default rate limiter")
         self.client.protocol.rate_limiter = DefaultRateLimiter()
```

### Comparing `stravalib-1.3.0/stravalib/tests/functional/test_client_write.py` & `stravalib-1.3.0rc0/stravalib/tests/functional/test_client_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def test_create_activity(self):
         """
         Test Client.create_activity simple case.
         """
         now = datetime.now().replace(microsecond=0)
         a = self.client.create_activity(
             "test_create_activity#simple",
-            activity_type="Ride",
+            activity_type='Ride',
             start_date_local=now,
             elapsed_time=timedelta(hours=3, minutes=4, seconds=5),
             distance=uh.miles(15.2),
         )
         print(a)
 
         self.assertIsInstance(a, model.Activity)
@@ -36,15 +36,15 @@
     def test_update_activity(self):
         """
         Test Client.update_activity simple case.
         """
         now = datetime.now().replace(microsecond=0)
         a = self.client.create_activity(
             "test_update_activity#create",
-            activity_type="Ride",
+            activity_type='Ride',
             start_date_local=now,
             elapsed_time=timedelta(hours=3, minutes=4, seconds=5),
             distance=uh.miles(15.2),
         )
 
         self.assertIsInstance(a, model.Activity)
         self.assertEqual("test_update_activity#create", a.name)
```

### Comparing `stravalib-1.3.0/stravalib/tests/functional/test_result_iterator.py` & `stravalib-1.3.0rc0/stravalib/tests/functional/test_result_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         results = list(results)
         self.assertEqual(10, len(results))
 
         # TODO: use a mock here to figure out how many calls are happening under the hood.
 
     def test_empty(self):
         """Test iterating over empty results."""
-
         # Specify two thing that we happen to know will return 0 results
         def pretend_fetcher(page, per_page):
             return []
 
         ri = BatchedResultsIterator(
             entity=model.Shoe, result_fetcher=pretend_fetcher
         )
```

### Comparing `stravalib-1.3.0/stravalib/tests/integration/strava_api_stub.py` & `stravalib-1.3.0rc0/stravalib/tests/integration/strava_api_stub.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/integration/test_client.py` & `stravalib-1.3.0rc0/stravalib/tests/integration/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,75 +42,58 @@
     else:
         activity = client.get_activity(test_activity_id)
     assert mock_strava_api.calls[-1].request.url.endswith(expected_url)
     assert activity.id == test_activity_id
 
 
 def test_get_activity_laps(mock_strava_api, client):
-    mock_strava_api.get(
-        "/activities/{id}/laps",
-        response_update={"distance": 1000},
-        n_results=2,
-    )
+    mock_strava_api.get('/activities/{id}/laps', response_update={'distance': 1000}, n_results=2)
     laps = list(client.get_activity_laps(42))
     assert len(laps) == 2
     assert laps[0].distance == meters(1000)
 
 
 def test_get_club_activities(mock_strava_api, client):
-    mock_strava_api.get(
-        "/clubs/{id}/activities",
-        response_update={"distance": 1000},
-        n_results=2,
-    )
+    mock_strava_api.get('/clubs/{id}/activities', response_update={'distance': 1000}, n_results=2)
     activities = list(client.get_club_activities(42))
     assert len(activities) == 2
     assert activities[0].distance == meters(1000)
 
 
 def test_get_activity_zones(mock_strava_api, client):
     # Unfortunately, there is no example response for this endpoint in swagger.json
-    with open(
-        os.path.join(RESOURCES_DIR, "example_zone_response.json"), "r"
-    ) as zone_response_fp:
+    with open(os.path.join(RESOURCES_DIR, 'example_zone_response.json'), 'r') as zone_response_fp:
         zone_response = json.load(zone_response_fp)
-    mock_strava_api.get("/activities/{id}/zones", json=zone_response)
+    mock_strava_api.get('/activities/{id}/zones', json=zone_response)
     activity_zones = client.get_activity_zones(42)
     assert len(activity_zones) == 2
-    assert activity_zones[0].type == "heartrate"
+    assert activity_zones[0].type == 'heartrate'
     assert activity_zones[0].sensor_based
 
 
 def test_get_activity_streams(mock_strava_api, client):
     # TODO: parameterize test to cover all branching
     mock_strava_api.get(
-        "/activities/{id}/streams", response_update={"data": [1, 2, 3]}
+        '/activities/{id}/streams',
+        response_update={'data': [1, 2, 3]}
     )
     # the example in swagger.json returns a distance stream
     streams = client.get_activity_streams(42)
-    assert streams["distance"].data == [1, 2, 3]
+    assert streams['distance'].data == [1, 2, 3]
 
 
 @pytest.mark.parametrize(
     "update_kwargs,expected_params,expected_warning,expected_exception",
     (
         ({}, {}, None, None),
         ({"name": "foo"}, {"name": "foo"}, None, None),
         ({"activity_type": "foo"}, {}, None, ValueError),
-        ({"activity_type": "Run"}, {"type": "run"}, DeprecationWarning, None),
-        ({"activity_type": "run"}, {"type": "run"}, DeprecationWarning, None),
-        ({"activity_type": "RUN"}, {"type": "run"}, DeprecationWarning, None),
-        ({"sport_type": "foo"}, {}, None, ValueError),
-        ({"sport_type": "TrailRun"}, {"sport_type": "TrailRun"}, None, None),
-        (
-            {"activity_type": "Run", "sport_type": "TrailRun"},
-            {"sport_type": "TrailRun"},
-            DeprecationWarning,
-            None,
-        ),
+        ({"activity_type": "Run"}, {"type": "run"}, None, None),
+        ({"activity_type": "run"}, {"type": "run"}, None, None),
+        ({"activity_type": "RUN"}, {"type": "run"}, None, None),
         ({"private": True}, {"private": "1"}, DeprecationWarning, None),
         ({"commute": True}, {"commute": "1"}, None, None),
         ({"trainer": True}, {"trainer": "1"}, None, None),
         ({"gear_id": "fb42"}, {"gear_id": "fb42"}, None, None),
         ({"description": "foo"}, {"description": "foo"}, None, None),
         (
             {"device_name": "foo"},
@@ -387,71 +370,55 @@
         assert uploader.is_processing
         activity = uploader.wait()
         assert uploader.is_complete
         assert activity.id == test_activity_id
 
 
 def test_get_route(mock_strava_api, client):
-    with open(
-        os.path.join(RESOURCES_DIR, "example_route_response.json"), "r"
-    ) as route_response_fp:
+    with open(os.path.join(RESOURCES_DIR, 'example_route_response.json'), 'r') as route_response_fp:
         route_response = json.load(route_response_fp)
-    mock_strava_api.get("/routes/{id}", status=200, json=route_response)
+    mock_strava_api.get(
+        "/routes/{id}", status=200, json=route_response
+    )
     route = client.get_route(42)
     assert route.name == "15k, no traffic"
 
 
 @responses.activate
 def test_create_subscription(mock_strava_api, client):
     responses.post(
-        "https://www.strava.com/api/v3/push_subscriptions",
+        'https://www.strava.com/api/v3/push_subscriptions',
         json={
-            "application_id": 42,
-            "object_type": "activity",
-            "aspect_type": "create",
-            "callback_url": "https://foobar.com",
-            "created_at": 1674660406,
+            'application_id': 42,
+            'object_type': 'activity',
+            'aspect_type': 'create',
+            'callback_url': 'https://foobar.com',
+            'created_at': 1674660406
         },
-        status=200,
-    )
-    created_subscription = client.create_subscription(
-        42, 42, "https://foobar.com"
+        status=200
     )
+    created_subscription = client.create_subscription(42, 42, 'https://foobar.com')
     assert created_subscription.application_id == 42
 
 
 @pytest.mark.parametrize(
-    "raw,expected_verify_token,expected_response,expected_exception",
+    'raw,expected_verify_token,expected_response,expected_exception',
     (
-        (
-            {"hub.verify_token": "a", "hub.challenge": "b"},
-            "a",
-            {"hub.challenge": "b"},
-            None,
-        ),
-        (
-            {"hub.verify_token": "foo", "hub.challenge": "b"},
-            "a",
-            None,
-            AssertionError,
-        ),
-    ),
+        ({'hub.verify_token': 'a', 'hub.challenge': 'b'}, 'a', {'hub.challenge': 'b'}, None),
+        ({'hub.verify_token': 'foo', 'hub.challenge': 'b'}, 'a', None, AssertionError),
+    )
 )
 def test_handle_subscription_callback(
-    client, raw, expected_verify_token, expected_response, expected_exception
+        client, raw, expected_verify_token, expected_response, expected_exception
 ):
     if expected_exception:
         with pytest.raises(expected_exception):
             client.handle_subscription_callback(raw, expected_verify_token)
     else:
-        assert (
-            client.handle_subscription_callback(raw, expected_verify_token)
-            == expected_response
-        )
-
+        assert client.handle_subscription_callback(raw, expected_verify_token) == expected_response
 
 @pytest.mark.parametrize(
     "limit,n_raw_results,expected_n_segments",
     (
         (None, 0, 0),
         (None, 10, 10),
         (10, 10, 10),
@@ -488,25 +455,23 @@
     )
     clubs = client.get_athlete_clubs()
     assert len(clubs) == n_clubs
     if clubs:
         assert clubs[0].name == "foo"
 
 
-@pytest.mark.parametrize("n_members", (0, 2))
+@pytest.mark.parametrize('n_members', (0, 2))
 def test_get_club_members(mock_strava_api, client, n_members):
     mock_strava_api.get(
-        "/clubs/{id}/members",
-        response_update={"lastname": "Doe"},
-        n_results=n_members,
+        '/clubs/{id}/members', response_update={'lastname': 'Doe'}, n_results=n_members
     )
     members = list(client.get_club_members(42))
     assert len(members) == n_members
     if members:
-        assert members[0].lastname == "Doe"
+        assert members[0].lastname == 'Doe'
 
 
 @pytest.mark.parametrize(
     "athlete_id,authenticated_athlete,expected_biggest_ride_distance,expected_exception",
     (
         (42, True, 1000, None),
         (42, False, None, AccessUnauthorized),
@@ -581,35 +546,33 @@
     assert len(activity_list) == expected_n_activities
     if expected_n_activities > 0:
         assert activity_list[0].name == "test_activity"
 
 
 def test_get_activities_quantity_addition(mock_strava_api, client):
     mock_strava_api.get(
-        "/athlete/activities",
-        response_update={"distance": 1000.0},
-        n_results=2,
+        '/athlete/activities',
+        response_update={'distance': 1000.0},
+        n_results=2
     )
     act_list = list(client.get_activities(limit=2))
     total_d = uh.meters(0)
     total_d += act_list[0].distance
     total_d += act_list[1].distance
-    assert total_d == uh.meters(2000.0)
+    assert total_d == uh.meters(2000.)
 
 
 def test_get_segment(mock_strava_api, client):
-    mock_strava_api.get("/segments/{id}", response_update={"name": "foo"})
+    mock_strava_api.get('/segments/{id}', response_update={'name': 'foo'})
     segment = client.get_segment(42)
-    assert segment.name == "foo"
+    assert segment.name == 'foo'
 
 
 def test_get_segment_effort(mock_strava_api, client):
-    mock_strava_api.get(
-        "/segment_efforts/{id}", response_update={"max_heartrate": 170}
-    )
+    mock_strava_api.get('/segment_efforts/{id}', response_update={'max_heartrate': 170})
     effort = client.get_segment_effort(42)
     assert effort.max_heartrate == 170
 
 
 def test_get_activities_paged(mock_strava_api, client):
     for i in range(1, 4):
         params = {"page": i, "per_page": 200}
@@ -624,118 +587,104 @@
     assert activity_list[0].id == 1
     assert activity_list[400].id == 3
 
 
 @responses.activate
 def test_upload_activity_photo_works(client):
     """
-    Test uploading an activity with a photo.
+        Test uploading an activity with a photo.
 
-    """
+        """
 
-    strava_pre_signed_uri = "https://strava-photo-uploads-prod.s3-accelerate.amazonaws.com/12345.jpg"
-    photo_bytes = b"photo_data"
+    strava_pre_signed_uri = 'https://strava-photo-uploads-prod.s3-accelerate.amazonaws.com/12345.jpg'
+    photo_bytes = b'photo_data'
     photo_metadata_header = {
         "Content-Type": "image/jpeg",
-        "Expect": "100-continue",
-        "Host": "strava-photo-uploads-prod.s3-accelerate.amazonaws.com",
+        "Expect": '100-continue',
+        'Host': 'strava-photo-uploads-prod.s3-accelerate.amazonaws.com',
     }
     activity_upload_response = {
         "id": 12345,
         "external_id": "external_id",
         "error": None,
         "status": "Your activity is ready.",
         "activity_id": 12345,
-        "photo_metadata": [
-            {
-                "uri": strava_pre_signed_uri,
-                "header": photo_metadata_header,
-                "method": "PUT",
-                "max_size": 1600,
-            }
-        ],
+        "photo_metadata": [{
+            "uri": strava_pre_signed_uri,
+            "header": photo_metadata_header,
+            "method": "PUT",
+            "max_size": 1600,
+        }]
     }
-    with responses.RequestsMock(
-        assert_all_requests_are_fired=True
-    ) as _responses:
+    with responses.RequestsMock(assert_all_requests_are_fired=True) as _responses:
         _responses.add(
             responses.PUT,
             "https://strava-photo-uploads-prod.s3-accelerate.amazonaws.com/12345.jpg",
             status=200,
         )
 
         _responses.add(
             responses.GET,
             "https://www.strava.com/api/v3/uploads/12345",
             status=200,
-            json=activity_upload_response,
+            json=activity_upload_response
         )
 
-        activity_uploader = ActivityUploader(
-            client, response=activity_upload_response
-        )
+        activity_uploader = ActivityUploader(client, response=activity_upload_response)
 
         activity_uploader.upload_photo(photo=photo_bytes)
 
 
 def test_upload_activity_photo_fail_type_error(client):
     activity_uploader = ActivityUploader(client, response={})
 
     with pytest.raises(ActivityPhotoUploadFailed) as error:
-        activity_uploader.upload_photo(photo="photo_str")
+        activity_uploader.upload_photo(photo='photo_str')
 
-    assert str(error.value) == "Photo must be bytes type"
+    assert str(error.value) == 'Photo must be bytes type'
 
 
-@mock.patch("stravalib.client.ActivityUploader.poll")
+@mock.patch('stravalib.client.ActivityUploader.poll')
 def test_upload_activity_photo_fail_activity_upload_not_complete(client):
     activity_upload_response = {
         "id": 1234578,
         "external_id": "external_id",
         "error": None,
         "status": "Your activity is being processed.",
     }
-    activity_uploader = ActivityUploader(
-        client, response=activity_upload_response
-    )
+    activity_uploader = ActivityUploader(client, response=activity_upload_response)
 
     with pytest.raises(ActivityPhotoUploadFailed) as error:
-        activity_uploader.upload_photo(photo=b"photo_bytes")
+        activity_uploader.upload_photo(photo=b'photo_bytes')
 
-    assert str(error.value) == "Activity upload not complete"
+    assert str(error.value) == 'Activity upload not complete'
 
 
-@pytest.mark.parametrize(
-    "photo_metadata",
-    (
+@pytest.mark.parametrize('photo_metadata', (
         None,
         [],
         [{}],
-    ),
-)
-@mock.patch("stravalib.client.ActivityUploader.poll")
+))
+@mock.patch('stravalib.client.ActivityUploader.poll')
 def test_upload_activity_photo_fail_not_supported(client, photo_metadata):
     activity_upload_response = {
         "id": 1234578,
         "external_id": "external_id",
         "error": None,
         "status": "Your activity is ready.",
         "activity_id": 1234578,
-        "photo_metadata": photo_metadata,
+        "photo_metadata": photo_metadata
     }
 
-    activity_uploader = ActivityUploader(
-        client, response=activity_upload_response
-    )
+    activity_uploader = ActivityUploader(client, response=activity_upload_response)
 
     with pytest.raises(ActivityPhotoUploadFailed) as error:
-        activity_uploader.upload_photo(photo=b"photo_bytes")
-
-    assert str(error.value) == "Photo upload not supported"
+        activity_uploader.upload_photo(photo=b'photo_bytes')
 
+    assert str(error.value) == 'Photo upload not supported'
 
 def test_get_activity_comments(mock_strava_api, client):
     mock_strava_api.get(
         "/activities/{id}/comments",
         response_update={"text": "foo"},
         n_results=2,
     )
@@ -746,47 +695,39 @@
     assert comment_list[0].text == "foo"
 
 
 def test_explore_segments(mock_strava_api, client):
     # TODO parameterize test with multiple inputs
     # It is hard to patch the response for this one, since the
     # endpoint returns a nested list of segments.
-    mock_strava_api.get("/segments/explore")
+    mock_strava_api.get('/segments/explore')
     segment_list = client.explore_segments((1, 2, 3, 4))
     assert len(segment_list) == 1
-    assert segment_list[0].name == "Hawk Hill"
-
+    assert segment_list[0].name == 'Hawk Hill'
 
 def test_get_activity_kudos(mock_strava_api, client):
     mock_strava_api.get(
         "/activities/{id}/kudos",
         response_update={"lastname": "Doe"},
         n_results=2,
     )
     kudoer_list = list(client.get_activity_kudos(42))
     assert len(kudoer_list) == 2
     assert kudoer_list[0].lastname == "Doe"
 
 
 class TestIsAuthenticatedAthlete:
     def test_default(self, mock_strava_api, client):
-        mock_strava_api.get("/athlete", response_update={"id": 42})
+        mock_strava_api.get('/athlete', response_update={'id': 42})
         athlete = client.get_athlete()
         assert athlete.is_authenticated_athlete()
 
     def test_caching(self):
         athlete = Athlete(is_authenticated=True)
         assert athlete.is_authenticated_athlete()
 
-    @pytest.mark.parametrize(
-        "match_id,expected_result", ((False, False), (True, True))
-    )
-    def test_from_summary(
-        self, mock_strava_api, client, match_id, expected_result
-    ):
-        mock_strava_api.get(
-            "/clubs/{id}/members",
-            response_update={"id": 42 if match_id else 21},
-        )
-        mock_strava_api.get("/athlete", response_update={"id": 42})
+    @pytest.mark.parametrize('match_id,expected_result', ((False, False), (True, True)))
+    def test_from_summary(self, mock_strava_api, client, match_id, expected_result):
+        mock_strava_api.get('/clubs/{id}/members', response_update={'id': 42 if match_id else 21})
+        mock_strava_api.get('/athlete', response_update={'id': 42})
         club_members = list(client.get_club_members(99))
         assert club_members[0].is_authenticated_athlete() == expected_result
```

### Comparing `stravalib-1.3.0/stravalib/tests/resources/activity-manual.3.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/activity-manual.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/activity.3.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/activity.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/athlete.2.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/athlete.2.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/athlete.3.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/athlete.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/example_route_response.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/example_route_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/example_zone_response.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/example_zone_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/sample.tcx` & `stravalib-1.3.0rc0/stravalib/tests/resources/sample.tcx`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/resources/strava_swagger.json` & `stravalib-1.3.0rc0/stravalib/tests/resources/strava_swagger.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/unit/test_client_utils.py` & `stravalib-1.3.0rc0/stravalib/tests/unit/test_client_utils.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/unit/test_field_conversions.py` & `stravalib-1.3.0rc0/stravalib/tests/unit/test_field_conversions.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,27 +16,25 @@
         return x + 1
 
     assert foo(1) == 2
     assert foo(None) is None
 
 
 def test_enum_value():
-    assert enum_value(ActivityType(__root__="Run")) == "Run"
+    assert enum_value(ActivityType(__root__='Run')) == 'Run'
 
 
 def test_enum_values():
-    assert enum_values(
-        [ActivityType(__root__="Run"), SportType(__root__="Ride")]
-    ) == ["Run", "Ride"]
+    assert enum_values([ActivityType(__root__='Run'), SportType(__root__='Ride')]) == ["Run", "Ride"]
 
 
 @pytest.mark.parametrize(
-    "arg,expected_value",
+    'arg,expected_value',
     (
-        ("Factory", None),
-        ("(GMT+00:00) Factory", None),
-        ("Europe/Amsterdam", pytz.timezone("Europe/Amsterdam")),
-        ("(GMT+01:00) Europe/Amsterdam", pytz.timezone("Europe/Amsterdam")),
-    ),
+        ('Factory', None),
+        ('(GMT+00:00) Factory', None),
+        ('Europe/Amsterdam', pytz.timezone('Europe/Amsterdam')),
+        ('(GMT+01:00) Europe/Amsterdam', pytz.timezone('Europe/Amsterdam'))
+    )
 )
 def test_timezone(arg, expected_value):
     assert timezone(arg) == expected_value
```

### Comparing `stravalib-1.3.0/stravalib/tests/unit/test_limiter.py` & `stravalib-1.3.0rc0/stravalib/tests/unit/test_limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib/tests/unit/test_model.py` & `stravalib-1.3.0rc0/stravalib/tests/unit/test_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,179 +54,134 @@
         (Club, {"name": "foo"}, "foo"),
         (ActivityTotals, {"elapsed_time": 100}, timedelta(seconds=100)),
         (
             ActivityTotals,
             {"distance": 100.0},
             UnitConverter("meters")(100.0),
         ),
-        (
-            Activity,
-            {"timezone": "Europe/Amsterdam"},
-            pytz.timezone("Europe/Amsterdam"),
-        ),
-        (Club, {"activity_types": ["Run", "Ride"]}, ["Run", "Ride"]),
-        (Activity, {"sport_type": "Run"}, "Run"),
+        (Activity, {'timezone': 'Europe/Amsterdam'}, pytz.timezone('Europe/Amsterdam')),
+        (Club, {'activity_types': ['Run', 'Ride']}, ['Run', 'Ride']),
+        (Activity, {'sport_type': 'Run'}, 'Run')
     ),
 )
 def test_backward_compatibility_mixin_field_conversions(
     model_class, raw, expected_value
 ):
     obj = model_class.parse_obj(raw)
     assert getattr(obj, list(raw.keys())[0]) == expected_value
 
 
 @pytest.mark.parametrize(
-    "model_class,raw,expected_value",
+    'model_class,raw,expected_value',
     (
-        (Activity, {"start_latlng": "5.4,4.3"}, LatLon(__root__=[5.4, 4.3])),
-        (Activity, {"start_latlng": []}, None),
-        (Segment, {"start_latlng": []}, None),
-        (SegmentExplorerResult, {"start_latlng": []}, None),
-        (ActivityPhoto, {"location": []}, None),
-        (Activity, {"timezone": "foobar"}, None),
-        (
-            Activity,
-            {"start_date_local": "2023-01-17T11:06:07Z"},
-            datetime(2023, 1, 17, 11, 6, 7),
-        ),
-        (
-            BaseEffort,
-            {"start_date_local": "2023-01-17T11:06:07Z"},
-            datetime(2023, 1, 17, 11, 6, 7),
-        ),
-        (
-            ActivityLap,
-            {"start_date_local": "2023-01-17T11:06:07Z"},
-            datetime(2023, 1, 17, 11, 6, 7),
-        ),
-    ),
+        (Activity, {'start_latlng': "5.4,4.3"}, LatLon(__root__=[5.4, 4.3])),
+        (Activity, {'start_latlng': []}, None),
+        (Segment, {'start_latlng': []}, None),
+        (SegmentExplorerResult, {'start_latlng': []}, None),
+        (ActivityPhoto, {'location': []}, None),
+        (Activity, {'timezone': 'foobar'}, None),
+        (Activity, {'start_date_local': '2023-01-17T11:06:07Z'}, datetime(2023, 1, 17, 11, 6, 7)),
+        (BaseEffort, {'start_date_local': '2023-01-17T11:06:07Z'}, datetime(2023, 1, 17, 11, 6, 7)),
+        (ActivityLap, {'start_date_local': '2023-01-17T11:06:07Z'}, datetime(2023, 1, 17, 11, 6, 7))
+    )
 )
 def test_deserialization_edge_cases(model_class, raw, expected_value):
     obj = model_class.parse_obj(raw)
     assert getattr(obj, list(raw.keys())[0]) == expected_value
 
 
 def test_subscription_callback_field_names():
     sub_callback_raw = {
         "hub.mode": "subscribe",
         "hub.verify_token": "STRAVA",
         "hub.challenge": "15f7d1a91c1f40f8a748fd134752feb3",
     }
     sub_callback = SubscriptionCallback.parse_obj(sub_callback_raw)
-    assert sub_callback.hub_mode == "subscribe"
-    assert sub_callback.hub_verify_token == "STRAVA"
+    assert sub_callback.hub_mode == 'subscribe'
+    assert sub_callback.hub_verify_token == 'STRAVA'
 
 
 # Below are some toy classes to test type extensions and attribute lookup:
 class A(BaseModel, BackwardCompatibilityMixin):
     x: Optional[int] = None
 
 
 class ConversionA(A, BackwardCompatibilityMixin):
-    _field_conversions = {"x": uh.meters}
+    _field_conversions = {'x': uh.meters}
 
 
 class BoundA(A, BoundClientEntity):
     pass
 
-
 class B(BaseModel, BackwardCompatibilityMixin):
     a: Optional[A] = None
     bound_a: Optional[BoundA] = None
 
 
 class BoundB(B, BoundClientEntity):
     pass
 
-
 class C(BaseModel, BackwardCompatibilityMixin):
     a: Optional[List[A]] = None
     bound_a: Optional[List[BoundA]] = None
 
 
 class BoundC(C, BoundClientEntity):
     pass
 
 
 class D(BaseModel, BackwardCompatibilityMixin):
     a: Optional[LatLng] = None
 
-
 class ExtA(A):
     def foo(self):
         return self.x
 
 
 class ExtLatLng(LatLng):
     def foo(self):
-        return f"[{self[0], self[1]}]"
+        return f'[{self[0], self[1]}]'
 
 
 @pytest.mark.parametrize(
-    "lookup_expression,expected_result,expected_bound_client",
+    'lookup_expression,expected_result,expected_bound_client',
     (
         (A().x, None, False),
         (B().a, None, False),
         (A(x=1).x, 1, False),
         (B(a=A(x=1)).a, A(x=1), False),
         (C(a=[A(x=1), A(x=2)]).a[1], A(x=2), False),
-        (ConversionA(x=1).x, pint.Quantity("1 meter"), False),
+        (ConversionA(x=1).x, pint.Quantity('1 meter'), False),
         (BoundA(x=1).x, 1, False),
         (B(bound_a=BoundA(x=1)).bound_a, BoundA(x=1), None),
-        (
-            B(bound_a=BoundA(x=1, bound_client=1)).bound_a,
-            BoundA(x=1, bound_client=1),
-            True,
-        ),
+        (B(bound_a=BoundA(x=1, bound_client=1)).bound_a, BoundA(x=1, bound_client=1), True),
         (BoundB(a=A(x=1)).a, A(x=1), False),
         (BoundB(a=A(x=1), bound_client=1).a, A(x=1), False),
         (BoundB(bound_a=BoundA(x=1)).bound_a, BoundA(x=1), None),
-        (
-            BoundB(bound_a=BoundA(x=1), bound_client=1).bound_a,
-            BoundA(x=1, bound_client=1),
-            True,
-        ),
+        (BoundB(bound_a=BoundA(x=1), bound_client=1).bound_a, BoundA(x=1, bound_client=1), True),
         (C(bound_a=[BoundA(x=1), BoundA(x=2)]).bound_a[1], BoundA(x=2), None),
-        (
-            C(
-                bound_a=[
-                    BoundA(x=1, bound_client=1),
-                    BoundA(x=2, bound_client=1),
-                ]
-            ).bound_a[1],
-            BoundA(x=2, bound_client=1),
-            True,
-        ),
+        (C(bound_a=[BoundA(x=1, bound_client=1), BoundA(x=2, bound_client=1)]).bound_a[1],
+         BoundA(x=2, bound_client=1), True),
         (BoundC(a=[A(x=1), A(x=2)]).a[1], A(x=2), False),
         (BoundC(a=[A(x=1), A(x=2)], bound_client=1).a[1], A(x=2), False),
-        (
-            BoundC(bound_a=[BoundA(x=1), BoundA(x=2)]).bound_a[1],
-            BoundA(x=2),
-            None,
-        ),
-        (
-            BoundC(bound_a=[BoundA(x=1), BoundA(x=2)], bound_client=1).bound_a[
-                1
-            ],
-            BoundA(x=2, bound_client=1),
-            True,
-        ),
-    ),
+        (BoundC(bound_a=[BoundA(x=1), BoundA(x=2)]).bound_a[1],
+         BoundA(x=2), None),
+        (BoundC(bound_a=[BoundA(x=1), BoundA(x=2)], bound_client=1).bound_a[1],
+         BoundA(x=2, bound_client=1), True)
+    )
 )
-def test_backward_compatible_attribute_lookup(
-    lookup_expression, expected_result, expected_bound_client
-):
+def test_backward_compatible_attribute_lookup(lookup_expression, expected_result, expected_bound_client):
     assert lookup_expression == expected_result
 
     if expected_bound_client:
         assert lookup_expression.bound_client is not None
     elif expected_bound_client is None:
         assert lookup_expression.bound_client is None
     elif not expected_bound_client:
-        assert not hasattr(lookup_expression, "bound_client")
+        assert not hasattr(lookup_expression, 'bound_client')
 
 
 class ModelTest(TestBase):
     def setUp(self):
         super(ModelTest, self).setUp()
 
     def test_entity_collections(self):
```

### Comparing `stravalib-1.3.0/stravalib/tests/unit/test_unithelper.py` & `stravalib-1.3.0rc0/stravalib/tests/unit/test_unithelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,15 @@
             assert uh.is_quantity_type(obj) == expected_result
     else:
         assert uh.is_quantity_type(obj) == expected_result
 
 
 def test_legacy_accessors():
     assert uh.meters(10).num == 10
-    assert uh.meters(10).unit == "meter"
-
+    assert uh.meters(10).unit == 'meter'
 
 def test_arithmetic_comparison_support():
     assert int(uh.meters(2.1)) == 2
     assert float(uh.meters(2.1)) == 2.1
     assert uh.meters(2) == uh.meters(2)
     assert uh.meters(2) > uh.meters(1)
     assert uh.meters(2) + uh.meters(1) == uh.meters(3)
```

### Comparing `stravalib-1.3.0/stravalib/unithelper.py` & `stravalib-1.3.0rc0/stravalib/unithelper.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,26 +72,26 @@
     elif isinstance(obj, UnitsQuantity):  # check using Duck Typing
         warn_units_deprecated()
         return True
     else:
         return False
 
 
-meter = meters = UnitConverter("m")
-second = seconds = UnitConverter("s")
-hour = hours = UnitConverter("hour")
-foot = feet = UnitConverter("ft")
-mile = miles = UnitConverter("mi")
-kilometer = kilometers = UnitConverter("km")
-
-meters_per_second = UnitConverter("m/s")
-miles_per_hour = mph = UnitConverter("mi/hour")
-kilometers_per_hour = kph = UnitConverter("km/hour")
-kilogram = kilograms = kg = kgs = UnitConverter("kg")
-pound = pounds = lb = lbs = UnitConverter("lb")
+meter = meters = UnitConverter('m')
+second = seconds = UnitConverter('s')
+hour = hours = UnitConverter('hour')
+foot = feet = UnitConverter('ft')
+mile = miles = UnitConverter('mi')
+kilometer = kilometers = UnitConverter('km')
+
+meters_per_second = UnitConverter('m/s')
+miles_per_hour = mph = UnitConverter('mi/hour')
+kilometers_per_hour = kph = UnitConverter('km/hour')
+kilogram = kilograms = kg = kgs = UnitConverter('kg')
+pound = pounds = lb = lbs = UnitConverter('lb')
 
 
 def c2f(celsius):
     """
     Convert Celsius to Fahrenheit.
 
     Parameters
```

### Comparing `stravalib-1.3.0/stravalib/util/limiter.py` & `stravalib-1.3.0rc0/stravalib/util/limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.0/stravalib.egg-info/PKG-INFO` & `stravalib-1.3.0rc0/stravalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stravalib
-Version: 1.3.0
+Version: 1.3.0rc0
 Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
 Author-email: Hans Lellelid <hans@xmpl.org>
 Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong
 License: Apache 2.0 License
 Project-URL: homepage, https://example.com
 Project-URL: documentation, https://stravalib.readthedocs.io
 Project-URL: repository, https://github.com/stravalib/stravalib
```

### Comparing `stravalib-1.3.0/stravalib.egg-info/SOURCES.txt` & `stravalib-1.3.0rc0/stravalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

