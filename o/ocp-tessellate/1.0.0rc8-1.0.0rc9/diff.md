# Comparing `tmp/ocp_tessellate-1.0.0rc8.tar.gz` & `tmp/ocp_tessellate-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.0.0rc8.tar", last modified: Mon Feb 27 20:17:09 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.0.0rc9.tar", last modified: Mon Mar  6 08:01:37 2023, max compression
```

## Comparing `ocp_tessellate-1.0.0rc8.tar` & `ocp_tessellate-1.0.0rc9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-02-27 20:17:09.102233 ocp_tessellate-1.0.0rc8/
--rw-r--r--   0 bernhard   (501) staff       (20)      777 2023-02-27 20:17:09.102293 ocp_tessellate-1.0.0rc8/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.0.0rc8/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-02-27 20:17:09.101520 ocp_tessellate-1.0.0rc8/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1126 2023-02-27 20:17:00.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    12251 2023-02-11 20:57:00.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    22400 2023-02-27 20:08:42.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10345 2023-02-26 17:10:57.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19108 2023-02-27 20:08:05.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13136 2023-02-26 16:25:33.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     5824 2023-02-11 19:32:38.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-02-27 20:17:09.102133 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      777 2023-02-27 20:17:09.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      532 2023-02-27 20:17:09.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-02-27 20:17:09.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-02-27 20:17:09.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      129 2023-02-27 20:17:09.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-02-27 20:17:09.000000 ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      674 2023-02-27 20:17:09.102556 ocp_tessellate-1.0.0rc8/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1647 2023-02-27 20:17:00.000000 ocp_tessellate-1.0.0rc8/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-03-06 08:01:37.339228 ocp_tessellate-1.0.0rc9/
+-rw-r--r--   0 bernhard   (501) staff       (20)      777 2023-03-06 08:01:37.339287 ocp_tessellate-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.0rc9/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-03-06 08:01:37.338524 ocp_tessellate-1.0.0rc9/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1126 2023-03-04 18:58:11.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    12354 2023-03-05 17:05:19.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    23309 2023-03-05 17:41:50.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10345 2023-02-27 07:20:24.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19108 2023-03-01 18:54:17.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13212 2023-03-05 18:04:14.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     5824 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-03-06 08:01:37.339146 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      777 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      532 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      129 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-03-06 08:01:37.000000 ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      674 2023-03-06 08:01:37.339547 ocp_tessellate-1.0.0rc9/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1647 2023-03-04 18:58:11.000000 ocp_tessellate-1.0.0rc9/setup.py
```

### Comparing `ocp_tessellate-1.0.0rc8/PKG-INFO` & `ocp_tessellate-1.0.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/__init__.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/_version.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.0.0rc8"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.0.0rc9"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/cad_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,29 +152,30 @@
                 )
 
                 t.info = f"{{quality:{quality:.4f}, angular_tolerance:{angular_tolerance:.2f}}}"
 
         with Timer(timeit, self.name, "bounding box:   ", 2):
             t, q = loc_to_tq(get_location(loc))
             if parallel and is_apply_result(mesh):
-                mesh = {"result": mesh, "t": t, "q": q}
+                # store the instance mesh
+                if ind is not None and INSTANCES[ind].mesh is None:
+                    INSTANCES[ind].mesh = mesh
+                    INSTANCES[ind].quality = quality
+                mesh = {"ref": ind, "t": t, "q": q}
                 bb = {}
             else:
                 bb = np_bbox(mesh["vertices"], t, q)
                 # store the instance mesh
                 if ind is not None and INSTANCES[ind].mesh is None:
                     INSTANCES[ind].mesh = mesh
                     INSTANCES[ind].quality = quality
 
                 if isinstance(self.shape, dict):
                     mesh = self.shape  # return the instance id
 
-        if progress == "without_cache":
-            progress.update()
-
         if isinstance(self.color, tuple):
             color = [c.web_color for c in self.color]  # pylint: disable=not-an-iterable
             alpha = 1.0
         else:
             color = self.color.web_color
             alpha = self.color.a
 
@@ -256,16 +257,16 @@
                 d = discretize_edge(edge, deflection)
                 if len(d) == 1 and not is_line(edge):
                     num = int(0.1 / deflection)
                     d = discretize_edge(edge, num=num)
                 edges.extend(d)
             edges = np.asarray(edges)
 
-        if progress is not None and not isinstance(progress, str):
-            progress.update()
+        if progress is not None:
+            progress.update("e")
 
         color = (
             [c.web_color for c in self.color]
             if isinstance(self.color, tuple)
             else self.color.web_color
         )
 
@@ -307,22 +308,24 @@
         progress=None,
         timeit=False,
     ):
         self.id = f"{path}/{self.name}"
 
         bb = bounding_box(self.shape, loc=get_location(loc))
 
