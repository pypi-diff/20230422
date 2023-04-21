# Comparing `tmp/commutation-0.0.7.tar.gz` & `tmp/commutation-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutation-0.0.7.tar", last modified: Fri Apr 21 21:07:11 2023, max compression
+gzip compressed data, was "commutation-0.1.0.tar", last modified: Fri Apr 21 21:41:50 2023, max compression
```

## Comparing `commutation-0.0.7.tar` & `commutation-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.569575 commutation-0.0.7/
--rw-r--r--   0 alaricsanders   (501) staff       (20)       43 2023-04-21 19:55:14.000000 commutation-0.0.7/.gitignore
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.568145 commutation-0.0.7/Examples/
--rw-r--r--   0 alaricsanders   (501) staff       (20)    22896 2023-04-21 19:59:01.000000 commutation-0.0.7/Examples/Demonstrations.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    25995 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/KKJ.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    89564 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/Ringflip.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1937 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/Spin Algebra.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    17703 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/Triangles.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    76632 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/hexamer.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)     8225 2023-04-21 19:16:47.000000 commutation-0.0.7/Examples/test.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.0.7/LICENSE
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 21:07:11.569339 commutation-0.0.7/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.0.7/README.md
--rw-r--r--   0 alaricsanders   (501) staff       (20)      725 2023-04-21 21:07:01.000000 commutation-0.0.7/pyproject.toml
--rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 21:07:11.569619 commutation-0.0.7/setup.cfg
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.564825 commutation-0.0.7/src/
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.568541 commutation-0.0.7/src/commutation/
--rw-r--r--   0 alaricsanders   (501) staff       (20)       63 2023-04-21 21:06:36.000000 commutation-0.0.7/src/commutation/__init__.py
--rw-r--r--   0 alaricsanders   (501) staff       (20)    27553 2023-04-21 19:16:47.000000 commutation-0.0.7/src/commutation/main.py
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:07:11.569117 commutation-0.0.7/src/commutation.egg-info/
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)      420 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/SOURCES.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/dependency_links.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)       12 2023-04-21 21:07:11.000000 commutation-0.0.7/src/commutation.egg-info/top_level.txt
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:41:50.994396 commutation-0.1.0/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       43 2023-04-21 19:55:14.000000 commutation-0.1.0/.gitignore
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:41:50.992864 commutation-0.1.0/Examples/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    23921 2023-04-21 21:25:53.000000 commutation-0.1.0/Examples/Demonstrations.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    25995 2023-04-21 19:16:47.000000 commutation-0.1.0/Examples/KKJ.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    89564 2023-04-21 19:16:47.000000 commutation-0.1.0/Examples/Ringflip.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1937 2023-04-21 19:16:47.000000 commutation-0.1.0/Examples/Spin Algebra.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    17703 2023-04-21 19:16:47.000000 commutation-0.1.0/Examples/Triangles.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    76632 2023-04-21 19:16:47.000000 commutation-0.1.0/Examples/hexamer.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     8225 2023-04-21 19:16:47.000000 commutation-0.1.0/Examples/test.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.1.0/LICENSE
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 21:41:50.994226 commutation-0.1.0/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.1.0/README.md
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      725 2023-04-21 21:41:23.000000 commutation-0.1.0/pyproject.toml
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 21:41:50.994434 commutation-0.1.0/setup.cfg
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:41:50.989767 commutation-0.1.0/src/
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:41:50.993326 commutation-0.1.0/src/commutation/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       63 2023-04-21 21:06:36.000000 commutation-0.1.0/src/commutation/__init__.py
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    27751 2023-04-21 21:41:06.000000 commutation-0.1.0/src/commutation/main.py
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 21:41:50.994024 commutation-0.1.0/src/commutation.egg-info/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 21:41:50.000000 commutation-0.1.0/src/commutation.egg-info/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      420 2023-04-21 21:41:50.000000 commutation-0.1.0/src/commutation.egg-info/SOURCES.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 21:41:50.000000 commutation-0.1.0/src/commutation.egg-info/dependency_links.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       12 2023-04-21 21:41:50.000000 commutation-0.1.0/src/commutation.egg-info/top_level.txt
```

### Comparing `commutation-0.0.7/Examples/Demonstrations.ipynb` & `commutation-0.1.0/Examples/Demonstrations.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9598088321124985%*

 * *Differences: {"'cells'": "{2: {'execution_count': 7, 'outputs': {0: {'output_type': 'stream', 'name': 'stdout', "*

 * *            "'text': ['a\\n', 'a\\n', 'b\\n', 'S^z_b\\n'], delete: ['ename', 'evalue', "*

 * *            "'traceback']}}, 'source': {insert: [(1, 'from fractions import Fraction\\n')]}}, 3: "*

 * *            "{'execution_count': 8}, 6: {'execution_count': 22, 'outputs': {0: {'text': {insert: "*

 * *            "[(1, '-\\\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d\\n'), (2, '-\\\\frac{15}{2} S^z_a "*

 * *            "S^z_b S^z_c S^z […]*

```diff
@@ -1,39 +1,47 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "1d603737",
+            "metadata": {},
+            "source": [
+                "This is a kind of 'cheat sheet' for using the module."
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "fcc3fa1e-3a41-4561-ae20-878d2f7bf187",
             "metadata": {},
             "source": [
                 "## Constructing `Operator`\n",
                 "Operators are the basic building blocks of `Expression`s. \n",
                 "these inherit `__eq__` from object, so they should *not* be recreated!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 7,
             "id": "bf301c99-8f00-4ed7-8ff3-e1712f1ab8b5",
             "metadata": {},
             "outputs": [
                 {
-                    "ename": "ModuleNotFoundError",
-                    "evalue": "No module named 'commutation'",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[0;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
-                        "Input \u001b[0;32mIn [2]\u001b[0m, in \u001b[0;36m<cell line: 1>\u001b[0;34m()\u001b[0m\n\u001b[0;32m----> 1\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mcommutation\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;241m*\u001b[39m\n\u001b[1;32m      3\u001b[0m \u001b[38;5;66;03m# Use the constructor\u001b[39;00m\n\u001b[1;32m      4\u001b[0m a \u001b[38;5;241m=\u001b[39m Operator(\u001b[38;5;124m'\u001b[39m\u001b[38;5;124ma\u001b[39m\u001b[38;5;124m'\u001b[39m)\n",
-                        "\u001b[0;31mModuleNotFoundError\u001b[0m: No module named 'commutation'"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "a\n",
+                        "a\n",
+                        "b\n",
+                        "S^z_b\n"
                     ]
                 }
             ],
             "source": [
                 "from commutation import *\n",
+                "from fractions import Fraction\n",
                 "\n",
                 "# Use the constructor\n",
                 "a = Operator('a')\n",
                 "print(a)\n",
                 "print(a.latex_string)\n",
                 "\n",
                 "b = Operator('b','S^z_b')\n",
@@ -44,15 +52,15 @@
                 "\n",
                 "# Operator can also be declared scalar\n",
                 "KA = Operator('KA','K_A',scalar=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 8,
             "id": "7e3b66b8-744a-4af4-8acb-e1ca5fcd836c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -76,99 +84,128 @@
                 "## Constructing `Term`\n",
                 "\n",
                 "A `Term` is a product of Operators and \"true\" scalars, i.e. `int` and `Fraction`.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 21,
+            "id": "1aed89cc",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "+1\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# A default Term is 1:\n",
+                "print(Term())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 22,
             "id": "8891e8ed-d43d-4730-84c4-2389207e3643",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "-15/2 a b c d\n",
-                        "+1\n",
-                        "-9 a S^z_b\n",
-                        "-9 S^z_a S^z_b\n"
+                        "-\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d\n",
+                        "-\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d\n"
                     ]
                 }
             ],
             "source": [
                 "# creating them with the constructor:\n",
                 "t = Term(-9,a,b,Fraction(5,6),c,d)\n",
                 "print(t)\n",
-                "\n",
-                "# A default Term is 1:\n",
-                "print(Term())\n",
-                "\n",
-                "# Terms are also naturally built when multiplying Operators\n",
-                "t = a*b*-9\n",
-                "\n",
                 "print(t.as_latex())\n",
                 "\n",
                 "# you can change the rendering of `a` on the fly:\n",
                 "a.latex_string = 'S^z_a'\n",
                 "print(t.as_latex())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 26,
+            "id": "9a32b837",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "-9 a b\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Terms are naturally built when multiplying Operators:\n",
+                "t = a*b*-9\n",
+                "print(t)\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
             "id": "abf04aaf-a6b6-4d93-9479-285e034a6c90",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "-9 a b\n",
+                        "-9 a c\n",
                         "-9 a c\n"
                     ]
                 }
             ],
             "source": [
                 "# Copying should be done with the copy constructor\n",
-                "# Assignment will only make a shallow copy\n",
                 "t2 = Term(t)\n",
                 "t2.ops[1] = c\n",
                 "print(t)\n",
                 "print(t2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 14,
             "id": "407c3bfc-be3d-4d53-ae33-c157de9f0ebf",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "-9 a b\n",
                         "-9 a c\n",
-                        "-9 a c\n"
+                        "-9 a c -9 a c\n"
                     ]
                 }
             ],
             "source": [
-                "### DON'T do this\n",
+                "### DON'T do this unless you mean to:\n",
+                "# Assignment makes a shallow copy\n",
                 "t2 = t\n",
                 "print(t2)\n",
                 "t2.ops[1] = c\n",
-                "print(t)\n",
-                "print(t2)"
+                "print(t, t2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 15,
             "id": "7e04aa1e-157a-4697-80ae-3c948b3b12ca",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -182,40 +219,55 @@
                 "\n",
                 "print(a*b == a*b)\n",
                 "print(a*b == b*a)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 16,
             "id": "73df0b0f-e33e-4d8d-99fc-852014935dd9",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[0, 4, 9]\n",
-                        "[1, 3]\n"
+                        "[0, 4, 9]\n"
                     ]
                 }
             ],
             "source": [
                 "# Terms are searchable:\n",
                 "tt = a*b*b*b*a*b*a*a*c*a*b\n",
-                "print(tt.findall(a*b))\n",
-                "\n",
-                "# This also avoids collisions:\n",
+                "print(tt.findall(a*b))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "id": "939c0019",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[1, 3]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Searching avoids collisions\n",
                 "tt = a*b*b*b*b*b*a*a*c*a*b\n",
                 "print(tt.findall(b*b))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 19,
             "id": "9f3b8ffa-2f9e-4720-b092-14d637518adf",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 \\zeta_3 \\zeta_1^* S^z_a +1 \\zeta_1 \\zeta_2^* S^z_b S^z_a $"
@@ -237,111 +289,133 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "\n",
-                "\n",
-                "z1 = Operator('z1',r'\\zeta_1')\n",
-                "z2 = Operator('z2',r'\\zeta_2')\n",
-                "z3 = Operator('z3',r'\\zeta_3')\n",
-                "\n",
-                "z1_bar = Operator('z1b',r'\\zeta_1^*')\n",
-                "z2_bar = Operator('z2b',r'\\zeta_2^*')\n",
-                "z3_bar = Operator('z3b',r'\\zeta_3^*')\n",
+                "z1 = Operator('z1',r'\\zeta_1',scalar=True)\n",
+                "z2 = Operator('z2',r'\\zeta_2', scalar=True)\n",
+                "z3 = Operator('z3',r'\\zeta_3', scalar=True)\n",
+                "\n",
+                "z1_bar = Operator('z1b',r'\\zeta_1^*', scalar=True)\n",
+                "z2_bar = Operator('z2b',r'\\zeta_2^*', scalar=True)\n",
+                "z3_bar = Operator('z3b',r'\\zeta_3^*', scalar=True)\n",
                 "\n",
                 "def conjugate(x):\n",
                 "     return x.replaceall((z1, z1_bar), (z2, z2_bar), (z3, z3_bar), (z1_bar, z1), (z2_bar, z2), (z3_bar, z3))\n",
                 "    \n",
                 "xpr = z3*z1_bar*a + z1*z2_bar*b*a\n",
                 "xpr.show()\n",
                 "xprbar=conjugate(xpr)\n",
-                "xprbar.show()\n",
-                "\n",
-                "\n",
-                "# replacements with Expression should be done on an Expression."
+                "xprbar.show()\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aa3c4085-5703-4243-a6ec-59ddbd45b458",
             "metadata": {},
             "source": [
                 "## Constructing `Expression`\n",
                 "An `Expression` is a sum of Terms."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 27,
             "id": "5dbf589b-7bcc-4115-9b0c-4656a58edf7c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "  +1\n",
                         "\n"
                     ]
-                },
+                }
+            ],
+            "source": [
+                "# A default `Expression` is 0: (renders as empty space)\n",
+                "print(Expression() + 1)\n",
+                "print(Expression())"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 28,
+            "id": "16c9dc01",
+            "metadata": {},
+            "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_b S^z_b S^z_c +1 S^z_b S^z_c +1 S^z_a S^z_b S^z_c $"
                         ],
                         "text/plain": [
                             "<IPython.core.display.Latex object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
-                },
+                }
+            ],
+            "source": [
+                "# Expressions can be constructed from multiple arguments:\n",
+                "x = Expression(a*b*b*c,b*c,a*b*c)\n",
+                "x.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 29,
+            "id": "ad897c37",
+            "metadata": {},
+            "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_b S^z_c +1 S^z_a S^z_b S^z_b S^z_c +1 S^z_b S^z_c $"
                         ],
                         "text/plain": [
                             "<IPython.core.display.Latex object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
-                },
+                }
+            ],
+            "source": [
+                "# or as sums of Terms:\n",
+                "x2 = a*b*c + a*b*b*c + b*c \n",
+                "x2.show()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 30,
+            "id": "51b6b123",
+            "metadata": {},
+            "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "True\n"
                     ]
                 }
             ],
             "source": [
-                "# A default `Expression` is 0: (renders as empty space)\n",
-                "print(Expression() + 1)\n",
-                "print(Expression())\n",
-                "\n",
-                "# Expressions can be constructed from multiple arguments:\n",
-                "x = Expression(a*b*b*c,b*c,a*b*c)\n",
-                "x.show()\n",
-                "\n",
-                "# or more naturally, using symbolic algebra:\n",
-                "x2 = a*b*c + a*b*b*c + b*c \n",
-                "x2.show()\n",
-                "\n",
-                "# equality is commutative:\n",
-                "print(x2 == x)\n"
+                "# equality is commutative with respect to rearrangements of the sum:\n",
+                "print(x2 == x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 33,
             "id": "f4abd87f-f63d-4359-ac16-8db3bdd7dccd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+\\frac{17}{8} S^z_a S^z_b -10 S^z_b S^z_b $"
@@ -353,32 +427,32 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\n"
+                        "  +1 a b\n"
                     ]
                 }
             ],
             "source": [
                 "# collect() collects like terms:\n",
                 "x = a*b + b*b + Fraction(9/8)*a*b + b*-11*b\n",
                 "x.collect()\n",
                 "x.show()\n",
                 "# and even cancels:\n",
-                "x = a*b + -1*a*b\n",
+                "x = 2*a*b + -1*a*b\n",
                 "x.collect()\n",
                 "print(x)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 34,
             "id": "a10421a8-fbf3-4adb-ad07-cec334b68700",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_b S^z_b S^z_b S^z_a S^z_c S^z_a S^z_a S^z_c S^z_a S^z_b +1 $"
@@ -395,26 +469,14 @@
                     "output_type": "stream",
                     "text": [
                         "  +1 a b b b a c a a c a b  +1\n",
                         "  +1 c b b a c a a c c  +1 c b b a c a a c d  +1 d b b a c a a c c  +1 d b b a c a a c d  +1\n",
                         "  +1 a b b b a c a a c a b  +1\n",
                         "  +1 a b b a c a a c c  +1 c b b a c a a c d  +1 d b b a c a a c c  +1 d b b a c a a c d  +1\n"
                     ]
-                },
-                {
-                    "data": {
-                        "text/latex": [
-                            "$+\\frac{1}{1024} S^z_a +1 $"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.Latex object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Expressions can be substituted into:\n",
                 "\n",
                 "tt = a*b*b*b*a*c*a*a*c*a*b\n",
                 "\n",
@@ -423,29 +485,50 @@
                 "\n",
                 "assert xx.terms[0].ops[0] == a\n",
                 "\n",
                 "y = xx.substitute(a*b,c+d)\n",
                 "print(xx)\n",
                 "print(y)\n",
                 "\n",
-                "# this method returns a deep copy\n",
+                "# substitute returns a deep copy\n",
                 "y.terms[0].ops[0] = a\n",
                 "print(xx)\n",
-                "print(y)\n",
-                "\n",
+                "print(y)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 35,
+            "id": "98cd9f0a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/latex": [
+                            "$+\\frac{1}{1024} S^z_a +1 $"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.Latex object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
                 "# multiple substitutions can be chained:\n",
                 "q = Fraction(1,4)\n",
                 "\n",
                 "z = xx.sub(b*b, q).sub(a*a,q).sub(c*c, q).sub(a*a,q).sub(b*b, q).sub(c*c,q)\n",
                 "z.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 36,
             "id": "62b991da-344a-42b6-b39d-f14e71dfd118",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -483,58 +566,66 @@
                         ],
                         "text/plain": [
                             "<IPython.core.display.Latex object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "+1 a * [  +10 b b  +4/5 c b b  +1 d b b  +1 c a a b b  ] =   +10 a b b  +4/5 a c b b  +1 a d b b  +1 a c a a b b\n",
-                        "[  +10 a  +4/5 a c  +1 a d  +1 a c a a  ] * +1 b b =   +10 a b b  +4/5 a c b b  +1 a d b b  +1 a c a a b b\n"
-                    ]
                 }
             ],
             "source": [
                 "# Coefficients of known terms can be pulled out\n",
                 "\n",
                 "xx = 7*a*b*b + Fraction(4,5)*a*c*b*b + a*d*b*b + a*c*a*a*b*b + 3*a*b*b\n",
                 "print(xx)\n",
                 "\n",
                 "y = xx.coefficient(a*c,'right')\n",
                 "y.show()\n",
                 "y = xx.coefficient(a*c)\n",
                 "y.show()\n",
                 "y = xx.coefficient(b*b)\n",
-                "y.show()\n",
-                "\n",
-                "\n",
+                "y.show()\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 37,
+            "id": "58bb68ce",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "+1 a * [  +10 b b  +4/5 c b b  +1 d b b  +1 c a a b b  ] =   +10 a b b  +4/5 a c b b  +1 a d b b  +1 a c a a b b\n",
+                        "[  +10 a  +4/5 a c  +1 a d  +1 a c a a  ] * +1 b b =   +10 a b b  +4/5 a c b b  +1 a d b b  +1 a c a a b b\n"
+                    ]
+                }
+            ],
+            "source": [
                 "# Factorisation of leading or trailing terms can be done without specifying which term to look for\n",
                 "\n",
                 "fr, ba = xx.factor('right')\n",
                 "print(str(fr) + ' * [' + str(ba) + '  ] = ' +str(fr*ba))\n",
                 "\n",
                 "fr, ba = xx.factor()\n",
-                "print('['+str(fr) + '  ] * ' + str(ba) + ' = ' +str(fr*ba))\n"
+                "print('['+str(fr) + '  ] * ' + str(ba) + ' = ' +str(fr*ba))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2b74fd70-48ae-4352-89d4-e090b30cb2e9",
             "metadata": {},
             "source": [
                 "## Constructing a CommutatorAlgebra"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 38,
             "id": "26390ab5-91ae-4681-89e2-1e3c11d96aaf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ca = CommutatorAlgebra()\n",
                 "\n",
                 "az = Operator('az','S^z_a')\n",
@@ -545,15 +636,15 @@
                 "ca.set_commutator(az,ap)(ap)\n",
                 "ca.set_commutator(az,am)(-1*am)\n",
                 "ca.set_commutator(ap,am)(2*az)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 39,
             "id": "56b15e04-5ee3-4321-b52f-1f8840ab27c0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^+_a S^-_a S^z_a S^z_a S^z_a -2 S^+_a S^-_a S^z_a S^z_a +1 S^+_a S^-_a S^z_a $"
@@ -574,17 +665,25 @@
                             "<IPython.core.display.Latex object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/opt/homebrew/lib/python3.10/site-packages/commutation/main.py:666: UserWarning: Non-scalar operator \"c\" is not in the commutator database, assuming it commutes...\n",
+                        "  warn(s)\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/latex": [
-                            "$+1 S^+_a S^-_a c S^-_a S^z_a -1 S^+_a S^-_a c S^-_a $"
+                            "$+1 S^+_a S^-_a S^z_c S^-_a S^z_a -1 S^+_a S^-_a S^z_c S^-_a $"
                         ],
                         "text/plain": [
                             "<IPython.core.display.Latex object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -600,15 +699,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# there are two modes: move_left and move_right\n",
-                "# Note that pathological commutators will make these fall into recursion loops, don't do this!\n",
+                "# Note that pathological commutators will make these fall into recursion loops...\n",
                 "\n",
                 "xpr = Expression(az*ap*az*az*am)\n",
                 "ca.move_right(xpr, az)\n",
                 "xpr.collect()\n",
                 "xpr.show()\n",
                 "\n",
                 "xpr = Expression(az*ap*az*az*am)\n",
@@ -627,15 +726,15 @@
                 "ca.move_right(xpr3, az)\n",
                 "xpr3.collect()\n",
                 "xpr3.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 40,
             "id": "22287386-63cb-469a-b5d7-dd86585501e0",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -657,22 +756,22 @@
                 "print(y)\n",
                 "y.collect()\n",
                 "print(y)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 42,
             "id": "1872487e-f075-4398-9d11-c0a3b39b6e3b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
-                            "$+1 K_A K_A a b c +1 K_A K_A b $"
+                            "$+1 K_A K_A S^z_a S^z_b S^z_c +1 K_A K_A S^z_b $"
                         ],
                         "text/plain": [
                             "<IPython.core.display.Latex object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -698,15 +797,15 @@
                 "print(trm)\n",
                 "trm.move_scalars()\n",
                 "print(trm)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 41,
             "id": "59921b95-cf5c-4506-899a-71f328d9c930",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_a S^z_a S^+_a S^-_a -2 S^z_a S^z_a S^+_a S^-_a +1 S^z_a S^+_a S^-_a $"
@@ -742,20 +841,20 @@
                 "xpr = Expression(az*ap*az*az*am)\n",
                 "# ca.move_right(xpr, az)\n",
                 "ca.move_left(xpr, az)\n",
                 "ca.move_left(xpr, az)\n",
                 "xpr.collect()\n",
                 "xpr.show()\n",
                 "\n",
-                "# answers are the same. Promising!"
+                "# answers are the same. Phew!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 43,
             "id": "faff4dab-283e-4f17-a9a9-ab76e5c6988f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 b c d a +1 -\\frac{7}{2} c d a -\\frac{33}{10} b c d +\\frac{11}{3} b d a +\\frac{11}{3} b b d d -\\frac{77}{6} d a -\\frac{77}{6} b d d -\\frac{7}{10} c d +\\frac{11}{15} b d -\\frac{77}{30} d $"
@@ -820,15 +919,15 @@
                 "x.show()\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 44,
             "id": "e61dc1ee-8319-4e89-85ed-775dfd2712ea",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 c b a a -3 c a a +2 c c a a -1 b a a +1 a a $"
@@ -863,53 +962,53 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7b99482e-94bd-4804-8eb0-1665d5eadab3",
             "metadata": {},
             "source": [
-                "# Working with `Expression`"
+                "## Working with `Expression`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 47,
             "id": "53e195f8-ab52-4aa4-8089-003211d707fe",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "(   +1 a b c  +1 a b b )*( +1 d f )\n",
-                        "(   +1 a b c  +1 a b b )*( +1 d f )\n",
-                        "( +1 a b )*(   +1 c d f  +1 b d f )\n"
+                        "x = (  +1 a b c  +1 a b b) * (+1 d f) \n",
+                        "x = (  +1 a b c  +1 a b b) * (+1 d f) \n",
+                        "x = (+1 a b) * (  +1 c d f  +1 b d f) \n"
                     ]
                 }
             ],
             "source": [
                 "f = Operator('f','S^z_f')\n",
                 "\n",
                 "x = a*b*c*d*f + a*b*b*d*f\n",
                 "fr, ba = x.factor()\n",
-                "print('(',fr, ')*(', ba,')')\n",
+                "print(f\"x = ({fr}) * ({ba}) \")\n",
                 "# (   +1 a b c  +1 a b b )*( +1 d f )\n",
                 "\n",
                 "fr, ba = x.factor('left')\n",
-                "print('(',fr, ')*(', ba,')')\n",
+                "print(f\"x = ({fr}) * ({ba}) \")\n",
                 "# (   +1 a b c  +1 a b b )*( +1 d f )\n",
                 "\n",
                 "fr, ba = x.factor('right')\n",
-                "print('(',fr, ')*(', ba,')')\n",
+                "print(f\"x = ({fr}) * ({ba}) \")\n",
                 "# ( +1 a b )*(   +1 c d f  +1 b d f )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 48,
             "id": "f496805b-59a1-490f-bcbe-abbb5fc7463a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
```

### Comparing `commutation-0.0.7/Examples/KKJ.ipynb` & `commutation-0.1.0/Examples/KKJ.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/Examples/Ringflip.ipynb` & `commutation-0.1.0/Examples/Ringflip.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/Examples/Spin Algebra.ipynb` & `commutation-0.1.0/Examples/Spin Algebra.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/Examples/Triangles.ipynb` & `commutation-0.1.0/Examples/Triangles.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/Examples/hexamer.ipynb` & `commutation-0.1.0/Examples/hexamer.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/Examples/test.ipynb` & `commutation-0.1.0/Examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/LICENSE` & `commutation-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/PKG-INFO` & `commutation-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutation
-Version: 0.0.7
+Version: 0.1.0
 Summary: A library for doing noncommutative operator algebra
 Author-email: Alaric Sanders <als217@cam.ac.uk>
 Project-URL: Homepage, https://github.com/Spuriosity1/Commutation/
 Project-URL: Bug Tracker, https://github.com/Spuriosity1/Commutation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `commutation-0.0.7/README.md` & `commutation-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `commutation-0.0.7/pyproject.toml` & `commutation-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "commutation"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Alaric Sanders", email="als217@cam.ac.uk" },
 ]
 description = "A library for doing noncommutative operator algebra"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commutation-0.0.7/src/commutation/main.py` & `commutation-0.1.0/src/commutation/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from fractions import Fraction
 from warnings import warn
