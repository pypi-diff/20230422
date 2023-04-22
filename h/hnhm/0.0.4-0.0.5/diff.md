# Comparing `tmp/hnhm-0.0.4.tar.gz` & `tmp/hnhm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnhm-0.0.4.tar", max compression
+gzip compressed data, was "hnhm-0.0.5.tar", max compression
```

## Comparing `hnhm-0.0.4.tar` & `hnhm-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      707 2023-04-10 21:45:28.420638 hnhm-0.0.4/hnhm/__init__.py
--rw-r--r--   0        0        0     5189 2023-04-10 21:45:28.420638 hnhm-0.0.4/hnhm/cli.py
--rw-r--r--   0        0        0      551 2023-04-10 21:45:28.420638 hnhm-0.0.4/hnhm/core/__init__.py
--rw-r--r--   0        0        0     1084 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/attribute.py
--rw-r--r--   0        0        0      554 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/entity.py
--rw-r--r--   0        0        0       80 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/error.py
--rw-r--r--   0        0        0      311 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/group.py
--rw-r--r--   0        0        0      543 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/layout.py
--rw-r--r--   0        0        0      654 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/link.py
--rw-r--r--   0        0        0     1724 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/mutations.py
--rw-r--r--   0        0        0       80 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/priority.py
--rw-r--r--   0        0        0      511 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/sql.py
--rw-r--r--   0        0        0      621 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/storage.py
--rw-r--r--   0        0        0     1545 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/core/tasks.py
--rw-r--r--   0        0        0      564 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/file_storage.py
--rw-r--r--   0        0        0     7561 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/flow.py
--rw-r--r--   0        0        0     9084 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/hnhm.py
--rw-r--r--   0        0        0      902 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/hnhm_attribute.py
--rw-r--r--   0        0        0     3682 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/hnhm_entity.py
--rw-r--r--   0        0        0     2547 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/hnhm_link.py
--rw-r--r--   0        0        0      419 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/hnhm_registry.py
--rw-r--r--   0        0        0        0 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/__init__.py
--rw-r--r--   0        0        0    12233 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql.py
--rw-r--r--   0        0        0      459 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/__init__.py
--rw-r--r--   0        0        0      456 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/create_attribute.py
--rw-r--r--   0        0        0      477 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/create_group.py
--rw-r--r--   0        0        0      272 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/create_hub.py
--rw-r--r--   0        0        0      504 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/create_link.py
--rw-r--r--   0        0        0      228 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/create_stage.py
--rw-r--r--   0        0        0      425 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/load_hub.py
--rw-r--r--   0        0        0      905 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/load_ignore.py
--rw-r--r--   0        0        0     4326 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/load_new.py
--rw-r--r--   0        0        0     1905 2023-04-10 21:45:28.424638 hnhm-0.0.4/hnhm/postgres/sql_templates/load_update.py
--rw-r--r--   0        0        0      707 2023-04-10 21:45:28.424638 hnhm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      707 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/__init__.py
+-rw-r--r--   0        0        0     5725 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/cli.py
+-rw-r--r--   0        0        0      600 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/attribute.py
+-rw-r--r--   0        0        0      554 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/entity.py
+-rw-r--r--   0        0        0       80 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/error.py
+-rw-r--r--   0        0        0      311 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/group.py
+-rw-r--r--   0        0        0      543 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/layout.py
+-rw-r--r--   0        0        0      654 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/link.py
+-rw-r--r--   0        0        0     2493 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/mutations.py
+-rw-r--r--   0        0        0       80 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/priority.py
+-rw-r--r--   0        0        0      511 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/sql.py
+-rw-r--r--   0        0        0      621 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/storage.py
+-rw-r--r--   0        0        0     1545 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/core/tasks.py
+-rw-r--r--   0        0        0      564 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/file_storage.py
+-rw-r--r--   0        0        0     7561 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/flow.py
+-rw-r--r--   0        0        0    11451 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm.py
+-rw-r--r--   0        0        0      902 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_attribute.py
+-rw-r--r--   0        0        0     3865 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_entity.py
+-rw-r--r--   0        0        0     2547 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_link.py
+-rw-r--r--   0        0        0     1297 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/hnhm_registry.py
+-rw-r--r--   0        0        0        0 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/__init__.py
+-rw-r--r--   0        0        0    13167 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql.py
+-rw-r--r--   0        0        0      459 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/__init__.py
+-rw-r--r--   0        0        0      528 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_attribute.py
+-rw-r--r--   0        0        0      549 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_group.py
+-rw-r--r--   0        0        0      344 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_hub.py
+-rw-r--r--   0        0        0      576 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_link.py
+-rw-r--r--   0        0        0      228 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/create_stage.py
+-rw-r--r--   0        0        0      507 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_hub.py
+-rw-r--r--   0        0        0      983 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_ignore.py
+-rw-r--r--   0        0        0     4563 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_new.py
+-rw-r--r--   0        0        0     2139 2023-04-22 10:35:50.042288 hnhm-0.0.5/hnhm/postgres/sql_templates/load_update.py
+-rw-r--r--   0        0        0      707 2023-04-22 10:35:50.042288 hnhm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.5/PKG-INFO
```

### Comparing `hnhm-0.0.4/hnhm/__init__.py` & `hnhm-0.0.5/hnhm/__init__.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/cli.py` & `hnhm-0.0.5/hnhm/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
+    AddGroupAttribute,
+    RemoveGroupAttribute,
 )
 
 
 def import_registry(module: str) -> HnhmRegistry:
     sys.path.append(".")
     imported_module = importlib.import_module(module)
     registry: HnhmRegistry = getattr(imported_module, "__registry__", None)