-        if progress is not None and not isinstance(progress, str):
-            progress.update()
+        if progress is not None:
+            progress.update("v")
 
         return {
             "id": self.id,
             "type": "vertices",
             "name": self.name,
-            "shape": np.asarray([get_point(vertex) for vertex in self.shape], dtype="float32"),
+            "shape": np.asarray(
+                [get_point(vertex) for vertex in self.shape], dtype="float32"
+            ),
             "color": self.color.web_color,
             "size": self.size,
             "bb": bb.to_dict(),
         }
 
 
 class OCP_PartGroup(CADObject):
```

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/convert.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,33 +137,37 @@
                 bb = c_bb(shape, bb)
         return bb
 
     bb = c_bb(shapes, None)
     return bb
 
 
-def mp_get_results(shapes, progress):
+def mp_get_results(instances, shapes, progress):
     def walk(shapes):
         for shape in shapes["parts"]:
             if shape.get("parts") is None:
                 if shape.get("type") == "shapes":
-                    if is_apply_result(shape["shape"].get("result")):
-                        mesh = get_mp_result(shape["shape"]["result"])
-                        t = shape["shape"]["t"]
-                        q = shape["shape"]["q"]
-                        shape["shape"] = mesh
-                        shape["bb"] = np_bbox(mesh["vertices"], t, q)
+                    mesh = instances[shape["shape"]["ref"]]
+                    t = shape["shape"].get("t")
+                    q = shape["shape"].get("q")
+                    shape["shape"] = {"ref": shape["shape"]["ref"]}  # remove t and q
+                    shape["bb"] = np_bbox(mesh["vertices"], t, q)
 
                     if progress is not None:
-                        progress.update()
+                        progress.update("r")
             else:
                 walk(shape)
 
+    for i in range(len(instances)):
+        if is_apply_result(instances[i]):
+            instances[i] = get_mp_result(instances[i])
+
     walk(shapes)
-    return shapes
+
+    return instances, shapes
 
 
 def get_accuracies(shapes):
     def _get_accuracies(shapes, lengths):
         if shapes.get("parts"):
             for shape in shapes["parts"]:
                 _get_accuracies(shape, lengths)
@@ -253,15 +257,15 @@
             _debug(f"build123d Assembly {grp_id}: {type(cad_obj)}")
             cad_objs = []
             raise NotImplemented("build123d assemblies not implemented yet")
 
         # build123d Compound
         else:
             _debug(f"build123d Compound {grp_id}: {type(cad_obj)}")
-            cad_objs = [downcast(obj.wrapped) for obj in cad_obj]
+            cad_objs = [cad_obj.wrapped]
 
     elif is_build123d_shape(cad_obj):
         _debug(f"build123d Shape {grp_id}: {type(cad_obj)}")
         cad_objs = get_downcasted_shape(cad_obj.wrapped)
 
     elif is_cadquery_sketch(cad_obj):
         cad_objs = conv_sketch(cad_obj)
@@ -272,15 +276,15 @@
             if is_cadquery_sketch(v):
                 obj = conv_sketch(v)
 
             elif is_vector(v):
                 obj = [vertex(v.wrapped)]
 
             else:
-                obj = get_downcasted_shape(v.wrapped)
+                obj = [v.wrapped]
 
             cad_objs.extend(obj)
 
     elif is_wrapped(cad_obj):
         if is_vector(cad_obj):
             cad_objs = [vertex(cad_obj.wrapped)]
         else:
@@ -295,15 +299,15 @@
         else:
             raise ValueError("Empty list cannot be tessellated")
 
     elif is_topods_compound(cad_obj):
         _debug(f"CAD Obj {grp_id}: TopoDS Compound")
 
         # Get the highest level shape
-        cad_objs = get_downcasted_shape(cad_obj)
+        cad_objs = [cad_obj]
 
     elif is_topods_shape(cad_obj):
         _debug(f"CAD Obj {grp_id}: TopoDS Shape")
         cad_objs = [downcast(cad_obj)]
 
     else:
         raise RuntimeError(f"Cannot transform {cad_objs}({type(cad_objs)}) to OCP")
@@ -351,41 +355,79 @@
         return OCP_Vertices(
             cad_objs,
             name=name,
             color=get_rgba(obj_color, 1.0, THICK_EDGE_COLOR),
             size=6,
         )
     elif is_compound_list(cad_objs):
-        name = f"{obj_name if obj_name is not None else 'Solid'}_{grp_id}"
-        return OCP_Part(
-            cad_objs,
-            name=name,
-            color=get_rgba(obj_color, obj_alpha, Color(default_color)),
-        )
+        obj_list = get_downcasted_shape(cad_objs[0])
+        if is_solid_list(obj_list):
+            name = f"{obj_name if obj_name is not None else 'Solids'}_{grp_id}"
+            return OCP_Part(
+                cad_objs,  # use compound
+                name=name,
+                color=get_rgba(obj_color, obj_alpha, Color(default_color)),
+            )
+        elif is_face_list(obj_list):
+            name = f"{obj_name if obj_name is not None else 'Faces'}_{grp_id}"
+            return OCP_Faces(
+                cad_objs,  # use compound
+                name=name,
+                color=get_rgba(obj_color, obj_alpha, Color(FACE_COLOR)),
+            )
+
+        elif is_edge_list(obj_list) or is_wire_list(obj_list):
+            if is_wire_list(obj_list):
+                edges = []
+                for wire in obj_list:
+                    edges.extend(get_edges(wire))
+                obj_list = edges
+
+            name = f"{obj_name if obj_name is not None else 'Edges'}_{grp_id}"
+            return OCP_Edges(
+                obj_list,  # use object list
+                name=name,
+                color=get_rgba(obj_color, 1.0, Color(THICK_EDGE_COLOR)),
+                width=2,
+            )
+
+        elif is_vertex_list(obj_list):
+            name = f"{obj_name if obj_name is not None else 'Vertices'}_{grp_id}"
+            return OCP_Vertices(
+                obj_list,  # use object list
+                name=name,
+                color=get_rgba(obj_color, 1.0, THICK_EDGE_COLOR),
+                size=6,
+            )
+
     else:
         raise RuntimeError(
             f"Cannot transform {cad_objs}, e.g. mixed Compounds not supported here?"
         )
 
 
-def get_instance(obj, grp_id, name, rgba, instances):
+def get_instance(obj, grp_id, name, rgba, instances, progress):
     is_instance = False
     part = None
 
     # check if the same instance is already available
     for i, ref in enumerate(instances):
         if ref[0] == get_tshape(obj):
             # create a referential OCP_Part
             part = OCP_Part(
                 {"ref": i},
                 f"{name}_{grp_id}",
                 rgba,
             )
             # and stop the loop
             is_instance = True
+
+            if progress is not None:
+                progress.update("-")
+
             break
 
     if not is_instance:
         # Transform the new instance to OCP
         part = conv(obj, grp_id, name, rgba[:3], rgba[3])
         if not isinstance(part, OCP_PartGroup):
             # append the new instance
@@ -428,14 +470,15 @@
     mate_scale=1,
     default_color=None,
     show_parent=False,
     loc=None,
     grp_id=0,
     mates=None,
     instances=None,
+    progress=None,
 ):
     if names is None:
         names = [None] * len(cad_objs)
 
     if colors is None:
         colors = [None] * len(cad_objs)
 
@@ -484,15 +527,17 @@
 
                 if is_cadquery_massembly(cad_obj):
                     # get_instance fails for MAssemblies when a mate is not at the
                     # shape origin after relocation, see hexapod "top" object
                     # workaround: do not handle TShapes
                     part = conv(cad_obj.obj, grp_id, cad_obj.name, color, alpha)
                 else:
-                    part = get_instance(cad_obj.obj, grp_id, pg.name, rgba, instances)
+                    part = get_instance(
+                        cad_obj.obj, grp_id, pg.name, rgba, instances, progress
+                    )
                 pg.add(part)
 
             # render mates
             top_level_mates = None
             if render_mates and hasattr(cad_obj, "mates") and cad_obj.mates is not None:
                 top_level_mates = cad_obj.mates if mates is None else mates
 
@@ -528,14 +573,15 @@
                     names=[obj_name],
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     mates=top_level_mates,
                     render_mates=render_mates,
                     mate_scale=mate_scale,
                     instances=instances,
+                    progress=progress,
                 )
                 pg.add(part)
 
         elif is_compound(cad_obj):
             #
             # Iterate over Compound (includes build123d assemblies)
             #
@@ -557,51 +603,33 @@
                     part.name = get_name(part, grp_id)
                 pg.add(part)
                 done = True
 
             elif is_build123d_assembly(cad_obj):
                 # There is no top level shape, hence only get childern
                 children = cad_obj.children
-
-            else:
-                # For an iterable compound, ...
-                children = list(cad_obj)
-                cw = [c.wrapped for c in children]
-                # ... check whether all elements have the same type
-                if (
-                    is_face_list(cw)
-                    or is_edge_list(cw)
-                    or is_vertex_list(cw)
-                    or is_wire_list(cw)
-                ):
-                    # If so, don't explode homogenous lists, e.g build123d ShapeLists
-                    # If this should be exploded, the user can provide "*shape_list"
-                    part = conv(children, grp_id, obj_name, color, alpha)
-                    if obj_name is None:
-                        part.name = get_name(part, grp_id)
-                        grp_id += 1
-                    pg.add(part)
-                    done = True
-
-            # if not homogenous, iterate over all children
-            if not done:
                 for child in children:
                     part, instances, grp_id = _to_assembly(
                         child,
                         grp_id=grp_id,
                         default_color=default_color,
                         names=[obj_name],
                         colors=[obj_color],
                         alphas=[obj_alpha],
                         render_mates=render_mates,
                         mate_scale=mate_scale,
                         instances=instances,
+                        progress=progress,
                     )
                     pg.add(part)
 
+            else:
+                part = conv(cad_obj.wrapped, grp_id, obj_name, color, alpha)
+                pg.add(part)
+
         elif is_cadquery_sketch(cad_obj):
             #
             # Special treatment for cadquery sketches
             #
 
             for child in conv_sketch(cad_obj):
                 part, instances, grp_id = _to_assembly(
@@ -610,14 +638,15 @@
                     default_color=default_color,
                     names=[obj_name],
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     render_mates=render_mates,
                     mate_scale=mate_scale,
                     instances=instances,
+                    progress=progress,
                 )
                 pg.add(part)
 
         else:
             #
             # Render non iterable objects
             #
@@ -652,16 +681,18 @@
 
             if is_solid:
                 # Split solids into a solid at the XY plane origin and the location
                 cad_obj, loc = relocate(cad_obj)
                 # create a partgroup and move part location into it
                 pg2 = OCP_PartGroup([], name=f"Group_{grp_id}", loc=loc)
 
-                # transform the olid to OCP
-                part = get_instance(cad_obj, 0, obj_name, rgba, instances)
+                # transform the solid to OCP
+                part = get_instance(
+                    cad_obj, grp_id, obj_name, rgba, instances, progress
+                )
 
                 if obj_name is None:
                     part.name = get_name(part, grp_id)
                 # change part's location to identity, since location is in partgroup
                 pg.loc = identity_location()
 
                 pg2.add(part)
@@ -702,24 +733,26 @@
     mate_scale=1,
     default_color=None,
     show_parent=False,
     loc=None,
     grp_id=0,
     mates=None,
     instances=None,
+    progress=None,
 ):
     pg, instances, _ = _to_assembly(
         *cad_objs,
         names=names,
         colors=colors,
         alphas=alphas,
         render_mates=render_mates,
         mate_scale=mate_scale,
         default_color=default_color,
         show_parent=show_parent,
         loc=loc,
         grp_id=grp_id,
         mates=mates,
         instances=instances,
+        progress=progress,
     )
     set_instances([instance[1] for instance in instances])
     return pg
```

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/defaults.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/tessellator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,28 +57,32 @@
     shape,
     deviation,
     quality,
     angular_tolerance,
     compute_edges=True,
     compute_faces=True,
     debug=False,
