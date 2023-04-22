# Comparing `tmp/gdtoolkit-4.0.0.tar.gz` & `tmp/gdtoolkit-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/godot-gdscript-toolkit/godot-gdscript-toolkit/dist/.tmp-bairnrmi/gdtoolkit-4.0.0.tar", last modified: Wed Mar  1 18:48:41 2023, max compression
+gzip compressed data, was "/home/runner/work/godot-gdscript-toolkit/godot-gdscript-toolkit/dist/.tmp-rer1ho88/gdtoolkit-4.0.1.tar", last modified: Sat Apr 22 08:51:12 2023, max compression
```

## Comparing `gdtoolkit-4.0.0.tar` & `gdtoolkit-4.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/common/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7462 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/class_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/const_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33810 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/expression_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/expression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/function_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/safety_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/statement_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/formatter/var_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/gd2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/gd2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/gd2py/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/gdradon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/gdradon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/gdradon/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/linter/
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/basic_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/class_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/design_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/format_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/if_return_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/misc_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/name_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/problem_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/linter/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/parser/comments.lark
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/parser/gdscript.lark
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/gdtoolkit/parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/gdtoolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 18:48:41.000000 gdtoolkit-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-01 18:48:32.000000 gdtoolkit-4.0.0/tests/test_ast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/class_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/const_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33975 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/expression_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/expression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/function_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/safety_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/statement_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/var_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/gd2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gd2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gd2py/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/gdradon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gdradon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gdradon/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/basic_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/class_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/design_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/format_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/if_return_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/misc_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/name_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/problem_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/comments.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/gdscript.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/tests/test_ast.py
```

### Comparing `gdtoolkit-4.0.0/LICENSE` & `gdtoolkit-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/PKG-INFO` & `gdtoolkit-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtoolkit
-Version: 4.0.0
+Version: 4.0.1
 Summary: Independent set of tools for working with GDScript - parser, linter and formatter
 Home-page: https://github.com/Scony/godot-gdscript-toolkit
 Author: Pawel Lampe
 Author-email: pawel.lampe@gmail.com
 License: MIT
 Keywords: GODOT,GDSCRIPT,PARSER,LINTER,FORMATTER
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gdtoolkit-4.0.0/README.md` & `gdtoolkit-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/common/ast.py` & `gdtoolkit-4.0.1/gdtoolkit/common/ast.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/common/utils.py` & `gdtoolkit-4.0.1/gdtoolkit/common/utils.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/__init__.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/__main__.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/annotation.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/annotation.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/block.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/block.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/class_statement.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/class_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,35 +30,23 @@
         "classname_stmt": _format_classname_statement,
         "classname_extends_stmt": _format_classname_extends_statement,
         "class_var_stmt": _format_var_statement,
         "const_stmt": format_const_statement,
         "docstr_stmt": _format_docstring_statement,
         "class_def": _format_class_statement,
         "func_def": _format_func_statement,
-        "static_func_def": partial(
-            _format_child_and_prepend_to_outcome, prefix="static "
+        "static_func_def": lambda s, c: _format_func_statement(
+            s.children[0], c, "static "
         ),
         "annotation": format_standalone_annotation,
         "property_body_def": format_property_body,
     }  # type: Dict[str, Callable]
     return handlers[statement.data](statement, context)
 
 
-def _format_child_and_prepend_to_outcome(
-    statement: Tree, context: Context, prefix: str
-) -> Outcome:
-    lines, last_processed_line = format_class_statement(statement.children[0], context)
-    first_line_no, first_line = lines[0]
-    return (
-        [(first_line_no, f"{context.indent_string}{prefix}{first_line.strip()}")]
-        + lines[1:],
-        last_processed_line,
-    )
-
-
 def _format_signal_statement(statement: Tree, context: Context) -> Outcome:
     if len(statement.children) == 1 or len(statement.children[1].children) == 0:
         return format_simple_statement(
             f"signal {statement.children[0].value}", statement, context
         )
     expression_context = ExpressionContext(
         f"signal {statement.children[0].value}",
@@ -163,31 +151,35 @@
         format_class_statement,
         context.create_child_context(last_processed_line_no),
     )
     formatted_lines += class_lines
     return (formatted_lines, last_processed_line_no)
 
 
