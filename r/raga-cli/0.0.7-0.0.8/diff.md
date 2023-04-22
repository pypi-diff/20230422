# Comparing `tmp/raga-cli-0.0.7.tar.gz` & `tmp/raga-cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.0.7.tar", last modified: Fri Apr 21 12:55:59 2023, max compression
+gzip compressed data, was "raga-cli-0.0.8.tar", last modified: Sat Apr 22 07:04:21 2023, max compression
```

## Comparing `raga-cli-0.0.7.tar` & `raga-cli-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.525062 raga-cli-0.0.7/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.0.7/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.0.7/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-21 12:55:59.524686 raga-cli-0.0.7/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.7/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2504 2023-04-21 12:54:24.000000 raga-cli-0.0.7/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.516887 raga-cli-0.0.7/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1029 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.517781 raga-cli-0.0.7/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.519320 raga-cli-0.0.7/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.0.7/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.0.7/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9323 2023-04-20 11:09:18.000000 raga-cli-0.0.7/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.520892 raga-cli-0.0.7/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.0.7/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.0.7/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.0.7/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.522429 raga-cli-0.0.7/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5050 2023-04-20 11:10:27.000000 raga-cli-0.0.7/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.522729 raga-cli-0.0.7/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.524167 raga-cli-0.0.7/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.0.7/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-21 12:55:59.525146 raga-cli-0.0.7/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.0.7/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.728372 raga-cli-0.0.8/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.0.8/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.0.8/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-22 07:04:21.728128 raga-cli-0.0.8/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.8/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2508 2023-04-22 07:02:35.000000 raga-cli-0.0.8/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.723496 raga-cli-0.0.8/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-22 07:04:21.000000 raga-cli-0.0.8/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-22 07:04:21.000000 raga-cli-0.0.8/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-22 07:04:21.000000 raga-cli-0.0.8/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-22 07:04:21.000000 raga-cli-0.0.8/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1033 2023-04-22 07:04:21.000000 raga-cli-0.0.8/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-22 07:04:21.000000 raga-cli-0.0.8/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.723934 raga-cli-0.0.8/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.724918 raga-cli-0.0.8/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.0.8/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.0.8/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9621 2023-04-22 06:59:03.000000 raga-cli-0.0.8/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.725904 raga-cli-0.0.8/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.0.8/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.0.8/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.0.8/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.726573 raga-cli-0.0.8/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5050 2023-04-22 07:01:22.000000 raga-cli-0.0.8/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.726732 raga-cli-0.0.8/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-22 07:04:21.727801 raga-cli-0.0.8/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.0.8/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.0.8/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-22 07:04:21.728425 raga-cli-0.0.8/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.0.8/setup.py
```

### Comparing `raga-cli-0.0.7/.gitignore` & `raga-cli-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/LICENSE` & `raga-cli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/PKG-INFO` & `raga-cli-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.7/pyproject.toml` & `raga-cli-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.0.7"
+version = "0.0.8"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
@@ -21,15 +21,15 @@
 ]
 license = { text = "Apache License 2.0" }
 authors = [{ name = "Manab Roy", email = "manabr@observancegroup.com" }]
 maintainers = [{ name = "Manab Roy", email = "support@observancegroup.com" }]
 dependencies = [
     "dvc==2.38.1",
     "dvc_s3==2.21.0",
-    "boto3==1.16.28"
+    "botocore==1.29.118"
 ]
 [project.optional-dependencies]
 azure = ["dvc-azure==2.20.5"]
 gdrive = ["dvc-gdrive==2.19.1"]
 gs = ["dvc-gs==2.20.0"]
 hdfs = ["dvc-hdfs==2.19.0"]
 oss = ["dvc-oss==2.19.0"]
```

### Comparing `raga-cli-0.0.7/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.0.8/raga_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.7/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.0.8/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/raga_cli.egg-info/requires.txt` & `raga-cli-0.0.8/raga_cli.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dvc==2.38.1
 dvc_s3==2.21.0
-boto3==1.16.28
+botocore==1.29.118
 
 [all]
 dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]
 
 [azure]
 dvc-azure==2.20.5
```

### Comparing `raga-cli-0.0.7/rc/cli/__init__.py` & `raga-cli-0.0.8/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/cli/parser.py` & `raga-cli-0.0.8/rc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/cli/utils.py` & `raga-cli-0.0.8/rc/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,26 +209,36 @@
                 d['children'] = [path_to_dict(os.path.join(path,x)) for x in os.listdir\
         (path)]
             else:
                 d['type'] = "file"
             return d 
 
 def upload_model_file_list_json(version):
-    import boto3    
+    logger.debug("MODEL FILE UPLOADING")
+    import botocore.session   
     model_file_list = json.loads(json.dumps(path_to_dict('.')))
     CLOUD_STORAGE_BUCKET = get_config_value_by_key('bucket_name')
     CLOUD_STORAGE_DIR = get_config_value_by_key('cloud_storage_dir')
     AWS_SECRET = get_config_value_by_key('remote_storage_secret_key')
     AWS_ACCESS = get_config_value_by_key('remote_storage_access_key')
     repo = get_repo()
     dest = f"{CLOUD_STORAGE_DIR}/{repo}/model_files/{version}.json"
-    s3 = boto3.client('s3', aws_access_key_id=AWS_ACCESS, aws_secret_access_key=AWS_SECRET)
+    # Create a botocore session with the AWS access key and secret key
+    session = botocore.session.Session()
+    session.set_credentials(AWS_ACCESS, AWS_SECRET)
+
+    # Create an S3 client using the botocore session
+    s3 = session.create_client('s3')
+
     with open(f'{version}.json', 'w', encoding='utf-8') as cred:    
-        json.dump(model_file_list, cred, ensure_ascii=False, indent=4)            
-    s3.upload_file(f'{version}.json', CLOUD_STORAGE_BUCKET, dest)
+        json.dump(model_file_list, cred, ensure_ascii=False, indent=4)  
+
+    # Upload the file to S3
+    with open(f'{version}.json', 'rb') as file:
+        s3.put_object(Bucket=CLOUD_STORAGE_BUCKET, Key=dest, Body=file)          
     pathlib.Path(f'{version}.json').unlink(missing_ok=True)
     
 def retry(ExceptionToCheck, tries=4, delay=3, backoff=2):
     """
     Retry calling the decorated function using an exponential backoff.
 
     Args:
```

### Comparing `raga-cli-0.0.7/rc/commands/get.py` & `raga-cli-0.0.8/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/commands/list.py` & `raga-cli-0.0.8/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/commands/put.py` & `raga-cli-0.0.8/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/commands/repo.py` & `raga-cli-0.0.8/rc/commands/repo.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/exceptions.py` & `raga-cli-0.0.8/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/prompt.py` & `raga-cli-0.0.8/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/repo/get.py` & `raga-cli-0.0.8/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/repo/put.py` & `raga-cli-0.0.8/rc/repo/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/utils/__init__.py` & `raga-cli-0.0.8/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/utils/request.py` & `raga-cli-0.0.8/rc/utils/request.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.7/rc/utils/sshKeyGen.py` & `raga-cli-0.0.8/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

