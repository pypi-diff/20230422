# Comparing `tmp/mammath-0.1.7.tar.gz` & `tmp/mammath-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammath-0.1.7.tar", last modified: Wed Apr 20 07:42:07 2022, max compression
+gzip compressed data, was "mammath-0.1.8.tar", last modified: Sat Apr 22 17:24:32 2023, max compression
```

## Comparing `mammath-0.1.7.tar` & `mammath-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-04-20 07:42:07.635253 mammath-0.1.7/
--rw-rw-rw-   0        0        0     1019 2022-04-20 07:42:07.631254 mammath-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      525 2022-04-20 06:39:37.000000 mammath-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2022-04-20 07:42:07.615254 mammath-0.1.7/mammath/
--rw-rw-rw-   0        0        0     2839 2022-04-20 06:25:53.000000 mammath-0.1.7/mammath/ShuntingYardAlgorithm.py
--rw-rw-rw-   0        0        0    37055 2022-04-20 07:41:07.000000 mammath-0.1.7/mammath/__init__.py
--rw-rw-rw-   0        0        0    37055 2022-04-20 07:41:00.000000 mammath-0.1.7/mammath/mammath.py
-drwxrwxrwx   0        0        0        0 2022-04-20 07:42:07.631254 mammath-0.1.7/mammath.egg-info/
--rw-rw-rw-   0        0        0     1019 2022-04-20 07:42:07.000000 mammath-0.1.7/mammath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2022-04-20 07:42:07.000000 mammath-0.1.7/mammath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-20 07:42:07.000000 mammath-0.1.7/mammath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-04-20 07:42:07.000000 mammath-0.1.7/mammath.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-04-20 07:42:07.000000 mammath-0.1.7/mammath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-10-13 04:05:08.000000 mammath-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-20 07:42:07.635253 mammath-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      782 2022-04-20 07:41:21.000000 mammath-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:24:32.201384 mammath-0.1.8/
+-rw-rw-rw-   0        0        0      968 2023-04-22 17:24:32.200387 mammath-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2022-04-20 06:39:37.000000 mammath-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 17:24:32.190413 mammath-0.1.8/mammath/
+-rw-rw-rw-   0        0        0    47932 2023-04-22 17:17:39.000000 mammath-0.1.8/mammath/__init__.py
+-rw-rw-rw-   0        0        0    47932 2023-04-22 16:01:57.000000 mammath-0.1.8/mammath/mammath.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:24:32.199390 mammath-0.1.8/mammath.egg-info/
+-rw-rw-rw-   0        0        0      968 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 17:24:32.000000 mammath-0.1.8/mammath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-10-13 04:05:08.000000 mammath-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-22 17:24:32.201384 mammath-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      772 2023-04-22 16:00:25.000000 mammath-0.1.8/setup.py
```

### Comparing `mammath-0.1.7/PKG-INFO` & `mammath-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: mammath
-Version: 0.1.7
-Summary: A package that contains all you will need when you need to do complicated maths in python
+Version: 0.1.8
+Summary: A package that contains all you will need when you need to do maths in python
 Author: Vihaan Mathur & Harihar Rengan
-Author-email: vihaan.harihar341@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: vihaan.harihar314@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # mammath
@@ -19,8 +17,7 @@
 It is built upon several other modules including sys, tkinter, string, time, math, cmath, fractions, mpmath, keyboard, numpy, sympy, tabulate, re, matplotlib, and modules within them.
 
 You can have full detail on its functions using the help(mammath) syntax in the shell after importing the module.
 
 We hope Mammath is a useful and reliable asset.
 
 Thank you!
