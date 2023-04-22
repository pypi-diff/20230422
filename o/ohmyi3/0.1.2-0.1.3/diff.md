# Comparing `tmp/ohmyi3-0.1.2.tar.gz` & `tmp/ohmyi3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmyi3-0.1.2.tar", max compression
+gzip compressed data, was "ohmyi3-0.1.3.tar", max compression
```

## Comparing `ohmyi3-0.1.2.tar` & `ohmyi3-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.2/LICENSE
--rw-r--r--   0        0        0       43 2023-04-15 22:50:07.408756 ohmyi3-0.1.2/README.md
--rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.2/ohmyi3/commands/entrypoint.py
--rw-r--r--   0        0        0     3204 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/commands/generate.py
--rw-r--r--   0        0        0      411 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/commands/info.py
--rw-r--r--   0        0        0     1529 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/commands/init.py
--rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.2/ohmyi3/config/app.py
--rw-r--r--   0        0        0     2238 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/config/package.py
--rw-r--r--   0        0        0      446 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/i3ctl.py
--rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.2/ohmyi3/services/bootstrap.py
--rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.2/ohmyi3/services/ohmyi3.py
--rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.2/ohmyi3/stubs/README.md
--rw-r--r--   0        0        0      810 2023-04-20 22:44:05.536672 ohmyi3-0.1.2/ohmyi3/stubs/config.d/00-header.conf
--rw-r--r--   0        0        0     1985 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/05-system.conf
--rw-r--r--   0        0        0     2904 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/10-autostart.conf
--rw-r--r--   0        0        0      662 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/15-borders.conf
--rw-r--r--   0        0        0     6436 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/20-navigation.conf
--rw-r--r--   0        0        0     3212 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/80-applications.conf
--rw-r--r--   0        0        0     6720 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/85-windows.conf
--rw-r--r--   0        0        0     3195 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.d/90-gaps.conf
--rw-r--r--   0        0        0    10089 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/config.py
--rw-r--r--   0        0        0       33 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/alacritty/__init__.py
--rw-r--r--   0        0        0      893 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/alacritty/alacritty.py
--rw-r--r--   0        0        0       29 2023-04-20 22:44:15.316835 ohmyi3-0.1.2/ohmyi3/stubs/plugins/archey3/__init__.py
--rw-r--r--   0        0        0      958 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/archey3/archey3.py
--rw-r--r--   0        0        0       31 2023-04-20 22:44:15.316835 ohmyi3-0.1.2/ohmyi3/stubs/plugins/nitrogen/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
--rw-r--r--   0        0        0       29 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/polybar/__init__.py
--rw-r--r--   0        0        0     2188 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/plugins/polybar/polybar.py
--rw-r--r--   0        0        0   385109 2023-04-20 22:44:29.983747 ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/background.jpg
--rw-r--r--   0        0        0     1874 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/theme.conf
--rw-r--r--   0        0        0   198158 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/background.jpg
--rw-r--r--   0        0        0     1915 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/theme.conf
--rw-r--r--   0        0        0     1869 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/i3status.conf
--rw-r--r--   0        0        0   108928 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/background.jpg
--rw-r--r--   0        0        0     1935 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/theme.conf
--rw-r--r--   0        0        0   514555 2023-04-20 22:44:29.987080 ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/background.jpg
--rw-r--r--   0        0        0     2422 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/theme.conf
--rw-r--r--   0        0        0     3747 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/ohmyi3/util.py
--rw-r--r--   0        0        0      703 2023-04-20 23:03:25.268975 ohmyi3-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ohmyi3-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-15 19:45:51.088364 ohmyi3-0.1.3/LICENSE
+-rw-r--r--   0        0        0    22565 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/README.md
+-rw-r--r--   0        0        0     1131 2023-04-16 01:52:38.895592 ohmyi3-0.1.3/ohmyi3/commands/entrypoint.py
+-rw-r--r--   0        0        0     3208 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/commands/generate.py
+-rw-r--r--   0        0        0      432 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/commands/info.py
+-rw-r--r--   0        0        0     1529 2023-04-20 23:03:25.268975 ohmyi3-0.1.3/ohmyi3/commands/init.py
+-rw-r--r--   0        0        0      591 2023-04-16 02:01:06.406276 ohmyi3-0.1.3/ohmyi3/config/app.py
+-rw-r--r--   0        0        0     2238 2023-04-20 23:03:25.268975 ohmyi3-0.1.3/ohmyi3/config/package.py
+-rw-r--r--   0        0        0      446 2023-04-20 23:03:25.268975 ohmyi3-0.1.3/ohmyi3/i3ctl.py
+-rw-r--r--   0        0        0      814 2023-04-15 19:45:51.085030 ohmyi3-0.1.3/ohmyi3/services/bootstrap.py
+-rw-r--r--   0        0        0     2529 2023-04-16 19:40:39.743720 ohmyi3-0.1.3/ohmyi3/services/ohmyi3.py
+-rw-r--r--   0        0        0      188 2023-04-16 20:00:12.022854 ohmyi3-0.1.3/ohmyi3/stubs/README.md
+-rw-r--r--   0        0        0      810 2023-04-22 16:38:39.408913 ohmyi3-0.1.3/ohmyi3/stubs/config.d/00-header.conf
+-rw-r--r--   0        0        0     1985 2023-04-22 16:38:39.408913 ohmyi3-0.1.3/ohmyi3/stubs/config.d/05-system.conf
+-rw-r--r--   0        0        0     3035 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/10-autostart.conf
+-rw-r--r--   0        0        0      775 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/15-borders.conf
+-rw-r--r--   0        0        0     6434 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/20-navigation.conf
+-rw-r--r--   0        0        0     3212 2023-04-22 16:38:39.412246 ohmyi3-0.1.3/ohmyi3/stubs/config.d/80-applications.conf
+-rw-r--r--   0        0        0     6720 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.d/85-windows.conf
+-rw-r--r--   0        0        0     3195 2023-04-22 16:38:39.412246 ohmyi3-0.1.3/ohmyi3/stubs/config.d/90-gaps.conf
+-rw-r--r--   0        0        0    12738 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/stubs/config.py
+-rw-r--r--   0        0        0       33 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/alacritty/__init__.py
+-rw-r--r--   0        0        0      893 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/alacritty/alacritty.py
+-rw-r--r--   0        0        0       29 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/archey3/__init__.py
+-rw-r--r--   0        0        0      958 2023-04-22 16:38:50.699004 ohmyi3-0.1.3/ohmyi3/stubs/plugins/archey3/archey3.py
+-rw-r--r--   0        0        0       31 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/nitrogen/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/nitrogen/nitrogen.py
+-rw-r--r--   0        0        0       29 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/polybar/__init__.py
+-rw-r--r--   0        0        0     2188 2023-04-22 16:38:50.702337 ohmyi3-0.1.3/ohmyi3/stubs/plugins/polybar/polybar.py
+-rw-r--r--   0        0        0   385109 2023-04-22 16:39:04.589120 ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/background.jpg
+-rw-r--r--   0        0        0     1874 2023-04-22 16:39:04.589120 ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/theme.conf
+-rw-r--r--   0        0        0   198158 2023-04-22 16:39:04.589120 ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/background.jpg
+-rw-r--r--   0        0        0     1915 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/theme.conf
+-rw-r--r--   0        0        0     1869 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/i3status.conf
+-rw-r--r--   0        0        0   108928 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/background.jpg
+-rw-r--r--   0        0        0     1935 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/theme.conf
+-rw-r--r--   0        0        0   514555 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/background.jpg
+-rw-r--r--   0        0        0     2422 2023-04-22 16:39:04.592453 ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/theme.conf
+-rw-r--r--   0        0        0     5683 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/ohmyi3/util.py
+-rw-r--r--   0        0        0      703 2023-04-22 16:39:52.219550 ohmyi3-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    23384 1970-01-01 00:00:00.000000 ohmyi3-0.1.3/PKG-INFO
```

### Comparing `ohmyi3-0.1.2/LICENSE` & `ohmyi3-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/commands/entrypoint.py` & `ohmyi3-0.1.3/ohmyi3/commands/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/commands/generate.py` & `ohmyi3-0.1.3/ohmyi3/commands/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     # Append config.d/* and theme.d/theme to new i3 config
     with open(i3config_file, "w") as f:
         # Loop and merge each config and append to
         for file in files:
             uvicore.log.item2(f"Appending {file}")
             f.write(template(file, values=config))
