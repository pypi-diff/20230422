# Comparing `tmp/pybliometrics-3.5.1.tar.gz` & `tmp/pybliometrics-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybliometrics-3.5.1.tar", last modified: Tue Apr  4 06:47:16 2023, max compression
+gzip compressed data, was "pybliometrics-3.5.2.tar", last modified: Sat Apr 22 15:39:15 2023, max compression
```

## Comparing `pybliometrics-3.5.1.tar` & `pybliometrics-3.5.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.807745 pybliometrics-3.5.1/
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.759745 pybliometrics-3.5.1/.github/
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.763745 pybliometrics-3.5.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 panther   (1000) panther   (1000)      180 2022-01-29 14:12:14.000000 pybliometrics-3.5.1/.github/ISSUE_TEMPLATE/bug.md
--rw-rw-r--   0 panther   (1000) panther   (1000)      167 2022-01-29 14:12:14.000000 pybliometrics-3.5.1/.github/ISSUE_TEMPLATE/feature.md
--rw-rw-r--   0 panther   (1000) panther   (1000)      336 2022-01-29 14:12:14.000000 pybliometrics-3.5.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 panther   (1000) panther   (1000)      668 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/.gitignore
--rw-rw-r--   0 panther   (1000) panther   (1000)      205 2023-04-03 19:19:38.000000 pybliometrics-3.5.1/.readthedocs.yaml
--rw-r--r--   0 panther   (1000) panther   (1000)     3180 2020-09-17 08:30:44.000000 pybliometrics-3.5.1/CONTRIBUTING.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1442 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/LICENSE
--rw-rw-r--   0 panther   (1000) panther   (1000)     4991 2023-04-04 06:47:16.807745 pybliometrics-3.5.1/PKG-INFO
--rw-r--r--   0 panther   (1000) panther   (1000)     3681 2021-07-29 13:47:12.000000 pybliometrics-3.5.1/README.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.767745 pybliometrics-3.5.1/docs/
--rw-r--r--   0 panther   (1000) panther   (1000)      603 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/Makefile
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.767745 pybliometrics-3.5.1/docs/_static/
--rw-r--r--   0 panther   (1000) panther   (1000)       29 2021-08-12 15:57:23.000000 pybliometrics-3.5.1/docs/_static/custom.css
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.771745 pybliometrics-3.5.1/docs/access/
--rw-rw-r--   0 panther   (1000) panther   (1000)     3563 2023-04-03 08:15:43.000000 pybliometrics-3.5.1/docs/access/errors.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     1660 2022-03-22 18:37:38.000000 pybliometrics-3.5.1/docs/access/general.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      779 2021-07-13 23:16:28.000000 pybliometrics-3.5.1/docs/access/quotas.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      109 2021-07-13 23:10:52.000000 pybliometrics-3.5.1/docs/access.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/authors.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/changelog.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.775745 pybliometrics-3.5.1/docs/classes/
--rw-rw-r--   0 panther   (1000) panther   (1000)    11918 2022-10-13 14:21:20.000000 pybliometrics-3.5.1/docs/classes/AbstractRetrieval.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     3146 2021-07-18 12:54:48.000000 pybliometrics-3.5.1/docs/classes/AffiliationRetrieval.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     5061 2021-07-18 12:23:49.000000 pybliometrics-3.5.1/docs/classes/AffiliationSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     8325 2021-07-18 12:39:42.000000 pybliometrics-3.5.1/docs/classes/AuthorRetrieval.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     4612 2021-12-01 15:58:12.000000 pybliometrics-3.5.1/docs/classes/AuthorSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     5931 2022-03-22 18:37:38.000000 pybliometrics-3.5.1/docs/classes/CitationOverview.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     2909 2021-07-13 11:29:24.000000 pybliometrics-3.5.1/docs/classes/PlumXMetrics.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)    11226 2021-12-24 13:33:20.000000 pybliometrics-3.5.1/docs/classes/ScopusSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     4127 2021-07-18 12:09:11.000000 pybliometrics-3.5.1/docs/classes/SerialSearch.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     4971 2023-04-03 07:13:54.000000 pybliometrics-3.5.1/docs/classes/SerialTitle.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     3965 2021-07-18 12:05:52.000000 pybliometrics-3.5.1/docs/classes/SubjectClassifications.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      804 2021-07-13 09:14:45.000000 pybliometrics-3.5.1/docs/classes.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)     2726 2023-04-04 06:13:05.000000 pybliometrics-3.5.1/docs/conf.py
--rw-r--r--   0 panther   (1000) panther   (1000)     5044 2023-04-03 08:11:51.000000 pybliometrics-3.5.1/docs/configuration.rst
--rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/contributing.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1644 2021-07-13 23:03:16.000000 pybliometrics-3.5.1/docs/index.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      707 2022-02-13 08:43:09.000000 pybliometrics-3.5.1/docs/installation.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      817 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/make.bat
--rw-rw-r--   0 panther   (1000) panther   (1000)       85 2023-04-04 06:13:15.000000 pybliometrics-3.5.1/docs/requirements.txt
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.779745 pybliometrics-3.5.1/docs/tips/
--rw-r--r--   0 panther   (1000) panther   (1000)      919 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/tips/affiliations.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      133 2020-01-28 09:17:21.000000 pybliometrics-3.5.1/docs/tips/configuration.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     1325 2021-07-10 22:32:12.000000 pybliometrics-3.5.1/docs/tips/database.rst
--rw-r--r--   0 panther   (1000) panther   (1000)     4619 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/tips/migration1.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      492 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/docs/tips/rename.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      599 2020-10-05 09:11:48.000000 pybliometrics-3.5.1/docs/tips/support.rst
--rw-r--r--   0 panther   (1000) panther   (1000)      205 2021-07-18 12:31:21.000000 pybliometrics-3.5.1/docs/tips.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.783745 pybliometrics-3.5.1/meta/
--rw-r--r--   0 panther   (1000) panther   (1000)   903447 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/meta/1-s2.0-S2352711019300573-main.pdf
--rw-r--r--   0 panther   (1000) panther   (1000)      290 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/meta/AUTHORS.rst
--rw-rw-r--   0 panther   (1000) panther   (1000)    24689 2023-04-04 06:45:37.000000 pybliometrics-3.5.1/meta/CHANGES.rst
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.783745 pybliometrics-3.5.1/pybliometrics/
--rw-rw-r--   0 panther   (1000) panther   (1000)      382 2023-04-03 19:01:18.000000 pybliometrics-3.5.1/pybliometrics/__init__.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.791745 pybliometrics-3.5.1/pybliometrics/scopus/
--rw-r--r--   0 panther   (1000) panther   (1000)      615 2021-02-11 11:49:49.000000 pybliometrics-3.5.1/pybliometrics/scopus/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    12540 2021-12-11 12:14:30.000000 pybliometrics-3.5.1/pybliometrics/scopus/abstract_citation.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    38145 2022-10-13 19:09:38.000000 pybliometrics-3.5.1/pybliometrics/scopus/abstract_retrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6493 2021-07-18 21:30:04.000000 pybliometrics-3.5.1/pybliometrics/scopus/affiliation_retrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     5586 2022-02-18 19:04:12.000000 pybliometrics-3.5.1/pybliometrics/scopus/affiliation_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    16321 2022-07-12 08:56:27.000000 pybliometrics-3.5.1/pybliometrics/scopus/author_retrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6393 2022-02-18 19:04:09.000000 pybliometrics-3.5.1/pybliometrics/scopus/author_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     2381 2022-11-17 11:15:30.000000 pybliometrics-3.5.1/pybliometrics/scopus/exception.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     7245 2022-02-18 19:04:38.000000 pybliometrics-3.5.1/pybliometrics/scopus/plumx_metrics.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    11101 2022-04-07 11:01:38.000000 pybliometrics-3.5.1/pybliometrics/scopus/scopus_search.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     7068 2022-02-18 18:43:43.000000 pybliometrics-3.5.1/pybliometrics/scopus/serial_search.py
--rw-r--r--   0 panther   (1000) panther   (1000)     9861 2023-04-03 07:10:02.000000 pybliometrics-3.5.1/pybliometrics/scopus/serial_title.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     4465 2021-07-18 21:26:45.000000 pybliometrics-3.5.1/pybliometrics/scopus/subject_classifications.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.795745 pybliometrics-3.5.1/pybliometrics/scopus/superclasses/
--rw-r--r--   0 panther   (1000) panther   (1000)      166 2020-04-05 10:53:54.000000 pybliometrics-3.5.1/pybliometrics/scopus/superclasses/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     6204 2022-08-29 14:14:46.000000 pybliometrics-3.5.1/pybliometrics/scopus/superclasses/base.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     1786 2022-02-18 18:57:59.000000 pybliometrics-3.5.1/pybliometrics/scopus/superclasses/retrieval.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2693 2022-02-18 18:57:28.000000 pybliometrics-3.5.1/pybliometrics/scopus/superclasses/search.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.799745 pybliometrics-3.5.1/pybliometrics/scopus/tests/
--rw-r--r--   0 panther   (1000) panther   (1000)      668 2021-07-10 22:21:27.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/README.md
--rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-13 10:35:18.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/__init__.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    19824 2022-10-13 19:14:53.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AbstractRetrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     3420 2021-10-16 15:30:16.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AffiliationRetrieval.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1124 2021-07-13 22:10:31.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AffiliationSearch.py
--rw-rw-r--   0 panther   (1000) panther   (1000)    11224 2021-07-18 12:57:06.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AuthorRetrieval.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     1245 2021-12-01 15:58:12.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AuthorSearch.py
--rw-r--r--   0 panther   (1000) panther   (1000)     4503 2022-10-13 13:55:31.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_CitationOverview.py
--rw-r--r--   0 panther   (1000) panther   (1000)     4713 2022-04-07 08:14:21.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_PlumXMetrics.py
--rw-r--r--   0 panther   (1000) panther   (1000)     5076 2021-12-24 13:29:19.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_ScopusSearch.py
--rw-r--r--   0 panther   (1000) panther   (1000)     1309 2021-06-13 19:14:51.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_SerialSearch.py
--rw-r--r--   0 panther   (1000) panther   (1000)     4327 2023-04-03 07:10:54.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_SerialTitle.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2025 2021-02-11 11:48:13.000000 pybliometrics-3.5.1/pybliometrics/scopus/tests/test_SubjectClassifications.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.803745 pybliometrics-3.5.1/pybliometrics/scopus/utils/
--rw-r--r--   0 panther   (1000) panther   (1000)      311 2021-06-14 19:12:26.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/__init__.py
--rw-r--r--   0 panther   (1000) panther   (1000)      267 2021-02-11 07:22:49.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/checks.py
--rw-r--r--   0 panther   (1000) panther   (1000)     2541 2023-01-19 14:41:04.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/constants.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     2277 2023-04-03 07:41:51.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/create_config.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     5907 2023-04-03 18:58:03.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/get_content.py
--rw-rw-r--   0 panther   (1000) panther   (1000)     5535 2023-04-03 07:06:54.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/parse_content.py
--rw-rw-r--   0 panther   (1000) panther   (1000)      648 2022-01-01 15:13:32.000000 pybliometrics-3.5.1/pybliometrics/scopus/utils/startup.py
-drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-04 06:47:16.787745 pybliometrics-3.5.1/pybliometrics.egg-info/
--rw-rw-r--   0 panther   (1000) panther   (1000)     4991 2023-04-04 06:47:16.000000 pybliometrics-3.5.1/pybliometrics.egg-info/PKG-INFO
--rw-rw-r--   0 panther   (1000) panther   (1000)     2894 2023-04-04 06:47:16.000000 pybliometrics-3.5.1/pybliometrics.egg-info/SOURCES.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)        1 2023-04-04 06:47:16.000000 pybliometrics-3.5.1/pybliometrics.egg-info/dependency_links.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)       14 2023-04-04 06:47:16.000000 pybliometrics-3.5.1/pybliometrics.egg-info/top_level.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)     1595 2023-04-03 19:04:23.000000 pybliometrics-3.5.1/pyproject.toml
--rw-rw-r--   0 panther   (1000) panther   (1000)       25 2023-04-03 14:24:21.000000 pybliometrics-3.5.1/requirements.txt
--rw-rw-r--   0 panther   (1000) panther   (1000)       38 2023-04-04 06:47:16.807745 pybliometrics-3.5.1/setup.cfg
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.757130 pybliometrics-3.5.2/
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.637130 pybliometrics-3.5.2/.github/
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.645130 pybliometrics-3.5.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 panther   (1000) panther   (1000)      180 2022-01-29 14:12:14.000000 pybliometrics-3.5.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-rw-r--   0 panther   (1000) panther   (1000)      167 2022-01-29 14:12:14.000000 pybliometrics-3.5.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-rw-r--   0 panther   (1000) panther   (1000)      336 2022-01-29 14:12:14.000000 pybliometrics-3.5.2/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 panther   (1000) panther   (1000)      668 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/.gitignore
+-rw-rw-r--   0 panther   (1000) panther   (1000)      168 2023-04-18 19:33:38.000000 pybliometrics-3.5.2/.readthedocs.yaml
+-rw-r--r--   0 panther   (1000) panther   (1000)     3180 2020-09-17 08:30:44.000000 pybliometrics-3.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1442 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/LICENSE
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4991 2023-04-22 15:39:15.757130 pybliometrics-3.5.2/PKG-INFO
+-rw-r--r--   0 panther   (1000) panther   (1000)     3681 2021-07-29 13:47:12.000000 pybliometrics-3.5.2/README.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.653130 pybliometrics-3.5.2/docs/
+-rw-r--r--   0 panther   (1000) panther   (1000)      603 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/Makefile
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.653130 pybliometrics-3.5.2/docs/_static/
+-rw-r--r--   0 panther   (1000) panther   (1000)       29 2021-08-12 15:57:23.000000 pybliometrics-3.5.2/docs/_static/custom.css
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.657130 pybliometrics-3.5.2/docs/access/
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3563 2023-04-03 08:15:43.000000 pybliometrics-3.5.2/docs/access/errors.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1660 2022-03-22 18:37:38.000000 pybliometrics-3.5.2/docs/access/general.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      779 2021-07-13 23:16:28.000000 pybliometrics-3.5.2/docs/access/quotas.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      109 2021-07-13 23:10:52.000000 pybliometrics-3.5.2/docs/access.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/authors.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/changelog.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.665130 pybliometrics-3.5.2/docs/classes/
+-rw-rw-r--   0 panther   (1000) panther   (1000)    11918 2022-10-13 14:21:20.000000 pybliometrics-3.5.2/docs/classes/AbstractRetrieval.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3146 2021-07-18 12:54:48.000000 pybliometrics-3.5.2/docs/classes/AffiliationRetrieval.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     5061 2021-07-18 12:23:49.000000 pybliometrics-3.5.2/docs/classes/AffiliationSearch.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     8325 2021-07-18 12:39:42.000000 pybliometrics-3.5.2/docs/classes/AuthorRetrieval.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4612 2021-12-01 15:58:12.000000 pybliometrics-3.5.2/docs/classes/AuthorSearch.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     5931 2022-03-22 18:37:38.000000 pybliometrics-3.5.2/docs/classes/CitationOverview.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2909 2021-07-13 11:29:24.000000 pybliometrics-3.5.2/docs/classes/PlumXMetrics.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)    11226 2021-12-24 13:33:20.000000 pybliometrics-3.5.2/docs/classes/ScopusSearch.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4127 2021-07-18 12:09:11.000000 pybliometrics-3.5.2/docs/classes/SerialSearch.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4971 2023-04-03 07:13:54.000000 pybliometrics-3.5.2/docs/classes/SerialTitle.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3965 2021-07-18 12:05:52.000000 pybliometrics-3.5.2/docs/classes/SubjectClassifications.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      804 2021-07-13 09:14:45.000000 pybliometrics-3.5.2/docs/classes.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2664 2023-04-05 18:18:28.000000 pybliometrics-3.5.2/docs/conf.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     5044 2023-04-03 08:11:51.000000 pybliometrics-3.5.2/docs/configuration.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)       33 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/contributing.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1644 2021-07-13 23:03:16.000000 pybliometrics-3.5.2/docs/index.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      707 2022-02-13 08:43:09.000000 pybliometrics-3.5.2/docs/installation.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      817 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/make.bat
+-rw-rw-r--   0 panther   (1000) panther   (1000)       86 2023-04-18 18:52:06.000000 pybliometrics-3.5.2/docs/requirements.txt
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.669130 pybliometrics-3.5.2/docs/tips/
+-rw-r--r--   0 panther   (1000) panther   (1000)      919 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/tips/affiliations.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      133 2020-01-28 09:17:21.000000 pybliometrics-3.5.2/docs/tips/configuration.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     1325 2021-07-10 22:32:12.000000 pybliometrics-3.5.2/docs/tips/database.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)     4619 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/tips/migration1.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      492 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/docs/tips/rename.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      599 2020-10-05 09:11:48.000000 pybliometrics-3.5.2/docs/tips/support.rst
+-rw-r--r--   0 panther   (1000) panther   (1000)      205 2021-07-18 12:31:21.000000 pybliometrics-3.5.2/docs/tips.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.717130 pybliometrics-3.5.2/meta/
+-rw-r--r--   0 panther   (1000) panther   (1000)   903447 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/meta/1-s2.0-S2352711019300573-main.pdf
+-rw-r--r--   0 panther   (1000) panther   (1000)      290 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/meta/AUTHORS.rst
+-rw-rw-r--   0 panther   (1000) panther   (1000)    24805 2023-04-22 15:37:53.000000 pybliometrics-3.5.2/meta/CHANGES.rst
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.717130 pybliometrics-3.5.2/pybliometrics/
+-rw-rw-r--   0 panther   (1000) panther   (1000)      382 2023-04-03 19:01:18.000000 pybliometrics-3.5.2/pybliometrics/__init__.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.733130 pybliometrics-3.5.2/pybliometrics/scopus/
+-rw-r--r--   0 panther   (1000) panther   (1000)      615 2021-02-11 11:49:49.000000 pybliometrics-3.5.2/pybliometrics/scopus/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    12540 2021-12-11 12:14:30.000000 pybliometrics-3.5.2/pybliometrics/scopus/abstract_citation.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    38145 2022-10-13 19:09:38.000000 pybliometrics-3.5.2/pybliometrics/scopus/abstract_retrieval.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     6493 2021-07-18 21:30:04.000000 pybliometrics-3.5.2/pybliometrics/scopus/affiliation_retrieval.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     5586 2022-02-18 19:04:12.000000 pybliometrics-3.5.2/pybliometrics/scopus/affiliation_search.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    16321 2022-07-12 08:56:27.000000 pybliometrics-3.5.2/pybliometrics/scopus/author_retrieval.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     6393 2022-02-18 19:04:09.000000 pybliometrics-3.5.2/pybliometrics/scopus/author_search.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2381 2022-11-17 11:15:30.000000 pybliometrics-3.5.2/pybliometrics/scopus/exception.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     7245 2022-02-18 19:04:38.000000 pybliometrics-3.5.2/pybliometrics/scopus/plumx_metrics.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    11101 2022-04-07 11:01:38.000000 pybliometrics-3.5.2/pybliometrics/scopus/scopus_search.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     7068 2022-02-18 18:43:43.000000 pybliometrics-3.5.2/pybliometrics/scopus/serial_search.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     9861 2023-04-03 07:10:02.000000 pybliometrics-3.5.2/pybliometrics/scopus/serial_title.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4465 2021-07-18 21:26:45.000000 pybliometrics-3.5.2/pybliometrics/scopus/subject_classifications.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.737130 pybliometrics-3.5.2/pybliometrics/scopus/superclasses/
+-rw-r--r--   0 panther   (1000) panther   (1000)      166 2020-04-05 10:53:54.000000 pybliometrics-3.5.2/pybliometrics/scopus/superclasses/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     6204 2022-08-29 14:14:46.000000 pybliometrics-3.5.2/pybliometrics/scopus/superclasses/base.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1786 2022-02-18 18:57:59.000000 pybliometrics-3.5.2/pybliometrics/scopus/superclasses/retrieval.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     2693 2022-02-18 18:57:28.000000 pybliometrics-3.5.2/pybliometrics/scopus/superclasses/search.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.749130 pybliometrics-3.5.2/pybliometrics/scopus/tests/
+-rw-r--r--   0 panther   (1000) panther   (1000)      668 2021-07-10 22:21:27.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/README.md
+-rw-r--r--   0 panther   (1000) panther   (1000)        0 2020-01-13 10:35:18.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/__init__.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    19824 2022-10-13 19:14:53.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AbstractRetrieval.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     3420 2021-10-16 15:30:16.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AffiliationRetrieval.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1124 2021-07-13 22:10:31.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AffiliationSearch.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)    11224 2021-07-18 12:57:06.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AuthorRetrieval.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1245 2021-12-01 15:58:12.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AuthorSearch.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     4503 2022-10-13 13:55:31.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_CitationOverview.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     4713 2022-04-07 08:14:21.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_PlumXMetrics.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     5076 2021-12-24 13:29:19.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_ScopusSearch.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     1309 2021-06-13 19:14:51.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_SerialSearch.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     4327 2023-04-03 07:10:54.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_SerialTitle.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     2025 2021-02-11 11:48:13.000000 pybliometrics-3.5.2/pybliometrics/scopus/tests/test_SubjectClassifications.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.757130 pybliometrics-3.5.2/pybliometrics/scopus/utils/
+-rw-r--r--   0 panther   (1000) panther   (1000)      311 2021-06-14 19:12:26.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/__init__.py
+-rw-r--r--   0 panther   (1000) panther   (1000)      267 2021-02-11 07:22:49.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/checks.py
+-rw-r--r--   0 panther   (1000) panther   (1000)     2541 2023-01-19 14:41:04.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/constants.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2277 2023-04-03 07:41:51.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/create_config.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     5844 2023-04-18 18:06:20.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/get_content.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)     5535 2023-04-03 07:06:54.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/parse_content.py
+-rw-rw-r--   0 panther   (1000) panther   (1000)      648 2022-01-01 15:13:32.000000 pybliometrics-3.5.2/pybliometrics/scopus/utils/startup.py
+drwxrwxr-x   0 panther   (1000) panther   (1000)        0 2023-04-22 15:39:15.721130 pybliometrics-3.5.2/pybliometrics.egg-info/
+-rw-rw-r--   0 panther   (1000) panther   (1000)     4991 2023-04-22 15:39:15.000000 pybliometrics-3.5.2/pybliometrics.egg-info/PKG-INFO
+-rw-rw-r--   0 panther   (1000) panther   (1000)     2913 2023-04-22 15:39:15.000000 pybliometrics-3.5.2/pybliometrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)        1 2023-04-22 15:39:15.000000 pybliometrics-3.5.2/pybliometrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)       22 2023-04-22 15:39:15.000000 pybliometrics-3.5.2/pybliometrics.egg-info/requires.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)       14 2023-04-22 15:39:15.000000 pybliometrics-3.5.2/pybliometrics.egg-info/top_level.txt
+-rw-rw-r--   0 panther   (1000) panther   (1000)     1641 2023-04-18 19:28:48.000000 pybliometrics-3.5.2/pyproject.toml
+-rw-rw-r--   0 panther   (1000) panther   (1000)       38 2023-04-22 15:39:15.757130 pybliometrics-3.5.2/setup.cfg
```

### Comparing `pybliometrics-3.5.1/.gitignore` & `pybliometrics-3.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/CONTRIBUTING.rst` & `pybliometrics-3.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/LICENSE` & `pybliometrics-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/PKG-INFO` & `pybliometrics-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybliometrics
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python-based API-Wrapper to access Scopus
 Author-email: "'John Kitchin and Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pybliometrics-dev/pybliometrics
 Project-URL: Bug Tracker, https://github.com/pybliometrics-dev/pybliometrics/issues
 Project-URL: Documentation (stable), https://pybliometrics.readthedocs.io/en/stable/
