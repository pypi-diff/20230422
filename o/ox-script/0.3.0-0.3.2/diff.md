# Comparing `tmp/ox_script-0.3.0.tar.gz` & `tmp/ox_script-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ox_script-0.3.0.tar", last modified: Sat Apr 22 17:54:38 2023, max compression
+gzip compressed data, was "dist/ox_script-0.3.2.tar", last modified: Sat Apr 22 20:00:01 2023, max compression
```

## Comparing `ox_script-0.3.0.tar` & `ox_script-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 17:54:38.000000 ox_script-0.3.0/
--rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 17:54:38.000000 ox_script-0.3.0/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)       22 2023-04-22 17:54:04.000000 ox_script-0.3.0/__init__.py
--rw-------   0 jarvislu   (501) staff       (20)    38368 2023-04-22 17:09:09.000000 ox_script-0.3.0/pskfunc.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-0.3.0/MANIFEST.in
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 17:54:38.000000 ox_script-0.3.0/ox_script.egg-info/
--rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 17:54:38.000000 ox_script-0.3.0/ox_script.egg-info/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)      207 2023-04-22 17:54:38.000000 ox_script-0.3.0/ox_script.egg-info/SOURCES.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-22 17:54:38.000000 ox_script-0.3.0/ox_script.egg-info/requires.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 17:54:38.000000 ox_script-0.3.0/ox_script.egg-info/top_level.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 17:54:38.000000 ox_script-0.3.0/ox_script.egg-info/dependency_links.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)      875 2023-04-22 17:54:30.000000 ox_script-0.3.0/setup.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 17:54:38.000000 ox_script-0.3.0/setup.cfg
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 20:00:01.000000 ox_script-0.3.2/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 20:00:01.000000 ox_script-0.3.2/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-0.3.2/MANIFEST.in
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script/
+-rw-------   0 jarvislu   (501) staff       (20)    12092 2023-04-22 19:58:19.000000 ox_script-0.3.2/ox_script/general_purpose_apis.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 19:58:19.000000 ox_script-0.3.2/ox_script/__init__.py
+-rw-------   0 jarvislu   (501) staff       (20)    25033 2023-04-22 19:58:19.000000 ox_script-0.3.2/ox_script/printer_specific_apis.py
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)      275 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/requires.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       10 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/top_level.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 20:00:01.000000 ox_script-0.3.2/ox_script.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)      875 2023-04-22 19:58:29.000000 ox_script-0.3.2/setup.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 20:00:01.000000 ox_script-0.3.2/setup.cfg
```

### Comparing `ox_script-0.3.0/PKG-INFO` & `ox_script-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox_script
-Version: 0.3.0
+Version: 0.3.2
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Postek Electronics Co., Ltd.
 Author-email: support@postek.com.cn
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox_script-0.3.0/pskfunc.py` & `ox_script-0.3.2/ox_script/printer_specific_apis.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,20 +22,15 @@
 
 # For the functions that only have pass in this file, please refer to the ox script development manual for details
 # The functions are marked with pass only because they are meanted to be executed on the printer and will not function
 # correctly on your device. Please use the runtime environment on Postek printers for most accurate results
 
 
 # --coding: utf-8 --
-import re
-import pandas
-import openpyxl
 import string
-import os
-
 
 def debuglog(info: str):
     """
     Log the information to the debug log file stored inside the printer
 
     Parameters:
         info (str): The information to be logged
@@ -100,188 +95,188 @@
 
     Returns:
         bytes: The data read from the printer
     """
     pass
 
 
-def PTK_SendCmdToPrinter(cmd: str) -> bool/str:
+def PTK_SendCmdToPrinter(cmd: str) -> bool:
     """
     PTK_SendCmdToPrinter is used to send commands loadded from Forms to the printer
 
     Parameters:
         cmd (str): The command to be sent to the printer
 
     Returns:
         bool: The command was sent successfully
         String: The error message if the command was not sent successfully
     """
-    pass
+    return True
 
 # ===========================================================#
 # Functions related to the printer settings
 # ===========================================================#
 
 
 BOTTOM_RIGHT = "T"
 TOP_LEFT = "B"
 
 
