# Comparing `tmp/fittings-2.0.1.tar.gz` & `tmp/fittings-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fittings-2.0.1.tar", last modified: Fri Apr 21 05:03:00 2023, max compression
+gzip compressed data, was "dist/fittings-2.0.2.tar", last modified: Sat Apr 22 06:08:29 2023, max compression
```

## Comparing `fittings-2.0.1.tar` & `fittings-2.0.2.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-21 05:03:00.000000 fittings-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-21 05:02:49.000000 fittings-2.0.1/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/cogs/
--rw-rw-rw-   0 root         (0) root         (0)     8433 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/cogs/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templates/fittings/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/edit_fit.html
--rw-rw-rw-   0 root         (0) root         (0)    35122 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_fit.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templates/fittings/bundles/
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/multi-select-css.html
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/jquery.quicksearch-js.html
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/multi-select-js.html
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/slim-select-css.html
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/clipboard-js.html
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/bundles/slim-select-js.html
--rw-rw-rw-   0 root         (0) root         (0)     4517 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_all_categories.html
--rw-rw-rw-   0 root         (0) root         (0)     3705 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     6518 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3384 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_all_fits.html
--rw-rw-rw-   0 root         (0) root         (0)     5852 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/edit_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6080 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/add_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/base.html
--rw-rw-rw-   0 root         (0) root         (0)     8161 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/view_category.html
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/add_fit.html
--rw-rw-rw-   0 root         (0) root         (0)     6133 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/create_category.html
--rw-rw-rw-   0 root         (0) root         (0)     6419 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templates/fittings/edit_doctrine.html
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/management/commands/fittings_preload_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/
--rw-rw-rw-   0 root         (0) root         (0)     7759 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/zh.json
--rw-rw-rw-   0 root         (0) root         (0)     8110 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/it-IT.json
--rw-rw-rw-   0 root         (0) root         (0)     7731 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/en-GB.json
--rw-rw-rw-   0 root         (0) root         (0)     8452 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/fr-FR.json
--rw-rw-rw-   0 root         (0) root         (0)    10517 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/ru.json
--rw-rw-rw-   0 root         (0) root         (0)     8241 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/es-ES.json
--rw-rw-rw-   0 root         (0) root         (0)     2988 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/ja.json
--rw-rw-rw-   0 root         (0) root         (0)     7318 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/uk.json
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/ko.json
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/dt-i18n/de-DE.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/img/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/
--rw-rw-rw-   0 root         (0) root         (0)     8580 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/7m.png
--rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0l.png
--rw-rw-rw-   0 root         (0) root         (0)     5888 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5l.png
--rw-rw-rw-   0 root         (0) root         (0)    43642 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/h.png
--rw-rw-rw-   0 root         (0) root         (0)     7439 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/6m.png
--rw-rw-rw-   0 root         (0) root         (0)     7399 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5s.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/r.png
--rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3h.png
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2h.png
--rw-rw-rw-   0 root         (0) root         (0)    16840 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/circle.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/l.png
--rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3r.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/m.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0r.png
--rw-rw-rw-   0 root         (0) root         (0)     3720 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0s.png
--rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5h.png
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4l.png
--rw-rw-rw-   0 root         (0) root         (0)    33523 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/dustwheel.png
--rw-rw-rw-   0 root         (0) root         (0)     8972 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/8l.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/0h.png
--rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4s.png
--rw-rw-rw-   0 root         (0) root         (0)     6270 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/5m.png
--rw-rw-rw-   0 root         (0) root         (0)    38343 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_default.png
--rw-rw-rw-   0 root         (0) root         (0)    43560 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_blue.png
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/working.jpg
--rw-rw-rw-   0 root         (0) root         (0)     8067 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/7l.png
--rw-rw-rw-   0 root         (0) root         (0)     2512 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1r.png
--rw-rw-rw-   0 root         (0) root         (0)     8879 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/noship.png
--rw-rw-rw-   0 root         (0) root         (0)     1976 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1l.png
--rw-rw-rw-   0 root         (0) root         (0)     5309 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/4h.png
--rw-rw-rw-   0 root         (0) root         (0)     8288 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/7h.png
--rw-rw-rw-   0 root         (0) root         (0)     3523 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/3l.png
--rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/6h.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1h.png
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/1m.png
--rw-rw-rw-   0 root         (0) root         (0)    42868 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_revelations.png
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/blank.png
--rw-rw-rw-   0 root         (0) root         (0)     2570 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2l.png
--rw-rw-rw-   0 root         (0) root         (0)     3497 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/2r.png
--rw-rw-rw-   0 root         (0) root         (0)     7014 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/6l.png
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/error.jpg
--rw-rw-rw-   0 root         (0) root         (0)    42833 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_darkred.png
--rw-rw-rw-   0 root         (0) root         (0)     9541 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/8m.png
--rw-rw-rw-   0 root         (0) root         (0)     9276 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/img/pannel/8h.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/
--rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/
--rw-rw-rw-   0 root         (0) root         (0)    19224 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    10904 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery,quicksearch.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/
--rw-rw-rw-   0 root         (0) root         (0)     6240 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css
--rw-rw-rw-   0 root         (0) root         (0)    35553 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6647 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/models.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/tests.py
--rw-rw-rw-   0 root         (0) root         (0)    24902 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/views.py
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0005_unicategory.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0003_remove_type_description_not_null.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0008_auto_20200605_0736.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0014_serverversion.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0010_auto_20200718_2227.py
--rw-rw-rw-   0 root         (0) root         (0)     6132 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0011_auto_20200815_2022.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0012_typehistory.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0013_alter_doctrine_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0007_auto_20200605_0735.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0004_add_item_category_and_group.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0009_auto_20200605_2117.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0002_add_dgm_unique_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/migrations/0006_auto_20200605_0724.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10229 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10085 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    10038 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13534 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5263 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13034 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templatetags/filters.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/templatetags/tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-21 05:02:49.000000 fittings-2.0.1/fittings/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-21 05:02:49.000000 fittings-2.0.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1645 2023-04-21 05:02:49.000000 fittings-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 05:03:00.000000 fittings-2.0.1/fittings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5574 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6120 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 05:02:59.000000 fittings-2.0.1/fittings.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-21 05:02:49.000000 fittings-2.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-21 05:03:00.000000 fittings-2.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-22 06:08:29.000000 fittings-2.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2023-04-22 06:08:18.000000 fittings-2.0.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/cogs/
+-rw-rw-rw-   0 root         (0) root         (0)     8423 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/cogs/fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     9979 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/templates/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)     2414 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/edit_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)    35061 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/view_fit.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/templates/fittings/bundles/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/bundles/multi-select-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/bundles/jquery.quicksearch-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/bundles/multi-select-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      359 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/bundles/slim-select-css.html
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/bundles/clipboard-js.html
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/bundles/slim-select-js.html
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/view_all_categories.html
+-rw-rw-rw-   0 root         (0) root         (0)     3776 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     6546 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/view_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3443 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/view_all_fits.html
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/edit_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6015 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/add_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     8300 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/view_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     2369 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/add_fit.html
+-rw-rw-rw-   0 root         (0) root         (0)     6129 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/create_category.html
+-rw-rw-rw-   0 root         (0) root         (0)     6411 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templates/fittings/edit_doctrine.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/providers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/management/commands/fittings_preload_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     7759 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/zh.json
+-rw-rw-rw-   0 root         (0) root         (0)     8110 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/it-IT.json
+-rw-rw-rw-   0 root         (0) root         (0)     7731 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/en-GB.json
+-rw-rw-rw-   0 root         (0) root         (0)     8452 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/fr-FR.json
+-rw-rw-rw-   0 root         (0) root         (0)    10517 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/ru.json
+-rw-rw-rw-   0 root         (0) root         (0)     8241 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/es-ES.json
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/ja.json
+-rw-rw-rw-   0 root         (0) root         (0)     7318 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/uk.json
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/ko.json
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/dt-i18n/de-DE.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/img/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/7m.png
+-rw-rw-rw-   0 root         (0) root         (0)     4956 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/4m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/0l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5888 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/5l.png
+-rw-rw-rw-   0 root         (0) root         (0)    43642 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/h.png
+-rw-rw-rw-   0 root         (0) root         (0)     7439 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/6m.png
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/5s.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/r.png
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/3h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/2h.png
+-rw-rw-rw-   0 root         (0) root         (0)    16840 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/circle.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/l.png
+-rw-rw-rw-   0 root         (0) root         (0)     4886 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/3r.png
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/m.png
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/2m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/0r.png
+-rw-rw-rw-   0 root         (0) root         (0)     3720 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/3m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/0m.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/0s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6109 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/5h.png
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/4l.png
+-rw-rw-rw-   0 root         (0) root         (0)    33523 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/dustwheel.png
+-rw-rw-rw-   0 root         (0) root         (0)     8972 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/8l.png
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/0h.png
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/4s.png
+-rw-rw-rw-   0 root         (0) root         (0)     6270 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/5m.png
+-rw-rw-rw-   0 root         (0) root         (0)    38343 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_default.png
+-rw-rw-rw-   0 root         (0) root         (0)    43560 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_blue.png
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/working.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     8067 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/7l.png
+-rw-rw-rw-   0 root         (0) root         (0)     2512 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/1r.png
+-rw-rw-rw-   0 root         (0) root         (0)     8879 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/noship.png
+-rw-rw-rw-   0 root         (0) root         (0)     1976 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/1l.png
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/4h.png
+-rw-rw-rw-   0 root         (0) root         (0)     8288 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/7h.png
+-rw-rw-rw-   0 root         (0) root         (0)     3523 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/3l.png
+-rw-rw-rw-   0 root         (0) root         (0)     7203 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/6h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/1h.png
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/1m.png
+-rw-rw-rw-   0 root         (0) root         (0)    42868 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_revelations.png
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/blank.png
+-rw-rw-rw-   0 root         (0) root         (0)     2570 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/2l.png
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/2r.png
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/6l.png
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/error.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    42833 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_darkred.png
+-rw-rw-rw-   0 root         (0) root         (0)     9541 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/8m.png
+-rw-rw-rw-   0 root         (0) root         (0)     9276 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/img/pannel/8h.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/clipboard.js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10753 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19224 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/jquery.quicksearch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10904 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery,quicksearch.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/slim-select/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/slim-select/1.26.0/
+-rw-rw-rw-   0 root         (0) root         (0)     6240 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css
+-rw-rw-rw-   0 root         (0) root         (0)    35553 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6647 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)    24838 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/views.py
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0005_unicategory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0003_remove_type_description_not_null.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0008_auto_20200605_0736.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0014_serverversion.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0010_auto_20200718_2227.py
+-rw-rw-rw-   0 root         (0) root         (0)     6132 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0011_auto_20200815_2022.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0012_typehistory.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0013_alter_doctrine_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0007_auto_20200605_0735.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0004_add_item_category_and_group.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0009_auto_20200605_2117.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0002_add_dgm_unique_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/migrations/0006_auto_20200605_0724.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10229 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10085 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    10038 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13534 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12224 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13034 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templatetags/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/templatetags/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-22 06:08:18.000000 fittings-2.0.2/fittings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-22 06:08:18.000000 fittings-2.0.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1645 2023-04-22 06:08:18.000000 fittings-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6120 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 06:08:29.000000 fittings-2.0.2/fittings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)     4554 2023-04-22 06:08:18.000000 fittings-2.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-22 06:08:29.000000 fittings-2.0.2/setup.cfg
```

### Comparing `fittings-2.0.1/PKG-INFO` & `fittings-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `fittings-2.0.1/LICENSE` & `fittings-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/auth_hooks.py` & `fittings-2.0.2/fittings/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/cogs/fittings.py` & `fittings-2.0.2/fittings/cogs/fittings.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 def fitting_details(fit_id):
     try:
         fit = Fitting.objects.get(id=fit_id)
     except ObjectDoesNotExist:
         embed = Embed(title="Fitting Not Found")
         return
 
-    embed = Embed(title=f"{fit.ship_type.type_name}: {fit.name}")
+    embed = Embed(title=f"{fit.ship_type.name}: {fit.name}")
     embed.set_thumbnail(
         url=f"https://images.evetech.net/types/{fit.ship_type_type_id}/render?size=128"
     )
     embed.description = fit.description
 
     doctrines_value = ''
     for doctrine in Doctrine.objects.filter(fittings=fit).values("name", "id"):
@@ -215,15 +215,15 @@
     embed.set_thumbnail(
         url=doctrine.icon_url
     )
     embed.description = doctrine.description
 
     for fit in doctrine.fittings.all():
         embed.add_field(
-            name=fit.ship_type.type_name,
+            name=fit.ship_type.name,
             value=f"[{fit.name}]({get_site_url()}/fittings/fit/{fit.id}/)"
         )
 
     embed.add_field(
         name="URL",
         value=f"{get_site_url()}/fittings/doctrine/{doctrine_id}/",
         inline=False
```