-
```

### Comparing `mammath-0.1.7/README.md` & `mammath-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `mammath-0.1.7/mammath/__init__.py` & `mammath-0.1.8/mammath/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,169 +15,153 @@
 import sys
 import keyboard
 import matplotlib.pyplot as plt
 from mpl_toolkits import mplot3d
 import inspect
 import re
 import mpmath
-##
-import re
 
-operatorsDict = {"**": 5, "*": 2, "/": 2, "+": 1, 'u': 6,  '^': 5, "%": 2, '': 4, "-": 1, }
-otherDict = {'u': 1}
+"""
+SHUNTING YARD ALGORITHM
+A safe replacement for eval
+"""
+
+operatorsDict = {"*": 2, "/": 2, "+": 1, "%": 2, '': 4, "-": 1, "^": 3, "**": 3}
 operators = operatorsDict.keys()
-operatorsBracket = list(operators)[:]
-operatorsBracket.append('(')
 
 def tokenize(inputExpression):
     return re.split("([()" + ''.join(operators) + "])", inputExpression.replace(" ", ""))
 
 def shunting_yard(inputExpression):
     queue = []
     stack = []
 
     tokens = tokenize(inputExpression)
     tokens = [x for x in tokens if x]
-
-    x = 0
-   
-       
-  #  print(tokens)
-
-    for x in range(0, len(tokens)):
-        if(tokens[x] == '-' and (x == 0 or tokens[x - 1] in operatorsBracket)):
-            tokens[x] = 'u'
-           
     for token in tokens:
         if(token not in operators and token != "(" and token != ")"):
             queue.append(token)
 
         if(token == "("):
             stack.append(token)
        
         if(token == ")"):
             while(len(stack) != 0 and stack[-1] != "("):
                 queue.append(stack.pop())
      
             stack.pop()
        
         if(token in operators):
-            if(token == 'u'):  
-                while(len(stack) != 0 and stack[-1] in operators and operatorsDict[stack[-1]] > operatorsDict[token]):
-                    queue.append(stack.pop())
-
-                stack.append(token)
-
-                continue
-           
             while(len(stack) != 0 and stack[-1] in operators and operatorsDict[stack[-1]] >= operatorsDict[token]):
                 queue.append(stack.pop())
 
             stack.append(token)
 
     while(len(stack) != 0):
         queue.append(stack.pop())
 
     return queue
 
 def evaluatePostfix(inputList):
     stack = []
-
-##    print(inputList)
+    
     for token in inputList:
         if(token not in operators):
             stack.append(token)
         else:
-            if(token == 'u'):
-##                print(stack)
-                operand = float(stack.pop())
-                stack.append(-1 * operand)
-
-                continue
             operand2 = float(stack.pop())
             operand1 = float(stack.pop())
-##            print("current ")
-##            print(operand1)
-##            print(operand2)
-##            print(token)
             if(token == "+"):
                 stack.append(operand1 + operand2)
 
             if(token == "-"):
                 stack.append(operand1 - operand2)
 
             if(token == "*"):
                 stack.append(operand1 * operand2)
 
             if(token == "/"):
                 stack.append(operand1 / operand2)
 
             if(token == '^'):
                 stack.append(operand1 ** operand2)
-
-##            print(stack)
                
     return stack[0]
 
 def evaluateExpression(inputExpression):
     return evaluatePostfix(shunting_yard(inputExpression))
 
+"""
+END OF SHUNTING YARD
+"""
+
+
+
+"""
+MATH TEACHERS
+"""
 
 def teach_me_trig():
-    print("welcome to the trig basics course!")
+    print("Welcome to the trigonometry basics course!")
     time.sleep(0.5)
-    print("a basics trigonometric formula is a^2 + b^2 = c^2, the pythagorean theorom")
+    print("One of the most fundamental formulas in trigonometry is the Pythagorean theorem - a^2 + b^2 = c^2, which allows you to find missing sides in a right angled triangle.")
     time.sleep(2)
     print("it works on all right angled triangles")
     time.sleep(1)
-    print(" soh cah toa will help you remember:")
+    print("Then, to calculate sides given an angle and one other side, SOHCAHTOA will help you remember the ratios:")
     time.sleep(0.5)
     print("sin = opposite/hypotenuse")
     time.sleep(1)
-    print("cos = adjacent over hypotenuse")
+    print("cos = adjacent/hypotenuse")
     time.sleep(1)
-    print("and tan = opposite over adjacent")
+    print("and tan = opposite/adjacent")
     time.sleep(1)
     ans = input("If one side of a triangle is 3 and another is 4, what is the hypotenuse? ")
     chances = 2
-    while ans not in ["hypotenuse = 5", "Hypotenuse = 5", "Hyp = 5, hyp = 5", "5", "hyp=5", "Hyp=5", "Hypotenuse=5", "hypotenuse=5"] and chances > 0:
-        print("not correct")
+    while ans.lower().replace(" ", "") not in ["hypotenuse=5", "hyp=5", "5", "five"] and chances > 0:
+        print("That is not correct. Please refer to the pythagorean theorem!")
         ans = input("If one side of a triangle is 3 and another is 4, what is the hypotenuse? ")
         chances = chances - 1
-    if ans in ["hypotenuse = 5", "Hypotenuse = 5", "Hyp = 5, hyp = 5", "5", "hyp=5", "Hyp=5", "Hypotenuse=5", "hypotenuse=5"]:
-        print("great job!")
+    if ans in ["hypotenuse=5", "hyp=5", "5", "five"]:
+        print("Great job! This is also a special case for right angled triangles and is known as a Pythagorean triplet.")
     else:
-        print("the answer was 5")
-    print("wikipedia, mathisfun, and other websites can help too")
-    print("thank you!")
+        print("The answer was 5. We needed to use the Pythagorean theorem which states that a^2 + b^2 = c^2, therefore, 3^2 + 4^2 = c^2, and c = 5")
+    print("Wikipedia, mathisfun, and other websites can help too")
+    print("Thank you!")
+    
 def teach_me_algebra():
-    print("welcome to the algebra basics course!")
+    print("Welcome to the algebra basics course!")
     time.sleep(0.5)
-    print("a you solve basic equations by moving variables to one side and numbers to the other")
+    print("In this basic algebra course, you will learn the basics of solving equations and working with variables.")
     time.sleep(2)
-    print("remember, change the operation when it crosses the equals sign")
-    time.sleep(1)
-    print(" - becomes +, + becomes -")
-    time.sleep(1)
-    print("x becomes /, / becomes x")
-    time.sleep(1)
-    print("and ^n becomes root(n), root(n) becomes ^n")
+    print("In order to solve one step equations, we will try to isolate all of the varaibles. This means that we want all instances of a variable on one side, and all regular numbers on another.")
+    time.sleep(3)
+    print("You will often be given an equation where you will have a few operations taking place on either side of the equation. If an 'x' variable is on a side with other numbers, we will perform the opposite operation that eliminates it from that side that it is on.")
+    time.sleep(3)
+    print("For instance, if we have x+3 = 5, we notice that we have a 3 on the same side as the x. In order to solve for x, we notice that we are adding a three, therefore, we will subtract a three to eliminate it from the x side. However, we need to remember to do the same thing on the other side of the equation. Therefore, the right side becomes 5 -3 = 2. x = 2.")
+    time.sleep(3)
+    print("In general, a + on one side becomes a - to eliminate it, a * becomes a /, a ^ becomes a root. ")
     time.sleep(1)
     ans = input("3x+5=8, what is x? ")
     chances = 2
-    while ans not in ["X = 1", "x = 1", "x=1", "X=1", "3"] and chances > 0:
-        print("not correct")
+    while ans.lower().replace(" ", "") not in ["x=1", "1", "one"] and chances > 0:
+        if chances == 2:
+            print("That is not correct. Notice that the 3x means 3*x.")
+        elif chances == 1:
+            print("That is not correct. First, subtract the 5 on both sides. As we have 3*x. We will need to divide both sides by three to solve for x.")
         ans = input("3x+5=8, what is x? ")
         chances = chances - 1
-    if ans in ["X = 1", "x = 1", "x=1", "X=1", "3"]:
-        print("great job!")
+    if ans in ["x=1", "1", "one"]:
+        print("Great job!")
     else:
-        print("the answer was 3")
-    print("wikipedia, mathisfun, and other websites can help too")
-    print("thank you!")
+        print("The answer was 1")
+        
+    print("Wikipedia, mathisfun, and other websites can help too")
+    print("Thank you!")
+    
 def teach_me_derivitives():
     print("welcome to the derivitives basics course!")
     time.sleep(0.5)
     print("a you solve basic derivitives by using a set of rules")
     time.sleep(0.5)
     print("use this link")
     time.sleep(1)
@@ -390,65 +374,64 @@
     val=""
 def clear():
     global val
     val =""
     data.set(val)
     
 
+"""
+END OF MATH TEACHERS
+"""
+
+
+def recLimit(a):
+    messagebox.askyesno("RECURSION SETTINGS", "Setting your recursion limit may slow your laptop or cause a crash. Proceed with caution. Do You wish to continue?")
 
     
+"""
+OPERATIONS
+"""
+
 def add(*args):
     return sum(args)
+
 def subtract(a, *args):
     return a - sum(args)
+
 def multiply(*args):
     x = 1
     y = 0
     while y < len(args):
         x = x*args[y]
         y+=1
     return x
+
 def divide(a, *args):
     return a / listMultiply(args)
-def listMultiply(List):
+
+#Multiplies all of the elements in a list
+def listMultiply(lis):
     x = 1
     y = 0
     while y < len(List):
         x = x*List[y]
         y+=1
     return x
-def power(a, *args):    
-    b = multiply(args)
-    x = a**(b)
-    if b < 1:
-        return root(a, 1/b)
-    else:
-        return x
-    
-def recLimit(a):
-    messagebox.askyesno("RECURSION SETTINGS", "Setting your recursion limit may slow your laptop or cause a crash. Proceed with caution. Do You wish to continue?")
+
+def power(base, exponent):
+    if exponent == 0:
+        return 1
+    if exponent > 0:
+        return (base * power(base, exponent - 1))
+    return 1 /(base * power(base, -exponent - 1))
+
 def sqrt(a):
     return math.sqrt(a)
 
-def addFraction(a, b):
-    ans = Fraction(a) + Fraction(b)
-    return str(ans)
-def subtractFraction(a, b):
-    ans = Fraction(a) - Fraction(b)
-    return str(ans)
-def multiplyFraction(a, b):
-    ans = Fraction(a) * Fraction(b)
-    return str(ans)
-def divideFraction(a, b):
-    ans = Fraction(a) / Fraction(b)
-    return str(ans)
-def simplifyFraction(a):
-    return str(Fraction(a).limit_denominator())
-
-def root(a, b):    #
+def root(a, b):    
     x = a**(1/b)
     try:
         y = round(x)
         if y-x <= 0.000000000000001:
             if x**(b) != a:
                 if b % 2 == 0 and a < 0:
                     z = str(abs(y)) + 'i'
@@ -483,69 +466,87 @@
     except:
         c = b/2
         t = cmath.sqrt(a)
         while c > 2:
              t = cmath.sqrt(t)
              c -= 1
         return t
-    
+
+def factorial(a):
+    x = 1
+    while a > 0:
+        x *=a
+        a -=1
+    return x
+
 def log(a, b):
     return math.log(a, b)
-def sf(a, b):
+def sigFig(a, b):
     rounded = round(a, b - int(math.floor(math.log10(abs(a)))) - 1)
     return rounded
 def absVal(a):
     return math.fabs(a)
 def remainder(a, b):
     return math.remainder(a, b)
-def toDegrees(a):
-    return math.degrees(a)
-def toRadians(a):
-    return math.radians(a)
 
 def HCF(a, b):
     a, b = max(a, b), min(a, b)
     while b!=0:
         a, b = b, a % b
     return a
 def LCM(a, b):
     return (a*b)/HCF(a, b)
+
+"""
+END OF OPERATIONS
+"""
+
+
+
+"""
+PRIME NUMBERS
+"""
+
 def primeFactors(n):
     while n % 2 == 0:
-            print(2)
-            n = n / 2  
+        print(2)
+        n = n / 2  
     for i in range(3,int(math.sqrt(n))+1,2):
-            while n % i== 0:
-                    print(i)
-                    n = n / i
+        while n % i== 0:
+            print(i)
+            n = n / i
     if n > 2:
-            print(n)
+        print(n)
 
-def factorial(a):
-    x = 1
-    while a > 0:
-        x *=a
-        a -=1
-    return x
 def checkPrime(num):
     x = False
     for i in range(2, num):
         if num % i == 0:
             x = True
     if x:
         return False
     return True
+
 def primeNumberPrinter(low, high):
     for num in range(low, high+1):
         if num > 1:
             for i in range(2, num):
                 if num % i == 0:
                     break
             else:
                 print(num)
+"""
+END OF PRIME NUMBERS
+"""
+
+
+"""
+NUMBER/SEQUENCE CHECKS
+"""
+
 def perfectSquare(num):
     root = math.sqrt(num)
 
     if math.trunc(root)-root==0:
         return True
     return False
 
@@ -581,74 +582,161 @@
             break
     return p == n
 
 def pentagonalPrinter(low, high):
     for i in range(low, high):
         if pentagonalCheck(i) == True:
             print(i)
-def fibonacci(n):
+
+"""
+END OF NUMBER/SEQUENCE CHECKS
+"""
+
+
+
+"""
+FIBONACCI
+"""
+
+def fibonacciBinet(n):
     x = (((((1+math.sqrt(5))/2)**n)-((((1-math.sqrt(5))/2)**n))))/math.sqrt(5)
     return round(x)
+def fibonacci(n):
+    n0, n = n, abs(n)
+    F = {}
+    
+    qinx = []  
+    qinx.append(n)
+    F[n] = -1
+    while qinx:
+        k = qinx.pop() >> 1
+        if k not in F:
+            F[k] = -1
+            qinx.append(k)
+        if (k + 1) not in F:
+            F[k+1] = -1
+            qinx.append(k + 1)
+    
+    F[0], F[1], F[2] = 0, 1, 1
+    keys_sorted = sorted(F.keys())
+    for k in keys_sorted[3:]:
+        k2 = k >> 1
+        f1, f2 = F[k2], F[k2 + 1]
+        if k % 2 == 0:
+            F[k] = 2 * f2 * f1 - f1 * f1
+        else:
+            F[k] = f2 * f2 + f1 * f1
+    
+    r = F[n]
+    if n0 < 0:
+        return negativeFib(n, r)
+    return r
+
 def fibonacciCheck(n):
     return perfectSquareCheck(5*n*n + 4) or perfectSquareCheck(5*n*n - 4)
 def fibonacciPrinter(low, high):
     for i in range(low, high+1):
         if fibonacciCheck(i) == True:
             print(i)
-            
-def divis2Check(num):
+
+"""
+END OF FIBONACCI
+"""
+
+
+
+"""
+DIVISIBILITY CHECKS
+"""
+
+def div2Check(num):
     if num % 2 == 0:
         return True
     else:
         return False
-def divis3Check(num):
+def div3Check(num):
     if num % 3 == 0:
         return True
     else:
         return False
-def divis4Check(num):
+def div4Check(num):
     if num % 4 == 0:
         return True
     else:
         return False
-def divis5Check(num):
+def div5Check(num):
     if num % 5 == 0:
         return True
     else:
         return False
-def divis6Check(num):
+def div6Check(num):
     if num % 6 == 0:
         return True
     else:
         return False
-def divis7Check(num):
+def div7Check(num):
     if num % 7 == 0:
         return True
     else:
         return False
-def divis8Check(num):
+def div8Check(num):
     if num % 8 == 0:
         return True
     else:
         return False
-def divis9Check(num):
+def div9Check(num):
     if num % 9 == 0:
         return True
     else:
         return False
-def divisCheck(num, num2):
+def divCheck(num, num2):
     if num % num2 == 0:
         return True
     else:
         return False
+
+"""
+END OF DIVISIBILITY CHECKS
+"""
+
+    
 def summate(n, a, b):
     return sum(nthRange(n, a, b))
 def product(n, a, b):
     return listMultiply(nthRange(n, a, b))
 
+def timesTables(n):
+    for i in range(1, n+1):
+        for j in range(i, (n*i)+i, i):
+            print(str(j) + " ", end="")
+        print("")
+
+def CoefficientsQuadratic(string):
+    string = "".join(" " if i == "x" or i == "+" else i for i in string)
+    string = string.replace("^2", " ")
+    return list(map(int, string.split()))
+"""
+FRACTIONS
+"""
+
+def addFraction(a, b):
+    ans = Fraction(a) + Fraction(b)
+    return str(ans)
+def subtractFraction(a, b):
+    ans = Fraction(a) - Fraction(b)
+    return str(ans)
+def multiplyFraction(a, b):
+    ans = Fraction(a) * Fraction(b)
+    return str(ans)
+def divideFraction(a, b):
+    ans = Fraction(a) / Fraction(b)
+    return str(ans)
+def simplifyFraction(a):
+    return str(Fraction(a).limit_denominator())
+
 def PercentagetoDecimal(percentage):
     return percentage / 100
 def PerToFrac(p):
     dec = p / 100
     fraction = Fraction(dec)
     return str(fraction)
 def PercentagetoFraction(percentage):
@@ -661,14 +749,29 @@
     return f * 100
 def DecimaltoPercentage(decimal):
     percentage = "{:.0%}".format(decimal)
     return str(percentage)
 def DecimaltoFraction(decimal):
     return str(Fraction(decimal).limit_denominator())
 
+"""
+END OF FRACTIONS
+"""
+
+
+
+"""
+GEOMETRY
+"""
+
+def validTriangle(s1, s2, s3):
+    if s1 + s2 >= s3 and s2 + s3 >= s1 and s1 + s3 >= s2:
+        return True
+    return False
+
 def triangleArea(l, w):
     return (l*w)/2
 def trapeziumArea(a, b, h):
     return (a+b)/h
 def paraHeight(a, b):
     return a/b
 def paraArea(b, h):
@@ -755,14 +858,19 @@
 def cot(a):
     return round(1/tan(a), 5)
 def gamma(a):
     return math.gamma(a)
 def lgamma(a):
     return math.lgamma(a)
 
+def toDegrees(a):
+    return math.degrees(a)
+def toRadians(a):
+    return math.radians(a)
+
 def pytheoromside(a, b):
     if a > c:
         a1 = a*a
         b1 = b*b
         c1 = a1 - b1
         c = math.sqrt(c1)
     else:
@@ -804,63 +912,60 @@
     tanpart = math.tan(intan)
     down = 4*tanpart
     ans = up/down
     return ans
 def pythagoreanTriplets(n):
   for b in range(n):
     for a in range(1, b):
-        c = math.sqrt( a * a + b * b)
+        c = math.sqrt(a * a + b * b)
         if c % 1 == 0:
             print(a, b, int(c))
 def pythagoreanTripletsCheck(a, b, c):
-    if (a ** 2) + (b ** 2) == (c ** 2):
-        return True
-    else:
-        return False
-    
-def speedCalc(d, t):
-    return d/t
-def distCalc(s, t):
-    return s*t
-def timeCalc(s, d):
-    return s*d
-    
+    return True if a * a + b * b == c * c else False
+
+"""
+END OF OF GEOMETRY
+"""
+
 def quadraticSolver(a,b,c):
     dis = b * b - 4 * a * c
     sqrt_val = math.sqrt(abs(dis))
     if dis > 0:
-            print(" real and different roots ")
-            print((-b + sqrt_val)/(2 * a))
-            print((-b - sqrt_val)/(2 * a))
+        print((-b + sqrt_val)/(2 * a))
+        print((-b - sqrt_val)/(2 * a))
     elif dis == 0:
-            print(" real and same roots")
-            print(-b / (2 * a))
+        print(-b / (2 * a))
     else:
-            print("Complex Roots")
-            print(- b / (2 * a), " + i", sqrt_val)
-            print(- b / (2 * a), " - i", sqrt_val)
+        print("Complex Roots")
+        print(- b / (2 * a), " + i", sqrt_val)
+        print(- b / (2 * a), " - i", sqrt_val)
 
-def sequenceChecker(a, b, c, d, e):
-    while 1 < 2:
+"""
+SEQUENCES
+"""
+
+def sequenceChecker(a, b, c):
+    while True:
         if b - a == c - b:
             print("Arithmetic")
             break
         if b / a == c / b or a / b == b / c:
             print("Geometric")
             break
         else:
             print("Quadratic")
             break
 
 def nthFinder(a, b):
     a = str(a)
     b = str(b)
     x = a.replace("n", b)
-    y = evaluateExpression(x)
+    y = eval(x)
     return y
+
 def nthRange(a, b, c):
     ls = []
     a = str(a)
     b = str(b)
     c = str(c)
     if int(b) > int(c):
         while int(c) < int(b)+1:
@@ -917,15 +1022,53 @@
         
     else:
         if before < 0:
             print("Nth Term:", str(dif) + "n" + str(before))
             print(str(term) + "th term:", str(newTerm)) 
         else:
             print("Nth Term:", str(dif) + "n" + " + " + str(before))
-            print(str(term) + "th term:", str(newTerm))  
+            print(str(term) + "th term:", str(newTerm))
+
+def removeDecimal(num):
+        if(num == int(num)):
+            return int(num)
+        return num
+    
+def Nth_Term_Quadratic(*series):
+    
+    r1d1 = series[1] - series[0]
+    r1d2 = series[2] - series[1] 
+    d2 = r1d2 - r1d1 
+    a = d2/2
+    b = r1d1 - 3 * a
+    c = series[0] - (a + b)
+    
+    a = removeDecimal(a) 
+    b = removeDecimal(b)
+    c = removeDecimal(c)
+    
+    quadraticDict = {0: "", 1: "n^2", -1: "-n^2"}
+    linearDict = {0: "", 1: "n", -1: "-n"}
+    constantDict = {0: ""}
+
+    quadraticTerm = "{}n^2".format(a) if (a != 0 and a != 1 and a != -1) else quadraticDict[a]
+    linearTerm = "{}n".format(b) if (b != 0 and b != 1 and b != -1) else linearDict[b]
+    constantTerm = "{}".format(c) if (c != 0) else constantDict[c]
+
+    bSign = "+" if b > 0 else ""
+    cSign = "+" if c > 0 else ""
+
+    print(quadraticTerm + bSign + linearTerm + cSign + constantTerm)
+    
+"""
+END OF SEQUENCES
+"""
+
+
+
 
 def percentageChange(a, b):
     if a == b:
         return 100.0
     try:
         return round(((b - a)/a)*100, 3)
     except ZeroDivisionError:
@@ -985,22 +1128,51 @@
         eq += str(args[int(i)]) + '*(n**' + str(i) + ') +'
         i = int(i)
         i += 1
         i = str(i)
     eq += '0'  
     return nthTable(eq, a, b)
 
-def F(m, a):
+
+
+"""
+FORMULAS
+"""
+#Force, Mass, Acceleration - F=ma
+def Force(m, a):
     return m*a
-def M(f, a):
+def Mass(f, a):
     return f/a
-def A(f, m):
+def Acceleration(f, m):
     return f/m
 
+#Speed, Distance, Time - S=d/t
+def Speed(d, t):
+    return d/t
+def Distance(s, t):
+    return s*t
+def Time(s, d):
+    return s*d
+"""
+END OF FORMULAS
+"""
+
+
+
+"""
+BASE CONVERSIONS
+"""
+
 def baseConverter(x, base):
+    if not isinstance(x, int):
+        if x.isdigit():
+            x = int(x)
+        else:
+            x = int("".join(map(str, [ord(i) for i in x])))
+            
     digs = string.digits + string.ascii_letters
     if x < 0:
         sign = -1
     elif x == 0:
         return digs[0]
     else:
         sign = 1
@@ -1018,30 +1190,40 @@
     digits.reverse()
     return "".join(digits)
 
 def IntToBinary(num):
     return bin(num)[2:]
 def BinaryToInt(num):
     return int(str(num), 2)
+
 def IntToHexa(num):
     return hex(num)[2:]
 def HexaToInt(num):
     return int(str(num, 2))
+
+def BinaryToHex(num):
+    return hex(int(str(num), 2))[2:]
+def HexToBinary(num):
+    return bin(int(str(num), 2))[2:]
+
 def binaryAdd(a, b):
     sum = BinaryToInt(a) + BinaryToInt(b)
     print("Binary:", IntToBinary(sum))
     print("Base 10:", sum)
+    
 def binarySubtract(a, b):
     sub = BinaryToInt(a) - BinaryToInt(b)
     print("Binary:", IntToBinary(sub))
     print("Base 10:", sub)
+    
 def binaryMultiply(a, b):
     mult = BinaryToInt(a) * BinaryToInt(b)
     print("Binary:", IntToBinary(mult))
     print("Base 10:", mult)
+    
 def binaryDivide(a, b):
     div = BinaryToInt(a) / BinaryToInt(b)
     print("Binary:", IntToBinary(div))
     print("Base 10:", div)
     
 def hexaAdd(a, b):
     sum = HexaToInt(a) + HexaToInt(b)
@@ -1056,14 +1238,20 @@
     print("Hexadecimal:", IntToHexa(mult))
     print("Base 10:", mult)
 def hexaDivide(a, b):
     div = HexaToInt(a) / HexaToInt(b)
     print("Hexadecimal:", IntToHexa(div))
     print("Base 10:", div)
 
+"""
+END OF BASE CONVERSIONS
+"""
+
+
+
 def constSearch(con):
     G = 6.67384*10**(-11)
     c = 2.99792458*10**(8)
     h = 6.626070040*10**(-34)
     k = 1.38064852*10**(-23)
     F = 9.648533289*10**(4)
     pi = 3.141592653589793238462643
@@ -1076,38 +1264,43 @@
     while x < 10:
         variable_name = [k for k, v in locals().items() if v == conlist[x]][0]
         if variable_name == con:
             constant = conlist[x]
             return constant
         x += 1
     return None
+
 def constTable():
     G = 6.67384*10**(-11)
     c = 2.99792458*10**(8)
     h = 6.626070040*10**(-34)
     k = 1.38064852*10**(-23)
     F = 9.648533289*10**(4)
     pi = 3.141592653589793238462643
     e = 2.718281828459045235360287
     π = pi
     phi = 1.618033988749894848204586
     φ = phi
     conlist = [["The gravitational constant", "G", G], ["The speed of light in vacuum", "c", c], ["Planck's constant", "h", h], ["Boltzmann's constant", "k", k], ["Faraday's constant", "F", F], ["e", "e", e], ["pi", "φ", π], ["Phi", "φ", φ]]
     headers = ["Name", "Symbol", "Value"]
-    thing = tabulate(conlist, headers = headers)
-    print(thing)
+    constants = tabulate(conlist, headers = headers)
+    print(constants)
+
 
+def f(fx, x, y):
+    if type(eval(fx)) == np.ndarray:
+        return eval(fx)
+
+#graph("2*x", "3*x")
 def graph(*args, lrangex=-10, urangex=10, lrangey=-10, urangey=10, graph_points=100, gridset=True, scaling=True, graph_title=None, xtitle=None, ytitle=None):
     i = 0
     x = np.linspace(lrangex, urangex, graph_points)
     while i < len(args):
-        if type(evaluateExpression(args[i])) == np.ndarray:
-            y = evaluateExpression(args[i])
-        else:
-            pass
+        if type(eval(args[i])) == np.ndarray:
+            y = eval(args[i])
         fig = plt.figure()
         ax = fig.add_subplot(1, 1, 1)
         ax.spines["left"].set_position("center")
         ax.spines["bottom"].set_position("zero")
         ax.spines["right"].set_color("none")
         ax.spines["top"].set_color("none")
         ax.xaxis.set_ticks_position("bottom")
@@ -1121,29 +1314,16 @@
     plt.grid(gridset)
     if lrangex or urangex != False:
         plt.xlim([lrangex,urangex])
     if lrangey or urangey != False:
         plt.ylim([lrangey,urangey])
     plt.show()
 
-def isInfinite(x):
-    return mpmath.isinf(x)
-def isFinite(x):
-    return mpmath.isfinite(x)
-def isInt(x, gaussian = False): 
-    return mpmath.isint(x, gaussian)
 
-def Zeta(s):
-    return zeta(s)
 
-def f(fx, x, y):
-    if type(evaluateExpression(fx)) == np.ndarray:
-        return evaluateExpression(fx)
-    else:
-        pass
     
 def graph3dcontour(*args, lrangex=-10, lrangey=-10, urangex=10, urangey=10, lrangez=-10, urangez=10, graph_points=1000, lablex='x', labley='y', lablez='z', graph_title=None, cmap='binary'):
     x = np.linspace(lrangex, urangex, graph_points)
     y = np.linspace(lrangey, urangey, graph_points)
     fig = plt.figure()
     ax = plt.axes(projection='3d')
     i = 0
@@ -1170,20 +1350,20 @@
     fig = plt.figure()
     ax = plt.axes(projection='3d')
     i = 0
     while i < len(args):
         lis = args[i]
         fz = lis[0]
         fy = lis[1]
-        if type(evaluateExpression(fz)) == np.ndarray:
-            zline = evaluateExpression(fz)
+        if type(eval(fz)) == np.ndarray:
+            zline = eval(fz)
         else:
             pass
-        if type(evaluateExpression(fy)) == np.ndarray:
-            yline = evaluateExpression(fy)
+        if type(eval(fy)) == np.ndarray:
+            yline = eval(fy)
         else:
             pass
         ax.plot3D(x, yline, zline, color)
         i+=1
     ax.set_xlabel(lablex)
     ax.set_ylabel(labley)
     ax.set_zlabel(lablez)
@@ -1213,32 +1393,265 @@
             ax.plot_surface(X, Y, Z, rstride=1, cstride=1,
                     cmap=fill, edgecolor='none')
         else:
             raise TypeError('Parameter "edgecolor" must be a boolean operator')
         i += 1
     ax.set_xlabel(lablex)
     ax.set_ylabel(labley)
-    ax.set_zlabel(lablez)
+    ax.set_zlabel(lablez)   
     ax.set_title(graph_title)
     if lrangez != False or urangez == False:
         ax.set_zlim(lrangez, urangez)
     if lrangex != False or urangex == False:
         ax.set_zlim(lrangex, urangex)
     if lrangey != False or urangey == False:
         ax.set_zlim(lrangey, urangey)
     return plt.show()
 
+def isInfinite(x):
+    return mpmath.isinf(x)
+def isFinite(x):
+    return mpmath.isfinite(x)
+def isInt(x, gaussian = False): 
+    return mpmath.isint(x, gaussian)
+
+def Zeta(s):
+    return zeta(s)
+
+
+"""
+CALCULUS
+"""
+
 def derivative(f_of, solvefor):
     return diff(f_of, solvefor)
 def secondDerivative(f_of, *args):
     return diff(f_of, args)
 def integral(f_of, solvefor):
     integral = integrate(f_of, solvefor)
     return integral
 def IndefIntegral(f_of, solvefor):
     integral = str(integrate(f_of, solvefor)) + " + C"
     return integral
 def defIntegral(f_of, solvefor, lowerbound, upperbound):
     return integrate((f_of), (solvefor, lowerbound, upperbound))
 def Limit(f_of, solvefor, to):
     return limit(f_of, solvefor, to)
+
+
+"""
+END OF CALCULUS
+"""
+
+
+
+"""
+LINEAR ALGEBRA
+"""
+def Adjacent2x2(matrix):
+    return np.array([[matrix[1][1], -matrix[0][1]], [-matrix[1][0], matrix[0][0]]]).tolist()
+
+def Adjacent3x3(matrix):
+    a = np.array([[(matrix[1][1]*matrix[2][2]) - (matrix[1][2]*matrix[2][1]),
+                   -((matrix[1][0]*matrix[2][2]) - (matrix[1][2]*matrix[2][0])),
+                   ((matrix[1][0]*matrix[2][1]) - (matrix[1][1]*matrix[2][0]))],
+                                    
+                  [-((matrix[0][1]*matrix[2][2]) - (matrix[0][2]*matrix[2][1])),
+                    ((matrix[0][0]*matrix[2][2]) - (matrix[0][2]*matrix[2][0])),
+                    -((matrix[0][0]*matrix[2][1]) - (matrix[0][1]*matrix[2][0]))],
+                                    
+                  [((matrix[0][1]*matrix[1][2]) - (matrix[0][2]*matrix[1][1])),
+                   -((matrix[0][0]*matrix[1][2]) - (matrix[0][2]*matrix[1][0])),
+                    ((matrix[0][0]*matrix[1][1]) - (matrix[0][1]*matrix[1][0]))]])
+
+    return np.transpose(a)
+
+def DiagonalSum(mat):
+    left = 0
+    right = 0
+    for i in range(0, len(mat)):
+        left += mat[i][i]
+        right += mat[i][len(mat) - i - 1]
+    total = left + right
+    if len(mat) % 2 != 0:
+        return total - (mat[len(mat) // 2][len(mat) // 2])
+    return total
+
+def solveEquations(*equations):              
+    equations = list(equations)
+    for i in range(0, len(equations)):
+        equations[i] = equations[i].replace(" ", "")
+        
+    eqs = []
+    varis = set()
+    for k in range(len(equations)):
+        equations[k] = equations[k].replace('-','+-')
+        eqDict = dict()
+        sides = equations[k].split('=')
+        termsLeft = sides[0].split('+')
+        termsRight = sides[1].split('+')
+        for term in termsLeft:
+            if term != '':
+                if term.isnumeric():
+                    if 'constant' in eqDict:
+                        eqDict['constant'] += -int(term)
+                    else:
+                        eqDict['constant'] = -int(term)
+                    continue
+                elif not '-' in term:
+                    if term.isalpha():
+                        coeff = 1
+                        vari = term
+                    else:
+                        l = 0
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = int(term[:l])
+                        vari = term[l:]
+                else:
+                    if term[1:].isnumeric():
+                        if 'constant' in eqDict:
+                            eqDict['constant'] += -int(term)
+                        else:
+                            eqDict['constant'] = -int(term)
+                        continue
+                    elif term[1:].isalpha():
+                        coeff = -1
+                        vari = term[1:]
+                    else:
+                        l = 1
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = -int(term[1:l])
+                        vari = term[l:]
+                varis.add(vari)
+                if vari in eqDict:
+                    eqDict[vari] += coeff
+                else:
+                    eqDict[vari] = coeff
+        for term in termsRight:
+            if term != '':
+                if term.isnumeric():
+                    if 'constant' in eqDict:
+                        eqDict['constant'] += int(term)
+                    else:
+                        eqDict['constant'] = int(term)
+                    continue
+                elif not '-' in term:
+                    if term.isalpha():
+                        coeff = -1
+                        vari = term
+                    else:
+                        l = 0
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = -int(term[:l])
+                        vari = term[l:]
+                else:
+                    if term[1:].isnumeric():
+                        if 'constant' in eqDict:
+                            eqDict['constant'] += int(term)
+                        else:
+                            eqDict['constant'] = int(term)
+                        continue
+                    if term[1:].isalpha():
+                        coeff = 1
+                        vari = term[1:]
+                    else:
+                        l = 1
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = int(term[1:l])
+                        vari = term[l:]
+                varis.add(vari)
+                if vari in eqDict:
+                    eqDict[vari] += coeff
+                else:
+                    eqDict[vari] = coeff
+        if not 'constant' in eqDict:
+            eqDict['constant'] = 0
+        eqs.append(eqDict)
+    if len(eqs) < len(varis):
+        return None
+    varis = sorted(list(varis))
+    matrix = []
+    for eq in eqs:
+        row = []
+        for vari in varis:
+            if vari in eq:
+                row.append(eq[vari])
+            else:
+                row.append(0)
+        matrix.append(row)
+    b = [eq['constant'] for eq in eqs]
+    
+    nothingHappened = False
+    while not nothingHappened:
+        nothingHappened = True
+        for i1 in range(len(matrix)-1):
+            for i2 in range(1+i1,len(matrix)):
+                j1 = 0
+                while matrix[i1][j1] == 0:
+                    j1 += 1
+                j2 = 0
+                while matrix[i2][j2] == 0:
+                    j2 += 1
+                if [matrix[i1][j]/matrix[i1][j1] for j in range(len(matrix[i1]))] == [matrix[i2][j]/matrix[i2][j2] for j in range(len(matrix[i2]))]:
+                    if b[i1]/matrix[i1][j1] != b[i2]/matrix[i2][j2]:
+                        return None
+                    else:
+                        matrix = matrix[:i1]+matrix[i1+1:]
+                        b = b[:i1]+b[i1+1:]
+                        nothingHappened = False
+                        break
+            if not nothingHappened:
+                break
+    if len(matrix) != len(matrix[0]):
+        return None
+    n = 0
+    while n < len(matrix):
+        while matrix[n][n] == 0:
+            if n == len(matrix)-1:
+                return None
+            r = matrix[n]
+            matrix.pop(n)
+            matrix.append(r)
+            v = b[n]
+            b.pop(n)
+            b.append(v)
+        c = 1/matrix[n][n]
+        matrix[n] = [c*matrix[n][j] for j in range(len(matrix[n]))]
+        b[n] = c*b[n]
+        k = 1
+        while n+k < len(matrix):
+            c = matrix[n+k][n]
+            matrix[n+k] = [matrix[n+k][j] - c*matrix[n][j] for j in range(len(matrix[n]))]
+            if matrix[n+k] == [0]*len(matrix[n+k]):
+                return None
+            b[n+k] = b[n+k] - c*b[n]
+            k += 1
+        n += 1
+    n = len(matrix)-1
+    while n >= 0:
+        k = 1
+        while n-k >= 0:
+            c = matrix[n-k][n]
+            matrix[n-k] = [matrix[n-k][j] - c*matrix[n][j] for j in range(len(matrix[n]))]
+            b[n-k] = b[n-k] - c*b[n]
+            k += 1
+        n -= 1
+    answer = {}
+    for k in range(len(varis)):
+        answer[varis[k]] = b[k]
+    return answer
+
+
     
+
+
+
+"""
+END OF LINEAR ALGEBRA
+"""
+
+
+
```