-def PTK_SetPrintDirection(direction: string) -> bool/str:
+def PTK_SetPrintDirection(direction: string) -> bool:
     """
     PTK_SetPrintDirection is used to set the print direction of the printer. The default direction starts at bottom right.
 
     Parameters:
         direction (string): The direction to be used. "T" -> Top Left, "B" -> Bottom Right
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_CutPage(number_of_labels=1, save_in_flash=False) -> bool/str:
+def PTK_CutPage(number_of_labels=1, save_in_flash=False) -> bool:
     """
     PTK_CutPage is used to cut the page after printing the number of labels specified
 
     Parameters:
         number_of_labels (int): The number of labels to be printed before cutting the page
         save_in_flash (bool): Save the command in flash so that the value can be restored when the printer powers up again
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_Reset() -> bool/str:
+def PTK_Reset() -> bool:
     """
     PTK_Reset is used to reset the printer
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 # ===========================================================#
 # Functions for print job related settings
 # ===========================================================#
 
-def PTK_SetDarkness(darkness: int) -> bool/str:
+def PTK_SetDarkness(darkness: int) -> bool:
     """
     PTK_SetDarkness is used to set the darkness of the print. The default darkness is 8.
 
     Parameters:
         darkness (int): The darkness to be used. The range is 0 to 20.
 
     Returns:
         int: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_SetLabelHeight(height: int, gapH=1) -> bool/str:
+def PTK_SetLabelHeight(height: int, gapH=1) -> bool:
     """
     PTK_SetLabelHeight is used to set the height of the label.
 
     Parameters:
         height (int): The height of the label in mm
         gapH (int): The gap between the labels in mm
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_SetLabelWidth(width: int) -> bool/str:
+def PTK_SetLabelWidth(width: int) -> bool:
     """
     PTK_SetLabelWidth is used to set the width of the label.
 
     Parameters:
         width (int): The width of the label in mm
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_SetCoordinateOrigin(x=0, y=0) -> bool/str:
+def PTK_SetCoordinateOrigin(x=0, y=0) -> bool:
     """
     PTK_SetCoordinateOrigin is used to set the origin of the coordinates. The default origin is (0,0).
 
     Parameters:
         x (int): The x coordinate of the origin
         y (int): The y coordinate of the origin
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_SetPrintSpeed(speed) -> bool/str:
+def PTK_SetPrintSpeed(speed) -> bool:
     """
     PTK_SetPrintSpeed is used to set the print speed of the printer. The default speed depends on the model of the printer.
 
     Parameters:
         speed (float): The speed to be used in inches per second. The range depends upon the model of the printer.
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 # ===========================================================#
 # Text related functions
 # ===========================================================#
 
 NORMAL = "N"
 REVERSE = "R"
 SDRAM = 0
 FLASH = 1
 
 
