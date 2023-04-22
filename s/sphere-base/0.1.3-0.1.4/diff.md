# Comparing `tmp/sphere_base-0.1.3.tar.gz` & `tmp/sphere_base-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphere_base-0.1.3.tar", last modified: Fri Apr 21 09:00:59 2023, max compression
+gzip compressed data, was "sphere_base-0.1.4.tar", last modified: Sat Apr 22 14:09:52 2023, max compression
```

## Comparing `sphere_base-0.1.3.tar` & `sphere_base-0.1.4.tar`

### file list

```diff
@@ -1,180 +1,168 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.511082 sphere_base-0.1.3/
--rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.3/HISTORY.rst
--rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1987 2023-04-21 09:00:59.510082 sphere_base-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.286069 sphere_base-0.1.3/docs/
--rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.241067 sphere_base-0.1.3/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.241067 sphere_base-0.1.3/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.290069 sphere_base-0.1.3/docs/build/html/_static/
--rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.3/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.3/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.3/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.3/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.293069 sphere_base-0.1.3/docs/source/
--rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.3/docs/source/conf.py
--rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.3/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.364074 sphere_base-0.1.3/docs/source/rst/
--rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.mesh.rst
--rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.model.rst
--rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.models.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.obj_file_loader.rst
--rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.model.rst
--rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.rst
--rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_base_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
--rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
--rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_default_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
--rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_node_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.shader.uv_square_shader.rst
--rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
--rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
--rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
--rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
--rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
--rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
--rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
--rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
--rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
--rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
--rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
--rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
--rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
--rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
--rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
--rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
--rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
--rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
--rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
--rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
--rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 09:00:59.511082 sphere_base-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1574 2023-04-21 09:00:50.000000 sphere_base-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.372074 sphere_base-0.1.3/sphere_base/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/__init__.py
--rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.3/sphere_base/calc.py
--rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.3/sphere_base/clipboard.py
--rw-rw-rw-   0        0        0     5078 2023-04-14 08:50:15.000000 sphere_base-0.1.3/sphere_base/config.py
--rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.3/sphere_base/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.435078 sphere_base-0.1.3/sphere_base/edge/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.3/sphere_base/edge/__init__.py
--rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.3/sphere_base/edge/edge_drag.py
--rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.3/sphere_base/edge/graphic_edge.py
--rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.3/sphere_base/edge/graphic_line.py
--rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.3/sphere_base/edge/inter_sphere_edge.py
--rw-rw-rw-   0        0        0    14119 2023-04-20 17:33:34.000000 sphere_base-0.1.3/sphere_base/edge/surface_edge.py
--rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.3/sphere_base/history.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.441078 sphere_base-0.1.3/sphere_base/model/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.3/sphere_base/model/__init__.py
--rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/model/mesh.py
--rw-rw-rw-   0        0        0     6393 2023-04-20 17:27:51.000000 sphere_base-0.1.3/sphere_base/model/model.py
--rw-rw-rw-   0        0        0     3318 2023-04-04 11:04:51.000000 sphere_base-0.1.3/sphere_base/model/models.py
--rw-rw-rw-   0        0        0    23063 2023-04-21 06:52:17.000000 sphere_base-0.1.3/sphere_base/model/obj_file_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.442078 sphere_base-0.1.3/sphere_base/model/resources/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.443078 sphere_base-0.1.3/sphere_base/model/resources/icons/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.444078 sphere_base-0.1.3/sphere_base/model/resources/images/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.445078 sphere_base-0.1.3/sphere_base/model/resources/meshes/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/meshes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.446078 sphere_base-0.1.3/sphere_base/model/resources/shaders/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/shaders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.448078 sphere_base-0.1.3/sphere_base/model/resources/sphere_textures/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/sphere_textures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.449078 sphere_base-0.1.3/sphere_base/model/resources/textures/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/textures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.450079 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.451079 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/blue1/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/model/resources/textures/skybox/blue1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.459079 sphere_base-0.1.3/sphere_base/node/
--rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.3/sphere_base/node/__init__.py
--rw-rw-rw-   0        0        0     8018 2023-04-03 06:31:17.000000 sphere_base-0.1.3/sphere_base/node/graphic_disc.py
--rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.3/sphere_base/node/graphic_node.py
--rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.3/sphere_base/node/graphic_socket.py
--rw-rw-rw-   0        0        0    13282 2023-04-20 17:22:13.000000 sphere_base-0.1.3/sphere_base/node/node.py
--rw-rw-rw-   0        0        0     8797 2023-04-13 12:16:43.000000 sphere_base-0.1.3/sphere_base/node/socket.py
--rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.3/sphere_base/serializable.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.477080 sphere_base-0.1.3/sphere_base/shader/
--rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.3/sphere_base/shader/__init__.py
--rw-rw-rw-   0        0        0     9085 2023-04-20 17:12:04.000000 sphere_base-0.1.3/sphere_base/shader/base_shader.py
--rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/circle_shader.py
--rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/cross_shader.py
--rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.3/sphere_base/shader/default_shader.py
--rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.3/sphere_base/shader/drag_edge_shader.py
--rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.3/sphere_base/shader/edge_shader.py
--rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/flat_shader.py
--rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/holo_sphere_shader.py
--rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.3/sphere_base/shader/node_shader.py
--rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.3/sphere_base/shader/skybox_shader.py
--rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/socket_shader.py
--rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.3/sphere_base/shader/sphere_edge_shader.py
--rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/sphere_shader.py
--rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/sphere_small_shader.py
--rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.3/sphere_base/shader/square_shader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.482080 sphere_base-0.1.3/sphere_base/sphere/
--rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.3/sphere_base/sphere/__init__.py
--rw-rw-rw-   0        0        0    28884 2023-04-21 06:53:52.000000 sphere_base-0.1.3/sphere_base/sphere/sphere.py
--rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.3/sphere_base/sphere/sphere_lines.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.488081 sphere_base-0.1.3/sphere_base/sphere_overlay/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.489081 sphere_base-0.1.3/sphere_base/sphere_overlay/icons/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.492081 sphere_base-0.1.3/sphere_base/sphere_overlay/qss/
--rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/qss/__init__.py
--rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
--rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sov_conf.py
--rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere.py
--rw-rw-rw-   0        0        0     1598 2023-04-13 12:14:08.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere_node_base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.497081 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/
--rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/__init__.py
--rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
--rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
--rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.508082 sphere_base-0.1.3/sphere_base/sphere_universe_base/
--rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/__init__.py
--rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam.py
--rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam_movement.py
--rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_graphic_item.py
--rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_mouse_ray.py
--rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_rubber_band.py
--rw-rw-rw-   0        0        0     5392 2023-03-28 18:59:36.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_skybox.py
--rw-rw-rw-   0        0        0    14026 2023-04-14 08:50:15.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_universe.py
--rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_widget.py
--rw-rw-rw-   0        0        0     1494 2023-03-30 07:18:00.000000 sphere_base-0.1.3/sphere_base/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.394075 sphere_base-0.1.3/sphere_base.egg-info/
--rw-rw-rw-   0        0        0     1987 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6697 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.3/sphere_base.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      119 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 09:00:59.000000 sphere_base-0.1.3/sphere_base.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 09:00:59.509082 sphere_base-0.1.3/tests/
--rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.3/tests/test_000_import.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.721707 sphere_base-0.1.4/
+-rw-rw-rw-   0        0        0      978 2023-04-16 07:19:30.000000 sphere_base-0.1.4/HISTORY.rst
+-rw-rw-rw-   0        0        0     1105 2023-04-16 08:54:46.000000 sphere_base-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-03-15 14:22:33.000000 sphere_base-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1987 2023-04-22 14:09:52.720707 sphere_base-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-04-21 08:51:12.000000 sphere_base-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.495694 sphere_base-0.1.4/docs/
+-rw-rw-rw-   0        0        0      638 2023-03-15 17:55:12.000000 sphere_base-0.1.4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.470693 sphere_base-0.1.4/docs/build/
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.471693 sphere_base-0.1.4/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.499694 sphere_base-0.1.4/docs/build/html/_static/
+-rw-rw-rw-   0        0        0      286 2023-03-15 17:53:40.000000 sphere_base-0.1.4/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.4/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-03-15 17:53:40.000000 sphere_base-0.1.4/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      804 2023-03-15 17:55:12.000000 sphere_base-0.1.4/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.502695 sphere_base-0.1.4/docs/source/
+-rw-rw-rw-   0        0        0     1175 2023-03-16 20:29:33.000000 sphere_base-0.1.4/docs/source/conf.py
+-rw-rw-rw-   0        0        0      489 2023-03-16 21:15:47.000000 sphere_base-0.1.4/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.601700 sphere_base-0.1.4/docs/source/rst/
+-rw-rw-rw-   0        0        0      163 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.model.mesh.rst
+-rw-rw-rw-   0        0        0      166 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.model.model.rst
+-rw-rw-rw-   0        0        0      169 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.model.models.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.model.obj_file_loader.rst
+-rw-rw-rw-   0        0        0      369 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.model.rst
+-rw-rw-rw-   0        0        0      196 2023-03-16 21:18:48.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.rst
+-rw-rw-rw-   0        0        0      780 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_base_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_circle_shader.rst
+-rw-rw-rw-   0        0        0      203 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_cross_shader.rst
+-rw-rw-rw-   0        0        0      209 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_default_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_flat_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_holo_sphere_shader.rst
+-rw-rw-rw-   0        0        0      200 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_node_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_skybox_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_socket_shader.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_sphere_edge_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_sphere_shader.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_sphere_small_shader.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.shader.uv_square_shader.rst
+-rw-rw-rw-   0        0        0      602 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sov_conf.rst
+-rw-rw-rw-   0        0        0      206 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sov_edge.rst
+-rw-rw-rw-   0        0        0      212 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sov_sphere.rst
+-rw-rw-rw-   0        0        0      246 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sov_sphere_node_base.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sov_uv_widget.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.edge_sphere_item.rst
+-rw-rw-rw-   0        0        0      273 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.item_sphere_node.rst
+-rw-rw-rw-   0        0        0      279 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.person_sphere_node.rst
+-rw-rw-rw-   0        0        0      502 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.sphere_nodes.rst
+-rw-rw-rw-   0        0        0     1563 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_calc.rst
+-rw-rw-rw-   0        0        0      223 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_cam.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_cam_movement.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_clipboard.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_config.rst
+-rw-rw-rw-   0        0        0      241 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_constants.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_edge_drag.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_disc.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_item.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_node.rst
+-rw-rw-rw-   0        0        0      258 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_graphic_socket.rst
+-rw-rw-rw-   0        0        0      235 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_history.rst
+-rw-rw-rw-   0        0        0      243 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_mouse_ray.rst
+-rw-rw-rw-   0        0        0      226 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_node.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_rubber_band.rst
+-rw-rw-rw-   0        0        0      250 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_serializable.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_skybox.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_socket.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere.rst
+-rw-rw-rw-   0        0        0      249 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_sphere_edge.rst
+-rw-rw-rw-   0        0        0      252 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_surface_edge.rst
+-rw-rw-rw-   0        0        0      238 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_universe.rst
+-rw-rw-rw-   0        0        0      229 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_utils.rst
+-rw-rw-rw-   0        0        0      232 2023-03-16 21:09:16.000000 sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.suv_widget.rst
+-rw-rw-rw-   0        0        0      127 2023-03-15 17:49:53.000000 sphere_base-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 14:09:52.721707 sphere_base-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-04-22 14:09:46.000000 sphere_base-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.612701 sphere_base-0.1.4/sphere_base/
+-rw-rw-rw-   0        0        0      106 2023-04-21 12:08:43.000000 sphere_base-0.1.4/sphere_base/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-04-20 14:05:18.000000 sphere_base-0.1.4/sphere_base/calc.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 10:13:03.000000 sphere_base-0.1.4/sphere_base/clipboard.py
+-rw-rw-rw-   0        0        0     5131 2023-04-22 13:52:18.000000 sphere_base-0.1.4/sphere_base/config.py
+-rw-rw-rw-   0        0        0     4839 2023-04-20 17:12:04.000000 sphere_base-0.1.4/sphere_base/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.637702 sphere_base-0.1.4/sphere_base/edge/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:32:40.000000 sphere_base-0.1.4/sphere_base/edge/__init__.py
+-rw-rw-rw-   0        0        0     7711 2023-04-20 09:15:29.000000 sphere_base-0.1.4/sphere_base/edge/edge_drag.py
+-rw-rw-rw-   0        0        0     4592 2023-04-20 07:51:22.000000 sphere_base-0.1.4/sphere_base/edge/graphic_edge.py
+-rw-rw-rw-   0        0        0      809 2023-04-19 12:36:22.000000 sphere_base-0.1.4/sphere_base/edge/graphic_line.py
+-rw-rw-rw-   0        0        0     1859 2023-04-04 08:07:28.000000 sphere_base-0.1.4/sphere_base/edge/inter_sphere_edge.py
+-rw-rw-rw-   0        0        0    14126 2023-04-22 13:09:36.000000 sphere_base-0.1.4/sphere_base/edge/surface_edge.py
+-rw-rw-rw-   0        0        0     9835 2023-04-08 12:55:07.000000 sphere_base-0.1.4/sphere_base/history.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.644703 sphere_base-0.1.4/sphere_base/model/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.4/sphere_base/model/__init__.py
+-rw-rw-rw-   0        0        0     4197 2023-04-20 17:16:58.000000 sphere_base-0.1.4/sphere_base/model/mesh.py
+-rw-rw-rw-   0        0        0     6415 2023-04-22 13:52:18.000000 sphere_base-0.1.4/sphere_base/model/model.py
+-rw-rw-rw-   0        0        0     3379 2023-04-22 13:55:17.000000 sphere_base-0.1.4/sphere_base/model/models.py
+-rw-rw-rw-   0        0        0    23247 2023-04-22 13:52:18.000000 sphere_base-0.1.4/sphere_base/model/obj_file_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.646703 sphere_base-0.1.4/sphere_base/model/resources/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.4/sphere_base/model/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.647703 sphere_base-0.1.4/sphere_base/model/resources/meshes/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.4/sphere_base/model/resources/meshes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.649703 sphere_base-0.1.4/sphere_base/model/resources/shaders/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.4/sphere_base/model/resources/shaders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.663704 sphere_base-0.1.4/sphere_base/node/
+-rw-rw-rw-   0        0        0        0 2023-03-30 07:35:09.000000 sphere_base-0.1.4/sphere_base/node/__init__.py
+-rw-rw-rw-   0        0        0     8053 2023-04-22 13:09:36.000000 sphere_base-0.1.4/sphere_base/node/graphic_disc.py
+-rw-rw-rw-   0        0        0     2676 2023-04-03 06:31:17.000000 sphere_base-0.1.4/sphere_base/node/graphic_node.py
+-rw-rw-rw-   0        0        0     2449 2023-04-03 06:31:16.000000 sphere_base-0.1.4/sphere_base/node/graphic_socket.py
+-rw-rw-rw-   0        0        0    13296 2023-04-22 13:09:36.000000 sphere_base-0.1.4/sphere_base/node/node.py
+-rw-rw-rw-   0        0        0     8804 2023-04-22 13:09:36.000000 sphere_base-0.1.4/sphere_base/node/socket.py
+-rw-rw-rw-   0        0        0     1737 2023-03-30 07:13:13.000000 sphere_base-0.1.4/sphere_base/serializable.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.689705 sphere_base-0.1.4/sphere_base/shader/
+-rw-rw-rw-   0        0        0      258 2021-03-02 15:14:54.000000 sphere_base-0.1.4/sphere_base/shader/__init__.py
+-rw-rw-rw-   0        0        0     9269 2023-04-22 11:12:03.000000 sphere_base-0.1.4/sphere_base/shader/base_shader.py
+-rw-rw-rw-   0        0        0     1979 2023-04-20 17:16:57.000000 sphere_base-0.1.4/sphere_base/shader/circle_shader.py
+-rw-rw-rw-   0        0        0     1969 2023-04-20 17:16:57.000000 sphere_base-0.1.4/sphere_base/shader/cross_shader.py
+-rw-rw-rw-   0        0        0      572 2023-03-30 09:23:40.000000 sphere_base-0.1.4/sphere_base/shader/default_shader.py
+-rw-rw-rw-   0        0        0     2235 2023-04-20 09:28:14.000000 sphere_base-0.1.4/sphere_base/shader/drag_edge_shader.py
+-rw-rw-rw-   0        0        0     1164 2023-04-20 17:31:03.000000 sphere_base-0.1.4/sphere_base/shader/edge_shader.py
+-rw-rw-rw-   0        0        0      909 2023-04-20 17:16:58.000000 sphere_base-0.1.4/sphere_base/shader/flat_shader.py
+-rw-rw-rw-   0        0        0     1467 2023-04-20 17:16:57.000000 sphere_base-0.1.4/sphere_base/shader/holo_sphere_shader.py
+-rw-rw-rw-   0        0        0     1166 2023-04-20 17:16:57.000000 sphere_base-0.1.4/sphere_base/shader/node_shader.py
+-rw-rw-rw-   0        0        0     2150 2023-04-20 17:12:04.000000 sphere_base-0.1.4/sphere_base/shader/skybox_shader.py
+-rw-rw-rw-   0        0        0     1261 2023-04-20 17:16:58.000000 sphere_base-0.1.4/sphere_base/shader/socket_shader.py
+-rw-rw-rw-   0        0        0     3117 2023-04-20 17:31:03.000000 sphere_base-0.1.4/sphere_base/shader/sphere_edge_shader.py
+-rw-rw-rw-   0        0        0     1668 2023-04-20 17:16:58.000000 sphere_base-0.1.4/sphere_base/shader/sphere_shader.py
+-rw-rw-rw-   0        0        0     1254 2023-04-20 17:16:58.000000 sphere_base-0.1.4/sphere_base/shader/sphere_small_shader.py
+-rw-rw-rw-   0        0        0     1845 2023-04-20 17:16:58.000000 sphere_base-0.1.4/sphere_base/shader/square_shader.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.692705 sphere_base-0.1.4/sphere_base/sphere/
+-rw-rw-rw-   0        0        0        0 2023-03-28 18:59:07.000000 sphere_base-0.1.4/sphere_base/sphere/__init__.py
+-rw-rw-rw-   0        0        0    28884 2023-04-22 08:44:12.000000 sphere_base-0.1.4/sphere_base/sphere/sphere.py
+-rw-rw-rw-   0        0        0     6068 2023-04-21 07:05:58.000000 sphere_base-0.1.4/sphere_base/sphere/sphere_lines.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.698706 sphere_base-0.1.4/sphere_base/sphere_overlay/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.699706 sphere_base-0.1.4/sphere_base/sphere_overlay/icons/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.701706 sphere_base-0.1.4/sphere_base/sphere_overlay/qss/
+-rw-rw-rw-   0        0        0       25 2023-03-14 20:49:41.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/qss/__init__.py
+-rw-rw-rw-   0        0        0    30464 2021-01-18 11:54:48.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py
+-rw-rw-rw-   0        0        0     1875 2023-03-28 18:59:36.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sov_conf.py
+-rw-rw-rw-   0        0        0     2161 2023-04-20 13:43:23.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sov_sphere.py
+-rw-rw-rw-   0        0        0     1605 2023-04-22 13:09:36.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sov_sphere_node_base.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.706706 sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/
+-rw-rw-rw-   0        0        0      248 2021-03-02 15:18:12.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-04-04 13:53:39.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/edge_sphere_item.py
+-rw-rw-rw-   0        0        0     1084 2023-04-13 12:16:43.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py
+-rw-rw-rw-   0        0        0     1002 2023-04-13 12:14:08.000000 sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.718707 sphere_base-0.1.4/sphere_base/sphere_universe_base/
+-rw-rw-rw-   0        0        0       23 2021-03-11 14:37:00.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/__init__.py
+-rw-rw-rw-   0        0        0     7829 2023-04-15 12:02:34.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_cam.py
+-rw-rw-rw-   0        0        0     3434 2023-04-15 11:53:42.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_cam_movement.py
+-rw-rw-rw-   0        0        0      365 2023-03-28 18:59:36.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_graphic_item.py
+-rw-rw-rw-   0        0        0    15874 2023-04-14 08:50:15.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_mouse_ray.py
+-rw-rw-rw-   0        0        0     7211 2023-04-14 09:13:08.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_rubber_band.py
+-rw-rw-rw-   0        0        0     5378 2023-04-22 11:55:42.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_skybox.py
+-rw-rw-rw-   0        0        0    14150 2023-04-22 12:54:26.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_universe.py
+-rw-rw-rw-   0        0        0    17954 2023-04-20 15:39:40.000000 sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_widget.py
+-rw-rw-rw-   0        0        0     1493 2023-04-21 11:08:11.000000 sphere_base-0.1.4/sphere_base/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.628702 sphere_base-0.1.4/sphere_base.egg-info/
+-rw-rw-rw-   0        0        0     1987 2023-04-22 14:09:52.000000 sphere_base-0.1.4/sphere_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6381 2023-04-22 14:09:52.000000 sphere_base-0.1.4/sphere_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 14:09:52.000000 sphere_base-0.1.4/sphere_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 07:34:46.000000 sphere_base-0.1.4/sphere_base.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      119 2023-04-22 14:09:52.000000 sphere_base-0.1.4/sphere_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-22 14:09:52.000000 sphere_base-0.1.4/sphere_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-22 14:09:52.719707 sphere_base-0.1.4/tests/
+-rw-rw-rw-   0        0        0      530 2023-03-15 14:00:41.000000 sphere_base-0.1.4/tests/test_000_import.py
```

### Comparing `sphere_base-0.1.3/HISTORY.rst` & `sphere_base-0.1.4/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/LICENSE` & `sphere_base-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/PKG-INFO` & `sphere_base-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere_base
-Version: 0.1.3
+Version: 0.1.4
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.3/README.rst` & `sphere_base-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/docs/Makefile` & `sphere_base-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/docs/make.bat` & `sphere_base-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/docs/source/conf.py` & `sphere_base-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/docs/source/rst/sphere_base.shader.rst` & `sphere_base-0.1.4/docs/source/rst/sphere_base.shader.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_overlay.rst` & `sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_overlay.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/docs/source/rst/sphere_base.sphere_universe_base.rst` & `sphere_base-0.1.4/docs/source/rst/sphere_base.sphere_universe_base.rst`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/setup.py` & `sphere_base-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     keywords='sphere_base',
     name='sphere_base',
     packages=find_packages(include=['sphere_base*'], exclude=['examples*', 'test*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rboltze/spherebase',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `sphere_base-0.1.3/sphere_base/calc.py` & `sphere_base-0.1.4/sphere_base/calc.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/clipboard.py` & `sphere_base-0.1.4/sphere_base/clipboard.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/config.py` & `sphere_base-0.1.4/sphere_base/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 """
 A module containing the Configuration class.
 
 """
 
 from sphere_base.constants import *
