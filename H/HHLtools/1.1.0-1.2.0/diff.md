# Comparing `tmp/HHLtools-1.1.0-py2.py3-none-any.whl.zip` & `tmp/HHLtools-1.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 5127 bytes, number of entries: 7
--rw-r--r--  2.0 unx      338 b- defN 23-Apr-21 03:35 HHLtools/CN.py
--rw-r--r--  2.0 unx     9392 b- defN 23-Apr-21 05:52 HHLtools/__init__.py
--rwxrwxrwx  2.0 unx     1126 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1266 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      542 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/RECORD
-7 files, 12783 bytes uncompressed, 4169 bytes compressed:  67.4%
+Zip file size: 6693 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     8071 b- defN 23-Apr-21 15:34 HHLtools/ADT.py
+-rw-r--r--  2.0 unx      304 b- defN 23-Apr-22 03:39 HHLtools/CN.py
+-rw-r--r--  2.0 unx      592 b- defN 23-Apr-21 14:47 HHLtools/Herror.py
+-rw-r--r--  2.0 unx     4577 b- defN 23-Apr-22 03:39 HHLtools/Hmath.py
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-21 12:46 HHLtools/__init__.py
+-rw-r--r--  2.0 unx      594 b- defN 23-Apr-21 10:52 HHLtools/prints.py
+-rwxrwxrwx  2.0 unx     1126 b- defN 23-Apr-22 03:42 HHLtools-1.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1385 b- defN 23-Apr-22 03:42 HHLtools-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-22 03:42 HHLtools-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-22 03:42 HHLtools-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      833 b- defN 23-Apr-22 03:42 HHLtools-1.2.0.dist-info/RECORD
+11 files, 17605 bytes uncompressed, 5295 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
+Filename: HHLtools/ADT.py
+Comment: 
+
 Filename: HHLtools/CN.py
 Comment: 
 
+Filename: HHLtools/Herror.py
+Comment: 
+
+Filename: HHLtools/Hmath.py
+Comment: 
+
 Filename: HHLtools/__init__.py
 Comment: 
 
-Filename: HHLtools-1.1.0.dist-info/LICENSE.txt
+Filename: HHLtools/prints.py
+Comment: 
+
+Filename: HHLtools-1.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: HHLtools-1.1.0.dist-info/METADATA
+Filename: HHLtools-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: HHLtools-1.1.0.dist-info/WHEEL
+Filename: HHLtools-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: HHLtools-1.1.0.dist-info/top_level.txt
+Filename: HHLtools-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: HHLtools-1.1.0.dist-info/RECORD
+Filename: HHLtools-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## HHLtools/CN.py

```diff
@@ -1,9 +1,7 @@
-from HHLtools import Stack,Queue
-
 真 = True
 假 = False
 输出 = print
 输入 = input
 范围 = range
 整型 = int
 浮点型 = float
```

## HHLtools/__init__.py

