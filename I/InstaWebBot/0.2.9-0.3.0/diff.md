# Comparing `tmp/InstaWebBot-0.2.9.tar.gz` & `tmp/InstaWebBot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InstaWebBot-0.2.9.tar", last modified: Thu Mar 16 16:30:24 2023, max compression
+gzip compressed data, was "InstaWebBot-0.3.0.tar", last modified: Fri Apr 21 22:43:07 2023, max compression
```

## Comparing `InstaWebBot-0.2.9.tar` & `InstaWebBot-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 16:30:24.810185 InstaWebBot-0.2.9/
-drwxrwxrwx   0        0        0        0 2023-03-16 16:30:24.539185 InstaWebBot-0.2.9/InstaWebBot/
--rw-rw-rw-   0        0        0    16486 2023-03-16 16:29:10.000000 InstaWebBot-0.2.9/InstaWebBot/Instabot.py
--rw-rw-rw-   0        0        0      248 2023-03-12 20:48:15.000000 InstaWebBot-0.2.9/InstaWebBot/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-16 16:29:10.000000 InstaWebBot-0.2.9/InstaWebBot/version.py
-drwxrwxrwx   0        0        0        0 2023-03-16 16:30:24.544185 InstaWebBot-0.2.9/InstaWebBot.egg-info/
--rw-rw-rw-   0        0        0     3856 2023-03-16 16:30:24.000000 InstaWebBot-0.2.9/InstaWebBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-03-16 16:30:24.000000 InstaWebBot-0.2.9/InstaWebBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 16:30:24.000000 InstaWebBot-0.2.9/InstaWebBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-16 16:30:24.000000 InstaWebBot-0.2.9/InstaWebBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-16 16:30:24.000000 InstaWebBot-0.2.9/InstaWebBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18431 2023-03-12 20:13:21.000000 InstaWebBot-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     3856 2023-03-16 16:30:24.808369 InstaWebBot-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     2979 2023-03-16 16:29:09.000000 InstaWebBot-0.2.9/README.md
--rw-rw-rw-   0        0        0       42 2023-03-16 16:30:24.813287 InstaWebBot-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-03-16 16:26:14.000000 InstaWebBot-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 22:43:05.893835 InstaWebBot-0.3.0/
+drwxrwxrwx   0        0        0        0 2023-04-21 22:43:05.371835 InstaWebBot-0.3.0/InstaWebBot/
+-rw-rw-rw-   0        0        0    16971 2023-04-21 22:36:58.000000 InstaWebBot-0.3.0/InstaWebBot/Instabot.py
+-rw-rw-rw-   0        0        0      248 2023-03-12 20:48:15.000000 InstaWebBot-0.3.0/InstaWebBot/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-04-21 20:53:25.000000 InstaWebBot-0.3.0/InstaWebBot/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 22:43:05.379835 InstaWebBot-0.3.0/InstaWebBot.egg-info/
+-rw-rw-rw-   0        0        0     4011 2023-04-21 22:43:05.000000 InstaWebBot-0.3.0/InstaWebBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-04-21 22:43:05.000000 InstaWebBot-0.3.0/InstaWebBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 22:43:05.000000 InstaWebBot-0.3.0/InstaWebBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 22:43:05.000000 InstaWebBot-0.3.0/InstaWebBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-21 22:43:05.000000 InstaWebBot-0.3.0/InstaWebBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18431 2023-03-12 20:13:21.000000 InstaWebBot-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4011 2023-04-21 22:43:05.889879 InstaWebBot-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3134 2023-04-21 20:52:42.000000 InstaWebBot-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 22:43:05.899295 InstaWebBot-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1293 2023-03-16 16:26:14.000000 InstaWebBot-0.3.0/setup.py
```

### Comparing `InstaWebBot-0.2.9/InstaWebBot/Instabot.py` & `InstaWebBot-0.3.0/InstaWebBot/Instabot.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     end_err: str = "\033[0m"
     print(f"{err}Warning: {message}{end_err}")
 
 
 def write(input_field, message: str) -> None:
     """Simulates user text input."""
     typing_time: float = 0.1
-    for word in message:
+    for word in message.split():
         if len(word) > 2:
             input_field.send_keys(word[:1])
             time.sleep(typing_time)
             input_field.send_keys(word[1:2])
             time.sleep(typing_time + random.random() / 3)
             input_field.send_keys(word[2:])
         else:
@@ -35,20 +35,25 @@
 
 class InstaBot:
     """A Class for an InstaBot that can execute some simple tasks."""
 
     def __init__(self, username: str, password: str, **kwargs) -> None:
         """Initializes an instance of an InstaBot."""
         self.__headless: bool = kwargs.get("headless", False)
