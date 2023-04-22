# Comparing `tmp/tiktok_uploader-0.1.2.tar.gz` & `tmp/tiktok_uploader-1.0.0.tar.gz`

## Comparing `tiktok_uploader-0.1.2.tar` & `tiktok_uploader-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/.DS_Store
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/LISCENSE
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/.github/workflows/build-hatch.yml
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/examples/example_series_upload.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/__main__.py
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/auth.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/browsers.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/cli.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/config.toml
--rw-r--r--   0        0        0    12443 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/src/tiktok_uploader/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/tests/test_browsers.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/.gitignore
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/README.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 tiktok_uploader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.DS_Store
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/LISCENSE
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.github/workflows/build-hatch.yml
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.github/workflows/link_checker.yml
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/examples/basic_upload.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/examples/multiple_videos_at_once.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/examples/series_upload.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/__init__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/__main__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/auth.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/browsers.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/cli.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/config.toml
+-rw-r--r--   0        0        0    15745 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/upload.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/src/tiktok_uploader/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/tests/test_browsers.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/tests/test_upload.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/.gitignore
+-rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/README.md
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 tiktok_uploader-1.0.0/PKG-INFO
```

### Comparing `tiktok_uploader-0.1.2/.DS_Store` & `tiktok_uploader-1.0.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-0.1.2/LISCENSE` & `tiktok_uploader-1.0.0/LISCENSE`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-0.1.2/.github/workflows/build-hatch.yml` & `tiktok_uploader-1.0.0/.github/workflows/build-hatch.yml`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-0.1.2/examples/example_series_upload.py` & `tiktok_uploader-1.0.0/examples/series_upload.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-0.1.2/src/tiktok_uploader/auth.py` & `tiktok_uploader-1.0.0/src/tiktok_uploader/auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 from time import time, sleep
 
 from selenium.webdriver.common.by import By
 
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
-from tiktok_uploader import config
+from tiktok_uploader import config, logger
 from tiktok_uploader.browsers import get_browser
+from tiktok_uploader.utils import green
 
 class AuthBackend:
     """
     Handles authentication for TikTokUploader
     """
     username: str
     password: str
     cookies: list
 
     def __init__(self, username: str = '', password: str = '',
-                 cookies_list: list = None, cookies=None):
+                 cookies_list: list = None, cookies=None, sessionid: str = None):
         """
         Creates the authenticaiton backend
 
         Keyword arguments:
         - username -> the accounts's username or email
         - password -> the account's password
 
         - cookies -> a list of cookie dictionaries of cookies which is Selenium-compatable
         """
         if (username and not password) or (password and not username):
             raise InsufficientAuth()
 
         self.cookies = self.get_cookies(path=cookies) if cookies else []
         self.cookies += cookies_list if cookies_list else []
+        self.cookies += [{'name': 'sessionid', 'value': sessionid}] if sessionid else []
 
         if not (self.cookies or (username and password)):
             raise InsufficientAuth()
 
         self.username = username
         self.password = password
 
@@ -46,23 +48,25 @@
         """
         Authenticates the agent using the browser backend
         """
         # tries to use cookies
         if not self.cookies and self.username and self.password:
             self.cookies = login(driver, username=self.username, password=self.password)
 
+        logger.debug(green("Authenticating browser with cookies"))
+
         driver.get(config['paths']['main'])
 
         WebDriverWait(driver, config['explicit_wait']).until(EC.title_contains("TikTok"))
 
         for cookie in self.cookies:
             try:
                 driver.add_cookie(cookie)
             except Exception as _:
-                print(f'Failed to add cookie {cookie}')
+                logger.error('Failed to add cookie %s', cookie)
 
         return driver
 
 
     def get_cookies(self, path: str) -> dict:
         """
         Gets cookies from the passed file using the netscape standard
@@ -190,9 +194,21 @@
         cookie_jar.set_cookie(cookie)
 
     cookie_jar.save()
 
 
 class InsufficientAuth(Exception):
     """
-    Raised when there is insufficient authentication
+    Insufficient authentication:
+
+    > TikTok uses cookies to keep track of the user's authentication or session.
+
+    Either:
+        - Use a cookies file passed as the `cookies` argument
+            - easily obtained using https://github.com/kairi003/Get-cookies.txt-LOCALLY
+        - Use a cookies list passed as the `cookies_list` argument
+            - can be obtained from your browser's developer tools under storage -> cookies
+            - only the `sessionid` cookie is required
     """
+
+    def __init__(self, message=None):
+        super().__init__(message or self.__doc__)
```

### Comparing `tiktok_uploader-0.1.2/src/tiktok_uploader/browsers.py` & `tiktok_uploader-1.0.0/src/tiktok_uploader/browsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 from selenium.webdriver.firefox.service import Service as FirefoxService
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from selenium.webdriver.edge.service import Service as EdgeService
 
 from selenium import webdriver
 
-from tiktok_uploader import config
+from tiktok_uploader import config, logger
 
 
 def get_browser(name: str = 'chrome', options=None, *args, **kwargs) -> webdriver:
     """
     Gets a browser based on the name with the ability to pass in additional arguments
     """
+
     # get the web driver for the browser
     driver_to_use = get_driver(name=name, *args, **kwargs)
 
     # gets the options for the browser
+
     options = options or get_default_options(name=name, *args, **kwargs)
 
     # combines them together into a completed driver
     service = get_service(name=name)
     if service:
         driver = driver_to_use(service=service, options=options)
     else:
@@ -44,38 +46,37 @@
     return driver
 
 
 def get_driver(name: str = 'chrome', *args, **kwargs) -> webdriver:
     """
     Gets the web driver function for the browser
     """
-    if clean_name(name) in drivers:
+    if _clean_name(name) in drivers:
         return drivers[name]
 
     raise UnsupportedBrowserException()
 
 
 def get_service(name: str = 'chrome'):
     """
     Gets a service to install the browser driver per webdriver-manager docs
 
     https://pypi.org/project/webdriver-manager/
     """
-    if clean_name(name) in services:
+    if _clean_name(name) in services:
         return services[name]()
-  
+
     return None # Safari doesn't need a service
 
 
 def get_default_options(name: str, *args, **kwargs):
     """
     Gets the default options for each browser to help remain undetected
     """
-    name = clean_name(name)
-
+    name = _clean_name(name)
 
     if name in defaults:
         return defaults[name](*args, **kwargs)
 
     raise UnsupportedBrowserException()
 
 
@@ -92,19 +93,15 @@
 
     ## experimental
     options.add_experimental_option('excludeSwitches', ['enable-automation'])
     options.add_experimental_option('useAutomationExtension', False)
 
     # headless
     if headless:
-        options.add_argument('--headless')
-        options.add_argument('start-maximized')
-        options.add_argument('--disable-gpu')
-
-        options.add_argument(f'--user-agent{config["disguising"]["user_agent"]}')
+        options.add_argument('--headless=new')
 
     return options
 
 
 def firefox_defaults(*args, headless: bool = False, **kwargs) -> FirefoxOptions:
     """
     Creates Firefox with default options
