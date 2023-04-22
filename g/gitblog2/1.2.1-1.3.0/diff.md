# Comparing `tmp/gitblog2-1.2.1.tar.gz` & `tmp/gitblog2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitblog2-1.2.1.tar", max compression
+gzip compressed data, was "gitblog2-1.3.0.tar", max compression
```

## Comparing `gitblog2-1.2.1.tar` & `gitblog2-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-1.2.1/LICENSE
--rw-r--r--   0        0        0     4702 2023-04-08 12:29:11.807605 gitblog2-1.2.1/README.md
--rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-1.2.1/build.py
--rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-1.2.1/gitblog2/__init__.py
--rwxr-xr-x   0        0        0     1508 2023-04-08 12:27:45.407689 gitblog2-1.2.1/gitblog2/cli.py
--rw-r--r--   0        0        0    17030 2023-04-08 12:27:45.399689 gitblog2-1.2.1/gitblog2/lib.py
--rw-r--r--   0        0        0     1540 2023-02-18 16:19:17.029548 gitblog2-1.2.1/gitblog2/media/by.svg
--rw-r--r--   0        0        0     2543 2023-02-18 16:19:17.029548 gitblog2-1.2.1/gitblog2/media/cc.svg
--rw-r--r--   0        0        0      361 2023-02-18 16:19:17.029548 gitblog2-1.2.1/gitblog2/media/favicon.svg
--rw-r--r--   0        0        0        0 2023-04-08 12:32:27.247411 gitblog2-1.2.1/gitblog2/style.css
--rw-r--r--   0        0        0     1858 2023-04-08 12:28:12.531663 gitblog2-1.2.1/gitblog2/templates/article.html.j2
--rw-r--r--   0        0        0      360 2023-02-18 22:10:35.751606 gitblog2-1.2.1/gitblog2/templates/footer.html.j2
--rw-r--r--   0        0        0      213 2023-02-18 16:19:17.029548 gitblog2-1.2.1/gitblog2/templates/head_common.html.j2
--rw-r--r--   0        0        0      871 2023-04-08 12:28:12.531663 gitblog2-1.2.1/gitblog2/templates/index.html.j2
--rw-r--r--   0        0        0      379 2023-02-18 16:19:17.029548 gitblog2-1.2.1/gitblog2/templates/navbar.html.j2
--rw-r--r--   0        0        0      605 2023-04-08 12:31:33.923464 gitblog2-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 gitblog2-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4896 2023-04-22 18:35:43.638772 gitblog2-1.3.0/README.md
+-rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-1.3.0/build.py
+-rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-1.3.0/gitblog2/__init__.py
+-rwxr-xr-x   0        0        0     1508 2023-04-10 20:54:33.366345 gitblog2-1.3.0/gitblog2/cli.py
+-rw-r--r--   0        0        0    18143 2023-04-15 18:51:02.984473 gitblog2-1.3.0/gitblog2/lib.py
+-rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-1.3.0/gitblog2/media/favicon.svg
+-rw-r--r--   0        0        0     8767 2023-04-12 15:48:28.099547 gitblog2-1.3.0/gitblog2/media/icons.svg
+-rw-r--r--   0        0        0    13612 2023-04-12 16:05:09.595790 gitblog2-1.3.0/gitblog2/style.css
+-rw-r--r--   0        0        0     1774 2023-04-22 17:44:09.292386 gitblog2-1.3.0/gitblog2/templates/article.html.j2
+-rw-r--r--   0        0        0      313 2023-04-22 17:45:42.659838 gitblog2-1.3.0/gitblog2/templates/article_datetimes.html.j2
+-rw-r--r--   0        0        0      318 2023-04-14 23:02:37.663245 gitblog2-1.3.0/gitblog2/templates/author_aside.html.j2
+-rw-r--r--   0        0        0      343 2023-04-12 12:56:32.596295 gitblog2-1.3.0/gitblog2/templates/footer.html.j2
+-rw-r--r--   0        0        0      317 2023-04-13 20:06:07.643473 gitblog2-1.3.0/gitblog2/templates/head_common.html.j2
+-rw-r--r--   0        0        0     1001 2023-04-22 17:46:04.595692 gitblog2-1.3.0/gitblog2/templates/index.html.j2
+-rw-r--r--   0        0        0      199 2023-04-22 16:15:25.109009 gitblog2-1.3.0/gitblog2/templates/navbar.html.j2
+-rw-r--r--   0        0        0      605 2023-04-22 18:39:05.734318 gitblog2-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5512 1970-01-01 00:00:00.000000 gitblog2-1.3.0/PKG-INFO
```

### Comparing `gitblog2-1.2.1/LICENSE` & `gitblog2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitblog2-1.2.1/README.md` & `gitblog2-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # ![Gitblog2 Logo](https://blog.henritel.com/media/favicon.svg "title") Gitblog2
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)  
 
 **Git + Markdown = Blog**  
