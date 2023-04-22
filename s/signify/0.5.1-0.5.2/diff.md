# Comparing `tmp/signify-0.5.1.tar.gz` & `tmp/signify-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ralph\Development\signify\dist\.tmp-k6vew3jj\signify-0.5.1.tar", last modified: Wed Mar 22 19:22:17 2023, max compression
+gzip compressed data, was "C:\Users\ralph\Development\signify\dist\.tmp-cox3k7a6\signify-0.5.2.tar", last modified: Sat Apr 22 13:59:06 2023, max compression
```

## Comparing `signify-0.5.1.tar` & `signify-0.5.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.252456 signify-0.5.1/
--rw-rw-rw-   0        0        0     2018 2018-12-15 12:55:16.000000 signify-0.5.1/LICENSE
--rw-rw-rw-   0        0        0       94 2023-03-20 13:00:56.000000 signify-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2345 2023-03-22 19:22:17.251454 signify-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1279 2022-07-11 10:02:20.000000 signify-0.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.205457 signify-0.5.1/docs/
--rw-rw-rw-   0        0        0     7888 2018-12-15 12:55:16.000000 signify-0.5.1/docs/Makefile
--rw-rw-rw-   0        0        0     2708 2022-12-14 10:25:18.000000 signify-0.5.1/docs/authenticode.rst
--rw-rw-rw-   0        0        0     4382 2023-03-20 13:34:39.000000 signify-0.5.1/docs/authroot.rst
--rw-rw-rw-   0        0        0     1283 2021-03-01 14:52:02.000000 signify-0.5.1/docs/certificates.rst
--rw-rw-rw-   0        0        0     5571 2023-03-22 19:21:23.000000 signify-0.5.1/docs/changelog.rst
--rw-rw-rw-   0        0        0     9665 2021-03-01 10:05:05.000000 signify-0.5.1/docs/conf.py
--rw-rw-rw-   0        0        0     1486 2018-12-15 12:55:16.000000 signify-0.5.1/docs/fingerprinter.rst
--rw-rw-rw-   0        0        0      890 2022-12-14 09:16:53.000000 signify-0.5.1/docs/index.rst
--rwxrwxrwx   0        0        0     7257 2018-12-15 12:55:16.000000 signify-0.5.1/docs/make.bat
--rw-rw-rw-   0        0        0     1333 2021-03-01 14:52:42.000000 signify-0.5.1/docs/pkcs7.rst
--rw-rw-rw-   0        0        0       42 2023-03-22 19:22:17.252456 signify-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1925 2023-03-22 19:20:38.000000 signify-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.211480 signify-0.5.1/signify/
--rw-rw-rw-   0        0        0      353 2023-03-22 19:20:22.000000 signify-0.5.1/signify/__init__.py
--rw-rw-rw-   0        0        0     2322 2022-12-14 10:35:31.000000 signify-0.5.1/signify/_compat.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.227453 signify-0.5.1/signify/asn1/
--rw-rw-rw-   0        0        0     1160 2022-12-14 10:33:20.000000 signify-0.5.1/signify/asn1/__init__.py
--rw-rw-rw-   0        0        0     2403 2020-06-23 18:54:23.000000 signify-0.5.1/signify/asn1/ctl.py
--rw-rw-rw-   0        0        0     3282 2022-07-11 10:29:19.000000 signify-0.5.1/signify/asn1/helpers.py
--rw-rw-rw-   0        0        0     4111 2021-12-06 15:26:32.000000 signify-0.5.1/signify/asn1/oids.py
--rw-rw-rw-   0        0        0      170 2020-04-21 12:34:52.000000 signify-0.5.1/signify/asn1/pkcs7.py
--rw-rw-rw-   0        0        0     1159 2021-08-16 15:07:23.000000 signify-0.5.1/signify/asn1/preserving_der.py
--rw-rw-rw-   0        0        0     3867 2021-02-28 12:16:43.000000 signify-0.5.1/signify/asn1/spc.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.233452 signify-0.5.1/signify/authenticode/
--rw-rw-rw-   0        0        0      828 2023-03-20 13:02:16.000000 signify-0.5.1/signify/authenticode/__init__.py
--rw-rw-rw-   0        0        0    16847 2023-03-20 13:00:56.000000 signify-0.5.1/signify/authenticode/authroot.py
--rw-rw-rw-   0        0        0    13558 2022-12-14 10:36:12.000000 signify-0.5.1/signify/authenticode/signed_pe.py
--rw-rw-rw-   0        0        0    27604 2023-03-20 13:07:16.000000 signify-0.5.1/signify/authenticode/structures.py
--rw-rw-rw-   0        0        0     1344 2021-08-23 16:49:18.000000 signify-0.5.1/signify/exceptions.py
--rw-rw-rw-   0        0        0    11304 2021-03-01 14:56:01.000000 signify-0.5.1/signify/fingerprinter.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.237453 signify-0.5.1/signify/pkcs7/
--rw-rw-rw-   0        0        0      156 2022-12-14 10:47:23.000000 signify-0.5.1/signify/pkcs7/__init__.py
--rw-rw-rw-   0        0        0     4557 2021-08-16 13:48:19.000000 signify-0.5.1/signify/pkcs7/signeddata.py
--rw-rw-rw-   0        0        0    16807 2022-12-14 10:47:56.000000 signify-0.5.1/signify/pkcs7/signerinfo.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.242453 signify-0.5.1/signify/x509/
--rw-rw-rw-   0        0        0      267 2022-12-14 10:51:04.000000 signify-0.5.1/signify/x509/__init__.py
--rw-rw-rw-   0        0        0    11804 2022-12-14 10:59:36.000000 signify-0.5.1/signify/x509/certificates.py
--rw-rw-rw-   0        0        0    14704 2023-03-20 13:03:47.000000 signify-0.5.1/signify/x509/context.py
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.218454 signify-0.5.1/signify.egg-info/
--rw-rw-rw-   0        0        0     2345 2023-03-22 19:22:17.000000 signify-0.5.1/signify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1056 2023-03-22 19:22:17.000000 signify-0.5.1/signify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 19:22:17.000000 signify-0.5.1/signify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-03-22 19:22:17.000000 signify-0.5.1/signify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-22 19:22:17.000000 signify-0.5.1/signify.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 19:22:17.250486 signify-0.5.1/tests/
--rw-rw-rw-   0        0        0     4375 2021-03-01 14:45:09.000000 signify-0.5.1/tests/test_asn1.py
--rw-rw-rw-   0        0        0     9339 2021-08-16 15:08:21.000000 signify-0.5.1/tests/test_authenticode.py
--rw-rw-rw-   0        0        0      396 2021-03-01 14:46:55.000000 signify-0.5.1/tests/test_authroot.py
--rw-rw-rw-   0        0        0     2230 2022-07-11 09:40:17.000000 signify-0.5.1/tests/test_context.py
--rw-rw-rw-   0        0        0     4053 2020-01-19 16:03:11.000000 signify-0.5.1/tests/test_fingerprinter.py
--rw-rw-rw-   0        0        0     1718 2021-03-01 14:45:09.000000 signify-0.5.1/tests/test_signerinfo.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.854792 signify-0.5.2/
+-rw-rw-rw-   0        0        0     2018 2018-12-15 12:55:16.000000 signify-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       94 2023-03-20 13:00:56.000000 signify-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2345 2023-04-22 13:59:06.853792 signify-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1279 2022-07-11 10:02:20.000000 signify-0.5.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.794785 signify-0.5.2/docs/
+-rw-rw-rw-   0        0        0     7888 2018-12-15 12:55:16.000000 signify-0.5.2/docs/Makefile
+-rw-rw-rw-   0        0        0     2708 2022-12-14 10:25:18.000000 signify-0.5.2/docs/authenticode.rst
+-rw-rw-rw-   0        0        0     4382 2023-03-20 13:34:39.000000 signify-0.5.2/docs/authroot.rst
+-rw-rw-rw-   0        0        0     1283 2021-03-01 14:52:02.000000 signify-0.5.2/docs/certificates.rst
+-rw-rw-rw-   0        0        0     5720 2023-04-22 13:55:45.000000 signify-0.5.2/docs/changelog.rst
+-rw-rw-rw-   0        0        0     9665 2021-03-01 10:05:05.000000 signify-0.5.2/docs/conf.py
+-rw-rw-rw-   0        0        0     1486 2018-12-15 12:55:16.000000 signify-0.5.2/docs/fingerprinter.rst
+-rw-rw-rw-   0        0        0      890 2022-12-14 09:16:53.000000 signify-0.5.2/docs/index.rst
+-rwxrwxrwx   0        0        0     7257 2018-12-15 12:55:16.000000 signify-0.5.2/docs/make.bat
+-rw-rw-rw-   0        0        0     1333 2021-03-01 14:52:42.000000 signify-0.5.2/docs/pkcs7.rst
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:59:06.854792 signify-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1932 2023-04-22 13:38:42.000000 signify-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.801963 signify-0.5.2/signify/
+-rw-rw-rw-   0        0        0      353 2023-04-22 13:56:06.000000 signify-0.5.2/signify/__init__.py
+-rw-rw-rw-   0        0        0     2322 2022-12-14 10:35:31.000000 signify-0.5.2/signify/_compat.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.823966 signify-0.5.2/signify/asn1/
+-rw-rw-rw-   0        0        0     1160 2023-04-22 13:28:12.000000 signify-0.5.2/signify/asn1/__init__.py
+-rw-rw-rw-   0        0        0     2403 2020-06-23 18:54:23.000000 signify-0.5.2/signify/asn1/ctl.py
+-rw-rw-rw-   0        0        0     3282 2022-07-11 10:29:19.000000 signify-0.5.2/signify/asn1/helpers.py
+-rw-rw-rw-   0        0        0     4111 2021-12-06 15:26:32.000000 signify-0.5.2/signify/asn1/oids.py
+-rw-rw-rw-   0        0        0      170 2020-04-21 12:34:52.000000 signify-0.5.2/signify/asn1/pkcs7.py
+-rw-rw-rw-   0        0        0     1159 2021-08-16 15:07:23.000000 signify-0.5.2/signify/asn1/preserving_der.py
+-rw-rw-rw-   0        0        0     3867 2021-02-28 12:16:43.000000 signify-0.5.2/signify/asn1/spc.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.830963 signify-0.5.2/signify/authenticode/
+-rw-rw-rw-   0        0        0      828 2023-03-20 13:02:16.000000 signify-0.5.2/signify/authenticode/__init__.py
+-rw-rw-rw-   0        0        0    16847 2023-04-22 13:19:16.000000 signify-0.5.2/signify/authenticode/authroot.py
+-rw-rw-rw-   0        0        0    13558 2022-12-14 10:36:12.000000 signify-0.5.2/signify/authenticode/signed_pe.py
+-rw-rw-rw-   0        0        0    27604 2023-03-20 13:07:16.000000 signify-0.5.2/signify/authenticode/structures.py
+-rw-rw-rw-   0        0        0     1344 2021-08-23 16:49:18.000000 signify-0.5.2/signify/exceptions.py
+-rw-rw-rw-   0        0        0    11304 2021-03-01 14:56:01.000000 signify-0.5.2/signify/fingerprinter.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.837004 signify-0.5.2/signify/pkcs7/
+-rw-rw-rw-   0        0        0      156 2022-12-14 10:47:23.000000 signify-0.5.2/signify/pkcs7/__init__.py
+-rw-rw-rw-   0        0        0     4557 2021-08-16 13:48:19.000000 signify-0.5.2/signify/pkcs7/signeddata.py
+-rw-rw-rw-   0        0        0    16807 2022-12-14 10:47:56.000000 signify-0.5.2/signify/pkcs7/signerinfo.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.843398 signify-0.5.2/signify/x509/
+-rw-rw-rw-   0        0        0      267 2022-12-14 10:51:04.000000 signify-0.5.2/signify/x509/__init__.py
+-rw-rw-rw-   0        0        0    11804 2022-12-14 10:59:36.000000 signify-0.5.2/signify/x509/certificates.py
+-rw-rw-rw-   0        0        0    14704 2023-03-20 13:03:47.000000 signify-0.5.2/signify/x509/context.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.809988 signify-0.5.2/signify.egg-info/
+-rw-rw-rw-   0        0        0     2345 2023-04-22 13:59:06.000000 signify-0.5.2/signify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2023-04-22 13:59:06.000000 signify-0.5.2/signify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:59:06.000000 signify-0.5.2/signify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-04-22 13:59:06.000000 signify-0.5.2/signify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 13:59:06.000000 signify-0.5.2/signify.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 13:59:06.852792 signify-0.5.2/tests/
+-rw-rw-rw-   0        0        0     4375 2021-03-01 14:45:09.000000 signify-0.5.2/tests/test_asn1.py
+-rw-rw-rw-   0        0        0     9339 2021-08-16 15:08:21.000000 signify-0.5.2/tests/test_authenticode.py
+-rw-rw-rw-   0        0        0      396 2021-03-01 14:46:55.000000 signify-0.5.2/tests/test_authroot.py
+-rw-rw-rw-   0        0        0     2230 2022-07-11 09:40:17.000000 signify-0.5.2/tests/test_context.py
+-rw-rw-rw-   0        0        0     4053 2020-01-19 16:03:11.000000 signify-0.5.2/tests/test_fingerprinter.py
+-rw-rw-rw-   0        0        0     1718 2021-03-01 14:45:09.000000 signify-0.5.2/tests/test_signerinfo.py
```

### Comparing `signify-0.5.1/LICENSE` & `signify-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/PKG-INFO` & `signify-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: signify
-Version: 0.5.1
+Version: 0.5.2
 Summary: Module to generate and verify PE signatures
 Home-page: https://github.com/ralphje/signify