@@ -146,35 +143,47 @@
         options.add_argument('--headless')
 
     return options
 
 # Misc
 class UnsupportedBrowserException(Exception):
     """
-    Exception for when the browser is not supported
+    Browser is not supported by the library
+
+    Supported browsers are:
+        - Chrome
+        - Firefox
+        - Safari
+        - Edge
     """
 
-def clean_name(name: str) -> str:
+    def __init__(self, message=None):
+        super().__init__(message or self.__doc__)
+
+
+def _clean_name(name: str) -> str:
     """
     Cleans the name of the browser to make it easier to use
     """
     return name.strip().lower()
 
+
 drivers = {
     'chrome': webdriver.Chrome,
     'firefox': webdriver.Firefox,
     'safari': webdriver.Safari,
     'edge': webdriver.ChromiumEdge,
 }
 
 defaults = {
     'chrome': chrome_defaults,
     'firefox': firefox_defaults,
     'safari': safari_defaults,
     'edge': edge_defaults,
 }
 
+
 services = {
     'chrome': lambda : ChromeService(ChromeDriverManager().install()),
     'firefox': lambda : FirefoxService(GeckoDriverManager().install()),
     'edge': lambda : EdgeService(EdgeChromiumDriverManager().install()),
 }
```

### Comparing `tiktok_uploader-0.1.2/src/tiktok_uploader/cli.py` & `tiktok_uploader-1.0.0/src/tiktok_uploader/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # runs the program using the arguments provided
     result = upload_video(
         filename=args.video,
         description=args.description,
         username=args.username,
         password=args.password,
         cookies=args.cookies,
+        session_id=args.sessionid,
         headless=args.headless
     )
 
     print('-------------------------')
     if result:
         print('Error while uploading video')
     else:
@@ -45,19 +46,21 @@
 
     # primary arguments
     parser.add_argument('-v', '--video', help='Video file', required=True)
     parser.add_argument('-d', '--description', help='Description', default='')
 
     # authentication arguments
     parser.add_argument('-c', '--cookies', help='The cookies you want to use')
+    parser.add_argument('-s', '--sessionid', help='The session id you want to use')
+
     parser.add_argument('-u', '--username', help='Your TikTok email / username')
     parser.add_argument('-p', '--password', help='Your TikTok password')
 
     # selenium arguments
-    parser.add_argument('--headless', action='store_true', default=False,
+    parser.add_argument('--headless', action='store_true', default=True,
                          help='Runs the program in headless mode (no browser window)')
 
     return parser.parse_args()
 
 
 def validate_uploader_args(args: dict):
     """
```

### Comparing `tiktok_uploader-0.1.2/src/tiktok_uploader/config.toml` & `tiktok_uploader-1.0.0/src/tiktok_uploader/config.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # TikTok Uploader Default Configuation File
 
 headless = false
 quit_on_end = true
 
+# Messing around with inputs
+valid_path_names = ["path", "filename", "video", "video_path"]
+valid_descriptions = ["description", "desc", "caption"]
+
 # Selenium Webdriver Waits
 implicit_wait = 3 # seconds
 explicit_wait = 60 # seconds
 
 supported_file_types = ["mp4", "mov", "avi", "wmv", "flv", "webm", "mkv", "m4v", "3gp", "3g2", "gif"]
 
 max_description_length = 150 # characters
```

### Comparing `tiktok_uploader-0.1.2/src/tiktok_uploader/upload.py` & `tiktok_uploader-1.0.0/src/tiktok_uploader/upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,45 +3,51 @@
 
 Key Functions
 -------------
 upload_video : Uploads a single TikTok video
 upload_videos : Uploads multiple TikTok videos
 """
 from os.path import abspath, exists
+from typing import List
 import time
 
 from selenium.webdriver.common.by import By
 
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.keys import Keys
 
 from tiktok_uploader.browsers import get_browser
 from tiktok_uploader.auth import AuthBackend
-from tiktok_uploader import config
+from tiktok_uploader import config, logger
+from tiktok_uploader.utils import bold, green
 
 
 def upload_video(filename=None, description='', username='',
-                 password='', cookies='', *args, **kwargs):
+                 password='', cookies='', sessionid=None, cookies_list=None, *args, **kwargs):
     """
     Uploads a single TikTok video.
 
     Conder using `upload_videos` if using multiple videos
 
     Parameters
     ----------
     filename : str
         The path to the video to upload
     description : str
         The description to set for the video
     cookies : str
         The cookies to use for uploading
+    sessionid: str
+        The `sessionid` is the only required cookie for uploading,
+            but it is recommended to use all cookies to avoid detection
     """
-    auth = AuthBackend(username=username, password=password, cookies=cookies)
+    auth = AuthBackend(username=username, password=password, cookies=cookies, 
+                       cookies_list=cookies_list, sessionid=sessionid)
 
     return upload_videos(
             videos=[ { 'path': filename, 'description': description } ],
             auth=auth,
             *args, **kwargs
         )
 
@@ -61,65 +67,75 @@
         A selenium webdriver object to use for uploading
     on_complete : function
         A function to call when the upload is complete
     headless : bool
         Whether or not the browser should be run in headless mode
     num_retries : int
         The number of retries to attempt if the upload fails