### Comparing `fittings-2.0.1/fittings/tasks.py` & `fittings-2.0.2/fittings/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,36 +140,43 @@
                     types.append(_get_type(line.strip()))
         return all(_type is not None and _type.eve_group.eve_category.id == 87 for _type in types)
 
 
 def _get_type(type_name):
     try:
         type_obj = EveType.objects.get(name=type_name)
+
+        return type_obj
     except:
         # If the type is not already in the db, then we have to resolve type_id before we have eveuniverse
         # create the object.
         c = esi.client
-        type_id = c.Universe.post_universe_ids(names=[type_name]).result()['inventory_types'][0]["id"]
-        type_obj = EveType.objects.get_or_create_esi(id=type_id,enabled_sections=[EveType.Section.DOGMAS])
-        type_obj = type_obj[0]
-    return type_obj
+        try:
+            type_id = c.Universe.post_universe_ids(names=[type_name]).result()['inventory_types'][0]["id"]
+            type_obj = EveType.objects.get_or_create_esi(id=type_id, enabled_sections=[EveType.Section.DOGMAS])
+            type_obj = type_obj[0]
+
+            return type_obj
+        except TypeError as e:
+            logger.error(f"Type ID for {type_name} not returned via ESI. Consider removing this from your fit.")
+            raise e
 
 
 @shared_task()
 def create_fitting_item(fit, item):
     count = None
     quantity = None
     if 'count' in item:
         count = item['count']
 
     type_obj = _get_type(item['name'])
 
     # Dogma Effects
     flags = {11: 'LoSlot', 12: 'HiSlot', 13: 'MedSlot', 2663: 'RigSlot', 3772: 'SubSystemSlot', 6306: 'ServiceSlot'}
-    effects = type_obj.dogma_effects.filter(effect_id__in=flags).values_list('eve_dogma_effect_id', flat=True)
+    effects = type_obj.dogma_effects.filter(eve_dogma_effect_id__in=flags).values_list('eve_dogma_effect_id', flat=True)
     effects = list(effects)
     if count is None:
         flag = item['section_name']
         quantity = item['quantity']
     # Check due to active drug from pyfa not showing quantities
     elif len(effects) == 0:
         flag = 'Cargo'
@@ -240,15 +247,15 @@
 
 
 @shared_task
 def update_fit(eft_text, fit_id, description=None):
     parsed_eft = EftParser(eft_text).parse()
     fit = Fitting.objects.get(id=fit_id)
 