-def PTK_CreatFont(location, fontname, downloadfontname) -> bool/str:
+def PTK_CreatFont(location, fontname, downloadfontname) -> bool:
     """
     PTK_CreatFont is used to create a font in the printer
 
     Parameters:
         location (int): The location to store the font. 0 -> SDRAM, 1 -> Flash
         fontname (str): The name of the font to be created, the name should be in a single capital letters between A to Z
         downloadfontname (str): The name of the font to be downloaded
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 def PTK_DrawText(
     x_coordinate: int,
     y_coordinate: int,
     fonts: string,
     font_size: int,
     data: string,
     text_style="N",
     rotation=0,
     horizontal_multiplier=-1,
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawText is used to print text on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the text
         y_coordinate (int): The y coordinate of the text
         fonts (string): The font to be used. i.e "Inter", the Font should be stored in the fonts folder on the printer
@@ -291,24 +286,24 @@
         rotation (int): The rotation of the text. The range is 0 to 360
         horizontal_multiplier (int): The horizontal multiplier of the text. The range is 1 to 10
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 # ===========================================================#
 # 2D Barcode related functions
 # ===========================================================#
 
 
 def PTK_DrawBar2D_DATAMATRIX(
     x_coordinate: int, y_coordinate: int, multiplier: int, data: string, rotation=0
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawBar2D_DATAMATRIX is used to print a DataMatrix barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         multiplier (int): The multiplier of the barcode. The range is 1 to 9
@@ -316,28 +311,28 @@
         rotation (int): The rotation of the barcode. The range is 0 to 3 where
             0 = 0 degree, 1 = 90 degree, 2 = 180 degree, 3 = 270 degree
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 def PTK_DrawBar2D_QR(
     x_coordinate: int,
     y_coordinate: int,
     qr_version=0,
     rotation=0,
     multiplier=1,
     encode_mode=0,
     correction_level=0,
     masking=8,
     data='string',
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawBar2D_QR is used to print a QR barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         qr_version (int): The version of the QR code. The range is 0 to 40
@@ -350,54 +345,54 @@
         masking (int): The masking of the barcode. The range is 0 to 8
         data (string): The data to be printed in the barcode
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 UPS = 1
 NOT_UPS = 0
 
 
 def PTK_DrawBar2D_MaxiCode(
     x_coordinate: int, y_coordinate: int, mode: int, is_ups_data: int, data: string
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawBar2D_MaxiCode is used to print a MaxiCode barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         mode (int): The mode of the barcode. The range is 2 to 4
         is_ups_data (int): The ups data of the barcode. 0 -> Not UPS, 1 -> UPS
         data (string): The data to be printed in the barcode
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 def PTK_DrawBar2D_Pdf417(
     x_coordinate: int,
     y_coordinate: int,
     correction_level: int,
     data_compression_level: int,
     px: int,
     py: int,
     maxrow: int,
     maxcolumn: int,
     t: int,
     data: string,
     rotation=0,
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawBar2D_Pdf417 is used to print a Pdf417 barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         correction_level (int): The correction level of the barcode. The range is 0 to 8
@@ -411,27 +406,27 @@
         rotation (int): The rotation of the barcode. The range is 0 to 3 where
             0 = 0 degree, 1 = 90 degree, 2 = 180 degree, 3 = 270 degree
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 def PTK_DrawBar2D_HANXIN(
     x_coordinate: int,
     y_coordinate: int,
     multiplier: int,
     data: string,
     encoding=0,
     correction_level=0,
     masking=0,
     rotation=0,
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawBar2D_HANXIN is used to print a Han Xin barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         multiplier (int): The multiplier of the barcode. The range is 1 to 30
@@ -443,15 +438,15 @@
         rotation (int): The rotation of the barcode. The range is 0 to 3 where
             0 = 0 degree, 1 = 90 degree, 2 = 180 degree, 3 = 270 degree
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 # ===========================================================#
 # 1D Barcodes
 # ===========================================================#
 
 NO_TEXT = "N"
@@ -464,15 +459,15 @@
     barcode_type: string,
     narrow_unit_width: int,
     wide_unit_width: int,
     data: string,
     human_readable=TEXT,
     bar_height=10,
     rotation=0,
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawBarcode is used to print a 1D barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         barcode_type (string): The type of the barcode.
@@ -519,15 +514,15 @@
         rotation (int): The rotation of the barcode. The range is 0 to 3 where
             0 = 0 degree, 1 = 90 degree, 2 = 180 degree, 3 = 270 degree
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
 # ===========================================================#
 # Printing graphics
 # ===========================================================#
 
 def PTK_DrawGraphics(x, y, graphic_name):
@@ -539,181 +534,144 @@
         y (int): The y coordinate of the graphic
         graphic_name (string): The name of the graphic that is stored in the printer
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 # ===========================================================#
 # Printing lines
 # ===========================================================#
 
 
 def PTK_DrawDiagonal(
     x_coordinate: int,
     y_coordinate: int,
     thickness: int,
     end_point_x: int,
     end_point_y: int,
-) -> bool/str:
+) -> bool:
     """
      PTK_DrawDiagonal is used to draw lines on the label
 
      Parameters:
         x_coordinate (int): The x coordinate of the line
         y_coordinate (int): The y coordinate of the line
         thickness (int): The thickness of the line in mm
         end_point_x (int): The x coordinate of the end point of the line
         end_point_y (int): The y coordinate of the end point of the line
 
      Returns:
          bool: The function executed successfully
          String: The error message in string if an error occured
      """
-    pass
+    return True
 
 
 def PTK_DrawRectangle(
     x_coordinate: int,
     y_coordinate: int,
     thickness: int,
     end_point_x: int,
     end_point_y: int,
-) -> bool/str:
+) -> bool:
     """
     PTK_DrawRectangle is used to draw a rectangle on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the rectangle
         y_coordinate (int): The y coordinate of the rectangle
         thickness (int): The thickness of the rectangle in mm
         end_point_x (int): The x coordinate of the end point of the rectangle
         end_point_y (int): The y coordinate of the end point of the rectangle
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 # ===========================================================#
 # Printjob settings
 # ===========================================================#
 
 
