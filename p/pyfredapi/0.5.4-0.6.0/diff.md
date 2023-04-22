# Comparing `tmp/pyfredapi-0.5.4.tar.gz` & `tmp/pyfredapi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfredapi-0.5.4.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyfredapi-0.5.4.tar` & `pyfredapi-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,158 @@
--rw-r--r--   0        0        0     1067 2022-09-27 22:09:06.134268 pyfredapi-0.5.4/LICENSE
--rw-r--r--   0        0        0     1941 2022-10-28 22:07:01.709700 pyfredapi-0.5.4/README.md
--rw-r--r--   0        0        0     1704 2023-03-31 23:49:08.792034 pyfredapi-0.5.4/pyfredapi/__init__.py
--rw-r--r--   0        0        0     2521 2023-04-02 21:22:06.505837 pyfredapi-0.5.4/pyfredapi/_base.py
--rw-r--r--   0        0        0     8441 2023-04-17 01:31:33.691827 pyfredapi-0.5.4/pyfredapi/category.py
--rw-r--r--   0        0        0      148 2023-03-31 23:49:08.794567 pyfredapi-0.5.4/pyfredapi/exceptions/__init__.py
--rw-r--r--   0        0        0     1160 2023-03-31 23:49:08.795190 pyfredapi-0.5.4/pyfredapi/exceptions/exceptions.py
--rw-r--r--   0        0        0     5794 2023-04-17 01:26:06.450096 pyfredapi-0.5.4/pyfredapi/maps.py
--rw-r--r--   0        0        0        0 2022-10-12 01:34:52.474192 pyfredapi-0.5.4/pyfredapi/py.typed
--rw-r--r--   0        0        0     9561 2023-04-02 21:22:06.507234 pyfredapi-0.5.4/pyfredapi/releases.py
--rw-r--r--   0        0        0    20891 2023-04-02 21:22:06.508030 pyfredapi-0.5.4/pyfredapi/series.py
--rw-r--r--   0        0        0    13493 2023-04-02 20:58:44.394082 pyfredapi-0.5.4/pyfredapi/series_collection.py
--rw-r--r--   0        0        0     3570 2023-04-02 21:22:06.514616 pyfredapi-0.5.4/pyfredapi/sources.py
--rw-r--r--   0        0        0     4337 2023-04-02 21:22:06.514999 pyfredapi-0.5.4/pyfredapi/tags.py
--rw-r--r--   0        0        0       76 2023-03-31 23:49:08.800945 pyfredapi-0.5.4/pyfredapi/utils/__init__.py
--rw-r--r--   0        0        0      387 2022-10-27 01:47:28.858898 pyfredapi-0.5.4/pyfredapi/utils/_common_type_hints.py
--rw-r--r--   0        0        0     1511 2023-03-31 23:49:08.801548 pyfredapi-0.5.4/pyfredapi/utils/_convert_to_pandas.py
--rw-r--r--   0        0        0      221 2023-03-31 23:49:08.802190 pyfredapi-0.5.4/pyfredapi/utils/enums.py
--rw-r--r--   0        0        0     3380 2023-04-17 01:42:41.082084 pyfredapi-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 pyfredapi-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.flake8
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/RELEASE.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/mypy.ini
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/requirements.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/sonar-project.properties
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tox.ini
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/PULL_REQUEST_TEMPLATE/version_release.md
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/workflows/build-pyfredapi.yml
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/workflows/sonarcloud.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0     7992 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/requirements.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/_templates/layout.html
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/CHANGELOG.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/api.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.CategoryApiParameters.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_children.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_related.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_related_tags.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_series.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_tags.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.MapApiParameters.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries_info.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.get_shape_files.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.SeriesApiParameters.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.SeriesInfo.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.SeriesSearchParameters.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_all_releases.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_asof_date.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_categories.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_info.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_initial_release.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_releases.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_tags.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_updates.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_vintagedates.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.search_series.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.search_series_related_tags.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.search_series_tags.rst
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesData.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.SourceApiParameters.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.get_source.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.get_source_release.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.get_sources.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.TagsApiParameters.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.get_related_tags.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.get_series_matching_tags.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.get_tags.rst
+-rw-r--r--   0        0        0    51352 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/tutorials/maps.ipynb
+-rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/tutorials/series.ipynb
+-rw-r--r--   0        0        0  3857297 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/tutorials/series_collection.ipynb
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/__about__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/__init__.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/_base.py
+-rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/category.py
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/maps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/py.typed
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/releases.py
+-rw-r--r--   0        0        0    20891 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/series.py
+-rw-r--r--   0        0        0    13493 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/series_collection.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/sources.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/tags.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/exceptions/__init__.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/exceptions/exceptions.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/_common_type_hints.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/_convert_to_pandas.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/enums.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_base.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_category.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_maps.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_release.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_series.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_series_collection.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_sources.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_tags.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category.yaml
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_children.yaml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related.yaml
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related_tags[json].yaml
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_series.yaml
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_tags[json].yaml
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml
+-rw-r--r--   0        0        0    11038 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries[json].yaml
+-rw-r--r--   0        0        0    11181 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries[pandas].yaml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries_info.yaml
+-rw-r--r--   0        0        0    64017 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_shape_files.yaml
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release.yaml
+-rw-r--r--   0        0        0    16989 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_dates.yaml
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_related_tags.yaml
+-rw-r--r--   0        0        0    60220 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_series.yaml
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_sources.yaml
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_tables.yaml
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_tags.yaml
+-rw-r--r--   0        0        0   153657 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_releases.yaml
+-rw-r--r--   0        0        0    35336 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_releases_dates.yaml
+-rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series[json].yaml
+-rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series[pandas].yaml
+-rw-r--r--   0        0        0   121930 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml
+-rw-r--r--   0        0        0   121930 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml
+-rw-r--r--   0        0        0   111804 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml
+-rw-r--r--   0        0        0   111807 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_categories.yaml
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_info.yaml
+-rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml
+-rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_releases.yaml
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_tags.yaml
+-rw-r--r--   0        0        0   137616 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_updates.yaml
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_vintagedates.yaml
+-rw-r--r--   0        0        0    98930 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series[json].yaml
+-rw-r--r--   0        0        0    99086 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series[pandas].yaml
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_related_tags[json].yaml
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml
+-rw-r--r--   0        0        0    27622 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_tags[json].yaml
+-rw-r--r--   0        0        0    27627 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_tags[pandas].yaml
+-rw-r--r--   0        0        0    17912 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_add_series.yaml
+-rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_keep_realtime_cols.yaml
+-rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_list_methods_diff.yaml
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_list_methods_same.yaml
+-rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_asof.yaml
+-rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_long.yaml
+-rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_wide.yaml
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_after_add[dict].yaml
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_after_add[func].yaml
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_err.yaml
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_on_add[func].yaml
+-rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_partial.yaml
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_sources/test_get_source.yaml
+-rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_sources/test_get_source_release.yaml
+-rw-r--r--   0        0        0    18851 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_sources/test_get_sources.yaml
+-rw-r--r--   0        0        0    77768 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_tags/test_get_related_tags.yaml
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_tags/test_get_tag_series.yaml
+-rw-r--r--   0        0        0    75282 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_tags/test_get_tags.yaml
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/README.md
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/PKG-INFO
```

### Comparing `pyfredapi-0.5.4/LICENSE` & `pyfredapi-0.6.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Greg Moore
+Copyright (c) 2023 Greg Moore
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyfredapi-0.5.4/pyfredapi/__init__.py` & `pyfredapi-0.6.0/pyfredapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/_base.py` & `pyfredapi-0.6.0/pyfredapi/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import environ
 from typing import Any, Dict, Optional, Union
 
 import requests
 from frozendict import frozendict
 from pydantic import BaseModel, Extra
 
