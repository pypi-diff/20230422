# Comparing `tmp/edc-pharmacy-0.1.8.tar.gz` & `tmp/edc-pharmacy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-pharmacy-0.1.8.tar", last modified: Fri Apr 15 00:43:03 2022, max compression
+gzip compressed data, was "edc-pharmacy-0.1.9.tar", last modified: Fri Apr 15 14:57:37 2022, max compression
```

## Comparing `edc-pharmacy-0.1.8.tar` & `edc-pharmacy-0.1.9.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.976579 edc-pharmacy-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)    18046 2020-03-04 23:10:42.000000 edc-pharmacy-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      207 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1747 2022-04-15 00:43:03.976650 edc-pharmacy-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      883 2020-03-13 03:26:28.000000 edc-pharmacy-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.963075 edc-pharmacy-0.1.8/edc_pharmacy/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.8/edc_pharmacy/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      761 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/action_items.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.966637 edc-pharmacy-0.1.8/edc_pharmacy/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      868 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.966912 edc-pharmacy-0.1.8/edc_pharmacy/admin/actions/
--rw-r--r--   0 erikvw     (501) staff       (20)       62 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/actions/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1679 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/actions/print_stock_labels.py
--rw-r--r--   0 erikvw     (501) staff       (20)      661 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/autocomplete_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2211 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/dispensing_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      952 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/dosage_guideline_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1145 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/formulation_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1763 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/labels_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      834 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/list_model_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      685 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      940 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_lot_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3030 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_order_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1268 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_product_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1212 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_stock_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1550 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_stock_create_labels_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1411 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_stock_receiving_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      571 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/model_admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1644 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/return_history_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2466 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/rx_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6558 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin/rx_refill_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1897 2021-05-05 19:47:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      200 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      762 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/approve_prescription.py
--rw-r--r--   0 erikvw     (501) staff       (20)      221 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      636 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      495 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)      477 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.967168 edc-pharmacy-0.1.8/edc_pharmacy/dispense/
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/dispense/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/dispense/dispensing.py
--rw-r--r--   0 erikvw     (501) staff       (20)      806 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/dosage_per_day.py
--rw-r--r--   0 erikvw     (501) staff       (20)      351 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/exceptions.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.969294 edc-pharmacy-0.1.8/edc_pharmacy/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      779 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1224 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/dispensing_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      598 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/dosage_guideline_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      172 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/formulation_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      157 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/labels_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      169 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_lot_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      184 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_order_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      190 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_product_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      220 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_stock_create_labels_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      184 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_stock_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      211 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/medication_stock_receiving_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      178 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/return_history_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      696 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/rx_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/forms/rx_refill_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1177 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.970542 edc-pharmacy-0.1.8/edc_pharmacy/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)   166761 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.8/edc_pharmacy/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.8/edc_pharmacy/migrations/0002_alter_medication_unique_together.py
--rw-r--r--   0 erikvw     (501) staff       (20)      423 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/migrations/0003_alter_rxrefill_unique_together.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1754 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/migrations/0004_auto_20220414_1741.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.8/edc_pharmacy/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.973005 edc-pharmacy-0.1.8/edc_pharmacy/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      939 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1594 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/dispensing_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2451 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/dosage_guideline.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1886 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/formulation.py
--rw-r--r--   0 erikvw     (501) staff       (20)      813 2021-11-16 21:15:22.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/list_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      935 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication.py
--rw-r--r--   0 erikvw     (501) staff       (20)      687 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication_lot.py
--rw-r--r--   0 erikvw     (501) staff       (20)      196 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication_order.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1686 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication_product.py
--rw-r--r--   0 erikvw     (501) staff       (20)      871 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication_stock.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication_stock_create_labels.py
--rw-r--r--   0 erikvw     (501) staff       (20)      933 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/medication_stock_receiving.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3817 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      152 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/proxy_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1499 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/return_history.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4338 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/rx.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4750 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/rx_refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/search_slug_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2684 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/models/subject.py
--rw-r--r--   0 erikvw     (501) staff       (20)      129 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/offline_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.973239 edc-pharmacy-0.1.8/edc_pharmacy/prescribe/
--rw-r--r--   0 erikvw     (501) staff       (20)       53 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/prescribe/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1551 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/prescribe/create_prescription.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.973887 edc-pharmacy-0.1.8/edc_pharmacy/refill/
--rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1249 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/create_next_refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)      888 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/create_refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)      328 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/delete_next_refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/get_active_refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1853 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4013 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/refill/refill_creator.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.958586 edc-pharmacy-0.1.8/edc_pharmacy/static/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.958700 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.973998 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/js/
--rw-r--r--   0 erikvw     (501) staff       (20)     1331 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/js/edc_pharma.js
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.975080 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/
--rw-r--r--   0 erikvw     (501) staff       (20)      817 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_capsule.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)     1252 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_iv.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      826 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_suppositories.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      802 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_syrup.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_tablet.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      233 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/medication_stock_label.lbl
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/rando_pharmacy_label.lbl
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.958816 edc-pharmacy-0.1.8/edc_pharmacy/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.958869 edc-pharmacy-0.1.8/edc_pharmacy/templates/edc_pharmacy/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.975209 edc-pharmacy-0.1.8/edc_pharmacy/templates/edc_pharmacy/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)      410 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/templates/edc_pharmacy/bootstrap3/rx_refill_description.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.975403 edc-pharmacy-0.1.8/edc_pharmacy/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.8/edc_pharmacy/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      434 2021-10-12 04:57:02.000000 edc-pharmacy-0.1.8/edc_pharmacy/templatetags/edc_pharmacy_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.975745 edc-pharmacy-0.1.8/edc_pharmacy/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       61 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1087 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.976487 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4673 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_dispense.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4694 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_dosage_calculation.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5126 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_prescription.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10125 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_refill.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6760 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_study_medication_crf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1496 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.8/edc_pharmacy/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)      282 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.8/edc_pharmacy/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 00:43:03.963752 edc-pharmacy-0.1.8/edc_pharmacy.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1747 2022-04-15 00:43:03.000000 edc-pharmacy-0.1.8/edc_pharmacy.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     4695 2022-04-15 00:43:03.000000 edc-pharmacy-0.1.8/edc_pharmacy.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-04-15 00:43:03.000000 edc-pharmacy-0.1.8/edc_pharmacy.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:10:42.000000 edc-pharmacy-0.1.8/edc_pharmacy.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       13 2022-04-15 00:43:03.000000 edc-pharmacy-0.1.8/edc_pharmacy.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1003 2020-03-13 03:26:28.000000 edc-pharmacy-0.1.8/requirements.tests.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-06 01:25:23.000000 edc-pharmacy-0.1.8/requirements.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      188 2022-04-15 00:43:03.976879 edc-pharmacy-0.1.8/setup.cfg
--rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.8/setup.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.331037 edc-pharmacy-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)    18046 2020-03-04 23:10:42.000000 edc-pharmacy-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      207 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1747 2022-04-15 14:57:37.331107 edc-pharmacy-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      883 2020-03-13 03:26:28.000000 edc-pharmacy-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.316518 edc-pharmacy-0.1.9/edc_pharmacy/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.9/edc_pharmacy/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      761 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/action_items.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.319686 edc-pharmacy-0.1.9/edc_pharmacy/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      868 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.319949 edc-pharmacy-0.1.9/edc_pharmacy/admin/actions/
+-rw-r--r--   0 erikvw     (501) staff       (20)       62 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/actions/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1679 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/actions/print_stock_labels.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      661 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/autocomplete_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2211 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/dispensing_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      952 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/dosage_guideline_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1145 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/formulation_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1763 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/labels_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      834 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/list_model_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      685 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      940 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_lot_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3030 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_order_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1268 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_product_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1212 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_stock_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1550 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_stock_create_labels_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1411 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_stock_receiving_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      571 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/model_admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1644 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/return_history_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2466 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/rx_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6558 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin/rx_refill_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1897 2021-05-05 19:47:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      200 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      762 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/approve_prescription.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      221 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      636 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      495 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      477 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.320252 edc-pharmacy-0.1.9/edc_pharmacy/dispense/
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/dispense/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/dispense/dispensing.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      806 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/dosage_per_day.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      452 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/exceptions.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.322805 edc-pharmacy-0.1.9/edc_pharmacy/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      779 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1224 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/dispensing_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      598 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/dosage_guideline_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      172 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/formulation_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      157 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/labels_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      169 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_lot_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      184 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_order_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      190 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_product_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      220 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_stock_create_labels_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      184 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_stock_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      211 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/medication_stock_receiving_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      178 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/return_history_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      696 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/rx_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/forms/rx_refill_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1177 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.324450 edc-pharmacy-0.1.9/edc_pharmacy/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)   166761 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.9/edc_pharmacy/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      358 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.9/edc_pharmacy/migrations/0002_alter_medication_unique_together.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      423 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/migrations/0003_alter_rxrefill_unique_together.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1754 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/migrations/0004_auto_20220414_1741.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/migrations/0005_alter_rx_managers.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:11:39.000000 edc-pharmacy-0.1.9/edc_pharmacy/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.327223 edc-pharmacy-0.1.9/edc_pharmacy/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      939 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1594 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/dispensing_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2451 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/dosage_guideline.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1886 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/formulation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      813 2021-11-16 21:15:22.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/list_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      935 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      687 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication_lot.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      196 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication_order.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1686 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication_product.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      871 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication_stock.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication_stock_create_labels.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      933 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/medication_stock_receiving.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3795 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      152 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/proxy_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1499 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/return_history.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4338 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/rx.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4750 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/rx_refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/search_slug_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2684 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/models/subject.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      129 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/offline_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.327468 edc-pharmacy-0.1.9/edc_pharmacy/prescribe/
+-rw-r--r--   0 erikvw     (501) staff       (20)       53 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/prescribe/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1551 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/prescribe/create_prescription.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.328322 edc-pharmacy-0.1.9/edc_pharmacy/refill/
+-rw-r--r--   0 erikvw     (501) staff       (20)      231 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1249 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/create_next_refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      860 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/create_refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      328 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/delete_next_refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/get_active_refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1853 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4932 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/refill/refill_creator.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.312159 edc-pharmacy-0.1.9/edc_pharmacy/static/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.312251 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.328429 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/js/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1331 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/js/edc_pharma.js
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.329496 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/
+-rw-r--r--   0 erikvw     (501) staff       (20)      817 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_capsule.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)     1252 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_iv.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      826 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_suppositories.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      802 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_syrup.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_tablet.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      233 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/medication_stock_label.lbl
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/rando_pharmacy_label.lbl
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.312356 edc-pharmacy-0.1.9/edc_pharmacy/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.312397 edc-pharmacy-0.1.9/edc_pharmacy/templates/edc_pharmacy/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.329633 edc-pharmacy-0.1.9/edc_pharmacy/templates/edc_pharmacy/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)      410 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/templates/edc_pharmacy/bootstrap3/rx_refill_description.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.329831 edc-pharmacy-0.1.9/edc_pharmacy/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-10-12 04:57:01.000000 edc-pharmacy-0.1.9/edc_pharmacy/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      434 2021-10-12 04:57:02.000000 edc-pharmacy-0.1.9/edc_pharmacy/templatetags/edc_pharmacy_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.330193 edc-pharmacy-0.1.9/edc_pharmacy/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       61 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1087 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.330940 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4673 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_dispense.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4694 2022-03-07 00:52:46.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_dosage_calculation.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5061 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_prescription.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10163 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_refill.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9409 2022-04-15 14:57:28.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_study_medication_crf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1496 2021-11-19 00:52:31.000000 edc-pharmacy-0.1.9/edc_pharmacy/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      282 2020-03-04 23:11:40.000000 edc-pharmacy-0.1.9/edc_pharmacy/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-15 14:57:37.317176 edc-pharmacy-0.1.9/edc_pharmacy.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1747 2022-04-15 14:57:37.000000 edc-pharmacy-0.1.9/edc_pharmacy.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     4745 2022-04-15 14:57:37.000000 edc-pharmacy-0.1.9/edc_pharmacy.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-04-15 14:57:37.000000 edc-pharmacy-0.1.9/edc_pharmacy.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:10:42.000000 edc-pharmacy-0.1.9/edc_pharmacy.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       13 2022-04-15 14:57:37.000000 edc-pharmacy-0.1.9/edc_pharmacy.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1003 2020-03-13 03:26:28.000000 edc-pharmacy-0.1.9/requirements.tests.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-06 01:25:23.000000 edc-pharmacy-0.1.9/requirements.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      188 2022-04-15 14:57:37.331334 edc-pharmacy-0.1.9/setup.cfg
+-rw-r--r--   0 erikvw     (501) staff       (20)     1638 2022-04-15 00:42:54.000000 edc-pharmacy-0.1.9/setup.py
```

### Comparing `edc-pharmacy-0.1.8/LICENSE` & `edc-pharmacy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/PKG-INFO` & `edc-pharmacy-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-pharmacy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pharmacy module for clinicedc/edc projects
 Home-page: http://github.com/clinicedc/edc-pharmacy
 Author: Tshepiso Setsiba
 Author-email: ew2789@gmail.com
 Maintainer: Erik van Widenfelt
 License: GPL license, see LICENSE
 Keywords: django edc edc-pharmacy
