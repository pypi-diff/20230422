# Comparing `tmp/cushy-storage-1.0.1.tar.gz` & `tmp/cushy-storage-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cushy-storage-1.0.1.tar", last modified: Fri Apr 14 11:53:32 2023, max compression
+gzip compressed data, was "/home/runner/work/cushy-storage/cushy-storage/dist/.tmp-ukl_go3c/cushy-storage-1.0.2.tar", last modified: Sat Apr 22 08:52:11 2023, max compression
```

## Comparing `cushy-storage-1.0.1.tar` & `cushy-storage-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 cushy-storage-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5234 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4356 2023-04-14 11:53:05.000000 cushy-storage-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage/
--rw-rw-rw-   0        0        0      827 2023-03-13 14:13:17.000000 cushy-storage-1.0.1/cushy_storage/__init__.py
--rw-rw-rw-   0        0        0     6133 2023-04-14 11:51:52.000000 cushy-storage-1.0.1/cushy_storage/_core.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/
--rw-rw-rw-   0        0        0     5234 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1814 2023-04-14 11:53:31.000000 cushy-storage-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/tests/
--rw-rw-rw-   0        0        0     1971 2023-03-18 07:38:01.000000 cushy-storage-1.0.1/tests/test_base_dict.py
--rw-rw-rw-   0        0        0     1804 2023-03-18 08:01:59.000000 cushy-storage-1.0.1/tests/test_cushy_dict.py
--rw-rw-rw-   0        0        0     2365 2023-03-13 14:39:24.000000 cushy-storage-1.0.1/tests/test_dict_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/cushy_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/cushy_storage/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/cushy_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:52:11.000000 cushy-storage-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/tests/test_base_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/tests/test_cushy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-22 08:51:59.000000 cushy-storage-1.0.2/tests/test_dict_cache.py
```

### Comparing `cushy-storage-1.0.1/LICENSE` & `cushy-storage-1.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `cushy-storage-1.0.1/PKG-INFO` & `cushy-storage-1.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,144 +1,183 @@
-Metadata-Version: 2.1
-Name: cushy-storage
-Version: 1.0.1
-Summary: A data local persistence framework library
-Home-page: https://github.com/Undertone0809/cushy-storage
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: storage,serialization,json,cushy-storage,cushy_storage
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    cushy-storage
-</h1>
-<p align="center">
-  <strong>一个基于磁盘缓存的Python框架</strong>
-</p>
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
-   </a>
-    <a target="_blank" href=''>
-        <img src="https://static.pepy.tech/personalized-badge/cushy-socket?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
-   </a>
-</p>
-
-[English](/README_en.md) [中文](/README.md)
-
-# 简介
-cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。
-
-# 特性
-- 可以方便的将数据进行本地磁盘存储
-- 免去了直接操作文件的工作
-- 像操作dict一样读写，十分方便
-- 提供序列化操作
-- 提供多种数据压缩方式
-
-
-# 安装
-
-```bash
-pip install cushy-storage --upgrade 
-```
-
-# 快速上手
-
-`cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
-`BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
-
-## BaseDict类
-
-BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
-
-```python
-from cushy_storage import BaseDict
-
-# 初始化cache，保存在./data文件夹下
-cache = BaseDict('./data')
-cache['key'] = b'value'
-value = cache['key']
-print(value)
-
-```
-
-## CushyDict类
-
-CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
-
-```python
-from cushy_storage import CushyDict
-
-# 初始化cache，保存在./data文件夹下
-cache = CushyDict('./data')
-cache['key'] = {'value': 42}
-value = cache['key']
-print(value)
-
-```
-
-- 判断key是否存在
-
-```python
-from cushy_storage import CushyDict
-
-cache = CushyDict('./data')
-if 'key' in cache:
-    print("key exist")
-else:
-    print("key not exist")
-
-```
-
-## disk_cache装饰器函数
-
-disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
-
-```python
-from cushy_storage import disk_cache
-
-@disk_cache('./data')
-def my_func():
-    return {'value': 42}
-
-result = my_func()
-
-```
- 
- 
-# 待办
-
-- [ ] 提供单例模式解决方案，提供更加方便的磁盘缓存方案
-- [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
-- [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
-- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
-- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
-- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
-- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
-- [ ] 改善文档结构和代码注释，方便用户理解和使用库
-- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
-- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
-
-# 鸣谢
-本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage) 进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
-
-This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to RimoChan for his great work.
-
-# 贡献
-如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
+<h1 align="center">
+    cushy-storage
+</h1>
+<p align="center">
+  <strong>一个基于磁盘缓存的Python框架</strong>
+</p>
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/broadcast-service?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Total"/>
+   </a>
+    <a target="_blank" href=''>
+        <img src="https://static.pepy.tech/personalized-badge/cushy-socket?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/Week"/>
+   </a>
+</p>
+
+[English](/README_en.md) [中文](/README.md)
+
+# 简介
+cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。另一方面，
+cushy-storage让你无需花费精力在如何制订一套数据存储规范上，字典般的操作可以减少很多开发的成本。
+
+# 特性
+- 可以方便的将数据进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 像操作dict一样读写，十分方便
+- 提供序列化操作
+- 提供多种数据压缩方式
+
+
+# 安装
+
+```bash
+pip install cushy-storage --upgrade 
+```
+
+# 快速上手
+
+`cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
+`BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
+
+## BaseDict类
+
+BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
+
+```python
+from cushy_storage import BaseDict
+
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
+# Base Dict只能存储二进制数据，可以用于流式传输
+cache['key'] = b'value'
+value = cache['key']
+print(value)
+
+```
+
+## CushyDict类
+
+CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化，下面是一些简单的使用教程。
+
+```python
+from cushy_storage import CushyDict
+
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
+
+cache['key'] = {'value': 42}
+print(cache['key'])
+
+cache['a'] = 1
+print(cache['a'])
+
+cache['b'] = "hello world"
+print(cache['b'])
+
+cache['arr'] = [1,2,3,4,5]
+print(cache['arr'])
+
+```
+
+- 生成结果
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210730.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210837.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210825.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210809.png"/>
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230416210757.png"/>
+
+- 如果在初始化的时候不传入参数，则默认保存在`./data`文件夹下
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict()
+```
+
+
+- 判断key是否存在（和字典操作同理）
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict('./data')
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
+
+```
+
+- 用`CushyDict`存储对象信息
+
+```python
+from cushy_storage import CushyDict
+
+
+class User:
+    def __init__(self, name, age):
+        self.name = name
+        self.age = age
+
+
+def main():
+    cache = CushyDict('./data', serialize='pickle')
+    user = User("Jack", 18)
+    cache['user'] = user
+
+    print(cache['user'].name)
+    print(cache['user'].age)
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+
+## disk_cache装饰器函数
+
+disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
+
+```python
+from cushy_storage import disk_cache
+
+@disk_cache('./data')
+def my_func():
+    return {'value': 42}
+
+result = my_func()
+
+```
+ 
+ 
+# 待办
+
+- [ ] 提供单例模式解决方案，提供更加方便的工具类
+- [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
+- [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
+- [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
+- [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
+- [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
+- [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
+- [ ] 改善文档结构和代码注释，方便用户理解和使用库
+- [ ] 支持Python3中的异步IO，提高程序的并发性和性能
+- [ ] 增加基于内存的缓存组件，可以更加灵活地选择缓存存储方式
+- [ ] 支持更多数据格式的持久化方式，如json,xml的直接存储
+- [ ] 提供ORM框架，封装对象级的CRUD操作
+
+# 鸣谢
+本项目基于[https://github.com/RimoChan/rimo_storage](https://github.com/RimoChan/rimo_storage) 进行二次开发改进，感谢[RimoChan](https://github.com/RimoChan) 大佬。
+
+This project is based on https://github.com/RimoChan/rimo_storage for secondary development and improvement. Thanks to RimoChan for his great work.
+
+# 贡献
+如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `cushy-storage-1.0.1/cushy_storage/_core.py` & `cushy-storage-1.0.2/cushy_storage/_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,196 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import os
-import zlib
-import lzma
-import json
-import pickle
-import hashlib
-import threading
-from pathlib import Path
-from typing import MutableMapping, Callable, Tuple, Union, Any
-
-__all__ = ['BaseDict', 'CushyDict', 'disk_cache']
-
-# Compression algorithms and their corresponding functions
-_COMPRESS = {
-    'zlib': (
-        zlib.compress,
-        zlib.decompress,
-    ),
-    'lzma': (
-        lzma.compress,
-        lzma.decompress,
-    ),
-}
-
-# Serialization algorithms and their corresponding functions
-_SERIALIZATION = {
-    'pickle': (
-        pickle.dumps,
-        pickle.loads,
-    ),
-    'json': (
-        lambda x: json.dumps(x, sort_keys=True, ensure_ascii=False, separators=(',', ':')).encode('utf8'),
-        json.loads,
-    ),
-}
-
-# Locks for each hash value (hexadecimal representation of 0-255)
-_LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
-_F = Union[str, Tuple[Callable, Callable], None]
-
-
-def _cf(s: _F, d: dict) -> Tuple[Callable, Callable]:
-    """
-    Helper function to get the compression or serialization functions based on input parameter
-    """
-    if s is None:
-        return lambda x: x, lambda x: x
-    elif isinstance(s, str):
-        return d[s]
-    else:
-        return s
-
-
-class BaseDict(MutableMapping[str, bytes]):
-    def __init__(self, path: str, compress: _F = None):
-        self.path = Path(path)
-        if self.path.is_file():
-            raise Exception('path has exist')  # Raise an exception if the path already exists as a file
-        self.path.mkdir(parents=True, exist_ok=True)
-        self.dirs = set()
-        self.compress, self.decompress = _cf(compress, _COMPRESS)
-
-    def __contains__(self, k: str):
-        # Check if the file exists in the cache
-        return (self.path / k[:2] / (k[2:] + '_')).is_file()
-
-    def __getitem__(self, k: str):
-        # Retrieve the cached item using its key and decompress it
-        if k not in self:
-            raise KeyError(k)
-        rk = hashlib.md5(k.encode('utf8')).hexdigest()[:2]
-        with _LOCKS[rk]:
-            with open(self.path / k[:2] / (k[2:] + '_'), 'rb') as f:
-                t = f.read()
-        return self.decompress(t)
-
-    def __setitem__(self, k: str, v: bytes):
-        # Compress the value and store it in the cache using its key
-        if k[:2] not in self.dirs:
-            (self.path / k[:2]).mkdir(exist_ok=True)
-            self.dirs.add(k[:2])
-        t = self.compress(v)
-        rk = hashlib.md5(k.encode('utf8')).hexdigest()[:2]
-        with _LOCKS[rk]:
-            with open(self.path / k[:2] / (k[2:] + '_'), 'wb') as f:
-                f.write(t)
-
-    def __delitem__(self, k: str):
-        # Remove the cached item using its key
-        os.remove(self.path / k[:2] / (k[2:] + '_'))
-
-    def __len__(self):
-        # Get the total number of items in the cache
-        return sum([len(os.listdir(self.path / a)) for a in os.listdir(self.path)])
-
-    def __iter__(self):
-        # Iterate over all keys in the cache
-        for a in os.listdir(self.path):
-            for b in os.listdir(self.path / a):
-                yield a + b[:-1]
-
-
-class CushyDict(BaseDict):
-    """
-    A subclass of BaseDict that can serialize and deserialize values using different algorithms
-    """
-
-    def __init__(self, path: str, compress: _F = None, serialize: _F = 'json'):
-        """
-
-        :param path: the path to save
-        :param compress: zlib or lzma
-        :param serialize: json or pickle
-        """
-        super().__init__(path, compress)
-        self.serialize, self.deserialize = _cf(serialize, _SERIALIZATION)
-
-    def __getitem__(self, k: str):
-        return self.deserialize(super().__getitem__(k))
-
-    def __setitem__(self, k: str, v: Any):
-        return super().__setitem__(k, self.serialize(v))
-
-
-_EXT = {
-    'pickle': 'pkl',
-    'json': 'json',
-}
-
-
-def disk_cache(path: str = None, compress: str = None, serialize: str = 'json'):
-    """
-    Decorator that caches the output of a function to disk
-    """
-    ext = _EXT.get(serialize, '_')
-    dump = _cf(serialize, _SERIALIZATION)[0]
-
-    def decorator(func):
-        nonlocal path
-        name = func.__name__
-        if path is None:
-            # If no cache path is specified, create a default one based on the function name and serialization algorithm
-            path = f'./_cushycache_{name}_{serialize}'
-        map = CushyDict(path, serialize=serialize, compress=compress)
-
-        def cached_func(*args, **kwargs):
-            # Serialize the function arguments and use their MD5 hash as the cache key
-            input_data = [name, args, kwargs]
-            md5 = hashlib.md5(dump(input_data)).hexdigest()
-            filename = f'{md5}.{ext}'
-
-            if filename in map:
-                # If the cached output exists, return it
-                input_data, output_data = map[filename]
-                return output_data
-            else:
-                # Otherwise, call the original function and cache its output
-                output_data = func(*args, **kwargs)
-                cache_data = [input_data, output_data]
-                map[filename] = cache_data
-                return output_data
-
-        return cached_func
-
-    return decorator
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import os
+import zlib
+import lzma
+import json
+import pickle
+import hashlib
+import threading
+from pathlib import Path
+from typing import MutableMapping, Callable, Tuple, Union, Any
+
+__all__ = ['BaseDict', 'CushyDict', 'disk_cache']
+
+# Compression algorithms and their corresponding functions
+_COMPRESS = {
+    'zlib': (
+        zlib.compress,
+        zlib.decompress,
+    ),
+    'lzma': (
+        lzma.compress,
+        lzma.decompress,
+    ),
+}
+
+# Serialization algorithms and their corresponding functions
+_SERIALIZATION = {
+    'pickle': (
+        pickle.dumps,
+        pickle.loads,
+    ),
+    'json': (
+        lambda x: json.dumps(x, sort_keys=True, ensure_ascii=False, separators=(',', ':')).encode('utf8'),
+        json.loads,
+    ),
+}
+
+# Locks for each hash value (hexadecimal representation of 0-255)
+_LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
+_F = Union[str, Tuple[Callable, Callable], None]
+
+
+def _cf(s: _F, d: dict) -> Tuple[Callable, Callable]:
+    """
+    Helper function to get the compression or serialization functions based on input parameter
+    """
+    if s is None:
+        return lambda x: x, lambda x: x
+    elif isinstance(s, str):
+        return d[s]
+    else:
+        return s
+
+
+class BaseDict(MutableMapping[str, bytes]):
+    def __init__(self, path: str, compress: _F = None):
+        self.path = Path(path)
+        if self.path.is_file():
+            raise Exception('path has exist')  # Raise an exception if the path already exists as a file
+        self.path.mkdir(parents=True, exist_ok=True)
+        self.dirs = set()
+        self.compress, self.decompress = _cf(compress, _COMPRESS)
+
+    def __contains__(self, k: str):
+        """
+        Check if the file exists in the cache
+        """
+        return (self.path / k[:2] / (k[2:] + '_')).is_file()
+
+    def __getitem__(self, k: str):
+        """
+        Retrieve the cached item using its key and decompress it
+        """
+        if k not in self:
+            raise KeyError(k)
+        rk = hashlib.md5(k.encode('utf8')).hexdigest()[:2]
+        with _LOCKS[rk]:
+            with open(self.path / k[:2] / (k[2:] + '_'), 'rb') as f:
+                t = f.read()
+        return self.decompress(t)
+
+    def __setitem__(self, k: str, v: bytes):
+        """
+        Compress the value and store it in the cache using its key
+        """
+        if k[:2] not in self.dirs:
+            (self.path / k[:2]).mkdir(exist_ok=True)
+            self.dirs.add(k[:2])
+        t = self.compress(v)
+        rk = hashlib.md5(k.encode('utf8')).hexdigest()[:2]
+        with _LOCKS[rk]:
+            with open(self.path / k[:2] / (k[2:] + '_'), 'wb') as f:
+                f.write(t)
+
+    def __delitem__(self, k: str):
+        """
+        Remove the cached item using its key
+        """
+        os.remove(self.path / k[:2] / (k[2:] + '_'))
+
+    def __len__(self):
+        """
+        Get the total number of items in the cache
+        """
+        return sum([len(os.listdir(self.path / a)) for a in os.listdir(self.path)])
+
+    def __iter__(self):
+        """
+        Iterate over all keys in the cache
+        """
+        for a in os.listdir(self.path):
+            for b in os.listdir(self.path / a):
+                yield a + b[:-1]
+
+
+class CushyDict(BaseDict):
+    """
+    A subclass of BaseDict that can serialize and deserialize values using different algorithms
+    """
+
+    def __init__(self, path: str = './data', compress: _F = None, serialize: _F = 'json'):
+        """
+        Args:
+            path: the path to save
+            compress: zlib or lzma
+            serialize: json or pickle
+        """
+        super().__init__(path, compress)
+        self.serialize, self.deserialize = _cf(serialize, _SERIALIZATION)
+
+    def __getitem__(self, k: str):
+        return self.deserialize(super().__getitem__(k))
+
+    def __setitem__(self, k: str, v: Any):
+        return super().__setitem__(k, self.serialize(v))
+
+
+_EXT = {
+    'pickle': 'pkl',
+    'json': 'json',
+}
+
+
+def disk_cache(path: str = None, compress: str = None, serialize: str = 'json'):
+    """
+    Decorator that caches the output of a function to disk
+    """
+    ext = _EXT.get(serialize, '_')
+    dump = _cf(serialize, _SERIALIZATION)[0]
+
+    def decorator(func):
+        nonlocal path
+        name = func.__name__
+        if path is None:
+            # If no cache path is specified, create a default one based on the function name and serialization algorithm
+            path = f'./_cushycache_{name}_{serialize}'
+        map = CushyDict(path, serialize=serialize, compress=compress)
+
+        def cached_func(*args, **kwargs):
+            # Serialize the function arguments and use their MD5 hash as the cache key
+            input_data = [name, args, kwargs]
+            md5 = hashlib.md5(dump(input_data)).hexdigest()
+            filename = f'{md5}.{ext}'
+
+            if filename in map:
+                # If the cached output exists, return it
+                input_data, output_data = map[filename]
+                return output_data
+            else:
+                # Otherwise, call the original function and cache its output
+                output_data = func(*args, **kwargs)
+                cache_data = [input_data, output_data]
+                map[filename] = cache_data
+                return output_data
+
+        return cached_func
+
+    return decorator
```

### Comparing `cushy-storage-1.0.1/setup.py` & `cushy-storage-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import setuptools
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setuptools.setup(
-    name="cushy-storage",
-    version="1.0.1",
-    author="Zeeland",
-    author_email="zeeland@foxmail.com",
-    description="A data local persistence framework library",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Undertone0809/cushy-storage",
-    packages=setuptools.find_packages(),
-    license="Apache 2.0",
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-
-    ],
-    keywords="storage, serialization, json, cushy-storage, cushy_storage",
-)
+# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import setuptools
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+setuptools.setup(
+    name="cushy-storage",
+    version="1.0.2",
+    author="Zeeland",
+    author_email="zeeland@foxmail.com",
+    description="A data local persistence framework library",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Undertone0809/cushy-storage",
+    packages=setuptools.find_packages(),
+    license="Apache 2.0",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+
+    ],
+    keywords="storage, serialization, json, cushy-storage, cushy_storage",
+)
```

### Comparing `cushy-storage-1.0.1/tests/test_base_dict.py` & `cushy-storage-1.0.2/tests/test_base_dict.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import unittest
-from cushy_storage import CushyDict
-
-
-class TestBaseDict(unittest.TestCase):
-    def test_basic_operations(self):
-        cache = CushyDict('./test-cache')
-
-        # Test adding items to the cache
-        cache['foo'] = b'bar'
-        self.assertEqual(cache['foo'], b'bar')
-
-        # Test deleting items from the cache
-        del cache['foo']
-        with self.assertRaises(KeyError):
-            cache['foo']
-
-        # Test checking if an item is in the cache
-        self.assertFalse('foo' in cache)
-
-    def test_serialization(self):
-        cache = CushyDict('./test-cache', serialize='pickle')
-
-        # Test storing and retrieving a dictionary in the cache using pickle serialization
-        cache['data'] = {'foo': 'bar', 'baz': [1, 2, 3]}
-        self.assertEqual(cache['data'], {'foo': 'bar', 'baz': [1, 2, 3]})
-
-    def test_compression(self):
-        cache = CushyDict('./test-cache', compress='lzma')
-
-        # Test storing and retrieving a large string in the cache using LZMA compression
-        data = 'a' * (1024 * 1024)
-        cache['big_data'] = data.encode()
-        self.assertEqual(cache['big_data'].decode(), data)
-
-
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import unittest
+from cushy_storage import CushyDict
+
+
+class TestBaseDict(unittest.TestCase):
+    def test_basic_operations(self):
+        cache = CushyDict('./test-cache')
+
+        # Test adding items to the cache
+        cache['foo'] = b'bar'
+        self.assertEqual(cache['foo'], b'bar')
+
+        # Test deleting items from the cache
+        del cache['foo']
+        with self.assertRaises(KeyError):
+            cache['foo']
+
+        # Test checking if an item is in the cache
+        self.assertFalse('foo' in cache)
+
+    def test_serialization(self):
+        cache = CushyDict('./test-cache', serialize='pickle')
+
+        # Test storing and retrieving a dictionary in the cache using pickle serialization
+        cache['data'] = {'foo': 'bar', 'baz': [1, 2, 3]}
+        self.assertEqual(cache['data'], {'foo': 'bar', 'baz': [1, 2, 3]})
+
+    def test_compression(self):
+        cache = CushyDict('./test-cache', compress='lzma')
+
+        # Test storing and retrieving a large string in the cache using LZMA compression
+        data = 'a' * (1024 * 1024)
+        cache['big_data'] = data.encode()
+        self.assertEqual(cache['big_data'].decode(), data)
+
+
```

### Comparing `cushy-storage-1.0.1/tests/test_cushy_dict.py` & `cushy-storage-1.0.2/tests/test_cushy_dict.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import unittest
-from cushy_storage import CushyDict
-
-
-class TestCushyDict(unittest.TestCase):
-    def test_read_and_write_data(self):
-        cache = CushyDict("./test-cache")
-        cache['a'] = 10
-        self.assertEqual(cache['a'], 10)
-
-        cache['b'] = "test"
-        self.assertEqual(cache['b'], "test")
-
-        cache['c'] = [1, 2, 3, 4]
-        self.assertEqual(cache['c'], [1, 2, 3, 4])
-
-        cache['d'] = {"key": "value"}
-        self.assertEqual(cache['d'], {"key": "value"})
-
-        cache['e'] = ("hello", 1)
-        print(type(cache['e']))
-        self.assertEqual(cache['e'], ["hello", 1])
-
-    def test_data_type(self):
-        cache = CushyDict("./test-cache")
-        self.assertEqual(type(cache['a']), int)
-        self.assertEqual(type(cache['b']), str)
-        self.assertEqual(type(cache['c']), list)
-        self.assertEqual(type(cache['d']), dict)
-        # todo https://github.com/Undertone0809/cushy-stroage/issues/1
-        self.assertEqual(type(cache['e']), list)
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import unittest
+from cushy_storage import CushyDict
+
+
+class TestCushyDict(unittest.TestCase):
+    def test_read_and_write_data(self):
+        cache = CushyDict("./test-cache")
+        cache['a'] = 10
+        self.assertEqual(cache['a'], 10)
+
+        cache['b'] = "test"
+        self.assertEqual(cache['b'], "test")
+
+        cache['c'] = [1, 2, 3, 4]
+        self.assertEqual(cache['c'], [1, 2, 3, 4])
+
+        cache['d'] = {"key": "value"}
+        self.assertEqual(cache['d'], {"key": "value"})
+
+        cache['e'] = ("hello", 1)
+        print(type(cache['e']))
+        self.assertEqual(cache['e'], ["hello", 1])
+
+    def test_data_type(self):
+        cache = CushyDict("./test-cache")
+        self.assertEqual(type(cache['a']), int)
+        self.assertEqual(type(cache['b']), str)
+        self.assertEqual(type(cache['c']), list)
+        self.assertEqual(type(cache['d']), dict)
+        # todo https://github.com/Undertone0809/cushy-stroage/issues/1
+        self.assertEqual(type(cache['e']), list)
```

### Comparing `cushy-storage-1.0.1/tests/test_dict_cache.py` & `cushy-storage-1.0.2/tests/test_dict_cache.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/cushy-storage
-# Contact Email: zeeland@foxmail.com
-
-import time
-import unittest
-from cushy_storage import CushyDict, disk_cache
-
-
-class TestDiskCache(unittest.TestCase):
-    def test_basic_usage(self):
-        @disk_cache('./test-disk-cache')
-        def slow_function(x):
-            time.sleep(0.1)
-            return x + 1
-
-        # Test calling the function with different arguments and caching the output
-        self.assertEqual(slow_function(5), 6)
-        self.assertEqual(slow_function(5), 6)  # Should use cache this time
-        self.assertEqual(slow_function(10), 11)
-
-    def test_serialization(self):
-        @disk_cache('./test-disk-cache-serialize', serialize='pickle')
-        def slow_function(x):
-            time.sleep(0.1)
-            return {'result': x}
-
-        # Test caching the output of a function that returns a dictionary using pickle serialization
-        self.assertEqual(slow_function(5), {'result': 5})
-        self.assertEqual(slow_function(5), {'result': 5})  # Should use cache this time
-        self.assertEqual(slow_function(10), {'result': 10})
-
-    def test_compression(self):
-        @disk_cache('./test-disk-cache-compress', compress='lzma')
-        def slow_function(x):
-            time.sleep(0.1)
-            return 'a' * (1024 * 1024)
-
-        # Test caching the output of a function that returns a large string using LZMA compression
-        self.assertEqual(slow_function(5), 'a' * (1024 * 1024))
-        self.assertEqual(slow_function(5), 'a' * (1024 * 1024))  # Should use cache this time
-        self.assertEqual(slow_function(10), 'a' * (1024 * 1024))
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/cushy-storage
+# Contact Email: zeeland@foxmail.com
+
+import time
+import unittest
+from cushy_storage import CushyDict, disk_cache
+
+
+class TestDiskCache(unittest.TestCase):
+    def test_basic_usage(self):
+        @disk_cache('./test-disk-cache')
+        def slow_function(x):
+            time.sleep(0.1)
+            return x + 1
+
+        # Test calling the function with different arguments and caching the output
+        self.assertEqual(slow_function(5), 6)
+        self.assertEqual(slow_function(5), 6)  # Should use cache this time
+        self.assertEqual(slow_function(10), 11)
+
+    def test_serialization(self):
+        @disk_cache('./test-disk-cache-serialize', serialize='pickle')
+        def slow_function(x):
+            time.sleep(0.1)
+            return {'result': x}
+
+        # Test caching the output of a function that returns a dictionary using pickle serialization
+        self.assertEqual(slow_function(5), {'result': 5})
+        self.assertEqual(slow_function(5), {'result': 5})  # Should use cache this time
+        self.assertEqual(slow_function(10), {'result': 10})
+
+    def test_compression(self):
+        @disk_cache('./test-disk-cache-compress', compress='lzma')
+        def slow_function(x):
+            time.sleep(0.1)
+            return 'a' * (1024 * 1024)
+
+        # Test caching the output of a function that returns a large string using LZMA compression
+        self.assertEqual(slow_function(5), 'a' * (1024 * 1024))
+        self.assertEqual(slow_function(5), 'a' * (1024 * 1024))  # Should use cache this time
+        self.assertEqual(slow_function(10), 'a' * (1024 * 1024))
```

