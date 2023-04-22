# Comparing `tmp/profiwiki-0.1.3.tar.gz` & `tmp/profiwiki-0.1.4.tar.gz`

## Comparing `profiwiki-0.1.3.tar` & `profiwiki-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.pydevproject
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.vscode/settings.json
--rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/bashit
--rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/gencompose
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_27_7
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_30_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_31_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_33_1
--rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/profiwiki-install.sh
--rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/testinstall
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/wiki-config.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/image/phpinfo.php
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/image/profiwiki.php
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/docker.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/patch.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/profiwiki_cmd.py
--rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/profiwiki_core.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/version.py
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.3/scripts/install
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.3/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/basetest.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/test_patch.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/test_profiwiki.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.3/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.3/README.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 profiwiki-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 profiwiki-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.4/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.4/.pydevproject
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.4/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.4/.vscode/settings.json
+-rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/bashit
+-rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/gencompose
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/mw1_27_7
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/mw1_30_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/mw1_31_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/mw1_33_1
+-rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/profiwiki-install.sh
+-rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/testinstall
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/wiki-config.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/image/phpinfo.php
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.4/2018/image/profiwiki.php
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.4/profiwiki/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.4/profiwiki/docker.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.4/profiwiki/patch.py
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 profiwiki-0.1.4/profiwiki/profiwiki_cmd.py
+-rw-r--r--   0        0        0    11407 2020-02-02 00:00:00.000000 profiwiki-0.1.4/profiwiki/profiwiki_core.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.4/profiwiki/version.py
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.4/scripts/install
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.4/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.4/tests/basetest.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.4/tests/test_patch.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 profiwiki-0.1.4/tests/test_profiwiki.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.4/README.md
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 profiwiki-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 profiwiki-0.1.4/PKG-INFO
```

### Comparing `profiwiki-0.1.3/.github/workflows/build.yml` & `profiwiki-0.1.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/.github/workflows/upload-to-pypi.yml` & `profiwiki-0.1.4/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/2018/bashit` & `profiwiki-0.1.4/2018/bashit`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/2018/gencompose` & `profiwiki-0.1.4/2018/gencompose`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/2018/profiwiki-install.sh` & `profiwiki-0.1.4/2018/profiwiki-install.sh`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/2018/testinstall` & `profiwiki-0.1.4/2018/testinstall`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/profiwiki/docker.py` & `profiwiki-0.1.4/profiwiki/docker.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/profiwiki/patch.py` & `profiwiki-0.1.4/profiwiki/patch.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/profiwiki/profiwiki_cmd.py` & `profiwiki-0.1.4/profiwiki/profiwiki_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,27 +30,26 @@
         Returns:
             ArgumentParser: the argument parser
         """
         #script_path=Path(__file__)
         parser = ArgumentParser(description=description, formatter_class=RawDescriptionHelpFormatter)
         config.addArgs(parser)
         parser.add_argument("--about", help="show about info [default: %(default)s]", action="store_true")
+        parser.add_argument("--apache",help="generate apache configuration",action="store_true")
         parser.add_argument("--all",help="do all necessary steps for a full setup",action="store_true")
         parser.add_argument("--bash",help="bash into container",action="store_true")
         parser.add_argument("--create",action="store_true",help="create the wiki") 
         parser.add_argument("--check",action="store_true",help="check the wiki")  
         parser.add_argument("--update",action="store_true",help="start the update script -e.g. to fix SMW key")  
         parser.add_argument("--cron",action="store_true",help="start cron service")        
         parser.add_argument("--down", action="store_true", help="shutdown the wiki [default: %(default)s]")
         parser.add_argument("--patch", action="store_true", help="apply LocalSettings.php patches [default: %(default)s]")
         parser.add_argument("--list",action="store_true",help="list the available profi wikis [default: %(default)s]")
-        parser.add_argument("-fu","--forceuser",action="store_true",help="force overwrite of wikiuser")
         parser.add_argument("-fa", "--fontawesome",   action="store_true", help="install fontawesome")
-        parser.add_argument("-rp", "--randompassword",   action="store_true", help="create random password and create wikiuser while at it")
-        parser.add_argument("-wu","--wikiuser",   action="store_true", help="create wikiuser entry")
+        parser.add_argument("-wuc", "--wikiuser_check",   action="store_true", help="check wikiuser")
         parser.add_argument("-pu", "--plantuml",   action="store_true", help="install plantuml")
         parser.add_argument("-i", "--info", help="show system info", action="store_true")
         parser.add_argument("-V", "--version", action='version', version=version_msg)
         # debug args
         parser.add_argument('--debugServer', help="remote debug Server")
         parser.add_argument('--debugPort', type=int, help="remote debug Port", default=5678)
         parser.add_argument('--debugPathMapping', nargs='+',
```

### Comparing `profiwiki-0.1.3/profiwiki/profiwiki_core.py` & `profiwiki-0.1.4/profiwiki/profiwiki_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 import json
 import tempfile
 import platform
 import os
 from mwdocker.mwcluster import MediaWikiCluster
 from mwdocker.docker import DockerApplication
 from profiwiki.docker import ProfiWikiContainer
-from wikibot3rd.wikiuser import WikiUser
 from mwdocker.config import MwClusterConfig
 from profiwiki.patch import Patch
+from wikibot3rd.wikiuser import WikiUser
 
 class ProfiWiki():
     """
     ProfiWiki
     """
     
     def __init__(self,prefix:str="pw",smw_version="4.1.1",mw_version="1.39.3",port:int=9079):
         """
         constructor
         """        
         self.os_name=platform.system()
         self.os_uname=os.uname()
         self.os_release=platform.release()
         self.args=None
-        self.wikiUser=None
         self.config=MwClusterConfig()
-        self.config.smwVersion=smw_version
+        self.config.smw_version=smw_version
+        self.config.random_password=True
         self.config.prefix=prefix
-        self.config.basePort=port
-        self.config.sqlPort=port-1
+        self.config.base_port=port
+        self.config.sql_port=port-1
         self.config.port=port
         self.config.versions=[mw_version]
         self.config.container_base_name="pw"
-        self.config.extensionNameList=["Admin Links","Diagrams","Header Tabs","ImageMap","ImageLink","MagicNoCache","Maps9",
+        self.config.extensionNameList=["Admin Links","Diagrams","Graph","Header Tabs","ImageMap","ImageLink","MagicNoCache","Maps9",
                                "Mermaid","MsUpload","Nuke","Page Forms","ParserFunctions","PDFEmbed","Renameuser",
                                "Replace Text","Semantic Result Formats","SyntaxHighlight","Variables","UserFunctions"]
         self.config.logo="https://wiki.bitplan.com/images/wiki/thumb/6/63/Profiwikiicon.png/96px-Profiwikiicon.png"
         self.config.__post_init__()
         self.mwCluster=None
         pass
         
@@ -61,38 +61,45 @@
         """
         work as instructed by the arguments
         
         Args:
             args(Namespace): the command line arguments
         """
         self.config.fromArgs(args)
-        self.wiki_id=f"{self.config.container_base_name}"
+        # make sure the wikiId is set from the container base name
+        config_path=self.config.get_config_path()
+        if os.path.isfile(config_path) and not self.config.forceRebuild:
+            # reload the previous configuration e.g. based on container_name only
+            previous_config=self.config.load(config_path)
+            if self.config.verbose:
+                print(f"ProfiWiki with previous configuration from {config_path}...")
+            self.config=previous_config
+        self.config.wikiId=self.config.container_base_name
         if args.bash:
             cmd=f"docker exec -it {self.config.container_base_name}-mw /bin/bash"
             print(cmd)
             return
         mwApp=self.getMwApp(withGenerate=args.forceRebuild)
         if self.config.verbose:
-            print(f"ProfiWiki {mwApp.config.container_base_name} using port {mwApp.config.port} sqlport {mwApp.config.sqlPort}")
-   
-        if args.randompassword:
-            mwApp.config.password=self.config.random_password()
-            self.wikiUser=self.createOrModifyWikiUser(mwApp,force_overwrite=args.forceuser)
-        if args.wikiuser and not self.wikiUser:
-            self.createOrModifyWikiUser(mwApp,force_overwrite=args.forceuser)
+            print(f"ProfiWiki {mwApp.config.container_base_name} using port {mwApp.config.port} sqlport {mwApp.config.sql_port}")
+        if args.force_user:
+            mwApp.createWikiUser(store=True)
         if args.all:
-            if not self.wikiUser:
-                self.wikiUser=self.createOrModifyWikiUser(mwApp,force_overwrite=args.forceuser)
             self.create(mwApp, args.forceRebuild)
             pmw,_pdb=self.getProfiWikiContainers(mwApp)
             pmw.install_fontawesome()
             pmw.install_plantuml()
             self.patch(pmw)
             self.update(mwApp)
             pmw.start_cron()
+        if args.wikiuser_check:
+            self.check_wikiuser(mwApp)
+        if args.apache:
+            apache_config=self.apache_config(mwApp)
+            print(apache_config)
         if args.create:
             self.create(mwApp, args.forceRebuild)
         if args.check:
             self.check(mwApp)
         if args.down:
             self.down(mwApp,args.forceRebuild)
         if args.list:
@@ -105,32 +112,14 @@
                 pmw.install_fontawesome()
             if args.cron:
                 pmw.start_cron()
             if args.patch:
                 self.patch(pmw)
         if args.update:
             self.update(mwApp)
-            
-    def createOrModifyWikiUser(self,mwApp,force_overwrite:bool=False)->WikiUser:
-        """
-        create or modify the WikiUser for this profiwiki
-        
-        Args:
-            mwApp(DockerApplication): the mediawiki docker application
-            force_overwrite(bool): if True overwrite the wikuser info
-        """
-        wikiUsers=WikiUser.getWikiUsers(lenient=True)
-        if self.wiki_id in wikiUsers and not force_overwrite:
-            wikiUser=wikiUsers[self.wiki_id]          
-            if self.config.password != wikiUser.getPassword():
-                raise Exception(f"wikiUser for wiki {self.wiki_id} already exists but with different password")
-            pass
-        else:
-            wikiUser=mwApp.createWikiUser(self.wiki_id,store=True)
-        return wikiUser
     
     def getMwCluster(self,withGenerate:bool=True)->MediaWikiCluster:
         """
         get a mediawiki Cluster for my configuration
         
         Args:
             withGenerate(bool): if True regenerate the configuration files
