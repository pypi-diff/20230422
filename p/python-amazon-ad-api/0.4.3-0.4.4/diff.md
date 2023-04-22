# Comparing `tmp/python-amazon-ad-api-0.4.3.tar.gz` & `tmp/python-amazon-ad-api-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amazon-ad-api-0.4.3.tar", last modified: Tue Apr 18 09:10:01 2023, max compression
+gzip compressed data, was "python-amazon-ad-api-0.4.4.tar", last modified: Sat Apr 22 12:35:56 2023, max compression
```

## Comparing `python-amazon-ad-api-0.4.3.tar` & `python-amazon-ad-api-0.4.4.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.789287 python-amazon-ad-api-0.4.3/ad_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.797287 python-amazon-ad-api-0.4.3/ad_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/advertising_test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/brand_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/creative_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.797287 python-amazon-ad-api-0.4.3/ad_api/api/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/dsp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/eligibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/manager_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.805287 python-amazon-ad-api-0.4.3/ad_api/api/sb/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/ads_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/brands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/landing_page_asins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sb/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.809287 python-amazon-ad-api-0.4.3/ad_api/api/sd/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/brand_safety.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/budget_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns_budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/creatives.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sd/targeting_recommendations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.817287 python-amazon-ad-api-0.4.3/ad_api/api/sp/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_initial_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_consolidated_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/campaings_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/ranked_keywords_recommendations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/sp/suggested_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/api/validation_configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.821287 python-amazon-ad-api-0.4.3/ad_api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.821287 python-amazon-ad-api-0.4.3/ad_api/base/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/marketplaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/ad_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 09:10:01.000000 python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-18 09:10:01.825287 python-amazon-ad-api-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 09:09:48.000000 python-amazon-ad-api-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17362 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.351555 python-amazon-ad-api-0.4.4/ad_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.355555 python-amazon-ad-api-0.4.4/ad_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/advertising_test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/brand_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/creative_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.355555 python-amazon-ad-api-0.4.4/ad_api/api/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/dsp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/manager_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.359555 python-amazon-ad-api-0.4.4/ad_api/api/sb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/ads_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/landing_page_asins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sb/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.359555 python-amazon-ad-api-0.4.4/ad_api/api/sd/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/brand_safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19461 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/creatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13401 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sd/targeting_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.363555 python-amazon-ad-api-0.4.4/ad_api/api/sp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_initial_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_consolidated_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/campaings_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/ranked_keywords_recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/sp/suggested_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/api/validation_configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/ad_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/ad_api/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/marketplaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/ad_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 12:35:56.000000 python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 12:35:56.367555 python-amazon-ad-api-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-22 12:35:45.000000 python-amazon-ad-api-0.4.4/setup.py
```

### Comparing `python-amazon-ad-api-0.4.3/LICENSE` & `python-amazon-ad-api-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/PKG-INFO` & `python-amazon-ad-api-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-ad-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python wrapper for the Amazon Advertising API
 Home-page: https://github.com/denisneuf/python-amazon-ad-api
 Author: Daniel Alvaro
 Author-email: info@leadtech.es
 License: MIT
 Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
 Classifier: Programming Language :: Python :: 3