```

### Comparing `pybliometrics-3.5.1/README.rst` & `pybliometrics-3.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/Makefile` & `pybliometrics-3.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/access/errors.rst` & `pybliometrics-3.5.2/docs/access/errors.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/access/general.rst` & `pybliometrics-3.5.2/docs/access/general.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/access/quotas.rst` & `pybliometrics-3.5.2/docs/access/quotas.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/AbstractRetrieval.rst` & `pybliometrics-3.5.2/docs/classes/AbstractRetrieval.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/AffiliationRetrieval.rst` & `pybliometrics-3.5.2/docs/classes/AffiliationRetrieval.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/AffiliationSearch.rst` & `pybliometrics-3.5.2/docs/classes/AffiliationSearch.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/AuthorRetrieval.rst` & `pybliometrics-3.5.2/docs/classes/AuthorRetrieval.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/AuthorSearch.rst` & `pybliometrics-3.5.2/docs/classes/AuthorSearch.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/CitationOverview.rst` & `pybliometrics-3.5.2/docs/classes/CitationOverview.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/PlumXMetrics.rst` & `pybliometrics-3.5.2/docs/classes/PlumXMetrics.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/ScopusSearch.rst` & `pybliometrics-3.5.2/docs/classes/ScopusSearch.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/SerialSearch.rst` & `pybliometrics-3.5.2/docs/classes/SerialSearch.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/SerialTitle.rst` & `pybliometrics-3.5.2/docs/classes/SerialTitle.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes/SubjectClassifications.rst` & `pybliometrics-3.5.2/docs/classes/SubjectClassifications.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/classes.rst` & `pybliometrics-3.5.2/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/conf.py` & `pybliometrics-3.5.2/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'pybliometrics'
 author = 'Michael E. Rose and John Kitchin'
 copyright = f"2017-{date.today().year} {author}"
 