-def PTK_PrintLabel(number_of_label=1, number_of_copy=1) -> bool/str:
+def PTK_PrintLabel(number_of_label=1, number_of_copy=1) -> bool:
     """
     PTK_PrintLabel is used to print the label
 
     Parameters:
         number_of_label (int): The number of label to be printed.
         number_of_copy (int): The number of copies to be printed.
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_PrintConfigunation() -> bool/str:
+def PTK_PrintConfigunation() -> bool:
     """
     PTK_PrintConfigunation is used to print the current configuration of the printer onto the label.
     Usually only used for debugging purposes
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 
-def PTK_FeedMedia() -> bool/str:
+def PTK_FeedMedia() -> bool:
     """
     PTK_FeedMedia is used to feed one label
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
+    return True
 
-
-def PTK_MediaCalibration() -> bool/str:
+def PTK_MediaCalibration() -> bool:
     """
     PTK_MediaCalibration is used to calibrate the media. If the calibration is successful the
     media size information will be stored and used for the next printjob unless specificed through
     PTK_SetLabelHeight or specificed through print job configuration
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
-    pass
+    return True
 
 # ===========================================================#
 # Functions to display information on the printer screen
 # ===========================================================#
 
 # Parent class of all UI elements
 # This shouldn't be used directly
 class UIWidgets:
     def __init__(self, name, value, Onpressed):
-        self.value = value
-        self.name = name
-        self.Onpressed = Onpressed
-        self.id = 0
-
-    def execute_function(self):
-        return self.Onpressed(self.value)
-
-    # 用户改变lcd屏上小组件的值
-    def update(self, value):
         pass
 
 # Button class used for creating a button on the printer screen
 # To create UI Elements use UIInit and UIPage
 class UIButton(UIWidgets):
     def __init__(self, Onpressed, name="测试按钮", visible=True):
-        self.type = "button"
-        self.Onpressed = Onpressed
-        self.name = name
-        self.value = '0'
-        self.visible = visible
-        self.id = 0
-
-
-    def return_json(self):
-        return {
-            "type": self.type,
-            "id": self.id,
-            "name": self.name,
-            "visible": self.visible,
-        }
+        pass
 
 
 # Text class used for just displaying text on the printer screen
 # To create UI Elements use UIInit and UIPage
 class UIText(UIWidgets):
     def __init__(self, value="--", name="测试文本", visible=True):
-        self.type = "text"
-        self.value = value
-        self.name = name
-        self.visible = visible
-        self.id = 0
-
-    def return_json(self):
-        return {
-            "type": "text",
-            "id": self.id,
-            "name": self.name,
-            "value": self.value,
-            "visible": self.visible,
-        }
+        pass
 
 # List class that can be used to create a drop down list on the printer screen
 # To create UI Elements use UIInit and UIPage
 class UIList(UIWidgets):
     def __init__(
         self,
         Onpressed,
@@ -721,37 +679,15 @@
         name="testing list",
         value="0",
         valueType="int",
         valueMax="1",
         valueMin="0",
         visible=True,
     ):
