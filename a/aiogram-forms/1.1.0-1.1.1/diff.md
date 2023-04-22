# Comparing `tmp/aiogram_forms-1.1.0.tar.gz` & `tmp/aiogram_forms-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram_forms-1.1.0.tar", max compression
+gzip compressed data, was "aiogram_forms-1.1.1.tar", max compression
```

## Comparing `aiogram_forms-1.1.0.tar` & `aiogram_forms-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1075 2023-04-02 10:25:22.993494 aiogram_forms-1.1.0/LICENSE
--rw-r--r--   0        0        0     2591 2023-04-02 11:26:40.208668 aiogram_forms-1.1.0/README.md
--rw-r--r--   0        0        0      231 2023-04-02 10:25:22.993770 aiogram_forms-1.1.0/aiogram_forms/__init__.py
--rw-r--r--   0        0        0      102 2023-04-02 10:25:22.993883 aiogram_forms-1.1.0/aiogram_forms/const.py
--rw-r--r--   0        0        0        0 2023-04-02 10:25:22.993996 aiogram_forms-1.1.0/aiogram_forms/core/__init__.py
--rw-r--r--   0        0        0      864 2023-04-02 10:26:30.926575 aiogram_forms-1.1.0/aiogram_forms/core/entities.py
--rw-r--r--   0        0        0      659 2023-04-02 10:26:30.926670 aiogram_forms-1.1.0/aiogram_forms/core/manager.py
--rw-r--r--   0        0        0     1567 2023-04-02 10:25:22.994351 aiogram_forms-1.1.0/aiogram_forms/core/states.py
--rw-r--r--   0        0        0     2575 2023-04-02 10:26:30.926774 aiogram_forms-1.1.0/aiogram_forms/dispatcher.py
--rw-r--r--   0        0        0      568 2023-04-02 10:25:22.994575 aiogram_forms-1.1.0/aiogram_forms/enums.py
--rw-r--r--   0        0        0      293 2023-04-02 10:25:22.994672 aiogram_forms-1.1.0/aiogram_forms/errors.py
--rw-r--r--   0        0        0     1092 2023-04-02 10:26:30.926874 aiogram_forms-1.1.0/aiogram_forms/filters.py
--rw-r--r--   0        0        0      179 2023-04-02 10:25:22.994946 aiogram_forms-1.1.0/aiogram_forms/forms/__init__.py
--rw-r--r--   0        0        0     2647 2023-04-02 10:26:30.926978 aiogram_forms-1.1.0/aiogram_forms/forms/base.py
--rw-r--r--   0        0        0     3426 2023-04-02 10:26:30.927087 aiogram_forms-1.1.0/aiogram_forms/forms/fields.py
--rw-r--r--   0        0        0     3863 2023-04-02 10:50:41.557765 aiogram_forms-1.1.0/aiogram_forms/forms/manager.py
--rw-r--r--   0        0        0     2206 2023-04-02 10:26:30.927288 aiogram_forms-1.1.0/aiogram_forms/forms/validators.py
--rw-r--r--   0        0        0      869 2023-04-02 10:26:30.927384 aiogram_forms-1.1.0/aiogram_forms/middleware.py
--rw-r--r--   0        0        0      174 2023-04-02 10:26:30.927473 aiogram_forms-1.1.0/aiogram_forms/types.py
--rw-r--r--   0        0        0      354 2023-04-02 10:26:30.927560 aiogram_forms-1.1.0/aiogram_forms/utils.py
--rw-r--r--   0        0        0     1143 2023-04-02 10:40:26.879549 aiogram_forms-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 aiogram_forms-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-02 10:25:22.993494 aiogram_forms-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2591 2023-04-02 11:40:41.757982 aiogram_forms-1.1.1/README.md
+-rw-r--r--   0        0        0      231 2023-04-02 10:25:22.993770 aiogram_forms-1.1.1/aiogram_forms/__init__.py
+-rw-r--r--   0        0        0      102 2023-04-02 10:25:22.993883 aiogram_forms-1.1.1/aiogram_forms/const.py
+-rw-r--r--   0        0        0        0 2023-04-02 10:25:22.993996 aiogram_forms-1.1.1/aiogram_forms/core/__init__.py
+-rw-r--r--   0        0        0      864 2023-04-02 11:40:41.758190 aiogram_forms-1.1.1/aiogram_forms/core/entities.py
+-rw-r--r--   0        0        0      659 2023-04-02 11:40:41.758365 aiogram_forms-1.1.1/aiogram_forms/core/manager.py
+-rw-r--r--   0        0        0     1567 2023-04-02 10:25:22.994351 aiogram_forms-1.1.1/aiogram_forms/core/states.py
+-rw-r--r--   0        0        0     2564 2023-04-22 19:19:36.217502 aiogram_forms-1.1.1/aiogram_forms/dispatcher.py
+-rw-r--r--   0        0        0      568 2023-04-02 10:25:22.994575 aiogram_forms-1.1.1/aiogram_forms/enums.py
+-rw-r--r--   0        0        0      293 2023-04-02 10:25:22.994672 aiogram_forms-1.1.1/aiogram_forms/errors.py
+-rw-r--r--   0        0        0     1092 2023-04-02 11:40:41.758693 aiogram_forms-1.1.1/aiogram_forms/filters.py
+-rw-r--r--   0        0        0      179 2023-04-02 10:25:22.994946 aiogram_forms-1.1.1/aiogram_forms/forms/__init__.py
+-rw-r--r--   0        0        0     2673 2023-04-22 20:59:25.014289 aiogram_forms-1.1.1/aiogram_forms/forms/base.py
+-rw-r--r--   0        0        0     3431 2023-04-22 21:01:11.210230 aiogram_forms-1.1.1/aiogram_forms/forms/fields.py
+-rw-r--r--   0        0        0     3904 2023-04-22 21:00:51.539435 aiogram_forms-1.1.1/aiogram_forms/forms/manager.py
+-rw-r--r--   0        0        0     2206 2023-04-02 11:40:41.759529 aiogram_forms-1.1.1/aiogram_forms/forms/validators.py
+-rw-r--r--   0        0        0      869 2023-04-02 11:40:41.759669 aiogram_forms-1.1.1/aiogram_forms/middleware.py
+-rw-r--r--   0        0        0      174 2023-04-02 11:40:41.759822 aiogram_forms-1.1.1/aiogram_forms/types.py
+-rw-r--r--   0        0        0      354 2023-04-02 11:40:41.759956 aiogram_forms-1.1.1/aiogram_forms/utils.py
+-rw-r--r--   0        0        0     1143 2023-04-22 21:05:43.909656 aiogram_forms-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 aiogram_forms-1.1.1/PKG-INFO
```

### Comparing `aiogram_forms-1.1.0/LICENSE` & `aiogram_forms-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/README.md` & `aiogram_forms-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/core/entities.py` & `aiogram_forms-1.1.1/aiogram_forms/core/entities.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/core/manager.py` & `aiogram_forms-1.1.1/aiogram_forms/core/manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/core/states.py` & `aiogram_forms-1.1.1/aiogram_forms/core/states.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/dispatcher.py` & `aiogram_forms-1.1.1/aiogram_forms/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """Register entity with given name."""
         def wrapper(container: Type[EntityContainer]) -> Type[EntityContainer]:
             EntityContainerStatesGroup.bind(container)
 
             for filter_type, filter_ in container.filters().items():
                 getattr(self._router, str(filter_type.value))(filter_)(self._get_entity_container_handler(container))
 