```

### Comparing `edc-pharmacy-0.1.8/README.rst` & `edc-pharmacy-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/action_items.py` & `edc-pharmacy-0.1.9/edc_pharmacy/action_items.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/__init__.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/actions/print_stock_labels.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/actions/print_stock_labels.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/autocomplete_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/autocomplete_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/dispensing_history_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/dispensing_history_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/dosage_guideline_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/dosage_guideline_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/formulation_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/formulation_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/labels_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/labels_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/list_model_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/list_model_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_lot_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_lot_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_order_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_order_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_product_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_product_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_stock_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_stock_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_stock_create_labels_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_stock_create_labels_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/medication_stock_receiving_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/medication_stock_receiving_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/model_admin_mixin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/model_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/return_history_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/return_history_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/rx_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/rx_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin/rx_refill_admin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin/rx_refill_admin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/admin_mixin.py` & `edc-pharmacy-0.1.9/edc_pharmacy/admin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/approve_prescription.py` & `edc-pharmacy-0.1.9/edc_pharmacy/approve_prescription.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/auth_objects.py` & `edc-pharmacy-0.1.9/edc_pharmacy/auth_objects.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/auths.py` & `edc-pharmacy-0.1.9/edc_pharmacy/auths.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/dispense/dispensing.py` & `edc-pharmacy-0.1.9/edc_pharmacy/dispense/dispensing.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/dosage_per_day.py` & `edc-pharmacy-0.1.9/edc_pharmacy/dosage_per_day.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/forms/__init__.py` & `edc-pharmacy-0.1.9/edc_pharmacy/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/forms/dispensing_history_form.py` & `edc-pharmacy-0.1.9/edc_pharmacy/forms/dispensing_history_form.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/forms/dosage_guideline_form.py` & `edc-pharmacy-0.1.9/edc_pharmacy/forms/dosage_guideline_form.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/forms/rx_form.py` & `edc-pharmacy-0.1.9/edc_pharmacy/forms/rx_form.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/list_data.py` & `edc-pharmacy-0.1.9/edc_pharmacy/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/migrations/0001_initial.py` & `edc-pharmacy-0.1.9/edc_pharmacy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/migrations/0004_auto_20220414_1741.py` & `edc-pharmacy-0.1.9/edc_pharmacy/migrations/0004_auto_20220414_1741.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/__init__.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/dispensing_history.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/dispensing_history.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/dosage_guideline.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/dosage_guideline.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/formulation.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/formulation.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/list_models.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/list_models.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/medication.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/medication.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/medication_lot.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/medication_lot.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/medication_product.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/medication_product.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/medication_stock.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/medication_stock.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/medication_stock_create_labels.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/medication_stock_create_labels.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/medication_stock_receiving.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/medication_stock_receiving.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/model_mixins.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/model_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .medication_stock import MedicationStock
 
 
 class StudyMedicationRefillModelMixin(models.Model):
 
     """Declare with field subject_visit using a CRF model mixin"""
 