@@ -65,14 +67,18 @@
                     click.secho(f"  + attribute '{attribute.name}'", fg="green")
 
                 case CreateGroup(entity=_, group=group):
                     click.secho(f"  + group '{group.name}'", fg="green")
                     for attribute in group.attributes.values():
                         click.secho(f"    |attribute '{attribute.name}'", fg="green")
 
+                case AddGroupAttribute(entity=_, group=group, attribute=attribute):
+                    click.secho(f"  [u] group '{group.name}'", fg="yellow")
+                    click.secho(f"    +attribute '{attribute.name}'", fg="green")
+
                 case RemoveEntity(entity=entity):
                     if entity.layout.type == LayoutType.HNHM:
                         click.secho(f"  - hub '{entity.name}'", fg="red")
                     else:
                         click.secho(f"  - stage '{entity.name}'", fg="red")
                         for attribute in entity.attributes.values():
                             click.secho(f"    |attribute '{attribute.name}'", fg="red")
@@ -81,14 +87,18 @@
                     click.secho(f"  - attribute '{attribute.name}'", fg="red")
 
                 case RemoveGroup(entity=_, group=group):
                     click.secho(f"  - group '{group.name}'", fg="red")
                     for attribute in group.attributes.values():
                         click.secho(f"    | attribute '{attribute.name}'", fg="red")
 
+                case RemoveGroupAttribute(entity=_, group=group, attribute=attribute):
+                    click.secho(f"  [u] group '{group.name}'", fg="yellow")
+                    click.secho(f"    -attribute '{attribute.name}'", fg="red")
+
     for link_name, plan_collection in links_mutations:
         if plan_collection.type == PlanType.CREATE:
             symbol, color = "+", "green"
         elif plan_collection.type == PlanType.REMOVE:
             symbol, color = "-", "red"
         elif plan_collection.type == PlanType.UPDATE:
             symbol, color = "[u]", "yellow"
```

### Comparing `hnhm-0.0.4/hnhm/core/__init__.py` & `hnhm-0.0.5/hnhm/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,10 @@
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
+    AddGroupAttribute,
+    RemoveGroupAttribute,
 )
```

### Comparing `hnhm-0.0.4/hnhm/core/attribute.py` & `hnhm-0.0.5/hnhm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/core/entity.py` & `hnhm-0.0.5/hnhm/core/entity.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/core/layout.py` & `hnhm-0.0.5/hnhm/core/layout.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/core/link.py` & `hnhm-0.0.5/hnhm/core/link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/core/storage.py` & `hnhm-0.0.5/hnhm/core/storage.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/core/tasks.py` & `hnhm-0.0.5/hnhm/core/tasks.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/file_storage.py` & `hnhm-0.0.5/hnhm/file_storage.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/flow.py` & `hnhm-0.0.5/hnhm/flow.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/hnhm.py` & `hnhm-0.0.5/hnhm/hnhm.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
+    AddGroupAttribute,
+    RemoveGroupAttribute,
 )
 
 from .hnhm_link import HnhmLink
 from .hnhm_entity import HnhmEntity
 
 
 class PlanType(str, Enum):
@@ -99,39 +101,56 @@
                     mutations.append(CreateGroup(entity=entity, group=group))
 
             plan.entities_mutations[entity.name] = PlanCollection(
                 type=PlanType.CREATE,
                 mutations=mutations,
             )
 