+from sphere_base.utils import dump_exception
 import os
 
 
 class UvConfig:
     """
     The configuration class contains project wide variables which can be easily shared between modules and classes.
 
     """
-    def __init__(self, universe, skybox_img_dir="", sphere_texture_dir=""):
+    def __init__(self, universe, skybox_img_dir="", sphere_texture_dir="", sphere_icon_dir=""):
         """
         Constructor of the sphere_base class.
 
         :param universe: reference to the :class:`~sphere_iot.uv_universe.Universe`
         :type universe: :class:`~sphere_iot.uv_universe.Universe`
 
         :Instance Variables:
@@ -39,55 +40,60 @@
 
         self.mesh_id_counter = 0  # used in creating new indexes for meshes
 
         self._win_size_changed_listeners = []
         self._view_changed_listeners = []
 
         self.skybox_sets = self.create_skybox_set(skybox_img_dir)
-        self.sphere_textures = self.create_texture_set(SPHERE_TEXTURE_DIR, sphere_texture_dir)
-        self.all_textures = self.create_texture_dict(SPHERE_TEXTURE_DIR, sphere_texture_dir, TEXTURES_DIR, ICONS_DIR)
+        self.sphere_textures = self.create_texture_set(sphere_texture_dir)
+        self.all_textures = self.create_texture_dict(sphere_texture_dir, sphere_icon_dir)
 
     @staticmethod
     def create_skybox_set(skybox_dir=""):
-        set0 = [None]
-        set2 = []
-        set1 = [SKYBOX_IMG_DIR + name for name in os.listdir(SKYBOX_IMG_DIR) if
-                os.path.isdir(os.path.join(SKYBOX_IMG_DIR, name))]
-        if skybox_dir:
-            set2 = [skybox_dir + name for name in os.listdir(skybox_dir) if
-                    os.path.isdir(os.path.join(skybox_dir, name))]
-
-        return set0 + set1 + set2
-
-    def create_texture_dict(self, dir1, dir2, dir3, dir4):
-        # Get all textures from the 3 directories in a dictionary
-        textures = self.create_texture_set(dir1, dir2, dir3, dir4)
+
+        set0, set1 = [None], []
+        try:
+            if skybox_dir:
+                set1 = [skybox_dir + name for name in os.listdir(skybox_dir) if
+                        os.path.isdir(os.path.join(skybox_dir, name))]
+
+            return set0 + set1
+        except Exception as e:
+            dump_exception(e)
+
+    def create_texture_dict(self, dir1, dir2):
+        # Get all textures from the directories in a dictionary
+        textures = self.create_texture_set(dir1, dir2)
         _dict = {}
 
-        for index, file_name in enumerate(textures):
-            key = os.path.basename(file_name)
-            _type = os.path.split(os.path.dirname(file_name))[1]
-            if key in _dict:
-                continue
-            if os.path.isfile(file_name):
-                if file_name.endswith('.jpg') or file_name.endswith('.png'):
-                    _dict[key] = {}
-                    _dict[key]['file_name'] = key
-                    _dict[key]['img_id'] = index
-                    _dict[key]['file_dir_name'] = file_name
-                    _dict[key]['type'] = _type[:-1]  # removing the 's'
-        return _dict
+        try:
+            for index, file_name in enumerate(textures):
+                key = os.path.basename(file_name)
+                _type = os.path.split(os.path.dirname(file_name))[1]
+                if key in _dict:
+                    continue
+                if os.path.isfile(file_name):
+                    if file_name.endswith('.jpg') or file_name.endswith('.png'):
+                        _dict[key] = {}
+                        _dict[key]['file_name'] = key
+                        _dict[key]['img_id'] = index
+                        _dict[key]['file_dir_name'] = file_name
+                        _dict[key]['type'] = _type[:-1]  # removing the 's'
+            return _dict
+        except Exception as e:
+            dump_exception(e)
 
     @staticmethod
     def create_texture_set(*args):
         # puts all the files of all the directories in a list
         _set = []
         for directory in args:
             s = [directory + file_name for file_name in os.listdir(directory)]
             _set += s
+
         return _set
 
     def set_view_loc(self, view):
         """
         Setting the view matrix to be used in OpenGL
 
         :param view: The view matrix