-Download-URL: https://github.com/ralphje/signify/tarball/v0.5.1
+Download-URL: https://github.com/ralphje/signify/tarball/v0.5.2
 Author: Ralph Broenink
 Author-email: ralph@ralphbroenink.net
 License: MIT
 Keywords: authenticode,authentihash,fingerprinter,pe
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `signify-0.5.1/README.rst` & `signify-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/Makefile` & `signify-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/authenticode.rst` & `signify-0.5.2/docs/authenticode.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/authroot.rst` & `signify-0.5.2/docs/authroot.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/certificates.rst` & `signify-0.5.2/docs/certificates.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/changelog.rst` & `signify-0.5.2/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Release notes
 =============
 This page contains the most significant changes in Signify between each release.
 
+v0.5.2 (2023-04-22)
+-------------------
+* Pin pyasn1 dependency version to <0.5.0 for now, due to some apparent backwards-incompatible changes.
+
 v0.5.1 (2023-03-22)
 -------------------
 * Remove PyInstaller hook and optional requirements from setup.py
 
 v0.5.0 (2023-03-20)
 -------------------
 * Drop support for Python 3.6
```

### Comparing `signify-0.5.1/docs/conf.py` & `signify-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/fingerprinter.rst` & `signify-0.5.2/docs/fingerprinter.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/index.rst` & `signify-0.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/make.bat` & `signify-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/docs/pkcs7.rst` & `signify-0.5.2/docs/pkcs7.rst`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/setup.py` & `signify-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     url='https://github.com/ralphje/signify',
     download_url='https://github.com/ralphje/signify/tarball/v' + about['__version__'],
     license='MIT',
     author='Ralph Broenink',
     author_email='ralph@ralphbroenink.net',
     description='Module to generate and verify PE signatures',
     long_description=long_description,