-            if container.__name__ not in self._registry:
+            if 'forms' not in self._registry:
                 self._registry['forms'] = {}
 
             self._registry['forms'][name] = container
             return container
         return wrapper
 
     def get_entity_container(self, container_type: Type[EntityContainer], name: str) -> Type[EntityContainer]:
```

### Comparing `aiogram_forms-1.1.0/aiogram_forms/enums.py` & `aiogram_forms-1.1.1/aiogram_forms/enums.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/filters.py` & `aiogram_forms-1.1.1/aiogram_forms/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/forms/base.py` & `aiogram_forms-1.1.1/aiogram_forms/forms/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         types.InlineKeyboardMarkup,
         types.ReplyKeyboardMarkup,
         types.ReplyKeyboardRemove,
         types.ForceReply,
         None
     ]:
         """Field keyboard."""
-        return types.ReplyKeyboardRemove()
+        return types.ReplyKeyboardRemove()  # type: ignore[call-arg]
 
     async def extract(self, message: types.Message) -> Optional[str]:
         """Extract field value from message object."""
         return message.text
 
     async def process(self, value: Any) -> Any:
         """Process field value format."""
```

### Comparing `aiogram_forms-1.1.0/aiogram_forms/forms/fields.py` & `aiogram_forms-1.1.1/aiogram_forms/forms/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         types.ReplyKeyboardRemove,
         types.ForceReply,
         None
     ]:
         if self.share_contact:
             return types.ReplyKeyboardMarkup(
                 keyboard=[
-                    [types.KeyboardButton(text=self.label, request_contact=True)]
+                    [types.KeyboardButton(text=str(self.label), request_contact=True)]
                 ],
                 resize_keyboard=True
             )
         return super().reply_keyboard
 
     async def extract(self, message: types.Message) -> Optional[str]:
         if message.content_type == 'contact':