```

### Comparing `sphere_base-0.1.3/sphere_base/constants.py` & `sphere_base-0.1.4/sphere_base/constants.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/edge/edge_drag.py` & `sphere_base-0.1.4/sphere_base/edge/edge_drag.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/edge/graphic_edge.py` & `sphere_base-0.1.4/sphere_base/edge/graphic_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/edge/graphic_line.py` & `sphere_base-0.1.4/sphere_base/edge/graphic_line.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/edge/inter_sphere_edge.py` & `sphere_base-0.1.4/sphere_base/edge/inter_sphere_edge.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/edge/surface_edge.py` & `sphere_base-0.1.4/sphere_base/edge/surface_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 
         # start and end in angles
         return start, end
 
     def update_content(self, value, item_id):
         """
         This is called on all sphere_base items but is currently not used on edges.
-        Updates the content like icons and images
+        Updates the content like sphere_icons and images
 
         """
         # needs to be overridden
         pass
 
     def is_dragging(self, value=False):
         if self._edge_moved == value:
```

### Comparing `sphere_base-0.1.3/sphere_base/history.py` & `sphere_base-0.1.4/sphere_base/history.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/model/mesh.py` & `sphere_base-0.1.4/sphere_base/model/mesh.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/model/model.py` & `sphere_base-0.1.4/sphere_base/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.shader = eval(shader)(self, vertex_shader, fragment_shader, geometry_shader)
 
         if ".obj" == pathlib.Path(obj_file).suffix:
             self.loader = ObjectFileLoader(self, config=self.config)
             self.meshes = self.loader.get_meshes(obj_file)
         else:
             pass