-
 **Check the [live demo](https://blog.henritel.com)**  
 
 ## What is this?
 
 A blog generator that keeps things simple:  
 
 * 🏄 **Easy to use** - Just write Markdown, no need for a metadata header.
 * ⚡ **Minimal footprint** - No JavaScript, no divs, no class attributes, just semantic html.  
 * 🛠 **Familiar tech** - Git, Markdown, Jinja2 templating.
 
 With many features:
 
 * **RSS feeds** - Atom also provided
-* **Avatars** - from your Github and Codeberg account
+* **Profile card** - based on your Github profile
 
 ## Getting Started
 
 **From zero to a live blog.**
 
 You can see the full setup of a working blog [here](https://github.com/HenriTEL/blog).  
 For this tutorial we assume you'll use **Github** to host your repo and **Cloudflare Pages** to host your blog. You need to have account on those platforms as a prerequisite.  
@@ -42,63 +41,67 @@
         runs-on: ubuntu-latest
         steps:
           - uses: docker://henritel/gitblog2
             with:
               args: post-css cloudflare-pages
             env:
               SOURCE_REPO: https://github.com/${{ github.repository }}
-              URL_BASE: <YOUR_BLOG_URL>
+              GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+              BASE_URL: <YOUR_BLOG_URL>
               CLOUDFLARE_ACCOUNT_ID: ${{ secrets.CLOUDFLARE_ACCOUNT_ID }}
               CLOUDFLARE_API_TOKEN: ${{ secrets.CLOUDFLARE_API_TOKEN }}
     ```
 
-    Set `URL_BASE` with your blog's base url.  
+    Set `BASE_URL` with your blog's base url.  
     This will automatically publish your blog on Cloudflare Pages when you push changes to your repo.  
     It assumes your cloudflare project is named `blog` but if that's not the case you can add an `CLOUDFLARE_PROJECT` env to the workflow with the correponding name.
 3. In your repo's settings, go under `secrets/actions` to set the `CLOUDFLARE_ACCOUNT_ID` and `CLOUDFLARE_API_TOKEN` secrets based on your [Cloudflare API keys](https://developers.cloudflare.com/fundamentals/api/get-started/keys/#view-your-api-key).  
+You don't need to setup `GITHUB_TOKEN` as it will be provided a run time by GitHub.
 
 ## Installation
 
 ```bash
 pip install gitblog2
 ```
 
 ## Usage
 
 From the command line:
 
 ```bash
-gitblog2 https://codeberg.org/HenriTEL/gitblog2.git --repo-subdir=example --url-base=https://example.com
+gitblog2 https://codeberg.org/HenriTEL/gitblog2.git --repo-subdir=example --url-base=https://example.com --no-social
 ```
 
 From the library:
 
 ```python
 from gitblog2 import GitBlog
 
 source_repo = "https://codeberg.org/HenriTEL/git-blog.git"
 output_dir = "./www"
 url_base = "https://example.com"
 with GitBlog(source_repo, repo_subdir="example") as gb:
-    gb.write_blog(output_dir, url_base=url_base)
+    gb.write_blog(output_dir, base_url=url_base, with_social=False)
 ```
 
 From the container:
 
 ```bash
 docker run --rm -v $PWD/www:/www \
     -e SOURCE_REPO=https://github.com/HenriTEL/gitblog2.git \
     -e REPO_SUBDIR=example \
     -e URL_BASE=https://example.com \
+    -e NO_SOCIAL=true \
     henritel/gitblog2
 ```
 
 ## Customisation
 
-Gitblog2 just produces static file so it should easily integrate with the stack you're familiar with (cron jobs, commit hooks, nginx, apache, you name it.).
+Gitblog2 just produces static file so it should easily integrate with the stack you're familiar with (cron jobs, commit hooks, nginx, apache, you name it.).  
+You can use <https://simplecss.org/demo> as an alternate stylesheet.
 
 ## Dev quickstart
 
 Make sure to have [poetry](https://python-poetry.org/) installed, then  
 Setup your local web server:
 
 ```bash
@@ -107,44 +110,43 @@
 zip redbean.zip -j providers/assets/.init.lua
 chmod +x redbean.zip
 ```
 
 In one terminal, update the blog as needed:
 
 ```bash
-poetry run gitblog2 -l debug --repo-subdir=example --base-url=https://example.com
+poetry run gitblog2 -l debug --repo-subdir=example --base-url=https://example.com --no-social
 ```
 
 In another terminal, serve the blog:
 
 ```bash
 ./redbean.zip -D ./www
 ```
 
 ## Roadmap
 
 High priority:
 
-* Fix workflow
-* Calendar icon + read duration like in <https://www.andreinc.net/2023/02/01/demystifying-bitwise-ops>
-* Move author details in a sidebar
-* Move nav back on top, reduce it in mobile mode
+* Fix gh workflow
 * Add image in README like <https://github.com/nextcloud/server>
-* Add doc for customisation
-* Check draft support (set publish_date to first `mv`)
-* Deal with TODOs or make issues for newcomers
-* Add contributing section
-* Add showcase section
-* E2E tests
 
 Low priority:
 
+* Check draft support (set meta publish_date to first `mv`)
+* E2E tests
+* Deal with TODOs or make issues for newcomers
+* Add doc for customisation
+* Make a better TOC extension (remove div and classes)
 * Unit tests
 * Add contributing section
-* Add bio and picture from codeberg
-* Remove div and classes from TOC and footnotes
-* Fix root index.html not served by redbean
-* Make it work on non-unix systems (mainly dealing with windows file system separator)
+* Remove div and classes from footnotes
 
-## Internals
+## Golden resources
 
-Stylesheet is based on water.css
+<https://modernfontstacks.com/>
+<https://anthonyhobday.com/sideprojects/saferules/>
+<https://lawsofux.com/>
+<https://developer.mozilla.org/en-US/docs/Web/HTML>
+<https://developer.mozilla.org/en-US/docs/Web/CSS>
+<https://developer.mozilla.org/en-US/docs/Web/SVG>
+<https://icons.getbootstrap.com/>
```

### Comparing `gitblog2-1.2.1/gitblog2/cli.py` & `gitblog2-1.3.0/gitblog2/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     clone_dir: Optional[str] = typer.Option(None, envvar="CLONE_DIR"),
     repo_subdir: str = typer.Option("", envvar="REPO_SUBDIR"),
     fetch: bool = typer.Option(False, envvar="FETCH"),
     loglevel: LogLevel = typer.Option(
         LogLevel.INFO, "--loglevel", "-l", envvar="LOG_LEVEL"
     ),
     no_feeds: bool = typer.Option(False, envvar="NO_FEED"),
-    no_avatar: bool = typer.Option(False, envvar="NO_AVATAR"),
+    no_social: bool = typer.Option(False, envvar="NO_SOCIAL"),
     base_url: str = typer.Option(None, envvar="BASE_URL"),
 ):  # TODO add arguments descriptions
     logging.basicConfig(level=loglevel.upper(), format="%(message)s")
     logging.info(f"Generating blog into '{output_dir}'...")
     with GitBlog(source_repo, clone_dir, repo_subdir, fetch=fetch) as gb:
         parsed_url = urlparse(base_url) if base_url is not None else None
         gb.write_blog(
             output_dir,
             with_feeds=(not no_feeds),
-            with_avatar=(not no_avatar),
+            with_social=(not no_social),
             base_url=parsed_url,
         )
     logging.info("Done.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gitblog2-1.2.1/gitblog2/lib.py` & `gitblog2-1.3.0/gitblog2/lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,31 @@
 import os
 import re
 import shutil
 from tempfile import TemporaryDirectory
 from typing import cast, Any, DefaultDict, Dict, Generator, List, Optional, Tuple
 from urllib import request
 from urllib.parse import ParseResult, urlparse
+from functools import cached_property
 
 from feedgen.feed import FeedGenerator
 import jinja2
 from markdown import markdown
 import pygit2
 from pygit2 import Blob, Commit, Repository, Tree, GIT_OBJ_TREE
 import requests
 
 
 MD_LIB_EXTENSIONS = ["extra", "toc"]
+MD_LIB_EXTENSION_CONFIGS = {"toc": {"title": " Table of contents"}}
+GITHUB_API_HEADERS = {
+    "Accept": "application/vnd.github+json",
+    "Authorization": f"Bearer {os.getenv('GITHUB_TOKEN')}",
+    "X-GitHub-Api-Version": "2022-11-28",
+}
 
 
 class GitBlog:
     def __init__(
         self,
         source_repo: str,
         clone_dir: Optional[str] = None,
@@ -50,83 +57,109 @@
         ).rstrip("/")
 
         self.pkgdir = os.path.dirname(__file__)
         self.repo = self._init_repo(fetch)
         self.j2env = self._init_templating()
 
         self.section_to_paths: DefaultDict[str, set] = defaultdict(set)
-        self._articles_metadata = None
-        self._sections = None
 
-    @property
+    @cached_property
     def sections(self) -> List[str]:
-        if self._sections is None:
-            self._sections = list(self.gen_sections())
-            logging.debug("Built sections.")
-        return self._sections
+        _sections = list(self.gen_sections())
+        logging.debug("Built sections.")
+        return _sections
 
-    @property
+    @cached_property
     def articles_metadata(self) -> DefaultDict[str, Dict[str, Any]]:
-        if self._articles_metadata is None:
-            self._articles_metadata = defaultdict(dict)
-            for path, commit in self.gen_commits():
-                if "commits" in self._articles_metadata[path]:
-                    self._articles_metadata[path]["commits"].append(commit)
-                else:
-                    self._articles_metadata[path]["commits"] = [commit]
-            logging.debug("Built articles_metadata.")
-        return self._articles_metadata
+        _articles_metadata = defaultdict(dict)
+        for path, commit in self.gen_commits():
+            if "commits" in _articles_metadata[path]:
+                _articles_metadata[path]["commits"].append(commit)
+            else:
+                _articles_metadata[path]["commits"] = [commit]
+        logging.debug("Built articles_metadata.")
+        return _articles_metadata
 
     @property
     def last_commit(self) -> Commit:
         return cast(Commit, self.repo.revparse_single("HEAD"))
 
+    @cached_property
+    def repo_uri(self) -> Optional[ParseResult]:
+        if _is_uri(self.source_repo):
+            return _parse_uri(self.source_repo)
+        git_config = self.source_repo + "/.git/config"
+        url_prefix = "\turl = "
+        if not os.path.exists(git_config):
+            return None
+        # TODO better parse toml and move to a specific function
+        with open(git_config) as gc:
+            for line in gc:
+                if line.startswith(url_prefix):
+                    return _parse_uri(line.lstrip(url_prefix))
+        return None
+
+    @cached_property
+    def social_accounts(self) -> Dict[str, str]:
+        _social_accounts = {"syndication": "/atom.xml"}
+        if self.repo_uri.hostname == "github.com":
+            _social_accounts["github"] = (
+                "https://github.com/" + self.repo_uri.path.split("/")[0]
+            )
+            gh_social_accounts: List[Dict[str, str]] = self._github_api_get(
+                "/user/social_accounts"
+            )
+            for account in gh_social_accounts:
+                _social_accounts[account["provider"]] = account["url"]
+        return _social_accounts
+
     def write_blog(
         self,
         output_dir: str,
         with_feeds=True,
-        with_avatar=True,
+        with_social=True,
         base_url: Optional[ParseResult] = None,
     ):
-        self.write_articles(output_dir, with_avatar=with_avatar)
-        self.write_indexes(output_dir, with_feeds, with_avatar=with_avatar)
+        if with_social:
+            self.download_avatar(output_dir)
+
+        self.write_articles(output_dir, with_social=with_social)
+        self.write_indexes(output_dir, with_feeds, with_social=with_social)
         if with_feeds:
             if base_url is None:
-                raise ReferenceError(
+                raise ValueError(
                     "You need to provide your website base URL in order to generate a feed."
                 )
             self.write_syndication_feeds(output_dir, base_url=base_url)
         self.add_static_assets(output_dir)
-        if with_avatar:
-            self.download_avatar(output_dir)
 
-    def write_articles(self, output_dir: str, with_avatar=True):
+    def write_articles(self, output_dir: str, with_social=True):
         template = self.j2env.get_template("article.html.j2")
         for path, content in self.gen_articles_content():
             full_page = self.render_article(
-                content, path, template, with_avatar=with_avatar
+                content, path, template, with_social=with_social
             )
             target_path = output_dir + "/" + path.replace(".md", ".html")
             _write_file(full_page, target_path)
 
-    def write_indexes(self, output_dir: str, with_feeds=True, with_avatar=True):
+    def write_indexes(self, output_dir: str, with_feeds=True, with_social=True):
         template = self.j2env.get_template("index.html.j2")
         for section in self.sections:
             target_path = f"{output_dir}/{section}/index.html"
             try:
                 full_page = self.render_index(
-                    section, template, with_avatar=with_avatar
+                    section, template, with_social=with_social
                 )
             except Exception as e:
                 logging.error(f"Failed to render index for section {section}")
                 raise e
             _write_file(full_page, target_path)
 
         home_page = self.render_index(
-            template=template, with_feeds=with_feeds, with_avatar=with_avatar
+            template=template, with_feeds=with_feeds, with_social=with_social
         )
         _write_file(home_page, f"{output_dir}/index.html")
 
     def write_syndication_feeds(self, output_dir: str, base_url: ParseResult):
         url_hash = b64encode(base_url.geturl().encode()).decode()
         feed_id = f"ni://{base_url.hostname}/base64;{url_hash}"
         last_commit_dt = _get_commit_dt(self.last_commit)
@@ -158,43 +191,50 @@
         logging.debug("Wrote syndication feeds.")
 
     def render_article(
         self,
         content: str,
         path: str,
         template: Optional[jinja2.Template] = None,
-        with_avatar=True,
+        with_social=True,
     ) -> str:
         """content: Markdown content
         Return content in html format based on the jinja2 template"""
         if template is None:
             template = self.j2env.get_template("article.html.j2")
         title, description, md_content = self.parse_md(content)
         # TODO fix indexes not beeing rendered when render_article not previously called
         self.articles_metadata[path]["relative_path"] = path[:-3]
         self.articles_metadata[path]["title"] = title
         self.articles_metadata[path]["description"] = description
+        self.articles_metadata[path]["read_time_minutes"] = len(md_content) // 200 + 1
         section = path.split("/")[0]
         self.section_to_paths[section].add(path)
-        html_content = markdown(md_content, extensions=MD_LIB_EXTENSIONS)
+        html_content = markdown(
+            md_content,
+            extensions=MD_LIB_EXTENSIONS,
+            extension_configs=MD_LIB_EXTENSION_CONFIGS,
+        )
         return template.render(
             title=title,
             description=description,
             main_content=html_content,
             commits=self.articles_metadata[path]["commits"],
             sections=self.sections,
-            avatar_src="/media/avatar" if with_avatar else None,
+            read_time_minutes=self.articles_metadata[path]["read_time_minutes"],
+            avatar_url="/media/avatar" if with_social else None,
+            social_accounts=self.social_accounts if with_social else None,
         )
 
     def render_index(
         self,
         section: Optional[str] = None,
         template: Optional[jinja2.Template] = None,
         with_feeds=False,
-        with_avatar=False,
+        with_social=False,
     ) -> str:
         if template is None:
             template = self.j2env.get_template("index.html.j2")
         if section is None:
             # TODO sort by publication date
             paths = [p for ps in self.section_to_paths.values() for p in ps]
             section = "Home"
@@ -202,15 +242,15 @@
             paths = self.section_to_paths[section]
         articles = [self.articles_metadata[p] for p in paths]
         return template.render(
             title=section,
             articles=articles,
             sections=self.sections,
             feeds={"atom": "/atom.xml", "rss": "/rss.xml"} if with_feeds else {},
-            avatar_src="/media/avatar" if with_avatar else None,
+            avatar_src="/media/avatar" if with_social else None,
         )
 
     def add_static_assets(self, output_dir: str):
         """Copy static assets from the repo into the outupt dir.
         Use files from the package if not found"""
         media_dst = output_dir + "/media"
         custom_media = self.blog_path + "/media"
@@ -225,49 +265,33 @@
         if os.path.exists(custom_css):
             shutil.copyfile(custom_css, css_dst)
         else:
             shutil.copyfile(default_css, css_dst)
         logging.debug("Added static assets.")
 
     def download_avatar(self, output_dir: str):
-        avatar_dst = output_dir + "/media/avatar.jpg"
-        repo_uri = None
+        avatar_dst = output_dir + "/media/avatar"
         if os.path.exists(avatar_dst):
             # TODO add no-cache option
             return
-        # TODO try to get uri from .git/config as a fallback
-        if _is_uri(self.source_repo):
-            repo_uri = _parse_uri(self.source_repo)
-        else:
-            git_config = self.source_repo + "/.git/config"
-            if not os.path.exists(git_config):
-                return
-            # TODO better parse toml and move to a specific function
-            url_prefix = "\turl = "
-            with open(git_config) as gc:
-                for line in gc:
-                    if line.startswith(url_prefix):
-                        repo_uri = _parse_uri(line.lstrip(url_prefix))
-                        break
-        if not repo_uri:
+        if not self.repo_uri:
             return
         avatar_url = None
-        if repo_uri.hostname == "github.com":
-            username = repo_uri.path.split("/")[0]
-            response = requests.get("https://api.github.com/users/" + username)
-            avatar_url = response.json()["avatar_url"]
-        elif repo_uri.hostname == "codeberg.org":
-            avatar_url = self._get_codeberg_avatar_url(repo_uri)
+        if self.repo_uri.hostname == "github.com":
+            avatar_url = self._github_api_get("/user")["avatar_url"]
+        elif self.repo_uri.hostname == "codeberg.org":
+            avatar_url = self._get_codeberg_avatar_url()
 
         if avatar_url:
-            request.urlretrieve(avatar_url, avatar_dst)
-            logging.debug("Downloaded avatar.")
+            _, response = request.urlretrieve(avatar_url, avatar_dst)
+            logging.info("Avatar downloaded.")
+            logging.debug("Avatar download response headers:\n%s", response)
 
-    def _get_codeberg_avatar_url(repo_uri: ParseResult) -> str:
-        username = repo_uri.path.split("/")[0]
+    def _get_codeberg_avatar_url(self) -> str:
+        username = self.repo_uri.path.split("/")[0]
         user_page = request.urlopen("https://codeberg.org/" + username).read().decode()
         meta_pattern = r'<meta .+"(https://codeberg.org/avatars/\w+)">'
         avatar_url = re.search(meta_pattern, user_page, re.MULTILINE).group(1)
         return avatar_url.rstrip()
 
     def gen_commits(self) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
         def clean_commit(commit: Commit) -> Dict[str, Any]:
@@ -341,14 +365,21 @@
         desc_pattern = r"^\> (.+)\n"
         title = re.search(title_pattern, md_content, re.MULTILINE).group(1).rstrip()
         md_content = re.sub(title_pattern, "", md_content, 1, re.MULTILINE)
         desc = re.search(desc_pattern, md_content, re.MULTILINE).group(1).rstrip()
         md_content = re.sub(desc_pattern, "", md_content, 1, re.MULTILINE)
         return title, desc, md_content
 
+    def _github_api_get(self, resource: str):
+        response = requests.get(
+            "https://api.github.com" + resource, headers=GITHUB_API_HEADERS
+        )
+        response.raise_for_status()
+        return response.json()
+
     def _init_repo(self, fetch: bool = False) -> Repository:
         """Check if there is an existing repo at self.clone_dir and clone the repo there otherwise.
         Optionally fetch changes after that."""
 
         cloned_already = os.path.exists(self.clone_dir + "/.git/")
         if cloned_already:
             repo = Repository(self.clone_dir)
```

### Comparing `gitblog2-1.2.1/gitblog2/templates/article.html.j2` & `gitblog2-1.3.0/gitblog2/templates/article.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<!DOCTYPE html>
-<html>
+<!doctype html>
+<html lang="en">
 
 <head>
     {% include "head_common.html.j2" %}
 
     {% if description -%}
     <meta name="description" content="{{ description }}">
     {% endif -%}
@@ -11,32 +11,28 @@
     <meta property="article:published_time" content="{{ commits[-1].iso_time }}">
     {% if commits|length > 1 -%}
     <meta property="article:modified_time" content="{{ commits[0].iso_time }}">
     {% endif -%}
 </head>
 
 <body>
-    {% include "navbar.html.j2" %}
-    <article>
-        <header>
-            <h1>{{ title }}</h1>
-            <small>
-                {% if commits|length > 1 %}
-                Updated on
-                {% endif %}
-                {{ commits[-1].human_time }}
-            </small><br />
-            {% if description -%}
-            <span>{{ description }}</span>
-            {%- endif %}
-        </header>
-        <main>
-            {{ main_content }}
-        </main>
-        {%- if commits|length > 1 -%}
+    <header>
+        {% include "navbar.html.j2" %}
+        <h1>{{ title }}</h1>
+        {%- if avatar_url and social_accounts %}
+        {% include "author_aside.html.j2" %}
+        {%- endif %}
+        {% if description -%}
+        <p>{{ description }}</p>
+        {%- endif %}
+        {% include "article_datetimes.html.j2" %}
+    </header>
+    <main>
+        {{ main_content }}
+        {%- if commits|length > 1 %}
         <footer>
             <details>
                 <summary>Changelog</summary>
                 <table>
                     <thead>
                         <tr>
                             <th>Date</th>
@@ -51,14 +47,14 @@
                         </tr>
                         {%- endfor %}
                     </tbody>
                 </table>
             </details>
         </footer>
         {%- endif %}
-    </article>
+    </main>
     {% with author_name=commits[0].author.name %}
     {% include "footer.html.j2" %}
     {% endwith %}
 </body>
 
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 {% include "head_common.html.j2" %} {% if description -%}
  {% endif -%}
 
  {% if commits|length > 1 -%}
  {% endif -%}
-{% include "navbar.html.j2" %}
+ {% include "navbar.html.j2" %}
 ****** {{ title }} ******
-{% if commits|length > 1 %} Updated on {% endif %} {{ commits[-1].human_time }}
-{% if description -%} {{ description }} {%- endif %}   {{ main_content }}  {%-
-if commits|length > 1 -%}   Changelog
+{%- if avatar_url and social_accounts %} {% include "author_aside.html.j2" %}
+{%- endif %} {% if description -%}
+{{ description }}
+{%- endif %} {% include "article_datetimes.html.j2" %}   {{ main_content }} {%-
+if commits|length > 1 %}   Changelog
 Date                    Description
 {{ commit.human_time }} {{ commit.message|trim }}
   {%- endif %}  {% with author_name=commits[0].author.name %} {% include
 "footer.html.j2" %} {% endwith %}
```

### Comparing `gitblog2-1.2.1/gitblog2/templates/index.html.j2` & `gitblog2-1.3.0/gitblog2/templates/index.html.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-<!DOCTYPE html>
-<html>
+<!doctype html>
+<html lang="en">
 
 <head>
     {% include "head_common.html.j2" %}
     {%- for type, path in feeds.items() %}
     <link href="{{path}}" type="application/{{type}}+xml" rel="alternate" title="Sitewide {{type}} feed" />
     {%- endfor %}
 </head>
 
 <body>
-    {% include "navbar.html.j2" %}
+    <header>
+        {% include "navbar.html.j2" %}
+    </header>
 
     <main>
         {%- for article in articles %}
         <article>
             <header>
                 <a href="/{{ article.relative_path }}">
                     <h2>{{ article.title }}</h2>
                 </a>
             </header>
             <p>
                 {{ article.description }}
             </p>
-            <small>{{ article.commits[-1].human_time }}</small>
-            <hr />
+            {% with commits=article.commits, read_time_minutes=article.read_time_minutes %}
+            {% include "article_datetimes.html.j2" %}
+            {% endwith %}
         </article>
         {%- endfor %}
     </main>
     {% with author_name=articles[0].commits[0].author.name %}
     {% include "footer.html.j2" %}
     {% endwith %}
 </body>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% include "head_common.html.j2" %} {%- for type, path in feeds.items() %}
  {%- endfor %}
-{% include "navbar.html.j2" %}  {%- for article in articles %}
+ {% include "navbar.html.j2" %}   {%- for article in articles %}
 *****_{{_article.title_}}_*****
 
 {{ article.description }}
-{{ article.commits[-1].human_time }}
-===============================================================================
- {%- endfor %}  {% with author_name=articles[0].commits[0].author.name %} {%
-include "footer.html.j2" %} {% endwith %}
+{% with commits=article.commits, read_time_minutes=article.read_time_minutes %}
+{% include "article_datetimes.html.j2" %} {% endwith %}  {%- endfor %}  {% with
+author_name=articles[0].commits[0].author.name %} {% include "footer.html.j2"
+%} {% endwith %}
```

### Comparing `gitblog2-1.2.1/pyproject.toml` & `gitblog2-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitblog2"
-version = "1.2.1"
+version = "1.3.0"
 description = "Git + Markdown = blog"
 authors = ["Henri Hannetel <henri.hannetel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gitblog2"}]
 include = ["gitblog2/*"]
```

### Comparing `gitblog2-1.2.1/PKG-INFO` & `gitblog2-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitblog2
-Version: 1.2.1
+Version: 1.3.0
 Summary: Git + Markdown = blog
 License: MIT
 Author: Henri Hannetel
 Author-email: henri.hannetel@pm.me
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,29 +18,28 @@
 Description-Content-Type: text/markdown
 
 # ![Gitblog2 Logo](https://blog.henritel.com/media/favicon.svg "title") Gitblog2
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)  
 
 **Git + Markdown = Blog**  
