# Comparing `tmp/commutation-0.1.2.tar.gz` & `tmp/commutation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutation-0.1.2.tar", last modified: Fri Apr 21 22:19:17 2023, max compression
+gzip compressed data, was "commutation-0.1.3.tar", last modified: Fri Apr 21 22:49:15 2023, max compression
```

## Comparing `commutation-0.1.2.tar` & `commutation-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:19:17.046492 commutation-0.1.2/
--rw-r--r--   0 alaricsanders   (501) staff       (20)     6148 2023-04-21 20:57:24.000000 commutation-0.1.2/.DS_Store
--rw-r--r--   0 alaricsanders   (501) staff       (20)       43 2023-04-21 19:55:14.000000 commutation-0.1.2/.gitignore
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:19:17.044351 commutation-0.1.2/Examples/
--rw-r--r--   0 alaricsanders   (501) staff       (20)    23921 2023-04-21 21:25:53.000000 commutation-0.1.2/Examples/Demonstrations.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    25995 2023-04-21 19:16:47.000000 commutation-0.1.2/Examples/KKJ.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    89564 2023-04-21 19:16:47.000000 commutation-0.1.2/Examples/Ringflip.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1937 2023-04-21 19:16:47.000000 commutation-0.1.2/Examples/Spin Algebra.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    17703 2023-04-21 19:16:47.000000 commutation-0.1.2/Examples/Triangles.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    76632 2023-04-21 19:16:47.000000 commutation-0.1.2/Examples/hexamer.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)     8225 2023-04-21 19:16:47.000000 commutation-0.1.2/Examples/test.ipynb
--rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.1.2/LICENSE
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 22:19:17.046327 commutation-0.1.2/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1093 2023-04-21 19:16:47.000000 commutation-0.1.2/README.md
--rw-r--r--   0 alaricsanders   (501) staff       (20)      725 2023-04-21 22:19:10.000000 commutation-0.1.2/pyproject.toml
--rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 22:19:17.046531 commutation-0.1.2/setup.cfg
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:19:17.044530 commutation-0.1.2/src/
--rw-r--r--   0 alaricsanders   (501) staff       (20)     6148 2023-04-21 20:57:24.000000 commutation-0.1.2/src/.DS_Store
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:19:17.045556 commutation-0.1.2/src/commutation/
--rw-r--r--   0 alaricsanders   (501) staff       (20)      123 2023-04-21 22:17:01.000000 commutation-0.1.2/src/commutation/__init__.py
--rw-r--r--   0 alaricsanders   (501) staff       (20)     8169 2023-04-21 21:55:01.000000 commutation-0.1.2/src/commutation/commutatoralgebra.py
--rw-r--r--   0 alaricsanders   (501) staff       (20)    18836 2023-04-21 22:17:32.000000 commutation-0.1.2/src/commutation/expression.py
--rw-r--r--   0 alaricsanders   (501) staff       (20)      878 2023-04-21 22:09:15.000000 commutation-0.1.2/src/commutation/style.py
-drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:19:17.046132 commutation-0.1.2/src/commutation.egg-info/
--rw-r--r--   0 alaricsanders   (501) staff       (20)     1751 2023-04-21 22:19:16.000000 commutation-0.1.2/src/commutation.egg-info/PKG-INFO
--rw-r--r--   0 alaricsanders   (501) staff       (20)      512 2023-04-21 22:19:17.000000 commutation-0.1.2/src/commutation.egg-info/SOURCES.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 22:19:17.000000 commutation-0.1.2/src/commutation.egg-info/dependency_links.txt
--rw-r--r--   0 alaricsanders   (501) staff       (20)       12 2023-04-21 22:19:17.000000 commutation-0.1.2/src/commutation.egg-info/top_level.txt
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:49:15.138037 commutation-0.1.3/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     6148 2023-04-21 20:57:24.000000 commutation-0.1.3/.DS_Store
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       49 2023-04-21 22:34:09.000000 commutation-0.1.3/.gitignore
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:49:15.135314 commutation-0.1.3/Examples/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    23679 2023-04-21 22:44:28.000000 commutation-0.1.3/Examples/Demonstrations.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    25995 2023-04-21 19:16:47.000000 commutation-0.1.3/Examples/KKJ.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    89564 2023-04-21 19:16:47.000000 commutation-0.1.3/Examples/Ringflip.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     1843 2023-04-21 22:48:47.000000 commutation-0.1.3/Examples/Spin Algebra.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    17703 2023-04-21 19:16:47.000000 commutation-0.1.3/Examples/Triangles.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    76632 2023-04-21 19:16:47.000000 commutation-0.1.3/Examples/hexamer.ipynb
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    35150 2023-04-21 19:22:44.000000 commutation-0.1.3/LICENSE
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     3269 2023-04-21 22:49:15.137848 commutation-0.1.3/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     2611 2023-04-21 22:46:14.000000 commutation-0.1.3/README.md
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      202 2023-04-21 22:42:23.000000 commutation-0.1.3/TODO.md
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      725 2023-04-21 22:49:00.000000 commutation-0.1.3/pyproject.toml
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       38 2023-04-21 22:49:15.138080 commutation-0.1.3/setup.cfg
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:49:15.135630 commutation-0.1.3/src/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     6148 2023-04-21 20:57:24.000000 commutation-0.1.3/src/.DS_Store
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:49:15.136962 commutation-0.1.3/src/commutation/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      123 2023-04-21 22:17:01.000000 commutation-0.1.3/src/commutation/__init__.py
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     8169 2023-04-21 21:55:01.000000 commutation-0.1.3/src/commutation/commutatoralgebra.py
+-rw-r--r--   0 alaricsanders   (501) staff       (20)    18986 2023-04-21 22:48:03.000000 commutation-0.1.3/src/commutation/expression.py
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      967 2023-04-21 22:28:37.000000 commutation-0.1.3/src/commutation/style.py
+drwxr-xr-x   0 alaricsanders   (501) staff       (20)        0 2023-04-21 22:49:15.137634 commutation-0.1.3/src/commutation.egg-info/
+-rw-r--r--   0 alaricsanders   (501) staff       (20)     3269 2023-04-21 22:49:15.000000 commutation-0.1.3/src/commutation.egg-info/PKG-INFO
+-rw-r--r--   0 alaricsanders   (501) staff       (20)      500 2023-04-21 22:49:15.000000 commutation-0.1.3/src/commutation.egg-info/SOURCES.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)        1 2023-04-21 22:49:15.000000 commutation-0.1.3/src/commutation.egg-info/dependency_links.txt
+-rw-r--r--   0 alaricsanders   (501) staff       (20)       12 2023-04-21 22:49:15.000000 commutation-0.1.3/src/commutation.egg-info/top_level.txt
```

### Comparing `commutation-0.1.2/.DS_Store` & `commutation-0.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/Examples/Demonstrations.ipynb` & `commutation-0.1.3/Examples/Demonstrations.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.990089414044939%*

 * *Differences: {"'cells'": "{2: {'execution_count': 2}, 3: {'execution_count': 14}, 5: {'execution_count': 15}, "*

 * *            "6: {'execution_count': 16, 'outputs': {0: {'text': {insert: [(1, '-\\\\frac{15}{2} a "*

 * *            "S^z_b S^z_c S^z_d\\n')], delete: [1]}}, insert: [(1, OrderedDict([('data', "*

 * *            "OrderedDict([('text/latex', ['$-\\\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d$']), "*

 * *            "('text/plain', ['<IPython.core.display.Latex object>'])])), ('metadata', "*

 * *            "OrderedDict()), ('output_type' […]*

```diff
@@ -16,15 +16,15 @@
                 "## Constructing `Operator`\n",
                 "Operators are the basic building blocks of `Expression`s. \n",
                 "these inherit `__eq__` from object, so they should *not* be recreated!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 2,
             "id": "bf301c99-8f00-4ed7-8ff3-e1712f1ab8b5",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -52,15 +52,15 @@
                 "\n",
                 "# Operator can also be declared scalar\n",
                 "KA = Operator('KA','K_A',scalar=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 14,
             "id": "7e3b66b8-744a-4af4-8acb-e1ca5fcd836c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -84,15 +84,15 @@
                 "## Constructing `Term`\n",
                 "\n",
                 "A `Term` is a product of Operators and \"true\" scalars, i.e. `int` and `Fraction`.\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 15,
             "id": "1aed89cc",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -103,42 +103,55 @@
             "source": [
                 "# A default Term is 1:\n",
                 "print(Term())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 16,
             "id": "8891e8ed-d43d-4730-84c4-2389207e3643",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "-15/2 a b c d\n",
-                        "-\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d\n",
+                        "-\\frac{15}{2} a S^z_b S^z_c S^z_d\n",
                         "-\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d\n"
                     ]
+                },
+                {
+                    "data": {
+                        "text/latex": [
+                            "$-\\frac{15}{2} S^z_a S^z_b S^z_c S^z_d$"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.Latex object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "# creating them with the constructor:\n",
                 "t = Term(-9,a,b,Fraction(5,6),c,d)\n",
                 "print(t)\n",
                 "print(t.as_latex())\n",
                 "\n",
                 "# you can change the rendering of `a` on the fly:\n",
                 "a.latex_string = 'S^z_a'\n",
-                "print(t.as_latex())"
+                "print(t.as_latex())\n",
+                "show(t)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
+            "execution_count": 17,
             "id": "9a32b837",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -150,46 +163,46 @@
                 "# Terms are naturally built when multiplying Operators:\n",
                 "t = a*b*-9\n",
                 "print(t)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 18,
             "id": "abf04aaf-a6b6-4d93-9479-285e034a6c90",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "-9 a c\n",
+                        "-9 a b\n",
                         "-9 a c\n"
                     ]
                 }
             ],
             "source": [
                 "# Copying should be done with the copy constructor\n",
                 "t2 = Term(t)\n",
                 "t2.ops[1] = c\n",
                 "print(t)\n",
                 "print(t2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 19,
             "id": "407c3bfc-be3d-4d53-ae33-c157de9f0ebf",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "-9 a c\n",
+                        "-9 a b\n",
                         "-9 a c -9 a c\n"
                     ]
                 }
             ],
             "source": [
                 "### DON'T do this unless you mean to:\n",
                 "# Assignment makes a shallow copy\n",
@@ -197,15 +210,15 @@
                 "print(t2)\n",
                 "t2.ops[1] = c\n",
                 "print(t, t2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 20,
             "id": "7e04aa1e-157a-4697-80ae-3c948b3b12ca",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -219,15 +232,15 @@
                 "\n",
                 "print(a*b == a*b)\n",
                 "print(a*b == b*a)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 21,
             "id": "73df0b0f-e33e-4d8d-99fc-852014935dd9",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -239,15 +252,15 @@
                 "# Terms are searchable:\n",
                 "tt = a*b*b*b*a*b*a*a*c*a*b\n",
                 "print(tt.findall(a*b))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 22,
             "id": "939c0019",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -259,15 +272,15 @@
                 "# Searching avoids collisions\n",
                 "tt = a*b*b*b*b*b*a*a*c*a*b\n",
                 "print(tt.findall(b*b))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 23,
             "id": "9f3b8ffa-2f9e-4720-b092-14d637518adf",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 \\zeta_3 \\zeta_1^* S^z_a +1 \\zeta_1 \\zeta_2^* S^z_b S^z_a $"
@@ -301,31 +314,31 @@
                 "z2_bar = Operator('z2b',r'\\zeta_2^*', scalar=True)\n",
                 "z3_bar = Operator('z3b',r'\\zeta_3^*', scalar=True)\n",
                 "\n",
                 "def conjugate(x):\n",
                 "     return x.replaceall((z1, z1_bar), (z2, z2_bar), (z3, z3_bar), (z1_bar, z1), (z2_bar, z2), (z3_bar, z3))\n",
                 "    \n",
                 "xpr = z3*z1_bar*a + z1*z2_bar*b*a\n",
-                "xpr.show()\n",
+                "show(xpr)\n",
                 "xprbar=conjugate(xpr)\n",
-                "xprbar.show()\n"
+                "show(xprbar)\n"
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
-            "execution_count": 27,
+            "execution_count": 24,
             "id": "5dbf589b-7bcc-4115-9b0c-4656a58edf7c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -338,15 +351,15 @@
                 "# A default `Expression` is 0: (renders as empty space)\n",
                 "print(Expression() + 1)\n",
                 "print(Expression())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 25,
             "id": "16c9dc01",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_b S^z_b S^z_c +1 S^z_b S^z_c +1 S^z_a S^z_b S^z_c $"
@@ -358,20 +371,20 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Expressions can be constructed from multiple arguments:\n",
                 "x = Expression(a*b*b*c,b*c,a*b*c)\n",
-                "x.show()"
+                "show(x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 29,
+            "execution_count": 26,
             "id": "ad897c37",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_b S^z_c +1 S^z_a S^z_b S^z_b S^z_c +1 S^z_b S^z_c $"
@@ -383,20 +396,20 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# or as sums of Terms:\n",
                 "x2 = a*b*c + a*b*b*c + b*c \n",
-                "x2.show()"
+                "show(x2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 30,
+            "execution_count": 27,
             "id": "51b6b123",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -407,15 +420,15 @@
             "source": [
                 "# equality is commutative with respect to rearrangements of the sum:\n",
                 "print(x2 == x)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 28,
             "id": "f4abd87f-f63d-4359-ac16-8db3bdd7dccd",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+\\frac{17}{8} S^z_a S^z_b -10 S^z_b S^z_b $"
@@ -435,24 +448,24 @@
                     ]
                 }
             ],
             "source": [
                 "# collect() collects like terms:\n",
                 "x = a*b + b*b + Fraction(9/8)*a*b + b*-11*b\n",
                 "x.collect()\n",
-                "x.show()\n",
+                "show(x)\n",
                 "# and even cancels:\n",
                 "x = 2*a*b + -1*a*b\n",
                 "x.collect()\n",
                 "print(x)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 29,
             "id": "a10421a8-fbf3-4adb-ad07-cec334b68700",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_b S^z_b S^z_b S^z_a S^z_c S^z_a S^z_a S^z_c S^z_a S^z_b +1 $"
@@ -477,15 +490,15 @@
             ],
             "source": [
                 "# Expressions can be substituted into:\n",
                 "\n",
                 "tt = a*b*b*b*a*c*a*a*c*a*b\n",
                 "\n",
                 "xx = tt + 1\n",
-                "xx.show()\n",
+                "show(xx)\n",
                 "\n",
                 "assert xx.terms[0].ops[0] == a\n",
                 "\n",
                 "y = xx.substitute(a*b,c+d)\n",
                 "print(xx)\n",
                 "print(y)\n",
                 "\n",
@@ -493,15 +506,15 @@
                 "y.terms[0].ops[0] = a\n",
                 "print(xx)\n",
                 "print(y)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 30,
             "id": "98cd9f0a",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+\\frac{1}{1024} S^z_a +1 $"
@@ -515,20 +528,20 @@
                 }
             ],
             "source": [
                 "# multiple substitutions can be chained:\n",
                 "q = Fraction(1,4)\n",
                 "\n",
                 "z = xx.sub(b*b, q).sub(a*a,q).sub(c*c, q).sub(a*a,q).sub(b*b, q).sub(c*c,q)\n",
-                "z.show()"
+                "show(z)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 31,
             "id": "62b991da-344a-42b6-b39d-f14e71dfd118",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -575,24 +588,24 @@
             "source": [
                 "# Coefficients of known terms can be pulled out\n",
                 "\n",
                 "xx = 7*a*b*b + Fraction(4,5)*a*c*b*b + a*d*b*b + a*c*a*a*b*b + 3*a*b*b\n",
                 "print(xx)\n",
                 "\n",
                 "y = xx.coefficient(a*c,'right')\n",
-                "y.show()\n",
+                "show(y)\n",
                 "y = xx.coefficient(a*c)\n",
-                "y.show()\n",
+                "show(y)\n",
                 "y = xx.coefficient(b*b)\n",
-                "y.show()\n"
+                "show(y)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 37,
+            "execution_count": 32,
             "id": "58bb68ce",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -617,15 +630,15 @@
             "metadata": {},
             "source": [
                 "## Constructing a CommutatorAlgebra"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 4,
             "id": "26390ab5-91ae-4681-89e2-1e3c11d96aaf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ca = CommutatorAlgebra()\n",
                 "\n",
                 "az = Operator('az','S^z_a')\n",
@@ -636,105 +649,67 @@
                 "ca.set_commutator(az,ap)(ap)\n",
                 "ca.set_commutator(az,am)(-1*am)\n",
                 "ca.set_commutator(ap,am)(2*az)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 39,
+            "execution_count": 5,
             "id": "56b15e04-5ee3-4321-b52f-1f8840ab27c0",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/latex": [
-                            "$+1 S^+_a S^-_a S^z_a S^z_a S^z_a -2 S^+_a S^-_a S^z_a S^z_a +1 S^+_a S^-_a S^z_a $"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.Latex object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/latex": [
-                            "$+1 S^-_a S^z_a S^+_a S^z_a S^z_a -2 S^-_a S^z_a S^+_a S^z_a +2 S^z_a S^z_a S^z_a S^z_a -1 S^-_a S^+_a S^z_a S^z_a +1 S^-_a S^z_a S^+_a -4 S^z_a S^z_a S^z_a +2 S^-_a S^+_a S^z_a +2 S^z_a S^z_a -1 S^-_a S^+_a $"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.Latex object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "  +1 a\u207a a\u207b az az az  -2 a\u207a a\u207b az az  +1 a\u207a a\u207b az\n",
+                        "  +1 a\u207b az a\u207a az az  -2 a\u207b az a\u207a az  +2 az az az az  -1 a\u207b a\u207a az az  +1 a\u207b az a\u207a  -4 az az az  +2 a\u207b a\u207a az  +2 az az  -1 a\u207b a\u207a\n",
+                        "  +1 a\u207a a\u207b c a\u207b az  -1 a\u207a a\u207b c a\u207b\n",
+                        "  +1 a\u207a a\u207b KA a\u207b az  -1 a\u207a a\u207b KA a\u207b\n"
+                    ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/opt/homebrew/lib/python3.10/site-packages/commutation/main.py:666: UserWarning: Non-scalar operator \"c\" is not in the commutator database, assuming it commutes...\n",
+                        "/opt/homebrew/lib/python3.10/site-packages/commutation/commutatoralgebra.py:72: UserWarning: Non-scalar operator \"c\" is not in the commutator database, assuming it commutes...\n",
                         "  warn(s)\n"
                     ]
-                },
-                {
-                    "data": {
-                        "text/latex": [
-                            "$+1 S^+_a S^-_a S^z_c S^-_a S^z_a -1 S^+_a S^-_a S^z_c S^-_a $"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.Latex object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/latex": [
-                            "$+1 S^+_a S^-_a K_A S^-_a S^z_a -1 S^+_a S^-_a K_A S^-_a $"
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
                 "# there are two modes: move_left and move_right\n",
                 "# Note that pathological commutators will make these fall into recursion loops...\n",
                 "\n",
                 "xpr = Expression(az*ap*az*az*am)\n",
                 "ca.move_right(xpr, az)\n",
                 "xpr.collect()\n",
-                "xpr.show()\n",
+                "print(xpr) # +1 a\u207a a\u207b az az az  -2 a\u207a a\u207b az az  +1 a\u207a a\u207b az\n",
                 "\n",
                 "xpr = Expression(az*ap*az*az*am)\n",
                 "ca.move_left(xpr, am)\n",
                 "xpr.collect()\n",
-                "xpr.show()\n",
+                "print(xpr) # +1 a\u207b az a\u207a az az  -2 a\u207b az a\u207a az  +2 az az az az  -1 a\u207b a\u207a az az  +1 a\u207b az a\u207a  -4 az az az  +2 a\u207b a\u207a az  +2 az az  -1 a\u207b a\u207a\n",
                 "\n",
                 "# these will warn you if you add an unknown operator...\n",
                 "xpr2 = Expression(az*ap*am*c*am)\n",
                 "ca.move_right(xpr2, az)\n",
                 "xpr2.collect()\n",
-                "xpr2.show()\n",
+                "print(xpr2) #   +1 a\u207a a\u207b c a\u207b az  -1 a\u207a a\u207b c a\u207b\n",
                 "\n",
                 "# # ... but scalars are fine.\n",
                 "xpr3 = Expression(az*ap*am*KA*am)\n",
                 "ca.move_right(xpr3, az)\n",
                 "xpr3.collect()\n",
-                "xpr3.show()"
+                "print(xpr3) #   +1 a\u207a a\u207b KA a\u207b az  -1 a\u207a a\u207b KA a\u207b"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 40,
+            "execution_count": 35,
             "id": "22287386-63cb-469a-b5d7-dd86585501e0",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -756,15 +731,15 @@
                 "print(y)\n",
                 "y.collect()\n",
                 "print(y)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 42,
+            "execution_count": 36,
             "id": "1872487e-f075-4398-9d11-c0a3b39b6e3b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 K_A K_A S^z_a S^z_b S^z_c +1 K_A K_A S^z_b $"
@@ -785,27 +760,27 @@
                     ]
                 }
             ],
             "source": [
                 "# Scalar quantities can be bubbled to the front more efficiently:\n",
                 "x = a*b*KA*c*KA + KA*b*KA\n",
                 "x.move_scalars()\n",
-                "x.show()\n",
+                "show(x)\n",
                 "\n",
                 "\n",
                 "# this also works for Term:\n",
                 "trm = a*b*KA*c*KA\n",
                 "print(trm)\n",
                 "trm.move_scalars()\n",
                 "print(trm)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 37,
             "id": "59921b95-cf5c-4506-899a-71f328d9c930",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 S^z_a S^z_a S^z_a S^+_a S^-_a -2 S^z_a S^z_a S^+_a S^-_a +1 S^z_a S^+_a S^-_a $"
@@ -832,29 +807,29 @@
             ],
             "source": [
                 "# just a check\n",
                 "xpr = Expression(az*ap*az*az*am)\n",
                 "ca.move_right(xpr, az)\n",
                 "ca.move_left(xpr, az)\n",
                 "xpr.collect()\n",
-                "xpr.show()\n",
+                "show(xpr)\n",
                 "\n",
                 "xpr = Expression(az*ap*az*az*am)\n",
                 "# ca.move_right(xpr, az)\n",
                 "ca.move_left(xpr, az)\n",
                 "ca.move_left(xpr, az)\n",
                 "xpr.collect()\n",
-                "xpr.show()\n",
+                "show(xpr)\n",
                 "\n",
                 "# answers are the same. Phew!"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 38,
             "id": "faff4dab-283e-4f17-a9a9-ab76e5c6988f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 b c d a +1 -\\frac{7}{2} c d a -\\frac{33}{10} b c d +\\frac{11}{3} b d a +\\frac{11}{3} b b d d -\\frac{77}{6} d a -\\frac{77}{6} b d d -\\frac{7}{10} c d +\\frac{11}{15} b d -\\frac{77}{30} d $"
@@ -904,30 +879,30 @@
                 "cb.set_commutator(a,b)(Fraction(-7,2)*(a+b))\n",
                 "cb.set_commutator(a,c)(Fraction(11,3)*(a+b*d))\n",
                 "cb.set_commutator(a,d)(Fraction(1,5)*(d))\n",
                 "cb.set_commutator(b,c)(Fraction(11,5)*(a*b + c*a) )\n",
                 "\n",
                 "x = a*b*c*d + 1\n",
                 "cb.move_right(x,a)\n",
-                "x.show()\n",
+                "show(x)\n",
                 "\n",
                 "x = a*b*c*d + 1\n",
                 "cb.move_right(x,b)\n",
-                "x.show()\n",
+                "show(x)\n",
                 "\n",
                 "x = d*c*b*a + 1\n",
                 "cb.move_left(x,b)\n",
-                "x.show()\n",
+                "show(x)\n",
                 "\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 39,
             "id": "e61dc1ee-8319-4e89-85ed-775dfd2712ea",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/latex": [
                             "$+1 c b a a -3 c a a +2 c c a a -1 b a a +1 a a $"
@@ -952,30 +927,30 @@
                 "cb = CommutatorAlgebra()\n",
                 "\n",
                 "cb.set_commutator(a,b)(a+a*c)\n",
                 "cb.set_commutator(c,a)(a)\n",
                 "\n",
                 "x = a*c*a*b + 0\n",
                 "cb.move_right(x,a)\n",
-                "x.show()\n",
+                "show(x)\n",
                 "x.collect()\n",
                 "print(x)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7b99482e-94bd-4804-8eb0-1665d5eadab3",
             "metadata": {},
             "source": [
                 "## Working with `Expression`"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 40,
             "id": "53e195f8-ab52-4aa4-8089-003211d707fe",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1000,15 +975,15 @@
                 "fr, ba = x.factor('right')\n",
                 "print(f\"x = ({fr}) * ({ba}) \")\n",
                 "# ( +1 a b )*(   +1 c d f  +1 b d f )"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 48,
+            "execution_count": 41,
             "id": "f496805b-59a1-490f-bcbe-abbb5fc7463a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
```

### Comparing `commutation-0.1.2/Examples/KKJ.ipynb` & `commutation-0.1.3/Examples/KKJ.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/Examples/Ringflip.ipynb` & `commutation-0.1.3/Examples/Ringflip.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/Examples/Spin Algebra.ipynb` & `commutation-0.1.3/Examples/Spin Algebra.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759700176366843%*

 * *Differences: {"'cells'": "{0: {'execution_count': 1, 'source': {insert: [(0, 'from commutation import *\\n')], "*

 * *            "delete: [0]}}, 1: {'execution_count': 2, 'outputs': {0: {'text': ['  +2 S⁺ S⁻  -2 Sz  "*

 * *            "-4\\n']}}}, 2: {'source': ['c = Scalar()']}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3', 'name': 'python3'}, 'language_info': "*

 * *               "{'version': '3.10.9'}}"}*

```diff
@@ -1,26 +1,26 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 1,
             "id": "321ca776-398e-45a1-8cea-d75684f7cd14",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "+1 S^+ S^- S^z +1 S^- S^+ S^z +2 S^+ S^- +2 S^- S^+ \n",
                         "+2 S^+ S^- S^z +4 S^+ S^- -2 S^z S^z -4 S^z \n"
                     ]
                 }
             ],
             "source": [
-                "from Commutation import Operator, CommutatorAlgebra\n",
+                "from commutation import *\n",
                 "\n",
                 "Sz  = Operator('Sz','S^z')\n",
                 "Sup = Operator('S\u207a','S^+')\n",
                 "Sdn = Operator('S\u207b','S^-')\n",
                 "\n",
                 "ca = CommutatorAlgebra()\n",
                 "ca.set_commutator(Sz, Sup)(Sup)\n",
@@ -33,54 +33,56 @@
                 "# can further simplify\n",
                 "ca.move_left(x, Sup)\n",
                 "print(x.as_latex())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 2,
             "id": "27d74af8-773d-4112-a0d6-96d9f6e45edd",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "  +2 S^+ S^-  -2 S^z  -4\n"
+                        "  +2 S\u207a S\u207b  -2 Sz  -4\n"
                     ]
                 }
             ],
             "source": [
                 "print(x.coefficient(Sz))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "48d14018-8ccf-4730-8b34-f14d29cc19a9",
             "metadata": {},
             "outputs": [],
-            "source": []
+            "source": [
+                "c = Scalar()"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.10 64-bit",
+            "display_name": "Python 3",
             "language": "python",
-            "name": "python3910jvsc74a57bd050292dbb1f747f7151d445135d392af3138fb3c65386d17d9510cb605222b10b"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.10"
+            "version": "3.10.9"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `commutation-0.1.2/Examples/Triangles.ipynb` & `commutation-0.1.3/Examples/Triangles.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/Examples/hexamer.ipynb` & `commutation-0.1.3/Examples/hexamer.ipynb`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/LICENSE` & `commutation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/pyproject.toml` & `commutation-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "commutation"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Alaric Sanders", email="als217@cam.ac.uk" },
 ]
 description = "A library for doing noncommutative operator algebra"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `commutation-0.1.2/src/.DS_Store` & `commutation-0.1.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/src/commutation/commutatoralgebra.py` & `commutation-0.1.3/src/commutation/commutatoralgebra.py`

 * *Files identical despite different names*

### Comparing `commutation-0.1.2/src/commutation/expression.py` & `commutation-0.1.3/src/commutation/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         return self.latex_string
     
     def __eq__(self, other):
         if isinstance(other, (Operator, Term, Expression)):
             return self + other*-1 == 0
         return False
     
+# trivial overload
+class Scalar(Operator):
+    def __init__(self, name, latex_string=None):
+        super().__init__(name, latex_string, scalar=True)
 
 class Term(object):
     """Terms should be read as (Fraction * Term1*Terms2*...).
         These implement a noncommutative monoid structure for Term.
         
         Term.multiplier -> a Fraction, which absorbs scalar multiples of Terms.
         Term.ops        -> a list of Operators, which are understood as producted together.
```

### Comparing `commutation-0.1.2/src/commutation/style.py` & `commutation-0.1.3/src/commutation/style.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,8 +20,11 @@
         s = '\\frac{%d}{%d}' % (x.numerator, x.denominator)
     else:
         raise TypeError("show may only be called on Expression, Operator, Term, Fraction or int")
 
     try:
         ipdisp.display(ipdisp.Latex('$'+s+'$'))
     except AttributeError:
-        raise AttributeError("LaTeX rendering is only possible in a jupyter notebook.")
+        raise AttributeError("LaTeX rendering is only possible in a jupyter notebook.")
+    
+## Converts Expression, Term or Operator into Mathematica
+# def as_mathematica(x):
```