-def _format_func_statement(statement: Tree, context: Context) -> Outcome:
+def _format_func_statement(
+    statement: Tree, context: Context, prefix: str = ""
+) -> Outcome:
     func_header = statement.children[0]
-    formatted_lines, last_processed_line_no = _format_func_header(func_header, context)
+    formatted_lines, last_processed_line_no = _format_func_header(
+        func_header, context, prefix
+    )
     func_lines, last_processed_line_no = format_block(
         statement.children[1:],
         format_func_statement,
         context.create_child_context(last_processed_line_no),
     )
     formatted_lines += func_lines
     return (formatted_lines, last_processed_line_no)
 
 
-def _format_func_header(statement: Tree, context: Context) -> Outcome:
+def _format_func_header(statement: Tree, context: Context, prefix: str) -> Outcome:
     name = statement.children[0].value
     has_return_type = len(statement.children) > 2
     expression_context = ExpressionContext(
-        f"func {name}",
+        f"{prefix}func {name}",
         get_line(statement),
         f" -> {statement.children[2].value}:" if has_return_type else ":",
         get_end_line(statement),
     )
     func_args = statement.children[1]
     return format_concrete_expression(func_args, expression_context, context)
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/comments.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/comments.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/const_statement.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/const_statement.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/constants.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/constants.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/context.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/context.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/exceptions.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/exceptions.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/expression.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,16 @@
         "asless_mdr_expr": _format_operator_chain_based_expression_to_multiple_lines,
         "asless_actual_neg_expr": lambda e, ec, c: _append_to_expression_context_and_pass(
             f"{expression_to_str(e.children[0])}", e.children[1], ec, c
         ),
         "asless_actual_bitw_not": lambda e, ec, c: _append_to_expression_context_and_pass(
             f"{expression_to_str(e.children[0])}", e.children[1], ec, c
         ),
+        "pow_expr": _format_operator_chain_based_expression_to_multiple_lines,
+        "asless_pow_expr": _format_operator_chain_based_expression_to_multiple_lines,
         "type_test": _format_operator_chain_based_expression_to_multiple_lines,
         "asless_type_test": _format_operator_chain_based_expression_to_multiple_lines,
         "actual_type_cast": _format_operator_chain_based_expression_to_multiple_lines,
         "await_expr": _format_await_expression_to_multiple_lines,
         "standalone_call": _format_call_expression_to_multiple_lines,
         "getattr_call": _collapse_getattr_tree_to_dot_chain_and_format_to_multiple_lines,
         "getattr": _collapse_getattr_tree_to_dot_chain_and_format_to_multiple_lines,
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/expression_to_str.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/expression_to_str.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         "asless_shift_expr": _operator_chain_based_expression_to_str,
         "arith_expr": _operator_chain_based_expression_to_str,
         "asless_arith_expr": _operator_chain_based_expression_to_str,
         "mdr_expr": _operator_chain_based_expression_to_str,
         "asless_mdr_expr": _operator_chain_based_expression_to_str,
         "asless_actual_neg_expr": lambda e: f"-{expression_to_str(e.children[1])}",
         "asless_actual_bitw_not": lambda e: f"~{expression_to_str(e.children[1])}",
+        "pow_expr": _operator_chain_based_expression_to_str,
+        "asless_pow_expr": _operator_chain_based_expression_to_str,
         "type_test": _operator_chain_based_expression_to_str,
         "asless_type_test": _operator_chain_based_expression_to_str,
         "actual_type_cast": _operator_chain_based_expression_to_str,
         "await_expr": lambda e: "{} {}".format(
             " ".join(t.value for t in e.children[:-1]),
             expression_to_str(e.children[-1]),
         ),
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/expression_utils.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/expression_utils.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/formatter.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/function_statement.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/function_statement.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/property.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/property.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/safety_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/safety_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 
     def asless_arith_expr(self, args):
         return Tree("arith_expr", args)
 
     def asless_mdr_expr(self, args):
         return Tree("mdr_expr", args)
 