### Comparing `mammath-0.1.7/mammath/mammath.py` & `mammath-0.1.8/mammath/mammath.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,169 +15,153 @@
 import sys
 import keyboard
 import matplotlib.pyplot as plt
 from mpl_toolkits import mplot3d
 import inspect
 import re
 import mpmath
-##
-import re
 
-operatorsDict = {"**": 5, "*": 2, "/": 2, "+": 1, 'u': 6,  '^': 5, "%": 2, '': 4, "-": 1, }
-otherDict = {'u': 1}
+"""
+SHUNTING YARD ALGORITHM
+A safe replacement for eval
+"""
+
+operatorsDict = {"*": 2, "/": 2, "+": 1, "%": 2, '': 4, "-": 1, "^": 3, "**": 3}
 operators = operatorsDict.keys()
-operatorsBracket = list(operators)[:]
-operatorsBracket.append('(')
 
 def tokenize(inputExpression):
     return re.split("([()" + ''.join(operators) + "])", inputExpression.replace(" ", ""))
 
 def shunting_yard(inputExpression):
     queue = []
     stack = []
 
     tokens = tokenize(inputExpression)
     tokens = [x for x in tokens if x]
-
-    x = 0
-   
-       
-  #  print(tokens)
-
-    for x in range(0, len(tokens)):
-        if(tokens[x] == '-' and (x == 0 or tokens[x - 1] in operatorsBracket)):
-            tokens[x] = 'u'
-           
     for token in tokens:
         if(token not in operators and token != "(" and token != ")"):
             queue.append(token)
 
         if(token == "("):
             stack.append(token)
        
         if(token == ")"):
             while(len(stack) != 0 and stack[-1] != "("):
                 queue.append(stack.pop())
      
             stack.pop()
        
         if(token in operators):
