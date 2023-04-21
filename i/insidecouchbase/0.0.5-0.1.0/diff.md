# Comparing `tmp/insidecouchbase-0.0.5.tar.gz` & `tmp/insidecouchbase-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidecouchbase-0.0.5.tar", last modified: Sat Apr 15 11:33:13 2023, max compression
+gzip compressed data, was "insidecouchbase-0.1.0.tar", last modified: Fri Apr 21 23:15:57 2023, max compression
```

## Comparing `insidecouchbase-0.0.5.tar` & `insidecouchbase-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-15 09:54:30.000000 insidecouchbase-0.0.5/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     5198 2023-04-15 11:23:55.000000 insidecouchbase-0.0.5/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-15 10:44:14.000000 insidecouchbase-0.0.5/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-04-15 11:32:47.000000 insidecouchbase-0.0.5/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/src/couchbase/
--rw-rw-r--   0 demir     (1000) demir     (1000)       40 2023-04-15 11:08:25.000000 insidecouchbase-0.0.5/src/couchbase/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    13465 2023-04-15 11:32:22.000000 insidecouchbase-0.0.5/src/couchbase/couchbase.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-15 11:33:13.030942 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     5778 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-15 11:33:13.000000 insidecouchbase-0.0.5/src/insidecouchbase.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-21 20:42:51.000000 insidecouchbase-0.1.0/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     9451 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     8871 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-21 20:42:51.000000 insidecouchbase-0.1.0/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/src/couchbase/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       36 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/src/couchbase/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    19737 2023-04-21 23:15:49.000000 insidecouchbase-0.1.0/src/couchbase/couchbase.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-04-21 23:15:57.289905 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     9451 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      318 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-04-21 23:15:57.000000 insidecouchbase-0.1.0/src/insidecouchbase.egg-info/top_level.txt
```

### Comparing `insidecouchbase-0.0.5/LICENSE` & `insidecouchbase-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insidecouchbase-0.0.5/setup.cfg` & `insidecouchbase-0.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = insidecocuhbase
-version = 0.0.1
+version = 0.1.0
 author = Huseyin Demir
 author_email = huseyin.d3r@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/adiosamig/insidecocuhbase
 project_urls =
