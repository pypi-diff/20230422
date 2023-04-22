# Comparing `tmp/pyrobox-0.7.3.tar.gz` & `tmp/pyrobox-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrobox-0.7.3.tar", last modified: Fri Mar 17 13:37:53 2023, max compression
+gzip compressed data, was "pyrobox-0.7.4.tar", last modified: Sat Apr 22 19:18:07 2023, max compression
```

## Comparing `pyrobox-0.7.3.tar` & `pyrobox-0.7.4.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 13:37:53.704895 pyrobox-0.7.3/
--rw-rw-rw-   0        0        0     1062 2023-02-14 13:46:56.000000 pyrobox-0.7.3/LICENSE
--rw-rw-rw-   0        0        0     8509 2023-03-17 13:37:53.704895 pyrobox-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     7322 2023-03-17 13:34:15.000000 pyrobox-0.7.3/README.md
--rw-rw-rw-   0        0        0       90 2023-02-07 11:48:14.000000 pyrobox-0.7.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-17 13:37:53.684068 pyrobox-0.7.3/pyrobox.egg-info/
--rw-rw-rw-   0        0        0     8509 2023-03-17 13:37:53.000000 pyrobox-0.7.3/pyrobox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-03-17 13:37:53.000000 pyrobox-0.7.3/pyrobox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 13:37:53.000000 pyrobox-0.7.3/pyrobox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-17 13:37:53.000000 pyrobox-0.7.3/pyrobox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-03-17 13:37:53.000000 pyrobox-0.7.3/pyrobox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-17 13:37:53.000000 pyrobox-0.7.3/pyrobox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1027 2023-03-17 13:37:53.705895 pyrobox-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-03-04 18:36:13.000000 pyrobox-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-17 13:37:53.703903 pyrobox-0.7.3/src/
--rw-rw-rw-   0        0        0       83 2023-03-04 18:36:13.000000 pyrobox-0.7.3/src/__init__.py
--rw-rw-rw-   0        0        0       20 2023-03-04 18:36:13.000000 pyrobox-0.7.3/src/__main__.py
--rw-rw-rw-   0        0        0    45806 2023-03-17 13:34:29.000000 pyrobox-0.7.3/src/pyroboxCore.py
--rw-rw-rw-   0        0        0    81999 2023-03-17 13:34:29.000000 pyrobox-0.7.3/src/server.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:18:07.409946 pyrobox-0.7.4/
+-rw-rw-rw-   0        0        0     1062 2023-02-14 13:46:56.000000 pyrobox-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0    10271 2023-04-22 19:18:07.409946 pyrobox-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9052 2023-04-19 11:03:38.000000 pyrobox-0.7.4/README.md
+-rw-rw-rw-   0        0        0       90 2023-02-07 11:48:14.000000 pyrobox-0.7.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-22 19:18:07.400945 pyrobox-0.7.4/pyrobox.egg-info/
+-rw-rw-rw-   0        0        0    10271 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 19:18:07.000000 pyrobox-0.7.4/pyrobox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1027 2023-04-22 19:18:07.410945 pyrobox-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-03-04 18:36:13.000000 pyrobox-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 19:18:07.408945 pyrobox-0.7.4/src/
+-rw-rw-rw-   0        0        0       83 2023-03-04 18:36:13.000000 pyrobox-0.7.4/src/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-03-04 18:36:13.000000 pyrobox-0.7.4/src/__main__.py
+-rw-rw-rw-   0        0        0     1812 2023-04-19 10:26:44.000000 pyrobox-0.7.4/src/arg_parser.py
+-rw-rw-rw-   0        0        0      105 2023-04-22 14:53:09.000000 pyrobox-0.7.4/src/exceptions.py
+-rw-rw-rw-   0        0        0     8154 2023-04-22 18:54:58.000000 pyrobox-0.7.4/src/fs_utils.py
+-rw-rw-rw-   0        0        0    44164 2023-04-22 18:52:10.000000 pyrobox-0.7.4/src/page_templates.py
+-rw-rw-rw-   0        0        0    46390 2023-04-22 18:57:57.000000 pyrobox-0.7.4/src/pyroboxCore.py
+-rw-rw-rw-   0        0        0    32518 2023-04-22 19:14:09.000000 pyrobox-0.7.4/src/server.py
+-rw-rw-rw-   0        0        0     2191 2023-02-07 11:48:14.000000 pyrobox-0.7.4/src/zipfly_local.py
```

### Comparing `pyrobox-0.7.3/LICENSE` & `pyrobox-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrobox-0.7.3/PKG-INFO` & `pyrobox-0.7.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,188 +1,197 @@
-Metadata-Version: 2.1
-Name: pyrobox
-Version: 0.7.3
-Summary: Personal DropBox for Private Network
-Home-page: https://github.com/RaSan147/pyrobox
-Author-email: wwwqweasd147@gmail.com
-Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
-Project-URL: Documentation, https://github.com/RaSan147/pyrobox
-Project-URL: Source Code, https://github.com/RaSan147/pyrobox
-Project-URL: Release Notes, https://github.com/RaSan147/pyrobox/releases
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
-Classifier: Topic :: Communications :: File Sharing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyrobox 🔥
-
-**`Note :`** DEFAULT UPLOAD PASSWORD: `SECret`
-* you can change it by editing the code (see `config` class at top)
-* to set password from command line, use `-k` or `--password` flag
-
-# Status 
-[![Downloads](https://static.pepy.tech/badge/pyrobox)](https://pepy.tech/project/pyrobox)
-
-
-# Requesting for more suggesions and ideas
-
-Basic FEATURES
-----------------------------------------------------------------
-* File Hosting system (Serve files from local Storage system)
-* Access Shared File System from Multiple Devices
-
- Extra FEATURES 
-----------------------------------------------------------------
-* 🔽 DOWNLOAD AND VIDEO STREAM WITH **PAUSE AND RESUME**
-* 🔼 UPLOAD WITH **PASSWORD**
-* 👌 HTML5 drag and drop uploader
-* 📈 MULTIPLE FILE **UPLOAD**
-* 📝 RENAME
-* 📁 FOLDER DOWNLOAD as **ZIP** (uses temp folder)
-* ⏯ VIDEO PLAYER
-* 🔁 **DELETE FILE** (MOVE TO RECYCLE BIN)
-* 🔥 PERMANENTLY DELETE
-* ⛓ `File manager` like `NAVIGATION BAR`
-* 📑 Right click Context menu (Tap n hold on touch device)
-* 🧨 RELOAD SERVER FROM REMOTE [DEBUG PURPOSE]
-* 🆕 FOLDER CREATION
-* 💬 Pop-up messages UI(from my Web leach repo)
-* 🌐 (Didn't test yet) If you are using REAL IP AND ALLOW PYTHON TO USE PUBLIC NETWORK, YOUR SERVER CAN BE VISIBLE AROUND THE GLOBE. (also vulnerable, since you can't control access *yet*)
-* 🧬 Clone entire directory from Host to Client with least changes (last modified preserved)
-* 🔜 More comming soon
-
-
-Server side requirement
-----------------------------------------------------------------
-* Python 3.7 or higher. Older support available.[^1]
-* Basic knowledge about Python
-* `send2trash`, `natsort` pip package (if missing, will be auto installed when the code runs)
-
-[^1]: [<=3.4 compat] is on the way.
-
-
-# Installation
-----------------------------------------------------------------
-  * **Install Python 3.7 or higher**
-  * **Close older pyrobox process if already running**
-  1. Install using PIP
-  ### On Windows:
-  * Open `CMD` or `PowerShell`
-  * Run `pip install pyrobox`
-  * Run `pyrobox` to launch the server
-
-  ### On Linux:
-  * Open `Terminal`
-  * Run `pip3 install pyrobox`
-  * Run `pyrobox` to launch the server
-
-
-CHECK [FAQ](#faq) FOR FUTURE HELP AND ISSUE FIX
-
-
-# Customization
-1. Simply running the code on will create a server on `CURRENT WORKING DIRECTORY` on `Port: 6969`
-1. On browser (on device under same router/wifi network), go to `deviceIP:port_number` to see the output like this: `http://192.168.0.101:6969/`
-    * you must allow python in firewall to access network, check [FAQ](#faq) for more help
-1. To change the server running directory, 
-   - i) either edit the code  (see `config` class at top)
-   - ii) or add `-d` or `--directory` command line argument when launching the program
-        - `pyrobox -d .` to launch the server in current directory (where the file is)
-        - `pyrobox -d "D:\Server\Public folder\"`  (Use Double-Quotation while directory has space)
-        - `pyrobox -d "D:/Server/Public folder"` (Forward or backward slash really doesn't matter, unless your terminal thinks otherwise)
- 1. To change port number
-    - i) just edit the code for permanent change  (see `config` class at top)
-    - ii) or add the port number at the end of the command line arg  
-       -  `pyrobox 45678` # will run on port 45678
-       -  `pyrobox -d . 45678` # will run on port 45678 in current directory
-
-1. To specify alternate bind address
-    - Add bind add `-bind {address}` # ie: `-bind 127.0.0.2` or `-bind 127.0.0.99`
-
-1. To change upload password
-    - i) or add `-k` or `--password` command line argument when launching the program
-        - `pyrobox -k "my new password"` to launch the server with new password
-        - `pyrobox -k ""` to launch the server without password
-        - `pyrobox` to launch the server with default password (SECret)
-    - ii) just edit the code for permanent change  (see `config` class at top)
-
- TODO:
---------------------------------------------------------------
-
-* https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
-* https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
-* https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
-* check output ip and port accuracy on multiple os  
-* https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
-* https://github.com/RaSan147/pyrobox/issues/39 User login and user based permission set. 🔑
-
-# Support for more features
-
-
-Context menu:
---------------------------------------------------------------
-  **Right click on any file link**
-  <img src="https://user-images.githubusercontent.com/34002411/174422718-e19d33b2-4937-47d7-bcc2-610141c1e437.jpg" width=200>
-
-# FAQ:
-<details>
-  <summary>Using WSL, "PIP not found"</summary>
- 
-  > Run this to install `pip3` and add `pip` to path 
-  ```
-  sudo apt -y purge python3-pip
-  sudo python3 -m pip uninstall pip
-  sudo apt -y install python3-pip
-  pip3 install --upgrade pip
-  echo "export PATH=\"${HOME}/.local/bin:$PATH\"" >>"${HOME}"/.bashrc
-  ```
-  > Re-running the file should work.
-</details>
-
-<details>
-  <summary>Using Linux, "PIP not found"</summary>
-  
-  > Run this to install `pip3` 
-  ```
-  sudo apt -y purge python3-pip
-  sudo python3 -m pip uninstall pip
-  sudo apt -y install python3-pip
-  pip3 install --upgrade pip
-  ```
-  > Re-running the file should work.
-</details>
-
-
-<details>
-  <summary>Deleted (Move to Recycle), But WHERE ARE THEY?? [on LINUX & WSL]</summary>
-  
-  > Actually the feature is working fine, unfortunately NO-GUI mode linux and WSL don't recycle bin, so you can't find it!
-  > And to make things worse, **you need to manually clear the recyle bin** from `~/.local/share/Trash`
-  > **SO I'D RECOMMAND USING DELETE PARMANENTLY**
-</details>
-
-<details>
-  <summary>Running on WINDOWS, but can't access with other device [FIREWALL]</summary>
- 
-  > You probably have **FireWall ON** and Unconfigured.
-  > For your safety, I'd recommand you to allow Python on private network and run the server when your network is Private.
-  > IN SHORT: ALLOW PYTHON ON FIREWALL, RUN THE SERVER
- 
-  > *note: allowed on private but using public network on firewall will cause similar issue, you gotta make both same or allow python both on public and private*
-</details>
-
-# Thanks to:
-1. https://github.com/bones7456/bones7456/blob/master/SimpleHTTPServerWithUpload.py (the guy who made upload possible)
-2. https://gist.github.com/UniIsland/3346170 (the guy who made multiple file upload possible)
-3. https://github.com/SethMMorton/natsort (sorting titles)
-4. https://github.com/sandes/zipfly (*modified* lets you see the zip progress)
-5. https://github.com/sampotts/plyr (*improved* video player)
-
-***Disclaimer***: *the owner or the programmers or any content of this repository hold no responsibility for any kind of data loss or modification on your system and do not warrenty for such actions. I tried my best to prevent all sorts of ways (that I am currently aware of) to prevent data loss or unwanted data modification. See [Data Safety Measures](/DATA%20SAFETY.MD) taken on this projects to prevent unwanted data loss.*
+# pyrobox 🔥
+
+**`Note :`** DEFAULT UPLOAD PASSWORD: `SECret`
+* you can change it by editing the code (see `config` class at top)
+* to set password from command line, use `-k` or `--password` flag
+
+# Status 
+[![Downloads](https://static.pepy.tech/badge/pyrobox)](https://pepy.tech/project/pyrobox)
+
+
+# Requesting for more suggesions and ideas
+
+Basic FEATURES
+----------------------------------------------------------------
+* File Hosting system (Serve files from local Storage system)
+* Access Shared File System from Multiple Devices
+
+ Extra FEATURES 
+----------------------------------------------------------------
+* 🔽 DOWNLOAD AND VIDEO STREAM WITH **PAUSE AND RESUME**
+* 🔼 UPLOAD WITH **PASSWORD**
+* 👌 HTML5 drag and drop uploader
+* 📈 MULTIPLE FILE **UPLOAD**
+* 📝 RENAME
+* 📁 FOLDER DOWNLOAD as **ZIP** (uses temp folder)
+* ⏯ VIDEO PLAYER
+* 🔁 **DELETE FILE** (MOVE TO RECYCLE BIN)
+* 🔥 PERMANENTLY DELETE
+* ⛓ `File manager` like `NAVIGATION BAR`
+* 📑 Right click Context menu (Tap n hold on touch device)
+* 🧨 RELOAD SERVER FROM REMOTE [DEBUG PURPOSE]
+* 🆕 FOLDER CREATION
+* 💬 Pop-up messages UI(from my Web leach repo)
+* 🌐 (Didn't test yet) If you are using REAL IP AND ALLOW PYTHON TO USE PUBLIC NETWORK, YOUR SERVER CAN BE VISIBLE AROUND THE GLOBE. (also vulnerable, since you can't control access *yet*)
+* 🧬 Clone entire directory from Host to Client with least changes (last modified preserved)
+* 🔜 More comming soon
+
+
+Server side requirement
+----------------------------------------------------------------
+* Python 3.7 or higher. Older support available.[^1]
+* Basic knowledge about Python
+* `send2trash`, `natsort` pip package (if missing, will be auto installed when the code runs)
+
+[^1]: [<=3.4 compat] is on the way.
+
+
+# Installation
+----------------------------------------------------------------
+  * **Install Python 3.7 or higher**
+  * **Close older pyrobox process if already running**
+  1. Install using PIP
+  ### On Windows:
+  * Open `CMD` or `PowerShell`
+  * Run `pip install pyrobox`
+  * Run `pyrobox` to launch the server
+
+  ### On Linux:
+  * Open `Terminal`
+  * Run `pip3 install pyrobox`
+  * Run `pyrobox` to launch the server
+
+
+CHECK [FAQ](#faq) FOR FUTURE HELP AND ISSUE FIX
+
+
+# Customization
+1. Simply running the code on will create a server on `CURRENT WORKING DIRECTORY` on `Port: 6969`
+1. On browser (on device under same router/wifi network), go to `deviceIP:port_number` to see the output like this: `http://192.168.0.101:6969/`
+    * you must allow python in firewall to access network, check [FAQ](#faq) for more help
+1. To change the server running directory, 
+   - i) either edit the code  (see `config` class at top)
+   - ii) or add `-d` or `--directory` command line argument when launching the program
+        - `pyrobox -d .` to launch the server in current directory (where the file is)
+        - `pyrobox -d "D:\Server\Public folder\"`  (Use Double-Quotation while directory has space)
+        - `pyrobox -d "D:/Server/Public folder"` (Forward or backward slash really doesn't matter, unless your terminal thinks otherwise)
+ 1. To change port number
+    - i) just edit the code for permanent change  (see `config` class at top)
+    - ii) or add the port number at the end of the command line arg  
+       -  `pyrobox 45678` # will run on port 45678
+       -  `pyrobox -d . 45678` # will run on port 45678 in current directory
+
+1. To specify alternate bind address
+    - Add bind add `-bind {address}` # ie: `-bind 127.0.0.2` or `-bind 127.0.0.99`
+
+1. To change upload password
+    - i) or add `-k` or `--password` command line argument when launching the program
+        - `pyrobox -k "my new password"` to launch the server with new password
+        - `pyrobox -k ""` to launch the server without password
+        - `pyrobox` to launch the server with default password (SECret)
+    - ii) just edit the code for permanent change  (see `config` class at top)
+
+1. Optional configurations
+
+usage: `local_server_pyrobox.py [--password PASSWORD] [--no-upload] [--no-zip] [--no-update] [--no-delete] [--no-download] [--read-only] [--view-only] [--bind ADDRESS] [--directory DIRECTORY] [--version] [-h] [port]`
+
+# positional arguments:
+  | arg value             | Description |
+  | --------------------- | ------------|
+  | `port`                | Specify alternate port [default: 6969] |
+
+
+# options:
+  | arg `value`           | Description |
+  | --------------------- | ------------|
+  |--password `PASSWORD`, -k  `PASSWORD` | Upload Password (default: SECret)|
+  |--directory `DIRECTORY`, -d `DIRECTORY` | Specify alternative directory [default: current directory]
+  |--bind `ADDRESS`, -b `ADDRESS` | Specify alternate bind address [default: all interfaces]|
+
+
+# Customisation options:
+  | arg                  | Description |
+  | -------------------- | ------------|
+  |--no-upload, -nu      | Files can't be uploaded (default: False)|
+  |--no-zip, -nz         | Disable Folder->Zip downloading (default: False)|
+  |--no-update, -no      | Disable File Updating (ie: **renaming**, **overwriting existing files**) (On upload, if file exists, will add a number at the end(default: False)|
+  |--no-delete, -nd      | Disable File Deletion (default: False)|
+  |--no-download, -ndw   | Disable File Downloading [**videos won't play either**] (default: False)|
+  |--read-only, -ro      | Read Only Mode *disables upload and any modifications ie: rename, delete* (default: False)|
+  |--view-only, -vo      | Only allowed to see file list, nothing else (default: False)|
+  --version, -v          | show program's version number and exit|
+  -h, --help             | show this help message and exit|
+
+
+ TODO:
+--------------------------------------------------------------
+
+* https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
+* https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
+* https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
+* check output ip and port accuracy on multiple os  
+* https://github.com/RaSan147/pyrobox/issues/37 Backup code if Reload causes unhandled issue and can't be accessed
+* https://github.com/RaSan147/pyrobox/issues/39 User login and user based permission set. 🔑
+
+# Support for more features
+
+
+Context menu:
+--------------------------------------------------------------
+  **Right click on any file link**
+  <img src="https://user-images.githubusercontent.com/34002411/174422718-e19d33b2-4937-47d7-bcc2-610141c1e437.jpg" width=200>
+
+# FAQ:
+<details>
+  <summary>Using WSL, "PIP not found"</summary>
+ 
+  > Run this to install `pip3` and add `pip` to path 
+  ```
+  sudo apt -y purge python3-pip
+  sudo python3 -m pip uninstall pip
+  sudo apt -y install python3-pip
+  pip3 install --upgrade pip
+  echo "export PATH=\"${HOME}/.local/bin:$PATH\"" >>"${HOME}"/.bashrc
+  ```
+  > Re-running the file should work.
+</details>
+
+<details>
+  <summary>Using Linux, "PIP not found"</summary>
+  
+  > Run this to install `pip3` 
+  ```
+  sudo apt -y purge python3-pip
+  sudo python3 -m pip uninstall pip
+  sudo apt -y install python3-pip
+  pip3 install --upgrade pip
+  ```
+  > Re-running the file should work.
+</details>
+
+
+<details>
+  <summary>Deleted (Move to Recycle), But WHERE ARE THEY?? [on LINUX & WSL]</summary>
+  
+  > Actually the feature is working fine, unfortunately NO-GUI mode linux and WSL don't recycle bin, so you can't find it!
+  > And to make things worse, **you need to manually clear the recyle bin** from `~/.local/share/Trash`
+  > **SO I'D RECOMMAND USING DELETE PARMANENTLY**
+</details>
+
+<details>
+  <summary>Running on WINDOWS, but can't access with other device [FIREWALL]</summary>
+ 
+  > You probably have **FireWall ON** and Unconfigured.
+  > For your safety, I'd recommand you to allow Python on private network and run the server when your network is Private.
+  > IN SHORT: ALLOW PYTHON ON FIREWALL, RUN THE SERVER
+ 
+  > *note: allowed on private but using public network on firewall will cause similar issue, you gotta make both same or allow python both on public and private*
+</details>
+
+# Thanks to:
+1. https://github.com/bones7456/bones7456/blob/master/SimpleHTTPServerWithUpload.py (the guy who made upload possible)
+2. https://gist.github.com/UniIsland/3346170 (the guy who made multiple file upload possible)
+3. https://github.com/SethMMorton/natsort (sorting titles)
+4. https://github.com/sandes/zipfly (*modified* lets you see the zip progress)
+5. https://github.com/sampotts/plyr (*improved* video player)
+
+***Disclaimer***: *the owner or the programmers or any content of this repository hold no responsibility for any kind of data loss or modification on your system and do not warrenty for such actions. I tried my best to prevent all sorts of ways (that I am currently aware of) to prevent data loss or unwanted data modification. See [Data Safety Measures](/DATA%20SAFETY.MD) taken on this projects to prevent unwanted data loss.*
```

### Comparing `pyrobox-0.7.3/pyrobox.egg-info/PKG-INFO` & `pyrobox-0.7.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrobox
-Version: 0.7.3
+Version: 0.7.4
 Summary: Personal DropBox for Private Network
 Home-page: https://github.com/RaSan147/pyrobox
 Author-email: wwwqweasd147@gmail.com
 Project-URL: Bug Tracker, https://github.com/RaSan147/pyrobox/issues
 Project-URL: Documentation, https://github.com/RaSan147/pyrobox
 Project-URL: Source Code, https://github.com/RaSan147/pyrobox
 Project-URL: Release Notes, https://github.com/RaSan147/pyrobox/releases
@@ -109,14 +109,46 @@
 1. To change upload password
     - i) or add `-k` or `--password` command line argument when launching the program
         - `pyrobox -k "my new password"` to launch the server with new password
         - `pyrobox -k ""` to launch the server without password
         - `pyrobox` to launch the server with default password (SECret)
     - ii) just edit the code for permanent change  (see `config` class at top)
 
