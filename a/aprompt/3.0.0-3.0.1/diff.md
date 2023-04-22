# Comparing `tmp/aprompt-3.0.0.tar.gz` & `tmp/aprompt-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aprompt-3.0.0.tar", last modified: Wed Mar 22 16:54:51 2023, max compression
+gzip compressed data, was "aprompt-3.0.1.tar", last modified: Sat Apr 22 13:13:22 2023, max compression
```

## Comparing `aprompt-3.0.0.tar` & `aprompt-3.0.1.tar`

### file list

```diff
@@ -1,181 +1,67 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:51.236828 aprompt-3.0.0/
--rwxrwxrwx   0 root         (0) root         (0)      189 2023-03-22 14:49:30.000000 aprompt-3.0.0/.readthedocs.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:42.490721 aprompt-3.0.0/.tox/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:42.980732 aprompt-3.0.0/.tox/py311/
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-03-22 14:59:56.000000 aprompt-3.0.0/.tox/py311/.tox-info.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:43.029383 aprompt-3.0.0/.tox/py39/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-03-22 14:55:09.000000 aprompt-3.0.0/.tox/py39/.tox-info.json
--rwxrwxrwx   0 root         (0) root         (0)     1092 2023-03-08 22:23:44.000000 aprompt-3.0.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     2540 2023-03-22 16:54:51.236828 aprompt-3.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1903 2023-03-22 15:13:38.000000 aprompt-3.0.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:43.471822 aprompt-3.0.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-03-08 13:46:51.000000 aprompt-3.0.0/docs/Makefile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:42.542410 aprompt-3.0.0/docs/_build/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:44.263207 aprompt-3.0.0/docs/_build/doctrees/
--rwxrwxrwx   0 root         (0) root         (0)  2312759 2023-03-22 15:54:09.000000 aprompt-3.0.0/docs/_build/doctrees/api.doctree
--rwxrwxrwx   0 root         (0) root         (0)     8186 2023-03-22 15:54:09.000000 aprompt-3.0.0/docs/_build/doctrees/changelog.doctree
--rwxrwxrwx   0 root         (0) root         (0)     4293 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/clean-up.doctree
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:44.333134 aprompt-3.0.0/docs/_build/doctrees/contributing/
--rwxrwxrwx   0 root         (0) root         (0)     3401 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/contributing/index.doctree
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:44.644234 aprompt-3.0.0/docs/_build/doctrees/customization/
--rwxrwxrwx   0 root         (0) root         (0)     4214 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/customization/custom-formatter.doctree
--rwxrwxrwx   0 root         (0) root         (0)    16909 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/customization/custom-prompt-engine.doctree
--rwxrwxrwx   0 root         (0) root         (0)     6905 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/customization/custom-widgets.doctree
--rwxrwxrwx   0 root         (0) root         (0)     5601 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/customization/directory-structure.doctree
--rwxrwxrwx   0 root         (0) root         (0)     4269 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/customization/index.doctree
--rwxrwxrwx   0 root         (0) root         (0)  2678348 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/environment.pickle
--rwxrwxrwx   0 root         (0) root         (0)  2383407 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/extensions.doctree
--rwxrwxrwx   0 root         (0) root         (0)     4389 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/index.doctree
--rwxrwxrwx   0 root         (0) root         (0)     7442 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/license.doctree
--rwxrwxrwx   0 root         (0) root         (0)  2508768 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/prompts.doctree
--rwxrwxrwx   0 root         (0) root         (0)    10456 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/quickstart.doctree
--rwxrwxrwx   0 root         (0) root         (0)     8817 2023-03-22 15:54:10.000000 aprompt-3.0.0/docs/_build/doctrees/testing.doctree
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:45.467056 aprompt-3.0.0/docs/_build/html/
--rwxrwxrwx   0 root         (0) root         (0)      230 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/.buildinfo
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:45.609956 aprompt-3.0.0/docs/_build/html/_images/
--rwxrwxrwx   0 root         (0) root         (0)    86590 2023-03-12 14:54:21.000000 aprompt-3.0.0/docs/_build/html/_images/prompt-choice.gif
--rwxrwxrwx   0 root         (0) root         (0)    39675 2023-03-12 14:47:07.000000 aprompt-3.0.0/docs/_build/html/_images/prompt-confirm.gif
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:46.152577 aprompt-3.0.0/docs/_build/html/_sources/
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-03-10 12:18:56.000000 aprompt-3.0.0/docs/_build/html/_sources/api.md.txt
--rwxrwxrwx   0 root         (0) root         (0)     1061 2023-03-08 22:01:20.000000 aprompt-3.0.0/docs/_build/html/_sources/changelog.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      623 2023-03-10 15:13:59.000000 aprompt-3.0.0/docs/_build/html/_sources/clean-up.md.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:46.213340 aprompt-3.0.0/docs/_build/html/_sources/contributing/
--rwxrwxrwx   0 root         (0) root         (0)      199 2023-03-08 22:36:19.000000 aprompt-3.0.0/docs/_build/html/_sources/contributing/index.md.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:46.480806 aprompt-3.0.0/docs/_build/html/_sources/customization/
--rwxrwxrwx   0 root         (0) root         (0)      225 2023-03-10 20:57:07.000000 aprompt-3.0.0/docs/_build/html/_sources/customization/custom-formatter.md.txt
--rwxrwxrwx   0 root         (0) root         (0)     2705 2023-03-14 14:53:08.000000 aprompt-3.0.0/docs/_build/html/_sources/customization/custom-prompt-engine.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      884 2023-03-10 12:07:40.000000 aprompt-3.0.0/docs/_build/html/_sources/customization/custom-widgets.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      729 2023-03-10 12:03:26.000000 aprompt-3.0.0/docs/_build/html/_sources/customization/directory-structure.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-03-14 14:43:26.000000 aprompt-3.0.0/docs/_build/html/_sources/customization/index.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      103 2023-03-22 15:08:36.000000 aprompt-3.0.0/docs/_build/html/_sources/extensions.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-03-22 14:36:18.000000 aprompt-3.0.0/docs/_build/html/_sources/index.md.txt
--rwxrwxrwx   0 root         (0) root         (0)     1349 2023-03-08 22:10:55.000000 aprompt-3.0.0/docs/_build/html/_sources/license.md.txt
--rwxrwxrwx   0 root         (0) root         (0)      360 2023-03-22 14:42:59.000000 aprompt-3.0.0/docs/_build/html/_sources/prompts.md.txt
--rwxrwxrwx   0 root         (0) root         (0)     1691 2023-03-13 15:05:55.000000 aprompt-3.0.0/docs/_build/html/_sources/quickstart.md.txt
--rwxrwxrwx   0 root         (0) root         (0)     1412 2023-03-09 18:02:08.000000 aprompt-3.0.0/docs/_build/html/_sources/testing.md.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:47.698877 aprompt-3.0.0/docs/_build/html/_static/
--rwxrwxrwx   0 root         (0) root         (0)    14813 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/_static/basic.css
--rwxrwxrwx   0 root         (0) root         (0)      313 2023-01-08 00:17:38.000000 aprompt-3.0.0/docs/_build/html/_static/check-solid.svg
--rwxrwxrwx   0 root         (0) root         (0)     9031 2023-01-08 00:17:38.000000 aprompt-3.0.0/docs/_build/html/_static/clipboard.min.js
--rwxrwxrwx   0 root         (0) root         (0)      411 2023-01-08 00:17:38.000000 aprompt-3.0.0/docs/_build/html/_static/copy-button.svg
--rwxrwxrwx   0 root         (0) root         (0)     2060 2023-01-08 00:17:38.000000 aprompt-3.0.0/docs/_build/html/_static/copybutton.css
--rwxrwxrwx   0 root         (0) root         (0)     8472 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/_static/copybutton.js
--rwxrwxrwx   0 root         (0) root         (0)     2698 2023-01-08 00:17:38.000000 aprompt-3.0.0/docs/_build/html/_static/copybutton_funcs.js
--rwxrwxrwx   0 root         (0) root         (0)     1266 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/debug.css
--rwxrwxrwx   0 root         (0) root         (0)     4472 2023-03-08 13:27:11.000000 aprompt-3.0.0/docs/_build/html/_static/doctools.js
--rwxrwxrwx   0 root         (0) root         (0)      420 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/_static/documentation_options.js
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-03-08 13:27:11.000000 aprompt-3.0.0/docs/_build/html/_static/file.png
--rwxrwxrwx   0 root         (0) root         (0)     4758 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/_static/language_data.js
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-03-08 13:27:11.000000 aprompt-3.0.0/docs/_build/html/_static/minus.png
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-03-08 13:27:11.000000 aprompt-3.0.0/docs/_build/html/_static/plus.png
--rwxrwxrwx   0 root         (0) root         (0)    21072 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/_static/pygments.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:47.981401 aprompt-3.0.0/docs/_build/html/_static/scripts/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/scripts/furo-extensions.js
--rwxrwxrwx   0 root         (0) root         (0)     5265 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/scripts/furo.js
--rwxrwxrwx   0 root         (0) root         (0)      187 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/scripts/furo.js.LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)    28242 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/scripts/furo.js.map
--rwxrwxrwx   0 root         (0) root         (0)    18215 2023-03-08 13:27:11.000000 aprompt-3.0.0/docs/_build/html/_static/searchtools.js
--rwxrwxrwx   0 root         (0) root         (0)     6034 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/skeleton.css
--rwxrwxrwx   0 root         (0) root         (0)     4712 2023-03-08 13:27:11.000000 aprompt-3.0.0/docs/_build/html/_static/sphinx_highlight.js
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:48.296980 aprompt-3.0.0/docs/_build/html/_static/styles/
--rwxrwxrwx   0 root         (0) root         (0)     5529 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/styles/furo-extensions.css
--rwxrwxrwx   0 root         (0) root         (0)     7809 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/styles/furo-extensions.css.map
--rwxrwxrwx   0 root         (0) root         (0)    48512 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/styles/furo.css
--rwxrwxrwx   0 root         (0) root         (0)    73326 2023-01-08 00:17:45.000000 aprompt-3.0.0/docs/_build/html/_static/styles/furo.css.map
--rwxrwxrwx   0 root         (0) root         (0)   114280 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/api.html
--rwxrwxrwx   0 root         (0) root         (0)    14756 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/changelog.html
--rwxrwxrwx   0 root         (0) root         (0)    15151 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/clean-up.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:48.377412 aprompt-3.0.0/docs/_build/html/contributing/
--rwxrwxrwx   0 root         (0) root         (0)    12997 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/contributing/index.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:48.709322 aprompt-3.0.0/docs/_build/html/customization/
--rwxrwxrwx   0 root         (0) root         (0)    13135 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/customization/custom-formatter.html
--rwxrwxrwx   0 root         (0) root         (0)    21555 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/customization/custom-prompt-engine.html
--rwxrwxrwx   0 root         (0) root         (0)    14632 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/customization/custom-widgets.html
--rwxrwxrwx   0 root         (0) root         (0)    13481 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/customization/directory-structure.html
--rwxrwxrwx   0 root         (0) root         (0)    13524 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/customization/index.html
--rwxrwxrwx   0 root         (0) root         (0)    23014 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/extensions.html
--rwxrwxrwx   0 root         (0) root         (0)    25142 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/genindex.html
--rwxrwxrwx   0 root         (0) root         (0)    15969 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/index.html
--rwxrwxrwx   0 root         (0) root         (0)    13704 2023-03-22 15:54:11.000000 aprompt-3.0.0/docs/_build/html/license.html
--rwxrwxrwx   0 root         (0) root         (0)      981 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/objects.inv
--rwxrwxrwx   0 root         (0) root         (0)    54712 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/prompts.html
--rwxrwxrwx   0 root         (0) root         (0)    13086 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/py-modindex.html
--rwxrwxrwx   0 root         (0) root         (0)    17376 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/quickstart.html
--rwxrwxrwx   0 root         (0) root         (0)    11607 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/search.html
--rwxrwxrwx   0 root         (0) root         (0)    22184 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/searchindex.js
--rwxrwxrwx   0 root         (0) root         (0)    15571 2023-03-22 15:54:12.000000 aprompt-3.0.0/docs/_build/html/testing.html
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-03-10 12:18:56.000000 aprompt-3.0.0/docs/api.md
--rwxrwxrwx   0 root         (0) root         (0)     1061 2023-03-08 22:01:20.000000 aprompt-3.0.0/docs/changelog.md
--rwxrwxrwx   0 root         (0) root         (0)      623 2023-03-10 15:13:59.000000 aprompt-3.0.0/docs/clean-up.md
--rwxrwxrwx   0 root         (0) root         (0)     1207 2023-03-22 15:53:58.000000 aprompt-3.0.0/docs/conf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:48.771656 aprompt-3.0.0/docs/contributing/
--rwxrwxrwx   0 root         (0) root         (0)      199 2023-03-08 22:36:19.000000 aprompt-3.0.0/docs/contributing/index.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:49.026572 aprompt-3.0.0/docs/customization/
--rwxrwxrwx   0 root         (0) root         (0)      225 2023-03-10 20:57:07.000000 aprompt-3.0.0/docs/customization/custom-formatter.md
--rwxrwxrwx   0 root         (0) root         (0)     2705 2023-03-14 14:53:08.000000 aprompt-3.0.0/docs/customization/custom-prompt-engine.md
--rwxrwxrwx   0 root         (0) root         (0)      884 2023-03-10 12:07:40.000000 aprompt-3.0.0/docs/customization/custom-widgets.md
--rwxrwxrwx   0 root         (0) root         (0)      729 2023-03-10 12:03:26.000000 aprompt-3.0.0/docs/customization/directory-structure.md
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-03-14 14:43:26.000000 aprompt-3.0.0/docs/customization/index.md
--rwxrwxrwx   0 root         (0) root         (0)      103 2023-03-22 15:08:36.000000 aprompt-3.0.0/docs/extensions.md
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-03-22 14:36:18.000000 aprompt-3.0.0/docs/index.md
--rwxrwxrwx   0 root         (0) root         (0)     1349 2023-03-08 22:10:55.000000 aprompt-3.0.0/docs/license.md
--rwxrwxrwx   0 root         (0) root         (0)      800 2023-03-08 13:46:51.000000 aprompt-3.0.0/docs/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:49.136327 aprompt-3.0.0/docs/media/
--rwxrwxrwx   0 root         (0) root         (0)    86590 2023-03-12 14:54:21.000000 aprompt-3.0.0/docs/media/prompt-choice.gif
--rwxrwxrwx   0 root         (0) root         (0)    39675 2023-03-12 14:47:07.000000 aprompt-3.0.0/docs/media/prompt-confirm.gif
--rwxrwxrwx   0 root         (0) root         (0)      360 2023-03-22 14:42:59.000000 aprompt-3.0.0/docs/prompts.md
--rwxrwxrwx   0 root         (0) root         (0)     1691 2023-03-13 15:05:55.000000 aprompt-3.0.0/docs/quickstart.md
--rwxrwxrwx   0 root         (0) root         (0)     1412 2023-03-09 18:02:08.000000 aprompt-3.0.0/docs/testing.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:49.278994 aprompt-3.0.0/examples/
--rwxrwxrwx   0 root         (0) root         (0)      659 2023-03-03 18:49:34.000000 aprompt-3.0.0/examples/poll.py
--rwxrwxrwx   0 root         (0) root         (0)      756 2023-03-10 12:26:15.000000 aprompt-3.0.0/examples/signup.py
--rwxrwxrwx   0 root         (0) root         (0)      431 2023-03-08 14:54:46.000000 aprompt-3.0.0/examples/using_argparse.py
--rwxrwxrwx   0 root         (0) root         (0)      121 2023-02-26 14:35:02.000000 aprompt-3.0.0/examples/yesno.py
--rwxrwxrwx   0 root         (0) root         (0)     1336 2023-03-22 15:53:24.000000 aprompt-3.0.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-03-22 16:54:51.236828 aprompt-3.0.0/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:42.728513 aprompt-3.0.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:49.689400 aprompt-3.0.0/src/aprompt/
--rwxrwxrwx   0 root         (0) root         (0)     6328 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:50.557263 aprompt-3.0.0/src/aprompt/__pycache__/
--rwxrwxrwx   0 root         (0) root         (0)     5485 2023-03-22 14:36:26.000000 aprompt-3.0.0/src/aprompt/__pycache__/__init__.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     1814 2023-03-16 11:18:29.000000 aprompt-3.0.0/src/aprompt/__pycache__/_cli.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     2388 2023-03-22 15:52:38.000000 aprompt-3.0.0/src/aprompt/__pycache__/_utils.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     1341 2023-03-22 14:36:26.000000 aprompt-3.0.0/src/aprompt/__pycache__/exceptions.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     2192 2023-03-22 14:36:26.000000 aprompt-3.0.0/src/aprompt/__pycache__/formatters.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     9974 2023-03-22 14:36:26.000000 aprompt-3.0.0/src/aprompt/__pycache__/prompts.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     1104 2023-03-22 14:36:26.000000 aprompt-3.0.0/src/aprompt/__pycache__/result.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)      950 2023-03-03 15:26:39.000000 aprompt-3.0.0/src/aprompt/__pycache__/utils.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     2783 2023-03-22 14:36:26.000000 aprompt-3.0.0/src/aprompt/__pycache__/widgets.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     1370 2023-03-22 15:07:55.000000 aprompt-3.0.0/src/aprompt/_utils.py
--rwxrwxrwx   0 root         (0) root         (0)      828 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:42.760983 aprompt-3.0.0/src/aprompt/ext/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:50.621501 aprompt-3.0.0/src/aprompt/ext/argparse/
--rwxrwxrwx   0 root         (0) root         (0)     2147 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/ext/argparse/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:50.683970 aprompt-3.0.0/src/aprompt/ext/argparse/__pycache__/
--rwxrwxrwx   0 root         (0) root         (0)     2770 2023-03-22 14:36:27.000000 aprompt-3.0.0/src/aprompt/ext/argparse/__pycache__/__init__.cpython-310.pyc
--rwxrwxrwx   0 root         (0) root         (0)     3125 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/formatters.py
--rwxrwxrwx   0 root         (0) root         (0)    12829 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/prompts.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-02-26 15:32:52.000000 aprompt-3.0.0/src/aprompt/py.typed
--rwxrwxrwx   0 root         (0) root         (0)      667 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/result.py
--rwxrwxrwx   0 root         (0) root         (0)     1287 2023-03-22 14:34:46.000000 aprompt-3.0.0/src/aprompt/widgets.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:49.968602 aprompt-3.0.0/src/aprompt.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     2540 2023-03-22 16:54:37.000000 aprompt-3.0.0/src/aprompt.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5484 2023-03-22 16:54:42.000000 aprompt-3.0.0/src/aprompt.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-03-22 16:54:37.000000 aprompt-3.0.0/src/aprompt.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      123 2023-03-22 16:54:37.000000 aprompt-3.0.0/src/aprompt.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-03-22 16:54:37.000000 aprompt-3.0.0/src/aprompt.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:50.841804 aprompt-3.0.0/tests/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-22 16:54:51.175251 aprompt-3.0.0/tests/__pycache__/
--rwxrwxrwx   0 root         (0) root         (0)     2558 2023-03-08 18:18:38.000000 aprompt-3.0.0/tests/__pycache__/test_confirm.cpython-310-pytest-7.2.1.pyc
--rwxrwxrwx   0 root         (0) root         (0)     2558 2023-03-22 15:23:51.000000 aprompt-3.0.0/tests/__pycache__/test_confirm.cpython-310-pytest-7.2.2.pyc
--rwxrwxrwx   0 root         (0) root         (0)     1791 2023-03-08 18:16:15.000000 aprompt-3.0.0/tests/__pycache__/test_meta.cpython-310-pytest-7.2.1.pyc
--rwxrwxrwx   0 root         (0) root         (0)     1791 2023-03-22 15:23:52.000000 aprompt-3.0.0/tests/__pycache__/test_meta.cpython-310-pytest-7.2.2.pyc
--rwxrwxrwx   0 root         (0) root         (0)     3136 2023-03-08 21:10:06.000000 aprompt-3.0.0/tests/__pycache__/test_number.cpython-310-pytest-7.2.1.pyc
--rwxrwxrwx   0 root         (0) root         (0)     3136 2023-03-22 15:23:52.000000 aprompt-3.0.0/tests/__pycache__/test_number.cpython-310-pytest-7.2.2.pyc
--rwxrwxrwx   0 root         (0) root         (0)     3011 2023-03-08 21:09:27.000000 aprompt-3.0.0/tests/__pycache__/test_pin.cpython-310-pytest-7.2.1.pyc
--rwxrwxrwx   0 root         (0) root         (0)     3011 2023-03-22 15:23:52.000000 aprompt-3.0.0/tests/__pycache__/test_pin.cpython-310-pytest-7.2.2.pyc
--rwxrwxrwx   0 root         (0) root         (0)      389 2023-03-08 18:18:33.000000 aprompt-3.0.0/tests/test_confirm.py
--rwxrwxrwx   0 root         (0) root         (0)      892 2023-03-08 18:09:35.000000 aprompt-3.0.0/tests/test_meta.py
--rwxrwxrwx   0 root         (0) root         (0)      808 2023-03-08 21:10:03.000000 aprompt-3.0.0/tests/test_number.py
--rwxrwxrwx   0 root         (0) root         (0)      719 2023-03-08 21:08:31.000000 aprompt-3.0.0/tests/test_pin.py
--rwxrwxrwx   0 root         (0) root         (0)      363 2023-03-22 15:06:45.000000 aprompt-3.0.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.626548 aprompt-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-04-22 12:09:39.000000 aprompt-3.0.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      177 2023-04-22 12:09:39.000000 aprompt-3.0.1/.readthedocs.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/.tox/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/.tox/py311/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-22 12:09:39.000000 aprompt-3.0.1/.tox/py311/.tox-info.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/.tox/py39/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-22 12:09:39.000000 aprompt-3.0.1/.tox/py39/.tox-info.json
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-04-22 12:09:39.000000 aprompt-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-04-22 13:13:22.626548 aprompt-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-04-22 12:09:39.000000 aprompt-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      487 2023-04-22 12:25:52.000000 aprompt-3.0.1/docs/api.md
+-rw-r--r--   0 root         (0) root         (0)      193 2023-04-22 12:50:42.000000 aprompt-3.0.1/docs/changelog.md
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/clean-up.md
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-04-22 13:09:44.000000 aprompt-3.0.1/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/docs/contributing/
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-22 12:42:04.000000 aprompt-3.0.1/docs/contributing/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/docs/customization/
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/customization/custom-formatter.md
+-rw-r--r--   0 root         (0) root         (0)     2704 2023-04-22 12:37:36.000000 aprompt-3.0.1/docs/customization/custom-prompt-engine.md
+-rw-r--r--   0 root         (0) root         (0)      884 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/customization/custom-widgets.md
+-rw-r--r--   0 root         (0) root         (0)      729 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/customization/directory-structure.md
+-rw-r--r--   0 root         (0) root         (0)      410 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/customization/index.md
+-rw-r--r--   0 root         (0) root         (0)      105 2023-04-22 13:06:44.000000 aprompt-3.0.1/docs/extensions.md
+-rw-r--r--   0 root         (0) root         (0)      399 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-22 12:42:42.000000 aprompt-3.0.1/docs/license.md
+-rw-r--r--   0 root         (0) root         (0)      800 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/docs/media/
+-rw-r--r--   0 root         (0) root         (0)    86590 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/media/prompt-choice.gif
+-rw-r--r--   0 root         (0) root         (0)    39675 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/media/prompt-confirm.gif
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/prompts.md
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-04-22 12:31:00.000000 aprompt-3.0.1/docs/quickstart.md
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-04-22 12:09:39.000000 aprompt-3.0.1/docs/testing.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/examples/
+-rw-r--r--   0 root         (0) root         (0)      659 2023-04-22 12:09:39.000000 aprompt-3.0.1/examples/poll.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-04-22 12:09:39.000000 aprompt-3.0.1/examples/signup.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-04-22 12:09:39.000000 aprompt-3.0.1/examples/using_argparse.py
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-22 12:09:39.000000 aprompt-3.0.1/examples/yesno.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-04-22 13:10:04.000000 aprompt-3.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 13:13:22.626548 aprompt-3.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/src/aprompt/
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/_utils.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/src/aprompt/ext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/src/aprompt/ext/argparse/
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/ext/argparse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/formatters.py
+-rw-r--r--   0 root         (0) root         (0)    13218 2023-04-22 13:04:49.000000 aprompt-3.0.1/src/aprompt/prompts.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/py.typed
+-rw-r--r--   0 root         (0) root         (0)      667 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/result.py
+-rw-r--r--   0 root         (0) root         (0)     1287 2023-04-22 12:09:39.000000 aprompt-3.0.1/src/aprompt/widgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/src/aprompt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3009 2023-04-22 13:13:22.000000 aprompt-3.0.1/src/aprompt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-22 13:13:22.000000 aprompt-3.0.1/src/aprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 13:13:22.000000 aprompt-3.0.1/src/aprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-22 13:13:22.000000 aprompt-3.0.1/src/aprompt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-22 13:13:22.000000 aprompt-3.0.1/src/aprompt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 13:13:22.616547 aprompt-3.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-22 12:09:39.000000 aprompt-3.0.1/tests/test_confirm.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-04-22 12:09:39.000000 aprompt-3.0.1/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-22 12:09:39.000000 aprompt-3.0.1/tests/test_number.py
+-rw-r--r--   0 root         (0) root         (0)      719 2023-04-22 12:09:39.000000 aprompt-3.0.1/tests/test_pin.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-22 12:09:39.000000 aprompt-3.0.1/tox.ini
```

### Comparing `aprompt-3.0.0/LICENSE` & `aprompt-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/PKG-INFO` & `aprompt-3.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aprompt
-Version: 3.0.0
+Version: 3.0.1
 Summary: Advanced Prompts
 License: MIT
