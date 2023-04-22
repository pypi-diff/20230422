# Comparing `tmp/ssm-selector-0.1.0.tar.gz` & `tmp/ssm-selector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-selector-0.1.0.tar", max compression
+gzip compressed data, was "ssm-selector-0.1.1.tar", max compression
```

## Comparing `ssm-selector-0.1.0.tar` & `ssm-selector-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      405 2023-04-21 15:16:10.910838 ssm-selector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 14:31:35.790826 ssm-selector-0.1.0/ssm_selector/__init__.py
--rw-r--r--   0        0        0     2362 2023-04-21 15:17:35.930847 ssm-selector-0.1.0/ssm_selector/instance_selector.py
--rw-r--r--   0        0        0      837 2023-04-21 14:32:12.360848 ssm-selector-0.1.0/ssm_selector/start_session.py
--rw-r--r--   0        0        0      733 2023-04-21 15:21:17.291100 ssm-selector-0.1.0/setup.py
--rw-r--r--   0        0        0      350 2023-04-21 15:21:17.291262 ssm-selector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-21 16:57:32.860835 ssm-selector-0.1.1/LICENSE
+-rw-r--r--   0        0        0      459 2023-04-22 04:16:10.732511 ssm-selector-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 14:31:35.790826 ssm-selector-0.1.1/ssm_selector/__init__.py
+-rw-r--r--   0        0        0     2526 2023-04-21 16:30:44.980859 ssm-selector-0.1.1/ssm_selector/instance_selector.py
+-rw-r--r--   0        0        0     1567 2023-04-22 04:13:26.672523 ssm-selector-0.1.1/ssm_selector/start_session.py
+-rw-r--r--   0        0        0      733 2023-04-22 04:16:15.934592 ssm-selector-0.1.1/setup.py
+-rw-r--r--   0        0        0      350 2023-04-22 04:16:15.934765 ssm-selector-0.1.1/PKG-INFO
```

### Comparing `ssm-selector-0.1.0/ssm_selector/instance_selector.py` & `ssm-selector-0.1.1/ssm_selector/instance_selector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,84 @@
-import boto3
+import curses
 import sys
-import termios
-import tty
-import os
+
+import boto3
 
 
 class InstanceSelector:
     def __init__(self, region_name):
-        self.ec2 = boto3.resource('ec2', region_name=region_name)
+        self.ec2 = boto3.resource("ec2", region_name=region_name)
 
     def select_instance(self):
         instances = self.ec2.instances.filter(
-            Filters=[
-                {'Name': 'instance-state-name', 'Values': ['running']}
-            ]
+            Filters=[{"Name": "instance-state-name", "Values": ["running"]}]
         )
         instance_list = []
         for i, instance in enumerate(instances):
-            instance_list.append({
-                'index': i,
-                'instance_id': instance.id,
-                'instance_name': self.get_instance_name(instance)
-            })
+            instance_list.append(
+                {
+                    "index": i,
+                    "instance_id": instance.id,
+                    "instance_name": self.get_instance_name(instance),
+                }
+            )
 
         if not instance_list:
-            print('No running instances found.')
+            print("No running instances found.")
             sys.exit(1)
 
-        self.print_instance_list(instance_list)
+        instance_list.append(
+            {"index": len(instance_list), "instance_name": "Cancel instance selection"}
+        )
+
+        selected_instance = self.select_instance_with_curses(instance_list)
+
+        return selected_instance
+
+    def select_instance_with_curses(self, instance_list):
+        screen = curses.initscr()
+        curses.noecho()
+        curses.cbreak()
+        screen.keypad(True)
+
+        cursor_y = 0
+
+        while True:
+            screen.clear()
+            screen.addstr(
+                0, 0, "Select an instance (line number to move, enter to select):"
+            )
+            for i, instance in enumerate(instance_list):
+                screen.addstr(
+                    i + 1, 0, "{:>3}: {}".format(i + 1, instance["instance_name"])
+                )
+                if i == cursor_y:
+                    screen.chgat(i + 1, 0, -1, curses.A_REVERSE)
+
+            screen.refresh()
+
+            key = screen.getch()
+
+            if key == curses.KEY_UP and cursor_y > 0:
+                cursor_y -= 1
+            elif key == curses.KEY_DOWN and cursor_y < len(instance_list) - 1:
+                cursor_y += 1
+            elif key == curses.KEY_ENTER or key == 10:
+                if cursor_y == len(instance_list) - 1:
+                    selected_instance = None
+                    break
+                else:
+                    selected_instance = instance_list[cursor_y]["instance_id"]
+                    break
+
+        curses.nocbreak()
+        screen.keypad(False)
+        curses.echo()
+        curses.endwin()
 
-        # ユーザーからの入力を受け付ける
-        index = self.get_user_input(len(instance_list))
-        selected_instance = instance_list[index]['instance_id']
         return selected_instance
 
     def get_instance_name(self, instance):
         for tag in instance.tags or []:
-            if tag['Key'] == 'Name':
-                return tag['Value']
+            if tag["Key"] == "Name":
+                return tag["Value"]
         return instance.id
-
-    def print_instance_list(self, instance_list):
-        # インスタンスの一覧を表示する
-        for instance in instance_list:
-            print(f"{instance['index']}: {instance['instance_name']} ({instance['instance_id']})")
-
-    def get_user_input(self, max_index):
-        # ユーザーからの入力を受け付ける
-        print("Select an instance (index): ", end='', flush=True)
-        old_settings = termios.tcgetattr(sys.stdin)
-        try:
-            tty.setcbreak(sys.stdin.fileno())
-            index = ''
-            while True:
-                char = os.read(sys.stdin.fileno(), 1).decode()
-                if char == '\n':
-                    break
-                elif char == '\x7f': # バックスペース
-                    index = index[:-1]
-                elif char.isdigit():
-                    index += char
-                print(f"\rSelect an instance (index): {index}", end='', flush=True)
-                if int(index) >= max_index:
-                    index = str(max_index - 1)
-        finally:
-            termios.tcsetattr(sys.stdin, termios.TCSADRAIN, old_settings)
-
-        print()
-        return int(index)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ssm-selector-0.1.0/setup.py` & `ssm-selector-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['boto3>=1.26.117,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ssm-selector = ssm_selector.start_session:main']}
 
 setup_kwargs = {
     'name': 'ssm-selector',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': "An interactive SSM Session starter'",
     'long_description': None,
     'author': 'kkmiura',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