-from pbr.version import VersionInfo
+import pybliometrics
 
-_v = VersionInfo('pybliometrics').semantic_version()
-version = _v.release_string()
+version = pybliometrics.__version__
 
 language = 'en'
 
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 pygments_style = 'sphinx'
 todo_include_todos = False
```

### Comparing `pybliometrics-3.5.1/docs/configuration.rst` & `pybliometrics-3.5.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/index.rst` & `pybliometrics-3.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/installation.rst` & `pybliometrics-3.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/make.bat` & `pybliometrics-3.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/tips/affiliations.rst` & `pybliometrics-3.5.2/docs/tips/affiliations.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/tips/database.rst` & `pybliometrics-3.5.2/docs/tips/database.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/tips/migration1.rst` & `pybliometrics-3.5.2/docs/tips/migration1.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/docs/tips/support.rst` & `pybliometrics-3.5.2/docs/tips/support.rst`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/meta/1-s2.0-S2352711019300573-main.pdf` & `pybliometrics-3.5.2/meta/1-s2.0-S2352711019300573-main.pdf`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/meta/CHANGES.rst` & `pybliometrics-3.5.2/meta/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Change Log
 ----------
 
 .. toctree::
 
+3.5.2
+~~~~~
+
+2023-04-22
+
+* Drop simpleJSON code and dependency.
+* Fix bug related to wrong dependency declaration.
+
 3.5.1
 ~~~~~
 
 2023-04-04
 
 * Fix bug related to installation files.
 * Use `importlib` to generate version (except for Sphinx).