-    progress=False,
+    progress=None,
 ):  # pylint: disable=unused-argument
     # quality is a measure of bounding box and deviation, hence can be ignored (and should due to accuracy issues
     # of non optimal bounding boxes. debug and progress are also irrelevant for tessellation results)
     if not isinstance(shape, (tuple, list)):
         shape = [shape]
 
     key = (
         tuple(((s.HashCode(MAX_HASH_KEY), id(s)) for s in shape)),
         deviation,
         angular_tolerance,
         compute_edges,
         compute_faces,
     )
+
+    if progress is not None and cache.get(key) is not None:
+        progress.update("c")
+
     return key
 
 
 def get_size(obj):
     size = sys.getsizeof(obj)
     if isinstance(obj, dict):
         size += sum([get_size(v) + len(k) for k, v in obj.items()])
@@ -313,16 +317,16 @@
     quality: float,
     angular_tolerance: float,
     compute_faces=True,
     compute_edges=True,
     debug=False,
     progress=None,
 ):
-    if progress == "with_cache":
-        print(".", end="", flush=True)
+    if progress is not None:
+        progress.update("+")
 
     compound = (
         make_compound(shapes) if len(shapes) > 1 else shapes[0]
     )  # pylint: disable=protected-access
     tess = Tessellator()
     tess.compute(
         compound, quality, angular_tolerance, compute_faces, compute_edges, debug
```

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate/utils.py` & `ocp_tessellate-1.0.0rc9/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-tessellate
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.0rc8/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.0.0rc9/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.0rc8/setup.cfg` & `ocp_tessellate-1.0.0rc9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0rc8
+current_version = 1.0.0rc9
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.0.0rc8/setup.py` & `ocp_tessellate-1.0.0rc9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.0.0rc8",
+    "version": "1.0.0rc9",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