+        self.__development: bool = kwargs.get("development", False)
         selenium_driver: str = kwargs.get("firefox", "geckodriver")
         self.__allow_output: bool = kwargs.get("output", False)
         self.success("Output enabled.")
+        if self.__allow_output:
+            warning("Please be aware that too many actions within a short period of time could result in action by "
+                    "Instagram against the account.")
         self.waiting_time: float = kwargs.get("time", None)
         if self.waiting_time is not None and self.waiting_time < 1.5:
-            warning("A short waiting time could help Instagram detect bot activity.")
+            warning("Just a heads up, doing too many things in a short time on Instagram could get the account in "
+                    "trouble.")
         self.__binary_location: str = kwargs.get("binary", None)
         self.success(f"Using {selenium_driver} as driver for selenium.")
         if not self.__headless:
             self.success(f"Running in normal mode (headless: {self.__headless}")
         self.path: str = os.path.abspath(__file__)
         self.__session_data: dict = dict()
         self.__decimal: str = locale.localeconv()["decimal_point"]
@@ -60,15 +65,15 @@
         self.__version__: str = VERSION
 
     def __initialize_driver(self) -> None:
         """Initializes a driver instance for selenium."""
         options = webdriver.FirefoxOptions()
         # I strongly suggest to not use the headless option (Instagram might detect a headless browser)
         if self.__headless:
-            warning("Using the headless option makes it easier to be detected by Instagram.")
+            warning("Enabling the headless option facilitates detection by Instagram.")
             options.add_argument("--headless")
         self.driver = webdriver.Firefox(options=options)
 
     def rest(self, **kwargs) -> None:
         """Rests for a few seconds to avoid detection by Instagram."""
         if self.waiting_time is not None:
             time.sleep(self.waiting_time)
@@ -89,15 +94,16 @@
         """Logs the bot into Instagram."""
         self.driver.get(self.base_url)
         self.rest()
         # cookies
         try:
             self.driver.find_element(By.CLASS_NAME, "_a9--._a9_1").click()
         except Exception as e:
-            warning(e.__str__())
+            if self.__development:
+                warning(e.__str__())
 
         # login attempt
         self.rest()
         username_input = self.driver.find_element(By.NAME, "username")
         username_input.send_keys(self.username)
         self.rest()
         password_input = self.driver.find_element(By.NAME, "password")
@@ -110,21 +116,24 @@
         self.success(f"Logged in @{self.username}")
         self.rest(add=4.5)
 
         try:
             self.driver.find_element(By.CLASS_NAME, "_acan._acao._acas._aj1-").click()
             self.rest()
         except Exception as e:
-            warning(e.__str__())
+            if self.__development:
+                warning(e.__str__())
         try:
             self.driver.find_element(By.CLASS_NAME, "_a9--._a9_1").click()
             self.rest()
             # last index is 0 or one - depending on the output btn
         except Exception as e:
-            warning(e.__str__())
+            if self.__development:
+                warning(e.__str__())
+            self.rest()
 
     def __on_profile(self) -> None:
         """Checks if the driver is currently on a profile."""
         if not re.match(f"{self.base_url}.+/", self.driver.current_url):
             raise Exception("You are currently not on the correct page.")
 
     def search(self, query: str) -> None:
```

### Comparing `InstaWebBot-0.2.9/InstaWebBot.egg-info/PKG-INFO` & `InstaWebBot-0.3.0/InstaWebBot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InstaWebBot
-Version: 0.2.9
+Version: 0.3.0
 Summary: A simple library for managing an Instagram bot as a web application.
 Home-page: https://github.com/Julius-W/InstaBot
 Author: Julius-W
 License: GPL-2.0
 Keywords: python,Instagram,bot,automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,40 +18,42 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # InstaBot
