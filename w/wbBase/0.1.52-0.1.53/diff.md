# Comparing `tmp/wbBase-0.1.52.tar.gz` & `tmp/wbBase-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbBase-0.1.52.tar", last modified: Fri Apr  7 14:44:05 2023, max compression
+gzip compressed data, was "wbBase-0.1.53.tar", last modified: Sat Apr 22 07:30:58 2023, max compression
```

## Comparing `wbBase-0.1.52.tar` & `wbBase-0.1.53.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.171622 wbBase-0.1.52/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-07 14:44:03.000000 wbBase-0.1.52/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.158621 wbBase-0.1.52/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.164621 wbBase-0.1.52/Lib/wbBase/
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23824 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/application.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/applicationInfo.py
--rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/applicationWindow.py
--rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/artprovider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.168622 wbBase-0.1.52/Lib/wbBase/control/
--rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/externalToolConfig.py
--rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/externalToolConfigUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/filling.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/iePanel.py
--rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/propgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    47311 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/control/textEditControl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.169622 wbBase-0.1.52/Lib/wbBase/dialog/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/dialog/multiSaveModifiedDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/dialog/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.171622 wbBase-0.1.52/Lib/wbBase/document/
--rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/document/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/document/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/document/template.py
--rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/document/view.py
--rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/panelManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1773 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/pluginManager.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/pluginManager_old.py
--rw-rw-rw-   0 root         (0) root         (0)     8136 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/scripting.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-07 14:44:03.000000 wbBase-0.1.52/Lib/wbBase/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 14:44:05.165622 wbBase-0.1.52/Lib/wbBase.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-07 14:44:05.000000 wbBase-0.1.52/Lib/wbBase.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1027 2023-04-07 14:44:05.000000 wbBase-0.1.52/Lib/wbBase.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 14:44:05.000000 wbBase-0.1.52/Lib/wbBase.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-07 14:44:05.000000 wbBase-0.1.52/Lib/wbBase.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-07 14:44:05.000000 wbBase-0.1.52/Lib/wbBase.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2382 2023-04-07 14:44:05.171622 wbBase-0.1.52/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-04-07 14:44:03.000000 wbBase-0.1.52/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1941 2023-04-07 14:44:05.172622 wbBase-0.1.52/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-07 14:44:03.000000 wbBase-0.1.52/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.475400 wbBase-0.1.53/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-22 07:30:56.000000 wbBase-0.1.53/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.462399 wbBase-0.1.53/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.468400 wbBase-0.1.53/Lib/wbBase/
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/applicationInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)    20585 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/applicationWindow.py
+-rw-rw-rw-   0 root         (0) root         (0)   309800 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/artprovider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.472400 wbBase-0.1.53/Lib/wbBase/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4414 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/externalToolConfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     5891 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/externalToolConfigUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/iePanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8569 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/propgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    47198 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/control/textEditControl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.473400 wbBase-0.1.53/Lib/wbBase/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2342 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3293 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    20381 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/dialog/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.475400 wbBase-0.1.53/Lib/wbBase/document/
+-rw-rw-rw-   0 root         (0) root         (0)    23492 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36999 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4743 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     8016 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9208 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/document/view.py
+-rw-rw-rw-   0 root         (0) root         (0)    21455 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/panelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/pluginManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/pluginManager_old.py
+-rw-rw-rw-   0 root         (0) root         (0)     8136 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/scripting.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-22 07:30:56.000000 wbBase-0.1.53/Lib/wbBase/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 07:30:58.470400 wbBase-0.1.53/Lib/wbBase.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-22 07:30:58.000000 wbBase-0.1.53/Lib/wbBase.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-22 07:30:58.475400 wbBase-0.1.53/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-04-22 07:30:56.000000 wbBase-0.1.53/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-04-22 07:30:58.476400 wbBase-0.1.53/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 07:30:56.000000 wbBase-0.1.53/setup.py
```

### Comparing `wbBase-0.1.52/LICENSE` & `wbBase-0.1.53/LICENSE`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/application.py` & `wbBase-0.1.53/Lib/wbBase/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,17 @@
         :return: Return code
         """
         self.TopWindow.Show(True)
         self._handleCmdLineArguments()
         if self._splashScreen:
             self._splashScreen.Destroy()
             self._splashScreen = None
+        main = sys.modules.get("__main__")
+        if "main" in main.__dict__:
+            del main.__dict__["main"]
         return super().OnRun()
 
     def run(self) -> int:
         """
         Start the application by calling :meth:`OnRun`
 
         :return: Return code
```