+    def asless_pow_expr(self, args):
+        return Tree("pow_expr", args)
+
     def string(self, args):
         string_token = args[0]
         return expression_to_str(string_token)
 
     def signal_stmt(self, args):
         if len(args) > 1 and len(args[1].children) == 0:
             return Tree("signal_stmt", args[:-1])
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit/formatter/var_statement.py` & `gdtoolkit-4.0.1/gdtoolkit/formatter/var_statement.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/gd2py/__init__.py` & `gdtoolkit-4.0.1/gdtoolkit/gd2py/__init__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/gd2py/__main__.py` & `gdtoolkit-4.0.1/gdtoolkit/gd2py/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/gdradon/__main__.py` & `gdtoolkit-4.0.1/gdtoolkit/gdradon/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/__init__.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/__init__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/__main__.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/basic_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/basic_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/class_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/class_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/design_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/design_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             for statement in function.all_statements
             if statement.kind == "return_stmt"
         ]
         if len(returns) > threshold:
             problems.append(
                 Problem(
                     name="max-returns",
-                    description='Function "{}" has more than {} arguments'.format(
+                    description='Function "{}" has more than {} return statements'.format(
                         function.name, threshold
                     ),
                     line=get_line(returns[-1].lark_node),
                     column=get_column(returns[-1].lark_node),
                 )
             )
     return problems
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/format_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/format_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/if_return_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/if_return_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/misc_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/misc_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/linter/name_checks.py` & `gdtoolkit-4.0.1/gdtoolkit/linter/name_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/parser/__main__.py` & `gdtoolkit-4.0.1/gdtoolkit/parser/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit/parser/gdscript.lark` & `gdtoolkit-4.0.1/gdtoolkit/parser/gdscript.lark`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                   | const_stmt
                   | docstr_stmt
 ?compound_class_stmt: class_def
                     | property_body_def
                     | func_def
                     | "static" func_def -> static_func_def
 annotation: "@" NAME [annotation_args]
-annotation_args: "(" test_expr ("," test_expr)* [trailing_comma] ")"
+annotation_args: "(" [test_expr ("," test_expr)* [trailing_comma]] ")"
 
 pass_stmt: "pass"
 enum_stmt: enum_regular
          | enum_named
 enum_regular: "enum" enum_body
 enum_named: "enum" NAME enum_body
 enum_body: "{" [enum_element ("," enum_element)* [trailing_comma]] "}"
@@ -151,15 +151,15 @@
 ?dict_pattern_element: kv_pair_pattern
                      | atom_pattern
 kv_pair_pattern: test_pattern ":" test_pattern
 
 expr: type_cast
     | assnmnt_expr
 assnmnt_expr: attr_expr _assnmnt_op type_cast
-!_assnmnt_op: "=" | "+=" | "-=" | "*=" | "/=" | "%=" | "&=" | "|=" | "^=" | ">>=" | "<<="
+!_assnmnt_op: "=" | "+=" | "-=" | "*=" | "/=" | "%=" | "&=" | "|=" | "^=" | ">>=" | "<<=" | "**="
 ?type_cast: test_expr
           | actual_type_cast
 !?actual_type_cast: test_expr ("as" TYPE_HINT)+
 !?test_expr: or_test ["if" asless_or_test "else" asless_test_expr]
            | actual_type_cast "if" asless_or_test "else" asless_test_expr
 !?asless_test_expr: asless_or_test ["if" asless_or_test "else" asless_test_expr]
 !?or_test: and_test (("or" | "||") asless_and_test)*
@@ -199,19 +199,22 @@
           | actual_type_cast (("*" | "/" | "%") asless_neg_expr)+
 !?asless_mdr_expr: asless_neg_expr (("*" | "/" | "%") asless_neg_expr)*
 ?neg_expr: bitw_not
          | asless_actual_neg_expr
 !?asless_actual_neg_expr: "-" asless_neg_expr
 ?asless_neg_expr: asless_bitw_not
                 | asless_actual_neg_expr
-?bitw_not: type_test
+?bitw_not: pow_expr
          | asless_actual_bitw_not
 !?asless_actual_bitw_not: "~" asless_bitw_not
-?asless_bitw_not: asless_type_test
+?asless_bitw_not: asless_pow_expr
                 | asless_actual_bitw_not
+!?pow_expr: type_test ("**" asless_type_test)*
+          | actual_type_cast ("**" asless_type_test)+
+!?asless_pow_expr: asless_type_test ("**" asless_type_test)*
 !?type_test: await_expr ("is" TYPE_HINT)*
            | actual_type_cast ("is" TYPE_HINT)+
 !?asless_type_test: await_expr ("is" TYPE_HINT)*
 !?await_expr: ("await")* call_expr
 ?call_expr: attr_expr
           | NAME _call_arglist -> standalone_call
           | getattr _call_arglist -> getattr_call
@@ -253,15 +256,15 @@
 trailing_comma: ","
 dict: "{" [c_dict_element ("," c_dict_element)* [trailing_comma]] "}"
     | "{" [eq_dict_element ("," eq_dict_element)* [trailing_comma]] "}"
 c_dict_element: type_cast ":" type_cast
 eq_dict_element: NAME "=" type_cast
 
 TYPE: NAME ([" "] "." [" "] NAME)*
-TYPE_HINT: NAME ([" "] "." [" "] NAME)* ["[" NAME "]"]
+TYPE_HINT: NAME ([" "] "." [" "] NAME)* ["[" NAME ([" "] "." [" "] NAME)* "]"]
 NUMBER: ["+"|"-"] (FLOAT | INT)
 FLOAT: INT _EXP | DECIMAL _EXP?
 _EXP: ("e"|"E") SIGNED_INT
 SIGNED_INT: ["+"|"-"] INT
 DECIMAL: INT "." INT? | "." INT
 INT: DIGIT (DIGIT | "_")*
 DIGIT: "0".."9"
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit/parser/parser.py` & `gdtoolkit-4.0.1/gdtoolkit/parser/parser.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/gdtoolkit.egg-info/PKG-INFO` & `gdtoolkit-4.0.1/gdtoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtoolkit
-Version: 4.0.0
+Version: 4.0.1
 Summary: Independent set of tools for working with GDScript - parser, linter and formatter
 Home-page: https://github.com/Scony/godot-gdscript-toolkit
 Author: Pawel Lampe
 Author-email: pawel.lampe@gmail.com
 License: MIT
 Keywords: GODOT,GDSCRIPT,PARSER,LINTER,FORMATTER
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gdtoolkit-4.0.0/gdtoolkit.egg-info/SOURCES.txt` & `gdtoolkit-4.0.1/gdtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.0/setup.py` & `gdtoolkit-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="gdtoolkit",
-    version="4.0.0",
+    version="4.0.1",
     description="Independent set of tools for working with GDScript - parser, linter and formatter",
     keywords=["GODOT", "GDSCRIPT", "PARSER", "LINTER", "FORMATTER"],
     url="https://github.com/Scony/godot-gdscript-toolkit",
     author="Pawel Lampe",
     author_email="pawel.lampe@gmail.com",
     license="MIT",
     packages=[
@@ -30,15 +30,15 @@
         ]
     },
     include_package_data=True,
     install_requires=[
         "lark[regex]==1.1.5",
         "docopt-ng==0.8.1",
         "pyyaml>=5.1",
-        "radon>=5.1",
+        "radon==6.0.1",
     ],
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `gdtoolkit-4.0.0/tests/test_ast.py` & `gdtoolkit-4.0.1/tests/test_ast.py`

 * *Files identical despite different names*