@@ -295,29 +295,29 @@
 * [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
 * [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
 * [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 
 
 ### [Modules Available Sponsored Brands 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v3.html)
 
-* Campaigns(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
-* Ad Groups(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
-* Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
-* Negative Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
-* Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
-* Negative Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
-* Targeting Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
-* Bid Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
-* Stores(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
-* Landing Page Asins(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
-* Media(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
-* Brands(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
-* Moderation(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
-* Reports(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
-* Snapshots
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
+* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
+* [Targeting Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
+* [Stores](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
+* [Landing Page Asins](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
+* [Media](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
+* [Brands](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
+* [Moderation](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
+* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/snapshots.html)
 
 ### [Modules Available Sponsored Brands 4.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v4.html)
 
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
 * [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
 
@@ -334,17 +334,17 @@
 * [Creatives](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/creatives.html)
 * [Brand Safety List](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/brand_safety.html)
 * [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/budget_rules.html)
 * [Campaigns Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaign_budget_usage.html)
 * [Forecasts](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/forecast.html)
 * [Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/recommendations.html)
 
-### Modules Available DSP
+### [Modules Available DSP](https://python-amazon-ad-api.readthedocs.io/en/latest/dsp.html)
 
-* Reports
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/dsp/reports.html)
 
 ### Simple Example Usage Campaigns with Credentials
 
 ```python
 import logging
 from ad_api.base import AdvertisingApiException
 from ad_api.api.sp import Campaigns
```

### Comparing `python-amazon-ad-api-0.4.3/README.md` & `python-amazon-ad-api-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -280,29 +280,29 @@
 * [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
 * [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
 * [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 
 
 ### [Modules Available Sponsored Brands 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v3.html)
 
-* Campaigns(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
-* Ad Groups(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
-* Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
-* Negative Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
-* Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
-* Negative Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
-* Targeting Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
-* Bid Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
-* Stores(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
-* Landing Page Asins(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
-* Media(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
-* Brands(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
-* Moderation(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
-* Reports(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
-* Snapshots
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
+* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
+* [Targeting Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
+* [Stores](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
+* [Landing Page Asins](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
+* [Media](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
+* [Brands](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
+* [Moderation](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
+* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/snapshots.html)
 
 ### [Modules Available Sponsored Brands 4.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v4.html)
 
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
 * [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
 
@@ -319,17 +319,17 @@
 * [Creatives](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/creatives.html)
 * [Brand Safety List](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/brand_safety.html)
 * [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/budget_rules.html)
 * [Campaigns Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaign_budget_usage.html)
 * [Forecasts](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/forecast.html)
 * [Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/recommendations.html)
 
-### Modules Available DSP
+### [Modules Available DSP](https://python-amazon-ad-api.readthedocs.io/en/latest/dsp.html)
 
-* Reports
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/dsp/reports.html)
 
 ### Simple Example Usage Campaigns with Credentials
 
 ```python
 import logging
 from ad_api.base import AdvertisingApiException
 from ad_api.api.sp import Campaigns
```

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/__init__.py` & `python-amazon-ad-api-0.4.4/ad_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/advertising_test_account.py` & `python-amazon-ad-api-0.4.4/ad_api/api/advertising_test_account.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/attribution.py` & `python-amazon-ad-api-0.4.4/ad_api/api/attribution.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/audiences.py` & `python-amazon-ad-api-0.4.4/ad_api/api/audiences.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/billing.py` & `python-amazon-ad-api-0.4.4/ad_api/api/billing.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/brand_metrics.py` & `python-amazon-ad-api-0.4.4/ad_api/api/brand_metrics.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/creative_assets.py` & `python-amazon-ad-api-0.4.4/ad_api/api/creative_assets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/dsp/client.py` & `python-amazon-ad-api-0.4.4/ad_api/api/dsp/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/dsp/credential_provider.py` & `python-amazon-ad-api-0.4.4/ad_api/api/dsp/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/dsp/reports.py` & `python-amazon-ad-api-0.4.4/ad_api/api/dsp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/eligibility.py` & `python-amazon-ad-api-0.4.4/ad_api/api/eligibility.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/history.py` & `python-amazon-ad-api-0.4.4/ad_api/api/history.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/insights.py` & `python-amazon-ad-api-0.4.4/ad_api/api/insights.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/invoices.py` & `python-amazon-ad-api-0.4.4/ad_api/api/invoices.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/localization.py` & `python-amazon-ad-api-0.4.4/ad_api/api/localization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/manager_accounts.py` & `python-amazon-ad-api-0.4.4/ad_api/api/manager_accounts.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/metadata.py` & `python-amazon-ad-api-0.4.4/ad_api/api/metadata.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/portfolios.py` & `python-amazon-ad-api-0.4.4/ad_api/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/profiles.py` & `python-amazon-ad-api-0.4.4/ad_api/api/profiles.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/reports.py` & `python-amazon-ad-api-0.4.4/ad_api/api/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse
+from ad_api.base import Client, sp_endpoint, fill_query_params, ApiResponse, Utils
 
 
 class Reports(Client):
     """Sponsored Products Reports Version 3
 
     Documentation: https://advertising.amazon.com/API/docs/en-us/offline-report-prod-3p
 
@@ -31,15 +31,15 @@
                     | **values** (list > string): The values to be filtered by.
                 | **timeUnit** (string): [required] Enum: The aggregation level of report data. If the timeUnit is set to SUMMARY, the report data is aggregated at the time period specified. The availability of time unit breakdowns depends on the selection of reportTypeId. [ SUMMARY, DAILY ]
 
         Returns:
             ApiResponse
 
         """
-        return self._request(kwargs.pop('path'), data=kwargs.pop('body'), params=kwargs)
+        return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs)
 
     @sp_endpoint('/reporting/reports/{}', method='GET')
     def get_report(self, reportId, **kwargs) -> ApiResponse:
         r"""
         Gets a generation status of a report by id. Uses the reportId value from the response of previously requested report via POST /reporting/reports operation. When status is set to COMPLETED, the report will be available to be downloaded at url.
         Report generation can take as long as 3 hours. Repeated calls to check report status may generate a 429 response, indicating that your requests have been throttled. To retrieve reports programmatically, your application logic should institute a delay between requests.
```

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/__init__.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/ad_groups_v4.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/ad_groups_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/ads_v4.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/ads_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/bid_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/brands.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/brands.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/campaigns_v4.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/campaigns_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/keywords.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/landing_page_asins.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/landing_page_asins.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/media.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/media.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/moderation.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/moderation.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_keywords.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/negative_product_targeting.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/product_targeting.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/reports.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/snapshots.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/stores.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/stores.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sb/targeting_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sb/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/__init__.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/ad_groups.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/bid_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/brand_safety.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/brand_safety.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/budget_rules.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/budget_rules.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/campaigns_budget_usage.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/campaigns_budget_usage.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/creatives.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/creatives.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/forecast.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/forecast.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/negative_product_targeting.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/product_ads.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/product_targeting.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/reports.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/snapshots.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sd/targeting_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sd/targeting_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/__init__.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/ad_groups_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/ad_groups_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/bid_recommendations_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/bid_recommendations_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_initial_recommendation.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_initial_recommendation.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/budget_rules_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/budget_rules_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_consolidated_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_consolidated_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_keywords_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaign_negative_targets.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaign_negative_targets.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_budget_usage.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_budget_usage.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaigns_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaigns_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/campaings_optimization.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/campaings_optimization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/keywords_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/keywords_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         Listing product keywords.
 
         Request Body (optional)
 
         Returns
             ApiResponse
         """
-        json_version = 'application/vnd.spKeyword.v3+json' + str(version) + "+json"
+        json_version = 'application/vnd.spKeyword.v' + str(version) + "+json"
         headers = {
             "Accept": json_version,
             "Content-Type": json_version
         }
 
         return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs,
                              headers=headers)
@@ -35,15 +35,15 @@
             | **state**: *string*, The current resource state.' , 'Enum': '[ enabled ]
             | **keywordText**: *string*, The text of the expression to match against a search query.
             | **matchType**: *string*, 'The type of match.' , 'Enum': '[EXACT, PHRASE, BROAD]
 
         Returns
             ApiResponse
         """
-        json_version = 'application/vnd.spKeyword.v3+json' + str(version) + "+json"
+        json_version = 'application/vnd.spKeyword.v' + str(version) + "+json"
 
         headers = {
             "Accept": json_version,
             "Content-Type": json_version
         }
 
         prefer_value = 'return=representation'
@@ -63,15 +63,15 @@
             | '**state**': *string*, {'description': 'The current resource state.' , 'Enum': '[ enabled, paused, archived ]'}
             | '**bid**': *float* {'description': 'Bid associated with this keyword. Applicable to biddable match types only.'}
 
         Returns
             ApiResponse
         """
 
-        json_version = 'application/vnd.spKeyword.v3+json' + str(version) + "+json"
+        json_version = 'application/vnd.spKeyword.v' + str(version) + "+json"
         headers = {
             "Accept": json_version,
             "Content-Type": json_version
         }
 
         prefer_value = 'return=representation'
         if prefer:
@@ -89,15 +89,15 @@
             | **keywordIdFilter** {} : Filter keywords by the list of objectIds
                 include [string] : list of keywordsIds as String to be used as filter. MinItems : 0, MaxItems :1000
 
         Returns
             ApiResponse
         """
 
-        json_version = 'application/vnd.spKeyword.v3+json' + str(version) + "+json"
+        json_version = 'application/vnd.spKeyword.v' + str(version) + "+json"
         headers = {
             "Accept": json_version,
             "Content-Type": json_version
         }
 
         return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs,
                              headers=headers)
```

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_keywords_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_keywords_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/negative_product_targeting_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/negative_product_targeting_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_ads_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_ads_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             | **max_results** (int) Number of records to include in the paginated response. Defaults to max page size for given API. Minimum 10 and a Maximum of 100 [optional]
             | **includeExtendedDataFields** (boolean) Whether to get entity with extended data fields such as creationDate, lastUpdateDate, servingStatus [optional]
 
         Returns:
             ApiResponse
         """
 
-        json_version = 'application/vnd.spCampaign.v' + str(version) + "+json"
+        json_version = 'application/vnd.spproductAd.v' + str(version) + "+json"
 
         headers = {
             "Accept": json_version,
             "Content-Type": json_version
         }
 
         return self._request(kwargs.pop('path'), data=Utils.convert_body(kwargs.pop('body'), False), params=kwargs,
```

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/product_targeting_v3.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/product_targeting_v3.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/ranked_keywords_recommendations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/ranked_keywords_recommendations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/reports.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/snapshots.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/snapshots.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/sp/suggested_keywords.py` & `python-amazon-ad-api-0.4.4/ad_api/api/sp/suggested_keywords.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/api/validation_configurations.py` & `python-amazon-ad-api-0.4.4/ad_api/api/validation_configurations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/auth/access_token_client.py` & `python-amazon-ad-api-0.4.4/ad_api/auth/access_token_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 import logging
 from cachetools import TTLCache
 from ad_api.base import BaseClient
 
 from .credentials import Credentials
 from .access_token_response import AccessTokenResponse
 from .exceptions import AuthorizationError
+# from .credential_provider import CredentialProvider
+
 import os
 
 cache = TTLCache(maxsize=int(os.environ.get('AD_API_AUTH_CACHE_SIZE', 10)), ttl=3200)
 grantless_cache = TTLCache(maxsize=int(os.environ.get('AD_API_AUTH_CACHE_SIZE', 10)), ttl=3200)
 
 logger = logging.getLogger(__name__)
 
 
 class AccessTokenClient(BaseClient):
     host = 'api.amazon.com'
     grant_type = 'refresh_token'
     path = '/auth/o2/token'
 
-    def __init__(self, account='default', credentials=None, credentials_class=Credentials, proxies=None, verify=True, timeout=None):
-        super().__init__(account, credentials)
-        self.cred = credentials_class(self.credentials)
+    def __init__(self, credentials=None, proxies=None, verify=True, timeout=None):
+
+        self.cred = Credentials(credentials)
         self.timeout = timeout
         self.proxies = proxies
         self.verify = verify
 
     def _request(self, url, data, headers):
         response = requests.post(
             url,
```

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/__init__.py` & `python-amazon-ad-api-0.4.4/ad_api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/api_response.py` & `python-amazon-ad-api-0.4.4/ad_api/base/api_response.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/client.py` & `python-amazon-ad-api-0.4.4/ad_api/base/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 import json
+from json import JSONDecodeError
 import logging
 from cachetools import TTLCache
 from requests import request
 from ad_api.auth.credentials import Credentials
 from ad_api.auth import AccessTokenClient, AccessTokenResponse
 from .api_response import ApiResponse
 from .base_client import BaseClient
-from .exceptions import get_exception_for_content
+from .exceptions import get_exception_for_code, get_exception_for_content
 from .marketplaces import Marketplaces
 import os
 import requests
 from io import BytesIO
 import gzip
 from zipfile import ZipFile
 import zipfile
 from urllib.parse import urlparse, quote
+from ad_api.base.credential_provider import CredentialProvider
 
 log = logging.getLogger(__name__)
 role_cache = TTLCache(maxsize=int(os.environ.get('AD_API_AUTH_CACHE_SIZE', 10)), ttl=3200)
 
 
 class Client(BaseClient):
-    access_token_client_class = AccessTokenClient
-    credentials_class = Credentials
-    grantless_scope = ''
 
     def __init__(
             self,
             account='default',
             marketplace: Marketplaces = Marketplaces[os.environ[
                 'AD_API_DEFAULT_MARKETPLACE']] if 'AD_API_DEFAULT_MARKETPLACE' in os.environ else Marketplaces.EU,
             credentials=None,
             proxies=None,
             verify=True,
             timeout=None,
             debug=False
     ):
 
-        super().__init__(account, credentials)
-        self.endpoint = marketplace.endpoint
-        self.debug = debug
-        self._auth = self.access_token_client_class(
-            account=account,
-            credentials=credentials,
-            credentials_class=self.credentials_class,
+        self.credentials = CredentialProvider(account, credentials).credentials
+        self._auth = AccessTokenClient(
+            credentials=self.credentials,
             proxies=proxies,
             verify=verify,
             timeout=timeout,
         )
+        self.endpoint = marketplace.endpoint
+        self.debug = debug
         self.timeout = timeout
         self.proxies = proxies
         self.verify = verify
 
     @property
     def headers(self):
         return {
             'User-Agent': self.user_agent,
-            'Amazon-Advertising-API-ClientId': self.credentials.client_id,
+            'Amazon-Advertising-API-ClientId': self.credentials['client_id'],
             'Authorization': 'Bearer %s' % self.auth.access_token,
-            'Amazon-Advertising-API-Scope': self.credentials.profile_id,
+            'Amazon-Advertising-API-Scope': self.credentials['profile_id'],
             'Content-Type': 'application/json'
         }
 
     @property
     def auth(self) -> AccessTokenResponse:
         return self._auth.get_auth()
 
@@ -259,85 +256,65 @@
             proxies=self.proxies,
             verify=self.verify,
         )
 
         if self.debug:
             logging.info(headers or self.headers)
 
+
             if params:
                 str_query = ""
                 for key, value in params.items():
                     str_query += key + "=" + quote(str(value))
                 message = method + " " + self.endpoint + path + "?" + str_query
             else:
                 message = method + " " + self.endpoint + path
 
             logging.info(message)
             if data is not None:
                 logging.info(data)
 
-        return self._check_response(res)
+            logging.info(vars(res))
 
-    # @staticmethod
-    def _check_response(self, res) -> ApiResponse:
+        return self._check_response(res)
 
-        if self.debug:
-            logging.info(vars(res))
+    @staticmethod
+    def _check_response(res) -> ApiResponse:
 
         content = vars(res).get('_content')
-        str_content = content.decode('utf8')
+        headers = vars(res).get('headers')
+        status_code = vars(res).get('status_code')
 
-        if type(str_content) is str and str_content[0:50] == '<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">' and vars(res).get('_content_consumed') is True:
+        if 200 <= res.status_code < 300:
+
+            try:
+                js = res.json() or {}
+            except JSONDecodeError:
+                js = {}
+
+            try:
+                error = js.get('error', None) # Dict.get(key, default=None)
+            except AttributeError:
+                error = None
+
+            if error:
+                exception = get_exception_for_content(error[0].get('code'))
+                raise exception(error[0].get('code'), error[0], headers)
+
+            next_token = vars(res).get('_next')
+
+            return ApiResponse(js, next_token, headers=headers)
+
+        else:
+
+            exception = get_exception_for_code(res.status_code)
+
+            try:
+                js = res.json()
+            except JSONDecodeError:
+                js = res.content
+
+
+            raise exception(status_code, js, headers)
+            exit(res.status_code)
 
-            dictionary = {"status_code": vars(res).get('status_code'), "msg": "Unauthorized"}
-            exception = get_exception_for_content(dictionary)
-            raise exception(dictionary)
-
-        if type(str_content) is str and str_content[0:15] == 'Invalid request' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "msg": str_content}
-            exception = get_exception_for_content(dictionary)
-            raise exception(dictionary)
-
-        data = json.loads(str_content)
-
-        if type(data) is dict and data.get('code') == 'UNAUTHORIZED':
-            exception = get_exception_for_content(data)
-            raise exception(data)
-
-        if type(data) is dict and data.get('message') == 'Too Many Requests' and vars(res).get('_content_consumed') is True:
-            exception = get_exception_for_content(data)
-            raise exception(data)
-
-        if type(data) is dict and data.get('code') == 'NOT_FOUND' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "code": data.get('code'), "details": data.get('details'), "requestId": data.get('requestId')}
-            exception = get_exception_for_content(data)
-            raise exception(dictionary)
-
-        if type(data) is dict and data.get('code') == 'SERVER_IS_BUSY' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "code": data.get('code'), "details": data.get('details'), "requestId": data.get('requestId')}
-            exception = get_exception_for_content(data)
-            raise exception(dictionary)
-
-        if type(data) is dict and data.get('message') == 'Unauthorized' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "message": "Unauthorized"}
-            exception = get_exception_for_content(dictionary)
-            raise exception(dictionary)
-
-        if type(data) is dict and data.get('details') == 'Invalid authorization inputs' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "message": "Invalid authorization inputs"}
-            exception = get_exception_for_content(dictionary)
-            raise exception(dictionary)
-
-        if type(data) is dict and data.get('message') == 'Missing Authentication Token' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "message": "Missing Authentication Token"}
-            exception = get_exception_for_content(dictionary)
-            raise exception(dictionary)
-
-        if type(data) is dict and data.get('details') == 'Cannot consume content type' and vars(res).get('_content_consumed') is True:
-            dictionary = {"status_code": vars(res).get('status_code'), "message": data.get('details')}
-            exception = get_exception_for_content(dictionary)
-            raise exception(dictionary)
 
-        headers = vars(res).get('headers')
-        status_code = vars(res).get('status_code')
-        next_token = vars(res).get('_next')
-        return ApiResponse(data, next_token, headers=headers)
```

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/config.py` & `python-amazon-ad-api-0.4.4/ad_api/base/config.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/helpers.py` & `python-amazon-ad-api-0.4.4/ad_api/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/marketplaces.py` & `python-amazon-ad-api-0.4.4/ad_api/base/marketplaces.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/ad_api/base/utils.py` & `python-amazon-ad-api-0.4.4/ad_api/base/utils.py`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/PKG-INFO` & `python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-ad-api
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python wrapper for the Amazon Advertising API
 Home-page: https://github.com/denisneuf/python-amazon-ad-api
 Author: Daniel Alvaro
 Author-email: info@leadtech.es
 License: MIT
 Project-URL: Bug Tracker, https://github.com/denisneuf/python-amazon-ad-api/issues
 Classifier: Programming Language :: Python :: 3
@@ -295,29 +295,29 @@
 * [Product Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/budget_recommendations.html)
 * [Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sp/campaign_budget_usage.html)
 * [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/api/reports.html)
 
 
 ### [Modules Available Sponsored Brands 3.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v3.html)
 
-* Campaigns(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
-* Ad Groups(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
-* Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
-* Negative Keywords(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
-* Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
-* Negative Product Targeting(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
-* Targeting Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
-* Bid Recommendations(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
-* Stores(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
-* Landing Page Asins(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
-* Media(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
-* Brands(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
-* Moderation(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
-* Reports(https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
-* Snapshots
+* [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns.html)
+* [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups.html)
+* [Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/keywords.html)
+* [Negative Keywords](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_keywords.html)
+* [Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/product_targeting.html)
+* [Negative Product Targeting](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/negative_product_targeting.html)
+* [Targeting Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/targeting_recommendations.html)
+* [Bid Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/bid_recommendations.html)
+* [Stores](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/stores.html)
+* [Landing Page Asins](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/landing_page_asins.html)
+* [Media](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/media.html)
+* [Brands](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/brands.html)
+* [Moderation](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/moderation.html)
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/reports.html)
+* [Snapshots](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/snapshots.html)
 
 ### [Modules Available Sponsored Brands 4.0](https://python-amazon-ad-api.readthedocs.io/en/latest/sb_v4.html)
 
 * [Campaigns](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/campaigns_v4.html)
 * [Ad Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ad_groups_v4.html)
 * [Ads Groups](https://python-amazon-ad-api.readthedocs.io/en/latest/sb/ads_v4.html)
 
@@ -334,17 +334,17 @@
 * [Creatives](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/creatives.html)
 * [Brand Safety List](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/brand_safety.html)
 * [Budget Rules](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/budget_rules.html)
 * [Campaigns Budget Usage](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/campaign_budget_usage.html)
 * [Forecasts](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/forecast.html)
 * [Recommendations](https://python-amazon-ad-api.readthedocs.io/en/latest/sd/recommendations.html)
 
-### Modules Available DSP
+### [Modules Available DSP](https://python-amazon-ad-api.readthedocs.io/en/latest/dsp.html)
 
-* Reports
+* [Reports](https://python-amazon-ad-api.readthedocs.io/en/latest/dsp/reports.html)
 
 ### Simple Example Usage Campaigns with Credentials
 
 ```python
 import logging
 from ad_api.base import AdvertisingApiException
 from ad_api.api.sp import Campaigns
```

### Comparing `python-amazon-ad-api-0.4.3/python_amazon_ad_api.egg-info/SOURCES.txt` & `python-amazon-ad-api-0.4.4/python_amazon_ad_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-amazon-ad-api-0.4.3/setup.cfg` & `python-amazon-ad-api-0.4.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-amazon-ad-api
-version = 0.4.3
+version = 0.4.4
 author = Daniel Alvaro
 author_email = denisneuf@hotmail.com
 description = Python wrapper for the Amazon Advertising API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/denisneuf/python-amazon-ad-api
 project_urls =
```

### Comparing `python-amazon-ad-api-0.4.3/setup.py` & `python-amazon-ad-api-0.4.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='python-amazon-ad-api',
-    version='0.4.3',
+    version='0.4.4',
     install_requires=[
         "requests>=2.27.1,<2.29.0",
         "six~=1.16.0",
         "cachetools>=5.0,<5.4",
         "pycryptodome>=3.13,<3.18",
         "python-dotenv>=0.19.2,<1.1.0",
         "pytz>=2021.3,<2024.0",
```