-from .exceptions import APIKeyNotFoundError, FredAPIRequestError, InvalidAPIKey
+from .exceptions import APIKeyNotFound, FredAPIRequestError, InvalidAPIKey
 from .utils._common_type_hints import JsonType
 
 
 class BaseApiParameters(BaseModel):
     """Represents the parameters accepted by all FRED Series endpoints."""
 
     api_key: str
@@ -26,15 +26,15 @@
 @lru_cache
 def _get_api_key(api_key: Optional[str] = None) -> str:
     """Get FRED_API_KEY from the environment."""
     if api_key is None:
         api_key = environ.get("FRED_API_KEY", None)
 
     if api_key is None:
-        raise APIKeyNotFoundError()
+        raise APIKeyNotFound()
     elif not api_key.isalnum() or len(api_key) != 32:
         raise InvalidAPIKey()
 
     return api_key
 
 
 @lru_cache
```

### Comparing `pyfredapi-0.5.4/pyfredapi/category.py` & `pyfredapi-0.6.0/pyfredapi/category.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/exceptions/exceptions.py` & `pyfredapi-0.6.0/pyfredapi/exceptions/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self):
         """Error raised when the API Key is invalid."""
         super().__init__(
             "API key must be a 32 character lower-cased alpha-numeric string."
         )
 
 
-class APIKeyNotFoundError(BaseFredAPIError):
+class APIKeyNotFound(BaseFredAPIError):
     """Error raised when FRED_API_KEY not found in the environment."""
 
     def __init__(self):
         super().__init__(
             """API key not found. Either set a FRED_API_KEY environment variable or pass your API key to the api_key parameter"""
         )