-    if parsed_eft['ship'] != fit.ship_type.type_name:
+    if parsed_eft['ship'] != fit.ship_type.name:
         logger.info("Cannot update a fitting with different ship type")
         return
 
     logger.info("Updating Fit name: {parsed_eft['name']}, Type: {parsed_eft['ship']}")  
 
     FittingItem.objects.filter(fit__id=fit_id).delete()
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/edit_fit.html` & `fittings-2.0.2/fittings/templates/fittings/edit_fit.html`

 * *Files 1% similar despite different names*

```diff
@@ -27,23 +27,23 @@
                             {% csrf_token %}
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">{% translate "Description" %}</label>
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" maxlength="500" rows="3">{{ fit.description }}</textarea>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <div class="form-group" >
                                 <label for="eft" class="col-sm-2 control-label">{% translate "Fit" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <textarea class="form-control" name="eft" id="eft" rows="50">{{ fit.eft }}</textarea>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
-{% endblock %}
+{% endblock %}
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/view_fit.html` & `fittings-2.0.2/fittings/templates/fittings/view_fit.html`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         <div class="modal-dialog" role="document">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                     <h4 class="modal-title" id="modalTitle">{% translate "Are you sure?" %}</h4>
                 </div>
                 <div class="modal-body">
-                    <p style="white-space: pre-line">{% translate "Are you sure you wish to delete this fit?" %}
+                    <p style="white-space: pre-line;">{% translate "Are you sure you wish to delete this fit?" %}
 
                         <i><strong>{% translate "This action is permanent." %}</strong></i></p>
                 </div>
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">{% translate "No - Close" %}</button>
                     <a href="{% url 'fittings:delete_fit' fit.pk %}" type="button" class="btn btn-danger">{% translate "Yes - Delete" %}</a>
                 </div>
@@ -32,25 +32,25 @@
         <div class="modal-dialog" role="document">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                     <h4 class="modal-title" id="modalTitle">{{ fit.name }}</h4>
                 </div>
                 <div class="modal-body">
-                    <textarea style="width: 100%; height: 100%" rows="25" onclick="this.select()" readonly>{{ fit.eft }}</textarea>
+                    <textarea style="width: 100%; height: 100%;" rows="25" onclick="this.select()" readonly>{{ fit.eft }}</textarea>
                 </div>
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">{% translate "Close" %}</button>
                 </div>
             </div>
         </div>
     </div>
 
     {# modal end #}
-    <br />
+    <br>
     <div class="col-md-3">
         <div class="panel panel-primary">
             <div class="panel-heading">
                 {% translate "Fit Information" %}
                 {% if perms.fittings.manage %}
                 <span data-toggle="modal" data-target="#deleteModal">
                         <button class="btn btn-xs btn-danger" style="float: right; margin-left: 5px;" data-toggle="tooltip" data-placement="top" title="{% translate 'Delete Fit' %}"><span class="fa fas fa-times"></span> </button>
@@ -91,63 +91,63 @@
     <div class="col-md-9">
         <div class="panel panel-default">
             <div class="panel-heading"> {% translate "Fittings" %} </div>
             <div class="panel-body">
                 <div class="row">
                     <div class="col-sm-12 col-md-6 text-center">
                         <div id="Fitting_Panel" style="position: relative; height:398px; width:398px; z-index: 3; margin: 0 auto;" >
-                            <div id="mask" style="position:absolute; left: 0px; top: 0px; width:398px; height:398px; z-index:-1;">
-                                <img style="position:absolute; left: 0px; top: 0px;  height:398px; width:398px; border:0px" src="{% static 'fittings/img/pannel/tyrannis.png' %}" alt="" />
+                            <div id="mask" style="position:absolute; left: 0; top: 0; width:398px; height:398px; z-index:-1;">
+                                <img style="position:absolute; left: 0; top: 0;  height:398px; width:398px; border:0;" src="{% static 'fittings/img/pannel/tyrannis.png' %}" alt="">
                             </div>
 
-                            <div id="highx" style="position:absolute; left: 0px; top: 0px; width: 398px; height: 398px; z-index:-1;">
-                                <img src="/static/fittings/img/pannel/{{ slots.high }}h.png" alt="" style="border:0px;" />
+                            <div id="highx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
+                                <img src="/static/fittings/img/pannel/{{ slots.high }}h.png" alt="" style="border:0;">
                             </div>
                             <div id="high1" style="position:absolute; left:73px; top:60px; width:32px; height:32px;">{% if fitting.HiSlot0 %}<img src="{{ fitting.HiSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot0.item_name }}">{% endif %}</div>
                             <div id="high2" style="position:absolute; left:102px; top:42px; width:32px; height:32px;">{% if fitting.HiSlot1 %}<img src="{{ fitting.HiSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot1.item_name }}">{% endif %}</div>
                             <div id="high3" style="position:absolute; left:134px; top:27px; width:32px; height:32px;">{% if fitting.HiSlot2 %}<img src="{{ fitting.HiSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot2.item_name }}">{% endif %}</div>
                             <div id="high4" style="position:absolute; left:169px; top:21px; width:32px; height:32px;">{% if fitting.HiSlot3 %}<img src="{{ fitting.HiSlot3.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot3.item_name }}">{% endif %}</div>
                             <div id="high5" style="position:absolute; left:203px; top:22px; width:32px; height:32px;">{% if fitting.HiSlot4 %}<img src="{{ fitting.HiSlot4.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot4.item_name }}">{% endif %}</div>
                             <div id="high6" style="position:absolute; left:238px; top:30px; width:32px; height:32px;">{% if fitting.HiSlot5 %}<img src="{{ fitting.HiSlot5.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot5.item_name }}">{% endif %}</div>
                             <div id="high7" style="position:absolute; left:270px; top:45px; width:32px; height:32px;">{% if fitting.HiSlot6 %}<img src="{{ fitting.HiSlot6.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot6.item_name }}">{% endif %}</div>
                             <div id="high8" style="position:absolute; left:295px; top:64px; width:32px; height:32px;">{% if fitting.HiSlot7 %}<img src="{{ fitting.HiSlot7.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot7.item_name }}">{% endif %}</div>
 
-                            <div id="midx" style="position:absolute; left: 0px; top: 0px; width: 398px; height: 398px; z-index:-1;">
-                                <img src="/static/fittings/img/pannel/{{ slots.med }}m.png" alt="" style="border:0px;" />
+                            <div id="midx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
+                                <img src="/static/fittings/img/pannel/{{ slots.med }}m.png" alt="" style="border:0;">
                             </div>
                             <div id="mid1" style="position:absolute; left:26px; top:140px; width:32px; height:32px;">{% if fitting.MedSlot0 %}<img src="{{ fitting.MedSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot0.item_name }}">{% endif %}</div>
                             <div id="mid2" style="position:absolute; left:24px; top:176px; width:32px; height:32px;">{% if fitting.MedSlot1 %}<img src="{{ fitting.MedSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot1.item_name }}">{% endif %}</div>
                             <div id="mid3" style="position:absolute; left:23px; top:212px; width:32px; height:32px;">{% if fitting.MedSlot2 %}<img src="{{ fitting.MedSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot2.item_name }}">{% endif %}</div>
                             <div id="mid4" style="position:absolute; left:30px; top:245px; width:32px; height:32px;">{% if fitting.MedSlot3 %}<img src="{{ fitting.MedSlot3.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot3.item_name }}">{% endif %}</div>
                             <div id="mid5" style="position:absolute; left:46px; top:278px; width:32px; height:32px;">{% if fitting.MedSlot4 %}<img src="{{ fitting.MedSlot4.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot4.item_name }}">{% endif %}</div>
                             <div id="mid6" style="position:absolute; left:69px; top:304px; width:32px; height:32px;">{% if fitting.MedSlot5 %}<img src="{{ fitting.MedSlot5.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot5.item_name }}">{% endif %}</div>
                             <div id="mid7" style="position:absolute; left:100px; top:328px; width:32px; height:32px;">{% if fitting.MedSlot6 %}<img src="{{ fitting.MedSlot6.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot6.item_name }}">{% endif %}</div>
                             <div id="mid8" style="position:absolute; left:133px; top:342px; width:32px; height:32px;">{% if fitting.MedSlot7 %}<img src="{{ fitting.MedSlot7.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot7.item_name }}">{% endif %}</div>
 
-                            <div id="lowx" style="position:absolute; left: 0px; top: 0px; width: 398px; height: 398px; z-index:-1;">
-                                <img src="/static/fittings/img/pannel/{{ slots.low }}l.png" alt="" style="border:0px;" />
+                            <div id="lowx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
+                                <img src="/static/fittings/img/pannel/{{ slots.low }}l.png" alt="" style="border:0;">
                             </div>
                             <div id="low1" style="position:absolute; left:344px; top:143px; width:32px; height:32px;">{% if fitting.LoSlot0 %}<img src="{{ fitting.LoSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot0.item_name }}">{% endif %}</div>
                             <div id="low2" style="position:absolute; left:350px; top:178px; width:32px; height:32px;">{% if fitting.LoSlot1 %}<img src="{{ fitting.LoSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot1.item_name }}">{% endif %}</div>
                             <div id="low3" style="position:absolute; left:349px; top:213px; width:32px; height:32px;">{% if fitting.LoSlot2 %}<img src="{{ fitting.LoSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot2.item_name }}">{% endif %}</div>
                             <div id="low4" style="position:absolute; left:340px; top:246px; width:32px; height:32px;">{% if fitting.LoSlot3 %}<img src="{{ fitting.LoSlot3.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot3.item_name }}">{% endif %}</div>
                             <div id="low5" style="position:absolute; left:323px; top:277px; width:32px; height:32px;">{% if fitting.LoSlot4 %}<img src="{{ fitting.LoSlot4.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot4.item_name }}">{% endif %}</div>
                             <div id="low6" style="position:absolute; left:300px; top:304px; width:32px; height:32px;">{% if fitting.LoSlot5 %}<img src="{{ fitting.LoSlot5.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot5.item_name }}">{% endif %}</div>
                             <div id="low7" style="position:absolute; left:268px; top:324px; width:32px; height:32px;">{% if fitting.LoSlot6 %}<img src="{{ fitting.LoSlot6.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot6.item_name }}">{% endif %}</div>
                             <div id="low8" style="position:absolute; left:234px; top:338px; width:32px; height:32px;">{% if fitting.LoSlot7 %}<img src="{{ fitting.LoSlot7.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot7.item_name }}">{% endif %}</div>
 
-                            <div id="rigxx" style="position:absolute; left: 0px; top: 0px; width: 398px; height: 398px; z-index:-1;">
-                                <img src="/static/fittings/img/pannel/{{ slots.rig }}r.png" alt="" style="border:0px;" />
+                            <div id="rigxx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
+                                <img src="/static/fittings/img/pannel/{{ slots.rig }}r.png" alt="" style="border:0;">
                             </div>
                             <div id="rig1" style="position:absolute; left:148px; top:259px; width:32px; height:32px;">{% if fitting.RigSlot0 %}<img src="{{ fitting.RigSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.RigSlot0.item_name }}">{% endif %}</div>
                             <div id="rig2" style="position:absolute; left:185px; top:267px; width:32px; height:32px;">{% if fitting.RigSlot1 %}<img src="{{ fitting.RigSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.RigSlot1.item_name }}">{% endif %}</div>
                             <div id="rig3" style="position:absolute; left:221px; top:259px; width:32px; height:32px;">{% if fitting.RigSlot2 %}<img src="{{ fitting.RigSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.RigSlot2.item_name }}">{% endif %}</div>
                             {% if slots.sub %}
-                                <div id="subx" style="position:absolute; left: 0px; top: 0px; width: 398px; height: 398px; z-index:-1;">
-                                    <img src="/static/fittings/img/pannel/{{ slots.sub }}s.png" alt="" style="border:0px;" />
+                                <div id="subx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
+                                    <img src="/static/fittings/img/pannel/{{ slots.sub }}s.png" alt="" style="border:0;">
                                 </div>
                                 <div id="sub1" style="position:absolute; left:117px; top:131px; width:32px; height:32px;">{% if fitting.SubSystemSlot0 %}<img src="{{ fitting.SubSystemSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot0.item_name }}">{% endif %}</div>
                                 <div id="sub2" style="position:absolute; left:147px; top:108px; width:32px; height:32px;">{% if fitting.SubSystemSlot1 %}<img src="{{ fitting.SubSystemSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot1.item_name }}">{% endif %}</div>
                                 <div id="sub3" style="position:absolute; left:184px; top:98px; width:32px; height:32px;">{% if fitting.SubSystemSlot2 %}<img src="{{ fitting.SubSystemSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot2.item_name }}">{% endif %}</div>
                                 <div id="sub4" style="position:absolute; left:221px; top:107px; width:32px; height:32px;">{% if fitting.SubSystemSlot3 %}<img src="{{ fitting.SubSystemSlot3.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot3.item_name }}">{% endif %}</div>
                             {% endif %}
                             <div id="bigship" style='position:absolute; left:72px; top:71px; width:256px; height:256px; z-index:-2;'>
@@ -155,15 +155,15 @@
                             </div>
                         </div>
                     </div>
                     <div class="col-sm-12 col-md-6">
                         <div class="col-sm-12 col-md-12 text-center" style="margin-bottom: 5px;">
                             <h3>{{fit.name}}</h3>
                             {% for cat in cats %}
-                            <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
+                            <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                             {% endfor %}
                         </div>
                         <div class="col-sm-12 col-md-12">
                             <div class="panel panel-warning">
                                 <div class="panel-heading text-center">
                                     {% translate "Hull" %}
                                 </div>
@@ -171,45 +171,45 @@
                                     {{ fit.ship_type.name }}
                                 </div>
                                 <div class="panel-heading text-center">
                                     {% translate "Fitting Notes" %}
                                 </div>
                                 <div class="panel-body">
                                     <div class="well">
-                                        <p style="white-space: pre-wrap; white-space: -moz-pre-wrap; white-space: -pre-wrap; white-space: -o-pre-wrap; word-wrap: break-word;">{{ fit.description|break_html_lines|striptags|urlize }}</p>
+                                        <p style="white-space: pre-wrap; white-space: -moz-pre-wrap; white-space: pre-wrap; white-space: -o-pre-wrap; word-wrap: break-word;">{{ fit.description|break_html_lines|striptags|urlize }}</p>
                                     </div>
                                 </div>
                             </div>
                         </div>
 
                     </div>
                 </div>
             </div>
 
             <div class="panel-heading">
               <h4 class="panel-title">
                 {% translate "Fit" %}
                   <div class="pull-right">
                     <a href="{% url 'fittings:save_fit' fit.pk %}" class="btn btn-xs btn-success" style="margin-top: -2px;">{% translate "Save to EVE" %}</a>
-                    <button class='btn btn-xs btn-success' id="buyAllButton" style="margin-top: -2px;" data-clipboard-text="{{fit.ship_type.type_name}}&#10;{% if fitting.LoSlot0 %}{{fitting.LoSlot0.item_name}}&#10;{% endif %}{% if fitting.LoSlot1 %}{{fitting.LoSlot1.item_name}}&#10;{% endif %}{% if fitting.LoSlot2 %}{{fitting.LoSlot2.item_name}}&#10;{% endif %}{% if fitting.LoSlot3 %}{{fitting.LoSlot3.item_name}}&#10;{% endif %}{% if fitting.LoSlot4 %}{{fitting.LoSlot4.item_name}}&#10;{% endif %}{% if fitting.LoSlot5 %}{{fitting.LoSlot5.item_name}}&#10;{% endif %}{% if fitting.LoSlot6 %}{{fitting.LoSlot6.item_name}}&#10;{% endif %}{% if fitting.LoSlot7 %}{{fitting.LoSlot7.item_name}}&#10;{% endif %}{% if fitting.MedSlot0 %}{{fitting.MedSlot0.item_name}}&#10;{% endif %}{% if fitting.MedSlot1 %}{{fitting.MedSlot1.item_name}}&#10;{% endif %}{% if fitting.MedSlot2 %}{{fitting.MedSlot2.item_name}}&#10;{% endif %}{% if fitting.MedSlot3 %}{{fitting.MedSlot3.item_name}}&#10;{% endif %}{% if fitting.MedSlot4 %}{{fitting.MedSlot4.item_name}}&#10;{% endif %}{% if fitting.MedSlot5 %}{{fitting.MedSlot5.item_name}}&#10;{% endif %}{% if fitting.MedSlot6 %}{{fitting.MedSlot6.item_name}}&#10;{% endif %}{% if fitting.MedSlot7 %}{{fitting.MedSlot7.item_name}}&#10;{% endif %}{% if fitting.HiSlot0 %}{{fitting.HiSlot0.item_name}}&#10;{% endif %}{% if fitting.HiSlot1 %}{{fitting.HiSlot1.item_name}}&#10;{% endif %}{% if fitting.HiSlot2 %}{{fitting.HiSlot2.item_name}}&#10;{% endif %}{% if fitting.HiSlot3 %}{{fitting.HiSlot3.item_name}}&#10;{% endif %}{% if fitting.HiSlot4 %}{{fitting.HiSlot4.item_name}}&#10;{% endif %}{% if fitting.HiSlot5 %}{{fitting.HiSlot5.item_name}}&#10;{% endif %}{% if fitting.HiSlot6 %}{{fitting.HiSlot6.item_name}}&#10;{% endif %}{% if fitting.HiSlot7 %}{{fitting.HiSlot7.item_name}}&#10;{% endif %}{% if fitting.RigSlot0 %}{{fitting.RigSlot0.item_name}}&#10;{% endif %}{% if fitting.RigSlot1 %}{{fitting.RigSlot1.item_name}}&#10;{% endif %}{% if fitting.RigSlot2 %}{{fitting.RigSlot2.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot0 %}{{fitting.SubSystemSlot0.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot1 %}{{fitting.SubSystemSlot1.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot2 %}{{fitting.SubSystemSlot2.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot3 %}{{fitting.SubSystemSlot3.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot0 %}{{fitting.ServiceSlot0.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot1 %}{{fitting.ServiceSlot1.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot2 %}{{fitting.ServiceSlot2.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot3 %}{{fitting.ServiceSlot3.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot4 %}{{fitting.ServiceSlot4.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot5 %}{{fitting.ServiceSlot5.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot6 %}{{fitting.ServiceSlot6.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot7 %}{{fitting.ServiceSlot7.item_name}}&#10;{% endif %}{% if fitting.FighterTube0 %}{{fitting.FighterTube0.item_name}}&#10;{% endif %}{% if fitting.FighterTube1 %}{{fitting.FighterTube1.item_name}}&#10;{% endif %}{% if fitting.FighterTube2 %}{{fitting.FighterTube2.item_name}}&#10;{% endif %}{% if fitting.FighterTube3 %}{{fitting.FighterTube3.item_name}}&#10;{% endif %}{% if fitting.FighterTube4 %}{{fitting.FighterTube4.item_name}}&#10;{% endif %}{% for ammo in fitting.Cargo %}{{ammo.item_name}} x{{ammo.quantity}}&#10;{% endfor %}{% for fighter in fitting.FighterBay %}{{fighter.item_name}} x{{fighter.quantity}}&#10;{% endfor %}{% for drone in fitting.DroneBay %}{{drone.item_name}} x{{drone.quantity}}&#10;{% endfor %}">
+                    <button class='btn btn-xs btn-success' id="buyAllButton" style="margin-top: -2px;" data-clipboard-text="{{fit.ship_type.name}}&#10;{% if fitting.LoSlot0 %}{{fitting.LoSlot0.item_name}}&#10;{% endif %}{% if fitting.LoSlot1 %}{{fitting.LoSlot1.item_name}}&#10;{% endif %}{% if fitting.LoSlot2 %}{{fitting.LoSlot2.item_name}}&#10;{% endif %}{% if fitting.LoSlot3 %}{{fitting.LoSlot3.item_name}}&#10;{% endif %}{% if fitting.LoSlot4 %}{{fitting.LoSlot4.item_name}}&#10;{% endif %}{% if fitting.LoSlot5 %}{{fitting.LoSlot5.item_name}}&#10;{% endif %}{% if fitting.LoSlot6 %}{{fitting.LoSlot6.item_name}}&#10;{% endif %}{% if fitting.LoSlot7 %}{{fitting.LoSlot7.item_name}}&#10;{% endif %}{% if fitting.MedSlot0 %}{{fitting.MedSlot0.item_name}}&#10;{% endif %}{% if fitting.MedSlot1 %}{{fitting.MedSlot1.item_name}}&#10;{% endif %}{% if fitting.MedSlot2 %}{{fitting.MedSlot2.item_name}}&#10;{% endif %}{% if fitting.MedSlot3 %}{{fitting.MedSlot3.item_name}}&#10;{% endif %}{% if fitting.MedSlot4 %}{{fitting.MedSlot4.item_name}}&#10;{% endif %}{% if fitting.MedSlot5 %}{{fitting.MedSlot5.item_name}}&#10;{% endif %}{% if fitting.MedSlot6 %}{{fitting.MedSlot6.item_name}}&#10;{% endif %}{% if fitting.MedSlot7 %}{{fitting.MedSlot7.item_name}}&#10;{% endif %}{% if fitting.HiSlot0 %}{{fitting.HiSlot0.item_name}}&#10;{% endif %}{% if fitting.HiSlot1 %}{{fitting.HiSlot1.item_name}}&#10;{% endif %}{% if fitting.HiSlot2 %}{{fitting.HiSlot2.item_name}}&#10;{% endif %}{% if fitting.HiSlot3 %}{{fitting.HiSlot3.item_name}}&#10;{% endif %}{% if fitting.HiSlot4 %}{{fitting.HiSlot4.item_name}}&#10;{% endif %}{% if fitting.HiSlot5 %}{{fitting.HiSlot5.item_name}}&#10;{% endif %}{% if fitting.HiSlot6 %}{{fitting.HiSlot6.item_name}}&#10;{% endif %}{% if fitting.HiSlot7 %}{{fitting.HiSlot7.item_name}}&#10;{% endif %}{% if fitting.RigSlot0 %}{{fitting.RigSlot0.item_name}}&#10;{% endif %}{% if fitting.RigSlot1 %}{{fitting.RigSlot1.item_name}}&#10;{% endif %}{% if fitting.RigSlot2 %}{{fitting.RigSlot2.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot0 %}{{fitting.SubSystemSlot0.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot1 %}{{fitting.SubSystemSlot1.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot2 %}{{fitting.SubSystemSlot2.item_name}}&#10;{% endif %}{% if fitting.SubSystemSlot3 %}{{fitting.SubSystemSlot3.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot0 %}{{fitting.ServiceSlot0.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot1 %}{{fitting.ServiceSlot1.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot2 %}{{fitting.ServiceSlot2.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot3 %}{{fitting.ServiceSlot3.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot4 %}{{fitting.ServiceSlot4.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot5 %}{{fitting.ServiceSlot5.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot6 %}{{fitting.ServiceSlot6.item_name}}&#10;{% endif %}{% if fitting.ServiceSlot7 %}{{fitting.ServiceSlot7.item_name}}&#10;{% endif %}{% if fitting.FighterTube0 %}{{fitting.FighterTube0.item_name}}&#10;{% endif %}{% if fitting.FighterTube1 %}{{fitting.FighterTube1.item_name}}&#10;{% endif %}{% if fitting.FighterTube2 %}{{fitting.FighterTube2.item_name}}&#10;{% endif %}{% if fitting.FighterTube3 %}{{fitting.FighterTube3.item_name}}&#10;{% endif %}{% if fitting.FighterTube4 %}{{fitting.FighterTube4.item_name}}&#10;{% endif %}{% for ammo in fitting.Cargo %}{{ammo.item_name}} x{{ammo.quantity}}&#10;{% endfor %}{% for fighter in fitting.FighterBay %}{{fighter.item_name}} x{{fighter.quantity}}&#10;{% endfor %}{% for drone in fitting.DroneBay %}{{drone.item_name}} x{{drone.quantity}}&#10;{% endfor %}">
                         {% translate "Copy Buy All" %}
                     </button>
 
                      <span data-toggle="modal" data-target="#eftModal">
                         <button class='btn btn-xs btn-success' id="copyEftButton" style="margin-top: -2px;" data-toggle="tooltip" data-placement="top" title="{% translate 'Copy Fit (EFT)' %}">{% translate "Copy Fit (EFT)" %}</button>
                     </span>
                   </div>
               </h4>
             </div>
 
             <div id="fitting">
               <div class="panel-body">
                 <ul class="list-group">
                     <li class="list-group-item list-group-item-warning">{% translate "Hull" %}</li>
-                    <li class="list-group-item"><img src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.name }}</li>
+                    <li class="list-group-item"><img src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.name }}"> {{ fit.ship_type.name }}</li>
                     {% if fitting.SubSystemSlot0 %}
                         <li class="list-group-item list-group-item-warning">{% translate "SubSystems" %}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot0.item_name }}"> {{fitting.SubSystemSlot0.item_name}}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot1.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot1.item_name }}"> {{fitting.SubSystemSlot1.item_name}}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot2.item_name }}"> {{fitting.SubSystemSlot2.item_name}}</li>
                         <li class="list-group-item"><img src="{{ fitting.SubSystemSlot3.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot3.item_name }}"> {{fitting.SubSystemSlot3.item_name}}</li>
                     {% endif %}
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/bundles/jquery.quicksearch-js.html` & `fittings-2.0.2/fittings/templates/fittings/bundles/jquery.quicksearch-js.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/templates/fittings/bundles/multi-select-js.html` & `fittings-2.0.2/fittings/templates/fittings/bundles/multi-select-js.html`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/templates/fittings/view_all_categories.html` & `fittings-2.0.2/fittings/templates/fittings/view_all_categories.html`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,32 @@
         </h2>
         <div class="panel panel-default">
             <div class="panel-heading">
                 {% translate "Fits" %}
             </div>
             <div class="panel-body">
                 {% if not cats %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Categories Found" %}</div>
+                    <div class="alert alert-warning text-center">{% translate "No Categories Found" %}</div>
                 {% else %}
                     <table class="table table-hover dataTable" id="fitTable">
                         <thead>
-                            <th>{% translate "Name" %}</th>
-                            <th>{% translate "Doctrines Assigned" %}</th>
-                            <th>{% translate "Fittings Assigned" %}</th>
-                            {% if perms.fittings.manage %}
-                                <th>{% translate "Groups Assigned" %}</th>
-                                <th> </th>
-                            {% endif %}
+                            <tr>
+                                <th>{% translate "Name" %}</th>
+                                <th>{% translate "Doctrines Assigned" %}</th>
+                                <th>{% translate "Fittings Assigned" %}</th>
+                                {% if perms.fittings.manage %}
+                                    <th>{% translate "Groups Assigned" %}</th>
+                                    <th> </th>
+                                {% endif %}
+                            </tr>
                         </thead>
                         <tbody>
                             {% for cat in cats %}
                                 <tr>
-                                    <td> <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span> </td>
+                                    <td> <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span> </td>
                                     <td> {{ cat.doctrines_count }}</td>
                                     <td> {{ cat.total_fits }} </td>
                                     {% if perms.fittings.manage %}
                                         <td> {{ cat.groups_count }}</td>
                                         <td>
                                             <a href="{% url 'fittings:view_category' cat.pk %}" type="button" class="btn btn-sm btn-primary" data-toggle="tooltip" data-placement="top" title="{% translate 'View Category' %}">
                                                 <span class="fa fas fa-eye"></span>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/dashboard.html` & `fittings-2.0.2/fittings/templates/fittings/dashboard.html`

 * *Files 10% similar despite different names*

```diff
@@ -30,38 +30,40 @@
         </h2>
         <div class="panel panel-default">
             <div class="panel-heading">
                 {% translate "Doctrines" %}
             </div>
             <div class="panel-body">
                 {% if not docs %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Doctrines Found" %} </div>
+                    <div class="alert alert-warning text-center">{% translate "No Doctrines Found" %} </div>
                 {% else %}
                     <table class="table table-hover dataTable" id="docTable">
                         <thead>
-                            <th> </th>
-                            <th>{% translate "Name" %}</th>
-                            <th>{% translate "Categories" %}</th>
-                            <th>{% translate "Description" %}</th>
-                            <th>{% translate "Ships" %}</th>
+                            <tr>
+                                <th> </th>
+                                <th>{% translate "Name" %}</th>
+                                <th>{% translate "Categories" %}</th>
+                                <th>{% translate "Description" %}</th>
+                                <th>{% translate "Ships" %}</th>
+                            </tr>
                         </thead>
                         <tbody>
                             {% for doc in docs %}
                                 <tr>
-                                    <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}"><img src="{{ doc.icon_url }}" class="img-circle" style="display: block; margin: auto;"/> </a></td>
+                                    <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}"><img src="{{ doc.icon_url }}" class="img-circle" style="display: block; margin: auto;"> </a></td>
                                     <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}">{{ doc.name }}</a> </td>
                                     <td>
                                         {% for cat in doc.category.all %}
-                                            <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
+                                            <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                                         {% endfor %}
                                     </td>
                                     <td> {{ doc.description|linebreaks }} </td>
                                     <td>
                                         {% for fitting in doc_dict|get_item:doc.pk %}
-                                            <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-circle" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.name }}"/>
+                                            <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-circle" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.name }}">
                                         {% endfor %}
                                     </td>
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
                 {% endif %}
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/view_doctrine.html` & `fittings-2.0.2/fittings/templates/fittings/view_doctrine.html`

 * *Files 4% similar despite different names*

```diff
@@ -14,50 +14,50 @@
         <div class="modal-dialog" role="document">
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                     <h4 class="modal-title" id="modalTitle">{% translate "Are you sure?" %}</h4>
                 </div>
                 <div class="modal-body">
-                    <p style="white-space: pre-line">
+                    <p style="white-space: pre-line;">
                         {% translate "Are you sure you wish to delete this doctrine?" %}
                         <i><strong>{% translate "This action is permanent." %}</strong></i>
                     </p>
                 </div>
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">{% translate "No - Close" %}</button>
                     <a href="{% url 'fittings:delete_doctrine' doctrine.pk %}" type="button" class="btn btn-danger">{% translate "Yes - Delete" %}</a>
                 </div>
             </div>
         </div>
     </div>
 
     {# modal end #}
-    <br />
+    <br>
     <div class="col-md-3">
         <div class="panel panel-primary">
             <div class="panel-heading">
                 {% translate "Doctrine Information" %}
 
                 {% if perms.fittings.manage %}
                     <span data-toggle="modal" data-target="#deleteModal">
                         <button class="btn btn-xs btn-danger" style="float: right; margin-left: 5px;" data-toggle="tooltip" data-placement="top" title="{% translate 'Delete Doctrine' %}"><span class="fa fas fa-times"></span> </button>
                     </span>
-                    <a href="{% url 'fittings:edit_doctrine' doctrine.pk %}" class="btn btn-xs btn-warning" style="float: right" data-toggle="tooltip" data-placement="top" title="{% translate 'Edit Doctrine' %}"><span class="fa fas fa-pencil-alt"></span> </a>
+                    <a href="{% url 'fittings:edit_doctrine' doctrine.pk %}" class="btn btn-xs btn-warning" style="float: right;" data-toggle="tooltip" data-placement="top" title="{% translate 'Edit Doctrine' %}"><span class="fa fas fa-pencil-alt"></span> </a>
                 {% endif %}
             </div>
             <div class="panel-body">
-                <img src="{{ doctrine.icon_url }}" class="img-circle center-block" style="text-align: center"/>
-                <h4 style="text-align: center">{{ doctrine.name }}</h4>
-                <h5 style="text-align: center">
+                <img src="{{ doctrine.icon_url }}" class="img-circle center-block text-center">
+                <h4 class="text-center">{{ doctrine.name }}</h4>
+                <h5 class="text-center">
                         {% for cat in d_cats %}
-                            <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
+                            <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                         {% endfor %}
                 </h5>
-                <hr />
+                <hr>
                 <dl>
                     <dt>{% translate "Description" %}</dt>
                     <dd><pre>{{ doctrine.description|break_html_lines|striptags }}</pre></dd>
                     {% if doctrine.created %}
                     <dt>{% translate "Created" %}</dt>
                         {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
                             <dd>{{ doctrine.created|date:'Y-m-d / H:i:s' }}</dd>
@@ -78,34 +78,36 @@
         </div>
     </div>
     <div class="col-md-9">
         <div class="panel panel-default">
             <div class="panel-heading">{% translate "Doctrine Fits" %}</div>
             <div class="panel-body">
                 {% if not fits %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Fits Found" %}</div>
+                    <div class="alert alert-warning text-center">{% translate "No Fits Found" %}</div>
                 {% else %}
                     <table class="table table-hover dataTable" id="fitsTable">
                         <thead>
-                            <th>{% translate "Name" %}</th>
-                            <th>{% translate "Category" %}</th>
-                            <th>{% translate "Description" %}</th>
-                            <th>{% translate "Ship Type" %}</th>
+                            <tr>
+                                <th>{% translate "Name" %}</th>
+                                <th>{% translate "Category" %}</th>
+                                <th>{% translate "Description" %}</th>
+                                <th>{% translate "Ship Type" %}</th>
+                            </tr>
                         </thead>
                         <tbody>
                                 {% for fit in fits %}
                                     <tr>
                                         <td> <a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a> </td>
                                         <td>
                                             {% for cat in f_cats|get_item:fit.pk %}
-                                            <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
+                                            <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                                             {% endfor %}
                                         </td>
                                         <td> {{ fit.description }} </td>
-                                        <td> <img class="img-circle" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.type_name }}</td>
+                                        <td> <img class="img-circle" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.name }}"> {{ fit.ship_type.name }}</td>
                                     </tr>
                                 {% endfor %}
                         </tbody>
                     </table>
                 {% endif %}
             </div>
         </div>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/view_all_fits.html` & `fittings-2.0.2/fittings/templates/fittings/view_all_fits.html`

 * *Files 8% similar despite different names*

```diff
@@ -32,34 +32,36 @@
         </h2>
         <div class="panel panel-default">
             <div class="panel-heading">
                 {% translate "Fits" %}
             </div>
             <div class="panel-body">
                 {% if not fits %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Fits Found" %}</div>
+                    <div class="alert alert-warning text-center">{% translate "No Fits Found" %}</div>
                 {% else %}
                     <table class="table table-hover dataTable" id="fitTable">
                         <thead>
-                            <th>{% translate "Name" %}</th>
-                            <th>{% translate "Categories" %}</th>
-                            <th>{% translate "Description" %}</th>
-                            <th>{% translate "Ship Type" %}</th>
+                            <tr>
+                                <th>{% translate "Name" %}</th>
+                                <th>{% translate "Categories" %}</th>
+                                <th>{% translate "Description" %}</th>
+                                <th>{% translate "Ship Type" %}</th>
+                            </tr>
                         </thead>
                         <tbody>
                             {% for fit in fits %}
                                 <tr>
                                     <td> <a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a> </td>
                                     <td>
                                         {% for cat in cats|get_item:fit.pk %}
-                                        <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
+                                        <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span>
                                         {% endfor %}
                                     </td>
                                     <td> {{ fit.description }} </td>
-                                    <td> <img class="img-circle" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.type_name }} </td>
+                                    <td> <img class="img-circle" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.name }}"> {{ fit.ship_type.name }} </td>
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
                 {% endif %}
             </div>
         </div>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/edit_category.html` & `fittings-2.0.2/fittings/templates/fittings/edit_category.html`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,22 @@
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form" role="form" action="" method="POST">
                             {% csrf_token %}
                             <div class="row">
                                 <div class="col-sm-10">
                                     <div class="form-group">
                                         <label for="name">{% translate "Category Name" %}</label>
-                                        <input type="text" class="form-control" name="name" id="name" value="{{cat.name}}" required/>
+                                        <input type="text" class="form-control" name="name" id="name" value="{{cat.name}}" required>
                                     </div>
                                 </div>
                                 <div class="col-sm-2">
                                     <div class="form-group">
                                         <label for="color">{% translate "Category Color" %}</label>
                                         <div class="form-control col-sm-1" id="color-wrapper" style="padding:0 !important;">
-                                            <input type="color" name="color" id="color" value="{{cat.color}}" required/>
+                                            <input type="color" name="color" id="color" value="{{cat.color}}" required>
                                         </div>
                                     </div>
                                 </div>
                             </div>
                             <div class="row">
                                 <div class="col-sm-12">
                                     <div class="form-group">
@@ -88,15 +88,15 @@
                                             {% for doc in docs %}
                                             <option value="{{doc.pk}}" {% if doc in cat.doctrines.all %} selected {% endif %}>{{doc.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/add_doctrine.html` & `fittings-2.0.2/fittings/templates/fittings/add_doctrine.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
 {% load evelinks %}
 
 {% block more_css %}
-    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/multi-select/0.9.12/css/multi-select.min.css" />
+    {% include 'fittings/bundles/multi-select-css.html' %}
     <style>
         .form-control {
             margin: 2px;
         }
 
         .ms-container {
             width: 100% !important;
@@ -41,15 +41,15 @@
                 <div class="row">
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form-signin" role="form" action="" method="POST">
                             {% csrf_token %}
                             <div class="form-group">
                                 <label for="name" class="col-sm-2 control-label">{% translate "Doctrine Name" %}</label>
                                 <div class="col-sm-10">
-                                    <input type="text" class="form-control" name="name" id="name" required/>
+                                    <input type="text" class="form-control" name="name" id="name" required>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">{% translate "Doctrine Description" %}</label>
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" rows="4"></textarea>
                                 </div>
@@ -71,15 +71,15 @@
                                         {% for ship in ships %}
                                             <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__name}}</option>
                                         {% endfor %}
                                     </select>
                                     <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
-filters %} {% load static %} {% load evelinks %} {% block more_css %}
+filters %} {% load static %} {% load evelinks %} {% block more_css %} {%
+include 'fittings/bundles/multi-select-css.html' %}
  {% endblock %} {% block page_title %}{% translate "Add Doctrine" %}{% endblock
 %} {% block fittings_block %} {% if msg %}
  ×  {% if msg.0 != 'warning' %}
 *** {% if msg.0 == 'danger' %}Oh No!{% elif msg.0 == 'success' %}Success!{%
 endif %} ***
 {% endif %}
 {{ msg.1 }}
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/base.html` & `fittings-2.0.2/fittings/templates/fittings/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         }
     </style>
     {% include 'bundles/datatables-css.html' %}
     {% block more_css %}{%endblock%}
 {% endblock extra_css %}
 {% block content %}
     <div class="col-lg-12">