-            if(token == 'u'):  
-                while(len(stack) != 0 and stack[-1] in operators and operatorsDict[stack[-1]] > operatorsDict[token]):
-                    queue.append(stack.pop())
-
-                stack.append(token)
-
-                continue
-           
             while(len(stack) != 0 and stack[-1] in operators and operatorsDict[stack[-1]] >= operatorsDict[token]):
                 queue.append(stack.pop())
 
             stack.append(token)
 
     while(len(stack) != 0):
         queue.append(stack.pop())
 
     return queue
 
 def evaluatePostfix(inputList):
     stack = []
-
-##    print(inputList)
+    
     for token in inputList:
         if(token not in operators):
             stack.append(token)
         else:
-            if(token == 'u'):
-##                print(stack)
-                operand = float(stack.pop())
-                stack.append(-1 * operand)
-
-                continue
             operand2 = float(stack.pop())
             operand1 = float(stack.pop())
-##            print("current ")
-##            print(operand1)
-##            print(operand2)
-##            print(token)
             if(token == "+"):
                 stack.append(operand1 + operand2)
 
             if(token == "-"):
                 stack.append(operand1 - operand2)
 
             if(token == "*"):
                 stack.append(operand1 * operand2)
 
             if(token == "/"):
                 stack.append(operand1 / operand2)
 
             if(token == '^'):
                 stack.append(operand1 ** operand2)