+    options : SeleniumOptions
+        The options to pass into the browser -> custom privacy settings, etc.
     *args :
         Additional arguments to pass into the upload function
     **kwargs :
         Additional keyword arguments to pass into the upload function
 
     Returns
     -------
     failed : list
         A list of videos which failed to upload
     """
-    if not videos:
-        print("No videos were provided")
-        return
+    videos = _convert_videos_dict(videos)
+
+    if videos and len(videos) > 1:
+        logger.debug("Uploading %d videos", len(videos))
 
     if not browser_agent: # user-specified browser agent
+        logger.debug('Create a %s browser instance %s', browser,
+                    'in headless mode' if headless else '')
         driver = get_browser(name=browser, headless=headless, *args, **kwargs)
     else:
+        logger.debug('Using user-defined browser agent')
         driver = browser_agent
 
     driver = auth.authenticate_agent(driver)
 
     failed = []
     # uploads each video
     for video in videos:
-        print(f'Uploading {video.get("path")}')
         try:
             path = abspath(video.get('path'))
             description = video.get('description', '')
 
+            logger.debug('Posting %s%s', bold(video.get('path')),
+            f'\n{" " * 15}with description: {bold(description)}' if description else '')
+
             # Video must be of supported type
             if not _check_valid_path(path):
                 print(f'{path} is invalid, skipping')
                 failed.append(video)
                 continue
 
             complete_upload_form(driver, path, description,
-                                 num_retires = num_retires, *args, **kwargs)
+                                 num_retires = num_retires, headless=headless, 
+                                 *args, **kwargs)
         except Exception as exception:
-            print(exception)
+            logger.error('Failed to upload %s', path)
+            logger.error(exception)
             failed.append(video)
 
         if on_complete is callable: # calls the user-specified on-complete function
             on_complete(video)
 
     if config['quit_on_end']:
         driver.quit()
 
     return failed
 
 
-def complete_upload_form(driver, path: str, description: str, *args, **kwargs) -> None:
+def complete_upload_form(driver, path: str, description: str, headless=False, *args, **kwargs) -> None:
     """
     Actually uploades each video
 
     Parameters
     ----------
     driver : selenium.webdriver
         The selenium webdriver to use for uploading
@@ -137,14 +153,16 @@
     """
     Navigates to the upload page, switches to the iframe and waits for it to load
 
     Parameters
     ----------
     driver : selenium.webdriver
     """
+    logger.debug(green('Navigating to upload page'))
+
     driver.get(config['paths']['upload'])
 
     # changes to the iframe
     iframe_selector = EC.presence_of_element_located(
         (By.XPATH, config['selectors']['upload']['iframe'])
         )
     iframe = WebDriverWait(driver, config['explicit_wait']).until(iframe_selector)
@@ -165,51 +183,49 @@
     description : str
         The description to set
     """
     if description is None:
         # if no description is provided, filename
         return
 
+    logger.debug(green('Setting description'))
+
     saved_description = description # save the description in case it fails
 
     desc = driver.find_element(By.XPATH, config['selectors']['upload']['description'])
 
     # desc populates with filename before clearing
     WebDriverWait(driver, config['explicit_wait']).until(lambda driver: desc.text != '')
 
     _clear(desc)
 
     try:
         while description:
             nearest_mention = description.find('@')
             nearest_hash = description.find('#')
-            print("description: ", description)
 
             if nearest_mention == 0 or nearest_hash == 0:
                 desc.send_keys('@' if nearest_mention == 0 else '#')
 
                 # wait for the frames to load
                 time.sleep(config['implicit_wait'])
 
                 name = description[1:].split(' ')[0]
-                print("name: ", name)
-                # TODO: sending keys directly for mentions may not work
                 if nearest_mention == 0: # @ case
                     mention_xpath = config['selectors']['upload']['mention_box']
                     condition = EC.presence_of_element_located((By.XPATH, mention_xpath))
                     mention_box = WebDriverWait(driver, config['explicit_wait']).until(condition)
                     mention_box.send_keys(name)
                 else:
                     desc.send_keys(name)
 
                 time.sleep(config['implicit_wait'])
 
                 if nearest_mention == 0: # @ case
                     mention_xpath = config['selectors']['upload']['mentions'].format('@' + name)
-                    print(mention_xpath)
                     condition = EC.presence_of_element_located((By.XPATH, mention_xpath))
                 else:
                     hashtag_xpath = config['selectors']['upload']['hashtags'].format(name)
                     condition = EC.presence_of_element_located((By.XPATH, hashtag_xpath))
 
                 elem = WebDriverWait(driver, config['explicit_wait']).until(condition)
 
@@ -232,32 +248,31 @@
     Clears the text of the element (an issue with the TikTok website when automating)
 
     Parameters
     ----------
     element
         The text box to clear
     """
-    # element.send_keys(Keys.CONTROL + 'a')
-    # element.send_keys(Keys.DELETE)
-
-    element.send_keys(2 * len(element.text) * Keys.BACKSPACE) # margin of safety
+    element.send_keys(2 * len(element.text) * Keys.BACKSPACE)
 
 
 def _set_video(driver, path: str = '', num_retries: int = 3, **kwargs) -> None:
     """
     Sets the video to upload
 
     Parameters
     ----------
     driver : selenium.webdriver
     path : str
         The path to the video to upload
     num_retries : number of retries (can occassionally fail)
     """
     # uploades the element
+    logger.debug(green('Uploading video file'))
+
     for _ in range(num_retries):
         try:
             upload_box = driver.find_element(
                 By.XPATH, config['selectors']['upload']['upload_video']
             )
             upload_box.send_keys(path)
             # waits for the upload progress bar to disappear
@@ -280,37 +295,19 @@
             # wait until a non-draggable image is found
             process_confirmation = EC.presence_of_element_located(
                 (By.XPATH, config['selectors']['upload']['process_confirmation'])
                 )
             WebDriverWait(driver, config['explicit_wait']).until(process_confirmation)
             return
         except Exception as exception:
-            print('Upload exception:', exception)
+            print(exception)
 
     raise FailedToUpload()
 
 