-    refill_date = models.DateField(null=True, blank=False)
+    refill_date = models.DateField()
 
     dosage_guideline = models.ForeignKey(
         DosageGuideline, on_delete=PROTECT, null=True, blank=False
     )
 
     formulation = models.ForeignKey(
         Formulation, on_delete=PROTECT, null=True, blank=False
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/return_history.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/return_history.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/rx.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/rx.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/rx_refill.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/rx_refill.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/models/signals.py` & `edc-pharmacy-0.1.9/edc_pharmacy/models/signals.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/prescribe/create_prescription.py` & `edc-pharmacy-0.1.9/edc_pharmacy/prescribe/create_prescription.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/refill/create_next_refill.py` & `edc-pharmacy-0.1.9/edc_pharmacy/refill/create_next_refill.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/refill/create_refill.py` & `edc-pharmacy-0.1.9/edc_pharmacy/refill/create_refill.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if instance.subject_visit.appointment.next:
         number_of_days = (
             instance.subject_visit.appointment.next.appt_datetime
             - instance.subject_visit.appointment.appt_datetime
         ).days
     RefillCreator(
         subject_identifier=instance.subject_visit.subject_identifier,
-        refill_date=instance.subject_visit.appointment.appt_datetime,
+        refill_date=instance.refill_date,
         visit_code=instance.subject_visit.appointment.visit_code,
         visit_code_sequence=instance.subject_visit.appointment.visit_code_sequence,
         number_of_days=number_of_days,
         dosage_guideline=instance.dosage_guideline,
         formulation=instance.formulation,
         make_active=True,
     )
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/refill/refill.py` & `edc-pharmacy-0.1.9/edc_pharmacy/refill/refill.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/refill/refill_creator.py` & `edc-pharmacy-0.1.9/edc_pharmacy/refill/refill_creator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from datetime import date, datetime
 from typing import Any, Optional, Union
 
 import arrow
+from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import IntegrityError, models, transaction
+from edc_utils import convert_php_dateformat
 
-from ..exceptions import PrescriptionError, RefillAlreadyExists
+from ..exceptions import (
+    PrescriptionError,
+    PrescriptionExpired,
+    PrescriptionNotStarted,
+    RefillAlreadyExists,
+)
 from ..models import Rx, RxRefill
 from .refill import Refill
 
 
 def convert_to_utc_date(dte: Union[datetime, date]) -> date:
     try:
         dt = dte.date()
@@ -32,15 +39,16 @@
         make_active: Optional[bool] = None,
         force_active: Optional[bool] = None,
         **kwargs,
     ):
         """Creates a refill.
 
         :type instance: model instance with other
-                        attrs (visit_code, ...)
+                        attrs (visit_code, ...),
+                        e.g. study medication CRF
         """
         super().__init__(**kwargs)
         if instance:
             self.subject_identifier = instance.get_subject_identifier()
             self.visit_code = instance.visit_code
             self.visit_code_sequence = instance.visit_code_sequence
             self.refill_date = convert_to_utc_date(instance.refill_date)