-        # Entity: create/remove Attribute/Group
+        # Entity: create/remove/update Attribute/Group
         for entity in core_entities.values():
             if entity.name not in self.data.entities:
                 continue
 
-            if entity.layout.type != LayoutType.HNHM:
-                continue
-
             attributes_state = self.data.entities[entity.name].attributes
             groups_state = self.data.entities[entity.name].groups
 
             mutations = []
             # Create Attribute
             for attribute_name, attribute in entity.attributes.items():
                 if attribute_name not in attributes_state:
                     mutations.append(CreateAttribute(entity=entity, attribute=attribute))
 
             # Remove Attribute
             for attribute_name, attribute in attributes_state.items():
                 if attribute_name not in entity.attributes:
                     mutations.append(RemoveAttribute(entity=entity, attribute=attribute))
 
-            # Create Group
+            # Create/Update Group
             for group_name, group in entity.groups.items():
-                if group_name not in groups_state:
+                # Update
+                if group_name in groups_state:
+                    group_state = groups_state[group_name]
+                    # Add an Attribute to a Group
+                    for attribute_name, attribute in group.attributes.items():
+                        if attribute_name not in group_state.attributes:
+                            mutations.append(
+                                AddGroupAttribute(
+                                    entity=entity, group=group, attribute=attribute
+                                )
+                            )
+                    # Remove an Attribute from a Group
+                    for attribute_name, attribute in group_state.attributes.items():
+                        if attribute_name not in group.attributes:
+                            mutations.append(
+                                RemoveGroupAttribute(
+                                    entity=entity, group=group, attribute=attribute
+                                )
+                            )
+                # Create
+                else:
                     mutations.append(CreateGroup(entity=entity, group=group))
 
             # Remove Group
             for group_name, group in groups_state.items():
                 if group_name not in entity.groups:
                     mutations.append(RemoveGroup(entity=entity, group=group))
 
@@ -232,14 +251,44 @@
 
                 case RemoveGroup(entity=entity, group=group):
                     assert entity.name in self.data.entities
                     assert group.name in self.data.entities[entity.name].groups
                     self.sql.execute(sql)
                     del self.data.entities[entity.name].groups[group.name]
 
+                case AddGroupAttribute(entity=entity, group=group, attribute=attribute):
+                    assert entity.name in self.data.entities
+                    assert group.name in self.data.entities[entity.name].groups
+                    assert (
+                        attribute.name
+                        not in self.data.entities[entity.name]
+                        .groups[group.name]
+                        .attributes
+                    )
+                    self.sql.execute(sql)
+                    self.data.entities[entity.name].groups[group.name].attributes[
+                        attribute.name
+                    ] = attribute
+
+                case RemoveGroupAttribute(
+                    entity=entity, group=group, attribute=attribute
+                ):
+                    assert entity.name in self.data.entities
+                    assert group.name in self.data.entities[entity.name].groups
+                    assert (
+                        attribute.name
+                        in self.data.entities[entity.name].groups[group.name].attributes
+                    )
+                    self.sql.execute(sql)
+                    del (
+                        self.data.entities[entity.name]
+                        .groups[group.name]
+                        .attributes[attribute.name]
+                    )
+
                 case CreateLink(link=link):
                     assert link.name not in self.data.links
                     self.sql.execute(sql)
                     self.data.links[link.name] = link
 
                 case RemoveLink(link=link):
                     assert link.name in self.data.links
```

### Comparing `hnhm-0.0.4/hnhm/hnhm_attribute.py` & `hnhm-0.0.5/hnhm/hnhm_attribute.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/hnhm_entity.py` & `hnhm-0.0.5/hnhm/hnhm_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,57 +9,59 @@
 class HnhmEntity(abc.ABC):
     __layout__: Layout = None
     __keys__: list[HnhmAttribute] | None = None
 
     def to_core(self) -> Entity:
         inspected = dict(inspect.getmembers(self))
 
-        if "__layout__" not in inspected or not inspected["__layout__"]:
+        if not inspected.get("__layout__"):
             raise HnhmError(
                 f"Layout not found for entity: '{self}'."
                 " Please, specify Layout via '__layout__' attribute."
             )
         layout: Layout = inspected["__layout__"]
         if not layout.type:
             raise HnhmError(
                 f"Type for Layout '{layout}' is required for entity."
                 " Please, specify LayoutType via 'type' attribute."
             )
 
         name = layout.name
 