```

### Comparing `aiogram_forms-1.1.0/aiogram_forms/forms/manager.py` & `aiogram_forms-1.1.1/aiogram_forms/forms/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.state = self.data['state']
 
     async def show(self, name: str) -> None:
         entity_container: Type['Form'] = self._get_form_by_name(name)
 
         first_entity = cast(Field, entity_container.state.get_states()[0].entity)
         await self.state.set_state(first_entity.state)
-        await self.event.answer(first_entity.label, reply_markup=first_entity.reply_keyboard)
+        await self.event.answer(first_entity.label, reply_markup=first_entity.reply_keyboard)  # type: ignore[arg-type]
 
     async def handle(self, form: Type['Form']) -> None:
         """Handle form field."""
         state_label = await self.state.get_state()
         current_state: 'EntityState' = next(iter([
             st for st in form.state.get_states() if st.state == state_label
         ]))
@@ -38,35 +38,35 @@
         try:
             value = await field.process(
                 await field.extract(self.event)
             )
             await field.validate(value)
         except ValidationError as error:
             error_message = field.error_messages.get(error.code) or error.message
-            await self.event.answer(error_message, reply_markup=field.reply_keyboard)
+            await self.event.answer(error_message, reply_markup=field.reply_keyboard)  # type: ignore[arg-type]
             return
 
         data = await self.state.get_data()
         form_data = data.get(form.__name__, {})
         form_data.update({field.state.state.split(':')[-1]: value})  # type: ignore[union-attr]
         await self.state.update_data({form.__name__: form_data})
 
         next_state_index = cast(
             Dict['EntityState', Optional['EntityState']],
-            dict(zip(current_state.group, list(current_state.group)[1:]))  # type: ignore[arg-type]
+            dict(zip(current_state.group, list(current_state.group)[1:]))
         )
         next_entity_state: Optional['EntityState'] = next_state_index.get(current_state)
         if next_entity_state:
             next_field: Field = cast(Field, next_entity_state.entity)
             await self.state.set_state(next_field.state)
             await self.event.answer(
                 '\n'.join([
-                    next_field.label,
-                    next_field.help_text or ""
-                ] if next_field.help_text else [next_field.label]),
+                    str(next_field.label),
+                    str(next_field.help_text) or ""
+                ] if next_field.help_text else [str(next_field.label)]),
                 reply_markup=next_field.reply_keyboard
             )
         else:
             await self.state.set_state(None)
             await form.callback(self.event, **self.data)
 
     async def get_data(self, form: Union[Type['Form'], str]) -> Dict[str, Any]:
```

### Comparing `aiogram_forms-1.1.0/aiogram_forms/forms/validators.py` & `aiogram_forms-1.1.1/aiogram_forms/forms/validators.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/aiogram_forms/middleware.py` & `aiogram_forms-1.1.1/aiogram_forms/middleware.py`

 * *Files identical despite different names*

### Comparing `aiogram_forms-1.1.0/pyproject.toml` & `aiogram_forms-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiogram-forms"
-version = "1.1.0"
+version = "1.1.1"
 description = "Forms for aiogram"
 authors = ["Ivan Borisenko <i.13g10n@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://13g10n.com/docs/aiogram-forms"
 repository = "https://github.com/13g10n/aiogram-forms"
 classifiers = [
```

### Comparing `aiogram_forms-1.1.0/PKG-INFO` & `aiogram_forms-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-forms
-Version: 1.1.0
+Version: 1.1.1
 Summary: Forms for aiogram
 Home-page: https://13g10n.com/docs/aiogram-forms
 License: MIT
 Keywords: aiogram,telegram,forms
 Author: Ivan Borisenko
 Author-email: i.13g10n@icloud.com
 Requires-Python: >=3.8,<4.0
```