-            f.write("\n\n\n")
+            f.write("\n\n\n\n\n")
 
         # Append the selected theme files
         theme_file = path([active_theme_path, 'theme.conf'])
         if os.path.exists(theme_file):
             uvicore.log.item(f"Appending THEME {config.theme}")
             f.write(template(theme_file, values=config))
```

### Comparing `ohmyi3-0.1.2/ohmyi3/commands/init.py` & `ohmyi3-0.1.3/ohmyi3/commands/init.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/config/app.py` & `ohmyi3-0.1.3/ohmyi3/config/app.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/config/package.py` & `ohmyi3-0.1.3/ohmyi3/config/package.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/services/bootstrap.py` & `ohmyi3-0.1.3/ohmyi3/services/bootstrap.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/services/ohmyi3.py` & `ohmyi3-0.1.3/ohmyi3/services/ohmyi3.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/00-header.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/00-header.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/05-system.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/05-system.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/10-autostart.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/10-autostart.conf`

 * *Files 15% similar despite different names*

```diff
@@ -6,72 +6,77 @@
 # The --no-startup-id parameter disables startup-notification support for this
 # particular exec command. With startup-notification, i3 can make sure that a window
 # appears on the workspace on which you used the exec command. Also, it will change
 # the X11 cursor to watch (a clock) while the application is launching. So, if an
 # application is not startup-notification aware (most GTK and Qt using applications
 # seem to be, though), you will end up with a watch cursor for 60 seconds.
 