```

### Comparing `insidecouchbase-0.0.5/setup.py` & `insidecouchbase-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidecouchbase",
-    version = "0.0.5",
+    version = "0.1.0",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidecocuhbase",
     install_requires=[
```

### Comparing `insidecouchbase-0.0.5/src/couchbase/couchbase.py` & `insidecouchbase-0.1.0/src/couchbase/couchbase.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 import requests
 import telnetlib
 import sys
 from tabulate import tabulate
 import pandas as pd
 
-class couchbasePlatform:
+class couchbaseNode:
     def __init__(self,hostName,loginInformation,loginSecret):
         self.hostname=hostName
         self.logininformation=loginInformation
         self.loginsecret=loginSecret
         self.clusterDefinition=''
+        self.clusterScore=100
+        self.allBucketHaveAtLeastOneReplica=True
+        self.allNodesAreHealthy=True
+        self.mdsApplied=True
+        self.allBucketPrimaryVbucketGood=True
+        self.allBucketsResident=True
+        self.allNodesSameVersion=True
+        self.getClusterName()
+        self.getClusterVersion()
+        self.getNodesOnCluster()
+        self.getRebalance()
+        self.getSettings()
+        self.getUsersOnCluster()
+        self.getXdcrConnections()
+        self.prepareBucketData()
+        #self.prepareIndexData()
+        self.generateResults()
+        self.generateReport()
+        self.takePicture()
+        
+    def uniqueVersions(list1):
+ 
+    # initialize a null list
+        unique_list = []
+ 
+    # traverse for all elements
+        for x in list1:
+            # check if exists in unique_list or not
+            if x not in unique_list:
+                unique_list.append(x)
+        return unique_list
 
     def getClusterVersion(self):
         try:
             urlForHealth = f"http://{self.hostname}:8091/pools"
             #print(self.hostname)
             getNodeDetails = requests.get(
                 url=urlForHealth, auth=(self.logininformation, self.loginsecret))
@@ -169,14 +200,15 @@
     def getSettings(self):
         try:
             urlForHealth = f"http://{self.hostname}:8091/settings/autoFailover"
             getNodeDetails = requests.get(
                 url=urlForHealth, auth=(self.logininformation, self.loginsecret))
             resultParsed = getNodeDetails.json()
             settingsArray=[]
+            self.autofailoverEnabled=resultParsed.get('enabled')
             settingModel={
                 "configName": 'autofailover',
                 "status": resultParsed.get('enabled'),
             }
             settingsArray.append(settingModel)
             urlForHealth = f"http://{self.hostname}:8091/settings/alerts"
             getNodeDetails = requests.get(
@@ -195,88 +227,222 @@
                 "configName": 'auto-compaction',
                 "status": resultParsed.get('autoCompactionSettings').get('databaseFragmentationThreshold').get('percentage')
             }
             settingsArray.append(settingModel)
             self.settingsCluster=settingsArray
         except Exception as couchbaseBucketException:
             print(couchbaseBucketException)
-    def takePicture(self):
+    def generateReport(self):
+        reportDetail=[]
+        if self.allNodesAreHealthy==True:
+            tableRecord={
+                "Statement" : "All nodes are healthy and joined cluster",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                 "Statement" : "All nodes are healthy and joined cluster",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        if self.allNodesSameVersion==True:
+            tableRecord={
+                "Statement" : "All nodes using same version of Cocuhbase",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : "All nodes using same version of Cocuhbase",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        if self.mdsApplied==True:
+            tableRecord={
+                "Statement" : "MDS model applied",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : "MDS model applied",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        if self.allBucketsResident==True:
+            tableRecord={
+                "Statement" : "All buckets have resident ratio greater than %50",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : "All buckets have resident ratio greater than %50",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        if self.allBucketHaveAtLeastOneReplica==True:
+            tableRecord={
+                "Statement" : "All bucket have at least 1 replica to protect data",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : "All bucket have at least 1 replica to protect data",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        if self.allBucketPrimaryVbucketGood==True:
+            tableRecord={
+                "Statement" : "There is no missing primary vbucket",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : "There is no missing primary vbucket",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        if self.autofailoverEnabled==True:
+            tableRecord={
+                "Statement" : "Auto-failover setting is enabled",
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : "Auto-failover setting is enabled",
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+
+        if self.clusterScore > 50:
+            tableRecord={
+                "Statement" : f'''Cluster Score {self.clusterScore}''',
+                "Result": "\U0001F7E2"
+            }
+            reportDetail.append(tableRecord)
+        else:
+            tableRecord={
+                "Statement" : f'''Cluster Score {self.clusterScore}''',
+                "Result": "\u274C"
+            }
+            reportDetail.append(tableRecord)
+        dataFrameReport=pd.DataFrame(reportDetail)
+        print(tabulate(dataFrameReport, headers = 'keys', tablefmt = 'fancy_grid',numalign="center", stralign="center"))
+        if len(self.checkResults) > 0:
+            dataFrameResults=pd.DataFrame(self.checkResults)
+            print(tabulate(dataFrameResults, headers = 'keys', tablefmt = 'fancy_grid',numalign="center", stralign="center"))
+        return True
+    def generateResults(self):
         clusterNodes=self.clusterNodes
         clusterBuckets=self.buckets
-        clusterRoles=self.usersOnCluster
-        clusterSettings=self.settingsCluster
-        clusterXdcr=self.xdcrConnections
-        dataFrameforNodes=pd.DataFrame(clusterNodes)
-        dataFrameforBuckets=pd.DataFrame(clusterBuckets)
-        dataFrameforRoles=pd.DataFrame(clusterRoles)
-        dataFrameforXdcr=pd.DataFrame(clusterXdcr)
-        dataFrameFailover=pd.DataFrame(clusterSettings)
-        print("----- Cluster Nodes -----")
-        print(tabulate(dataFrameforNodes, headers = 'keys', tablefmt = 'psql'))
-        print("----- Cluster Buckets -----")
-        print(tabulate(dataFrameforBuckets, headers = 'keys', tablefmt = 'psql'))
-        print("----- Cluster XDCR -----")
-        print(tabulate(dataFrameforXdcr, headers = 'keys', tablefmt = 'psql'))
-        print("----- Cluster Roles -----")
-        print(tabulate(dataFrameforRoles, headers = 'keys', tablefmt = 'psql'))
-        print("----- Cluster Settings -----")
-        print(tabulate(dataFrameFailover, headers = 'keys', tablefmt = 'psql'))
         checkResults=[]
         nodeVersions=[]
+        if self.autofailoverEnabled==False:
+            self.clusterScore=self.clusterScore-10
+            checkModel={
+                    "problemStatement": 'Autofailover setting is not enabled',
+                    "problemArea": "Configuration",
+                    "problemSeverity": 'Critical'
+                }
+            checkResults.append(checkModel)
+        else:
+            pass
         for node in clusterNodes:
             healtStatus=node.get('healtStatus')
             clusterMember=node.get('clusterMember')
             nodeVersion=node.get('couchbaseVersion')
-            nodeVersions.append(nodeVersion)
+            if nodeVersion not in nodeVersions:
+                nodeVersions.append(nodeVersion)
             mdsControlCount=len(node.get('services'))
             if healtStatus!='healthy' or clusterMember!='active':
+                self.clusterScore=self.clusterScore-20
+                self.allNodesAreHealthy=False
                 checkModel={
                     "problemStatement": 'Node is not available or joined cluster.',
                     "problemArea": node.get('nodeIP'),
                     "problemSeverity": 'Critical'
                 }
                 checkResults.append(checkModel)
             else:
                 pass
             if mdsControlCount > 1:
+                self.mdsApplied=False
+                self.clusterScore=self.clusterScore-10
                 checkModel={
                     "problemStatement": 'The node has multiple couchbase services.For production MDS model should be followed.',
                     "problemArea": node.get('nodeIP'),
                     "problemSeverity": 'Medium'
                 }
                 checkResults.append(checkModel)
         for bucket in clusterBuckets:
             bucketReplica=bucket.get('bucketReplicas')
             vbucketCount=bucket.get('primaryVbucketCount')
             bucketResident=bucket.get('bucketResidentRatio')
             if bucketReplica==0:
+                self.allBucketHaveAtLeastOneReplica=False
+                self.clusterScore=self.clusterScore-20
                 checkModel={
                     "problemStatement": f''' {bucket.get('bucketName')} has no replica configured''',
                     "problemArea": 'Bucket',
                     "problemSeverity": 'Critical'
                 }
                 checkResults.append(checkModel)
             elif bucketReplica==3:
+                self.clusterScore=self.clusterScore-5
                 checkModel={
                     "problemStatement": f''' {bucket.get('bucketName')} has 3 replica configured''',
                     "problemArea": 'Bucket',
                     "problemSeverity": 'Warming'
                 }
                 checkResults.append(checkModel)
             if vbucketCount%1024!=0:
+                self.allBucketPrimaryVbucketGood=False
+                self.clusterScore=self.clusterScore-30
                 checkModel={
                     "problemStatement": f''' {bucket.get('bucketName')} has missing primary vbucket''',
                     "problemArea": 'Bucket',
                     "problemSeverity": 'Critical'
                 }
                 checkResults.append(checkModel)
             if bucketResident < 10:
+                self.clusterScore=self.clusterScore-20
+                self.allBucketsResident=False
                 checkModel={
                     "problemStatement": f''' {bucket.get('bucketName')} has low resident ratio''',
                     "problemArea": 'Bucket',
                     "problemSeverity": 'Critical'
                 }
                 checkResults.append(checkModel)
-        dataFrameResults=pd.DataFrame(checkResults)
-        print("----- Check Notes -----")
-        print(tabulate(dataFrameResults, headers = 'keys', tablefmt = 'psql'))
-        return f''' Finished healtcheck.'''
+            if len(nodeVersions) > 1:
+                self.clusterScore=self.clusterScore-10
+                self.allNodesSameVersion=False
+                checkModel={
+                    "problemStatement": "All nodes are not using the same version of Couchbase",
+                    "problemArea": 'Cluster',
+                    "problemSeverity": 'Critical'
+                }
+                checkResults.append(checkModel)
+        self.checkResults=checkResults
+    def takePicture(self):
+        clusterNodes=self.clusterNodes
+        clusterBuckets=self.buckets
+        clusterRoles=self.usersOnCluster
+        clusterSettings=self.settingsCluster
+        clusterXdcr=self.xdcrConnections
+        dataFrameforNodes=pd.DataFrame(clusterNodes)
+        dataFrameforBuckets=pd.DataFrame(clusterBuckets)
+        dataFrameforRoles=pd.DataFrame(clusterRoles)
+        dataFrameforXdcr=pd.DataFrame(clusterXdcr)
+        dataFrameFailover=pd.DataFrame(clusterSettings)
+        print("-- Details -- ")
+        print(tabulate(dataFrameforNodes, headers = 'keys', tablefmt = 'psql'))
+        print(tabulate(dataFrameforBuckets, headers = 'keys', tablefmt = 'psql'))
+        print(tabulate(dataFrameforXdcr, headers = 'keys', tablefmt = 'psql'))
+        print(tabulate(dataFrameforRoles, headers = 'keys', tablefmt = 'psql'))
+        print(tabulate(dataFrameFailover, headers = 'keys', tablefmt = 'psql'))
+        return f''' Finished healtcheck.'''
+
```