-InstaBot is a Python library that provides some automation for simple tasks on Instagram like following accounts and sending DMs on Instagram using Selenium.
+InstaBot is a Python library that provides some automation for simple tasks on Instagram like following accounts and sending DMs on Instagram using Selenium. Please note that this library is not associated with Instagram or Meta.
 
 ## Installation
 You can install the library from the [GitHub repository](https://github.com/Julius-W/InstaBot) or by using pip:
 
-```
+```bash
 pip install InstaWebBot
 ```
 
 ## Usage
-**_IMPORTANT:_** The driver file for Selenium must be located in the current working directory of your project. You can download the driver [here](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/). Please provide the driver name if you are not using the recommended geckodriver.
+**_IMPORTANT (version older than 0.3.0):_** The driver file for Selenium must be located in the current working directory of your project. You can download the driver [here](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/). Please provide the driver name if you are not using the recommended geckodriver.
 
 Initialize the bot by passing in your Instagram username and password as parameters:
 
 ```py
 from InstaWebBot import InstaBot
 bot = InstaBot('your_username', 'your_password')
+
+# A bot login is required before any other action will be executed.
+bot.login()
 ```
 
 Here is an example with some optional arguments (using their default value if default exists):
 
 ```py
 from InstaWebBot import InstaBot
 
 bot = InstaBot('your_username', 'your_password',
-               headless=False,
                driver="geckodriver",
                output=False,
                time=2.5)
 ```
 
 To log in to Instagram with the given username and password use
```

### Comparing `InstaWebBot-0.2.9/LICENSE` & `InstaWebBot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InstaWebBot-0.2.9/PKG-INFO` & `InstaWebBot-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InstaWebBot
-Version: 0.2.9
+Version: 0.3.0
 Summary: A simple library for managing an Instagram bot as a web application.
 Home-page: https://github.com/Julius-W/InstaBot
 Author: Julius-W
 License: GPL-2.0
 Keywords: python,Instagram,bot,automation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,40 +18,42 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # InstaBot
-InstaBot is a Python library that provides some automation for simple tasks on Instagram like following accounts and sending DMs on Instagram using Selenium.
+InstaBot is a Python library that provides some automation for simple tasks on Instagram like following accounts and sending DMs on Instagram using Selenium. Please note that this library is not associated with Instagram or Meta.
 
 ## Installation
 You can install the library from the [GitHub repository](https://github.com/Julius-W/InstaBot) or by using pip:
 
-```
+```bash
 pip install InstaWebBot
 ```
 
 ## Usage
-**_IMPORTANT:_** The driver file for Selenium must be located in the current working directory of your project. You can download the driver [here](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/). Please provide the driver name if you are not using the recommended geckodriver.
+**_IMPORTANT (version older than 0.3.0):_** The driver file for Selenium must be located in the current working directory of your project. You can download the driver [here](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/). Please provide the driver name if you are not using the recommended geckodriver.
 
 Initialize the bot by passing in your Instagram username and password as parameters:
 
 ```py
 from InstaWebBot import InstaBot
 bot = InstaBot('your_username', 'your_password')
+
+# A bot login is required before any other action will be executed.
+bot.login()
 ```
 
 Here is an example with some optional arguments (using their default value if default exists):
 
 ```py
 from InstaWebBot import InstaBot
 
 bot = InstaBot('your_username', 'your_password',
-               headless=False,
                driver="geckodriver",
                output=False,
                time=2.5)
 ```
 
 To log in to Instagram with the given username and password use
```

### Comparing `InstaWebBot-0.2.9/README.md` & `InstaWebBot-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # InstaBot
-InstaBot is a Python library that provides some automation for simple tasks on Instagram like following accounts and sending DMs on Instagram using Selenium.
+InstaBot is a Python library that provides some automation for simple tasks on Instagram like following accounts and sending DMs on Instagram using Selenium. Please note that this library is not associated with Instagram or Meta.
 
 ## Installation
 You can install the library from the [GitHub repository](https://github.com/Julius-W/InstaBot) or by using pip:
 
-```
+```bash
 pip install InstaWebBot
 ```
 
 ## Usage
-**_IMPORTANT:_** The driver file for Selenium must be located in the current working directory of your project. You can download the driver [here](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/). Please provide the driver name if you are not using the recommended geckodriver.
+**_IMPORTANT (version older than 0.3.0):_** The driver file for Selenium must be located in the current working directory of your project. You can download the driver [here](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/). Please provide the driver name if you are not using the recommended geckodriver.
 
 Initialize the bot by passing in your Instagram username and password as parameters:
 
 ```py
 from InstaWebBot import InstaBot
 bot = InstaBot('your_username', 'your_password')
+
+# A bot login is required before any other action will be executed.
+bot.login()
 ```
 
 Here is an example with some optional arguments (using their default value if default exists):
 
 ```py
 from InstaWebBot import InstaBot
 
 bot = InstaBot('your_username', 'your_password',
-               headless=False,
                driver="geckodriver",
                output=False,
                time=2.5)
 ```
 
 To log in to Instagram with the given username and password use
```

### Comparing `InstaWebBot-0.2.9/setup.py` & `InstaWebBot-0.3.0/setup.py`

 * *Files identical despite different names*