```

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/__init__.py` & `pybliometrics-3.5.2/pybliometrics/scopus/__init__.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/abstract_citation.py` & `pybliometrics-3.5.2/pybliometrics/scopus/abstract_citation.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/abstract_retrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/abstract_retrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/affiliation_retrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/affiliation_retrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/affiliation_search.py` & `pybliometrics-3.5.2/pybliometrics/scopus/affiliation_search.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/author_retrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/author_retrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/author_search.py` & `pybliometrics-3.5.2/pybliometrics/scopus/author_search.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/exception.py` & `pybliometrics-3.5.2/pybliometrics/scopus/exception.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/plumx_metrics.py` & `pybliometrics-3.5.2/pybliometrics/scopus/plumx_metrics.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/scopus_search.py` & `pybliometrics-3.5.2/pybliometrics/scopus/scopus_search.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/serial_search.py` & `pybliometrics-3.5.2/pybliometrics/scopus/serial_search.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/serial_title.py` & `pybliometrics-3.5.2/pybliometrics/scopus/serial_title.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/subject_classifications.py` & `pybliometrics-3.5.2/pybliometrics/scopus/subject_classifications.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/superclasses/base.py` & `pybliometrics-3.5.2/pybliometrics/scopus/superclasses/base.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/superclasses/retrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/superclasses/retrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/superclasses/search.py` & `pybliometrics-3.5.2/pybliometrics/scopus/superclasses/search.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/README.md` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/README.md`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AbstractRetrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AbstractRetrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AffiliationRetrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AffiliationRetrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AffiliationSearch.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AffiliationSearch.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AuthorRetrieval.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AuthorRetrieval.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_AuthorSearch.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_AuthorSearch.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_CitationOverview.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_CitationOverview.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_PlumXMetrics.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_PlumXMetrics.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_ScopusSearch.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_ScopusSearch.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_SerialSearch.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_SerialSearch.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_SerialTitle.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_SerialTitle.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/tests/test_SubjectClassifications.py` & `pybliometrics-3.5.2/pybliometrics/scopus/tests/test_SubjectClassifications.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/utils/constants.py` & `pybliometrics-3.5.2/pybliometrics/scopus/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/utils/create_config.py` & `pybliometrics-3.5.2/pybliometrics/scopus/utils/create_config.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/utils/get_content.py` & `pybliometrics-3.5.2/pybliometrics/scopus/utils/get_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,14 @@
     -------
     resp : byte-like object
         The content of the file, which needs to be serialized.
     """
     from random import shuffle
     from time import sleep, time
 
-    from simplejson import JSONDecodeError
-
     from pybliometrics.scopus.utils.startup import _throttling_params, KEYS
 
     # Set header, params and proxy
     try:
         header = {'X-ELS-APIKey': KEYS[0],
                   'Accept': 'application/json',
                   'User-Agent': user_agent}
@@ -106,15 +104,15 @@
     _throttling_params[api].append(time())
 
     # Eventually raise error, if possible with supplied error message
     try:
         error_type = errors[resp.status_code]
         try:
             reason = resp.json()['service-error']['status']['statusText']
-        except (JSONDecodeError, KeyError):
+        except KeyError:
             try:
                 reason = resp.json()['message']
             except:
                 reason = ""
         raise errors[resp.status_code](reason)
     except KeyError:
         resp.raise_for_status()
```

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/utils/parse_content.py` & `pybliometrics-3.5.2/pybliometrics/scopus/utils/parse_content.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics/scopus/utils/startup.py` & `pybliometrics-3.5.2/pybliometrics/scopus/utils/startup.py`

 * *Files identical despite different names*

### Comparing `pybliometrics-3.5.1/pybliometrics.egg-info/PKG-INFO` & `pybliometrics-3.5.2/pybliometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybliometrics
-Version: 3.5.1
+Version: 3.5.2
 Summary: Python-based API-Wrapper to access Scopus
 Author-email: "'John Kitchin and Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 Maintainer-email: "Michael E. Rose" <Michael.Ernst.Rose@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pybliometrics-dev/pybliometrics
 Project-URL: Bug Tracker, https://github.com/pybliometrics-dev/pybliometrics/issues
 Project-URL: Documentation (stable), https://pybliometrics.readthedocs.io/en/stable/