-        <br />
+        <br>
         <div class="col-lg-12 container">
             <nav class="navbar navbar-default">
                 <div class="container-fluid">
                     <div class="navbar-header">
                         <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target=".fittings-menus-collapse" aria-expanded="false">
                             <span class="sr-only">{% translate "Toggle navigation" %}</span>
                             <span class="icon-bar"></span>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/view_category.html` & `fittings-2.0.2/fittings/templates/fittings/view_category.html`

 * *Files 6% similar despite different names*

```diff
@@ -42,20 +42,20 @@
                         <span class="fa fas fa-times"></span>
                     </a>
                 </div>
                 {% endif %}
             </div>
             <div class="panel-body tp">
                 <strong>{% translate "Name" %}: </strong>
-                <br/>
-                <span class="label" style="background-color: {{cat.color}}">{{cat.name}}</span>
+                <br>
+                <span class="label" style="background-color: {{cat.color}};">{{cat.name}}</span>
                 <div id="spacer" style="padding-top: 5px;"></div>
                 {% if perms.fittings.manage %}
                     <strong>{% translate "Groups" %}: </strong>
-                    <br />
+                    <br>
                     {% if cat.groups.all|length != 0 %}
                       {% for group in cat.groups.all %} <span class="label label-primary">{{group.name}}</span> {% endfor %}
                     {% else %}
                       <span class="label label-warning">{% translate "Category is public" %}</span>
                     {% endif %}
                 {% endif %}
 