@@ -207,14 +196,16 @@
 $smwgPageSpecialProperties[] = '_LEDT';
 # Media type
 $smwgPageSpecialProperties[] = '_MEDIA';
 # MIME type
 $smwgPageSpecialProperties[] = '_MIME';
 // https://www.mediawiki.org/wiki/Extension:UserFunctions
 $wgUFEnabledPersonalDataFunctions = ['ip','nickname','realname','useremail','username',];
+// allow user functions in main mediawiki space
+$wgUFAllowedNamespaces[NS_MAIN] = true;
 # increase query limit
 $smwgQMaxLimit = 20000;
 //Default width for the PDF object container.
 $wgPdfEmbed['width'] = 800;
 //Default height for the PDF object container.
 $wgPdfEmbed['height'] = 1090;
 //Allow user the usage of the tag 
@@ -249,8 +240,71 @@
         mwApp.down(forceRebuild=forceRebuild)
         
     def list(self,mwApp):
         """
         list the profi wikis
         """
         print (json.dumps(mwApp.config.as_dict(),indent=2))
-        pass
+        pass
+    
+    def check_wikiuser(self,mwApp:DockerApplication):
+        """
+        """
+        print(f"Checking WikiUser ... for {mwApp.config.container_base_name}")
+        wikiUsers=WikiUser.getWikiUsers(lenient=True)
+        if not mwApp.config.wikiId:
+            print("no WikiId configured")
+            return
+        if not mwApp.config.wikiId in wikiUsers:
+            print(f"no wikiUser for wikiId {mwApp.config.wikiId} found")
+            return
+        wikiUser=wikiUsers[mwApp.config.wikiId]
+        if mwApp.config.password != wikiUser.getPassword():
+            print(f"configured password is different then {mwApp.config.wikiId}")
+        else:
+            print(f"wikiUser for wikiId {mwApp.config.wikiId} is available and password as configured")
+        pass
+            
+    def apache_config(self,mwApp:DockerApplication)->str:
+        """
+        get the apache configuration for the given mediawiki Docker application
+        
+        Args:
+            mwApp(DockerApplication): the docker application to generate the configuration for
+        """
+        config=mwApp.config
+        apache_config=f"""<VirtualHost *:80 >
+    # The ServerName directive sets the request scheme, hostname and port that
+    # the server uses to identify itself. This is used when creating
+    # redirection URLs. In the context of virtual hosts, the ServerName
+    # specifies what hostname must appear in the request's Host: header to
+    # match this virtual host. For the default virtual host (this file) this
+    # value is not decisive as it is used as a last resort host regardless.
+    # However, you must set it for any further virtual host explicitly.
+    ServerName {config.host}
+
+    ServerAdmin webmaster@{config.host}
+    #DocumentRoot /var/www/html
+
+    # Available loglevels: trace8, ..., trace1, debug, info, notice, warn,
+    # error, crit, alert, emerg.
+    # It is also possible to configure the loglevel for particular
+    # modules, e.g.
+    #LogLevel info ssl:warn
+
+    ErrorLog ${{APACHE_LOG_DIR}}/{config.container_base_name}_error.log
+    CustomLog ${{APACHE_LOG_DIR}}/{config.container_base_name}_access.log combined
+
+    # For most configuration files from conf-available/, which are
+    # enabled or disabled at a global level, it is possible to
+    # include a line for only one particular virtual host. For example the
+    # following line enables the CGI configuration for this host only
+    # after it has been globally disabled with "a2disconf".
+    #Include conf-available/serve-cgi-bin.conf
+
+    # Mediawiki installations 
+    ProxyPass / http://localhost:{config.port}/ 
+    ProxyPassReverse / http://localhost:{config.port}/
+</VirtualHost>"""
+        return apache_config
+        
+
```

### Comparing `profiwiki-0.1.3/profiwiki/version.py` & `profiwiki-0.1.4/profiwiki/version.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/tests/basetest.py` & `profiwiki-0.1.4/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/tests/test_patch.py` & `profiwiki-0.1.4/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/tests/test_profiwiki.py` & `profiwiki-0.1.4/tests/test_profiwiki.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """
         setUp the test environment
         """
         Basetest.setUp(self, debug=debug, profile=profile)
         # change the port for the testwiki to not spoil a wiki on the default port
         self.pw=ProfiWiki(prefix="pwt1",port=11000)
         self.mwApp=None