-
 **Check the [live demo](https://blog.henritel.com)**  
 
 ## What is this?
 
 A blog generator that keeps things simple:  
 
 * 🏄 **Easy to use** - Just write Markdown, no need for a metadata header.
 * ⚡ **Minimal footprint** - No JavaScript, no divs, no class attributes, just semantic html.  
 * 🛠 **Familiar tech** - Git, Markdown, Jinja2 templating.
 
 With many features:
 
 * **RSS feeds** - Atom also provided
-* **Avatars** - from your Github and Codeberg account
+* **Profile card** - based on your Github profile
 
 ## Getting Started
 
 **From zero to a live blog.**
 
 You can see the full setup of a working blog [here](https://github.com/HenriTEL/blog).  
 For this tutorial we assume you'll use **Github** to host your repo and **Cloudflare Pages** to host your blog. You need to have account on those platforms as a prerequisite.  
@@ -61,63 +60,67 @@
         runs-on: ubuntu-latest
         steps:
           - uses: docker://henritel/gitblog2
             with:
               args: post-css cloudflare-pages
             env:
               SOURCE_REPO: https://github.com/${{ github.repository }}
-              URL_BASE: <YOUR_BLOG_URL>
+              GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+              BASE_URL: <YOUR_BLOG_URL>
               CLOUDFLARE_ACCOUNT_ID: ${{ secrets.CLOUDFLARE_ACCOUNT_ID }}
               CLOUDFLARE_API_TOKEN: ${{ secrets.CLOUDFLARE_API_TOKEN }}
     ```
 
-    Set `URL_BASE` with your blog's base url.  
+    Set `BASE_URL` with your blog's base url.  
     This will automatically publish your blog on Cloudflare Pages when you push changes to your repo.  
     It assumes your cloudflare project is named `blog` but if that's not the case you can add an `CLOUDFLARE_PROJECT` env to the workflow with the correponding name.
 3. In your repo's settings, go under `secrets/actions` to set the `CLOUDFLARE_ACCOUNT_ID` and `CLOUDFLARE_API_TOKEN` secrets based on your [Cloudflare API keys](https://developers.cloudflare.com/fundamentals/api/get-started/keys/#view-your-api-key).  
+You don't need to setup `GITHUB_TOKEN` as it will be provided a run time by GitHub.
 
 ## Installation
 
 ```bash
 pip install gitblog2
 ```
 
 ## Usage
 
 From the command line:
 
 ```bash
-gitblog2 https://codeberg.org/HenriTEL/gitblog2.git --repo-subdir=example --url-base=https://example.com
+gitblog2 https://codeberg.org/HenriTEL/gitblog2.git --repo-subdir=example --url-base=https://example.com --no-social
 ```
 
 From the library:
 
 ```python
 from gitblog2 import GitBlog
 
 source_repo = "https://codeberg.org/HenriTEL/git-blog.git"
 output_dir = "./www"
 url_base = "https://example.com"
 with GitBlog(source_repo, repo_subdir="example") as gb:
-    gb.write_blog(output_dir, url_base=url_base)
+    gb.write_blog(output_dir, base_url=url_base, with_social=False)
 ```
 
 From the container:
 
 ```bash
 docker run --rm -v $PWD/www:/www \
     -e SOURCE_REPO=https://github.com/HenriTEL/gitblog2.git \
     -e REPO_SUBDIR=example \
     -e URL_BASE=https://example.com \
+    -e NO_SOCIAL=true \
     henritel/gitblog2
 ```
 
 ## Customisation
 
-Gitblog2 just produces static file so it should easily integrate with the stack you're familiar with (cron jobs, commit hooks, nginx, apache, you name it.).
+Gitblog2 just produces static file so it should easily integrate with the stack you're familiar with (cron jobs, commit hooks, nginx, apache, you name it.).  
+You can use <https://simplecss.org/demo> as an alternate stylesheet.
 
 ## Dev quickstart
 
 Make sure to have [poetry](https://python-poetry.org/) installed, then  
 Setup your local web server:
 
 ```bash
@@ -126,45 +129,44 @@
 zip redbean.zip -j providers/assets/.init.lua
 chmod +x redbean.zip
 ```
 
 In one terminal, update the blog as needed:
 
 ```bash
-poetry run gitblog2 -l debug --repo-subdir=example --base-url=https://example.com
+poetry run gitblog2 -l debug --repo-subdir=example --base-url=https://example.com --no-social
 ```
 
 In another terminal, serve the blog:
 
 ```bash
 ./redbean.zip -D ./www
 ```
 
 ## Roadmap
 
 High priority:
 
-* Fix workflow
-* Calendar icon + read duration like in <https://www.andreinc.net/2023/02/01/demystifying-bitwise-ops>
-* Move author details in a sidebar
-* Move nav back on top, reduce it in mobile mode
+* Fix gh workflow
 * Add image in README like <https://github.com/nextcloud/server>
-* Add doc for customisation
-* Check draft support (set publish_date to first `mv`)
-* Deal with TODOs or make issues for newcomers
-* Add contributing section
-* Add showcase section
-* E2E tests
 
 Low priority:
 
+* Check draft support (set meta publish_date to first `mv`)
+* E2E tests
+* Deal with TODOs or make issues for newcomers
+* Add doc for customisation
+* Make a better TOC extension (remove div and classes)
 * Unit tests
 * Add contributing section
-* Add bio and picture from codeberg
-* Remove div and classes from TOC and footnotes
-* Fix root index.html not served by redbean
-* Make it work on non-unix systems (mainly dealing with windows file system separator)
+* Remove div and classes from footnotes
 
-## Internals
+## Golden resources
 
-Stylesheet is based on water.css
+<https://modernfontstacks.com/>
+<https://anthonyhobday.com/sideprojects/saferules/>
+<https://lawsofux.com/>
+<https://developer.mozilla.org/en-US/docs/Web/HTML>
+<https://developer.mozilla.org/en-US/docs/Web/CSS>
+<https://developer.mozilla.org/en-US/docs/Web/SVG>
+<https://icons.getbootstrap.com/>
```