-def _post_video(driver) -> None:
-    """
-    Posts the video
-
-    Parameters
-    ----------
-    driver : selenium.webdriver
-    """
-    post = driver.find_element(By.XPATH, config['selectors']['upload']['post'])
-    post.click()
-
-    # waits for the video to upload
-    post_confirmation = EC.presence_of_element_located(
-        (By.XPATH, config['selectors']['upload']['post_confirmation'])
-        )
-    WebDriverWait(driver, config['explicit_wait']).until(post_confirmation)
-
-
 def _set_interactivity(driver, comment=True, stitch=True, duet=True, *args, **kwargs) -> None:
     """
     Sets the interactivity settings of the video
 
     Parameters
     ----------
     driver : selenium.webdriver
@@ -318,14 +315,16 @@
         Whether or not to allow comments
     stitch : bool
         Whether or not to allow stitching
     duet : bool
         Whether or not to allow duets
     """
     try:
+        logger.debug(green('Setting interactivity settings'))
+
         comment_box = driver.find_element(By.XPATH, config['selectors']['upload']['comment'])
         stitch_box = driver.find_element(By.XPATH, config['selectors']['upload']['stitch'])
         duet_box = driver.find_element(By.XPATH, config['selectors']['upload']['duet'])
 
         # xor the current state with the desired state
         if comment ^ comment_box.is_selected():
             comment_box.click()
@@ -333,33 +332,47 @@
         if stitch ^ stitch_box.is_selected():
             stitch_box.click()
 
         if duet ^ duet_box.is_selected():
             duet_box.click()
 
     except Exception as _:
-        print("Failed to set interactivity settings. Continuing...")
+        logger.error('Failed to set interactivity settings')
 
 
-def _check_valid_path(path: str) -> bool:
+def _post_video(driver) -> None:
     """
-    Returns whether or not the filetype is supported by TikTok
+    Posts the video by clicking the post button
+
+    Parameters
+    ----------
+    driver : selenium.webdriver
     """
-    return exists(path) and path.split('.')[-1] in config['supported_file_types']
+    logger.debug(green('Clicking the post button'))
 
+    post = driver.find_element(By.XPATH, config['selectors']['upload']['post'])
+    post.click()
 
-class DescriptionTooLong(Exception):
-    """
-    A video description longer than the maximum allowed by TikTok's website (not app) uploader
-    """
+    # waits for the video to upload
+    post_confirmation = EC.presence_of_element_located(
+        (By.XPATH, config['selectors']['upload']['post_confirmation'])
+        )
+    WebDriverWait(driver, config['explicit_wait']).until(post_confirmation)
 
-class FailedToUpload(Exception):
+    logger.debug(green('Video posted successfully'))
+
+
+# HELPERS
+
+def _check_valid_path(path: str) -> bool:
     """
-    A video failed to upload
+    Returns whether or not the filetype is supported by TikTok
     """