-        if "__doc__" not in inspected or not inspected["__doc__"]:
+        if not inspected.get("__doc__"):
             raise HnhmError(
-                f"Doc not found or empty for entity: '{name}'."
+                f"Doc not found or empty for entity: '{layout.type}.{name}'."
                 " Please, write a documentation for your entity."
             )
         doc: str = inspected["__doc__"]
 
         match layout.type:
             case LayoutType.STAGE:
                 keys = []
 
             case LayoutType.HNHM:
-                if "__keys__" not in inspected or not inspected["__keys__"]:
+                if not inspected.get("__keys__"):
                     raise HnhmError(
-                        f"At least one Key is required for entity '{self}' with Layout.type='{LayoutType.HNHM}'."
+                        f"At least one Key is required for entity '{layout.type}.{name}'."
                         " Please, specify entity's keys via the '__keys__' attribute."
                     )
 
                 keys_hnhm: list[HnhmAttribute] = inspected["__keys__"]
                 for key in keys_hnhm:
                     if key.change_type != ChangeType.IGNORE:
                         raise HnhmError(
                             f"Change type='{key.change_type}' is not supported for Key attributes."
-                            f" Please, use 'ChangeType.IGNORE' for the key attributes in the '{self}' entity."
+                            f" Use 'ChangeType.IGNORE' for the key attributes in the '{layout.type}.{name}' entity."
                         )
 
                 keys = [key.to_core() for key in keys_hnhm]
                 if len(keys) != len(set(keys)):
-                    raise HnhmError(f"Found duplicated keys for entity: '{self}'.")
+                    raise HnhmError(
+                        f"Found duplicated keys for entity: '{layout.type}.{name}'."
+                    )
 
             case _:
                 raise HnhmError(f"Unknown LayoutType='{layout.type}'")
 
         groups = {}
         attributes = {}
         for class_attribute in inspected.values():
@@ -76,22 +78,27 @@
                         name=group_name,
                         attributes={attribute_name: attribute},
                         change_type=attribute.change_type,
                     )
 
                 if groups[group_name].change_type != attribute.change_type:
                     raise HnhmError(
-                        f"Found conflicting ChangeType for the entity='{name}' group ='{group_name}'."
+                        f"Found conflicting ChangeType for the entity='{layout.type}.{name}' group='{group_name}'."
                         " Please, use single ChangeType for all attributes within the same group."
                     )
                 groups[group_name].attributes[attribute_name] = attribute
 
             elif attribute not in keys:
                 attributes[attribute_name] = attribute
 
+        if layout.type == LayoutType.STAGE and len(attributes) < 1:
+            raise HnhmError(
+                f"Entity='{layout.type}.{name}' should have at least 1 attribute."
+            )
+
         return Entity(
             name=name,
             layout=layout,
             doc=doc,
             keys=keys,
             attributes=attributes,
             groups=groups,
```

### Comparing `hnhm-0.0.4/hnhm/hnhm_link.py` & `hnhm-0.0.5/hnhm/hnhm_link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.4/hnhm/postgres/sql.py` & `hnhm-0.0.5/hnhm/postgres/sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     LoadAttribute,
     CreateAttribute,
     RemoveAttribute,
+    AddGroupAttribute,
+    RemoveGroupAttribute,
 )
 
 from .sql_templates import (
     SQL_TEMPLATE__LOAD_HUB,
     SQL_TEMPLATE__LOAD_NEW,
     SQL_TEMPLATE__CREATE_HUB,
     SQL_TEMPLATE__CREATE_LINK,
@@ -72,14 +74,17 @@
                 columns=columns,
                 columns_types=columns_types,
             )
 
         case CreateAttribute(entity=entity, attribute=attribute):
             attribute_type = PG_TYPES[attribute.type]
 