-            # No object file passed, meshes need to be loaded later.
+            # No object file passed, meshes need to be loaded later. This works for edges.
             self.loader = ObjectFileLoader(self, config=self.config)
             self.meshes = self.loader.create_empty_mesh()
 
     def get_number_of_meshes_in_model(self) -> int:
         """
         Returns the number of ``Meshes`` in this ``Model``
         """
```

### Comparing `sphere_base-0.1.3/sphere_base/model/models.py` & `sphere_base-0.1.4/sphere_base/model/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         """
         no_of_meshes = 0
 
         # iterate through all models from the Model dictionary
         for _name in MODELS.keys():
             model_name = _name
             model_id = MODELS[_name]["model_id"]
-            model_file = MESH_DIR + MODELS[_name]["model_file_name"]
+            # model_file = MESH_DIR + MODELS[_name]["model_file_name"]
+            model_file = MODELS[_name]["model_file_name"]
             shader = MODELS[_name]["shader"]
             vertex_shader = MODELS[_name]["vertex_shader"]
             fragment_shader = MODELS[_name]["fragment_shader"]
             geometry_shader = None if MODELS[_name]["geometry_shader"] == "none" else MODELS[_name]["geometry_shader"]
 
             if 'edge' not in model_name:
                 # Create a new model
```

### Comparing `sphere_base-0.1.3/sphere_base/model/obj_file_loader.py` & `sphere_base-0.1.4/sphere_base/model/obj_file_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from sphere_base.model.mesh import Mesh
 from sphere_base.utils import dump_exception
 from OpenGL.GL import *
 from PIL import Image
 
+from importlib_resources import files
+import sphere_base.model.resources.meshes
+
 DEBUG = False
 
 """
 Wavefront .obj file loader, replacing PyAssimp file loader which could not be installed on MAC.
 This replacement file loader is based on code from an OpenGl youtube course (ES
 OpenGL in python e15 - loading 3D .obj files) and only works with .obj wavefront files.
 