-        self.type = "list"
-        self.Onpressed = Onpressed
-        self.items = items
-        self.name = name
-        self.value = value
-        self.valueType = valueType
-        self.valueMax = valueMax
-        self.valueMin = valueMin
-        self.visible = visible
-        self.id = 0
-
-    def return_json(self):
-        return {
-            "type": "list",
-            "id": self.id,
-            "items": self.items,
-            "value": self.value,
-            "visible": self.visible,
-            "name": self.name,
-            "valueType": self.valueType,
-            "valueMax": self.valueMax,
-            "valueMin": self.valueMin,
-        }
+        pass
 
 # Input class that can be used to create a input box on the printer screen
 # To create UI Elements use UIInit and UIPage
 class UIInput(UIWidgets):
     def __init__(
         self,
         Onpressed,
@@ -759,72 +695,30 @@
         value="0",
         valueType="double",
         valueMax="10.0",
         valueMin="-10.0",
         dotNum=1,
         visible=True,
     ):
-        self.type = "input"
-        self.Onpressed = Onpressed
-        self.name = name
-        self.value = value
-        self.valueType = valueType
-        self.valueMax = valueMax
-        self.valueMin = valueMin
-        self.visible = visible
-        self.dotNum = dotNum
-        self.id = 0
-
-    def return_json(self):
-        return {
-            "type": "input",
-            "id": self.id,
-            "name": self.name,
-            "value": self.value,
-            "visible": self.visible,
-            "valueType": self.valueType,
-            "valueMax": self.valueMax,
-            "valueMin": self.valueMin,
-            "dotNum": self.dotNum,
-        }
+        pass
 
 # Checkbox class that can be used to create a checkbox on the printer screen
 # To create UI Elements use UIInit and UIPage
 class UICheckbox(UIWidgets):
     def __init__(
         self,
         Onpressed,
         name="测试复选框",
         value="0",
         valueType="bool",
         valueMax="1",
         valueMin="0",
         visible=True,
     ):
-        self.type = "checkbox"
-        self.Onpressed = Onpressed
-        self.name = name
-        self.value = value
-        self.valueType = valueType
-        self.valueMax = valueMax
-        self.valueMin = valueMin
-        self.visible = visible
-        self.id = 0
-
-    def return_json(self):
-        return {
-            "type": "checkbox",
-            "id": self.id,
-            "name": self.name,
-            "value": self.value,
-            "visible": self.visible,
-            "valueType": self.valueType,
-            "valueMax": self.valueMax,
-            "valueMin": self.valueMin,
-        }
+        pass
 
 
 def UIchangePage(pagenum):
     """
     UIchangePage can be used to change the page on the printer screen as
         a ox script can be used to create multiple pages
 
@@ -850,15 +744,15 @@
         *args (UIWidgets): The UI elements to be added to the page
 
     Returns:
         dict: The page in dictionary format, it is meanted to be used with UIInit and not
             used directly by the user
 
     """
-    pass
+    return {}
 
 # UI初始化
 def UIInit(*params, require_execute_confirmation=True) -> dict:
     """
     UIInit is used to initialize the UI elements on the printer screen. 
 
     Parameters:
@@ -879,280 +773,8 @@
     )
             
     Returns:
         controller (dict): The controller for the UI elements. The user can use the controllers
             to change the values of the UI elements on the printer screen
 
     """