-{% if desktop == 'i3' %}
+{% for name, cmd in autostart.items() %}{% if cmd %}
+# Start {{ name }}
+{{ cmd }}{% endif %}
+{% endfor %}
 
-    # Policy Kit authenticator
-    #exec --no-startup-id /usr/lib/polkit-gnome/polkit-gnome-authentication-agent-1
-    exec --no-startup-id /usr/lib/polkit-kde-authentication-agent-1
 
-    # arandr/xrandr to force default screen/monitor layout
-    exec --no-startup-id ~/.screenlayout/screen-laptop.sh; sleep 1
 
-    # Clipboard manager
-    exec --no-startup-id {{ apps.clipboard }}
+# if desktop == 'i3'
 
-    {% if os == 'manjaro' %}
-    exec --no-startup-id matray
-    {% endif %}
+#     # Policy Kit authenticator
+#     #exec --no-startup-id /usr/lib/polkit-gnome/polkit-gnome-authentication-agent-1
+#     exec --no-startup-id /usr/lib/polkit-kde-authentication-agent-1
 
-    # Network Manager icon in i3 bar
-    exec --no-startup-id {{ tray.network }}
+#     # arandr/xrandr to force default screen/monitor layout
+#     exec --no-startup-id ~/.screenlayout/screen-laptop.sh; sleep 1
 
-    # Volumn icon in i3 bar
-    exec --no-startup-id {{ tray.volume }}
+#     # Clipboard manager
+#     exec --no-startup-id {{ apps.clipboard }}
 
-    # Power Management and Screen Locking
-    # xss-lock waits until xfce4-power-manager (or any manager) turns off screen, then starts i3lock
-    exec_always --no-startup-id {{ apps.powermanager }}
-    exec_always --no-startup-id {{ apps.xsslock }}
-    #exec --no-startup-id xautolock -time 10 -locker blurlock
-    #exec --no-startup-id xss-lock -- blurlock
+#     {% if os == 'manjaro' %}
+#     exec --no-startup-id matray
+#     {% endif %}
 
-    # Reset keyboard speed and fix_xcursor
-    exec_always --no-startup-id xset r rate 250 50
-    #exec_always --no-startup-id fix_xcursor
+#     # Network Manager icon in i3 bar
+#     ###exec --no-startup-id  tray.network
 
-    # Start xfsettingsd to get xfce GTK themes (if running in i3 code with xfce desktop tools)
-    {% if desktop_tools == 'xfce' %}
-    exec --no-startup-id xfsettingsd
-    {% endif %}
+#     # Volumn icon in i3 bar
+#     ###exec --no-startup-id  tray.volume
 
-    # Polybar
-    exec_always --no-startup-id ~/.config/polybar/launch.sh --{{ polybar.theme }}
+#     # Power Management and Screen Locking
+#     # xss-lock waits until xfce4-power-manager (or any manager) turns off screen, then starts i3lock
+#     exec_always --no-startup-id {{ apps.powermanager }}
+#     exec_always --no-startup-id {{ apps.xsslock }}
+#     #exec --no-startup-id xautolock -time 10 -locker blurlock
+#     #exec --no-startup-id xss-lock -- blurlock
 
-{% endif %}
+#     # Reset keyboard speed and fix_xcursor
+#     exec_always --no-startup-id xset r rate 250 50
+#     #exec_always --no-startup-id fix_xcursor
 
+#     # Start xfsettingsd to get xfce GTK themes (if running in i3 code with xfce desktop tools)
+#     {% if desktop_tools == 'xfce' %}
+#     exec --no-startup-id xfsettingsd --replace
+#     {% endif %}
 