```diff
@@ -1,344 +1,2 @@
-from collections.abc import Iterable
-#CONSTANTS
-class FontStyle:
-    DEFAULT = 0
-    BOLD = 1
-    UNDERLINE = 4
-    BLINK = 5
-    REVERSE = 7
-
-class FontColor:
-    BLACK = 30
-    RED = 31
-    GREEN = 32
-    YELLOW = 33
-    BLUE = 34
-    PURPLE = 35
-    CYAN = 36
-    WHITE = 37
-
-class BackgroundColor:
-    DEFAULT = ''
-    BLACK = 40
-    RED = 41
-    GREEN = 42
-    YELLOW = 43
-    BLUE = 44
-    PURPLE = 45
-    CYAN = 46
-    WHITE = 47
-
-
-def fibonacci(n:int):
-    if type(n) != int:
-        raise TypeError
-    if n < 1:
-        return "error, n should be a positive number which is greater than 1"
-    if n < 3:
-        return 1
-    a, b = 1, 1
-
-    for i in range(2, n):
-        a = a + b if i % 2 == 0 else a
-        b = a + b if i % 2 == 1 else b
-    return a if a > b else b
-
-def fibonacci_list(n):
-    if type(n) != int:
-        raise TypeError
-    if n < 1:
-        return "error, n should be a positive number which is greater than 1"
-    if n == 1:
-        return [1]
-    if n == 2:
-        return [1, 1]
-    list = [1, 1]
-    for i in range(2, n):
-        list.append(list[i - 2] + list[i - 1])
-    return list
-
-class Queue:
-    def __init__(self,size:int = -1):
-        if size > 0:
-            self.__size = size
-            self.__queue = [0] * size
-            self.__head = 0
-            self.__tail = 0
-            self.__count = 0
-        else:
-            self.__size = size
-            self.__queue = []
-
-    def __repr__(self):
-        return f'Queue({str(self.__queue)}, ' \
-               f'headPointer = {self.__head if self.__size != -1 else len(self.__queue) - 1}, ' \
-               f'tailPointer = {self.__tail if self.__size != -1 else 0})'
-
-    def __len__(self):
-        return self.__count if self.__size != -1 else len(self.__queue)
-
-    def __iter__(self):
-        return iter(self.getlist())
-
-    def __contains__(self, item):
-        return item in self.getlist()
-
-    def __getitem__(self, item):
-        return self.getlist()[int(item)]
-
-    def getlist(self):
-        contents = []
-        if self.__size == -1:
-            contents = self.__queue[:]
-        else:
-            head = self.__head
-            while 1:
-                contents.append(self.__queue[head])
-                head += 1
-                head = head % self.__size
-                if head == self.__tail:
-                    break
-        return contents
-
-    def show(self):
-        contents = self.getlist()
-        maxlen = 0
-        for c in contents:
-            if len(str(c)) > maxlen:
-                maxlen = len(str(c))
-        print('='*(15+maxlen+15))
-        for c in range(len(contents)):
-            front = ' '*15
-            end = ' '
-            if c == self.__head:
-                front = 'headPointer    '
-            if c == self.__tail:
-                end = (maxlen+4)*' ' +'tailPointer'
-            print(front+str(contents[c])+' '*(maxlen-len(str(contents[c])))+end)
-        print('=' * (15 + maxlen + 15))
-
-    def push(self, content: int|str|float):
-        if type(content) not in (int, str, float):
-            raise TypeError
-        if self.__size > 0:
-            if self.__count == self.__size:
-                print('the queue is full, try pop()')
-                return
-            self.__queue[self.__tail] = content
-            self.__tail = (self.__tail+1)%self.__size
-            self.__count += 1
-        else:
-            try:
-                self.__queue.append(content)
-            except:
-                print('invalid input')
-
-    def pop(self):
-        if self.__size > 0:
-            if self.__count == 0:
-                print('the queue is empty, try push()')
-                return
-            print('remove:', self.__queue[self.__head])
-            self.__head = (self.__head + 1)%self.__size
-            self.__count -= 1
-        else:
-            try:
-                del self.__queue[0]
-            except IndexError:
-                print('warning : no value in the queue,try push(content) to add one')
-
-
-class Stack():
-    def __init__(self,size:int=-1):
-        self.a = 0
-        if size > 0:
-            self.__stack = [0]*size
-        else:
-            self.__stack = []
-        self.__size = size
-        self.__top = -1
-
-    def __repr__(self):
-        return f'Stack({str(self.__stack)}, topPointer = {self.__top if self.__top != -1 else len(self.__stack)-1})'
-
-    def __len__(self):
-        return self.__top if self.__size != -1 else len(self.__stack)
-
-    def __iter__(self):
-        return iter(self.getlist())
-
-    def __contains__(self, item):
-        return item in self.getlist()
-
-    def __getitem__(self, item):
-        return self.getlist()[int(item)]
-
-    def getlist(self):
-        contents = []
-        if self.__size == -1:
-            contents = self.__stack[:]
-        else:
-            for i in range(0, self.__top):
-                contents.append(self.__stack[i])
-        return contents
-
-    def push(self, content: int|str|float):
-        if type(content) not in (int, str, float):
-            raise TypeError
-        if self.__size > 0:
-            if self.__top < self.__size - 1:
-                self.__top += 1
-                self.__stack[self.__top] = content
-            else:
-                print('stack is full, try pop()')
-        else:
-            self.__stack.insert(0,content)
-
-    def pop(self):
-        if self.__size > 0:
-            if self.__top > -1:
-                print(self.__stack[self.__top])
-                self.__top -= 1
-            else:
-                print('warning : stack is empty ,try push(content)')
-        else:
-            try:
-                print(self.__stack[0])
-                del self.__stack[0]
-            except IndexError:
-                print('warning : stack is empty ,try push(content)')
-
-class Hmath:
-    class Functions:
-        def __init__(self, expression: str, variable: str):
-            if type(expression) != str or type(variable) != str:
-                raise TypeError
-            self.__expression = expression
-            self.__var = variable
-
-        def evaluate(self, value: int|float):
-            if type(value) not in (int, float):
-                raise TypeError
-            expression = self.__expression.replace(self.__var, str(value))
-            return eval(expression)
-
-        def gradient(self, accuracy:float, value: int|float):
-            if type(value) not in (int, float) or type(accuracy) != float:
-                raise TypeError
-            x1 = value
-            x2 = value + 10 ** -accuracy
-            y1 = self.evaluate(x1)
-            y2 = self.evaluate(x2)
-            res = (y2 - y1) / (x2 - x1)
-            return round(res, 1) if res - int(res) > 0.999 or res - int(res) < 0.001 else round(res, 3)
-
-
-def prints(content,fontStyle=FontStyle.DEFAULT,fontColor=FontColor.WHITE,backgroundColor=BackgroundColor.DEFAULT):
-    print("\033[{};{};{}m{}\033[0m".format(fontStyle,fontColor,backgroundColor,content))
-
-class LinkedListNode:
-    def __init__(self, val):
-        if type(val) not in (int, str, float):
-            raise TypeError
-        self.val = val
-        self.next = None
-
-    def __repr__(self):
-        result = ''
-        temp = self
-        while temp != None:
-            result += (str(temp.val) + ' --> ')
-            temp = temp.next
-        print(result[:-5])
-        return f'LinkedList({result})'
-
-    def __iter__(self):
-        return iter(self.getlist())
-
-    def __contains__(self, item):
-        return item in self.getlist()
-
-    def __getitem__(self, item):
-        return self.getlist()[int(item)]
-
-    def getlist(self):
-        content = []
-        temp = self
-        while temp != None:
-            content.append(temp.val)
-            temp = temp.next
-        return content
-
-def create_linkedlist_from_list(lst:list):
-    if type(lst) != list:
-        raise TypeError
-    if len(lst) == 0:
-        return LinkedListNode(None)
-    node = LinkedListNode(lst[0])
-    temp = node
-    for i in lst[1:]:
-        temp.next = LinkedListNode(i)
-        temp = temp.next
-    return node
-
-def create_stack_from_list(lst:list, Fixedlength:bool = True):
-    if type(lst) != list:
-        raise TypeError
-
-    if Fixedlength:
-        stack = Stack(len(lst))
-    else:
-        stack = Stack()
-    for i in lst:
-        stack.push(i)
-    return stack
-
-def create_queue_from_list(lst:list, Fixedlength:bool = True):
-    if type(lst) != list:
-        raise TypeError
-
-    if Fixedlength:
-        queue = Queue(len(lst))
-    else:
-        queue = Queue()
-    for i in lst:
-        queue.push(i)
-    return queue
-
-
-
-def BinarySearch(iterable, target):
-    if not isinstance(iterable, Iterable):
-        raise TypeError
-    found = False
-    highIndex = len(iterable)-1
-    lowIndex = 0
-    while not found and lowIndex <= highIndex:
-
-        mid = (highIndex + lowIndex) // 2
-        if iterable[mid] == target:
-            found = True
-            print(mid)
-        elif iterable[mid] > target:
-            highIndex = mid - 1
-        else:
-            lowIndex = mid + 1
-
-    if not found:
-        print("not found")
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

## Comparing `HHLtools-1.1.0.dist-info/LICENSE.txt` & `HHLtools-1.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `HHLtools-1.1.0.dist-info/METADATA` & `HHLtools-1.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: HHLtools
-Version: 1.1.0
-Summary: A tool for CAIE 9618 learner
+Version: 1.2.0
+Summary: A tool for CAIE 9618 learner, and some math function
 Author: hhaolin
 Author-email: 2813579566@qq.com
 License: MIT
 Keywords: HHLtools
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -44,8 +44,11 @@
 2022/11/4
     | 1.0.8 Chinese extension
     | 1.0.8.1 debug
 
 2023/4/21
     | 1.1.0 add linked list, and some useful modifications to previous function
 
+2023/4/22
+    | 1.2.0 fix bugs, modify the error display, add Vector (only 2 or 3 dimensions)
+
```

