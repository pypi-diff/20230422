# Comparing `tmp/copier_template_tester-1.0.2.tar.gz` & `tmp/copier_template_tester-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier_template_tester-1.0.2.tar", max compression
+gzip compressed data, was "copier_template_tester-1.1.0.tar", max compression
```

## Comparing `copier_template_tester-1.0.2.tar` & `copier_template_tester-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1066 2022-11-20 18:06:32.236067 copier_template_tester-1.0.2/LICENSE
--rw-r--r--   0        0        0      197 2022-11-21 03:43:31.887221 copier_template_tester-1.0.2/copier_template_tester/__init__.py
--rw-r--r--   0        0        0     2499 2022-11-21 03:33:45.676125 copier_template_tester-1.0.2/copier_template_tester/main.py
--rw-r--r--   0        0        0     3289 2022-11-21 03:43:52.235133 copier_template_tester-1.0.2/docs/README.md
--rw-r--r--   0        0        0     1713 2022-11-21 03:43:31.908228 copier_template_tester-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 copier_template_tester-1.0.2/setup.py
--rw-r--r--   0        0        0     4408 1970-01-01 00:00:00.000000 copier_template_tester-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 20:25:06.309423 copier_template_tester-1.1.0/LICENSE
+-rw-r--r--   0        0        0      197 2023-04-22 05:28:52.956518 copier_template_tester-1.1.0/copier_template_tester/__init__.py
+-rw-r--r--   0        0        0     4624 2023-04-22 05:22:37.340488 copier_template_tester-1.1.0/copier_template_tester/main.py
+-rw-r--r--   0        0        0     3438 2023-04-22 05:28:58.497540 copier_template_tester-1.1.0/docs/README.md
+-rw-r--r--   0        0        0     1445 2023-04-22 05:28:52.972477 copier_template_tester-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 copier_template_tester-1.1.0/PKG-INFO
```

### Comparing `copier_template_tester-1.0.2/LICENSE` & `copier_template_tester-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `copier_template_tester-1.0.2/docs/README.md` & `copier_template_tester-1.1.0/docs/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 cd ~/your/copier/project
 ctt
 ```
 
 ### More Examples
 
-For more example code, see the [tests] directory or how this utility is used in a real project: [KyleKing/calcipy_template](https://github.com/KyleKing/calcipy_template)
+For more example code, see the [scripts] directory or the [tests].
 
 ## Project Status
 
 See the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].
 
 ## Contributing
 
@@ -89,24 +89,25 @@
 
 ## Code of Conduct
 
 We follow the [Contributor Covenant Code of Conduct][contributor-covenant].
 
 ### Open Source Status
 
-We try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/copier_template_tester)
+We try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/copier-template-tester)
 
 ## Responsible Disclosure
 
 If you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).
 
 ## License
 
 [LICENSE]
 
-[changelog]: ./docs/CHANGELOG.md
-[code_tag_summary]: ./docs/CODE_TAG_SUMMARY.md
+[changelog]: https://copier-template-tester.kyleking.me/docs/CHANGELOG
+[code_tag_summary]: https://copier-template-tester.kyleking.me/docs/CODE_TAG_SUMMARY
 [contributor-covenant]: https://www.contributor-covenant.org
-[developer_guide]: ./docs/DEVELOPER_GUIDE.md
-[license]: https://github.com/kyleking/copier-template-tester/LICENSE
-[style_guide]: ./docs/STYLE_GUIDE.md
-[tests]: https://github.com/kyleking/copier-template-tester/tests
+[developer_guide]: https://copier-template-tester.kyleking.me/docs/DEVELOPER_GUIDE
+[license]: https://github.com/kyleking/copier-template-tester/blob/main/LICENSE
+[scripts]: https://github.com/kyleking/copier-template-tester/blob/main/scripts
+[style_guide]: https://copier-template-tester.kyleking.me/docs/STYLE_GUIDE
+[tests]: https://github.com/kyleking/copier-template-tester/blob/main/tests
```

### Comparing `copier_template_tester-1.0.2/PKG-INFO` & `copier_template_tester-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: copier-template-tester
-Version: 1.0.2
+Version: 1.1.0
 Summary: Test copier templates
 Home-page: https://github.com/kyleking/copier-template-tester
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.10.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beartype (>=0.11.0)
 Requires-Dist: copier (>=7.0.1)
-Requires-Dist: tomli (>=2.0.1); python_version < "3.11"
+Requires-Dist: corallium (>=0.2.0)
 Project-URL: Bug Tracker, https://github.com/kyleking/copier-template-tester/issues
 Project-URL: Changelog, https://github.com/kyleking/copier-template-tester/blob/main/docs/docs/CHANGELOG.md
-Project-URL: Documentation, https://github.com/kyleking/copier-template-tester/docs
+Project-URL: Documentation, https://copier-template-tester.kyleking.me
 Project-URL: Repository, https://github.com/kyleking/copier-template-tester
 Description-Content-Type: text/markdown
 
 # copier-template-tester
 
 ![./ctt-logo.png](./ctt-logo.png)
 
@@ -95,15 +94,15 @@
 
 cd ~/your/copier/project
 ctt
 ```
 
 ### More Examples
 
-For more example code, see the [tests] directory or how this utility is used in a real project: [KyleKing/calcipy_template](https://github.com/KyleKing/calcipy_template)
+For more example code, see the [scripts] directory or the [tests].
 
 ## Project Status
 
 See the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].
 
 ## Contributing
 
@@ -114,25 +113,26 @@
 
 ## Code of Conduct
 
 We follow the [Contributor Covenant Code of Conduct][contributor-covenant].
 
 ### Open Source Status
 
-We try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/copier_template_tester)
+We try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/copier-template-tester)
 
 ## Responsible Disclosure
 
 If you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).
 
 ## License
 
 [LICENSE]
 
-[changelog]: ./docs/CHANGELOG.md
-[code_tag_summary]: ./docs/CODE_TAG_SUMMARY.md
+[changelog]: https://copier-template-tester.kyleking.me/docs/CHANGELOG
+[code_tag_summary]: https://copier-template-tester.kyleking.me/docs/CODE_TAG_SUMMARY
 [contributor-covenant]: https://www.contributor-covenant.org
-[developer_guide]: ./docs/DEVELOPER_GUIDE.md
-[license]: https://github.com/kyleking/copier-template-tester/LICENSE
-[style_guide]: ./docs/STYLE_GUIDE.md
-[tests]: https://github.com/kyleking/copier-template-tester/tests
+[developer_guide]: https://copier-template-tester.kyleking.me/docs/DEVELOPER_GUIDE
+[license]: https://github.com/kyleking/copier-template-tester/blob/main/LICENSE
+[scripts]: https://github.com/kyleking/copier-template-tester/blob/main/scripts
+[style_guide]: https://copier-template-tester.kyleking.me/docs/STYLE_GUIDE
+[tests]: https://github.com/kyleking/copier-template-tester/blob/main/tests
```