-# Nitrogen to set i3 background wallpaper
-# AND picom compositor after nitrogen has loaded
-#exec --no-startup-id nitrogen --restore; sleep 1; picom -b
-exec_always --no-startup-id nitrogen --restore
-exec_always --no-startup-id picom --config ~/.config/picom/picom.conf -b
+#     # Polybar
+#     exec_always --no-startup-id ~/.config/polybar/launch.sh --{{ polybar.theme }}
 
-# Pamac out of date packages icon in i3 bar
-#exec --no-startup-id pamac-tray
+# endif
 
-# Windows like alttab for i3
-# Colors: manjaro green
-exec_always --no-startup-id "alttab -fg '#106E5C' -bg '#0E2229' -frame '#106E5C' -t 128x150 -i 127x64"
+# # Background/Wallpaper Manager (ie Nitrogen and feh)
+# exec_always --no-startup-id {{ autostart.wallpaper }}
 
+# # Compositor (picom, compton (which is old picom) etc...)
+# exec_always --no-startup-id {{ autostart.compositor }}
 
 
+# # Pamac out of date packages icon in i3 bar
+# #exec --no-startup-id pamac-tray
+
+# # Windows like alttab for i3
+# # Colors: manjaro green
+# exec_always --no-startup-id "alttab -fg '#106E5C' -bg '#0E2229' -frame '#106E5C' -t 128x150 -i 127x64"
+
 # Not Used
 #exec --no-startup-id clipit
 #exec --no-startup-id blueman-applet
 #exec_always --no-startup-id sbxkb
 #exec --no-startup-id start_conky_maia
 #exec --no-startup-id start_conky_green
```

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/15-borders.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/15-borders.conf`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 ################################################################################
 # Border Configuration
-# ################################################################################
+################################################################################
 
 # Configure border style <normal|1pixel|pixel xx|none|pixel>
 default_border pixel 1
 default_floating_border normal
 
 # Toggle borders for terminal
-bindsym $mod+b exec i3-msg '[class="(?i){{ apps.terminal }}"] border toggle 1'
+bindsym $mod+b exec --no-startup-id i3-msg '[class="(?i){{ apps.terminal }}"] border pixel 1'
+bindsym $mod+Shift+b exec --no-startup-id i3-msg '[class="(?i){{ apps.terminal }}"] border pixel 0'
 
 # You can hide container borders adjacent to the screen edges
 # hide_edge_borders none|vertical|horizontal|both|smart
 hide_edge_borders none
 
 # Change borders
 #bindsym $mod+u border none
```

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/20-navigation.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/20-navigation.conf`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ################################################################################
 # Navigation Configuration
-# ################################################################################
+################################################################################
 
 # Use Mouse+$mod to drag floating windows
 floating_modifier $mod
 
 # focus_follows_mouse no
 
 # Change focus of containers (between all parent and children)
```

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/80-applications.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/80-applications.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/85-windows.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/85-windows.conf`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # Open applications on specific workspaces
 # assign [class="Thunderbird"] $ws1
 # assign [class="Pale moon"] $ws2
 # assign [class="Pcmanfm"] $ws3
 # assign [class="Skype"] $ws5
 
 # Enable window icons for all windows
-for_window [all] title_window_icon on
 {% if os != 'lmde' %}
+for_window [all] title_window_icon on
 for_window [all] title_window_icon padding 5px
 {% endif %}
 
 # Open these applications in floating mode
 # Options are
 #   floating enable
 #   sticky enable