@@ -65,75 +65,79 @@
                     <li class="active mv"><a data-toggle="tab" href="#doctrines">{% translate "Doctrines" %}</a></li>
                     <li><a data-toggle="tab" href="#fittings">{% translate "Fittings" %}</a></li>
                 </ul>
                 <div class="tab-content">
                     <div class="tab-pane fade-in active panel-default pd" id="doctrines">
                         <table class="table table-striped dataTable" role="table" id="docTable">
                             <thead>
-                                <th> </th>
-                                <th>{% translate "Name" %}</th>
-                                <th>{% translate "Categories" %}</th>
-                                <th>{% translate "Description" %}</th>
-                                <th>{% translate "Ships" %}</th>
+                                <tr>
+                                    <th> </th>
+                                    <th>{% translate "Name" %}</th>
+                                    <th>{% translate "Categories" %}</th>
+                                    <th>{% translate "Description" %}</th>
+                                    <th>{% translate "Ships" %}</th>
+                                </tr>
                             </thead>
                             <tbody>
                                 {% if not docs %}
                                     <tr>
                                         <td colspan="5">
-                                            <div class="alert alert-warning" style="text-align: center"> {% translate "No Doctrines Found" %} </div>
+                                            <div class="alert alert-warning text-center"> {% translate "No Doctrines Found" %} </div>
                                         </td>
                                     </tr>
                                 {% else %}
                                     {% for doc in docs %}
                                         <tr>