@@ -54,15 +57,17 @@
         vert = []  # vertex coordinates
         tex = []  # texture coordinates
         norm = []  # vertex normals
         all_indices = []  # indices for indexed drawing
         meshes, buffer = [], []
 
         try:
-            with open(file_name, 'r') as f:
+            # with open(file_name, 'r') as f:
+            with files(sphere_base.model.resources.meshes).joinpath(file_name).open('r') as f:
+
                 for line in self.non_blank_lines(f):
 
                     values = line.split()
 
                     if values[0] == 'v':
                         vert = self.search_data(values, vert, 'v', 'float')
                     elif values[0] == 'vt':
```

### Comparing `sphere_base-0.1.3/sphere_base/node/graphic_disc.py` & `sphere_base-0.1.4/sphere_base/node/graphic_disc.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,20 +50,20 @@
         self.current_border_width = self.default_border_width
 
         self.last_img_id = self.default_img_id
         self.init_assets()
 
     def _init_unified_icons(self, img_id: int) -> int:
         """
-        This function sets all icons the same, independent of its state. Therefore
+        This function sets all sphere_icons the same, independent of its state. Therefore
         there is no difference between hovered, _selected and default.
 
         .. Warning::
 
-            In some cases all icons should be the same and independent of the state of the item.
+            In some cases all sphere_icons should be the same and independent of the state of the item.
             This is not always desired
 
         """
 
         self.default_img_id, self.selected_img_id, self.hover_img_id = img_id, img_id, img_id
         self.current_img_id, self.last_img_id = img_id, img_id
         return img_id