```

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.d/90-gaps.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/config.d/90-gaps.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/config.py` & `ohmyi3-0.1.3/ohmyi3/stubs/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import uvicore
 from ohmyi3 import util
 from uvicore.typing import Dict
 from uvicore.configuration import env
 from uvicore.support.dumper import dump, dd
-from ohmyi3.util import Overridable, gather, path, plugin
+from ohmyi3.util import set, gather, path, plugin
 
-# Settings and hooks for ohmyi3 i3ctl config generator.
-# Configs as python gives unlimited flexibility and programability.
-# All of these self.* variables are accessible as jinja2 variables
-# to dynamically control your i3 configs and anything else that
-# requires automation (see the plugins)
+# Ohmyi3 user configuration.
+#
+# This config is what drives the i3ctl generator.
+# All variables inside config() will be available to the jinja2 templating engine
+# and may be used in your config.d/* i3 configs for dynamic conditions.
+# Use the before_generate() and after_generate() hooks to fire off plugins/*
+# to control the rest of your system (set wallpaper, alacritty themes, polybar...)
+# From here on out, the power is in your hands.  Automation is now limitless!
 
 def config():
     """Ohmyi3 variables for configuring and templating i3"""
 
     # Hostname and user from system
     host = util.hostname()
     user = util.loggedinuser()
 
-    # Refresh overridables with all local variables thus far
-    set = Overridable(**locals())
 
     # Paths to all relevant locations
     # If you need to change the ohmyi3 path, use the
     # environment variable OHMYI3_PATH (default ~/.config/ohmyi3)
     ohmyi3_path = uvicore.config('ohmyi3.config_path')
     paths = set({
         'ohmyi3': path(ohmyi3_path),
@@ -31,157 +32,182 @@
         'ohmyi3_themes': path([ohmyi3_path, 'themes']),
         'i3': path('~/.config/i3'),
         'i3status': path('~/.config/i3status'),
         'alacritty': path('~/.config/alacritty'),
         'polybar': path('~/.config/polybar'),
     })
 
-    # OS variant
-    os = set('manjaro', if_host={
-        'p14s': 'lmde'
+    # Unix OS Variant
+    os = set('manjaro', host, {
+        'p14s': 'lmde',
     })
 
+
     # Main network interface
-    net_interface = set('enp11s0', if_host={
+    net_interface = set('enp11s0', host, {
         'p15': 'enp11s0',
         'p53': 'wlp0s20f3',
         'deajaro': 'wlp2s0',
     })
 
+
     # Has battery (laptop?)
-    has_battery = set(True, if_host={
+    has_battery = set(True, host, {
         'sunjaro': False,
         'p53': True,
         'p15': True,
         'p14s': True,
     })
     battery_device = set('BAT0')
 
+
     # Backlinght
     backlight_device = set('intel_backlight')
 
+
     # Desktop Environment (kde, xfce, i3, cinnamon, mate, gnome)
     # I like to run i3 inside kde and xfce etc...  If runing under these DE's
     # I need to tweak the configs (no screen lock, different autostarts etc...)
-    desktop = set('i3', if_host={
+    desktop = set('i3', host, {
         'sunjaro': 'kde',
         'p53': 'i3',
         'p15': 'i3',
         #'p14s': 'cinnamon',
     })
 
+
     # Main desktop tools (kde, xfce...)
     # Not the same as desktop, which is the running Desktop Environment
-    desktop_tools = set('kde', if_host={
+    desktop_tools = set('kde', host, {
         'deajaro': 'xfce'
     })
 
+
     # Using i3 capable of gaps
-    i3_gaps = set(True, if_host={
+    i3_gaps = set(True, host, {
         'p14s': False
     })
 
+
     # Restart i3 command
-    i3_restart = set('~/.files/scripts/i3ctl-dev generate && i3-msg restart', if_host={
+    i3_restart = set('~/.files/scripts/i3ctl-dev generate && i3-msg restart', host, {
         'deajaro': 'i3ctl generate && i3-msg restart',
+        'p14s': '/home/mreschke/.pyenv/shims/i3ctl generate && i3-msg restart',
     })
 
+
     # Wallpaper base
-    wallpaper_base = set('~/Wallpaper', if_host={
+    wallpaper_base = set('~/Wallpaper', host, {
         'sunjaro': '~/Pictures/Wallpaper',
         'p53': '~/Pictures/Wallpaper',
     })
 
+
     # Current theme (amber, archlinux, manjaro, pink)
-    theme = set('manjaro', if_host={
+    theme = set('manjaro', host, {
         'sunjaro': 'manjaro',
         'p53': 'manjaro',
-        'p15': 'pink',
+        'p15': 'amber',
         'p14s': 'manjaro',
     })
 
-    # Refresh overridables with all local variables thus far
-    set = Overridable(**locals())
 
     # Extra theme details
     # Wallpaper is an OVERRIDE, else defaults to the themes folder/background.[jpg|png]
     themes = set({
         'amber': {
+            'color': '#EF5B1A',
+            'archey3': 'yellow',
             #'wallpaper': 'Abstract/cracked_orange.jpg',
             #'wallpaper': 'Manjaro/antelope-canyon-984055.jpg',
             #'wallpaper': 'Scenes/digital_sunset.jpg',
             #'wallpaper': 'LinuxMint/linuxmint-vera/mpiwnicki_red_dusk.jpg',
             #'wallpaper': 'LinuxMint/linuxmint-vanessa/navi_india.jpg',
-            'wallpaper': 'LinuxMint/linuxmint-una/nwatson_eclipse.jpg',
+            #'wallpaper': 'LinuxMint/linuxmint-una/nwatson_eclipse.jpg',
             #'wallpaper': 'LinuxMint/linuxmint-vera/navi_india.jpg',
             #'wallpaper': 'LinuxMint/linuxmint-ulyssa/tangerine_nanpu.jpg',
             #'wallpaper': 'Manjaro/sky-3189347.jpg',
-            'archey3': 'yellow',
         },
         'archlinux': {
-            #'wallpaper': 'Archlinux/349880.jpg',
+            'color': '#1793D1',
             'archey3': 'blue',
+            #'wallpaper': 'Archlinux/349880.jpg',
             'wallpaper': 'De/budgie.jpg',
+
         },
         'manjaro': {
+            'color': '#106E5C',
+            'archey3': 'green',
             #'wallpaper': 'Manjaro/illyria-default-lockscreen-nobrand.jpg',
             #'wallpaper': 'Manjaro/wpM_orbit2_textured.jpg'
             'wallpaper': 'De/deepin.jpg',
-            'archey3': 'green',
+
         },
         'pink': {
+            'color': '#b41474',
+            'archey3': 'magenta',
             #'wallpaper': 'Abstract/artistic_colors2.jpg',
             #'wallpaper': 'Landscape/backlit-chiemsee-dawn-1363876.jpg',
             #`'wallpaper': 'Manjaro/DigitalMilkyway.png',
             #'wallpaper': 'LinuxMint/linuxmint-una/eeselioglu_istanbul.jpg',
             #'wallpaper': 'Abstract/neon_huawei.jpg',