```

### Comparing `pybliometrics-3.5.1/pybliometrics.egg-info/SOURCES.txt` & `pybliometrics-3.5.2/pybliometrics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 .readthedocs.yaml
 CONTRIBUTING.rst
 LICENSE
 README.rst
 pyproject.toml
-requirements.txt
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/question.md
 docs/Makefile
 docs/access.rst
 docs/authors.rst
 docs/changelog.rst
@@ -45,14 +44,15 @@
 meta/1-s2.0-S2352711019300573-main.pdf
 meta/AUTHORS.rst
 meta/CHANGES.rst
 pybliometrics/__init__.py
 pybliometrics.egg-info/PKG-INFO
 pybliometrics.egg-info/SOURCES.txt
 pybliometrics.egg-info/dependency_links.txt
+pybliometrics.egg-info/requires.txt
 pybliometrics.egg-info/top_level.txt
 pybliometrics/scopus/__init__.py
 pybliometrics/scopus/abstract_citation.py
 pybliometrics/scopus/abstract_retrieval.py
 pybliometrics/scopus/affiliation_retrieval.py
 pybliometrics/scopus/affiliation_search.py
 pybliometrics/scopus/author_retrieval.py
```

### Comparing `pybliometrics-3.5.1/pyproject.toml` & `pybliometrics-3.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 [project]
 name = "pybliometrics"
 authors = [{name = "'John Kitchin and Michael E. Rose", email = "Michael.Ernst.Rose@gmail.com"}]
 maintainers = [{name = "Michael E. Rose", email = "Michael.Ernst.Rose@gmail.com"}]
 description = "Python-based API-Wrapper to access Scopus"
 readme = "README.rst"
 license = {text = "MIT"}
+dependencies = [
+    "requests",
+    "tqdm",
+    "urllib3",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.6",
@@ -20,15 +25,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Information Analysis",
 ]
 keywords = ["scopus"]
-dynamic = ["version", "dependencies"]
+dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pybliometrics-dev/pybliometrics"
 "Bug Tracker" = "https://github.com/pybliometrics-dev/pybliometrics/issues"
 "Documentation (stable)" = "https://pybliometrics.readthedocs.io/en/stable/"
 "Documentation (latest)" = "https://pybliometrics.readthedocs.io/en/latest/"
```