-    install_requires=['pyasn1>=0.4.0',
+    install_requires=['pyasn1>=0.4.0,<0.5.0',
                       'certvalidator>=0.11',
                       'asn1crypto>=1.3,<2',
                       'oscrypto>=1.1,<2',
                       'pyasn1-modules>=0.2.8',
                       'mscerts'],
     keywords=['authenticode', 'authentihash', 'fingerprinter', 'pe'],
     classifiers=[
```

### Comparing `signify-0.5.1/signify/_compat.py` & `signify-0.5.2/signify/_compat.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/asn1/__init__.py` & `signify-0.5.2/signify/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/asn1/ctl.py` & `signify-0.5.2/signify/asn1/ctl.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/asn1/helpers.py` & `signify-0.5.2/signify/asn1/helpers.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/asn1/oids.py` & `signify-0.5.2/signify/asn1/oids.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/asn1/preserving_der.py` & `signify-0.5.2/signify/asn1/preserving_der.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/asn1/spc.py` & `signify-0.5.2/signify/asn1/spc.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/authenticode/__init__.py` & `signify-0.5.2/signify/authenticode/__init__.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/authenticode/authroot.py` & `signify-0.5.2/signify/authenticode/authroot.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/authenticode/signed_pe.py` & `signify-0.5.2/signify/authenticode/signed_pe.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/authenticode/structures.py` & `signify-0.5.2/signify/authenticode/structures.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/exceptions.py` & `signify-0.5.2/signify/exceptions.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/fingerprinter.py` & `signify-0.5.2/signify/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/pkcs7/signeddata.py` & `signify-0.5.2/signify/pkcs7/signeddata.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/pkcs7/signerinfo.py` & `signify-0.5.2/signify/pkcs7/signerinfo.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/x509/certificates.py` & `signify-0.5.2/signify/x509/certificates.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify/x509/context.py` & `signify-0.5.2/signify/x509/context.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/signify.egg-info/PKG-INFO` & `signify-0.5.2/signify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: signify
-Version: 0.5.1
+Version: 0.5.2
 Summary: Module to generate and verify PE signatures
 Home-page: https://github.com/ralphje/signify
-Download-URL: https://github.com/ralphje/signify/tarball/v0.5.1
+Download-URL: https://github.com/ralphje/signify/tarball/v0.5.2
 Author: Ralph Broenink
 Author-email: ralph@ralphbroenink.net
 License: MIT
 Keywords: authenticode,authentihash,fingerprinter,pe
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `signify-0.5.1/signify.egg-info/SOURCES.txt` & `signify-0.5.2/signify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/tests/test_asn1.py` & `signify-0.5.2/tests/test_asn1.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/tests/test_authenticode.py` & `signify-0.5.2/tests/test_authenticode.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/tests/test_context.py` & `signify-0.5.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/tests/test_fingerprinter.py` & `signify-0.5.2/tests/test_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `signify-0.5.1/tests/test_signerinfo.py` & `signify-0.5.2/tests/test_signerinfo.py`

 * *Files identical despite different names*