-            'wallpaper': 'De/budgie.jpg',
-            'archey3': 'magenta',
+            #'wallpaper': 'De/budgie.jpg',
+            'wallpaper': 'De/deepin.jpg',
         },
     },
-        if_host={
+        host, {
             #'p15': {'manjaro.wallpaper': 'Manjaro/wpM_orbit2_textured.jpg'}
-            'p15': {'manjaro.wallpaper': 'De/deepin.jpg'}
+            #'p53': {'manjaro.wallpaper': 'De/deepin.jpg!!!'}
         }
     )
 
+
     # Polybar
     # Specific to the custom qpanel theme made from this https://github.com/adi1090x/polybar-themes
     polybar = set({
         'enabled': True,
         # blocks|colorblocks|cuts|docky|forest|grayblocks|hack|material
         # panels|pwidgets|qpanels|shades|shapes
         'theme': 'qpanels',
         # budgie|deepin|elight|edark|gnomw|klight|kdark
         # liri|mint|ugnome|unity|xubuntu|zorin
         'subtheme': 'deepin'
-    }, if_host={
-        'p14s': {'polybar.enabled': False},
+    }, host, {
+        'p14s': {'enabled': False},
     })
 
+
     # Rofi
     rofi = set({
         'launcher': f'~/.config/polybar/{polybar.theme}/scripts/launcher.sh --{polybar.subtheme}',
         'powermenu': f'~/.config/polybar/{polybar.theme}/scripts/powermenu.sh --{polybar.subtheme}',
-    },
-        if_host={
-            'p14s': {'launcher': 'rofi -show drun'}
-        }
-    )
+    }, host, {
+        'p14s': {'launcher': 'rofi -show drun'}
+    })
+
 
     # Alacritty
     alacritty = set({
-        'font_size': '10.0',
-    }, if_host={
+        'font_size': '9.0',
+    }, host, {
         'p15': {'font_size': '8.0'}
     })
 
+
     # Default font for window titles (not bar.font)
     font = set('xft:URWGothic-Book 9')
 
