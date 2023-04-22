# Comparing `tmp/tcod-ecs-1.0.0.tar.gz` & `tmp/tcod-ecs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod-ecs-1.0.0.tar", last modified: Wed Apr 12 01:34:08 2023, max compression
+gzip compressed data, was "tcod-ecs-1.1.0.tar", last modified: Sat Apr 22 05:31:06 2023, max compression
```

## Comparing `tcod-ecs-1.0.0.tar` & `tcod-ecs-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-1.0.0/.flake8
--rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-1.0.0/.gitattributes
--rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1706 2023-04-09 03:23:14.272745 tcod-ecs-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-1.0.0/.gitignore
--rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-1.0.0/.readthedocs.yml
--rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-1.0.0/.vscode/launch.json
--rw-r--r--   0        0        0     1493 2023-04-12 00:56:27.890449 tcod-ecs-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-1.0.0/.vscode/tasks.json
--rw-r--r--   0        0        0      327 2023-04-12 01:32:27.757712 tcod-ecs-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-1.0.0/LICENSE
--rw-r--r--   0        0        0     8642 2023-04-12 01:06:47.372874 tcod-ecs-1.0.0/README.md
--rw-r--r--   0        0        0      581 2023-04-12 01:13:36.306949 tcod-ecs-1.0.0/conftest.py
--rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-1.0.0/docs/api.rst
--rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-1.0.0/docs/conf.py
--rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-1.0.0/docs/head.md
--rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-1.0.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-1.0.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     3569 2023-04-12 01:31:24.101693 tcod-ecs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    29235 2023-04-12 01:30:58.631013 tcod-ecs-1.0.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     7285 2023-04-12 01:13:36.373623 tcod-ecs-1.0.0/tcod/ecs/test_ecs.py
--rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 tcod-ecs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-1.1.0/.flake8
+-rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-1.1.0/.gitattributes
+-rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1706 2023-04-09 03:23:14.272745 tcod-ecs-1.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-1.1.0/.gitignore
+-rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-1.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0     1493 2023-04-12 00:56:27.890449 tcod-ecs-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-1.1.0/.vscode/tasks.json
+-rw-r--r--   0        0        0      550 2023-04-22 05:22:42.237610 tcod-ecs-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8642 2023-04-12 01:06:47.372874 tcod-ecs-1.1.0/README.md
+-rw-r--r--   0        0        0      581 2023-04-12 01:13:36.306949 tcod-ecs-1.1.0/conftest.py
+-rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-1.1.0/docs/api.rst
+-rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-1.1.0/docs/conf.py
+-rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-1.1.0/docs/head.md
+-rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-1.1.0/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-1.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     3569 2023-04-12 08:17:44.588593 tcod-ecs-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    31850 2023-04-22 05:23:44.626693 tcod-ecs-1.1.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     7530 2023-04-22 01:26:15.421648 tcod-ecs-1.1.0/tcod/ecs/test_ecs.py
+-rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 tcod-ecs-1.1.0/PKG-INFO
```

### Comparing `tcod-ecs-1.0.0/.gitattributes` & `tcod-ecs-1.1.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/.github/workflows/python-package.yml` & `tcod-ecs-1.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/.gitignore` & `tcod-ecs-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/.readthedocs.yml` & `tcod-ecs-1.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/.vscode/launch.json` & `tcod-ecs-1.1.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/.vscode/settings.json` & `tcod-ecs-1.1.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/.vscode/tasks.json` & `tcod-ecs-1.1.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/LICENSE` & `tcod-ecs-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/README.md` & `tcod-ecs-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/conftest.py` & `tcod-ecs-1.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/docs/Makefile` & `tcod-ecs-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/docs/conf.py` & `tcod-ecs-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/docs/make.bat` & `tcod-ecs-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/pyproject.toml` & `tcod-ecs-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcod-ecs-1.0.0/tcod/ecs/__init__.py` & `tcod-ecs-1.1.0/tcod/ecs/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A type-hinted Entity Component System based on Python dictionaries and sets."""
 from __future__ import annotations
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 import sys
 from functools import partial
 from typing import (
     AbstractSet,
     Any,
     DefaultDict,
     Final,
@@ -32,14 +32,15 @@
 T = TypeVar("T")
 _T1 = TypeVar("_T1")
 _T2 = TypeVar("_T2")
 _T3 = TypeVar("_T3")
 _T4 = TypeVar("_T4")
 _T5 = TypeVar("_T5")
 _ComponentKey = Union[Type[T], Tuple[object, Type[T]]]
+"""ComponentKey is plain `type` or tuple `(tag, type)`."""
 
 
 def abstract_component(cls: type[T]) -> type[T]:
     """Register class `cls` as an abstract component and return it."""
     cls._TCOD_BASE_COMPONENT = cls  # type: ignore[attr-defined]
     return cls
 
@@ -167,14 +168,18 @@
     def __repr__(self) -> str:
         """Return a representation of this entity."""
         items = [self.__class__.__name__]
         name = self.name
         items.append(f"0x{id(self):X}" if name is None else f"name={name!r}")
         return f"<{' '.join(items)}>"
 
+    def __reduce__(self) -> tuple[type[Entity], tuple[World]]:  # Private function.  # noqa: D105
+        # Note: This was added after version 1.0.0, objects pickled in <=1.0.0 will call __setstate__.
+        return self.__class__, (self.world,)
+
 
 class EntityComponents(MutableMapping[Union[Type[Any], Tuple[object, Type[Any]]], Any]):
     """A proxy attribute to access an entities components like a dictionary.
 
     See :any:`Entity.components`.
     """
 
@@ -291,32 +296,32 @@
     def __init__(self, entity: Entity, key: object) -> None:
         """Initialize this attribute for the given entity."""
         self.entity: Final = entity
         self.key: Final = key
         assert key not in {None, Ellipsis}
 
     def add(self, target: Entity) -> None:
-        """Add a relation target to this key."""
+        """Add a relation target to this tag."""
         world = self.entity.world
-        world._relations_by_key[self.key][self.entity].add(target)
+        world._relation_tags_by_entity[self.entity][self.key].add(target)
 
         world._relations_lookup[(self.key, target)].add(self.entity)
         world._relations_lookup[(self.key, ...)].add(self.entity)
         world._relations_lookup[(self.entity, self.key, None)].add(target)
         world._relations_lookup[(..., self.key, None)].add(target)
 
     def discard(self, target: Entity) -> None:
-        """Discard a relation target from this key."""
+        """Discard a relation target from this tag."""
         world = self.entity.world
 
-        world._relations_by_key[self.key][self.entity].discard(target)
-        if not world._relations_by_key[self.key][self.entity]:
-            del world._relations_by_key[self.key][self.entity]
-            if not world._relations_by_key[self.key]:
-                del world._relations_by_key[self.key]
+        world._relation_tags_by_entity[self.entity][self.key].discard(target)
+        if not world._relation_tags_by_entity[self.entity][self.key]:
+            del world._relation_tags_by_entity[self.entity][self.key]
+            if not world._relation_tags_by_entity[self.entity]:
+                del world._relation_tags_by_entity[self.entity]
 
         world._relations_lookup[(self.key, target)].discard(self.entity)
         if not world._relations_lookup[(self.key, target)]:
             del world._relations_lookup[(self.key, target)]
 
         world._relations_lookup[(self.key, ...)].discard(self.entity)
         if not world._relations_lookup[(self.key, ...)]:
@@ -331,22 +336,22 @@
             del world._relations_lookup[(..., self.key, None)]
 
     def __contains__(self, target: Entity) -> bool:  # type: ignore[override]
         """Return True if this relation contains the given value."""
         return bool(self.entity.world._relations_lookup.get((self.key, target), ()))
 
     def __iter__(self) -> Iterator[Entity]:
-        """Iterate over this relations targets."""
-        relations = self.entity.world._relations_by_key.get(self.key)
-        return iter(relations.get(self.entity, ())) if relations is not None else iter(())
+        """Iterate over this relation tags targets."""
+        by_entity = self.entity.world._relation_tags_by_entity.get(self.entity)
+        return iter(by_entity.get(self.key, ())) if by_entity is not None else iter(())
 
     def __len__(self) -> int:
-        """Return the number of targets in this relation."""
-        relations = self.entity.world._relations_by_key.get(self.key)
-        return len(relations.get(self.entity, ())) if relations is not None else 0
+        """Return the number of targets for this relation tag."""
+        by_entity = self.entity.world._relation_tags_by_entity.get(self.entity)
+        return len(by_entity.get(self.key, ())) if by_entity is not None else 0
 
 
 class EntityRelations(MutableMapping[object, EntityRelationsMapping]):
     """A proxy attribute to access entity relations like a dict of sets.
 
     See :any:`Entity.relation_tags_many`.
     """
@@ -354,39 +359,39 @@
     __slots__ = ("entity",)
 
     def __init__(self, entity: Entity) -> None:
         """Initialize this attribute for the given entity."""
         self.entity: Final = entity
 
     def __getitem__(self, key: object) -> EntityRelationsMapping:
-        """Return the relation mapping for a key."""
+        """Return the relation mapping for a tag."""
         return EntityRelationsMapping(self.entity, key)
 
     def __setitem__(self, key: object, values: Iterable[Entity]) -> None:
-        """Overwrite the targets of a relation key with the new values."""
+        """Overwrite the targets of a relation tag with the new values."""
         assert not isinstance(values, Entity), "Did you mean `entity.relations[key] = (target,)`?"
         mapping = EntityRelationsMapping(self.entity, key)
         mapping.clear()
         for v in values:
             mapping.add(v)
 
     def __delitem__(self, key: object) -> None:
-        """Clear the relation targets of a relation key."""
+        """Clear the relation tags of an entity.
+
+        This does not remove relation tags towards this entity.
+        """
         self[key].clear()
 
     def __iter__(self) -> Iterator[Any]:
-        """Iterate over the keys of this entities relations."""
-        # Slow!
-        for key, value in self.entity.world._relations_by_key.items():
-            if self.entity in value:
-                yield key
+        """Iterate over the unique relation tags of this entity."""
+        return iter(self.entity.world._relation_tags_by_entity.get(self.entity, {}).keys())
 
     def __len__(self) -> int:
-        """Return the number of relations this entity has."""
-        return len(list(self.__iter__()))  # Slow!
+        """Return the number of unique relation tags this entity has."""
+        return len(self.entity.world._relation_tags_by_entity.get(self.entity, {}))
 
 
 class EntityRelationsExclusive(MutableMapping[object, Entity]):
     """A proxy attribute to access entity relations exclusively.
 
     See :any:`Entity.relation_tags`.
     """
@@ -444,36 +449,36 @@
         """Initialize this attribute for the given entity."""
         assert isinstance(entity, Entity), entity
         self.entity: Final = entity
         self.key: _ComponentKey[T] = key
 
     def __getitem__(self, target: Entity) -> T:
         """Return the component related to a target entity."""
-        return self.entity.world._relation_components[self.key][self.entity][target]  # type: ignore[no-any-return]
+        return self.entity.world._relation_components_by_entity[self.entity][self.key][target]  # type: ignore[no-any-return]
 
     def __setitem__(self, target: Entity, component: T) -> None:
         """Assign a component to the target entity."""
         world = self.entity.world
-        if target in world._relation_components[self.key][self.entity] is not None:
+        if target in world._relation_components_by_entity[self.entity][self.key] is not None:
             del self[target]
-        world._relation_components[self.key][self.entity][target] = component
+        world._relation_components_by_entity[self.entity][self.key][target] = component
 
         world._relations_lookup[(self.key, target)] = {self.entity}
         world._relations_lookup[(self.key, ...)].add(self.entity)
         world._relations_lookup[(self.entity, self.key, None)] = {target}
         world._relations_lookup[(..., self.key, None)].add(target)
 
     def __delitem__(self, target: Entity) -> None:
         """Delete a component assigned to the target entity."""
         world = self.entity.world
-        del world._relation_components[self.key][self.entity][target]
-        if not world._relation_components[self.key][self.entity]:
-            del world._relation_components[self.key][self.entity]
-        if not world._relation_components[self.key]:
-            del world._relation_components[self.key]
+        del world._relation_components_by_entity[self.entity][self.key][target]
+        if not world._relation_components_by_entity[self.entity][self.key]:
+            del world._relation_components_by_entity[self.entity][self.key]
+        if not world._relation_components_by_entity[self.entity]:
+            del world._relation_components_by_entity[self.entity]
 
         world._relations_lookup[(self.key, target)].discard(self.entity)
         if not world._relations_lookup[(self.key, target)]:
             del world._relations_lookup[(self.key, target)]
 
         world._relations_lookup[(self.key, ...)].discard(self.entity)
         if not world._relations_lookup[(self.key, ...)]:
@@ -485,21 +490,21 @@
 
         world._relations_lookup[(..., self.key, None)].discard(self.entity)
         if not world._relations_lookup[(..., self.key, None)]:
             del world._relations_lookup[(..., self.key, None)]
 
     def __iter__(self) -> Iterator[Entity]:
         """Iterate over the targets with assigned components."""
-        relations_by_type = self.entity.world._relation_components.get(self.key)
-        return iter(()) if relations_by_type is None else iter(relations_by_type.get(self.entity, ()))
+        by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
+        return iter(()) if by_entity is None else iter(by_entity.get(self.key, ()))
 
     def __len__(self) -> int:
         """Return the count of targets for this component relation."""
-        relations_by_type = self.entity.world._relation_components.get(self.key)
-        return 0 if relations_by_type is None else len(relations_by_type.get(self.entity, ()))
+        by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
+        return 0 if by_entity is None else len(by_entity.get(self.key, ()))
 
 
 class EntityComponentRelations:
     """Proxy to access the component relations of an entity.
 
     See :any:`Entity.relation_components`.
     """
@@ -521,58 +526,114 @@
 
 
 class World:
     """A container for entities and components."""
 
     def __init__(self) -> None:
         """Initialize a new world."""
-        # Spare-set components.
-        # ComponentKey is `type` or `(tag, type)`, see annotation.
-        # dict[ComponentKey][Entity] = component_instance
         self._components_by_type: DefaultDict[_ComponentKey[object], dict[Entity, Any]] = DefaultDict(dict)
-        # dict[Entity] = {component_keys_owned_by_entity}
+        """Query table entity components.
+
+        dict[ComponentKey][Entity] = component_instance
+        """
         self._components_by_entity: DefaultDict[Entity, set[_ComponentKey[object]]] = DefaultDict(set)
+        """Random access entity components.
+
+        dict[Entity] = {component_keys_owned_by_entity}
+        """
 
-        # Sparse-set tags.
-        # dict[tag] = {all_entities_with_tag}
         self._tags_by_key: DefaultDict[object, set[Entity]] = DefaultDict(set)
-        # dict[Entity] = {all_tags_for_entity}
+        """Query table entity tags.
+
+        dict[tag] = {all_entities_with_tag}
+        """
         self._tags_by_entity: DefaultDict[Entity, set[Any]] = DefaultDict(set)
+        """Random access entity tags.
+
+        dict[Entity] = {all_tags_for_entity}
+        """
 
-        # Sparse-set relations.
-        # dict[tag][this_entity] = {target_entities_for_entity}
-        self._relations_by_key: DefaultDict[object, DefaultDict[Entity, set[Entity]]] = DefaultDict(
+        self._relation_tags_by_entity: DefaultDict[Entity, DefaultDict[object, set[Entity]]] = DefaultDict(
             partial(DefaultDict, set)  # type: ignore[arg-type]
         )
-        # Sparse-set relations owning components.
-        # dict[ComponentKey][own_entity][target_entity] = component
-        self._relation_components: DefaultDict[
-            _ComponentKey[object], DefaultDict[Entity, dict[Entity, Any]]
+        """Random access tag multi-relations.
+
+        dict[entity][tag] = {target_entities}
+        """
+        self._relation_components_by_entity: DefaultDict[
+            Entity, DefaultDict[_ComponentKey[object], dict[Entity, Any]]
         ] = DefaultDict(
             partial(DefaultDict, dict)  # type: ignore[arg-type]
         )
-        # Tag:
-        # dict[(tag, this_entity)] = {target_entities_for_entity}
-        # dict[(tag, None)] = {target_entities_for_tag}
-        # dict[(target_entity, tag, None)] = {origin_entities_for_target}
-        # dict[(None, tag, None)] = {all_origen_entities_for_tag}
-        # Component:
-        # dict[(ComponentKey, target_entity)] = {origin_entities}
-        # dict[(ComponentKey, None)] = {all_origin_entities}
-        # dict[(origin_entity, ComponentKey, None)] = {target_entities}
-        # dict[(None, ComponentKey, None)] = {all_target_entities}
+        """Random access relations owning components.
+
+        dict[entity][ComponentKey][target_entity] = component
+        """
         self._relations_lookup: DefaultDict[
             tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]
         ] = DefaultDict(set)
+        """Relations query table.  Tags and components are mixed together.
+
+        Tag:
+            dict[(tag, this_entity)] = {target_entities_for_entity}
+            dict[(tag, None)] = {target_entities_for_tag}
+            dict[(target_entity, tag, None)] = {origin_entities_for_target}
+            dict[(None, tag, None)] = {all_origen_entities_for_tag}
+        Component:
+            dict[(ComponentKey, target_entity)] = {origin_entities}
+            dict[(ComponentKey, None)] = {all_origin_entities}
+            dict[(origin_entity, ComponentKey, None)] = {target_entities}
+            dict[(None, ComponentKey, None)] = {all_target_entities}
+        """
 
-        # Named objects dictionary.
-        # dict[name] = named_entity
         self._names_by_name: dict[object, Entity] = {}
-        # dict[Entity] = entities_name
+        """Name query table.
+
+        dict[name] = named_entity
+        """
         self._names_by_entity: dict[Entity, object] = {}
+        """Name lookup table.
+
+        dict[Entity] = entities_name
+        """
+
+        self.global_: Final = Entity(self)
+        """A unique globally accessible entity.
+
+        This can be used to store globally accessible components in the world itself without any extra boilerplate.
+        Otherwise this entity is not special and will show up with other entities in queries, etc.
+
+        .. versionadded:: 1.1
+
+        Example::
+
+            >>> world.global_.components[("turn", int)] = 0
+        """
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        """Unpickle this object and handle state migration."""
+        # Migrate from version <=1.0.0.
+        state.setdefault("global_", Entity(self))
+        if "_relation_components" in state:
+            _relation_components: dict[_ComponentKey[object], dict[Entity, dict[Entity, Any]]] = state.pop(
+                "_relation_components"
+            )
+            self._relation_components_by_entity = DefaultDict(partial(DefaultDict, dict))  # type: ignore[arg-type]
+            for component_key, component_key_relations in _relation_components.items():
+                for entity, entities_component_table in component_key_relations.items():
+                    for target_entity, target_component in entities_component_table.items():
+                        self._relation_components_by_entity[entity][component_key][target_entity] = target_component
+
+            _relations_by_key: dict[object, dict[Entity, set[Entity]]] = state.pop("_relations_by_key")
+            self._relation_tags_by_entity = DefaultDict(partial(DefaultDict, set))  # type: ignore[arg-type]
+            for tag, tag_relations in _relations_by_key.items():
+                for entity, targets in tag_relations.items():
+                    self._relation_tags_by_entity[entity][tag] = targets
+
+        self.__dict__.update(state)
 
     @property
     def named(self) -> Mapping[object, Entity]:
         """A view into this worlds named entities."""
         return self._names_by_name
 
     def new_entity(
```

### Comparing `tcod-ecs-1.0.0/tcod/ecs/test_ecs.py` & `tcod-ecs-1.1.0/tcod/ecs/test_ecs.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,7 +160,15 @@
     check_world_v1(unpickled)
 
 
 def test_unpickle_v1_0() -> None:
     WORLD_v1_0 = b"\x80\x04\x95\xc7\x02\x00\x00\x00\x00\x00\x00\x8c\x08tcod.ecs\x94\x8c\x05World\x94\x93\x94)\x81\x94}\x94(\x8c\x13_components_by_type\x94\x8c\x0bcollections\x94\x8c\x0bdefaultdict\x94\x93\x94\x8c\x08builtins\x94\x8c\x04dict\x94\x93\x94\x85\x94R\x94(h\t\x8c\x03str\x94\x93\x94}\x94h\x00\x8c\x06Entity\x94\x93\x94)\x81\x94N}\x94\x8c\x05world\x94h\x03s\x86\x94b\x8c\x03str\x94s\x8c\x03foo\x94h\x0f\x86\x94}\x94h\x13h\x18su\x8c\x15_components_by_entity\x94h\x08h\t\x8c\x03set\x94\x93\x94\x85\x94R\x94h\x13\x8f\x94(h\x19h\x0f\x90s\x8c\x0c_tags_by_key\x94h\x08h\x1d\x85\x94R\x94\x8c\x03tag\x94\x8f\x94(h\x13\x90s\x8c\x0f_tags_by_entity\x94h\x08h\x1d\x85\x94R\x94h\x13\x8f\x94(h$\x90s\x8c\x11_relations_by_key\x94h\x08\x8c\tfunctools\x94\x8c\x07partial\x94\x93\x94\x8c\x06typing\x94\x8c\x0bDefaultDict\x94\x93\x94\x85\x94R\x94(h0h\x1d\x85\x94}\x94Nt\x94b\x85\x94R\x94\x8c\x07ChildOf\x94h\x08h\x1d\x85\x94R\x94h\x12)\x81\x94N}\x94h\x15h\x03s\x86\x94b\x8f\x94(h\x13\x90ss\x8c\x14_relation_components\x94h\x08h-h0\x85\x94R\x94(h0h\x0b\x85\x94}\x94Nt\x94b\x85\x94R\x94h\x0fh\x08h\x0b\x85\x94R\x94h;}\x94h\x13h\x17sss\x8c\x11_relations_lookup\x94h\x08h\x1d\x85\x94R\x94(h8h\x13\x86\x94\x8f\x94(h;\x90h8h\t\x8c\x08Ellipsis\x94\x93\x94\x86\x94\x8f\x94(h;\x90h;h8N\x87\x94\x8f\x94(h\x13\x90hPh8N\x87\x94\x8f\x94(h\x13\x90h\x0fh\x13\x86\x94\x8f\x94(h;\x90h\x0fhP\x86\x94\x8f\x94(h;\x90h;h\x0fN\x87\x94\x8f\x94(h\x13\x90hPh\x0fN\x87\x94\x8f\x94(h\x13\x90u\x8c\x0e_names_by_name\x94}\x94(\x8c\x01A\x94h\x13\x8c\x01B\x94h;u\x8c\x10_names_by_entity\x94}\x94(h\x13hah;hbuub."  # cspell: disable-line
     unpickled: tcod.ecs.World = pickle.loads(WORLD_v1_0)
     check_world_v1(unpickled)
+    unpickled.new_entity()
+    assert not unpickled.global_.components
+
+
+def test_global() -> None:
+    world = tcod.ecs.World()
+    world.global_.components[int] = 1
+    assert set(world.Q[tcod.ecs.Entity, int]) == {(world.global_, 1)}
```

### Comparing `tcod-ecs-1.0.0/PKG-INFO` & `tcod-ecs-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 1.0.0
+Version: 1.1.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