@@ -71,40 +71,40 @@
     def _init_unified_background_colors(self, background_color: list):
         """
         This function sets all background colours the same, independent of its state. Therefore
         there is no difference between hovered, _selected and default.
 
         .. Warning::
 
-            In some cases all icons should be the same and independent of the state of the item.
+            In some cases all sphere_icons should be the same and independent of the state of the item.
             This is not always desired
 
         """
 
         self.default_background_color = background_color
         self.selected_background_color = background_color
         self.hover_background_color = background_color
         self.current_background_color = background_color
 
     def set_icon_by_name(self, img_name: str) -> int:
         """
-        Receives an image name, sets all icons to that image and returns its id.
+        Receives an image name, sets all sphere_icons to that image and returns its id.
 
         :param img_name: The name of image
         :type img_name: ``str``
         :returns: ``int`` img_id
 
         """
 
         img_id = self.node.config.get_img_id(img_name)
         return self._init_unified_icons(img_id)
 
     def set_icon_by_id(self, img_id: int) -> int:
         """
-        Receives an image id and sets all icons to that image and returns the same id.
+        Receives an image id and sets all sphere_icons to that image and returns the same id.
 
         :param img_id: The id of the image
         :type img_id: ``int``
         :returns: ``int`` img_id
 
         """
```

### Comparing `sphere_base-0.1.3/sphere_base/node/graphic_node.py` & `sphere_base-0.1.4/sphere_base/node/graphic_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/node/graphic_socket.py` & `sphere_base-0.1.4/sphere_base/node/graphic_socket.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/node/node.py` & `sphere_base-0.1.4/sphere_base/node/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     def update_collision_object(self):
         # set the collision object for mouse pointer ray collision
         self.ray.reset_position_collision_object(self)
         self.socket.update_collision_object()
 
     def update_content(self, texture_id: int, sphere_id: int):
         """
-        Updates the content like icons and images
+        Updates the content like sphere_icons and images
 
         :param texture_id: new texture, image or icon
         :type texture_id: ``int``
         :param sphere_id: current target_sphere
         :type sphere_id:  ``int``
         """
 
@@ -273,15 +273,15 @@
 
         self.grNode = None
         self.sphere.uv.mouse_ray.delete_collision_object(self)
         self.sphere.remove_item(self)
 
     def draw(self):
         """
-        Renders all the icons and circles of the node_disc.
+        Renders all the sphere_icons and circles of the node_disc.
         """
         self.socket.draw()
         self.node_disc.draw(self, texture_id=self.texture_id, color=self.gr_node.main_image_color, switch=0)
         self.node_disc.draw(self, color=self.gr_node.current_background_color, switch=2)
 
         self.circle.shader.line_width = self.gr_node.current_border_width
         self.circle.draw(self, scale=self.gr_node.circle_scale, color=self.gr_node.current_border_color)
```

### Comparing `sphere_base-0.1.3/sphere_base/node/socket.py` & `sphere_base-0.1.4/sphere_base/node/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         """
         Returns the 'dragging status' of the node this socket belongs to.
         """
         return self.node.is_dragging(value)
 
     def draw(self):
         """
-        Renders all the icons and circles of the ``Socket``.
+        Renders all the sphere_icons and circles of the ``Socket``.
         """
         if self.gr_socket.is_hover():
             self.socket_disc.draw(self, color=self.gr_socket.current_background_color, switch=2)
             self.circle.shader.line_width = self.gr_socket.current_border_width
             self.circle.draw(self, scale=self.gr_socket.circle_scale, color=self.gr_socket.current_border_color)
 
     def remove(self, with_edges: bool = True):