@@ -89,21 +97,35 @@
 
     @property
     def _rx(self) -> Any:
         """Returns Rx model instance else raises PrescriptionError"""
         opts = dict(
             subject_identifier=self.subject_identifier,
             medications__in=[self.formulation.medication],
-            rx_date__lte=self.refill_date,
         )
         try:
             obj = Rx.objects.get(**opts)
         except ObjectDoesNotExist:
             raise PrescriptionError(
-                f"Subject does not have a valid prescription. Got {opts}."
+                f"Subject does not have a prescription. Got {opts}."
             )
         else:
-            if obj.rx_expiration_date and self.refill_date > obj.rx_expiration_date:
-                raise PrescriptionError(
-                    f"Subject prescription has expired. Got {self.subject_identifier} on {obj.rx_expiration_date}."
+            refill_date = self.refill_date.strftime(
+                convert_php_dateformat(settings.DATETIME_FORMAT)
+            )
+            if self.refill_date < obj.rx_date:
+                rx_date = obj.rx_date.strftime(
+                    convert_php_dateformat(settings.DATETIME_FORMAT)
+                )
+                raise PrescriptionNotStarted(
+                    f"Subject's prescription not started. Starts on {rx_date}. "
+                    f"Got {self.subject_identifier} attempting refill on {refill_date}."
+                )
+            elif obj.rx_expiration_date and self.refill_date > obj.rx_expiration_date:
+                rx_expiration_date = obj.rx_expiration_date.strftime(
+                    convert_php_dateformat(settings.DATETIME_FORMAT)
+                )
+                raise PrescriptionExpired(
+                    f"Subject prescription has expired. Expired on {rx_expiration_date}. "
+                    f"Got {self.subject_identifier} attempting refill on {refill_date}."
                 )
         return obj
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/js/edc_pharma.js` & `edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/js/edc_pharma.js`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_capsule.lbl` & `edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_capsule.lbl`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_iv.lbl` & `edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_iv.lbl`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_suppositories.lbl` & `edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_suppositories.lbl`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_syrup.lbl` & `edc-pharmacy-0.1.9/edc_pharmacy/static/edc_pharmacy/label_templates/dispense_label_syrup.lbl`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/models.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/models.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_dispense.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_dispense.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_dosage_calculation.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_dosage_calculation.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_prescription.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_prescription.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,21 +88,20 @@
             subject_identifier=self.registered_subject.subject_identifier,
             report_datetime=self.registered_subject.registration_datetime,
             medications=[self.medication],
         )
         rx = Rx.objects.get(
             subject_identifier=self.registered_subject.subject_identifier
         )
-        with self.assertRaises(PrescriptionAlreadyExists) as cm:
+        with self.assertRaises(PrescriptionAlreadyExists):
             create_prescription(
                 subject_identifier=self.registered_subject.subject_identifier,
                 report_datetime=self.registered_subject.registration_datetime,
                 medications=[self.medication],
             )
-        self.assertIn(rx.rx_identifier, str(cm.exception))
 
     def test_create_prescripition_from_func_for_rct(self):
         randomizer = site_randomizers.get("default")
         randomizer.import_list(verbose=False, sid_count_for_tests=3)
         site_randomizers.randomize(
             "default",
             subject_identifier=self.registered_subject.subject_identifier,
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_refill.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_refill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dateutil.relativedelta import relativedelta
 from django.test import TestCase, tag
 from edc_constants.constants import FEMALE
-from edc_pharmacy.exceptions import PrescriptionError
+from edc_pharmacy.exceptions import PrescriptionError, PrescriptionNotStarted
 from edc_pharmacy.models import (
     DosageGuideline,
     Formulation,
     FormulationType,
     FrequencyUnits,
     Medication,
     Route,
@@ -126,20 +126,20 @@
             formulation=self.formulation,
         )
         self.assertTrue(refill_creator.refill.rx)
 
     def test_refill_raises_on_gets_rx(self):
         """Assert raises if refill date before Rx"""
         self.assertRaises(
-            PrescriptionError,
+            PrescriptionNotStarted,
             RefillCreator,
             subject_identifier=self.subject_identifier,
             visit_code="1000",
             visit_code_sequence=0,
-            refill_date=get_utcnow() - relativedelta(years=1),
+            refill_date=(get_utcnow() - relativedelta(years=1)).date(),
             number_of_days=32,
             dosage_guideline=self.dosage_guideline,
             formulation=self.formulation,
         )
 
     def test_refill_create_and_no_active_refill(self):
         refill_creator = RefillCreator(
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/tests/test_study_medication_crf.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/tests/test_study_medication_crf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from dateutil.relativedelta import relativedelta
 from django.db.models.signals import pre_save
-from django.test import TestCase, tag
+from django.test import TestCase
 from edc_appointment.creators import AppointmentsCreator
 from edc_appointment.models import Appointment
 from edc_constants.constants import NO, YES
 from edc_facility import import_holidays
-from edc_pharmacy.exceptions import NextRefillError
+from edc_pharmacy.exceptions import (
+    NextRefillError,
+    PrescriptionExpired,
+    PrescriptionNotStarted,
+)
 from edc_pharmacy.models import (
     DosageGuideline,
     Formulation,
     FormulationType,
     FrequencyUnits,
     Medication,
     MedicationOrder,
@@ -34,23 +39,26 @@
 
     def setUp(self) -> None:
         site_visit_schedules._registry = {}
         site_visit_schedules.loaded = False
 
         site_visit_schedules.register(visit_schedule)
         self.subject_identifier = "12345"
-        RegisteredSubject.objects.create(subject_identifier=self.subject_identifier)
-        report_datetime = get_utcnow()
+        RegisteredSubject.objects.create(
+            subject_identifier=self.subject_identifier,
+            registration_datetime=get_utcnow() - relativedelta(years=5),
+        )
+        self.registration_datetime = get_utcnow() - relativedelta(years=5)
         creator = AppointmentsCreator(
             subject_identifier=self.subject_identifier,
             visit_schedule=visit_schedule,
             schedule=schedule,
-            report_datetime=report_datetime,
+            report_datetime=self.registration_datetime,
         )
-        creator.create_appointments(base_appt_datetime=report_datetime)
+        creator.create_appointments(base_appt_datetime=self.registration_datetime)
 
         self.assertGreater(
             Appointment.objects.filter(
                 subject_identifier=self.subject_identifier
             ).count(),
             0,
         )
@@ -82,33 +90,90 @@
             frequency=2,
             frequency_units=FrequencyUnits.objects.get(name="day"),
         )
 
         self.rx = Rx.objects.create(
             subject_identifier=self.subject_identifier,
             weight_in_kgs=40,
-            report_datetime=report_datetime,
+            report_datetime=self.registration_datetime,
+            rx_date=self.registration_datetime.date(),
         )
         self.rx.medications.add(self.medication)
 
     def test_ok(self):
         appointment = Appointment.objects.all().order_by("timepoint")[0]
         subject_visit = SubjectVisit.objects.create(
-            appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
+            appointment=appointment,
+            report_datetime=appointment.appt_datetime,
+            reason=SCHEDULED,
         )
-        obj = StudyMedication.objects.create(
+
+        obj = StudyMedication(
             subject_visit=subject_visit,
+            refill_date=subject_visit.report_datetime,
             dosage_guideline=self.dosage_guideline_100,
             formulation=self.formulation,
             order_next=YES,
             next_dosage_guideline=self.dosage_guideline_200,
             next_formulation=self.formulation,
         )
+        obj.save()
+
+        # calc num of days until next visit
+        number_of_days = (
+            obj.subject_visit.appointment.next.appt_datetime
+            - obj.subject_visit.appointment.appt_datetime
+        ).days
+
         self.assertIsNotNone(obj.number_of_days)
-        self.assertEqual(obj.number_of_days, 7)
+        self.assertEqual(obj.number_of_days, number_of_days)
+        self.assertGreater(obj.number_of_days, 0)
+
+    def test_refill_before_rx(self):
+        appointment = Appointment.objects.all().order_by("timepoint")[0]
+        subject_visit = SubjectVisit.objects.create(
+            appointment=appointment,
+            report_datetime=appointment.appt_datetime,
+            reason=SCHEDULED,
+        )
+
+        obj = StudyMedication(
+            subject_visit=subject_visit,
+            refill_date=self.rx.rx_date - relativedelta(years=1),
+            dosage_guideline=self.dosage_guideline_100,
+            formulation=self.formulation,
+            order_next=YES,
+            next_dosage_guideline=self.dosage_guideline_200,
+            next_formulation=self.formulation,
+        )
+        with self.assertRaises(PrescriptionNotStarted):
+            obj.save()
+
+    def test_refill_for_expired_rx(self):
+        appointment = Appointment.objects.all().order_by("timepoint")[0]
+        subject_visit = SubjectVisit.objects.create(
+            appointment=appointment,
+            report_datetime=appointment.appt_datetime,
+            reason=SCHEDULED,
+        )
+        self.rx.rx_expiration_date = subject_visit.report_datetime
+        self.rx.save()
+        self.rx.refresh_from_db()
+
+        obj = StudyMedication(
+            subject_visit=subject_visit,
+            refill_date=subject_visit.report_datetime + relativedelta(years=1),
+            dosage_guideline=self.dosage_guideline_100,
+            formulation=self.formulation,
+            order_next=YES,
+            next_dosage_guideline=self.dosage_guideline_200,
+            next_formulation=self.formulation,
+        )
+        with self.assertRaises(PrescriptionExpired):
+            obj.save()
 
     def test_for_all_appts(self):
         """Assert for all appointments.
 
         Captures exception at last appointment where "next" is none
         """
         for appointment in Appointment.objects.all().order_by("timepoint"):
@@ -118,31 +183,34 @@
                 reason=SCHEDULED,
             )
             if not appointment.next:
                 self.assertRaises(
                     NextRefillError,
                     StudyMedication.objects.create,
                     subject_visit=subject_visit,
+                    refill_date=subject_visit.report_datetime,
                     dosage_guideline=self.dosage_guideline_100,
                     formulation=self.formulation,
                     order_next=YES,
                     next_dosage_guideline=self.dosage_guideline_100,
                     next_formulation=self.formulation,
                 )
                 StudyMedication.objects.create(
                     subject_visit=subject_visit,
+                    refill_date=subject_visit.report_datetime,
                     dosage_guideline=self.dosage_guideline_100,
                     formulation=self.formulation,
                     next_dosage_guideline=None,
                     next_formulation=None,
                     order_next=NO,
                 )
             else:
                 StudyMedication.objects.create(
                     subject_visit=subject_visit,
+                    refill_date=subject_visit.report_datetime,
                     dosage_guideline=self.dosage_guideline_100,
                     formulation=self.formulation,
                     order_next=YES,
                     next_dosage_guideline=self.dosage_guideline_100,
                     next_formulation=self.formulation,
                 )
 
@@ -150,14 +218,15 @@
         appointment = Appointment.objects.all().order_by("timepoint")[0]
         subject_visit = SubjectVisit.objects.create(
             appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
         self.assertEqual(RxRefill.objects.all().count(), 0)
         StudyMedication.objects.create(
             subject_visit=subject_visit,
+            refill_date=subject_visit.report_datetime,
             dosage_guideline=self.dosage_guideline_100,
             formulation=self.formulation,
             order_next=YES,
             next_dosage_guideline=self.dosage_guideline_200,
             next_formulation=self.formulation,
         )
         self.assertEqual(RxRefill.objects.all().count(), 2)
@@ -165,13 +234,14 @@
     def test_refill_creates_next_refill_for_next_dosage(self):
         appointment = Appointment.objects.all().order_by("timepoint")[0]
         subject_visit = SubjectVisit.objects.create(
             appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
         StudyMedication.objects.create(
             subject_visit=subject_visit,
+            refill_date=subject_visit.report_datetime,
             dosage_guideline=self.dosage_guideline_100,
             formulation=self.formulation,
             order_next=YES,
             next_dosage_guideline=self.dosage_guideline_200,
             next_formulation=self.formulation,
         )
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy/tests/visit_schedule.py` & `edc-pharmacy-0.1.9/edc_pharmacy/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy.egg-info/PKG-INFO` & `edc-pharmacy-0.1.9/edc_pharmacy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-pharmacy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pharmacy module for clinicedc/edc projects
 Home-page: http://github.com/clinicedc/edc-pharmacy
 Author: Tshepiso Setsiba
 Author-email: ew2789@gmail.com
 Maintainer: Erik van Widenfelt
 License: GPL license, see LICENSE
 Keywords: django edc edc-pharmacy
```

### Comparing `edc-pharmacy-0.1.8/edc_pharmacy.egg-info/SOURCES.txt` & `edc-pharmacy-0.1.9/edc_pharmacy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 edc_pharmacy/forms/return_history_form.py
 edc_pharmacy/forms/rx_form.py
 edc_pharmacy/forms/rx_refill_form.py
 edc_pharmacy/migrations/0001_initial.py
 edc_pharmacy/migrations/0002_alter_medication_unique_together.py
 edc_pharmacy/migrations/0003_alter_rxrefill_unique_together.py
 edc_pharmacy/migrations/0004_auto_20220414_1741.py
+edc_pharmacy/migrations/0005_alter_rx_managers.py
 edc_pharmacy/migrations/__init__.py
 edc_pharmacy/models/__init__.py
 edc_pharmacy/models/dispensing_history.py
 edc_pharmacy/models/dosage_guideline.py
 edc_pharmacy/models/formulation.py
 edc_pharmacy/models/list_models.py
 edc_pharmacy/models/medication.py
```

### Comparing `edc-pharmacy-0.1.8/requirements.tests.txt` & `edc-pharmacy-0.1.9/requirements.tests.txt`

 * *Files identical despite different names*

### Comparing `edc-pharmacy-0.1.8/setup.py` & `edc-pharmacy-0.1.9/setup.py`

 * *Files identical despite different names*