-                                            <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}"><img src="{{ doc.icon_url }}" class="img-circle" style="display: block; margin: auto;"/> </a></td>
+                                            <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}"><img src="{{ doc.icon_url }}" class="img-circle" style="display: block; margin: auto;"> </a></td>
                                             <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}">{{ doc.name }}</a> </td>
                                             <td>
                                                 {% for cate in doc.category.all %}
-                                                <span class="label" style="background-color: {{cate.color}}"><a href="{% url 'fittings:view_category' cate.pk %}" class="nostyle">{{cate.name}}</a></span>
+                                                <span class="label" style="background-color: {{cate.color}};"><a href="{% url 'fittings:view_category' cate.pk %}" class="nostyle">{{cate.name}}</a></span>
                                                 {% endfor %}
                                             </td>
                                             <td> {{ doc.description }} </td>
                                             <td>
                                                 {% for fitting in doc_dict|get_item:doc.pk %}
-                                                    <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-circle" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.type_name }}"/>
+                                                    <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-circle" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.name }}">
                                                 {% endfor %}
                                             </td>
                                         </tr>
                                     {% endfor %}
                                 {% endif %}
                             </tbody>
                         </table>
                     </div>
                     <div class="tab-pane fade-in panel-default pd" id="fittings">
                         <table class="table table-hover dataTable" id="fitTable">
                             <thead>