### Comparing `wbBase-0.1.52/Lib/wbBase/applicationInfo.py` & `wbBase-0.1.53/Lib/wbBase/applicationInfo.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/applicationWindow.py` & `wbBase-0.1.53/Lib/wbBase/applicationWindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,10 +572,10 @@
         adv.AboutBox(info)
 
     def on_help_about_plugin(self, event: wx.CommandEvent):
         message = "Plugin version info\n============================\n"
         for pluginName in sorted(self.pluginManager, key=str.lower):
             plugin = self.pluginManager[pluginName]
             if hasattr(plugin, "__version__"):
-                message += f"{pluginName:20}\t{plugin.__version__}\n"
+                message += f"{pluginName:30}\t{plugin.__version__}\n"
         with ScrolledMessageDialog(self, message, "About Plugins") as dlg:
             dlg.ShowModal()
```

### Comparing `wbBase-0.1.52/Lib/wbBase/artprovider.py` & `wbBase-0.1.53/Lib/wbBase/artprovider.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/__init__.py` & `wbBase-0.1.53/Lib/wbBase/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/externalToolConfig.py` & `wbBase-0.1.53/Lib/wbBase/control/externalToolConfig.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/externalToolConfigUI.py` & `wbBase-0.1.53/Lib/wbBase/control/externalToolConfigUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/filling.py` & `wbBase-0.1.53/Lib/wbBase/control/filling.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/iePanel.py` & `wbBase-0.1.53/Lib/wbBase/control/iePanel.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/propgrid.py` & `wbBase-0.1.53/Lib/wbBase/control/propgrid.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/control/textEditControl.py` & `wbBase-0.1.53/Lib/wbBase/control/textEditControl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1192,23 +1192,23 @@
         self.syntax["STC_P_STRINGEOL"] = "fore:#800080"
 
 
 class XmlTextEditConfig(TextEditConfig):
     def __init__(self, parent):
         super().__init__(parent)
         self.syntax["STC_H_DEFAULT"] = "fore:black,back:white"
