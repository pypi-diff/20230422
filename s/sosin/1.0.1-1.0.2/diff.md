# Comparing `tmp/sosin-1.0.1.tar.gz` & `tmp/sosin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.0.1.tar", last modified: Wed Apr 19 14:56:48 2023, max compression
+gzip compressed data, was "sosin-1.0.2.tar", last modified: Sat Apr 22 13:06:34 2023, max compression
```

## Comparing `sosin-1.0.1.tar` & `sosin-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.476827 sosin-1.0.1/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-04-19 14:56:48.476827 sosin-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 14:56:48.476827 sosin-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-19 14:56:38.000000 sosin-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.443100 sosin-1.0.1/sosin/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.1/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.465416 sosin-1.0.1/sosin/databases/
--rw-rw-rw-   0        0        0     6203 2023-04-19 13:20:07.000000 sosin-1.0.1/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.466416 sosin-1.0.1/sosin/rpa/
--rw-rw-rw-   0        0        0     9951 2023-04-18 14:45:09.000000 sosin-1.0.1/sosin/rpa/email_mgr.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.471417 sosin-1.0.1/sosin/utils/
--rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/utils/secret.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.474463 sosin-1.0.1/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.1/sosin/web/content.py
--rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4796 2023-04-17 11:46:46.000000 sosin-1.0.1/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:56:48.464414 sosin-1.0.1/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 14:56:48.000000 sosin-1.0.1/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.316430 sosin-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-04-22 13:06:34.315329 sosin-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:06:34.316430 sosin-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-04-22 13:05:48.000000 sosin-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.278792 sosin-1.0.2/sosin/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.2/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.304280 sosin-1.0.2/sosin/databases/
+-rw-rw-rw-   0        0        0     6203 2023-04-19 13:20:07.000000 sosin-1.0.2/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.305795 sosin-1.0.2/sosin/rpa/
+-rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.0.2/sosin/rpa/email_mgr.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.310814 sosin-1.0.2/sosin/utils/
+-rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/secret.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.314321 sosin-1.0.2/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.2/sosin/web/content.py
+-rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4796 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.302774 sosin-1.0.2/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-04-22 13:06:33.000000 sosin-1.0.2/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.0.1/LICENSE` & `sosin-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/PKG-INFO` & `sosin-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.0.1/README.md` & `sosin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/setup.py` & `sosin-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.0.1",
+    version                             = "1.0.2",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'beautifulsoup4', 'PyMySQL',],
```

### Comparing `sosin-1.0.1/sosin/databases/rdb.py` & `sosin-1.0.2/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/sosin/rpa/email_mgr.py` & `sosin-1.0.2/sosin/rpa/email_mgr.py`

 * *Files 10% similar despite different names*

```diff
@@ -250,14 +250,42 @@
             return True
 
         except Exception:
             traceback.print_exc()
         
         return False
 
+def _get_emails(email_id, email_pw, **kwargs):
+    """
+    kwargs
+    mail_server = ['gmail', 'naver']
+    header_subjects:list=[], header_since:str=None, header_from:str=None, 
+    label:str=None, save_path:str=None, 
+
+    remove_email=True,
+    encode_type='utf-8',
+    """
+    emgr = EmailManager(email_id, email_pw, mail_server=kwargs.pop('mail_server', 'naver'), mode='get')
+    emails = emgr.get_email(**kwargs)
+    del emgr
+    return emails
+
+def _send_email(email_id, email_pw, **kwargs):
+    """
+    kwargs
+    mail_server = ['gmail', 'naver']
+    from_user:str, to_users:list, 
+    subject:str, contents:list[Union[tuple, str]],
+    attachments:list=[], cc_targets=[]
+    """
+    emgr = EmailManager(email_id, email_pw, mail_server=kwargs.pop('mail_server', 'naver'))
+    result = emgr.send_email(**kwargs)
+    del emgr
+    return result
+
 if __name__ == '__main__':
     config = {
         'EMAIL_ID': 'your-email-id',
         'EMAIL_PW': 'your-email-pw',
     }
     emgr = EmailManager(config.get('EMAIL_ID'), config.get('EMAIL_PW'), mail_server='gmail')
     emgr.send_email(config['EMAIL_ID'], ['target-user-email'], 'this is test email !',
```

### Comparing `sosin-1.0.1/sosin/utils/currency.py` & `sosin-1.0.2/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/sosin/utils/progress.py` & `sosin-1.0.2/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/sosin/web/content.py` & `sosin-1.0.2/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/sosin/web/translate.py` & `sosin-1.0.2/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/sosin/web/virtual.py` & `sosin-1.0.2/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.1/sosin.egg-info/PKG-INFO` & `sosin-1.0.2/sosin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