-                                <th>{% translate "Name" %}</th>
-                                <th>{% translate "Categories" %}</th>
-                                <th>{% translate "Description" %}</th>
-                                <th>{% translate "Ship Type" %}</th>
+                                <tr>
+                                    <th>{% translate "Name" %}</th>
+                                    <th>{% translate "Categories" %}</th>
+                                    <th>{% translate "Description" %}</th>
+                                    <th>{% translate "Ship Type" %}</th>
+                                </tr>
                             </thead>
                             <tbody>
                                 {% if not fits %}
                                     <tr>
                                         <td colspan="4">
-                                            <div class="alert alert-warning" style="text-align: center"> {% translate "No Fits Found" %} </div>
+                                            <div class="alert alert-warning text-center"> {% translate "No Fits Found" %} </div>
                                         </td>
                                     </tr>
                                 {% else %}
                                     {% for fit in fits %}
                                         <tr>
                                             <td> <a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a> </td>
                                             <td>
                                                 {% for cate in cats|get_item:fit.pk %}
-                                                <span class="label" style="background-color: {{cate.color}}"><a href="{% url 'fittings:view_category' cate.pk %}" class="nostyle">{{cate.name}}</a></span>
+                                                <span class="label" style="background-color: {{cate.color}};"><a href="{% url 'fittings:view_category' cate.pk %}" class="nostyle">{{cate.name}}</a></span>
                                                 {% endfor %}
                                             </td>
                                             <td> {{ fit.description }} </td>
-                                            <td> <img class="img-circle" src="{{ fit.ship_type_type_id|type_render_url:128 }}" style="height: 32px; width: 32px;" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.type_name }}</td>
+                                            <td> <img class="img-circle" src="{{ fit.ship_type_type_id|type_render_url:128 }}" style="height: 32px; width: 32px;" title="{{ fit.ship_type.name }}"> {{ fit.ship_type.name }}</td>
                                         </tr>
                                     {% endfor %}
                                 {% endif %}
                             </tbody>
                         </table>
                     </div>
                 </div>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/add_fit.html` & `fittings-2.0.2/fittings/templates/fittings/add_fit.html`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,23 @@
                             {% csrf_token %}
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">{% translate "Description" %}</label>
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" maxlength="500" rows="3"></textarea>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <div class="form-group" >
                                 <label for="eft" class="col-sm-2 control-label">{% translate "Fit" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <textarea class="form-control" name="eft" id="eft" rows="50"></textarea>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
-{% endblock %}
+{% endblock %}
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/create_category.html` & `fittings-2.0.2/fittings/templates/fittings/create_category.html`

 * *Files 5% similar despite different names*