-Project-URL: Documentation, https://phoenixr-codes.github.io/aprompt/
+Project-URL: Documentation, https://aprompt.readthedocs.io/
 Project-URL: Source Code, https://github.com/phoenixr-codes/aprompt/
 Keywords: form,input,prompt
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -16,22 +16,26 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
-aprompt - Advanced Prompts
-==========================
+aprompt - Advanced Prompt
+=========================
 
 Why use `input()` when you can go _advanced_?
 
 *aprompt* lets you prompt users in a neat way. It comes with a UI system
 and everything is customizable!
 
+![Demonstration](https://raw.githubusercontent.com/phoenixr-codes/aprompt/main/docs/media/prompt-choice.gif)
+
+[![Documentation Status](https://readthedocs.org/projects/aprompt/badge/?version=latest)](https://aprompt.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Features
 --------
 
 * ✅ Large set of built-in prompts.
 * ✅ Custom prompts
 * ✅ Custom themes
@@ -39,30 +43,30 @@
   [argparse](https://docs.python.org/3/library/argparse.html?highlight=argparse#module-argparse)
 * ✅ Test API
 
 
 Available Prompts
 -----------------
 
-While it is easily possible to create custom prompts. aprompt comes with
+While it is easily possible to create custom prompts, aprompt comes with
 a lot of useful prompts.
 
 * [x] Text
 * [x] Integer
 * [x] Confirmation
 * [x] PIN Code
-* [x] Sort[^1]
+* [x] Sort
 * [x] Choice
 * [x] Multiple Choice
 * [ ] Path
 * [ ] Datetime
 * [ ] Date
 * [ ] Time
 
-[^1]: This feature is unstable. Sorting upwards does not work.
+_Unchecked prompts are planned for the future_
 
 
 Basic Usage
 -----------
 
 ```python
 from aprompt import prompt
@@ -102,18 +106,20 @@
 
 
 Links
 -----
 
 * [🐍 Repo](https://github.com/phoenixr-codes/aprompt)
 * [📦 PyPI](https://pypi.org/project/aprompt)
-* 📖 Docs *(soon)*
+* [📖 Docs](https://aprompt.readthedocs.io/)
 
 
 ToDo
 ----
 
-* add path prompt as 
+* add path prompt (as extension) and document it
 * turn `match`es to `if-else`s
-* add demo file and add a GIF of it to the README
-* add GIFs to prompt engines docs
+* add demo file and add a GIF of it to the README (instead of only the choice variant)
+* add GIFs to all prompt engines docs
+* turn simple formatter into a class
 * add logo
+
```

### Comparing `aprompt-3.0.0/README.md` & `aprompt-3.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-aprompt - Advanced Prompts
-==========================
+aprompt - Advanced Prompt
+=========================
 
 Why use `input()` when you can go _advanced_?
 
 *aprompt* lets you prompt users in a neat way. It comes with a UI system
 and everything is customizable!
 
+![Demonstration](https://raw.githubusercontent.com/phoenixr-codes/aprompt/main/docs/media/prompt-choice.gif)
+
+[![Documentation Status](https://readthedocs.org/projects/aprompt/badge/?version=latest)](https://aprompt.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Features
 --------
 
 * ✅ Large set of built-in prompts.
 * ✅ Custom prompts
 * ✅ Custom themes
@@ -17,30 +21,30 @@
   [argparse](https://docs.python.org/3/library/argparse.html?highlight=argparse#module-argparse)
 * ✅ Test API
 
 
 Available Prompts
 -----------------
 
-While it is easily possible to create custom prompts. aprompt comes with
+While it is easily possible to create custom prompts, aprompt comes with
 a lot of useful prompts.
 
 * [x] Text
 * [x] Integer
 * [x] Confirmation
 * [x] PIN Code
-* [x] Sort[^1]
+* [x] Sort
 * [x] Choice
 * [x] Multiple Choice
 * [ ] Path
 * [ ] Datetime
 * [ ] Date
 * [ ] Time
 
-[^1]: This feature is unstable. Sorting upwards does not work.
+_Unchecked prompts are planned for the future_
 
 
 Basic Usage
 -----------
 
 ```python
 from aprompt import prompt
@@ -80,18 +84,20 @@
 
 
 Links
 -----
 
 * [🐍 Repo](https://github.com/phoenixr-codes/aprompt)
 * [📦 PyPI](https://pypi.org/project/aprompt)
-* 📖 Docs *(soon)*
+* [📖 Docs](https://aprompt.readthedocs.io/)
 
 
 ToDo
 ----
 
-* add path prompt as 
+* add path prompt (as extension) and document it
 * turn `match`es to `if-else`s
-* add demo file and add a GIF of it to the README
-* add GIFs to prompt engines docs
+* add demo file and add a GIF of it to the README (instead of only the choice variant)
+* add GIFs to all prompt engines docs
+* turn simple formatter into a class
 * add logo
+
```

### Comparing `aprompt-3.0.0/docs/Makefile` & `aprompt-3.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/docs/_build/html/_images/prompt-choice.gif` & `aprompt-3.0.1/docs/media/prompt-choice.gif`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/docs/_build/html/_images/prompt-confirm.gif` & `aprompt-3.0.1/docs/media/prompt-confirm.gif`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/clean-up.md.txt` & `aprompt-3.0.1/docs/clean-up.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,13 +12,28 @@
 
 username = prompt("Please enter your username.", text())
 CACHE.write_text(f"username={username}")
 
 try:
     password = prompt("Please enter your password.", text(hide=True))
 except SystemExit as exc:
-    CACHE.write_text("")
+    CACHE.write_text("")  # erease the cache
     raise exc
 
 CACHE.write_text(CACHE.read_text() + f"\npassword={password}")
+```
+
+Prompts can be configured to be exited with {kbd}`CTRL+D`. The differnce to
+exiting normally with {kbd}`CTRL+C` is that the program should not exit but
+instead move on to the next or previous prompt. This option is usually used to
+implement an undo operation.
+
+```python
+from pathlib import Path
+from aprompt import prompt
+from aprompt.exceptions import PromptExit
+from aprompt.prompts import text
+
+CACHE = Path("cache")
 
+# ... WIP ...
 ```
```

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/customization/custom-prompt-engine.md.txt` & `aprompt-3.0.1/docs/customization/custom-prompt-engine.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 linenos: true
 emphasize-lines: 6,7,8,9,16,17
 ---
 from aprompt import PromptEngine
 from aprompt.result import Result
 from readchar import keys as k
 
-def my_prompt(arguments) -> PromptEngine[result_type]:
+def my_prompt(arguments) -> PromptEngine[ResultType]:
     alert = False
     while True:
         key = yield [
             w.Alert() if alert else None,
             widget1,
             widget2,
             ...
```

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/customization/custom-widgets.md.txt` & `aprompt-3.0.1/docs/customization/custom-widgets.md`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/customization/directory-structure.md.txt` & `aprompt-3.0.1/docs/customization/directory-structure.md`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/license.md.txt` & `aprompt-3.0.1/docs/license.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 Conditions
 > * License and copyright notice
 
 Limitations
 > * Liability
 > * Warranty
 
+------------------------------------------------------------------------------
 
 ```text
 MIT License
 
 Copyright (c) 2023 Jonas da Silva
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/quickstart.md.txt` & `aprompt-3.0.1/docs/quickstart.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 This page will guide you through the installation process and the creation
 of your first prompt.
 
 ## Installation
 
 You can install aprompt with [pip](https://pip.pypa.io/en/stable/):
 
-```{code-block} text
----
-caption: Console
----
+```console
 pip install -U aprompt
 ```
 
 ## Basic Usage
 
 Each prompt consists of three main parts:
```

### Comparing `aprompt-3.0.0/docs/_build/html/_sources/testing.md.txt` & `aprompt-3.0.1/docs/testing.md`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/docs/conf.py` & `aprompt-3.0.1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 #####################
 # Project Information
 
 project = 'aprompt'
 copyright = '2023, phoenixR'
 author = 'phoenixR'
-release = '3.0.0'
+release = '3.0.1'
 
 
 ###############
 # Configuration
 
 extensions = [
     'sphinx.ext.autodoc',
```

### Comparing `aprompt-3.0.0/docs/make.bat` & `aprompt-3.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/examples/poll.py` & `aprompt-3.0.1/examples/poll.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/examples/signup.py` & `aprompt-3.0.1/examples/signup.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/pyproject.toml` & `aprompt-3.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aprompt"
-version = "3.0.0"
+version = "3.0.1"
 description = "Advanced Prompts"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = [
     "form",
     "input",
     "prompt",
@@ -36,15 +36,15 @@
     "myst-parser>=1.0",
     "Sphinx>=6.1",
     "sphinx-copybutton>=0.5",
 ]
 dev = ["mypy", "pytest"]
 
 [project.urls]
-"Documentation" = "https://phoenixr-codes.github.io/aprompt/"
+"Documentation" = "https://aprompt.readthedocs.io/"
 "Source Code" = "https://github.com/phoenixr-codes/aprompt/"
 
 [tool.mypy]
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
```

### Comparing `aprompt-3.0.0/src/aprompt/__init__.py` & `aprompt-3.0.1/src/aprompt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         The question to ask / The prompt text.
 
     prompt_fn
         The prompt engine.
 
     validate
         A callable returning ``True``/``False`` or an instance of
-        ``BaseException``/``None`` depending on the reult.
+        ``BaseException``/``None`` depending on the result.
 
         If the validation fails, the prompt will continue.
 
     formatter
         Defaults to :func:`aprompt.formatters.simple`.
 
     file
```

### Comparing `aprompt-3.0.0/src/aprompt/_utils.py` & `aprompt-3.0.1/src/aprompt/_utils.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/src/aprompt/exceptions.py` & `aprompt-3.0.1/src/aprompt/exceptions.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/src/aprompt/ext/argparse/__init__.py` & `aprompt-3.0.1/src/aprompt/ext/argparse/__init__.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/src/aprompt/formatters.py` & `aprompt-3.0.1/src/aprompt/formatters.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/src/aprompt/prompts.py` & `aprompt-3.0.1/src/aprompt/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 While the prompts are documented to return something they internally
 *yield* the final result. The documented result is actually returned by
 :func:`aprompt.prompt`.
 """
 
 from __future__ import annotations
 
-from collections.abc import Callable
+from collections.abc import Callable, Container
 from itertools import cycle, repeat
 from typing import Any, Literal, Optional, overload
 
 from readchar import key as k
 
 from aprompt import PromptEngine, widgets as w
 from aprompt.result import Result
@@ -216,34 +216,37 @@
                 alert = True
 
 
 @overload
 def choice(
     *choices: str,
     multiple: Literal[True],
-    require: Callable[[int], bool] | int | None = None,
+    require: Callable[[int], bool] | int | Container[int] | None = None,
 ) -> PromptEngine[list[str]]:
     ...
 
 
 @overload
 def choice(
     *choices: str, multiple: Literal[False] = False, require: None = None
 ) -> PromptEngine[str]:
     ...
 
 
 def choice(
     *choices: str,
     multiple: bool = False,
-    require: Callable[[int], bool] | int | None = None,
+    require: Callable[[int], bool] | int | Container[int] | None = None,
 ) -> PromptEngine[list[str]] | PromptEngine[str]:
     """Prompts for options.
 
     .. image:: media/prompt-choice.gif
+    
+    .. versionadded:: 3.0.1
+        ``require`` now accepts containers.
 
     Parameters
     ----------
     choices
         Options to choose from.
 
     multiple
@@ -256,14 +259,18 @@
             is set to ``True``.
 
         ``(int) → bool``
             A callable taking the amount of selected prompts as an
             integer as a single argument and returning a boolean
             whether to pass or deny the resut.
 
+        ``Container[int]``
+            A container (usually a ``range``) specifying possible amounts
+            that are required to be selected.
+
         ``int``
             An integer specifying the amount of options that are
             required to be selected.
 
         This parameter can be used as a shorthand for the
         ``validate`` parameter of the :func:`aprompt.prompt`
         function:
@@ -285,14 +292,17 @@
         w.Option(o, hover=not bool(i)) for i, o in enumerate(choices)
     ]
 
     if require is None:
         require = lambda _: True
     elif isinstance(require, int):
         require = lambda n: n == require
+    elif not callable(require):
+        # Container
+        require = lambda n: n in require  # type: ignore
 
     alert = False
     while True:
         key = yield [w.Alert() if alert else None, w.Options(options)]
         alert = False
 
         match key:
```

### Comparing `aprompt-3.0.0/src/aprompt/result.py` & `aprompt-3.0.1/src/aprompt/result.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/src/aprompt/widgets.py` & `aprompt-3.0.1/src/aprompt/widgets.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/src/aprompt.egg-info/PKG-INFO` & `aprompt-3.0.1/src/aprompt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: aprompt
-Version: 3.0.0
+Version: 3.0.1
 Summary: Advanced Prompts
 License: MIT
-Project-URL: Documentation, https://phoenixr-codes.github.io/aprompt/
+Project-URL: Documentation, https://aprompt.readthedocs.io/
 Project-URL: Source Code, https://github.com/phoenixr-codes/aprompt/
 Keywords: form,input,prompt
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
@@ -16,22 +16,26 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
-aprompt - Advanced Prompts
-==========================
+aprompt - Advanced Prompt
+=========================
 
 Why use `input()` when you can go _advanced_?
 
 *aprompt* lets you prompt users in a neat way. It comes with a UI system
 and everything is customizable!
 
+![Demonstration](https://raw.githubusercontent.com/phoenixr-codes/aprompt/main/docs/media/prompt-choice.gif)
+
+[![Documentation Status](https://readthedocs.org/projects/aprompt/badge/?version=latest)](https://aprompt.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Features
 --------
 
 * ✅ Large set of built-in prompts.
 * ✅ Custom prompts
 * ✅ Custom themes
@@ -39,30 +43,30 @@
   [argparse](https://docs.python.org/3/library/argparse.html?highlight=argparse#module-argparse)
 * ✅ Test API
 
 
 Available Prompts
 -----------------
 
-While it is easily possible to create custom prompts. aprompt comes with
+While it is easily possible to create custom prompts, aprompt comes with
 a lot of useful prompts.
 
 * [x] Text
 * [x] Integer
 * [x] Confirmation
 * [x] PIN Code
-* [x] Sort[^1]
+* [x] Sort
 * [x] Choice
 * [x] Multiple Choice
 * [ ] Path
 * [ ] Datetime
 * [ ] Date
 * [ ] Time
 
-[^1]: This feature is unstable. Sorting upwards does not work.
+_Unchecked prompts are planned for the future_
 
 
 Basic Usage
 -----------
 
 ```python
 from aprompt import prompt
@@ -102,18 +106,20 @@
 
 
 Links
 -----
 
 * [🐍 Repo](https://github.com/phoenixr-codes/aprompt)
 * [📦 PyPI](https://pypi.org/project/aprompt)
-* 📖 Docs *(soon)*
+* [📖 Docs](https://aprompt.readthedocs.io/)
 
 
 ToDo
 ----
 
-* add path prompt as 
+* add path prompt (as extension) and document it
 * turn `match`es to `if-else`s
-* add demo file and add a GIF of it to the README
-* add GIFs to prompt engines docs
+* add demo file and add a GIF of it to the README (instead of only the choice variant)
+* add GIFs to all prompt engines docs
+* turn simple formatter into a class
 * add logo
+
```

### Comparing `aprompt-3.0.0/tests/test_meta.py` & `aprompt-3.0.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/tests/test_number.py` & `aprompt-3.0.1/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `aprompt-3.0.0/tests/test_pin.py` & `aprompt-3.0.1/tests/test_pin.py`

 * *Files identical despite different names*