-        self.argv=["--prefix","pwt1","--basePort","11000","--sqlBasePort","11001"]
+        self.argv=["--prefix","pwt1","--base_port","11000","--sql_base_port","11001"]
         
     def testConfig(self):
         """
         test the config
         """
         config_dict=self.pw.config.as_dict()
         debug=self.debug
@@ -80,14 +80,25 @@
         test system pre requisites
         """
         info=self.pw.system_info()
         debug=True
         if debug:
             print(info)
             
+    def test_apache_config(self):
+        """
+        test the apache configuration handling
+        """
+        mwApp=self.getMwApp()
+        apache_config=self.pw.apache_config(mwApp)
+        debug=self.debug
+        debug=True
+        if debug:
+            print(apache_config)
+            
     def test_create(self):
         """
         test creating a wiki
         """
         # remember the docker application
         self.mwApp=self.startMwApp()
```

### Comparing `profiwiki-0.1.3/.gitignore` & `profiwiki-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/LICENSE` & `profiwiki-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/README.md` & `profiwiki-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.3/pyproject.toml` & `profiwiki-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 maintainers = [
   { name = "Wolfgang Fahl", email = "wf@bitplan.com" },
 ]
 readme = "README.md"
 license= "Apache-2.0"
 dependencies = [
   #https://pypi.org/project/pymediawikidocker/
-  "pymediawikidocker>=0.9.8",
+  "pymediawikidocker>=0.10.7",
   #https://pypi.org/project/py-3rdparty-mediawiki/
   "py-3rdparty-mediawiki"
 ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
```

### Comparing `profiwiki-0.1.3/PKG-INFO` & `profiwiki-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProfiWiki
-Version: 0.1.3
+Version: 0.1.4
 Project-URL: Home, https://github.com/BITPlan/ProfiWiki
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/ProfiWiki
 Project-URL: Source, https://github.com/BITPlan/ProfiWiki
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: py-3rdparty-mediawiki
-Requires-Dist: pymediawikidocker>=0.9.8
+Requires-Dist: pymediawikidocker>=0.10.7
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Requires-Dist: ptvsd; extra == 'test'
 Requires-Dist: pydevd; extra == 'test'
 Description-Content-Type: text/markdown
 
 # BITPlan ProfiWiki
```