```

### Comparing `sphere_base-0.1.3/sphere_base/serializable.py` & `sphere_base-0.1.4/sphere_base/serializable.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/base_shader.py` & `sphere_base-0.1.4/sphere_base/shader/base_shader.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 """
 
 from OpenGL.GL import *
 from pyrr import Vector3, matrix44
 import pyrr
 from OpenGL.GL.shaders import compileProgram, compileShader
 from sphere_base.constants import *
+from sphere_base.utils import dump_exception
+
+from importlib_resources import files
+import sphere_base.model.resources.shaders
 
 DEBUG = False
 
 
 class BaseShader:
 
     def __init__(self, parent, vertex_shader=None, fragment_shader=None, geometry_shader=None, *args, **kwargs):
@@ -85,23 +89,23 @@
         Retrieve shader from .glsl file
         :param file_name: Name of the shader to use
         :param file_name: ``str``
         :returns: the content of the shader to use
 
         """
 
-        file_name = SHADER_DIR + file_name
-
-        file_name = file_name.replace('\\', '/')
+        try:
 
-        with open(file_name, "r") as text:
-            output = ""
-            for line in text:
-                output += line
-        return output
+            with files(sphere_base.model.resources.shaders).joinpath(file_name).open('r') as text:
+                output = ""
+                for line in text:
+                    output += line
+            return output
+        except Exception as e:
+            dump_exception(e)
 
     def compile_shader(self):
         """
         compiling the OpenGL shaders
 
         """
```

### Comparing `sphere_base-0.1.3/sphere_base/shader/circle_shader.py` & `sphere_base-0.1.4/sphere_base/shader/circle_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/cross_shader.py` & `sphere_base-0.1.4/sphere_base/shader/cross_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/default_shader.py` & `sphere_base-0.1.4/sphere_base/shader/default_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/drag_edge_shader.py` & `sphere_base-0.1.4/sphere_base/shader/drag_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/edge_shader.py` & `sphere_base-0.1.4/sphere_base/shader/edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/flat_shader.py` & `sphere_base-0.1.4/sphere_base/shader/flat_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/holo_sphere_shader.py` & `sphere_base-0.1.4/sphere_base/shader/holo_sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/node_shader.py` & `sphere_base-0.1.4/sphere_base/shader/node_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/skybox_shader.py` & `sphere_base-0.1.4/sphere_base/shader/skybox_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/socket_shader.py` & `sphere_base-0.1.4/sphere_base/shader/socket_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/sphere_edge_shader.py` & `sphere_base-0.1.4/sphere_base/shader/sphere_edge_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/sphere_shader.py` & `sphere_base-0.1.4/sphere_base/shader/sphere_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/sphere_small_shader.py` & `sphere_base-0.1.4/sphere_base/shader/sphere_small_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/shader/square_shader.py` & `sphere_base-0.1.4/sphere_base/shader/square_shader.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere/sphere.py` & `sphere_base-0.1.4/sphere_base/sphere/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Constructor of the sphere_base class.
 
         :param universe: reference to the :class:`~sphere_iot.uv_universe.Universe`
         :type universe: :class:`~sphere_iot.uv_universe.Universe`
         :param position: position of the sphere_base in universe
         :type position: ``list`` with x, y, z values
         :param texture_id: number indicating which texture to use for the sphere_base
-        :type texture_id: int
+        :type texture_id: int.
 
         :Instance Attributes:
 
             - **node** - Instance of :class:`~sphere_iot.uv_node.Node`
             - **edge** - Instance of :class:`~sphere_iot.uv_edge.SphereSurfaceEdge`
             - **calc** - Instance of :class:`~sphere_iot.uv_calc.UvCalc`
             - **config** - Instance of :class:`~sphere_iot.uv_config.UvConfig`
@@ -366,15 +366,15 @@
 
         .. warning::
 
            Start and end sockets have no further meaning in this  implementation. There is no significant difference
            between start and end other than the order of where the line is initially drawn from.
 
            In future implementations there could be a need to indicate the direction of the relationship between parents
-           and children or the direction of owner ship that goes from a person to the product.
+           and children or the direction of ownership that goes from a person to the product.
 
            This type of order or direction is currently not implemented.
 
         """
 
         sockets = [start_socket, end_socket]
         edges = []
@@ -444,15 +444,15 @@
         .. note::
 
            Only existing nodes need to be dragged, as the position of sockets and edges are
            adjusted automatically. Updating the position of a node trickles down to adjusting the position of the
            center sockets of the _selected nodes and any connected edges.
 
            It is important to maintain the distance to the mouse. So we need to calculate the difference between the
-           current mouse position and the center of the items we are dragging. Otherwise the node centers jumps to
+           current mouse position and the center of the items we are dragging, otherwise the node centers jumps to
            the collision point.
 
         """
         for item in self.items_selected:
             if item.type == "node":
                 # only drag any nodes in the _selected item list
                 item.drag_to(mouse_ray_collision_point)
```

### Comparing `sphere_base-0.1.3/sphere_base/sphere/sphere_lines.py` & `sphere_base-0.1.4/sphere_base/sphere/sphere_lines.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py` & `sphere_base-0.1.4/sphere_base/sphere_overlay/qss/nodeeditor_dark_resources.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_overlay/sov_conf.py` & `sphere_base-0.1.4/sphere_base/sphere_overlay/sov_conf.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere.py` & `sphere_base-0.1.4/sphere_base/sphere_overlay/sov_sphere.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_overlay/sov_sphere_node_base.py` & `sphere_base-0.1.4/sphere_base/sphere_overlay/sov_sphere_node_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     def deserialize(self, data, hashmap={}, restore_id=True):
         res = super().deserialize(data, hashmap, restore_id)
         self.gr_node.set_icon_by_id(self.texture_id)
         return res
 
     def update_content(self, value, sphere_id):
-        """ Each texture (icon, image) has a unique short name. The dictionary node icons
+        """ Each texture (icon, image) has a unique short name. The dictionary node sphere_icons
         contains a translation between a listbox text in the editor content nodes with the image short name
         """
 
         if self.id != sphere_id:
             return
 
         if value in DICTIONARY_SPHERE_NODE_ICONS:
```

### Comparing `sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py` & `sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/item_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py` & `sphere_base-0.1.4/sphere_base/sphere_overlay/sphere_nodes/person_sphere_node.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_cam.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_cam_movement.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_cam_movement.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_mouse_ray.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_mouse_ray.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_rubber_band.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_rubber_band.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_skybox.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_skybox.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """
 
 from sphere_base.sphere_universe_base.suv_graphic_item import GraphicItem
 from collections import namedtuple
 from PIL import Image
 from random import randint
