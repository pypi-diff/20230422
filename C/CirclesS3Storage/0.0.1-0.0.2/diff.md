# Comparing `tmp/CirclesS3Storage-0.0.1.tar.gz` & `tmp/CirclesS3Storage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CirclesS3Storage-0.0.1.tar", last modified: Sun Apr 16 14:44:59 2023, max compression
+gzip compressed data, was "CirclesS3Storage-0.0.2.tar", last modified: Sat Apr 22 10:02:16 2023, max compression
```

## Comparing `CirclesS3Storage-0.0.1.tar` & `CirclesS3Storage-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:44:58.959596 CirclesS3Storage-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-16 14:44:58.514230 CirclesS3Storage-0.0.1/CirclesS3Storage.egg-info/
--rw-rw-rw-   0        0        0      477 2023-04-16 14:44:56.000000 CirclesS3Storage-0.0.1/CirclesS3Storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-16 14:44:57.000000 CirclesS3Storage-0.0.1/CirclesS3Storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:44:56.000000 CirclesS3Storage-0.0.1/CirclesS3Storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-16 14:44:56.000000 CirclesS3Storage-0.0.1/CirclesS3Storage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      477 2023-04-16 14:44:58.950009 CirclesS3Storage-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/README.md
--rw-rw-rw-   0        0        0       88 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 14:44:58.960583 CirclesS3Storage-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-04-16 14:44:53.000000 CirclesS3Storage-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:44:58.817174 CirclesS3Storage-0.0.1/src/
--rw-rw-rw-   0        0        0     1471 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/src/AWSStorage.py
--rw-rw-rw-   0        0        0     2609 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/src/StorageDB.py
--rw-rw-rw-   0        0        0      578 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/src/StorageInterface.py
--rw-rw-rw-   0        0        0        0 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:44:58.898532 CirclesS3Storage-0.0.1/tests/
--rw-rw-rw-   0        0        0     1535 2023-04-11 16:06:36.000000 CirclesS3Storage-0.0.1/tests/test_S3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-22 10:02:16.000000 CirclesS3Storage-0.0.2/CirclesS3Storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 10:02:16.222052 CirclesS3Storage-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-22 10:01:53.000000 CirclesS3Storage-0.0.2/tests/test_circles_storage.py
```

### Comparing `CirclesS3Storage-0.0.1/setup.py` & `CirclesS3Storage-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import setuptools
-
-setuptools.setup(
-    name='CirclesS3Storage',
-    version='0.0.1',
-    author="Circles",
-    author_email="info@circle.zone",
-    description="PyPI Package for Circles S3 functions",
-    long_description="This is a package for sharing common S3 function used in different repositories",
-    long_description_content_type="text/markdown",
-    url="https://github.com/javatechy/dokr",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-         "License :: Other/Proprietary License",
-         "Operating System :: OS Independent",
-    ],
-)
+import setuptools
+
+setuptools.setup(
+    name='CirclesS3Storage',
+    version='0.0.2',
+    author="Circles",
+    author_email="info@circle.zone",
+    description="PyPI Package for Circles S3 functions",
+    long_description="This is a package for sharing common S3 function used in different repositories",
+    long_description_content_type="text/markdown",
+    url="https://github.com/javatechy/dokr",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+         "License :: Other/Proprietary License",
+         "Operating System :: OS Independent",
+    ],
+)
```

### Comparing `CirclesS3Storage-0.0.1/src/AWSStorage.py` & `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-
-import boto3
-
-from src.StorageInterface import StorageInterface
-from src.StorageDB import StorageDB
-
-
-class AwsS3Storage(StorageInterface):
-
-    def __init__(self, bucket_name, region):
-        self.region = region
-        self.bucket_name = bucket_name
-        self.client = boto3.client('s3')
-        self.database = StorageDB()
-
-    # uploads file to S3
-    def upload_file(self, local_path, filename, remote_path, created_user_id):
-        read_binary = 'rb'
-        with open(local_path, read_binary) as file_obj:
-            file_contents = file_obj.read()
-
-        # Upload the file to S3 with the CRC32 checksum
-        response = self.client.put_object(
-            Bucket=self.bucket_name,
-            Key=remote_path+filename,
-            Body=file_contents,
-            ChecksumAlgorithm='crc32'
-        )
-        if 'ETag' in response:
-            id = self.database.uploadToDataBase(
-                remote_path, filename, self.region, created_user_id, 1, 1, 1)  # One's needs to be replaced by parameter
-            return id
-        return None
-
-    # download a file from s3 to local_path
-    def download_file(self, remote_path, local_path):
-        self.client.download_file(self.bucket_name, remote_path, local_path)
-
-    # logical delete
-    def delete_file(self, remote_path, filename, updated_user_id):
-        self.database.logicalDelete(
-            remote_path, filename, self.region, updated_user_id)
+
+import os
+import boto3
+
+from circles_local_aws_s3_storage_python.StorageInterface import StorageInterface
+from circles_local_aws_s3_storage_python.StorageDB import StorageDB
+
+
+class AwsS3Storage(StorageInterface):
+
+    def __init__(self, bucket_name, region):
+        self.region = region
+        self.bucket_name = bucket_name
+        self.database = StorageDB()
+        self.client = boto3.client('s3',
+                                   aws_access_key_id=os.getenv(
+                                       "AWS_ACCESS_KEY_ID"),
+                                   aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"))
+
+    # uploads file to S3
+
+    def upload_file(self, local_path, filename, remote_path, created_user_id):
+        read_binary = 'rb'
+        with open(local_path, read_binary) as file_obj:
+            file_contents = file_obj.read()
+
+        # Upload the file to S3 with the CRC32 checksum
+        response = self.client.put_object(
+            Bucket=self.bucket_name,
+            Key=remote_path+filename,
+            Body=file_contents,
+            ChecksumAlgorithm='crc32'
+        )
+        if 'ETag' in response:
+            id = self.database.uploadToDataBase(
+                remote_path, filename, self.region, created_user_id, 1, 1, 1)  # One's needs to be replaced by parameter
+            return id
+        return None
+
+    # download a file from s3 to local_path
+    def download_file(self, remote_path, local_path):
+        self.client.download_file(self.bucket_name, remote_path, local_path)
+
+    # logical delete
+    def delete_file(self, remote_path, filename, updated_user_id):
+        self.database.logicalDelete(
+            remote_path, filename, self.region, updated_user_id)
```

### Comparing `CirclesS3Storage-0.0.1/src/StorageDB.py` & `CirclesS3Storage-0.0.2/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import os
-import mysql.connector
-from dotenv.main import load_dotenv
-load_dotenv()
-
-
-class StorageDB:
-    def __init__(self) -> None:
-        self.mydb = mysql.connector.connect(
-            host=os.getenv("RDS_HOSTNAME"),
-            user=os.getenv("RDS_USERNAME"),
-            passwd=os.getenv("RDS_PASSWORD"),
-            database=os.getenv("RDS_DB_NAME")
-        )
-        self.cursor = mycursor = self.mydb.cursor()
-
-    def uploadToDataBase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
-        add_storage = ("INSERT INTO storage "
-                       "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, extension_id) "
-                       "VALUES (%s, %s, %s, %s, %s, %s, %s, %s)")
-        storage_data = (file_path, filename, region, created_user_id,
-                        created_user_id, storage_type_id, file_type_id, extension_id)
-        self.cursor.execute(add_storage, storage_data)
-        self.mydb.commit()
-        select_stmt = "SELECT LAST_INSERT_ID()"
-        self.cursor.execute(select_stmt)
-        last_insert_id = self.cursor.fetchone()[0]
-        return int(last_insert_id)
-
-    def closeConnection(self):
-        if (self.mydb != None):
-            self.mydb.close
-
-    def logicalDelete(self, remote_path, filename, region, updated_user_id) -> int:
-        select_stmt = "SELECT id FROM storage WHERE path = %s AND filename = %s AND region = %s"
-        select_data = (remote_path, filename, region)
-        self.cursor.execute(select_stmt, select_data)
-        id = self.cursor.fetchone()[0]
-        self.cursor.nextset()
-        update_stmt = "UPDATE storage SET end_timestamp = NOW(), updated_timestamp = NOW(), updated_user_id = %s WHERE path = %s AND filename = %s AND region = %s"
-        update_data = (updated_user_id, remote_path, filename, region)
-        self.cursor.execute(update_stmt, update_data)
-        self.mydb.commit()
-        return int(id)
-
-    def getEndTimeStampFromDB(self, remote_path, filename, region):
-        update_stmt = "SELECT end_timestamp FROM storage WHERE path = %s AND filename = %s AND region = %s"
-        update_data = (remote_path, filename, region)
-        self.cursor.execute(update_stmt, update_data)
-        return self.cursor.fetchone()
-
-    def getLastId(self) -> int:
-        select_stmt = "SELECT id FROM storage ORDER BY id DESC LIMIT 1"
-        self.cursor.execute(select_stmt)
-        last_insert_id = self.cursor.fetchone()[0]
-        return int(last_insert_id)
+import os
+import mysql.connector
+from dotenv.main import load_dotenv
+load_dotenv()
+
+
+class StorageDB:
+    def __init__(self) -> None:
+        self.mydb = mysql.connector.connect(
+            host=os.getenv("RDS_HOSTNAME"),
+            user=os.getenv("RDS_USERNAME"),
+            passwd=os.getenv("RDS_PASSWORD"),
+            database=os.getenv("RDS_DB_NAME")
+        )
+        self.cursor = self.mydb.cursor()
+
+    def uploadToDataBase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
+        add_storage = ("INSERT INTO storage.storage_table "
+                       "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, extension_id) "
+                       "VALUES (%s, %s, %s, %s, %s, %s, %s, %s)")
+        storage_data = (file_path, filename, region, created_user_id,
+                        created_user_id, storage_type_id, file_type_id, extension_id)
+        self.cursor.execute(add_storage, storage_data)
+        self.mydb.commit()
+        select_stmt = "SELECT LAST_INSERT_ID()"
+        self.cursor.execute(select_stmt)
+        last_insert_id = self.cursor.fetchone()[0]
+        return int(last_insert_id)
+
+    def closeConnection(self):
+        if (self.mydb != None):
+            self.mydb.close
+
+    def logicalDelete(self, remote_path, filename, region, updated_user_id) -> int:
+        select_stmt = "SELECT id FROM storage.storage_table WHERE path = %s AND filename = %s AND region = %s"
+        select_data = (remote_path, filename, region)
+        self.cursor.execute(select_stmt, select_data)
+        id = self.cursor.fetchone()[0]
+        self.cursor.nextset()
+        update_stmt = "UPDATE storage.storage_table SET end_timestamp = NOW(), updated_timestamp = NOW(), updated_user_id = %s WHERE path = %s AND filename = %s AND region = %s"
+        update_data = (updated_user_id, remote_path, filename, region)
+        self.cursor.execute(update_stmt, update_data)
+        self.mydb.commit()
+        return int(id)
+
+    def getEndTimeStampFromDB(self, remote_path, filename, region):
+        update_stmt = "SELECT end_timestamp FROM storage.storage_table WHERE path = %s AND filename = %s AND region = %s"
+        update_data = (remote_path, filename, region)
+        self.cursor.execute(update_stmt, update_data)
+        return self.cursor.fetchone()
+
+    def getLastId(self) -> int:
+        select_stmt = "SELECT id FROM storage.storage_table ORDER BY id DESC LIMIT 1"
+        self.cursor.execute(select_stmt)
+        last_insert_id = self.cursor.fetchone()[0]
+        return int(last_insert_id)
```