+1. Optional configurations
+
+usage: `local_server_pyrobox.py [--password PASSWORD] [--no-upload] [--no-zip] [--no-update] [--no-delete] [--no-download] [--read-only] [--view-only] [--bind ADDRESS] [--directory DIRECTORY] [--version] [-h] [port]`
+
+# positional arguments:
+  | arg value             | Description |
+  | --------------------- | ------------|
+  | `port`                | Specify alternate port [default: 6969] |
+
+
+# options:
+  | arg `value`           | Description |
+  | --------------------- | ------------|
+  |--password `PASSWORD`, -k  `PASSWORD` | Upload Password (default: SECret)|
+  |--directory `DIRECTORY`, -d `DIRECTORY` | Specify alternative directory [default: current directory]
+  |--bind `ADDRESS`, -b `ADDRESS` | Specify alternate bind address [default: all interfaces]|
+
+
+# Customisation options:
+  | arg                  | Description |
+  | -------------------- | ------------|
+  |--no-upload, -nu      | Files can't be uploaded (default: False)|
+  |--no-zip, -nz         | Disable Folder->Zip downloading (default: False)|
+  |--no-update, -no      | Disable File Updating (ie: **renaming**, **overwriting existing files**) (On upload, if file exists, will add a number at the end(default: False)|
+  |--no-delete, -nd      | Disable File Deletion (default: False)|
+  |--no-download, -ndw   | Disable File Downloading [**videos won't play either**] (default: False)|
+  |--read-only, -ro      | Read Only Mode *disables upload and any modifications ie: rename, delete* (default: False)|
+  |--view-only, -vo      | Only allowed to see file list, nothing else (default: False)|
+  --version, -v          | show program's version number and exit|
+  -h, --help             | show this help message and exit|
+
+
  TODO:
 --------------------------------------------------------------
 
 * https://github.com/RaSan147/pyrobox/issues/33 Show thumbnails, for png and jpg (how to do with just standard library?), For others, just show extension.
 * https://github.com/RaSan147/pyrobox/issues/34 Copy stream URL for videos to play with any video player
 * https://github.com/RaSan147/pyrobox/issues/36 Add side bar to do something 🤔
 * check output ip and port accuracy on multiple os
```

### Comparing `pyrobox-0.7.3/setup.cfg` & `pyrobox-0.7.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7972 6f62 6f78 0d0a 7665 7273   = pyrobox..vers
-00000020: 696f 6e20 3d20 302e 372e 330d 0a61 7574  ion = 0.7.3..aut
+00000020: 696f 6e20 3d20 302e 372e 340d 0a61 7574  ion = 0.7.4..aut
 00000030: 686f 7273 203d 2052 6173 616e 0d0a 6175  hors = Rasan..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 2077 7777  thor_email = www
 00000050: 7177 6561 7364 3134 3740 676d 6169 6c2e  qweasd147@gmail.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 2050 6572 736f 6e61 6c20 4472 6f70   = Personal Drop
 00000080: 426f 7820 666f 7220 5072 6976 6174 6520  Box for Private 
 00000090: 4e65 7477 6f72 6b0d 0a6c 6f6e 675f 6465  Network..long_de
```

### Comparing `pyrobox-0.7.3/src/pyroboxCore.py` & `pyrobox-0.7.4/src/pyroboxCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-__version__ = "0.7.3"
+__version__ = "0.7.4"
 enc = "utf-8"
 __all__ = [
 	"HTTPServer", "ThreadingHTTPServer", "BaseHTTPRequestHandler",
 	"SimpleHTTPRequestHandler",
 
 ]
 
 import os
 import atexit
 import logging
 from queue import Queue
 from typing import Union
+from string import Template
 
 import argparse
 
 
 logging.basicConfig(level=logging.INFO, format='%(levelname)s: \n%(message)s')
 
 logger = logging.getLogger(__name__)
@@ -83,15 +84,40 @@
 
 
 		# ASSET MAPPING
 		self.file_list = {}
 
 		# COMMANDLINE ARGUMENTS PARSER
 		self.parser = argparse.ArgumentParser(add_help=False)
-		
+
+
+
+
+		# Default error message template
+		self.DEFAULT_ERROR_MESSAGE = Template("""
+		<!DOCTYPE HTML>
+		<html lang="en">
+		<html>
+			<head>
+				<meta charset="utf-8">
+				<title>Error response</title>
+			</head>
+			<body>
+				<h1>Error response</h1>
+				<p>Error code: ${code}</p>
+				<p>Message: ${message}</p>
+				<p>Error code explanation: ${code} - ${explain}</p>
+				<h3>PyroBox Version: ${version}</h3>
+			</body>
+		</html>
+		""")
+
+		self.DEFAULT_ERROR_CONTENT_TYPE = "text/html;charset=utf-8"
+
+
 
 	def clear_temp(self):
 		for i in self.temp_file:
 			try:
 				os.remove(i)
 			except:
 				pass
@@ -111,48 +137,48 @@
 
 	def get_default_dir(self):
 		return './'
 
 
 	def address(self):
 		return "http://%s:%i"%(self.IP, self.port)
-	
+
 	def parse_default_args(self, port = None, directory = None, bind = None, ):
 		if port is None:
 			port = self.port
 		if directory is None:
 			directory = self.ftp_dir
 		if bind is None:
 			bind = None
 
 		parser = self.parser
 
-		parser.add_argument('--bind', '-b', 
+		parser.add_argument('--bind', '-b',
 							metavar='ADDRESS', default=bind,
 							help='Specify alternate bind address '
 								'[default: all interfaces]')
 		parser.add_argument('--directory', '-d', default=directory,
 							help='Specify alternative directory '
 							'[default: current directory]')
 		parser.add_argument('port', action='store',
 							default=port, type=int,
 							nargs='?',
-							help='Specify alternate port [default: 8000]')
+							help=f'Specify alternate port [default: {port}]')
 		parser.add_argument('--version', '-v', action='version',
 							version=__version__)
-		
+
 		self.parser.add_argument('-h', '--help', action='help',
-								default='==SUPPRESS==', 
+								default='==SUPPRESS==',
 								help=('show this help message and exit'))
-		
+
 		args = parser.parse_known_args()[0]
 
 		return args
-	
-		
+
+
 
 
 
 
 
 
 
@@ -380,35 +406,14 @@
 
 	dict_result = Callable_dict(urllib.parse.parse_qs(parse_result.query, keep_blank_values=True))
 
 	return (parse_result.path, dict_result, parse_result.fragment)
 
 
 
-# Default error message template
-DEFAULT_ERROR_MESSAGE = """
-<!DOCTYPE HTML>
-<html lang="en">
-<html>
-	<head>
-		<meta charset="utf-8">
-		<title>Error response</title>
-	</head>
-	<body>
-		<h1>Error response</h1>
-		<p>Error code: %(code)d</p>
-		<p>Message: %(message)s.</p>
-		<p>Error code explanation: %(code)s - %(explain)s.</p>
-		<h3>PyroBox Version: %(version)s
-	</body>
-</html>
-"""
-
-DEFAULT_ERROR_CONTENT_TYPE = "text/html;charset=utf-8"
-
 class HTTPServer(socketserver.TCPServer):
 
 	allow_reuse_address = True	# Seems to make sense in testing environment
 
 	def server_bind(self):
 		"""Override server_bind to store the server name."""
 		socketserver.TCPServer.server_bind(self)
@@ -459,16 +464,14 @@
 	sys_version = "Python/" + sys.version.split()[0]
 
 	# The server software version.  You may want to override this.
 	# The format is multiple whitespace-separated strings,
 	# where each string is of the form name[/version].
 	server_version = "BaseHTTP/" + __version__
 
-	error_message_format = DEFAULT_ERROR_MESSAGE
-	error_content_type = DEFAULT_ERROR_CONTENT_TYPE
 
 	# The default request version.  This only affects responses up until
 	# the point where the request line is parsed, so it mainly decides what
 	# the client gets back when sending a malformed request line.
 	# Most web servers default to HTTP 0.9, i.e. don't send a status line.
 	default_request_version = "HTTP/0.9"
 
@@ -637,15 +640,15 @@
 
 			_hash = abs(hash((self.raw_requestline, tools.random_string(10))))
 			self.req_hash = base64.b64encode(str(_hash).encode('ascii')).decode()[:10]
 
 			_w = tools.term_width()
 			w = _w - len(str(self.req_hash)) -2
 			w = w//2
-			logger.info('='*w + f' {self.req_hash} ' + '='*w + '\n'+ 
+			logger.info('='*w + f' {self.req_hash} ' + '='*w + '\n'+
 					'\n'.join(
 						[f'{self.req_hash}|=>\t request\t: {self.command}',
 						f'{self.req_hash}|=>\t url     \t: {url_path}',
 						f'{self.req_hash}|=>\t query   \t: {query}',
 						f'{self.req_hash}|=>\t fragment\t: {fragment}',
 						f'{self.req_hash}|=>\t full url \t: {self.path}',
 						]) + '\n'+
@@ -674,32 +677,45 @@
 		"""Handle multiple requests if necessary."""
 		self.close_connection = True
 
 		self.handle_one_request()
 		while not self.close_connection:
 			self.handle_one_request()
 
-	def send_error(self, code, message=None, explain=None):
+	def send_error(self, code, message=None, explain=None, error_message_format:Template=None):
 		"""Send and log an error reply.
 
 		Arguments are
 		* code:	an HTTP error code
 				   3 digits
 		* message: a simple optional 1 line reason phrase.
 				   *( HTAB / SP / VCHAR / %x80-FF )
 				   defaults to short entry matching the response code
 		* explain: a detailed message defaults to the long entry
 				   matching the response code.
+		* error_message_format: a `string.Template` for the error message
+				   defaults to `config.DEFAULT_ERROR_MESSAGE`
+
+				   auto-formatting values:
+						`${code}`: the HTTP error code
+						`${message}`: the HTTP error message
+						`${explain}`: the detailed error message
+						`${version}`: the server software version string
 
 		This sends an error response (so it must be called before any
 		output has been generated), logs the error, and finally sends
 		a piece of HTML explaining the error to the user.
 
 		"""
 
+
+		error_message_format = error_message_format if error_message_format else config.DEFAULT_ERROR_MESSAGE
+
+		error_content_type = config.DEFAULT_ERROR_CONTENT_TYPE
+
 		try:
 			shortmsg, longmsg = self.responses[code]
 		except KeyError:
 			shortmsg, longmsg = '???', '???'
 		if message is None:
 			message = shortmsg
 		if explain is None:
@@ -714,22 +730,22 @@
 		body = None
 		if (code >= 200 and
 			code not in (HTTPStatus.NO_CONTENT,
 						 HTTPStatus.RESET_CONTENT,
 						 HTTPStatus.NOT_MODIFIED)):
 			# HTML encode to prevent Cross Site Scripting attacks
 			# (see bug #1100201)
-			content = (self.error_message_format % {
-				'code': code,
-				'message': html.escape(message, quote=False),
-				'explain': html.escape(explain, quote=False),
-				'version': __version__
-			})
+			content = (error_message_format.safe_substitute(
+				code= code,
+				message= html.escape(message, quote=False),
+				explain= html.escape(explain, quote=False),
+				version= __version__
+			))
 			body = content.encode('UTF-8', 'replace')
-			self.send_header("Content-Type", self.error_content_type)
+			self.send_header("Content-Type", error_content_type)
 			self.send_header('Content-Length', str(len(body)))
 		self.end_headers()
 
 		if self.command != 'HEAD' and body:
 			self.wfile.write(body)
 
 	def send_response(self, code, message=None):
@@ -1241,15 +1257,15 @@
 
 
 		except Exception:
 			traceback.print_exc()
 
 			# if f and not f.closed(): f.close()
 			raise
-			
+
 	def send_file(self, path, filename=None, download=False):
 		'''sends the head and file to client'''
 		f = self.return_file(path, filename, download)
 		if self.command == "HEAD":
 			return # to avoid sending file on get request
 		try:
 			self.copyfile(f, self.wfile)
@@ -1459,15 +1475,15 @@
 	def get(self, show=F, strip=F, Timeout=20):
 		"""
 		show: print line
 		strip: strip \r\n at end
 		Timeout: if having network issue on any side, will keep trying to get content until Timeout (in seconds)
 		"""
 		req = self.req
-		
+
 
 		for _ in range(Timeout*2):
 			line = req.rfile.readline()
 			if line:
 				break
 			time.sleep(.5)
 		else:
@@ -1531,15 +1547,15 @@
 		ends at boundary
 		verify_name: name of the field (str|bytes|None)
 		verify_msg: message to verify (str|bytes)
 		decode: decode the message
 		* if None, skip checking field name
 		* if `empty string`, field name must be empty too'''
 		decoded = False
-		
+
 		if isinstance(verify_name, bytes):
 			verify_name = verify_name.decode()
 
 		field_name = self.match_name(verify_name) # LINE 1 (field name)
 		# if not verified, raise PostError
 
 		self.skip() # LINE 2 (blank line)
@@ -1555,15 +1571,15 @@
 		if decode:
 			line = line.decode()
 			decoded = True
 		if verify_msg is not None:
 			if not decoded:
 				if isinstance(verify_msg, str):
 					verify_msg = verify_msg.encode()
-					
+
 			if line != verify_msg:
 				raise PostError(f"Invalid post request.\n Expected: {[verify_msg]}\n Got: {[line]}")
 
 		# self.pass_bound() # LINE 5 (boundary)
 
 		return field_name, line
 
@@ -1689,14 +1705,17 @@
 		logger.warning(config.ftp_dir, "not found!\nReseting directory to current directory")
 		directory = "."
 
 	handler_class = partial(handler,
 								directory=directory)
 
 	config.port = port
+	if port > 65535 or port < 0:
+		raise ValueError("Port must be between 0 and 65535")
+
 	config.ftp_dir = directory
 
 	if not config.reload:
 		if sys.version_info>(3,8):
 			test(
 			HandlerClass=handler_class,
 			ServerClass=DualStackServer,
```