-
-##            print(stack)
                
     return stack[0]
 
 def evaluateExpression(inputExpression):
     return evaluatePostfix(shunting_yard(inputExpression))
 
+"""
+END OF SHUNTING YARD
+"""
+
+
+
+"""
+MATH TEACHERS
+"""
 
 def teach_me_trig():
-    print("welcome to the trig basics course!")
+    print("Welcome to the trigonometry basics course!")
     time.sleep(0.5)
-    print("a basics trigonometric formula is a^2 + b^2 = c^2, the pythagorean theorom")
+    print("One of the most fundamental formulas in trigonometry is the Pythagorean theorem - a^2 + b^2 = c^2, which allows you to find missing sides in a right angled triangle.")
     time.sleep(2)
     print("it works on all right angled triangles")
     time.sleep(1)
-    print(" soh cah toa will help you remember:")
+    print("Then, to calculate sides given an angle and one other side, SOHCAHTOA will help you remember the ratios:")
     time.sleep(0.5)
     print("sin = opposite/hypotenuse")
     time.sleep(1)
-    print("cos = adjacent over hypotenuse")
+    print("cos = adjacent/hypotenuse")
     time.sleep(1)
-    print("and tan = opposite over adjacent")
+    print("and tan = opposite/adjacent")
     time.sleep(1)
     ans = input("If one side of a triangle is 3 and another is 4, what is the hypotenuse? ")
     chances = 2
-    while ans not in ["hypotenuse = 5", "Hypotenuse = 5", "Hyp = 5, hyp = 5", "5", "hyp=5", "Hyp=5", "Hypotenuse=5", "hypotenuse=5"] and chances > 0:
-        print("not correct")
+    while ans.lower().replace(" ", "") not in ["hypotenuse=5", "hyp=5", "5", "five"] and chances > 0:
+        print("That is not correct. Please refer to the pythagorean theorem!")
         ans = input("If one side of a triangle is 3 and another is 4, what is the hypotenuse? ")
         chances = chances - 1
-    if ans in ["hypotenuse = 5", "Hypotenuse = 5", "Hyp = 5, hyp = 5", "5", "hyp=5", "Hyp=5", "Hypotenuse=5", "hypotenuse=5"]:
-        print("great job!")
+    if ans in ["hypotenuse=5", "hyp=5", "5", "five"]:
+        print("Great job! This is also a special case for right angled triangles and is known as a Pythagorean triplet.")
     else:
-        print("the answer was 5")
-    print("wikipedia, mathisfun, and other websites can help too")
-    print("thank you!")
+        print("The answer was 5. We needed to use the Pythagorean theorem which states that a^2 + b^2 = c^2, therefore, 3^2 + 4^2 = c^2, and c = 5")
+    print("Wikipedia, mathisfun, and other websites can help too")
+    print("Thank you!")
+    
 def teach_me_algebra():
-    print("welcome to the algebra basics course!")
+    print("Welcome to the algebra basics course!")
     time.sleep(0.5)
-    print("a you solve basic equations by moving variables to one side and numbers to the other")
+    print("In this basic algebra course, you will learn the basics of solving equations and working with variables.")
     time.sleep(2)
-    print("remember, change the operation when it crosses the equals sign")
-    time.sleep(1)
-    print(" - becomes +, + becomes -")
-    time.sleep(1)
-    print("x becomes /, / becomes x")
-    time.sleep(1)
-    print("and ^n becomes root(n), root(n) becomes ^n")
+    print("In order to solve one step equations, we will try to isolate all of the varaibles. This means that we want all instances of a variable on one side, and all regular numbers on another.")
+    time.sleep(3)
+    print("You will often be given an equation where you will have a few operations taking place on either side of the equation. If an 'x' variable is on a side with other numbers, we will perform the opposite operation that eliminates it from that side that it is on.")
+    time.sleep(3)
+    print("For instance, if we have x+3 = 5, we notice that we have a 3 on the same side as the x. In order to solve for x, we notice that we are adding a three, therefore, we will subtract a three to eliminate it from the x side. However, we need to remember to do the same thing on the other side of the equation. Therefore, the right side becomes 5 -3 = 2. x = 2.")
+    time.sleep(3)
+    print("In general, a + on one side becomes a - to eliminate it, a * becomes a /, a ^ becomes a root. ")
     time.sleep(1)
     ans = input("3x+5=8, what is x? ")
     chances = 2
-    while ans not in ["X = 1", "x = 1", "x=1", "X=1", "3"] and chances > 0:
-        print("not correct")
+    while ans.lower().replace(" ", "") not in ["x=1", "1", "one"] and chances > 0:
+        if chances == 2:
+            print("That is not correct. Notice that the 3x means 3*x.")
+        elif chances == 1:
+            print("That is not correct. First, subtract the 5 on both sides. As we have 3*x. We will need to divide both sides by three to solve for x.")
         ans = input("3x+5=8, what is x? ")
         chances = chances - 1
-    if ans in ["X = 1", "x = 1", "x=1", "X=1", "3"]:
-        print("great job!")
+    if ans in ["x=1", "1", "one"]:
+        print("Great job!")
     else:
-        print("the answer was 3")
-    print("wikipedia, mathisfun, and other websites can help too")
-    print("thank you!")
+        print("The answer was 1")
+        
+    print("Wikipedia, mathisfun, and other websites can help too")
+    print("Thank you!")
+    
 def teach_me_derivitives():
     print("welcome to the derivitives basics course!")
     time.sleep(0.5)
     print("a you solve basic derivitives by using a set of rules")
     time.sleep(0.5)
     print("use this link")
     time.sleep(1)
@@ -390,65 +374,64 @@
     val=""
 def clear():
     global val
     val =""
     data.set(val)
     
 
+"""
+END OF MATH TEACHERS
+"""
+
+
+def recLimit(a):
+    messagebox.askyesno("RECURSION SETTINGS", "Setting your recursion limit may slow your laptop or cause a crash. Proceed with caution. Do You wish to continue?")
 
     
+"""
+OPERATIONS
+"""
+
 def add(*args):
     return sum(args)
+
 def subtract(a, *args):
     return a - sum(args)
+
 def multiply(*args):
     x = 1
     y = 0
     while y < len(args):
         x = x*args[y]
         y+=1
     return x