-from IPython.display import display, Latex
 import copy as cp
 
+try:
+    import IPython.display as ipdisp
+except ImportError:
+    ipdisp=None
+    
+
 
 class Operator(object):
     """Represents (non-commutative) symbols. 
     Terms are built from lists of Operators.
     
     """
     def __init__(self, name, latex_string=None, scalar=False):
@@ -427,27 +432,30 @@
             
         return result
 
 
         
     def from_str(self, s):
         # cursed parser code, a problem for another day!
-        raise NotImplementedException
+        raise NotImplementedError
         
         
     def as_latex(self):
         s = ''
         for term in self.terms:
             s += term.as_latex() + ' '
         return s
         
     def show(self, max_len=200):
         if len(self.terms) > max_len:
             raise RuntimeError('Expression too long (override with expression.show(n), n is number of terms)')
-        display(Latex('$'+self.as_latex()+'$'))
+        try:
+            ipdisp.display(ipdisp.Latex('$'+self.as_latex()+'$'))
+        except AttributeError as e:
+            raise AttributeError("LaTeX rendering is only possible in a jupyter notebook.")
         
     def move_scalars(self, side='left'):
         for t in self.terms:
             t.move_scalars(side='left')
         
     def factor(self, side='left',x = None):
         # usage: factor (ABC + ABD) ---> AB, C+D
@@ -530,15 +538,15 @@
 #         self.terms.sort(reverse=reverse, key=compfuncs[rule])
         
     def sort(self, strategy='first'):
         #order the elements        
         self.collect()
         sorters = {
             'first': lambda tup: ' '.join([str(o) for o in tup.ops ]),
-            'last': lambda tup: ' '.join([str(o) for o in reversed(o.ops) ]),
+            'last': lambda tup: ' '.join([str(o) for o in reversed(tup.ops) ]),
             'multiplier': lambda tup : tup.multiplier
         }
         
         self.terms.sort(key=sorters[strategy])
                 
         
     def coefficient(self, term, side='left'):
```

### Comparing `commutation-0.0.7/src/commutation.egg-info/PKG-INFO` & `commutation-0.1.0/src/commutation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutation
-Version: 0.0.7
+Version: 0.1.0
 Summary: A library for doing noncommutative operator algebra
 Author-email: Alaric Sanders <als217@cam.ac.uk>
 Project-URL: Homepage, https://github.com/Spuriosity1/Commutation/
 Project-URL: Bug Tracker, https://github.com/Spuriosity1/Commutation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