```

### Comparing `pyfredapi-0.5.4/pyfredapi/maps.py` & `pyfredapi-0.6.0/pyfredapi/maps.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/releases.py` & `pyfredapi-0.6.0/pyfredapi/releases.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/series.py` & `pyfredapi-0.6.0/pyfredapi/series.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/series_collection.py` & `pyfredapi-0.6.0/pyfredapi/series_collection.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/sources.py` & `pyfredapi-0.6.0/pyfredapi/sources.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/tags.py` & `pyfredapi-0.6.0/pyfredapi/tags.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyfredapi/utils/_convert_to_pandas.py` & `pyfredapi-0.6.0/pyfredapi/utils/_convert_to_pandas.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.5.4/pyproject.toml` & `pyfredapi-0.6.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,99 @@
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling>=1.14.0"]
+build-backend = "hatchling.build"
 
-[tool.poetry]
+[project]
 name = "pyfredapi"
-version = "0.5.4"
 description = "A full featured API client for the FRED API web service."
-authors = ["Greg Moore <gwmoore.career@gmail.com>"]
+authors = [
+    { name = "Greg Moore", email =  "gwmoore.career@gmail.com" }
+]
 readme = "README.md"
+license = "MIT"
+requires-python = ">=3.8"
+keywords = [
+    "fred",
+    "federal reserve",
+    "economic data",
+    "economic indicators",
+    "economic statistics",
+    "economic time series",
+    "economic data api",
+    "economic data api client",
+    "economics",
+]
 classifiers = [
     "Development Status :: 4 - Beta",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests>=2.0.0",
+    "pandas>=1.0.0",
+    "pydantic>=1.0.0",
+    "rich>=13.0.0",
+    "plotly>=5.0.0",
+    "frozendict >=2.0.0"
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+docs = [
+    "jupyter==1.0.0",
+    "Sphinx==6.1.3",
+    "myst-parser==1.0.0",
+    "nbsphinx==0.9.1",
+    "sphinxcontrib-napoleon==0.7",
+    "sphinx-copybutton==0.5.1",
+    "sphinx-material==0.0.35",
+    "autodoc-pydantic==1.8.0",
+]
+
+lint = [
+    "types-requests==2.28.11.17",
+    "types-setuptools==67.6.0.6",
+    "black[jupyter]==23.3.0",
+    "ruff==0.0.260",
+    "pandas-stubs==1.5.3.230321",
+    "mypy==1.1.1",
+    "pre-commit==3.2.1",
+    "types-frozendict==2.0.9",
+]
+
+test = [
+    "pytest==7.2.2",
+    "tox==4.4.8",
+    "coverage==7.2.2",
+    "pytest-cov==4.0.0",
+    "pytest-vcr==1.0.2",
+]
+
+dev = [
+    "pip-tools==6.13.0",
+    "pyfredapi[docs]",
+    "pyfredapi[lint]",
+    "pyfredapi[test]",
+]
+
+[tool.hatch.version]
+path = "pyfredapi/__about__.py"
+
+
+[project.urls]
+Homepage = "https://pyfredapi.readthedocs.io/en/latest/"
+Source = "https://github.com/gw-moore/pyfredapi"
 
-[tool.poetry.dependencies]
-python = ">=3.8,<4.0.0"
-requests = ">=2"
-pandas = ">=1"
-pydantic = ">=1"
-rich = ">=13"
-plotly = ">=5"
-frozendict = ">=2"
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.lint]
-optional = true
-
-[tool.poetry.group.test]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-jupyter = "^1.0.0"
-Sphinx = "^6.1.3"
-myst-parser = "^1.0.0"
-nbsphinx = "^0.9.1"
-sphinxcontrib-napoleon = "^0.7"
-sphinx-copybutton = "^0.5.1"
-sphinx-material = "^0.0.35"
-autodoc-pydantic = "^1.8.0"
-
-[tool.poetry.group.lint.dependencies]
-types-requests = "^2.28.11.17"
-types-setuptools = "^67.6.0.6"
-black = {extras = ["jupyter"], version = "^23.3.0"}
-ruff = "^0.0.260"
-# pandas-stubs = "^1.5.3.230321"
-mypy = "^1.1.1"
-pre-commit = "^3.2.1"
-types-frozendict = "^2.0.9"
-
-
-[tool.poetry.group.test.dependencies]
-pytest = "^7.2.2"
-tox = "^4.4.8"
-coverage = "^7.2.2"
-pytest-cov = "^4.0.0"
-pytest-vcr = "^1.0.2"
 
 [tool.black]
 exclude = '''
 /(
     \.git
     | \.hg
     | \.mypy_cache
@@ -94,16 +118,18 @@
     "I",  # isort
     "D",  # pydocstyle
     "S",  # flake8-bandit
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501", # Line too long
-    "D106",  # Missing docstring in public nested class
-    "D101"  # Missing docstring in public class
+    "D106", # Missing docstring in public nested class
+    "D101", # Missing docstring in public class
+    "D203", # 1 blank line required before class docstring
+    "D213"  # Multi-line docstring summary should start at the second line
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
```