+            if entity.layout.type == LayoutType.STAGE:
+                return f"ALTER TABLE stg__{entity.name} ADD COLUMN {attribute.name} {attribute_type}"
+
             time_columns = ["valid_from TIMESTAMPTZ NOT NULL"]
             if attribute.change_type == ChangeType.NEW:
                 time_columns.append("valid_to TIMESTAMPTZ")
 
             template = jinja.from_string(SQL_TEMPLATE__CREATE_ATTRIBUTE)
             return template.render(
                 entity_name=entity.name,
@@ -102,14 +107,18 @@
             return template.render(
                 entity_name=entity.name,
                 group_name=group.name,
                 columns=columns,
                 time_columns=time_columns,
             )
 
+        case AddGroupAttribute(entity=entity, group=group, attribute=attribute):
+            attribute_type = PG_TYPES[attribute.type]
+            return f"ALTER TABLE group__{entity.name}__{group.name} ADD COLUMN {attribute.name} {attribute_type}"
+
         case CreateLink(link=link):
             entities = []
             for link_element in link.elements:
                 entities.append(link_element.entity.name)
 
             primary_keys = ["valid_from"]
             for key in link.keys:
@@ -126,19 +135,25 @@
             if entity.layout.type == LayoutType.HNHM:
                 table_name = f"hub__{entity.name}"
             else:
                 table_name = f"stg__{entity.name}"
             return f"DROP TABLE {table_name}"
 
         case RemoveAttribute(entity=entity, attribute=attribute):
+            if entity.layout.type == LayoutType.STAGE:
+                return f"ALTER TABLE stg__{entity.name} DROP COLUMN {attribute.name}"
+
             return f"DROP TABLE attr__{entity.name}__{attribute.name}"
 
         case RemoveGroup(entity=entity, group=group):
             return f"DROP TABLE group__{entity.name}__{group.name}"
 
+        case RemoveGroupAttribute(entity=entity, group=group, attribute=attribute):
+            return f"ALTER TABLE group__{entity.name}__{group.name} DROP COLUMN {attribute.name}"
+
         case RemoveLink(link=link):
             return f"DROP TABLE link__{link.name}"
 
         case LoadHub(
             source=source,
             target=target,
             business_time_field=business_time_field,
@@ -335,11 +350,18 @@
     def generate_sql(self, mutation_or_task: Mutation | Task) -> str:
         return generate_sql(mutation_or_task, self.jinja)
 
     def execute(self, sql: str, debug: bool = False):
         if debug:
             print(dedent(sql).strip())
 
-        with self.engine.connect() as conn:
+        conn = None
+        try:
+            conn = self.engine.connect()
             conn.execute(text(sql))
             conn.commit()
-        self.engine.dispose()
+        except Exception as e:
+            raise e
+        finally:
+            if conn:
+                conn.close()
+            self.engine.dispose()
```

### Comparing `hnhm-0.0.4/hnhm/postgres/sql_templates/load_ignore.py` & `hnhm-0.0.5/hnhm/postgres/sql_templates/load_ignore.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,22 +16,26 @@
         {{ source_table }}
 )
 INSERT INTO {{ target_table }}(
     {{ target_sk }},
     {% for target_attribute in target_attributes -%}
     {{ target_attribute }},
     {% endfor -%}
-    valid_from
+    valid_from,
+    _source,
+    _loaded_at
 )
 SELECT
     d.sk,
     {% for source_attribute in source_attributes -%}
         d.{{ source_attribute }},
     {% endfor -%}
-    d.valid_from
+    d.valid_from,
+    '{{ source_table }}',
+    CURRENT_TIMESTAMP
 FROM
     data d
 LEFT OUTER JOIN
     {{ target_table }} t
     ON d.sk = t.{{ target_sk }}
 WHERE
     t.{{ target_sk }} IS NULL
```

### Comparing `hnhm-0.0.4/hnhm/postgres/sql_templates/load_new.py` & `hnhm-0.0.5/hnhm/postgres/sql_templates/load_new.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,17 @@
         d1.{{ target_attribute }},
     {% endfor -%}
 
     d1.valid_from,
     CASE
         WHEN d2.valid_from IS NULL THEN 'infinity'
         ELSE d2.valid_from
-    END AS valid_to
+    END AS valid_to,
+    '{{ source_table }}' AS _source,
+    CURRENT_TIMESTAMP AS _loaded_at
 FROM
     data d1
 LEFT JOIN
     data d2
     ON d1.row_number = d2.row_number - 1
 
     {% for target_sk in target_sks -%}
@@ -96,15 +98,17 @@
         {% endfor -%}
 
         {% for target_attribute in target_attributes -%}
             tmp.{{ target_attribute }},
         {% endfor -%}
 
         tmp.valid_from,
-        tmp.valid_to
+        tmp.valid_to,
+        tmp._source,
+        tmp._loaded_at
     FROM
         _tmp__{{ target_table }}__load__new tmp
     LEFT OUTER JOIN
         {{ target_table }} t
         ON (
             {% for where_element in (target_sks+target_attributes+extra_sks) -%}
                 COALESCE(t.{{ where_element }}::TEXT, 'null')
@@ -124,31 +128,37 @@
 )
 INSERT INTO {{ target_table }}(
     {{ target_sks | join(', ') }},
     {% for target_attribute in target_attributes -%}
         {{ target_attribute }},
     {% endfor -%}
     valid_from,
-    valid_to
+    valid_to,
+    _source,
+    _loaded_at
 )
 SELECT
     {{ target_sks | join(', ') }},
     {% for target_attribute in target_attributes -%}
         {{ target_attribute }},
     {% endfor -%}
     valid_from,
-    valid_to
+    valid_to,
+    _source,
+    _loaded_at
 FROM
     inserts;
 
 
 UPDATE {{ target_table }} t
 SET
     valid_from = tmp.valid_from,
-    valid_to = tmp.valid_to
+    valid_to = tmp.valid_to,
+    _source = tmp._source,
+    _loaded_at = tmp._loaded_at
 FROM
     _tmp__{{ target_table }}__load__new tmp
 WHERE
     (
         {% for where_element in (target_sks+target_attributes+extra_sks) -%}
             COALESCE(t.{{ where_element }}::TEXT, 'null')
             {% if not loop.last %} || '-' || {% endif %}
```

### Comparing `hnhm-0.0.4/hnhm/postgres/sql_templates/load_update.py` & `hnhm-0.0.5/hnhm/postgres/sql_templates/load_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,42 @@
     {% for source_attribute in source_attributes -%}
         {{ source_attribute }},
     {% endfor -%}
 
     ROW_NUMBER() OVER (
         PARTITION BY {{ source_sk }}
         ORDER BY     {{ business_time_field }} DESC
-    ) AS row_number
+    ) AS row_number,
+    '{{ source_table }}' AS _source,
+    CURRENT_TIMESTAMP AS _loaded_at 
 FROM
     {{ source_table }};
 
 
 INSERT INTO {{ target_table }}(
     {{ target_sk }},
 
     {% for target_attribute in target_attributes -%}
         {{ target_attribute }},
     {% endfor -%}
 
-    valid_from
+    valid_from,
+    _source,
+    _loaded_at
 )
 SELECT
     d.sk,
 
     {% for source_attribute in source_attributes -%}
         d.{{ source_attribute }},
     {% endfor -%}
 
-    d.valid_from
+    d.valid_from,
+    d._source,
+    d._loaded_at
 FROM
     tmp__{{ target_table }}__load__update d
 LEFT OUTER JOIN
     {{ target_table }} t
     ON d.sk = t.{{ target_sk }}
 WHERE
     t.{{ target_sk }} IS NULL
@@ -48,15 +54,17 @@
 
 WITH updates AS (
     SELECT
         d.sk,
         {% for source_attribute in source_attributes -%}
             d.{{ source_attribute }},
         {% endfor -%}
-        d.valid_from
+        d.valid_from,
+        d._source,
+        d._loaded_at
     FROM
         tmp__{{ target_table }}__load__update d
     INNER JOIN
         {{ target_table }} t
         ON d.sk = t.{{ target_sk }}
     WHERE
         {% for source_attribute, target_attribute in zip(source_attributes, target_attributes) -%}
@@ -67,15 +75,17 @@
 )
 UPDATE
     {{ target_table }}
 SET
     {% for source_attribute, target_attribute in zip(source_attributes, target_attributes) -%}
         {{ target_attribute }} = u.{{ source_attribute }},
     {% endfor -%}
-    valid_from = u.valid_from
+    valid_from = u.valid_from,
+    _source = u._source,
+    _loaded_at = u._loaded_at
 FROM
     updates u
 WHERE
     {{ target_sk }} = u.sk;
 
 DROP TABLE tmp__{{ target_table }}__load__update;
```

### Comparing `hnhm-0.0.4/pyproject.toml` & `hnhm-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hnhm"
-version = "0.0.4"
+version = "0.0.5"
 description = "hNhM – highly Normalized hybrid Model."
 authors = ["Arseny Egorov <egoroff-ars@yandex.ru>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "1.10.7"
 click = "8.1.3"
 Jinja2 = "3.1.2"
 SQLAlchemy = "2.0.9"
 psycopg2-binary = "2.9.6"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "3.2.2"
-pytest = "7.3.0"
+pytest = "7.3.1"
 pytest-cov = "4.0.0"
 pygount = "1.5.1"
 pandas = "2.0.0"
 
 [tool.poetry.scripts]
 hnhm = "hnhm.cli:cli"
```

