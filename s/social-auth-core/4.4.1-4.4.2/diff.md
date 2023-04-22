# Comparing `tmp/social-auth-core-4.4.1.tar.gz` & `tmp/social-auth-core-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social-auth-core-4.4.1.tar", last modified: Thu Mar 30 10:59:43 2023, max compression
+gzip compressed data, was "social-auth-core-4.4.2.tar", last modified: Sat Apr 22 05:49:06 2023, max compression
```

## Comparing `social-auth-core-4.4.1.tar` & `social-auth-core-4.4.2.tar`

### file list

```diff
@@ -1,361 +1,363 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.344359 social-auth-core-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-30 10:59:43.344359 social-auth-core-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/requirements-azuread.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/requirements-base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/requirements-openidconnect.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/requirements-saml.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-30 10:59:43.344359 social-auth-core-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.316358 social-auth-core-4.4.1/social_auth_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-30 10:59:43.000000 social-auth-core-4.4.1/social_auth_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-03-30 10:59:43.000000 social-auth-core-4.4.1/social_auth_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:59:43.000000 social-auth-core-4.4.1/social_auth_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:59:43.000000 social-auth-core-4.4.1/social_auth_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-30 10:59:43.000000 social-auth-core-4.4.1/social_auth_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 10:59:43.000000 social-auth-core-4.4.1/social_auth_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.316358 social-auth-core-4.4.1/social_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.332358 social-auth-core-4.4.1/social_core/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/amazon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/angel.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/aol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/apple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/appsfuel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/asana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/atlassian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/azuread_b2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/azuread_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/battlenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/beats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/behance.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/belgiumeid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/box.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/bungie.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/changetip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/chatwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/cilogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/classlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/clef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/coursera.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/deezer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/discourse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/disqus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/douban.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/dribbble.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/drip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/echosign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/edmodo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/elixir.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/eventbrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/eveonline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/evernote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/exacttarget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/facebook_limited.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/fedora.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/fence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/fitbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/five_hundred_px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/flickr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/foursquare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/gae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/gitea.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/github_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/goclio.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/goclioeu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/google_openidconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/hubspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/itembase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/jawbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/justgiving.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/kakao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/khanacademy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/lastfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/launchpad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/linkedin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/livejournal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/loginradius.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/lyft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mailru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mapmyfitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/meetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mendeley.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/microsoft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mineid.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/monzo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/moves.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/musicbrainz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/nationbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/naver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/ngpvan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/nk.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/odnoklassniki.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/okta.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/okta_openidconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/open_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/open_id_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/openinfra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/openshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/openstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/openstreetmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/orbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/orcid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/osso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/patreon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/paypal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/persona.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/phabricator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/pinterest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/pixelpin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/podio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/professionali.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/qiita.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/qq.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/quizlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/rdio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/readability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/runkeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/scistarter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/seznam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/shimmering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/shopify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/simplelogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/sketchfab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/skyrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/stackoverflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/stocktwits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/strava.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/surveymonkey.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/suse.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/taobao.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/thisismyjam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/trello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/tripit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/tumblr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/twilio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/uber.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/ubuntu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/udata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/universe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/untappd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/upwork.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/vend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/weibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/weixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/withings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/wunderlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/xing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/yahoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/yammer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/backends/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.332358 social-auth-core-4.4.1/social_core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/social_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.332358 social-auth-core-4.4.1/social_core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.332358 social-auth-core-4.4.1/social_core/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/actions/test_associate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/actions/test_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/actions/test_login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.344359 social-auth-core-4.4.1/social_core/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:59:43.344359 social-auth-core-4.4.1/social_core/tests/backends/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/data/saml_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/data/saml_response.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/open_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_amazon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_angel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_apple.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_arcgis.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_asana.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_atlassian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_auth0.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_azuread_b2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_behance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_broken.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_chatwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_cilogon.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_clef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_coursera.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_deezer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_digitalocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_discourse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_disqus.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_dribbble.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_drip.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_edmodo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_elixir.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_eventbrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_evernote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_fence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_fitbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_five_hundred_px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_flickr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_foursquare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_gitea.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_github_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_google.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_itembase.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_kakao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_khanacademy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_linkedin.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_livejournal.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_lyft.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_mailru.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_mapmyfitness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_microsoft.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_mineid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_musicbrainz.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_nationbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_naver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_ngpvan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_open_id_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_orbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_orcid.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_osso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_patreon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_paypal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_phabricator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_pinterest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_podio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_qiita.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_quizlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_readability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_scistarter.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_seznam.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_simplelogin.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_sketchfab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_skyrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_soundcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_stackoverflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_stocktwits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_strava.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_taobao.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_thisismyjam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_tripit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_tumblr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_twitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_uber.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_udata.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_universe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_upwork.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_wunderlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_xing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_yahoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_yammer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_yandex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/backends/test_zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/tests/testkey.pem
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-03-30 10:59:34.000000 social-auth-core-4.4.1/social_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.858191 social-auth-core-4.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-22 05:49:06.858191 social-auth-core-4.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/requirements-azuread.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/requirements-base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/requirements-openidconnect.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/requirements-saml.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-22 05:49:06.858191 social-auth-core-4.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.826191 social-auth-core-4.4.2/social_auth_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-22 05:49:06.000000 social-auth-core-4.4.2/social_auth_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-04-22 05:49:06.000000 social-auth-core-4.4.2/social_auth_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:49:06.000000 social-auth-core-4.4.2/social_auth_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 05:49:06.000000 social-auth-core-4.4.2/social_auth_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-22 05:49:06.000000 social-auth-core-4.4.2/social_auth_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 05:49:06.000000 social-auth-core-4.4.2/social_auth_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.826191 social-auth-core-4.4.2/social_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.842191 social-auth-core-4.4.2/social_core/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/amazon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/angel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/aol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/apple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/appsfuel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/asana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/atlassian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/azuread_b2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/azuread_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/battlenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/beats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/behance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/belgiumeid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/bungie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/changetip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/chatwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/classlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/clef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/coursera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/deezer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/discourse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/disqus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/douban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/dribbble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/drip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/echosign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/edmodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/elixir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/eventbrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/eveonline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/evernote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/exacttarget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/facebook_limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/fedora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/fence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/five_hundred_px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/flickr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/foursquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/gae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/gitea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/github_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/goclio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/goclioeu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/google_openidconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/hubspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/itembase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/jawbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/justgiving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/kakao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/khanacademy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/lastfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/launchpad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/livejournal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/loginradius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/lyft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mailru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mapmyfitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/meetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mendeley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mineid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/monzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/moves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/musicbrainz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/nationbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/naver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/ngpvan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/odnoklassniki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/okta_openidconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/open_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/open_id_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/openinfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/openstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/openstreetmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/orbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/osso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/patreon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/paypal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/persona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/phabricator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/pinterest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/pixelpin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/podio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/professionali.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/qiita.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/quizlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/rdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/readability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/runkeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/scistarter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/seznam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/shimmering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/shopify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/simplelogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/sketchfab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/skyrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/stackoverflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/stocktwits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/strava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/surveymonkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/suse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/taobao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/thisismyjam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/trello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/tripit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/tumblr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/uber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/ubuntu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/udata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/universe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/untappd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/upwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/vend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/weibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/weixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/withings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/wunderlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/xing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/yammer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/backends/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.842191 social-auth-core-4.4.2/social_core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/social_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.842191 social-auth-core-4.4.2/social_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.842191 social-auth-core-4.4.2/social_core/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/actions/test_associate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/actions/test_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/actions/test_login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.854191 social-auth-core-4.4.2/social_core/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 05:49:06.858191 social-auth-core-4.4.2/social_core/tests/backends/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/data/saml_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17495 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/data/saml_response.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/open_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_amazon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_angel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_apple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_arcgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_asana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_atlassian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_azuread_b2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_behance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_broken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_chatwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_clef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_coursera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_deezer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_digitalocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_discourse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_disqus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_dribbble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_drip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_edmodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_elixir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_eventbrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_evernote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_fence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_fitbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_five_hundred_px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_flickr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_foursquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_gitea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_github_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_itembase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_kakao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_khanacademy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_linkedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_livejournal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_lyft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_mailru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_mapmyfitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_mineid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_musicbrainz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_nationbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_naver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_ngpvan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_open_id_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_orbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_orcid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_osso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_patreon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_paypal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_phabricator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_pinterest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_podio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_qiita.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_quizlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_readability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_scistarter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_seznam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_simplelogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_sketchfab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_skyrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_soundcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_stackoverflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_stocktwits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_strava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_taobao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_thisismyjam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_tripit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_tumblr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_uber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_udata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_universe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_upwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_wunderlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_xing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_yahoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_yammer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_yandex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/backends/test_zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/tests/testkey.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-22 05:48:55.000000 social-auth-core-4.4.2/social_core/utils.py
```

### Comparing `social-auth-core-4.4.1/CHANGELOG.md` & `social-auth-core-4.4.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [4.4.2](https://github.com/python-social-auth/social-core/releases/tag/4.4.2) - 2023-43-22
+
+### Changed
+- Fixed Azure AD Tenant authentication with custom signing keys
+- Added CAS OIDC backend
+
 ## [4.4.1](https://github.com/python-social-auth/social-core/releases/tag/4.4.1) - 2023-03-30
 
 ### Changed
 - Moved Facebook Limited Login to a separate module to avoid extra dependency
 - Update Azure AD B2C base URL to match updated endpoints
 
 ## [4.4.0](https://github.com/python-social-auth/social-core/releases/tag/4.4.0) - 2023-03-15
```

### Comparing `social-auth-core-4.4.1/LICENSE` & `social-auth-core-4.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/PKG-INFO` & `social-auth-core-4.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-core
-Version: 4.4.1
+Version: 4.4.2
 Summary: Python social authentication made simple.
 Home-page: https://github.com/python-social-auth/social-core
 Author: Matias Aguirre
 Author-email: matiasaguirre@gmail.com
 License: BSD
 Keywords: openid,oauth,saml,social auth
 Platform: UNKNOWN
```

### Comparing `social-auth-core-4.4.1/README.md` & `social-auth-core-4.4.2/README.md`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/setup.py` & `social-auth-core-4.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_auth_core.egg-info/PKG-INFO` & `social-auth-core-4.4.2/social_auth_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-core
-Version: 4.4.1
+Version: 4.4.2
 Summary: Python social authentication made simple.
 Home-page: https://github.com/python-social-auth/social-core
 Author: Matias Aguirre
 Author-email: matiasaguirre@gmail.com
 License: BSD
 Keywords: openid,oauth,saml,social auth
 Platform: UNKNOWN
```

### Comparing `social-auth-core-4.4.1/social_auth_core.egg-info/SOURCES.txt` & `social-auth-core-4.4.2/social_auth_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 social_core/backends/battlenet.py
 social_core/backends/beats.py
 social_core/backends/behance.py
 social_core/backends/belgiumeid.py
 social_core/backends/bitbucket.py
 social_core/backends/box.py
 social_core/backends/bungie.py
+social_core/backends/cas.py
 social_core/backends/changetip.py
 social_core/backends/chatwork.py
 social_core/backends/cilogon.py
 social_core/backends/classlink.py
 social_core/backends/clef.py
 social_core/backends/coding.py
 social_core/backends/cognito.py
@@ -242,14 +243,15 @@
 social_core/tests/backends/test_auth0.py
 social_core/tests/backends/test_azuread.py
 social_core/tests/backends/test_azuread_b2c.py
 social_core/tests/backends/test_behance.py
 social_core/tests/backends/test_bitbucket.py
 social_core/tests/backends/test_box.py
 social_core/tests/backends/test_broken.py
+social_core/tests/backends/test_cas.py
 social_core/tests/backends/test_chatwork.py
 social_core/tests/backends/test_cilogon.py
 social_core/tests/backends/test_clef.py
 social_core/tests/backends/test_cognito.py
 social_core/tests/backends/test_coinbase.py
 social_core/tests/backends/test_coursera.py
 social_core/tests/backends/test_dailymotion.py
```

### Comparing `social-auth-core-4.4.1/social_core/actions.py` & `social-auth-core-4.4.2/social_core/actions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/amazon.py` & `social-auth-core-4.4.2/social_core/backends/amazon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/angel.py` & `social-auth-core-4.4.2/social_core/backends/angel.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/apple.py` & `social-auth-core-4.4.2/social_core/backends/apple.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/appsfuel.py` & `social-auth-core-4.4.2/social_core/backends/appsfuel.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/arcgis.py` & `social-auth-core-4.4.2/social_core/backends/arcgis.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/asana.py` & `social-auth-core-4.4.2/social_core/backends/asana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/atlassian.py` & `social-auth-core-4.4.2/social_core/backends/atlassian.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/auth0.py` & `social-auth-core-4.4.2/social_core/backends/auth0.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/azuread.py` & `social-auth-core-4.4.2/social_core/backends/azuread.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/azuread_b2c.py` & `social-auth-core-4.4.2/social_core/backends/azuread_b2c.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/azuread_tenant.py` & `social-auth-core-4.4.2/social_core/backends/azuread_tenant.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,26 +42,33 @@
 See https://nicksnettravels.builttoroam.com/post/2017/01/24/Verifying-Azure-Active-Directory-JWT-Tokens.aspx
 for verifying JWT tokens.
 """
 
 
 class AzureADTenantOAuth2(AzureADOAuth2):
     name = "azuread-tenant-oauth2"
-    OPENID_CONFIGURATION_URL = "{base_url}/.well-known/openid-configuration"
-    JWKS_URL = "{base_url}/discovery/keys"
+    OPENID_CONFIGURATION_URL = "{base_url}/.well-known/openid-configuration{appid}"
+    JWKS_URL = "{base_url}/discovery/keys{appid}"
 
     @property
     def tenant_id(self):
         return self.setting("TENANT_ID", "common")
 
     def openid_configuration_url(self):
-        return self.OPENID_CONFIGURATION_URL.format(base_url=self.base_url)
+        return self.OPENID_CONFIGURATION_URL.format(
+            base_url=self.base_url, appid=self._appid()
+        )
 
     def jwks_url(self):
-        return self.JWKS_URL.format(base_url=self.base_url)
+        return self.JWKS_URL.format(base_url=self.base_url, appid=self._appid())
+
+    def _appid(self):
+        return (
+            f"?appid={self.setting('KEY')}" if self.setting("KEY") is not None else ""
+        )
 
     def get_certificate(self, kid):
         # retrieve keys from jwks_url
         resp = self.request(self.jwks_url(), method="GET")
         resp.raise_for_status()
 
         # find the proper key for the kid
@@ -97,18 +104,18 @@
             )
         except (DecodeError, ExpiredSignatureError) as error:
             raise AuthTokenError(self, error)
 
 
 class AzureADV2TenantOAuth2(AzureADTenantOAuth2):
     name = "azuread-v2-tenant-oauth2"
-    OPENID_CONFIGURATION_URL = "{base_url}/v2.0/.well-known/openid-configuration"
+    OPENID_CONFIGURATION_URL = "{base_url}/v2.0/.well-known/openid-configuration{appid}"
     AUTHORIZATION_URL = "{base_url}/oauth2/v2.0/authorize"
     ACCESS_TOKEN_URL = "{base_url}/oauth2/v2.0/token"
-    JWKS_URL = "{base_url}/discovery/v2.0/keys"
+    JWKS_URL = "{base_url}/discovery/v2.0/keys{appid}"
     DEFAULT_SCOPE = ["openid", "profile", "offline_access"]
 
     def get_user_id(self, details, response):
         """Use upn as unique id"""
         return response.get("preferred_username")
 
     def get_user_details(self, response):
```

### Comparing `social-auth-core-4.4.1/social_core/backends/base.py` & `social-auth-core-4.4.2/social_core/backends/base.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/battlenet.py` & `social-auth-core-4.4.2/social_core/backends/battlenet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/beats.py` & `social-auth-core-4.4.2/social_core/backends/beats.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/behance.py` & `social-auth-core-4.4.2/social_core/backends/behance.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/bitbucket.py` & `social-auth-core-4.4.2/social_core/backends/bitbucket.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/box.py` & `social-auth-core-4.4.2/social_core/backends/box.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/bungie.py` & `social-auth-core-4.4.2/social_core/backends/bungie.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/changetip.py` & `social-auth-core-4.4.2/social_core/backends/changetip.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/chatwork.py` & `social-auth-core-4.4.2/social_core/backends/chatwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/cilogon.py` & `social-auth-core-4.4.2/social_core/backends/cilogon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/classlink.py` & `social-auth-core-4.4.2/social_core/backends/classlink.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/clef.py` & `social-auth-core-4.4.2/social_core/backends/clef.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/coding.py` & `social-auth-core-4.4.2/social_core/backends/coding.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/cognito.py` & `social-auth-core-4.4.2/social_core/backends/cognito.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/coinbase.py` & `social-auth-core-4.4.2/social_core/backends/coinbase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/coursera.py` & `social-auth-core-4.4.2/social_core/backends/coursera.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/dailymotion.py` & `social-auth-core-4.4.2/social_core/backends/dailymotion.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/deezer.py` & `social-auth-core-4.4.2/social_core/backends/deezer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/digitalocean.py` & `social-auth-core-4.4.2/social_core/backends/digitalocean.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/discord.py` & `social-auth-core-4.4.2/social_core/backends/discord.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/discourse.py` & `social-auth-core-4.4.2/social_core/backends/discourse.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/disqus.py` & `social-auth-core-4.4.2/social_core/backends/disqus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/docker.py` & `social-auth-core-4.4.2/social_core/backends/docker.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/douban.py` & `social-auth-core-4.4.2/social_core/backends/douban.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/dribbble.py` & `social-auth-core-4.4.2/social_core/backends/dribbble.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/drip.py` & `social-auth-core-4.4.2/social_core/backends/drip.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/dropbox.py` & `social-auth-core-4.4.2/social_core/backends/dropbox.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/echosign.py` & `social-auth-core-4.4.2/social_core/backends/echosign.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/edmodo.py` & `social-auth-core-4.4.2/social_core/backends/edmodo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/elixir.py` & `social-auth-core-4.4.2/social_core/backends/elixir.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/eventbrite.py` & `social-auth-core-4.4.2/social_core/backends/eventbrite.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/eveonline.py` & `social-auth-core-4.4.2/social_core/backends/eveonline.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/evernote.py` & `social-auth-core-4.4.2/social_core/backends/evernote.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/exacttarget.py` & `social-auth-core-4.4.2/social_core/backends/exacttarget.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/facebook.py` & `social-auth-core-4.4.2/social_core/backends/facebook.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/facebook_limited.py` & `social-auth-core-4.4.2/social_core/backends/facebook_limited.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/fence.py` & `social-auth-core-4.4.2/social_core/backends/fence.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/fitbit.py` & `social-auth-core-4.4.2/social_core/backends/fitbit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/five_hundred_px.py` & `social-auth-core-4.4.2/social_core/backends/five_hundred_px.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/flat.py` & `social-auth-core-4.4.2/social_core/backends/flat.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/flickr.py` & `social-auth-core-4.4.2/social_core/backends/flickr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/foursquare.py` & `social-auth-core-4.4.2/social_core/backends/foursquare.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/gae.py` & `social-auth-core-4.4.2/social_core/backends/gae.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/gitea.py` & `social-auth-core-4.4.2/social_core/backends/gitea.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/github.py` & `social-auth-core-4.4.2/social_core/backends/github.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/github_enterprise.py` & `social-auth-core-4.4.2/social_core/backends/github_enterprise.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/gitlab.py` & `social-auth-core-4.4.2/social_core/backends/gitlab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/globus.py` & `social-auth-core-4.4.2/social_core/backends/globus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/goclio.py` & `social-auth-core-4.4.2/social_core/backends/goclio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/google.py` & `social-auth-core-4.4.2/social_core/backends/google.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/google_openidconnect.py` & `social-auth-core-4.4.2/social_core/backends/google_openidconnect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/grafana.py` & `social-auth-core-4.4.2/social_core/backends/grafana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/hubspot.py` & `social-auth-core-4.4.2/social_core/backends/hubspot.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/instagram.py` & `social-auth-core-4.4.2/social_core/backends/instagram.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/itembase.py` & `social-auth-core-4.4.2/social_core/backends/itembase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/jawbone.py` & `social-auth-core-4.4.2/social_core/backends/jawbone.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/justgiving.py` & `social-auth-core-4.4.2/social_core/backends/justgiving.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/kakao.py` & `social-auth-core-4.4.2/social_core/backends/kakao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/keycloak.py` & `social-auth-core-4.4.2/social_core/backends/keycloak.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/khanacademy.py` & `social-auth-core-4.4.2/social_core/backends/khanacademy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/lastfm.py` & `social-auth-core-4.4.2/social_core/backends/lastfm.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/legacy.py` & `social-auth-core-4.4.2/social_core/backends/legacy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/line.py` & `social-auth-core-4.4.2/social_core/backends/line.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/linkedin.py` & `social-auth-core-4.4.2/social_core/backends/linkedin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/live.py` & `social-auth-core-4.4.2/social_core/backends/live.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/livejournal.py` & `social-auth-core-4.4.2/social_core/backends/livejournal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/loginradius.py` & `social-auth-core-4.4.2/social_core/backends/loginradius.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/lyft.py` & `social-auth-core-4.4.2/social_core/backends/lyft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mailchimp.py` & `social-auth-core-4.4.2/social_core/backends/mailchimp.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mailru.py` & `social-auth-core-4.4.2/social_core/backends/mailru.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mapmyfitness.py` & `social-auth-core-4.4.2/social_core/backends/mapmyfitness.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mediawiki.py` & `social-auth-core-4.4.2/social_core/backends/mediawiki.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/meetup.py` & `social-auth-core-4.4.2/social_core/backends/meetup.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mendeley.py` & `social-auth-core-4.4.2/social_core/backends/mendeley.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/microsoft.py` & `social-auth-core-4.4.2/social_core/backends/microsoft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mineid.py` & `social-auth-core-4.4.2/social_core/backends/mineid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/mixcloud.py` & `social-auth-core-4.4.2/social_core/backends/mixcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/monzo.py` & `social-auth-core-4.4.2/social_core/backends/monzo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/moves.py` & `social-auth-core-4.4.2/social_core/backends/moves.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/musicbrainz.py` & `social-auth-core-4.4.2/social_core/backends/musicbrainz.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/nationbuilder.py` & `social-auth-core-4.4.2/social_core/backends/nationbuilder.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/naver.py` & `social-auth-core-4.4.2/social_core/backends/naver.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/ngpvan.py` & `social-auth-core-4.4.2/social_core/backends/ngpvan.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/nk.py` & `social-auth-core-4.4.2/social_core/backends/nk.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/oauth.py` & `social-auth-core-4.4.2/social_core/backends/oauth.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/odnoklassniki.py` & `social-auth-core-4.4.2/social_core/backends/odnoklassniki.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/okta.py` & `social-auth-core-4.4.2/social_core/backends/okta.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/open_id.py` & `social-auth-core-4.4.2/social_core/backends/open_id.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/open_id_connect.py` & `social-auth-core-4.4.2/social_core/backends/open_id_connect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/openinfra.py` & `social-auth-core-4.4.2/social_core/backends/openinfra.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/openshift.py` & `social-auth-core-4.4.2/social_core/backends/openshift.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/openstack.py` & `social-auth-core-4.4.2/social_core/backends/openstack.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/openstreetmap.py` & `social-auth-core-4.4.2/social_core/backends/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/orbi.py` & `social-auth-core-4.4.2/social_core/backends/orbi.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/orcid.py` & `social-auth-core-4.4.2/social_core/backends/orcid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/osso.py` & `social-auth-core-4.4.2/social_core/backends/osso.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/patreon.py` & `social-auth-core-4.4.2/social_core/backends/patreon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/paypal.py` & `social-auth-core-4.4.2/social_core/backends/paypal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/persona.py` & `social-auth-core-4.4.2/social_core/backends/persona.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/phabricator.py` & `social-auth-core-4.4.2/social_core/backends/phabricator.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/pinterest.py` & `social-auth-core-4.4.2/social_core/backends/pinterest.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/pixelpin.py` & `social-auth-core-4.4.2/social_core/backends/pixelpin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/pocket.py` & `social-auth-core-4.4.2/social_core/backends/pocket.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/podio.py` & `social-auth-core-4.4.2/social_core/backends/podio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/professionali.py` & `social-auth-core-4.4.2/social_core/backends/professionali.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/pushbullet.py` & `social-auth-core-4.4.2/social_core/backends/pushbullet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/qiita.py` & `social-auth-core-4.4.2/social_core/backends/qiita.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/qq.py` & `social-auth-core-4.4.2/social_core/backends/qq.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/quizlet.py` & `social-auth-core-4.4.2/social_core/backends/quizlet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/rdio.py` & `social-auth-core-4.4.2/social_core/backends/rdio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/readability.py` & `social-auth-core-4.4.2/social_core/backends/readability.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/reddit.py` & `social-auth-core-4.4.2/social_core/backends/reddit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/runkeeper.py` & `social-auth-core-4.4.2/social_core/backends/runkeeper.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/salesforce.py` & `social-auth-core-4.4.2/social_core/backends/salesforce.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/saml.py` & `social-auth-core-4.4.2/social_core/backends/saml.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/scistarter.py` & `social-auth-core-4.4.2/social_core/backends/scistarter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/seznam.py` & `social-auth-core-4.4.2/social_core/backends/seznam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/shimmering.py` & `social-auth-core-4.4.2/social_core/backends/shimmering.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/shopify.py` & `social-auth-core-4.4.2/social_core/backends/shopify.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/simplelogin.py` & `social-auth-core-4.4.2/social_core/backends/simplelogin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/sketchfab.py` & `social-auth-core-4.4.2/social_core/backends/sketchfab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/skyrock.py` & `social-auth-core-4.4.2/social_core/backends/skyrock.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/slack.py` & `social-auth-core-4.4.2/social_core/backends/slack.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/soundcloud.py` & `social-auth-core-4.4.2/social_core/backends/soundcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/spotify.py` & `social-auth-core-4.4.2/social_core/backends/spotify.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/stackoverflow.py` & `social-auth-core-4.4.2/social_core/backends/stackoverflow.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/steam.py` & `social-auth-core-4.4.2/social_core/backends/steam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/stocktwits.py` & `social-auth-core-4.4.2/social_core/backends/stocktwits.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/strava.py` & `social-auth-core-4.4.2/social_core/backends/strava.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/stripe.py` & `social-auth-core-4.4.2/social_core/backends/stripe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/surveymonkey.py` & `social-auth-core-4.4.2/social_core/backends/surveymonkey.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/taobao.py` & `social-auth-core-4.4.2/social_core/backends/taobao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/telegram.py` & `social-auth-core-4.4.2/social_core/backends/telegram.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/thisismyjam.py` & `social-auth-core-4.4.2/social_core/backends/thisismyjam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/trello.py` & `social-auth-core-4.4.2/social_core/backends/trello.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/tripit.py` & `social-auth-core-4.4.2/social_core/backends/tripit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/tumblr.py` & `social-auth-core-4.4.2/social_core/backends/tumblr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/twilio.py` & `social-auth-core-4.4.2/social_core/backends/twilio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/twitch.py` & `social-auth-core-4.4.2/social_core/backends/twitch.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/twitter.py` & `social-auth-core-4.4.2/social_core/backends/twitter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/uber.py` & `social-auth-core-4.4.2/social_core/backends/uber.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/udata.py` & `social-auth-core-4.4.2/social_core/backends/udata.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/universe.py` & `social-auth-core-4.4.2/social_core/backends/universe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/untappd.py` & `social-auth-core-4.4.2/social_core/backends/untappd.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/upwork.py` & `social-auth-core-4.4.2/social_core/backends/upwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/utils.py` & `social-auth-core-4.4.2/social_core/backends/utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/vend.py` & `social-auth-core-4.4.2/social_core/backends/vend.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/vimeo.py` & `social-auth-core-4.4.2/social_core/backends/vimeo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/vk.py` & `social-auth-core-4.4.2/social_core/backends/vk.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/weibo.py` & `social-auth-core-4.4.2/social_core/backends/weibo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/weixin.py` & `social-auth-core-4.4.2/social_core/backends/weixin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/withings.py` & `social-auth-core-4.4.2/social_core/backends/withings.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/wunderlist.py` & `social-auth-core-4.4.2/social_core/backends/wunderlist.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/xing.py` & `social-auth-core-4.4.2/social_core/backends/xing.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/yahoo.py` & `social-auth-core-4.4.2/social_core/backends/yahoo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/yammer.py` & `social-auth-core-4.4.2/social_core/backends/yammer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/yandex.py` & `social-auth-core-4.4.2/social_core/backends/yandex.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/zoom.py` & `social-auth-core-4.4.2/social_core/backends/zoom.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/backends/zotero.py` & `social-auth-core-4.4.2/social_core/backends/zotero.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/exceptions.py` & `social-auth-core-4.4.2/social_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/__init__.py` & `social-auth-core-4.4.2/social_core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/disconnect.py` & `social-auth-core-4.4.2/social_core/pipeline/disconnect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/mail.py` & `social-auth-core-4.4.2/social_core/pipeline/mail.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/partial.py` & `social-auth-core-4.4.2/social_core/pipeline/partial.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/social_auth.py` & `social-auth-core-4.4.2/social_core/pipeline/social_auth.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/user.py` & `social-auth-core-4.4.2/social_core/pipeline/user.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/pipeline/utils.py` & `social-auth-core-4.4.2/social_core/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/storage.py` & `social-auth-core-4.4.2/social_core/storage.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/store.py` & `social-auth-core-4.4.2/social_core/store.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/strategy.py` & `social-auth-core-4.4.2/social_core/strategy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/actions/actions.py` & `social-auth-core-4.4.2/social_core/tests/actions/actions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/actions/test_associate.py` & `social-auth-core-4.4.2/social_core/tests/actions/test_associate.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/actions/test_disconnect.py` & `social-auth-core-4.4.2/social_core/tests/actions/test_disconnect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/actions/test_login.py` & `social-auth-core-4.4.2/social_core/tests/actions/test_login.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/base.py` & `social-auth-core-4.4.2/social_core/tests/backends/base.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/data/saml_config.json` & `social-auth-core-4.4.2/social_core/tests/backends/data/saml_config.json`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/data/saml_response.txt` & `social-auth-core-4.4.2/social_core/tests/backends/data/saml_response.txt`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/legacy.py` & `social-auth-core-4.4.2/social_core/tests/backends/legacy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/oauth.py` & `social-auth-core-4.4.2/social_core/tests/backends/oauth.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/open_id.py` & `social-auth-core-4.4.2/social_core/tests/backends/open_id.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_amazon.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_amazon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_angel.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_angel.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_apple.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_apple.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_arcgis.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_arcgis.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_asana.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_asana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_atlassian.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_atlassian.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_auth0.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_auth0.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_azuread.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_azuread.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_azuread_b2c.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_azuread_b2c.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_behance.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_behance.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_bitbucket.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_box.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_box.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_broken.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_broken.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_chatwork.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_chatwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_cilogon.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_cilogon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_clef.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_clef.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_cognito.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_cognito.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_coinbase.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_coinbase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_coursera.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_coursera.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_dailymotion.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_deezer.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_deezer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_digitalocean.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_digitalocean.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_discourse.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_discourse.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_disqus.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_disqus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_dribbble.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_dribbble.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_drip.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_drip.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_dropbox.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_dummy.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_dummy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_edmodo.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_edmodo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_elixir.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_elixir.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_eventbrite.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_eventbrite.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_evernote.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_evernote.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_facebook.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_facebook.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_fence.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_fence.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_fitbit.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_fitbit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_five_hundred_px.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_five_hundred_px.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_flat.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_flat.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_flickr.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_flickr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_foursquare.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_foursquare.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_gitea.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_gitea.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_github.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_github.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_github_enterprise.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_github_enterprise.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_gitlab.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_globus.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_globus.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_google.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_google.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_grafana.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_grafana.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_instagram.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_instagram.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_itembase.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_itembase.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_kakao.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_kakao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_keycloak.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_khanacademy.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_khanacademy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_linkedin.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_linkedin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_live.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_live.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_livejournal.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_livejournal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_lyft.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_lyft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_mailru.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_mailru.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_mapmyfitness.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_mapmyfitness.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_microsoft.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_microsoft.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_mineid.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_mineid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_mixcloud.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_musicbrainz.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_musicbrainz.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_nationbuilder.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_nationbuilder.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_naver.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_naver.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_ngpvan.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_ngpvan.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_okta.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_okta.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_open_id_connect.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_open_id_connect.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_orbi.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_orbi.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_orcid.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_orcid.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_osso.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_osso.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_patreon.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_patreon.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_paypal.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_paypal.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_phabricator.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_pinterest.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_pinterest.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_podio.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_podio.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_qiita.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_qiita.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_quizlet.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_quizlet.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_readability.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_readability.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_reddit.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_reddit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_saml.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_saml.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_scistarter.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_scistarter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_seznam.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_seznam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_simplelogin.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_simplelogin.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_sketchfab.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_sketchfab.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_skyrock.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_skyrock.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_slack.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_slack.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_soundcloud.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_soundcloud.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_spotify.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_spotify.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_stackoverflow.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_stackoverflow.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_steam.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_steam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_stocktwits.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_stocktwits.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_strava.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_strava.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_stripe.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_stripe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_taobao.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_taobao.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_thisismyjam.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_thisismyjam.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_tripit.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_tripit.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_tumblr.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_tumblr.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_twitch.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_twitch.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_twitter.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_twitter.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_uber.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_uber.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_udata.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_udata.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_universe.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_universe.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_upwork.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_upwork.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_utils.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_vault.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_vault.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_vk.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_vk.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_wunderlist.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_wunderlist.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_xing.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_xing.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_yahoo.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_yammer.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_yammer.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_yandex.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_yandex.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_zoom.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_zoom.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/backends/test_zotero.py` & `social-auth-core-4.4.2/social_core/tests/backends/test_zotero.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/models.py` & `social-auth-core-4.4.2/social_core/tests/models.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/pipeline.py` & `social-auth-core-4.4.2/social_core/tests/pipeline.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/strategy.py` & `social-auth-core-4.4.2/social_core/tests/strategy.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/test_exceptions.py` & `social-auth-core-4.4.2/social_core/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/test_partial.py` & `social-auth-core-4.4.2/social_core/tests/test_partial.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/test_pipeline.py` & `social-auth-core-4.4.2/social_core/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/test_storage.py` & `social-auth-core-4.4.2/social_core/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/test_utils.py` & `social-auth-core-4.4.2/social_core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/tests/testkey.pem` & `social-auth-core-4.4.2/social_core/tests/testkey.pem`

 * *Files identical despite different names*

### Comparing `social-auth-core-4.4.1/social_core/utils.py` & `social-auth-core-4.4.2/social_core/utils.py`

 * *Files identical despite different names*