```diff
@@ -41,22 +41,22 @@
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form" role="form" action="" method="POST">
                             {% csrf_token %}
                             <div class="row">
                                 <div class="col-sm-10">
                                     <div class="form-group">
                                         <label for="name">{% translate "Category Name" %}</label>
-                                        <input type="text" class="form-control" name="name" id="name" required/>
+                                        <input type="text" class="form-control" name="name" id="name" required>
                                     </div>
                                 </div>
                                 <div class="col-sm-2">
                                     <div class="form-group">
                                         <label for="color">{% translate "Category Color" %}</label>
                                         <div class="form-control col-sm-1" id="color-wrapper" style="padding:0 !important;">
-                                            <input type="color" name="color" id="color" value="#39CCCC" required/>
+                                            <input type="color" name="color" id="color" value="#39CCCC" required>
                                         </div>
                                     </div>
                                 </div>
                             </div>
                             <div class="row">
                                 <div class="col-sm-12">
                                     <div class="form-group">
@@ -88,15 +88,15 @@
                                             {% for doc in docs %}
                                             <option value="{{doc.pk}}">{{doc.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `fittings-2.0.1/fittings/templates/fittings/edit_doctrine.html` & `fittings-2.0.2/fittings/templates/fittings/edit_doctrine.html`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 <div class="row">
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form-signin" role="form" action="" method="POST">
                             {% csrf_token %}
                             <div class="form-group">
                                 <label for="name" class="col-sm-2 control-label">{% translate "Doctrine Name" %}</label>
                                 <div class="col-sm-10">
-                                    <input type="text" class="form-control" name="name" id="name" value="{{ doctrine.name }}" required/>
+                                    <input type="text" class="form-control" name="name" id="name" value="{{ doctrine.name }}" required>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">{% translate "Doctrine Description" %}</label>
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" rows="4">{{ doctrine.description }}</textarea>
                                 </div>
@@ -56,15 +56,15 @@
                                 <label for="fitSelect" class="col-sm-2 control-label">{% translate "Select Fits" %}</label>
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <select multiple="multiple" id="fitSelect" name="fitSelect">
                                         {% for fit in doc_fits %}
                                             <option value="{{ fit.pk }}" selected>{{ fit.name }} ({{ fit.ship_type.name }})</option>
                                         {% endfor %}
                                         {% for fit in fits %}
-                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.type_name}})</option>
+                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.name}})</option>
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
                             <div class="form-group">
                                 <label for="iconSelect" class="col-sm-2 control-label">{% translate "Select Doctrine Icon" %}</label>
                                 <div class="col-sm-10">
@@ -73,15 +73,15 @@
                                         {% for ship in ships %}
                                             <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__name}}</option>
                                         {% endfor %}
                                     </select>
                                     <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
                                 </div>
                             </div>
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 [{{ doctrine.name }} ]
 {% translate "Doctrine Description" %}
 {{ doctrine.description }}
 {% translate "Select Fits" %}
 {% for fit in doc_fits %}
 {{ fit.name }} ({{ fit.ship_type.name }})
 {% endfor %} {% for fit in fits %}
-{{ fit.name }} ({{fit.ship_type.type_name}})
+{{ fit.name }} ({{fit.ship_type.name}})
 {% endfor %}
 {% translate "Select Doctrine Icon" %}
 {% for ship in ships %}
 {{ship.ship_type__name}}
 {% endfor %}
   {% translate "If you do not see the ship type that you would like to use for
 the icon, add a fit that uses that ship type and try again." %}
```

### Comparing `fittings-2.0.1/fittings/management/commands/fittings_preload_data.py` & `fittings-2.0.2/fittings/management/commands/fittings_preload_data.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/zh.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/zh.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/it-IT.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/it-IT.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/en-GB.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/en-GB.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/fr-FR.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/fr-FR.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/ru.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/ru.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/es-ES.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/es-ES.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/ja.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/ja.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/uk.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/uk.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/ko.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/ko.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/dt-i18n/de-DE.json` & `fittings-2.0.2/fittings/static/fittings/dt-i18n/de-DE.json`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/7m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/7m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/4m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/4m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/0l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/0l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/5l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/5l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/6m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/6m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/5s.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/5s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/r.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/3h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/3h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/2h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/2h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/circle.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/circle.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/3r.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/3r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/2m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/2m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/0r.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/0r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/3m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/3m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/0m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/0m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/0s.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/0s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/5h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/5h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/4l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/4l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/dustwheel.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/8l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/8l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/0h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/0h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/4s.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/4s.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/5m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/5m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_default.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_blue.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/working.jpg` & `fittings-2.0.2/fittings/static/fittings/img/pannel/working.jpg`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/7l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/7l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/1r.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/1r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/noship.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/noship.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/1l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/1l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/4h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/4h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/7h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/7h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/3l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/3l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/6h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/6h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/1h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/1h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/1m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/1m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_revelations.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/2l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/2l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/2r.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/2r.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/6l.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/6l.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/error.jpg` & `fittings-2.0.2/fittings/static/fittings/img/pannel/error.jpg`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/tyrannis_darkred.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/8m.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/8m.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/img/pannel/8h.png` & `fittings-2.0.2/fittings/static/fittings/img/pannel/8h.png`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js` & `fittings-2.0.2/fittings/static/fittings/ajax/libs/clipboard.js/2.0.4/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js` & `fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/js/jquery.multi-select.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css` & `fittings-2.0.2/fittings/static/fittings/ajax/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery,quicksearch.min.js` & `fittings-2.0.2/fittings/static/fittings/ajax/libs/jquery.quicksearch/2.4.0/jquery,quicksearch.min.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css` & `fittings-2.0.2/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js` & `fittings-2.0.2/fittings/static/fittings/ajax/libs/slim-select/1.26.0/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/models.py` & `fittings-2.0.2/fittings/models.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/admin.py` & `fittings-2.0.2/fittings/admin.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/views.py` & `fittings-2.0.2/fittings/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,27 +487,25 @@
             .annotate(groups_count=Count('groups', distinct=True))\
             .annotate(doctrines_count=Count('doctrines', distinct=True))\
             .annotate(fittings_count=Count('fittings', distinct=True))\
             .annotate(d_fittings_count=Count('doctrines__fittings', distinct=True))\
             .annotate(total_fits=F('fittings_count')+F('d_fittings_count'))
     else:
         cats = _get_accessible_categories(request.user)
-        logger.critical(cats)
     for cat in cats:
         logger.debug(f'{cat.name}: Groups {cat.groups_count}')
     ctx['cats'] = cats
     return render(request, 'fittings/view_all_categories.html', context=ctx)
 
 
 @permission_required('fittings.manage')
 @login_required()
 def add_category(request):
     ctx = {}
     if request.method == 'POST':
-        logger.critical("POSTED")
         name = request.POST['name']
         color = request.POST['color']
         fitSelect = [int(fit) for fit in request.POST.getlist('fitSelect')]
         docSelect = [int(doc) for doc in request.POST.getlist('docSelect')]
         groupSelect = [int(grp) for grp in request.POST.getlist('groupSelect')]
 
         cat = Category(name=name, color=color)
```

### Comparing `fittings-2.0.1/fittings/migrations/0005_unicategory.py` & `fittings-2.0.2/fittings/migrations/0005_unicategory.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py` & `fittings-2.0.2/fittings/migrations/0016_remove_dogmaattribute_type_remove_dogmaeffect_type_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py` & `fittings-2.0.2/fittings/migrations/0015_fitting_created_fitting_last_updated_and_more.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0014_serverversion.py` & `fittings-2.0.2/fittings/migrations/0014_serverversion.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0001_initial.py` & `fittings-2.0.2/fittings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0011_auto_20200815_2022.py` & `fittings-2.0.2/fittings/migrations/0011_auto_20200815_2022.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0012_typehistory.py` & `fittings-2.0.2/fittings/migrations/0012_typehistory.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0007_auto_20200605_0735.py` & `fittings-2.0.2/fittings/migrations/0007_auto_20200605_0735.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0004_add_item_category_and_group.py` & `fittings-2.0.2/fittings/migrations/0004_add_item_category_and_group.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0009_auto_20200605_2117.py` & `fittings-2.0.2/fittings/migrations/0009_auto_20200605_2117.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/migrations/0002_add_dgm_unique_constraints.py` & `fittings-2.0.2/fittings/migrations/0002_add_dgm_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/zh_Hans/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.mo` & `fittings-2.0.2/fittings/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/ru/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/es/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/fr_FR/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.mo` & `fittings-2.0.2/fittings/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/ja/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.mo` & `fittings-2.0.2/fittings/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/de/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.mo` & `fittings-2.0.2/fittings/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/locale/ko_KR/LC_MESSAGES/django.po` & `fittings-2.0.2/fittings/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/templatetags/filters.py` & `fittings-2.0.2/fittings/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/templatetags/tags.py` & `fittings-2.0.2/fittings/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings/urls.py` & `fittings-2.0.2/fittings/urls.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/setup.py` & `fittings-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/fittings.egg-info/PKG-INFO` & `fittings-2.0.2/fittings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fittings
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple fittings and doctrine management application.
 Home-page: https://gitlab.com/colcrunch/fittings
 Author: Col Crunch
 Author-email: it-team@serin.space
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `fittings-2.0.1/fittings.egg-info/SOURCES.txt` & `fittings-2.0.2/fittings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fittings-2.0.1/README.md` & `fittings-2.0.2/README.md`

 * *Files identical despite different names*