+
 def divide(a, *args):
     return a / listMultiply(args)
-def listMultiply(List):
+
+#Multiplies all of the elements in a list
+def listMultiply(lis):
     x = 1
     y = 0
     while y < len(List):
         x = x*List[y]
         y+=1
     return x
-def power(a, *args):    
-    b = multiply(args)
-    x = a**(b)
-    if b < 1:
-        return root(a, 1/b)
-    else:
-        return x
-    
-def recLimit(a):
-    messagebox.askyesno("RECURSION SETTINGS", "Setting your recursion limit may slow your laptop or cause a crash. Proceed with caution. Do You wish to continue?")
+
+def power(base, exponent):
+    if exponent == 0:
+        return 1
+    if exponent > 0:
+        return (base * power(base, exponent - 1))
+    return 1 /(base * power(base, -exponent - 1))
+
 def sqrt(a):
     return math.sqrt(a)
 
-def addFraction(a, b):
-    ans = Fraction(a) + Fraction(b)
-    return str(ans)
-def subtractFraction(a, b):
-    ans = Fraction(a) - Fraction(b)
-    return str(ans)
-def multiplyFraction(a, b):
-    ans = Fraction(a) * Fraction(b)
-    return str(ans)
-def divideFraction(a, b):
-    ans = Fraction(a) / Fraction(b)
-    return str(ans)
-def simplifyFraction(a):
-    return str(Fraction(a).limit_denominator())
-
-def root(a, b):    #
+def root(a, b):    
     x = a**(1/b)
     try:
         y = round(x)
         if y-x <= 0.000000000000001:
             if x**(b) != a:
                 if b % 2 == 0 and a < 0:
                     z = str(abs(y)) + 'i'
@@ -483,69 +466,87 @@
     except:
         c = b/2
         t = cmath.sqrt(a)
         while c > 2:
              t = cmath.sqrt(t)
              c -= 1
         return t
-    
+
+def factorial(a):
+    x = 1
+    while a > 0:
+        x *=a
+        a -=1
+    return x
+
 def log(a, b):
     return math.log(a, b)
-def sf(a, b):
+def sigFig(a, b):
     rounded = round(a, b - int(math.floor(math.log10(abs(a)))) - 1)
     return rounded
 def absVal(a):
     return math.fabs(a)
 def remainder(a, b):
     return math.remainder(a, b)
-def toDegrees(a):
-    return math.degrees(a)
-def toRadians(a):
-    return math.radians(a)
 
 def HCF(a, b):
     a, b = max(a, b), min(a, b)
     while b!=0:
         a, b = b, a % b
     return a
 def LCM(a, b):
     return (a*b)/HCF(a, b)
+
+"""
+END OF OPERATIONS
+"""
+
+
+
+"""
+PRIME NUMBERS
+"""
+
 def primeFactors(n):
     while n % 2 == 0:
-            print(2)
-            n = n / 2  
+        print(2)
+        n = n / 2  
     for i in range(3,int(math.sqrt(n))+1,2):
-            while n % i== 0:
-                    print(i)
-                    n = n / i
+        while n % i== 0:
+            print(i)
+            n = n / i
     if n > 2:
-            print(n)
+        print(n)
 
-def factorial(a):
-    x = 1
-    while a > 0:
-        x *=a
-        a -=1
-    return x
 def checkPrime(num):
     x = False
     for i in range(2, num):
         if num % i == 0:
             x = True
     if x:
         return False
     return True
+
 def primeNumberPrinter(low, high):
     for num in range(low, high+1):
         if num > 1:
             for i in range(2, num):
                 if num % i == 0:
                     break
             else:
                 print(num)
+"""
+END OF PRIME NUMBERS
+"""
+
+
+"""
+NUMBER/SEQUENCE CHECKS
+"""
+
 def perfectSquare(num):
     root = math.sqrt(num)
 
     if math.trunc(root)-root==0:
         return True
     return False
 
@@ -581,74 +582,161 @@
             break
     return p == n
 
 def pentagonalPrinter(low, high):
     for i in range(low, high):
         if pentagonalCheck(i) == True:
             print(i)
-def fibonacci(n):
+
+"""
+END OF NUMBER/SEQUENCE CHECKS
+"""
+
+
+
+"""
+FIBONACCI
+"""
+
+def fibonacciBinet(n):
     x = (((((1+math.sqrt(5))/2)**n)-((((1-math.sqrt(5))/2)**n))))/math.sqrt(5)
     return round(x)
+def fibonacci(n):
+    n0, n = n, abs(n)
+    F = {}
+    
+    qinx = []  
+    qinx.append(n)
+    F[n] = -1
+    while qinx:
+        k = qinx.pop() >> 1
+        if k not in F:
+            F[k] = -1
+            qinx.append(k)
+        if (k + 1) not in F:
+            F[k+1] = -1
+            qinx.append(k + 1)
+    
+    F[0], F[1], F[2] = 0, 1, 1
+    keys_sorted = sorted(F.keys())
+    for k in keys_sorted[3:]:
+        k2 = k >> 1
+        f1, f2 = F[k2], F[k2 + 1]
+        if k % 2 == 0:
+            F[k] = 2 * f2 * f1 - f1 * f1
+        else:
+            F[k] = f2 * f2 + f1 * f1
+    
+    r = F[n]
+    if n0 < 0:
+        return negativeFib(n, r)
+    return r
+
 def fibonacciCheck(n):
     return perfectSquareCheck(5*n*n + 4) or perfectSquareCheck(5*n*n - 4)
 def fibonacciPrinter(low, high):
     for i in range(low, high+1):
         if fibonacciCheck(i) == True:
             print(i)
-            
-def divis2Check(num):
+
+"""
+END OF FIBONACCI
+"""
+
+
+
+"""
+DIVISIBILITY CHECKS
+"""
+
+def div2Check(num):
     if num % 2 == 0:
         return True
     else:
         return False
-def divis3Check(num):
+def div3Check(num):
     if num % 3 == 0:
         return True
     else:
         return False
-def divis4Check(num):
+def div4Check(num):
     if num % 4 == 0:
         return True
     else:
         return False
-def divis5Check(num):
+def div5Check(num):
     if num % 5 == 0:
         return True
     else:
         return False
-def divis6Check(num):
+def div6Check(num):
     if num % 6 == 0:
         return True
     else:
         return False
-def divis7Check(num):
+def div7Check(num):
     if num % 7 == 0:
         return True
     else:
         return False
-def divis8Check(num):
+def div8Check(num):
     if num % 8 == 0:
         return True
     else:
         return False
-def divis9Check(num):
+def div9Check(num):
     if num % 9 == 0:
         return True
     else:
         return False
-def divisCheck(num, num2):
+def divCheck(num, num2):
     if num % num2 == 0:
         return True
     else:
         return False
+
+"""
+END OF DIVISIBILITY CHECKS
+"""
+
+    
 def summate(n, a, b):
     return sum(nthRange(n, a, b))
 def product(n, a, b):
     return listMultiply(nthRange(n, a, b))
 
+def timesTables(n):
+    for i in range(1, n+1):
+        for j in range(i, (n*i)+i, i):
+            print(str(j) + " ", end="")
+        print("")
+
+def CoefficientsQuadratic(string):
+    string = "".join(" " if i == "x" or i == "+" else i for i in string)
+    string = string.replace("^2", " ")
+    return list(map(int, string.split()))
+"""
+FRACTIONS
+"""
+
+def addFraction(a, b):
+    ans = Fraction(a) + Fraction(b)
+    return str(ans)
+def subtractFraction(a, b):
+    ans = Fraction(a) - Fraction(b)
+    return str(ans)
+def multiplyFraction(a, b):
+    ans = Fraction(a) * Fraction(b)
+    return str(ans)
+def divideFraction(a, b):
+    ans = Fraction(a) / Fraction(b)
+    return str(ans)
+def simplifyFraction(a):
+    return str(Fraction(a).limit_denominator())
+
 def PercentagetoDecimal(percentage):
     return percentage / 100
 def PerToFrac(p):
     dec = p / 100
     fraction = Fraction(dec)
     return str(fraction)
 def PercentagetoFraction(percentage):
@@ -661,14 +749,29 @@
     return f * 100
 def DecimaltoPercentage(decimal):
     percentage = "{:.0%}".format(decimal)
     return str(percentage)
 def DecimaltoFraction(decimal):
     return str(Fraction(decimal).limit_denominator())
 
+"""
+END OF FRACTIONS
+"""
+
+
+
+"""
+GEOMETRY
+"""
+
+def validTriangle(s1, s2, s3):
+    if s1 + s2 >= s3 and s2 + s3 >= s1 and s1 + s3 >= s2:
+        return True
+    return False
+
 def triangleArea(l, w):
     return (l*w)/2
 def trapeziumArea(a, b, h):
     return (a+b)/h
 def paraHeight(a, b):
     return a/b
 def paraArea(b, h):
@@ -755,14 +858,19 @@
 def cot(a):
     return round(1/tan(a), 5)
 def gamma(a):
     return math.gamma(a)
 def lgamma(a):
     return math.lgamma(a)
 
+def toDegrees(a):
+    return math.degrees(a)
+def toRadians(a):
+    return math.radians(a)
+
 def pytheoromside(a, b):
     if a > c:
         a1 = a*a
         b1 = b*b
         c1 = a1 - b1
         c = math.sqrt(c1)
     else:
@@ -804,63 +912,60 @@
     tanpart = math.tan(intan)
     down = 4*tanpart
     ans = up/down
     return ans
 def pythagoreanTriplets(n):
   for b in range(n):
     for a in range(1, b):
-        c = math.sqrt( a * a + b * b)
+        c = math.sqrt(a * a + b * b)
         if c % 1 == 0:
             print(a, b, int(c))
 def pythagoreanTripletsCheck(a, b, c):
-    if (a ** 2) + (b ** 2) == (c ** 2):
-        return True
-    else:
-        return False
-    
-def speedCalc(d, t):
-    return d/t
-def distCalc(s, t):
-    return s*t
-def timeCalc(s, d):
-    return s*d
-    
+    return True if a * a + b * b == c * c else False
+
+"""
+END OF OF GEOMETRY
+"""
+
 def quadraticSolver(a,b,c):
     dis = b * b - 4 * a * c
     sqrt_val = math.sqrt(abs(dis))
     if dis > 0:
-            print(" real and different roots ")
-            print((-b + sqrt_val)/(2 * a))
-            print((-b - sqrt_val)/(2 * a))
+        print((-b + sqrt_val)/(2 * a))
+        print((-b - sqrt_val)/(2 * a))
     elif dis == 0:
-            print(" real and same roots")
-            print(-b / (2 * a))
+        print(-b / (2 * a))
     else:
-            print("Complex Roots")
-            print(- b / (2 * a), " + i", sqrt_val)
-            print(- b / (2 * a), " - i", sqrt_val)
+        print("Complex Roots")
+        print(- b / (2 * a), " + i", sqrt_val)
+        print(- b / (2 * a), " - i", sqrt_val)
 
-def sequenceChecker(a, b, c, d, e):
-    while 1 < 2:
+"""
+SEQUENCES
+"""
+
+def sequenceChecker(a, b, c):
+    while True:
         if b - a == c - b:
             print("Arithmetic")
             break
         if b / a == c / b or a / b == b / c:
             print("Geometric")
             break
         else:
             print("Quadratic")
             break
 
 def nthFinder(a, b):
     a = str(a)
     b = str(b)
     x = a.replace("n", b)
-    y = evaluateExpression(x)
+    y = eval(x)
     return y
+
 def nthRange(a, b, c):
     ls = []
     a = str(a)
     b = str(b)
     c = str(c)
     if int(b) > int(c):
         while int(c) < int(b)+1:
@@ -917,15 +1022,53 @@
         
     else:
         if before < 0:
             print("Nth Term:", str(dif) + "n" + str(before))
             print(str(term) + "th term:", str(newTerm)) 
         else:
             print("Nth Term:", str(dif) + "n" + " + " + str(before))
-            print(str(term) + "th term:", str(newTerm))  
+            print(str(term) + "th term:", str(newTerm))
+
+def removeDecimal(num):
+        if(num == int(num)):
+            return int(num)
+        return num
+    
+def Nth_Term_Quadratic(*series):
+    
+    r1d1 = series[1] - series[0]
+    r1d2 = series[2] - series[1] 
+    d2 = r1d2 - r1d1 
+    a = d2/2
+    b = r1d1 - 3 * a
+    c = series[0] - (a + b)
+    
+    a = removeDecimal(a) 
+    b = removeDecimal(b)
+    c = removeDecimal(c)
+    
+    quadraticDict = {0: "", 1: "n^2", -1: "-n^2"}
+    linearDict = {0: "", 1: "n", -1: "-n"}
+    constantDict = {0: ""}
+
+    quadraticTerm = "{}n^2".format(a) if (a != 0 and a != 1 and a != -1) else quadraticDict[a]
+    linearTerm = "{}n".format(b) if (b != 0 and b != 1 and b != -1) else linearDict[b]
+    constantTerm = "{}".format(c) if (c != 0) else constantDict[c]
+
+    bSign = "+" if b > 0 else ""
+    cSign = "+" if c > 0 else ""
+
+    print(quadraticTerm + bSign + linearTerm + cSign + constantTerm)
+    
+"""
+END OF SEQUENCES
+"""
+
+
+
 
 def percentageChange(a, b):
     if a == b:
         return 100.0
     try:
         return round(((b - a)/a)*100, 3)
     except ZeroDivisionError:
@@ -985,22 +1128,51 @@
         eq += str(args[int(i)]) + '*(n**' + str(i) + ') +'
         i = int(i)
         i += 1
         i = str(i)
     eq += '0'  
     return nthTable(eq, a, b)
 
-def F(m, a):
+
+
+"""
+FORMULAS
+"""
+#Force, Mass, Acceleration - F=ma
+def Force(m, a):
     return m*a
-def M(f, a):
+def Mass(f, a):
     return f/a
-def A(f, m):
+def Acceleration(f, m):
     return f/m
 
+#Speed, Distance, Time - S=d/t
+def Speed(d, t):
+    return d/t
+def Distance(s, t):
+    return s*t
+def Time(s, d):
+    return s*d
+"""
+END OF FORMULAS
+"""
+
+
+
+"""
+BASE CONVERSIONS
+"""
+
 def baseConverter(x, base):
+    if not isinstance(x, int):
+        if x.isdigit():
+            x = int(x)
+        else:
+            x = int("".join(map(str, [ord(i) for i in x])))
+            
     digs = string.digits + string.ascii_letters
     if x < 0:
         sign = -1
     elif x == 0:
         return digs[0]
     else:
         sign = 1
@@ -1018,30 +1190,40 @@
     digits.reverse()
     return "".join(digits)
 
 def IntToBinary(num):
     return bin(num)[2:]
 def BinaryToInt(num):
     return int(str(num), 2)
+
 def IntToHexa(num):
     return hex(num)[2:]
 def HexaToInt(num):
     return int(str(num, 2))
+
+def BinaryToHex(num):
+    return hex(int(str(num), 2))[2:]
+def HexToBinary(num):
+    return bin(int(str(num), 2))[2:]
+
 def binaryAdd(a, b):
     sum = BinaryToInt(a) + BinaryToInt(b)
     print("Binary:", IntToBinary(sum))
     print("Base 10:", sum)
+    
 def binarySubtract(a, b):
     sub = BinaryToInt(a) - BinaryToInt(b)
     print("Binary:", IntToBinary(sub))
     print("Base 10:", sub)
+    
 def binaryMultiply(a, b):
     mult = BinaryToInt(a) * BinaryToInt(b)
     print("Binary:", IntToBinary(mult))
     print("Base 10:", mult)
+    
 def binaryDivide(a, b):
     div = BinaryToInt(a) / BinaryToInt(b)
     print("Binary:", IntToBinary(div))
     print("Base 10:", div)
     
 def hexaAdd(a, b):
     sum = HexaToInt(a) + HexaToInt(b)
@@ -1056,14 +1238,20 @@
     print("Hexadecimal:", IntToHexa(mult))
     print("Base 10:", mult)
 def hexaDivide(a, b):
     div = HexaToInt(a) / HexaToInt(b)
     print("Hexadecimal:", IntToHexa(div))
     print("Base 10:", div)
 
+"""
+END OF BASE CONVERSIONS
+"""
+
+
+
 def constSearch(con):
     G = 6.67384*10**(-11)
     c = 2.99792458*10**(8)
     h = 6.626070040*10**(-34)
     k = 1.38064852*10**(-23)
     F = 9.648533289*10**(4)
     pi = 3.141592653589793238462643
@@ -1076,38 +1264,43 @@
     while x < 10:
         variable_name = [k for k, v in locals().items() if v == conlist[x]][0]
         if variable_name == con:
             constant = conlist[x]
             return constant
         x += 1
     return None
+
 def constTable():
     G = 6.67384*10**(-11)
     c = 2.99792458*10**(8)
     h = 6.626070040*10**(-34)
     k = 1.38064852*10**(-23)
     F = 9.648533289*10**(4)
     pi = 3.141592653589793238462643
     e = 2.718281828459045235360287
     π = pi
     phi = 1.618033988749894848204586
     φ = phi
     conlist = [["The gravitational constant", "G", G], ["The speed of light in vacuum", "c", c], ["Planck's constant", "h", h], ["Boltzmann's constant", "k", k], ["Faraday's constant", "F", F], ["e", "e", e], ["pi", "φ", π], ["Phi", "φ", φ]]
     headers = ["Name", "Symbol", "Value"]
-    thing = tabulate(conlist, headers = headers)
-    print(thing)
+    constants = tabulate(conlist, headers = headers)
+    print(constants)
+
 
+def f(fx, x, y):
+    if type(eval(fx)) == np.ndarray:
+        return eval(fx)
+
+#graph("2*x", "3*x")
 def graph(*args, lrangex=-10, urangex=10, lrangey=-10, urangey=10, graph_points=100, gridset=True, scaling=True, graph_title=None, xtitle=None, ytitle=None):
     i = 0
     x = np.linspace(lrangex, urangex, graph_points)
     while i < len(args):
-        if type(evaluateExpression(args[i])) == np.ndarray:
-            y = evaluateExpression(args[i])
-        else:
-            pass
+        if type(eval(args[i])) == np.ndarray:
+            y = eval(args[i])
         fig = plt.figure()
         ax = fig.add_subplot(1, 1, 1)
         ax.spines["left"].set_position("center")
         ax.spines["bottom"].set_position("zero")
         ax.spines["right"].set_color("none")
         ax.spines["top"].set_color("none")
         ax.xaxis.set_ticks_position("bottom")
@@ -1121,29 +1314,16 @@
     plt.grid(gridset)
     if lrangex or urangex != False:
         plt.xlim([lrangex,urangex])
     if lrangey or urangey != False:
         plt.ylim([lrangey,urangey])
     plt.show()
 
-def isInfinite(x):
-    return mpmath.isinf(x)
-def isFinite(x):
-    return mpmath.isfinite(x)
-def isInt(x, gaussian = False): 
-    return mpmath.isint(x, gaussian)
 
-def Zeta(s):
-    return zeta(s)
 
-def f(fx, x, y):
-    if type(evaluateExpression(fx)) == np.ndarray:
-        return evaluateExpression(fx)
-    else:
-        pass
     
 def graph3dcontour(*args, lrangex=-10, lrangey=-10, urangex=10, urangey=10, lrangez=-10, urangez=10, graph_points=1000, lablex='x', labley='y', lablez='z', graph_title=None, cmap='binary'):
     x = np.linspace(lrangex, urangex, graph_points)
     y = np.linspace(lrangey, urangey, graph_points)
     fig = plt.figure()
     ax = plt.axes(projection='3d')
     i = 0
@@ -1170,20 +1350,20 @@
     fig = plt.figure()
     ax = plt.axes(projection='3d')
     i = 0
     while i < len(args):
         lis = args[i]
         fz = lis[0]
         fy = lis[1]
-        if type(evaluateExpression(fz)) == np.ndarray:
-            zline = evaluateExpression(fz)
+        if type(eval(fz)) == np.ndarray:
+            zline = eval(fz)
         else:
             pass
-        if type(evaluateExpression(fy)) == np.ndarray:
-            yline = evaluateExpression(fy)
+        if type(eval(fy)) == np.ndarray:
+            yline = eval(fy)
         else:
             pass
         ax.plot3D(x, yline, zline, color)
         i+=1
     ax.set_xlabel(lablex)
     ax.set_ylabel(labley)
     ax.set_zlabel(lablez)