+from sphere_base.utils import dump_exception
 import os
 
 
 class Skybox(GraphicItem):
     Face_texture = namedtuple("faces", "id, face_name, img_type, width, height, path, file_and_path, img_data")
 
     """
@@ -64,17 +65,14 @@
         self.model = self.uv.models.get_model('skybox')
         self.xyz = self.uv.cam.xyz
         self.cf = self.uv.config
 
         # We get the shader from the model
         self.shader = self.model.shader
 
-        self._init_variables()
-
-    def _init_variables(self):
         self.scale = None
         self.index = 0
         self.faces = []
         self.orientation = [0, 0, 0]
         self.paint_skybox = True
 
     def get_skybox_set(self, skybox_name=None, skybox_id=None, random=False):
@@ -117,23 +115,26 @@
         self.create_skybox_faces()
 
     def get_skybox_path(self) -> str:
         """
         Returns the image path of the current active Skybox id
 
         """
+
         path = self.cf.skybox_sets[self.skb_id]
         self.paint_skybox = True if path else False
         return path + "/" if path else path
 
+
     def create_skybox_faces(self):
         """
         Gets the six faces of the Skybox from the image path and adds them to the faces array.
 
         """
+
         path = self.get_skybox_path()
 
         if path:
             self.faces = []
             face_order = ["right", "left", "top", "bottom", "back", "front"]
             for i, face in enumerate(face_order):
                 img = Image.open(path + face + ".png")
```

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_universe.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_universe.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     Shader_class = DefaultShader
     Ray_class = MouseRay
     Skybox_class = Skybox
     RubberBand_class = RubberBand
     Clipboard_class = Clipboard
     Config_class = UvConfig
 
-    def __init__(self, parent, skybox_img_dir=None, sphere_texture_dir=None, pybullet_key=None):
+    def __init__(self, parent, skybox_img_dir=None, sphere_texture_dir=None, sphere_icon_dir=None,
+                 pybullet_key=None):
         """
         Constructor of the ``Universe`` class
 
         :param parent: Reference to the universe class universe widget.
         :type parent: :class:`~sphere_iot.uv_widget.UV_Widget` or  :class:`~sphere_iot.uv_widget_glfw.UWidgetGLFW`.
         :param pybullet_key: Used to run the universe in its own physics engine
         :type pybullet_key: ``str``
@@ -83,15 +84,16 @@
         self.mouse_offset = 0
         self.target_sphere = None
         self._has_been_modified = False
 
         self._init_listeners()
 
         self.config = self.__class__.Config_class(self, skybox_img_dir=skybox_img_dir,
-                                                  sphere_texture_dir=sphere_texture_dir)
+                                                  sphere_texture_dir=sphere_texture_dir,
+                                                  sphere_icon_dir=sphere_icon_dir)
         self.shader = self.__class__.Shader_class(self)
         self.cam = self.__class__.Camera_class(self)
         self.models = self.__class__.Models_class(self)
         self.Sphere = self.__class__.Sphere_class  # not instantiated here!
 
         self.mouse_ray = self.__class__.Ray_class(self, 1)
         self.skybox = self.__class__.Skybox_class(self)
```

### Comparing `sphere_base-0.1.3/sphere_base/sphere_universe_base/suv_widget.py` & `sphere_base-0.1.4/sphere_base/sphere_universe_base/suv_widget.py`

 * *Files identical despite different names*

### Comparing `sphere_base-0.1.3/sphere_base/utils.py` & `sphere_base-0.1.4/sphere_base/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # print("%s EXCEPTION:" % e.__class__.__name__, e)
     # traceback.print_tb(e.__traceback__)
     traceback.print_exc()
 
 
 def load_style_sheet(filename: str):
     """
-    Loads an qss stylesheet to current QApplication instance
+    Loads a qss stylesheet to current QApplication instance
 
     :param filename: Filename of qss stylesheet
     :type filename: str
     """
     print('STYLE loading:', filename)
     file = QFile(filename)
     file.open(QFile.ReadOnly | QFile.Text)
```

### Comparing `sphere_base-0.1.3/sphere_base.egg-info/PKG-INFO` & `sphere_base-0.1.4/sphere_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphere-base
-Version: 0.1.3
+Version: 0.1.4
 Summary: library for applications were information should appear on the surface of a sphere. It allows for creating spheres with nodes and edges that can be dragged on its surface. 
 Home-page: https://github.com/rboltze/spherebase
 Author: Richard Boltze
 Author-email: rboltze@protonmail.com
 License: MIT license
 Keywords: sphere_base
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sphere_base-0.1.3/sphere_base.egg-info/SOURCES.txt` & `sphere_base-0.1.4/sphere_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -89,22 +89,16 @@
 sphere_base/edge/surface_edge.py
 sphere_base/model/__init__.py
 sphere_base/model/mesh.py
 sphere_base/model/model.py
 sphere_base/model/models.py
 sphere_base/model/obj_file_loader.py
 sphere_base/model/resources/__init__.py
-sphere_base/model/resources/icons/__init__.py
-sphere_base/model/resources/images/__init__.py
 sphere_base/model/resources/meshes/__init__.py
 sphere_base/model/resources/shaders/__init__.py
-sphere_base/model/resources/sphere_textures/__init__.py
-sphere_base/model/resources/textures/__init__.py
-sphere_base/model/resources/textures/skybox/__init__.py
-sphere_base/model/resources/textures/skybox/blue1/__init__.py
 sphere_base/node/__init__.py
 sphere_base/node/graphic_disc.py
 sphere_base/node/graphic_node.py
 sphere_base/node/graphic_socket.py
 sphere_base/node/node.py
 sphere_base/node/socket.py
 sphere_base/shader/__init__.py
```

### Comparing `sphere_base-0.1.3/tests/test_000_import.py` & `sphere_base-0.1.4/tests/test_000_import.py`

 * *Files identical despite different names*