-    pass
-
-
-# ===========================================================#
-# General purpose functions
-# These functions can be executed directly on your device
-# and is designed to help you with data parsing, connecting to 
-# databases, and getting data in the format to be printed
-# ===========================================================#
-
-# This class defines the basis of a database to be used like this 
-# data_base = PTKDataBase()
-# data_base.read_excel_file("example/path/example_file.xlsx")
-class PTKDataBase:
-    def __init__(self):
-        self.data = {}
-
-    def __getitem__(self, key):
-        return self.data[key]
-
-    def __str__(self) -> str:
-        returnStr = "{"
-        for key in self.data:
-            returnStr += "\n"
-            returnStr += f"  Table Name : {key} \n"
-            # returnStr += f"\n\t\t{self.data[key]}"
-            lines = pandas.DataFrame(
-                self.data[key].data_table).to_string(col_space=10)
-            for line in lines.split("\n"):
-                returnStr += f"\n\t{line}"
-            returnStr += "\n\n"
-            returnStr += "------------------------------------------------------------"
-            returnStr += "\n"
-        returnStr = returnStr.rsplit(
-            "------------------------------------------------------------", 1)[0] + "}"
-        return returnStr
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    def keys(self):
-        return self.data.keys()
-
-    def read_excel_file(self, file_path: str):
-        ws = openpyxl.load_workbook(file_path).active
-        column_names = [cell.value for cell in ws[1]]
-        base_path = os.path.splitext(os.path.basename(file_path))[0]
-        temp = {}
-        for column_index, column_name in enumerate(column_names):
-            column, column_name = [], ""
-            for cell in ws.iter_rows(
-                min_row=2, min_col=column_index + 1, max_col=column_index + 1
-            ):
-                if cell[0].value == None:
-                    continue
-                if column_name == "":
-                    column_name = cell[0].value
-                else:
-                    column.append(cell[0].value)
-            if column_name != "" and len(column) != 0:
-                temp[column_name] = column
-        self.data[base_path] = DataBaseEntry(temp)
-
-# This class defines the basis for an entry in the data base, not to be used directly
-class DataBaseEntry:
-    def __init__(self, data_table: map):
-        self.data_table = data_table
-
-    def __str__(self) -> str:
-        return pandas.DataFrame(self.data_table).to_string(col_space=10)
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    def __getitem__(self, key):
-        return self.data_table[key]
-
-    def get_max_row(self):
-        print(self.data_table.keys())
-        max_row = 0
-        for key in self.data_table.keys():
-            if len(self.data_table[key]) > max_row:
-                max_row = len(self.data_table[key])
-        return max_row
-
-    def get_max_col(self):
-        return len(self.data_table.keys())
-
-    def get_column_headers(self):
-        return self.column_headers
-
-def retrieve_data(item_list: list, index: int, excluding=""):
-    """
-    retrieve_data is used to retrieve data from a list of items. It can be used to retrieve data from a list
-        of items and user can use the excluding parameter to exclude items from the list. the excluding parameter
-        should be in the following format "starting_index;ending_index;exclusion_index". 
-    
-    Parameters:
-        item_list (list): The list of items to be retrieved from   
-        index (int): The index of the item to be retrieved
-        excluding (str, optional): The string that defines the exclusion of items. Defaults to "".
-
-    Returns:
-        str: The data from the item_list at the index specified with the exclusion applied
-    """
-    if excluding == "":
-        return item_list[index]
-    else:
-        pattern = r'^(\d*;){2}\d*$'
-        if re.match(pattern=pattern, string=excluding):
-            return _exclusion(item_list, index, excluding)
-        else:
-            print(
-                "excluding string in wrong format, it should follow starting_index;ending_index;exclusion_index")
-            return "exclusion string error"
-
-# This is an internal function. Not meant to be used directly
-def _exclusion(item_list: list, current_index: int, parameters=";;"):
-    parameters = parameters.split(";")
-    i = 0
-    for items in parameters:
-        if items == "":
-            if i == 0:
-                parameters[0] = "1"
-            elif i == 1:
-                parameters[1] = str(len(item_list))
-            elif i == 2:
-                parameters[2] = ""
-        i = i + 1
-
-    return _get_item_with_exclusion(
-        item_list, current_index, int(parameters[0]), int(
-            parameters[1]), parameters[2]
-    )
-
-# This is an internal function. Not meant to be used directly
-def _get_item_with_exclusion(
-    item_list: list,
-    current_index: int,
-    starting_index: int,
-    ending_index: int,
-    exclusion_index: str,
-):
-    try:
-        current_index = current_index + starting_index - 1
-        if (current_index > ending_index):
-            return "Index Reached Ending Index"
-        excluding_rows = []
-        if exclusion_index != "":
-            if "," in exclusion_index:
-                exclusion_index = exclusion_index.split(",")
-                for item in exclusion_index:
-                    excluding_rows.extend(_get_excluding_row(item))
-            else:
-                excluding_rows = _get_excluding_row(exclusion_index)
-        for item in excluding_rows:
-            if (int(item) > ending_index) or int(item) > len(item_list):
-                print("exclusion index greater than ending index")
-                break
-            item_list.remove(item)
-        return item_list[current_index]
-    except IndexError:
-        return "Index Error"
-
-# This is an internal function. Not meant to be used directly
-def _get_excluding_row(exclusion_index: str):
-    if "-" in exclusion_index:
-        exclusion_index = exclusion_index.split("-")
-        return [
-            str(num)
-            for num in range(int(exclusion_index[0]), int(exclusion_index[1]) + 1)
-        ]
-    else:
-        return [(exclusion_index)]
-
-
-# ===========================================================#
-# Functions related to changing printjob forms genereated by
-# label editing softwares so the label can be easily designed
-# in other editing software and Ox Script can be used to update
-# the data on the label
-# ===========================================================#
-
-basepath = ""
-
-def get_all_form_variables(filepath) -> dict:
-    """
-    get_all_form_variables is used to retrive all the variables in the form so they can be
-        updated with the update_all_form_variables function.
-
-    Parameters:
-        filepath (string): The path to the form file. The form file can be generated by
-            label editing softwares and just place the form file next to the script so
-            the relative path can be accessed
-
-    Returns:
-        dict: A dictionary of the positions of the variables are in the form so that it can be
-            used to update the variables in the form
-    """
-    variable_locations = {}
-    if os.access(filepath, os.F_OK):
-        with open(filepath, "r") as fp:
-            # read all lines using readline()
-            lines = fp.readlines()
-            for line in lines:
-                # check if string present on a current line
-                word = "#OX:"
-                if line.find(word) != -1:
-                    for item in reversed(line.split(",")):
-                        if item.find(word) != -1:
-                            key = item
-                            item = item.replace(word, "")
-                            item = item.replace('"', "")
-                            item = item.replace("#\n", "")
-                            if item not in variable_locations.keys():
-                                variable_locations[item] = [
-                                    {
-                                        "position": lines.index(line),
-                                        "line": line,
-                                        "replacement_key": key,
-                                    },
-                                ]
-                            elif item in variable_locations.keys():
-                                variable_locations[item].append(
-                                    {
-                                        "position": lines.index(line),
-                                        "line": line,
-                                        "replacement_key": key,
-                                    }
-                                )
-        return variable_locations
-
-def update_all_form_variables(filename, **kwargs) -> str:
-    """
-    update_all_form_variables is used to update all the variables in the form
-
-    Parameters:
-        filename (string): The name of the form file. The form file can be generaed by
-            label editing softwares and just place the form file next to the script so
-            the relative path can be accessed
-        **kwargs: The key value pair of the variables to be updated
-    
-    e.x.:
-        cmd = update_all_form_variables(
-                'command1.txt',
-                Input1=data[0],
-                Input2=data[1],
-            )
-        PTK_SendCmdToPrinter(cmd)
-        where 'command1.txt' is the form file name and 'Input1' and 'Input2' are the variables
-            name defined when the form file is generated
-
-    Returns:
-        str: The updated form file in string that can be sent to the printer through the function
-            PTK_SendCmdToPrinter
-    """
-    filepath = basepath + filename
-    if os.access(filepath, os.F_OK):
-        variable_locations = get_all_form_variables(filepath)
-        with open(filepath, "r") as text_file:
-            lines = [line for line in text_file]
-            for key, value in kwargs.items():
-                if key in variable_locations.keys():
-                    for items in variable_locations[key]:
-                        position = items["position"]
-                        line = items["line"]
-                        line = line.replace(
-                            items["replacement_key"], '"' + value + '"')
-                        lines[position] = line + "\n"
-            return "".join(lines) + "\r\n"
-    else:
-        debuglog("Form file specified does not exist")
-        return ""
+    return {}
```

### Comparing `ox_script-0.3.0/ox_script.egg-info/PKG-INFO` & `ox_script-0.3.2/ox_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox-script
-Version: 0.3.0
+Version: 0.3.2
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Postek Electronics Co., Ltd.
 Author-email: support@postek.com.cn
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox_script-0.3.0/setup.py` & `ox_script-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ox_script',
-    version='0.3.0',
+    version='0.3.2',
     author='Postek Electronics Co., Ltd.',
     author_email='support@postek.com.cn',
     packages=find_packages(),
     license="MIT",
     description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
     url="https://github.com/POSTEK-OX-Script",
     install_requires=[
```