+    return exists(path) and path.split('.')[-1] in config['supported_file_types']
+
 
 def _get_splice_index(nearest_mention: int, nearest_hashtag: int, description: str) -> int:
     """
     Returns the index to splice the description at
 
     Parameters
     ----------
@@ -377,7 +390,86 @@
         return len(description)
     elif nearest_hashtag == -1:
         return nearest_mention
     elif nearest_mention == -1:
         return nearest_hashtag
     else:
         return min(nearest_mention, nearest_hashtag)
+
+def _convert_videos_dict(videos_list_of_dictionaries) -> List:
+    """
+    Takes in a videos dictionary and converts it.
+
+    This allows the user to use the wrong stuff and thing to just work
+    """
+    if not videos_list_of_dictionaries:
+        raise RuntimeError("No videos to upload")
+
+    valid_path = config['valid_path_names']
+    valid_description = config['valid_descriptions']
+
+    correct_path = valid_path[0]
+    correct_description = valid_description[0]
+
+    def intersection(lst1, lst2):
+        """ return the intersection of two lists """
+        return list(set(lst1) & set(lst2))
+
+    return_list = []
+    for elem in videos_list_of_dictionaries:
+        # preprocesses the dictionary
+        elem = {k.strip().lower(): v for k, v in elem.items()}
+
+        keys = elem.keys()
+        path_intersection = intersection(valid_path, keys)
+        description_interesection = intersection(valid_description, keys)
+
+        if path_intersection:
+            # we have a path
+            path = elem[path_intersection.pop()]
+
+            if not _check_valid_path(path):
+                raise RuntimeError("Invalid path: " + path)
+
+            elem[correct_path] = path
+        else:
+            # iterates over the elem and find a key which is a path with a valid extension
+            for _, value in elem.items():
+                if _check_valid_path(value):
+                    elem[correct_path] = value
+                    break
+            else:
+                # no valid path found
+                raise RuntimeError("Path not found in dictionary: " + str(elem))
+
+        if description_interesection:
+            # we have a description
+            elem[correct_description] = elem[description_interesection.pop()]
+        else:
+            # iterates over the elem and finds a description which is not a valid path
+            for _, value in elem.items():
+                if not _check_valid_path(value):
+                    elem[correct_description] = value
+                    break
+            else:
+                elem[correct_description] = '' # null description is fine
+
+        return_list.append(elem)
+
+    return return_list
+
+class DescriptionTooLong(Exception):
+    """
+    A video description longer than the maximum allowed by TikTok's website (not app) uploader
+    """
+
+    def __init__(self, message=None):
+        super().__init__(message or self.__doc__)
+
+
+class FailedToUpload(Exception):
+    """
+    A video failed to upload
+    """
+
+    def __init__(self, message=None):
+        super().__init__(message or self.__doc__)
```

### Comparing `tiktok_uploader-0.1.2/tests/test_browsers.py` & `tiktok_uploader-1.0.0/tests/test_browsers.py`

 * *Files identical despite different names*

### Comparing `tiktok_uploader-0.1.2/.gitignore` & `tiktok_uploader-1.0.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Customized items
 test.py
+*.txt
+*.mp4
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `tiktok_uploader-0.1.2/README.md` & `tiktok_uploader-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,72 @@
 # ⬆️ TikTok Uploader
 
 ![Forks](https://img.shields.io/github/forks/wkaisertexas/tiktok-uploader)
 ![Stars](https://img.shields.io/github/stars/wkaisertexas/tiktok-uploader)
-![Forks](https://img.shields.io/github/watchers/wkaisertexas/tiktok-uploader)
+![Watchers](https://img.shields.io/github/watchers/wkaisertexas/tiktok-uploader)
 
-> A **Selenium**-based automated **TikTok** video uploader
+A **Selenium**-based automated **TikTok** video uploader
 
+# Table of Contents
+- [Installation](#installation)
+  - [MacOS, Windows and Linux](#macos-windows-and-linux)
+    - [Downloading from PyPI (Recommended)](#downloading-from-pypi-recommended)
+  - [Building from source](#building-from-source)
+- [Usage](#usage)
+  - [💻 Commmand Line Interface (CLI)](#💻-commmand-line-interface-cli)
+  - [⬆️ Uploading Videos](#️⬆️-uploading-videos)
+  - [🫵 Mentions and Hashtags](#🫵-mentions-and-hashtags)
+  - [🪡 Stitches, Duets and Comments](#🪡-stitches-duets-and-comments)
+  - [🔐 Authentication](#🔐-authentication)
+  - [👀 Browser Selection](#👀-browser-selection)
+  - [🚲 Custom WebDriver Driver Options](#🚲-custom-webdriver-driver-options)
+  - [🤯 Headless Browsers](#🤯-headless-browsers)
+  - [🔨 Initial Setup](#🔨-initial-setup)
+- [♻️ Examples](#♻️-examples)
+- [📝 Notes](#📝-notes)
+- [Accounts made with](#accounts-made-using-tiktok-uploader)
 # Installation
 
 A prequisite to using this program is the installation of a [Selenium-compatable](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/) web browser. [Google Chrome](https://www.google.com/chrome/) is recommended.
 
 ## MacOS, Windows and Linux
 
 Install Python 3 or greater from [python.org](https://www.python.org/downloads/)
 
 ### Downloading from PyPI (Recommended)
 
 Install `tiktok-uploader` using `pip`
 
 ```bash
-$ pip install tiktok-uploader
+pip install tiktok-uploader
 ```
 
 ## Building from source
 
 Installing from source allows greater flexability to modify the module's code to extend default behavior. 
 
-First, `clone` and move into the repository. Next, install `hatch`, the build tool used for this project [^1]. Then, `build` the projet. Finally, `install` the project with the `-e` or editable flag.  
+First, `clone` and move into the repository. Next, install `hatch`, the build tool used for this project.[^1] Then, `build` the projet. Finally, `install` the project with the `-e` or editable flag.  
 ```bash
-$ git clone https://github.com/wkaisertexas/tiktok-uploader.git
-$ cd tiktok-uploader
-$ pip install hatch
-$ hatch build
-$ pip install -e . 
+git clone https://github.com/wkaisertexas/tiktok-uploader.git
+cd tiktok-uploader
+pip install hatch
+hatch build
+pip install -e . 
 ```
 
 # Usage
 
-While TikTok is strict about login in from Selenium, simply copying your session tokens is enough to bypass this restriction and be able to upload your videos.
+`tiktok-uploader` works by duplicating your browser's **cookies** which tricks **TikTok** into believing you are logged in on a remote-controlled browser.
 
 ## 💻 Commmand Line Interface (CLI)
 
 Using the CLI is as simple as calling `tiktok-uploader` with your videos: `path` (-v), `description`(-d) and `cookies` (-c)
 
 ```bash
-$ tiktok-uploader \
--v video.mp4 \
--d "this is my escaped \"description\"" \
--c cookies.txt
+tiktok-uploader -v video.mp4 -d "this is my escaped \"description\"" -c cookies.txt
 ```
 
 ```python
 from tiktok_uploader.upload import upload_video, upload_videos
 from tiktok_uploaader.auth import AuthBackend
 
 # single video
@@ -71,15 +86,15 @@
     }
 ]
 
 auth = AuthBackend(cookies='cookies.txt')
 upload_videos(videos=videos, auth=auth)
 ```
 
-## ⬆️ Uploading videos
+## ⬆️ Uploading Videos
 
 This library revolves around the `upload_videos` function which takes in a list of videos which have **filenames** and **descriptions** and are passed as follows:
 
 ```python
 from tiktok_uploader.upload import upload_videos
 from tiktok_uploader.auth import AuthBackend
 
@@ -101,54 +116,77 @@
     print(f'{video['video']} with description "{video['description']}" failed')
 ```
 
 ## 🫵 Mentions and Hashtags
 
 Mentions and Hashtags now work so long as they are followed by a space. However, you as the user are responsible for verifying a mention or hashtag exists before posting
 
-Example:
-
+**Example:**
 ```python
 from tiktok_uploader.upload import upload_video
 
 upload_video('video.mp4', '#fyp @icespicee', 'cookies.txt')
 ```
 
 ## 🪡 Stitches, Duets and Comments
 
-To set whether or not a video uploaded allows stitches, comments or duet, simply specifiy `comment`, `stitch` and `duet` as keyword arguments to `upload_video` or `upload_videos`.
+To set whether or not a video uploaded allows stitches, comments or duet, simply specifiy `comment`, `stitch` and/or `duet` as keyword arguments to `upload_video` or `upload_videos`.
 
 ```python
 upload_video(..., comment=True, stitch=True, duet=True)
 ```
 
 > Comments, Stiches and Duets are allowed by **default**
 
 ## 🔐 Authentication
-Authentication uses your browser's cookies. This workaround was done due to TikTok's stricter stance on authetication. 
+Authentication uses your browser's cookies. This workaround was done due to TikTok's stricter stance on authetication by a Selenium-controlled browser.
+
+Your `sessionid` is all that is required for authentication and can be passed as an argument to nearly any function
+
+[🍪 Get cookies.txt](https://github.com/kairi003/Get-cookies.txt-LOCALLY) makes getting cookies in a [NetScape cookies format](http://fileformats.archiveteam.org/wiki/Netscape_cookies.txt).
+
+After installing, open the extensions menu on [TikTok.com](https://tiktok.com/) and click `🍪 Get cookies.txt` to reveal your cookies. Select `Export As ⇩` and specify a location and name to save.
 
-To get your cookies, download [🍪 Get cookies.txt](https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid?hl=en) from the **Chrome Web Store**.
+**Optionally**, `cookies_list` is a list of dictionaries with keys `name`, `value`, `domain`, `path` and `expiry` which allow you to pass your own browser cookies. 
 
-Open the extensions menu on TikTok and click `🍪 Get cookies.txt` to reveal your cookies. Select `Export As ⇩` and specify a location and name to save.
+**Example:**
+
+```python
+cookies_list = [
+    {
+        'name': 'sessionid',
+        'value': '**your session id**',
+        'domain': 'https://tiktok.com',
+        'path': '/',
+        'expiry': '10/8/2023, 12:18:58 PM'
+    }
+]
 
-> Optionally, if you would like to pass your own cookies you may do as an array of dictionaries with keys `name`, `value`, `domain`, `path` and `expiry` 
+upload_video(..., cookies_list=cookies_list)
+```
 
 ## 👀 Browser Selection
 
-[Google Chrome](https://www.google.com/chrome) is the prefered browser for **TikTokUploader**. The default anti-detection techniques used in this packaged are optimized for this. However, if you wish to use a different browser you may specify that in `upload_videos`.
+[Google Chrome](https://www.google.com/chrome) is the prefered browser for **TikTokUploader**. The default anti-detection techniques used in this packaged are optimized for this. However, if you wish to use a different browser you may specify the `browser` in `upload_video` or `upload_videos`.
 
 ```python
 from tiktok_uploader.upload import upload_video
 
 from random import choice
 
-BROWSERS = ['chrome', 'safari', 'chromium', 'edge', 'firefox']
+BROWSERS = [
+    'chrome',
+    'safari',
+    'chromium',
+    'edge',
+    'firefox'
+]
 
 # randomly picks a web browser 
-upload_video(browser=choice(BROWSERS))
+upload_video(..., browser=choice(BROWSERS))
 ```
 
 ✅ Supported Browsers:
 - **Chrome** (Recommended)
 - **Safari**
 - **Chromium**
 - **Edge**
@@ -163,40 +201,45 @@
 ```python
 from selenium.webdriver.chrome.options import Options
 
 options = Options()
 
 options.add_argument('start-maximized')
 
-upload_videos(options=options)
+upload_videos(..., options=options)
 ```
 
 > Note: Make sure to use the right selenium options for your browser
 
 ## 🤯 Headless Browsers
 
-**Headless browsers do not work at this time** 
+Headless browsing only works on Chrome. When using Chrome, adding the `--headless` flag using the CLI or passing `headless` as a keyword argument to `upload_video` or `upload_videos` is all that is required.
 
-> If more experienced in Webscraping, I would really appreciate helping make this work. [undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver) was already tried and did not work
+```python
+upload_video(..., headless=True)
+upload_videos(..., headless=True)
+```
 
 ## 🔨 Initial Setup
 
 [WebDriverManager](https://bonigarcia.dev/webdrivermanager/) is used to manage driver versions. 
 
-On intial startup, you **may** be prompted to install the correct driver for your selected broswer. However, for **Chrome** and **Edge** this works without issue.
+On intial startup, you **may** be prompted to install the correct driver for your selected broswer. However, for **Chrome** and **Edge** the driver is automatically installed.
 
 # ♻️ Examples
 
-[Scheduled Uploader]() is an automation which is based off this package. Videos are read from a CSV file using [Pandas](https://pandas.pydata.org). A video upload attempt is made and **if and only if** it is successfull will the video be marked as uploaded.
+- **[Basic Upload Example](exmples/basic_upload.py):** Uses `upload_video` to make one post.
+
+- **[Series Upload Example](examples/series_upload.py):** Uploads the same video multiple times using `upload_videos`.
 
-## 📝 Notes
+- **[Scheduled Uploader Example](examples/example_series_upload.py):** Videos are read from a CSV file using [Pandas](https://pandas.pydata.org). A video upload attempt is made and **if and only if** it is successful will the video be marked as uploaded.
 
-This bot is not fool proof. Though I have not gotten an official ban, when the video will fail to upload after too many uploads. When testing, waiting several hours was sufficient to fix this problem. For this reason, please thing of this more as a scheduled uploader for TikTok videos, rather than a spam bot.
+# 📝 Notes
 
-> Please think of this package as more of a scheduled uploader for TikTok videos, rather than a spam bot
+This bot is not fool proof. Though I have not gotten an official ban, the video will fail to upload after too many uploads. In testing, waiting several hours was sufficient to fix this problem. For this reason, please thing of this more as a scheduled uploader for TikTok videos, rather than a spam bot.
 
-## Accounts made using `tiktok-uploader`
+# Accounts made with
 
 - [@C_Span](https://www.tiktok.com/@c_span?lang=en) - A split-screen channel with mobile games below featuring clips from C-Span's YouTube channel
-- [@habit_track](https://www.tiktok.com/@habit_track?lang=en) - A generic Dhar Mann TikTok bot
+- [@habit_track](https://www.tiktok.com/@habit_track?lang=en) - A Reddit bot to see which SubReddit is most viral on TikTok
 
-[^1]: If interested in Hatch, checkout the [website](https://hatch.pypa.io/latest/build/)
+[^1]: If interested in Hatch, checkout the [website](https://hatch.pypa.io/latest/build/)
```

### Comparing `tiktok_uploader-0.1.2/pyproject.toml` & `tiktok_uploader-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "tiktok-uploader"
-version = "0.1.2"
+version = "1.0.0"
 authors = [
   { name = "William Kaiser", email = "wkaisertexas@gmail.com" },
 ]
-description = "An automatic TikTok video uploader w/ CLI. Uses cookies from your browser to manage authentication and upload your videos automatically."
+description = "An automatic TikTok video uploader w/ CLI. Uploads videos automatically using an automated browser and your cookies for authentication."
 readme = "README.md"
 requires-python = ">=3.0"
 keywords = [
 	"Selenium",
 	"Automation",
 	"TikTok",
   "Video",
```

### Comparing `tiktok_uploader-0.1.2/PKG-INFO` & `tiktok_uploader-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tiktok-uploader
-Version: 0.1.2
-Summary: An automatic TikTok video uploader w/ CLI. Uses cookies from your browser to manage authentication and upload your videos automatically.
+Version: 1.0.0
+Summary: An automatic TikTok video uploader w/ CLI. Uploads videos automatically using an automated browser and your cookies for authentication.
 Project-URL: Source Code, https://github.com/wkaisertexas/tiktok-uploader
 Project-URL: Bug Tracker, https://github.com/wkaisertexas/tiktok-uploader/issues
 Author-email: William Kaiser <wkaisertexas@gmail.com>
 Keywords: Automation,CLI,Command Line,Python,Selenium,TikTok,Upload,Video
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -17,60 +17,75 @@
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ⬆️ TikTok Uploader
 
 ![Forks](https://img.shields.io/github/forks/wkaisertexas/tiktok-uploader)
 ![Stars](https://img.shields.io/github/stars/wkaisertexas/tiktok-uploader)
-![Forks](https://img.shields.io/github/watchers/wkaisertexas/tiktok-uploader)
+![Watchers](https://img.shields.io/github/watchers/wkaisertexas/tiktok-uploader)
 
-> A **Selenium**-based automated **TikTok** video uploader
+A **Selenium**-based automated **TikTok** video uploader
 
+# Table of Contents
+- [Installation](#installation)
+  - [MacOS, Windows and Linux](#macos-windows-and-linux)
+    - [Downloading from PyPI (Recommended)](#downloading-from-pypi-recommended)
+  - [Building from source](#building-from-source)
+- [Usage](#usage)
+  - [💻 Commmand Line Interface (CLI)](#💻-commmand-line-interface-cli)
+  - [⬆️ Uploading Videos](#️⬆️-uploading-videos)
+  - [🫵 Mentions and Hashtags](#🫵-mentions-and-hashtags)
+  - [🪡 Stitches, Duets and Comments](#🪡-stitches-duets-and-comments)
+  - [🔐 Authentication](#🔐-authentication)
+  - [👀 Browser Selection](#👀-browser-selection)
+  - [🚲 Custom WebDriver Driver Options](#🚲-custom-webdriver-driver-options)
+  - [🤯 Headless Browsers](#🤯-headless-browsers)
+  - [🔨 Initial Setup](#🔨-initial-setup)
+- [♻️ Examples](#♻️-examples)
+- [📝 Notes](#📝-notes)
+- [Accounts made with](#accounts-made-using-tiktok-uploader)
 # Installation
 
 A prequisite to using this program is the installation of a [Selenium-compatable](https://www.selenium.dev/documentation/webdriver/getting_started/install_drivers/) web browser. [Google Chrome](https://www.google.com/chrome/) is recommended.
 
 ## MacOS, Windows and Linux
 
 Install Python 3 or greater from [python.org](https://www.python.org/downloads/)
 
 ### Downloading from PyPI (Recommended)
 
 Install `tiktok-uploader` using `pip`
 
 ```bash
-$ pip install tiktok-uploader
+pip install tiktok-uploader
 ```
 
 ## Building from source
 
 Installing from source allows greater flexability to modify the module's code to extend default behavior. 
 
-First, `clone` and move into the repository. Next, install `hatch`, the build tool used for this project [^1]. Then, `build` the projet. Finally, `install` the project with the `-e` or editable flag.  
+First, `clone` and move into the repository. Next, install `hatch`, the build tool used for this project.[^1] Then, `build` the projet. Finally, `install` the project with the `-e` or editable flag.  
 ```bash
-$ git clone https://github.com/wkaisertexas/tiktok-uploader.git
-$ cd tiktok-uploader
-$ pip install hatch
-$ hatch build
-$ pip install -e . 
+git clone https://github.com/wkaisertexas/tiktok-uploader.git
+cd tiktok-uploader
+pip install hatch
+hatch build
+pip install -e . 
 ```
 
 # Usage
 
-While TikTok is strict about login in from Selenium, simply copying your session tokens is enough to bypass this restriction and be able to upload your videos.
+`tiktok-uploader` works by duplicating your browser's **cookies** which tricks **TikTok** into believing you are logged in on a remote-controlled browser.
 
 ## 💻 Commmand Line Interface (CLI)
 
 Using the CLI is as simple as calling `tiktok-uploader` with your videos: `path` (-v), `description`(-d) and `cookies` (-c)
 
 ```bash
-$ tiktok-uploader \
--v video.mp4 \
--d "this is my escaped \"description\"" \
--c cookies.txt
+tiktok-uploader -v video.mp4 -d "this is my escaped \"description\"" -c cookies.txt
 ```
 
 ```python
 from tiktok_uploader.upload import upload_video, upload_videos
 from tiktok_uploaader.auth import AuthBackend
 
 # single video
@@ -90,15 +105,15 @@
     }
 ]
 
 auth = AuthBackend(cookies='cookies.txt')
 upload_videos(videos=videos, auth=auth)
 ```
 
-## ⬆️ Uploading videos
+## ⬆️ Uploading Videos
 
 This library revolves around the `upload_videos` function which takes in a list of videos which have **filenames** and **descriptions** and are passed as follows:
 
 ```python
 from tiktok_uploader.upload import upload_videos
 from tiktok_uploader.auth import AuthBackend
 
@@ -120,54 +135,77 @@
     print(f'{video['video']} with description "{video['description']}" failed')
 ```
 
 ## 🫵 Mentions and Hashtags
 
 Mentions and Hashtags now work so long as they are followed by a space. However, you as the user are responsible for verifying a mention or hashtag exists before posting
 
-Example:
-
+**Example:**
 ```python
 from tiktok_uploader.upload import upload_video
 
 upload_video('video.mp4', '#fyp @icespicee', 'cookies.txt')
 ```
 
 ## 🪡 Stitches, Duets and Comments
 
-To set whether or not a video uploaded allows stitches, comments or duet, simply specifiy `comment`, `stitch` and `duet` as keyword arguments to `upload_video` or `upload_videos`.
+To set whether or not a video uploaded allows stitches, comments or duet, simply specifiy `comment`, `stitch` and/or `duet` as keyword arguments to `upload_video` or `upload_videos`.
 
 ```python
 upload_video(..., comment=True, stitch=True, duet=True)
 ```
 
 > Comments, Stiches and Duets are allowed by **default**
 
 ## 🔐 Authentication
-Authentication uses your browser's cookies. This workaround was done due to TikTok's stricter stance on authetication. 
+Authentication uses your browser's cookies. This workaround was done due to TikTok's stricter stance on authetication by a Selenium-controlled browser.
+
+Your `sessionid` is all that is required for authentication and can be passed as an argument to nearly any function
+
+[🍪 Get cookies.txt](https://github.com/kairi003/Get-cookies.txt-LOCALLY) makes getting cookies in a [NetScape cookies format](http://fileformats.archiveteam.org/wiki/Netscape_cookies.txt).
+
+After installing, open the extensions menu on [TikTok.com](https://tiktok.com/) and click `🍪 Get cookies.txt` to reveal your cookies. Select `Export As ⇩` and specify a location and name to save.
 
-To get your cookies, download [🍪 Get cookies.txt](https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid?hl=en) from the **Chrome Web Store**.
+**Optionally**, `cookies_list` is a list of dictionaries with keys `name`, `value`, `domain`, `path` and `expiry` which allow you to pass your own browser cookies. 
 
-Open the extensions menu on TikTok and click `🍪 Get cookies.txt` to reveal your cookies. Select `Export As ⇩` and specify a location and name to save.
+**Example:**
+
+```python
+cookies_list = [
+    {
+        'name': 'sessionid',
+        'value': '**your session id**',
+        'domain': 'https://tiktok.com',
+        'path': '/',
+        'expiry': '10/8/2023, 12:18:58 PM'
+    }
+]
 
-> Optionally, if you would like to pass your own cookies you may do as an array of dictionaries with keys `name`, `value`, `domain`, `path` and `expiry` 
+upload_video(..., cookies_list=cookies_list)
+```
 
 ## 👀 Browser Selection
 
-[Google Chrome](https://www.google.com/chrome) is the prefered browser for **TikTokUploader**. The default anti-detection techniques used in this packaged are optimized for this. However, if you wish to use a different browser you may specify that in `upload_videos`.
+[Google Chrome](https://www.google.com/chrome) is the prefered browser for **TikTokUploader**. The default anti-detection techniques used in this packaged are optimized for this. However, if you wish to use a different browser you may specify the `browser` in `upload_video` or `upload_videos`.
 
 ```python
 from tiktok_uploader.upload import upload_video
 
 from random import choice
 
-BROWSERS = ['chrome', 'safari', 'chromium', 'edge', 'firefox']
+BROWSERS = [
+    'chrome',
+    'safari',
+    'chromium',
+    'edge',
+    'firefox'
+]
 
 # randomly picks a web browser 
-upload_video(browser=choice(BROWSERS))
+upload_video(..., browser=choice(BROWSERS))
 ```
 
 ✅ Supported Browsers:
 - **Chrome** (Recommended)
 - **Safari**
 - **Chromium**
 - **Edge**
@@ -182,40 +220,45 @@
 ```python
 from selenium.webdriver.chrome.options import Options
 
 options = Options()
 
 options.add_argument('start-maximized')
 
-upload_videos(options=options)
+upload_videos(..., options=options)
 ```
 
 > Note: Make sure to use the right selenium options for your browser
 
 ## 🤯 Headless Browsers
 
-**Headless browsers do not work at this time** 
+Headless browsing only works on Chrome. When using Chrome, adding the `--headless` flag using the CLI or passing `headless` as a keyword argument to `upload_video` or `upload_videos` is all that is required.
 
-> If more experienced in Webscraping, I would really appreciate helping make this work. [undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver) was already tried and did not work
+```python
+upload_video(..., headless=True)
+upload_videos(..., headless=True)
+```
 
 ## 🔨 Initial Setup
 
 [WebDriverManager](https://bonigarcia.dev/webdrivermanager/) is used to manage driver versions. 
 
-On intial startup, you **may** be prompted to install the correct driver for your selected broswer. However, for **Chrome** and **Edge** this works without issue.
+On intial startup, you **may** be prompted to install the correct driver for your selected broswer. However, for **Chrome** and **Edge** the driver is automatically installed.
 
 # ♻️ Examples
 
-[Scheduled Uploader]() is an automation which is based off this package. Videos are read from a CSV file using [Pandas](https://pandas.pydata.org). A video upload attempt is made and **if and only if** it is successfull will the video be marked as uploaded.
+- **[Basic Upload Example](exmples/basic_upload.py):** Uses `upload_video` to make one post.
+
+- **[Series Upload Example](examples/series_upload.py):** Uploads the same video multiple times using `upload_videos`.
 
-## 📝 Notes
+- **[Scheduled Uploader Example](examples/example_series_upload.py):** Videos are read from a CSV file using [Pandas](https://pandas.pydata.org). A video upload attempt is made and **if and only if** it is successful will the video be marked as uploaded.
 
-This bot is not fool proof. Though I have not gotten an official ban, when the video will fail to upload after too many uploads. When testing, waiting several hours was sufficient to fix this problem. For this reason, please thing of this more as a scheduled uploader for TikTok videos, rather than a spam bot.
+# 📝 Notes
 
-> Please think of this package as more of a scheduled uploader for TikTok videos, rather than a spam bot
+This bot is not fool proof. Though I have not gotten an official ban, the video will fail to upload after too many uploads. In testing, waiting several hours was sufficient to fix this problem. For this reason, please thing of this more as a scheduled uploader for TikTok videos, rather than a spam bot.
 
-## Accounts made using `tiktok-uploader`
+# Accounts made with
 
 - [@C_Span](https://www.tiktok.com/@c_span?lang=en) - A split-screen channel with mobile games below featuring clips from C-Span's YouTube channel
-- [@habit_track](https://www.tiktok.com/@habit_track?lang=en) - A generic Dhar Mann TikTok bot
+- [@habit_track](https://www.tiktok.com/@habit_track?lang=en) - A Reddit bot to see which SubReddit is most viral on TikTok
 
-[^1]: If interested in Hatch, checkout the [website](https://hatch.pypa.io/latest/build/)
+[^1]: If interested in Hatch, checkout the [website](https://hatch.pypa.io/latest/build/)
```