## Comparing `HHLtools-1.1.0.dist-info/RECORD` & `HHLtools-1.2.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
-HHLtools/CN.py,sha256=1q6JLuIlFsffkvX2bQomQ6FalXDxHkBAvfe-VJMNv3I,338
-HHLtools/__init__.py,sha256=7ScMsKF166SeJSIVXRUFZMLLkob0KKYMAj8EBRgfySQ,9392
-HHLtools-1.1.0.dist-info/LICENSE.txt,sha256=vbOM-gZMeDz9xJ4Zfi9uXfb-FPKDFJAzLi5unV0lbc8,1126
-HHLtools-1.1.0.dist-info/METADATA,sha256=-74Gv_VphCU76BxVhhhZ4TGIVJV8sErBsDBGkWv2QFg,1266
-HHLtools-1.1.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-HHLtools-1.1.0.dist-info/top_level.txt,sha256=iWPR0VidexazFhZwXCYAmN4VW8BPH7H6s7y1PC-UvXE,9
-HHLtools-1.1.0.dist-info/RECORD,,
+HHLtools/ADT.py,sha256=lwJSO6Rc_qcGToyzvvyP5U6NHsjEXyzpV-w8OfyG42c,8071
+HHLtools/CN.py,sha256=WCtruq7X8VtgRt28TXuzeBbwdhTBctiwSXnYcYatnG0,304
+HHLtools/Herror.py,sha256=s8Y3tBmTEgAZLfreDGH7LnoAK8DvCDX03Hb11exKG8M,592
+HHLtools/Hmath.py,sha256=W09lga5QBzpheyn5-QaKvUx6VfbP4oIxue6yxOjxG2c,4577
+HHLtools/__init__.py,sha256=26UWatnbm6ZIwQMuu9NNzQ0IW1ACO4Oe9caModuTpWM,4
+HHLtools/prints.py,sha256=9hcepx9N83tl3tdGSl-EAuc2OJ47Snf9zYV-TYHCdZI,594
+HHLtools-1.2.0.dist-info/LICENSE.txt,sha256=vbOM-gZMeDz9xJ4Zfi9uXfb-FPKDFJAzLi5unV0lbc8,1126
+HHLtools-1.2.0.dist-info/METADATA,sha256=SIjvthleR16s5_XTytVb1CtBNoJmZhiR40OgAWteG4o,1385
+HHLtools-1.2.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+HHLtools-1.2.0.dist-info/top_level.txt,sha256=iWPR0VidexazFhZwXCYAmN4VW8BPH7H6s7y1PC-UvXE,9
+HHLtools-1.2.0.dist-info/RECORD,,
```