+
+    # Task tray
+    tasktray = set({
+        'enabled': True,
+        'position': 'right',
+    })
+
+
     # i3bar configs
     # All themes may obey these global bar configs, or they may set their own
     bar = set({
         'enabled': False,
         #'cmd': 'i3bar',
         'cmd': 'i3bar --transparency',
         'status_cmd': 'i3status',
@@ -192,80 +218,109 @@
         'mode': 'dock', # dock|hide|invisible
         'hidden_state': 'hide', # hide|show
 
         # Modifier makes the hidden bar show up while key is pressed
         'modifier': 'none',
         #'modifier': 'Ctrl+$alt',
     },
-        # FIXME, make an ifnot_desktop == i3
-        if_desktop={
-            'kde': {'mode': 'hide'}
+        desktop != 'i3', {
+            'mode': 'hide'
         },
-        if_hostname={
+        host, {
             'p15': {'position': 'top'},
             'p14s': {'enabled': True},
         },
     )
 
+
+    # Applications (not autostarts)
     # Preferred applications, could change depending on DE installed
     apps = set({
+        # These are mostly common generic all Desktop Environments and Installed Desktop Tools
         'terminal': 'alacritty',
-        'filemanager': 'dolphin',
         'webbrowser': 'firefox',
         'webbrowser2': 'chromium',
-        'calculator': 'kcalc',
-        'settings': 'systemsettings',
-        'screenshot': 'spectacle', # i3-scrot
-        'dmenu': path('~/.files/scripts/dmenu-run-blue'),
-        'screenlock': 'blurlock',
-        'powermanager': 'xfce4-power-manager',
-        'powermanagersettings': 'xfce4-power-manager-settings',
-        'xsslock': f'xss-lock -- blurlock',
-        #'xsslock': f'xss-lock -- i3lock --nofork --image {wallpaper_base}/De/deepin.jpg',
-        'networkeditor': 'nm-connection-editor',
+        'dmenu': set(path('~/.files/scripts/dmenu-run-blue'),
+            theme, {'manjaro': path('~/.files/scripts/dmenu-run-green')
+        }),
         'htop': 'htop',
         'bashtop': 'bashtop',
-        'taskmanager': 'ksysguard',
         'codeeditor': 'code',
-        'notepad': 'kate',
-        'colorpicker': 'kcolorchooser',
+        'screenlock': 'blurlock',
+        'powermanager': 'xfce4-power-manager', # move to autostart
+        'powermanagersettings': 'xfce4-power-manager-settings',
         'spotify': 'spotify',
-        'clipboard': 'clipit --daemon',
+        'networkeditor': 'nm-connection-editor',
     },
-        if_theme={
-            'manjaro': {'dmenu': path('~/.files/scripts/dmenu-run-green')}
-        },
-        if_host={
-            'p14s': {
-                'terminal': 'gnome-terminal',
-                'calculator': 'gnome-calculator',
-                'screenlock': 'i3lock',
-            },
-            'deajaro': {
-                'filemanager': 'thunar',
-                'calculator': 'xcalc',
-                'taskmanager': 'xfce4-taskmanager',
-                'settings': 'xfce4-settings-manager',
-            },
+        desktop_tools=='kde', {
+            #'terminal': 'konsole',
+            'filemanager': 'dolphin',
+            'calculator': 'kcalc',
+            'settings': 'systemsettings',
+            'taskmanager': 'ksysguard',
+            'screenshot': 'spectacle',
+            'colorpicker': 'kcolorchooser',
+            'notepad': 'kate',
+    },
+        desktop_tools=='xfce', {
+            #'terminal': 'gnome-terminal',
+            'filemanager': 'thunar',
+            'calculator': 'galculator', # xcalc
+            'settings': 'xfce4-settings-manager',
+            'taskmanager': 'xfce4-taskmanager',
+            'notepad': 'mousepad',
+    },
+        desktop_tools=='gnome', {
+            'filemanager': 'nautilus', # ???
+            'terminal': 'gnome-terminal',
+            'calculator': 'gnome-calculator',
+    })
+
+
+    # Autostarts
+    #exec --no-startup-id blueman-applet
+    #exec_always --no-startup-id sbxkb
+    #exec --no-startup-id start_conky_maia
+    #exec --no-startup-id start_conky_green
+    autostart = set({
+        # These only fire up if we are in pure i3 mode (no other desktop environment+i3)
+        'session':  set(None, desktop=='i3' and desktop_tools=='xfce', 'exec --no-startup-id xfsettingsd --replace'),
+        'locker':   set(None, desktop=='i3', 'exec_always --no-startup-id xss-lock -- blurlock'),
+        #'locker':  set(None, desktop=='i3', 'exec_always --no-startup-id xss-lock -- i3lock --nofork --image ' + wallpaper_base + '/De/deepin.jpg'),
+        'polkit':   set(None, desktop=='i3', 'exec --no-startup-id /usr/lib/polkit-kde-authentication-agent-1'),
+        'screen':   set(None, desktop=='i3', 'exec --no-startup-id ~/.screenlayout/screen-laptop.sh'),
+        'powerman': set(None, desktop=='i3', 'exec_always --no-startup-id ' + apps.powermanager),
+
+        # If using polybar in pure i3
+        'bar': set(None, desktop=='i3' and polybar.enabled, 'exec_always --no-startup-id ~/.config/polybar/launch.sh --' + polybar.theme),
+
+        # Threse always fire up, regardless of how i3 is used
+        'wallpaper': 'exec_always --no-startup-id nitrogen --restore',
+        'compositor': 'exec_always --no-startup-id picom --config ~/.config/picom/picom.conf -b',
+        'keyboard': 'exec_always --no-startup-id xset r rate 250 50',
+
+        # Theme specific alttab
+        'alttab': 'exec_always --no-startup-id "alttab -w 1 -s 1 -bw 0 -fg \'' + themes[theme].color + '\' -bg \'#0E2229\' -frame \'' + themes[theme].color + '\' -t 128x150 -i 127x64"',
+    },
+        # If tasktray is enabled running in pure i3
+        tasktray.enabled and desktop=='i3', {
+            'matray':  set(None, os=='manjaro', 'exec --no-startup-id matray'),
+            'clipman': set('exec --no-startup-id clipit --daemon'),
+            'netman':  set('exec --no-startup-id nm-applet'),
+            'volume':  set('exec --no-startup-id volumeicon'),
         },
     )
 
-    # Tray Icons
-    tray = set({
-        'volume': 'volumeicon',
-        'network': 'nm-applet',
-    })
-
     # Volume Control
     volume = set({
         'up': 'amixer -D pulse sset Master 5%+',
         'down': 'amixer -D pulse sset Master 5%-',
         'mute': 'amixer -D pulse set Master 1+ toggle',
-        # Or self.terminal + '-e alsamixer'
-        'mixer': 'pavucontrol'
+        #'mixer': apps.terminal + ' -e alsamixer',
+        'mixer': 'pavucontrol',
     })
 
     # Media Control
     media = set({
         'play_pause': 'playerctl play-pause',
         'next': 'playerctl next',
         'previous': 'playerctl previous',
@@ -273,14 +328,15 @@
 
     # Brightness Control
     brightness = set({
         'up': 'brightnessctl -q set 3%+',
         'down': 'brightnessctl --min-val=2 -q set 3%-',
     })
 
+
     # Dynamically Load and Instantiate Plugins
     # Pluging must be LAST after all variables are set
     _vars = gather(locals())
     plugins = set({
         'nitrogen': plugin('nitrogen.Nitrogen')(_vars),
         'archey3': plugin('archey3.Archey3')(_vars),
         'polybar': plugin('polybar.Polybar')(_vars),
@@ -288,26 +344,36 @@
     })
 
     # Return all variables to the ohmyi3 generator for templating
     return gather(locals())
 
 
 
+
 async def before_generate(config):
     """This hook fires before the new i3 config is generated"""
-    #dump('before hook')
+
+    # Kill some applications, as they don't re-autostart if already running
+    util.shell('killall alttab')
+
+
 
 async def after_generate(config):
     """This hook fires after the new i3 config is generated"""
     #dump('after hook')
 
+    # REVIEW all these plugins.  They are very specific
+    # For example, the polybar theme is specific to
+    # https://github.com/adi1090x/polybar-themes style themes only and
+    # is currently designed mostly for the "panels" variant.
+
     # Set themed wallpaper
-    config.plugins.nitrogen.set_wallpaper()
+    #config.plugins.nitrogen.set_wallpaper()
 
     # Set themed archey in my .zshrc and or .bashrc
-    config.plugins.archey3.set_archey()
+    #config.plugins.archey3.set_archey()
 
     # Modify polybar theme files (template some variables)
-    config.plugins.polybar.adjust_polybar()
+    #config.plugins.polybar.adjust_polybar()
 
     # Template the alacritty config
-    config.plugins.alacritty.template_config()
+    #config.plugins.alacritty.template_config()
```

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/plugins/alacritty/alacritty.py` & `ohmyi3-0.1.3/ohmyi3/stubs/plugins/alacritty/alacritty.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/plugins/archey3/archey3.py` & `ohmyi3-0.1.3/ohmyi3/stubs/plugins/archey3/archey3.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/plugins/nitrogen/nitrogen.py` & `ohmyi3-0.1.3/ohmyi3/stubs/plugins/nitrogen/nitrogen.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/plugins/polybar/polybar.py` & `ohmyi3-0.1.3/ohmyi3/stubs/plugins/polybar/polybar.py`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/background.jpg` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/amber/theme.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/amber/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/background.jpg` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/archlinux/theme.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/archlinux/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/i3status.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/i3status.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/background.jpg` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/manjaro/theme.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/manjaro/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/background.jpg` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/background.jpg`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/ohmyi3/stubs/themes/pink/theme.conf` & `ohmyi3-0.1.3/ohmyi3/stubs/themes/pink/theme.conf`

 * *Files identical despite different names*

### Comparing `ohmyi3-0.1.2/pyproject.toml` & `ohmyi3-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ohmyi3"
-version = "0.1.2"
+version = "0.1.3"
 license = "MIT"
 authors = ["Matthew Reschke <mail@mreschke.com>"]
 description = "Dynamic i3 Configuration Manager "
 homepage = "https://github.com/ohmyi3/ohmyi3"
 documentation = "https://github.com/ohmyi3/ohmyi3"
 repository = "https://github.com/ohmyi3/ohmyi3"
 readme = "README.md"
```