@@ -1213,32 +1393,265 @@
             ax.plot_surface(X, Y, Z, rstride=1, cstride=1,
                     cmap=fill, edgecolor='none')
         else:
             raise TypeError('Parameter "edgecolor" must be a boolean operator')
         i += 1
     ax.set_xlabel(lablex)
     ax.set_ylabel(labley)
-    ax.set_zlabel(lablez)
+    ax.set_zlabel(lablez)   
     ax.set_title(graph_title)
     if lrangez != False or urangez == False:
         ax.set_zlim(lrangez, urangez)
     if lrangex != False or urangex == False:
         ax.set_zlim(lrangex, urangex)
     if lrangey != False or urangey == False:
         ax.set_zlim(lrangey, urangey)
     return plt.show()
 
+def isInfinite(x):
+    return mpmath.isinf(x)
+def isFinite(x):
+    return mpmath.isfinite(x)
+def isInt(x, gaussian = False): 
+    return mpmath.isint(x, gaussian)
+
+def Zeta(s):
+    return zeta(s)
+
+
+"""
+CALCULUS
+"""
+
 def derivative(f_of, solvefor):
     return diff(f_of, solvefor)
 def secondDerivative(f_of, *args):
     return diff(f_of, args)
 def integral(f_of, solvefor):
     integral = integrate(f_of, solvefor)
     return integral
 def IndefIntegral(f_of, solvefor):
     integral = str(integrate(f_of, solvefor)) + " + C"
     return integral
 def defIntegral(f_of, solvefor, lowerbound, upperbound):
     return integrate((f_of), (solvefor, lowerbound, upperbound))
 def Limit(f_of, solvefor, to):
     return limit(f_of, solvefor, to)
+
+
+"""
+END OF CALCULUS
+"""
+
+
+
+"""
+LINEAR ALGEBRA
+"""
+def Adjacent2x2(matrix):
+    return np.array([[matrix[1][1], -matrix[0][1]], [-matrix[1][0], matrix[0][0]]]).tolist()
+
+def Adjacent3x3(matrix):
+    a = np.array([[(matrix[1][1]*matrix[2][2]) - (matrix[1][2]*matrix[2][1]),
+                   -((matrix[1][0]*matrix[2][2]) - (matrix[1][2]*matrix[2][0])),
+                   ((matrix[1][0]*matrix[2][1]) - (matrix[1][1]*matrix[2][0]))],
+                                    
+                  [-((matrix[0][1]*matrix[2][2]) - (matrix[0][2]*matrix[2][1])),
+                    ((matrix[0][0]*matrix[2][2]) - (matrix[0][2]*matrix[2][0])),
+                    -((matrix[0][0]*matrix[2][1]) - (matrix[0][1]*matrix[2][0]))],
+                                    
+                  [((matrix[0][1]*matrix[1][2]) - (matrix[0][2]*matrix[1][1])),
+                   -((matrix[0][0]*matrix[1][2]) - (matrix[0][2]*matrix[1][0])),
+                    ((matrix[0][0]*matrix[1][1]) - (matrix[0][1]*matrix[1][0]))]])
+
+    return np.transpose(a)
+
+def DiagonalSum(mat):
+    left = 0
+    right = 0
+    for i in range(0, len(mat)):
+        left += mat[i][i]
+        right += mat[i][len(mat) - i - 1]
+    total = left + right
+    if len(mat) % 2 != 0:
+        return total - (mat[len(mat) // 2][len(mat) // 2])
+    return total
+
+def solveEquations(*equations):              
+    equations = list(equations)
+    for i in range(0, len(equations)):
+        equations[i] = equations[i].replace(" ", "")
+        
+    eqs = []
+    varis = set()
+    for k in range(len(equations)):
+        equations[k] = equations[k].replace('-','+-')
+        eqDict = dict()
+        sides = equations[k].split('=')
+        termsLeft = sides[0].split('+')
+        termsRight = sides[1].split('+')
+        for term in termsLeft:
+            if term != '':
+                if term.isnumeric():
+                    if 'constant' in eqDict:
+                        eqDict['constant'] += -int(term)
+                    else:
+                        eqDict['constant'] = -int(term)
+                    continue
+                elif not '-' in term:
+                    if term.isalpha():
+                        coeff = 1
+                        vari = term
+                    else:
+                        l = 0
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = int(term[:l])
+                        vari = term[l:]
+                else:
+                    if term[1:].isnumeric():
+                        if 'constant' in eqDict:
+                            eqDict['constant'] += -int(term)
+                        else:
+                            eqDict['constant'] = -int(term)
+                        continue
+                    elif term[1:].isalpha():
+                        coeff = -1
+                        vari = term[1:]
+                    else:
+                        l = 1
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = -int(term[1:l])
+                        vari = term[l:]
+                varis.add(vari)
+                if vari in eqDict:
+                    eqDict[vari] += coeff
+                else:
+                    eqDict[vari] = coeff
+        for term in termsRight:
+            if term != '':
+                if term.isnumeric():
+                    if 'constant' in eqDict:
+                        eqDict['constant'] += int(term)
+                    else:
+                        eqDict['constant'] = int(term)
+                    continue
+                elif not '-' in term:
+                    if term.isalpha():
+                        coeff = -1
+                        vari = term
+                    else:
+                        l = 0
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = -int(term[:l])
+                        vari = term[l:]
+                else:
+                    if term[1:].isnumeric():
+                        if 'constant' in eqDict:
+                            eqDict['constant'] += int(term)
+                        else:
+                            eqDict['constant'] = int(term)
+                        continue
+                    if term[1:].isalpha():
+                        coeff = 1
+                        vari = term[1:]
+                    else:
+                        l = 1
+                        while term[l].isdigit():
+                            l += 1
+                        coeff = int(term[1:l])
+                        vari = term[l:]
+                varis.add(vari)
+                if vari in eqDict:
+                    eqDict[vari] += coeff
+                else:
+                    eqDict[vari] = coeff
+        if not 'constant' in eqDict:
+            eqDict['constant'] = 0
+        eqs.append(eqDict)
+    if len(eqs) < len(varis):
+        return None
+    varis = sorted(list(varis))
+    matrix = []
+    for eq in eqs:
+        row = []
+        for vari in varis:
+            if vari in eq:
+                row.append(eq[vari])
+            else:
+                row.append(0)
+        matrix.append(row)
+    b = [eq['constant'] for eq in eqs]
+    
+    nothingHappened = False
+    while not nothingHappened:
+        nothingHappened = True
+        for i1 in range(len(matrix)-1):
+            for i2 in range(1+i1,len(matrix)):
+                j1 = 0
+                while matrix[i1][j1] == 0:
+                    j1 += 1
+                j2 = 0
+                while matrix[i2][j2] == 0:
+                    j2 += 1
+                if [matrix[i1][j]/matrix[i1][j1] for j in range(len(matrix[i1]))] == [matrix[i2][j]/matrix[i2][j2] for j in range(len(matrix[i2]))]:
+                    if b[i1]/matrix[i1][j1] != b[i2]/matrix[i2][j2]:
+                        return None
+                    else:
+                        matrix = matrix[:i1]+matrix[i1+1:]
+                        b = b[:i1]+b[i1+1:]
+                        nothingHappened = False
+                        break
+            if not nothingHappened:
+                break
+    if len(matrix) != len(matrix[0]):
+        return None
+    n = 0
+    while n < len(matrix):
+        while matrix[n][n] == 0:
+            if n == len(matrix)-1:
+                return None
+            r = matrix[n]
+            matrix.pop(n)
+            matrix.append(r)
+            v = b[n]
+            b.pop(n)
+            b.append(v)
+        c = 1/matrix[n][n]
+        matrix[n] = [c*matrix[n][j] for j in range(len(matrix[n]))]
+        b[n] = c*b[n]
+        k = 1
+        while n+k < len(matrix):
+            c = matrix[n+k][n]
+            matrix[n+k] = [matrix[n+k][j] - c*matrix[n][j] for j in range(len(matrix[n]))]
+            if matrix[n+k] == [0]*len(matrix[n+k]):
+                return None
+            b[n+k] = b[n+k] - c*b[n]
+            k += 1
+        n += 1
+    n = len(matrix)-1
+    while n >= 0:
+        k = 1
+        while n-k >= 0:
+            c = matrix[n-k][n]
+            matrix[n-k] = [matrix[n-k][j] - c*matrix[n][j] for j in range(len(matrix[n]))]
+            b[n-k] = b[n-k] - c*b[n]
+            k += 1
+        n -= 1
+    answer = {}
+    for k in range(len(varis)):
+        answer[varis[k]] = b[k]
+    return answer
+
+
     
+
+
+
+"""
+END OF LINEAR ALGEBRA
+"""
+
+
+
```

### Comparing `mammath-0.1.7/mammath.egg-info/PKG-INFO` & `mammath-0.1.8/mammath.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: mammath
-Version: 0.1.7
-Summary: A package that contains all you will need when you need to do complicated maths in python
+Version: 0.1.8
+Summary: A package that contains all you will need when you need to do maths in python
 Author: Vihaan Mathur & Harihar Rengan
-Author-email: vihaan.harihar341@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: vihaan.harihar314@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # mammath
@@ -19,8 +17,7 @@
 It is built upon several other modules including sys, tkinter, string, time, math, cmath, fractions, mpmath, keyboard, numpy, sympy, tabulate, re, matplotlib, and modules within them.
 
 You can have full detail on its functions using the help(mammath) syntax in the shell after importing the module.
 
 We hope Mammath is a useful and reliable asset.
 
 Thank you!
-
```

### Comparing `mammath-0.1.7/setup.py` & `mammath-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mammath",
-    version="0.1.7",
+    version="0.1.8",
     author="Vihaan Mathur & Harihar Rengan",
-    author_email="vihaan.harihar341@gmail.com",
-    description="A package that contains all you will need when you need to do complicated maths in python",
+    author_email="vihaan.harihar314@gmail.com",
+    description="A package that contains all you will need when you need to do maths in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     packages = ["mammath"],
     python_requires=">=3.6",
     install_requires=["sympy", "tabulate", "numpy", "matplotlib", "keyboard"],
-)
+)
```