-        self.syntax["STC_H_XMLSTART"] = "fore:black,back:white"
-        self.syntax["STC_H_XMLEND"] = "fore:black,back:white"
-        self.syntax["STC_H_TAG"] = "fore:black,back:white"
-        self.syntax["STC_H_TAGEND"] = "fore:black,back:white"
-        self.syntax["STC_H_TAGUNKNOWN"] = "fore:black,back:white"
-        self.syntax["STC_H_ATTRIBUTE"] = "fore:black,back:white"
-        self.syntax["STC_H_ATTRIBUTEUNKNOWN"] = "fore:black,back:white"
-        self.syntax["STC_H_NUMBER"] = "fore:black,back:white"
-        self.syntax["STC_H_SINGLESTRING"] = "fore:black,back:white"
-        self.syntax["STC_H_DOUBLESTRING"] = "fore:black,back:white"
-        self.syntax["STC_H_OTHER"] = "fore:black,back:white"
-        self.syntax["STC_H_COMMENT"] = "fore:black,back:white"
-        self.syntax["STC_H_ENTITY"] = "fore:black,back:white"
-        self.syntax["STC_H_VALUE"] = "fore:black,back:white"
-        self.syntax["STC_H_QUESTION"] = "fore:black,back:white"
-        self.syntax["STC_H_CDATA"] = "fore:black,back:white"
+        self.syntax["STC_H_XMLSTART"] = "fore:#CA0000,bold"
+        self.syntax["STC_H_XMLEND"] = "fore:#CA0000,bold"
+        self.syntax["STC_H_TAG"] = "fore:#800040,bold"
+        self.syntax["STC_H_TAGEND"] = "#fore:800040,bold"
+        self.syntax["STC_H_TAGUNKNOWN"] = "#fore:800040,bold"
+        self.syntax["STC_H_ATTRIBUTE"] = "fore:#804000,italic"
+        self.syntax["STC_H_ATTRIBUTEUNKNOWN"] = "fore:#804000,italic"
+        self.syntax["STC_H_NUMBER"] = "fore:black"
+        self.syntax["STC_H_SINGLESTRING"] = "fore:#004080"
+        self.syntax["STC_H_DOUBLESTRING"] = "fore:#004080"
+        self.syntax["STC_H_OTHER"] = "fore:black"
+        self.syntax["STC_H_COMMENT"] = "fore:#8B8B8B"
+        self.syntax["STC_H_ENTITY"] = "fore:#008000"
+        self.syntax["STC_H_VALUE"] = "fore:black"
+        self.syntax["STC_H_QUESTION"] = "fore:black"
+        self.syntax["STC_H_CDATA"] = "fore:#8000FF"
```

### Comparing `wbBase-0.1.52/Lib/wbBase/dialog/multiSaveModifiedDialog.py` & `wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialog.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py` & `wbBase-0.1.53/Lib/wbBase/dialog/multiSaveModifiedDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/dialog/preferences.py` & `wbBase-0.1.53/Lib/wbBase/dialog/preferences.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/document/__init__.py` & `wbBase-0.1.53/Lib/wbBase/document/__init__.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/document/manager.py` & `wbBase-0.1.53/Lib/wbBase/document/manager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/document/notebook.py` & `wbBase-0.1.53/Lib/wbBase/document/notebook.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/document/template.py` & `wbBase-0.1.53/Lib/wbBase/document/template.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/document/view.py` & `wbBase-0.1.53/Lib/wbBase/document/view.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/panelManager.py` & `wbBase-0.1.53/Lib/wbBase/panelManager.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/pluginManager.py` & `wbBase-0.1.53/Lib/wbBase/pluginManager.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 pluginManager
 ========================================================
 
 Test new PluginManager class.
 """
 
 from __future__ import annotations
-
+from logging import getLogger
 import sys
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
 from typing import TYPE_CHECKING
 
 import wx
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
+log = getLogger(__name__)
+
 
 class PluginManager(dict):
     def __init__(self):
         super().__init__()
         self.loadPlugins()
 
     def __repr__(self) -> str:
@@ -42,23 +44,42 @@
         app.splashMessage("loading plugins")
         available_plugins = {}
         entryPoints = entry_points(group="wbbase.plugin")
         if entryPoints:
             available_plugins = {e.name: e for e in entryPoints}
         appInfo_plugins = app.info.Plugins
         disabled_plugins = app.cmdLineArguments.disabledPlugins or []
+        main = sys.modules.get("__main__")
+        main.__dict__["app"] = app
         for plugin in appInfo_plugins:
             if plugin.Installation == "exclude":
                 continue
             name = plugin.Name
             if name in disabled_plugins:
                 continue
             app.splashMessage(f"loading plugin {name}")
             if name in available_plugins:
-                self[name] = available_plugins[name].load()
+                try:
+                    module = available_plugins[name].load()
+                    if hasattr(module, "globalObjects"):
+                        for globalObject in module.globalObjects:
+                            if (
+                                globalObject not in main.__dict__
+                                and globalObject not in self.app.globalObjects
+                                and hasattr(module, globalObject)
+                            ):
+                                main.__dict__[globalObject] = getattr(
+                                    module, globalObject
+                                )
+                                self.app.globalObjects.append(globalObject)
+                    self[name] = module
+                except ImportError:
+                    log.exception(
+                        "=============== Can't load plugin %s ===============", name
+                    )
             elif plugin.Installation == "required":
                 wx.LogError(
                     "Missing required plugin\n\n"
                     f"Can't load plugin '{name}'\n"
                     "Application will terminate."
                 )
                 sys.exit(1)
```

### Comparing `wbBase-0.1.52/Lib/wbBase/pluginManager_old.py` & `wbBase-0.1.53/Lib/wbBase/pluginManager_old.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/scripting.py` & `wbBase-0.1.53/Lib/wbBase/scripting.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase/tools.py` & `wbBase-0.1.53/Lib/wbBase/tools.py`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/Lib/wbBase.egg-info/PKG-INFO` & `wbBase-0.1.53/Lib/wbBase.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.52
+Version: 0.1.53
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
@@ -21,18 +21,19 @@
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbBase
 
 This is the base package for WorkBench applications.
 Workbench is a plugin based RAD framework for platform independent GUI applications
@@ -52,14 +53,18 @@
 The following plugins are currently available as individual packages.
 
 - [wbpOutput](https://pypi.org/project/wbpoutput/), 
     an output panel for Workbench applications.
 - [wbpShell](https://pypi.org/project/wbpshell/), 
     a shell panel for Workbench applications.
 - [wbpLoglist](https://pypi.org/project/wbploglist/),
-    a log list panel panel for Workbench applications.
+    a log list panel for Workbench applications.
 - [wbpNamespace](https://pypi.org/project/wbpnamespace/),
     a namespace panel for Workbench applications.
 - [wbpWidgetinspector](https://pypi.org/project/wbpwidgetinspector/)
     integrates the Widgetinspector in Workbench applications.
 - [wbpFilebrowser](https://pypi.org/project/wbpfilebrowser/),
-    a file browser panel panel for Workbench applications.
+    a file browser panel for Workbench applications.
+- [wbpTextedit](https://pypi.org/project/wbptextedit/),
+    document templates to create, view and edit some text file types.
+- [wbpUItools](https://pypi.org/project/wbpuitools/),
+    collection of some useful functions for user interaction in Python scripts.
```

### Comparing `wbBase-0.1.52/Lib/wbBase.egg-info/SOURCES.txt` & `wbBase-0.1.53/Lib/wbBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbBase-0.1.52/PKG-INFO` & `wbBase-0.1.53/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbBase
-Version: 0.1.52
+Version: 0.1.53
 Summary: Base package for WorkBench applications.
 Home-page: https://gitlab.com/workbench2/wbbase
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/wbbase
 Project-URL: Documentation, https://workbench2.gitlab.io/wbbase
 Project-URL: Tracker, https://gitlab.com/workbench2/wbbase/-/issues
@@ -21,18 +21,19 @@
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbBase
 
 This is the base package for WorkBench applications.
 Workbench is a plugin based RAD framework for platform independent GUI applications
@@ -52,14 +53,18 @@
 The following plugins are currently available as individual packages.
 
 - [wbpOutput](https://pypi.org/project/wbpoutput/), 
     an output panel for Workbench applications.
 - [wbpShell](https://pypi.org/project/wbpshell/), 
     a shell panel for Workbench applications.
 - [wbpLoglist](https://pypi.org/project/wbploglist/),
-    a log list panel panel for Workbench applications.
+    a log list panel for Workbench applications.
 - [wbpNamespace](https://pypi.org/project/wbpnamespace/),
     a namespace panel for Workbench applications.
 - [wbpWidgetinspector](https://pypi.org/project/wbpwidgetinspector/)
     integrates the Widgetinspector in Workbench applications.
 - [wbpFilebrowser](https://pypi.org/project/wbpfilebrowser/),
-    a file browser panel panel for Workbench applications.
+    a file browser panel for Workbench applications.
+- [wbpTextedit](https://pypi.org/project/wbptextedit/),
+    document templates to create, view and edit some text file types.
+- [wbpUItools](https://pypi.org/project/wbpuitools/),
+    collection of some useful functions for user interaction in Python scripts.
```

### Comparing `wbBase-0.1.52/README.md` & `wbBase-0.1.53/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 The following plugins are currently available as individual packages.
 
 - [wbpOutput](https://pypi.org/project/wbpoutput/), 
     an output panel for Workbench applications.
 - [wbpShell](https://pypi.org/project/wbpshell/), 
     a shell panel for Workbench applications.
 - [wbpLoglist](https://pypi.org/project/wbploglist/),
-    a log list panel panel for Workbench applications.
+    a log list panel for Workbench applications.
 - [wbpNamespace](https://pypi.org/project/wbpnamespace/),
     a namespace panel for Workbench applications.
 - [wbpWidgetinspector](https://pypi.org/project/wbpwidgetinspector/)
     integrates the Widgetinspector in Workbench applications.
 - [wbpFilebrowser](https://pypi.org/project/wbpfilebrowser/),
-    a file browser panel panel for Workbench applications.
+    a file browser panel for Workbench applications.
+- [wbpTextedit](https://pypi.org/project/wbptextedit/),
+    document templates to create, view and edit some text file types.
+- [wbpUItools](https://pypi.org/project/wbpuitools/),
+    collection of some useful functions for user interaction in Python scripts.
```

### Comparing `wbBase-0.1.52/setup.cfg` & `wbBase-0.1.53/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.52
+current_version = 0.1.53
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -39,23 +39,24 @@
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.8,<3.11
 install_requires = 
 	appdirs>=1.4.4
 	wxpython>=4.2.0
 	GitPython>=3.1
 	PyYAML>=6.0
 	importlib_metadata;python_version<'3.10'
```

