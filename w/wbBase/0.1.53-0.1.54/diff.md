# Comparing `tmp/wbBase-0.1.53.tar.gz` & `tmp/wbBase-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.1.53.tar", last modified: Sat Apr 22 07:30:58 2023, max compression
+gzip compressed data, was "wbBase-0.1.54.tar", last modified: Sat Apr 22 15:07:46 2023, max compression
```

## Comparing `wbBase-0.1.53.tar` & `wbBase-0.1.54.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.475400 wbBase-0.1.53/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-22 07:30:56.000000 wbBase-0.1.53/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.462399 wbBase-0.1.53/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.468400 wbBase-0.1.53/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.472400 wbBase-0.1.53/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47198 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.473400 wbBase-0.1.53/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.475400 wbBase-0.1.53/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8136 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.470400 wbBase-0.1.53/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 07:30:58.475400 wbBase-0.1.53/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-22 07:30:56.000000 wbBase-0.1.53/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-22 07:30:58.476400 wbBase-0.1.53/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 07:30:56.000000 wbBase-0.1.53/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.038702 wbBase-0.1.54/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-22 15:07:44.000000 wbBase-0.1.54/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.026703 wbBase-0.1.54/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.032702 wbBase-0.1.54/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23965 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.035702 wbBase-0.1.54/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.036702 wbBase-0.1.54/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.038702 wbBase-0.1.54/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8136 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-22 15:07:44.000000 wbBase-0.1.54/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 15:07:46.033702 wbBase-0.1.54/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-22 15:07:46.000000 wbBase-0.1.54/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 15:07:46.038702 wbBase-0.1.54/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-22 15:07:44.000000 wbBase-0.1.54/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-22 15:07:46.039702 wbBase-0.1.54/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 15:07:44.000000 wbBase-0.1.54/setup.py
```

### Comparing `wbBase-0.1.53/LICENSE` & `wbBase-0.1.54/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/application.py` & `wbBase-0.1.54/Lib/wbBase/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,14 +536,15 @@
                         sharedMemory.write_byte(
                             ord("+")
                         )  # set finished writing marker
                         sharedMemory.flush()
                         break
                     else:
                         time.sleep(1)  # give enough time for buffer to be available
+            sys.exit(0)
         else:
             self.listenAndLoadTimer.Start(250)
 
     def prepareSharedDataFolder(self) -> None:
         self.splashMessage("Preparing shared data folder")
         cfg = self.config
         defaultFolder = os.path.join(self.dirs.user_data_dir, "shared")
```

### Comparing `wbBase-0.1.53/Lib/wbBase/applicationInfo.py` & `wbBase-0.1.54/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/applicationWindow.py` & `wbBase-0.1.54/Lib/wbBase/applicationWindow.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/artprovider.py` & `wbBase-0.1.54/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/__init__.py` & `wbBase-0.1.54/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.1.54/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.1.54/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/filling.py` & `wbBase-0.1.54/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/iePanel.py` & `wbBase-0.1.54/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/propgrid.py` & `wbBase-0.1.54/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/control/textEditControl.py` & `wbBase-0.1.54/Lib/wbBase/control/textEditControl.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.1.54/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/dialog/preferences.py` & `wbBase-0.1.54/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/document/__init__.py` & `wbBase-0.1.54/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/document/manager.py` & `wbBase-0.1.54/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/document/notebook.py` & `wbBase-0.1.54/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/document/template.py` & `wbBase-0.1.54/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/document/view.py` & `wbBase-0.1.54/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/panelManager.py` & `wbBase-0.1.54/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/pluginManager.py` & `wbBase-0.1.54/Lib/wbBase/pluginManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/pluginManager_old.py` & `wbBase-0.1.54/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/scripting.py` & `wbBase-0.1.54/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase/tools.py` & `wbBase-0.1.54/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.1.54/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.53
+Version: 0.1.54
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.53/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.1.54/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/PKG-INFO` & `wbBase-0.1.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.53
+Version: 0.1.54
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
```

### Comparing `wbBase-0.1.53/README.md` & `wbBase-0.1.54/README.md`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.53/setup.cfg` & `wbBase-0.1.54/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.53
+current_version = 0.1.54
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -64,15 +64,15 @@
 where = Lib
 
 [bumpversion:file:Lib/wbBase/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.3
+min_version = 4.4
 env_list = 
 	py38
 	py39
 	py10
 
 [testenv]
 deps =
```

