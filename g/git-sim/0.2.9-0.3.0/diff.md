# Comparing `tmp/git-sim-0.2.9.tar.gz` & `tmp/git-sim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-sim-0.2.9.tar", last modified: Sat Apr  1 03:58:10 2023, max compression
+gzip compressed data, was "git-sim-0.3.0.tar", last modified: Sat Apr 22 16:23:30 2023, max compression
```

## Comparing `git-sim-0.2.9.tar` & `git-sim-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 03:58:10.912400 git-sim-0.2.9/
--rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.2.9/LICENSE
--rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0    23011 2023-04-01 03:58:10.911399 git-sim-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    22204 2023-04-01 00:31:43.000000 git-sim-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 03:58:10.909399 git-sim-0.2.9/git_sim/
--rw-rw-rw-   0        0        0        0 2023-03-09 07:57:17.000000 git-sim-0.2.9/git_sim/__init__.py
--rw-rw-rw-   0        0        0     7653 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/__main__.py
--rw-rw-rw-   0        0        0     2852 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/add.py
--rw-rw-rw-   0        0        0     3631 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/animations.py
--rw-rw-rw-   0        0        0     1511 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/branch.py
--rw-rw-rw-   0        0        0     4415 2023-04-01 03:56:33.000000 git-sim-0.2.9/git_sim/checkout.py
--rw-rw-rw-   0        0        0     2302 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/cherrypick.py
--rw-rw-rw-   0        0        0     2974 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/clone.py
--rw-rw-rw-   0        0        0     7728 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/commands.py
--rw-rw-rw-   0        0        0     3175 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/commit.py
--rw-rw-rw-   0        0        0      224 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/enums.py
--rw-rw-rw-   0        0        0     2842 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/fetch.py
--rw-rw-rw-   0        0        0    44480 2023-04-01 03:52:38.000000 git-sim-0.2.9/git_sim/git_sim_base_command.py
--rw-rw-rw-   0        0        0     1415 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/log.py
--rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.2.9/git_sim/logo.png
--rw-rw-rw-   0        0        0     6940 2023-04-01 03:52:38.000000 git-sim-0.2.9/git_sim/merge.py
--rw-rw-rw-   0        0        0     3844 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/pull.py
--rw-rw-rw-   0        0        0     7164 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/push.py
--rw-rw-rw-   0        0        0     5755 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/rebase.py
--rw-rw-rw-   0        0        0     5042 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/reset.py
--rw-rw-rw-   0        0        0     2467 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/restore.py
--rw-rw-rw-   0        0        0     5305 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/revert.py
--rw-rw-rw-   0        0        0     1389 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/settings.py
--rw-rw-rw-   0        0        0     6505 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/stash.py
--rw-rw-rw-   0        0        0      829 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/status.py
--rw-rw-rw-   0        0        0     4413 2023-04-01 03:56:33.000000 git-sim-0.2.9/git_sim/switch.py
--rw-rw-rw-   0        0        0     1469 2023-04-01 00:31:43.000000 git-sim-0.2.9/git_sim/tag.py
-drwxrwxrwx   0        0        0        0 2023-04-01 03:58:10.911399 git-sim-0.2.9/git_sim.egg-info/
--rw-rw-rw-   0        0        0    23011 2023-04-01 03:58:10.000000 git-sim-0.2.9/git_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-04-01 03:58:10.000000 git-sim-0.2.9/git_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 03:58:10.000000 git-sim-0.2.9/git_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-01 03:58:10.000000 git-sim-0.2.9/git_sim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-04-01 03:58:10.000000 git-sim-0.2.9/git_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 03:58:10.000000 git-sim-0.2.9/git_sim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 03:58:10.912400 git-sim-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1429 2023-04-01 03:56:51.000000 git-sim-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:30.907142 git-sim-0.3.0/
+-rw-rw-rw-   0        0        0    18431 2023-03-09 07:57:29.000000 git-sim-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-03-09 07:57:17.000000 git-sim-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    25467 2023-04-22 16:23:30.907142 git-sim-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    24660 2023-04-21 21:10:02.000000 git-sim-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:30.894185 git-sim-0.3.0/git_sim/
+-rw-rw-rw-   0        0        0       23 2023-04-22 16:22:56.000000 git-sim-0.3.0/git_sim/__init__.py
+-rw-rw-rw-   0        0        0     8333 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/__main__.py
+-rw-rw-rw-   0        0        0     2852 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/add.py
+-rw-rw-rw-   0        0        0     3680 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/animations.py
+-rw-rw-rw-   0        0        0     1511 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/branch.py
+-rw-rw-rw-   0        0        0     4415 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/checkout.py
+-rw-rw-rw-   0        0        0     2302 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/cherrypick.py
+-rw-rw-rw-   0        0        0     3921 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/clean.py
+-rw-rw-rw-   0        0        0     2974 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/clone.py
+-rw-rw-rw-   0        0        0     8586 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/commands.py
+-rw-rw-rw-   0        0        0     3175 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/commit.py
+-rw-rw-rw-   0        0        0      572 2023-04-21 21:10:02.000000 git-sim-0.3.0/git_sim/enums.py
+-rw-rw-rw-   0        0        0     2842 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/fetch.py
+-rw-rw-rw-   0        0        0    46789 2023-04-21 21:10:02.000000 git-sim-0.3.0/git_sim/git_sim_base_command.py
+-rw-rw-rw-   0        0        0     1415 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/log.py
+-rw-rw-rw-   0        0        0    63319 2023-03-09 07:57:17.000000 git-sim-0.3.0/git_sim/logo.png
+-rw-rw-rw-   0        0        0     7251 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/merge.py
+-rw-rw-rw-   0        0        0     2937 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/mv.py
+-rw-rw-rw-   0        0        0     3844 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/pull.py
+-rw-rw-rw-   0        0        0     7226 2023-04-21 21:10:02.000000 git-sim-0.3.0/git_sim/push.py
+-rw-rw-rw-   0        0        0     6057 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/rebase.py
+-rw-rw-rw-   0        0        0     5042 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/reset.py
+-rw-rw-rw-   0        0        0     2467 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/restore.py
+-rw-rw-rw-   0        0        0     5607 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/revert.py
+-rw-rw-rw-   0        0        0     4541 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/rm.py
+-rw-rw-rw-   0        0        0     1380 2023-04-21 20:23:21.000000 git-sim-0.3.0/git_sim/settings.py
+-rw-rw-rw-   0        0        0     6505 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/stash.py
+-rw-rw-rw-   0        0        0      829 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/status.py
+-rw-rw-rw-   0        0        0     4413 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/switch.py
+-rw-rw-rw-   0        0        0     1469 2023-04-21 20:10:26.000000 git-sim-0.3.0/git_sim/tag.py
+drwxrwxrwx   0        0        0        0 2023-04-22 16:23:30.906145 git-sim-0.3.0/git_sim.egg-info/
+-rw-rw-rw-   0        0        0    25467 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 16:23:30.000000 git-sim-0.3.0/git_sim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 16:23:30.907142 git-sim-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2023-04-21 20:23:21.000000 git-sim-0.3.0/setup.py
```

### Comparing `git-sim-0.2.9/LICENSE` & `git-sim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/PKG-INFO` & `git-sim-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.2.9
+Version: 0.3.0
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # git-sim
+![git-sim-logo-with-tagline-1440x376p45](https://user-images.githubusercontent.com/49353917/232990611-58d0693f-69c0-45c8-b51d-cd540793d18c.gif)
+
 [![GitHub license](https://img.shields.io/github/license/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/blob/main/LICENSE)
 [![GitHub tag](https://img.shields.io/github/v/release/initialcommit-com/git-sim)](https://img.shields.io/github/v/release/initialcommit-com/git-sim)
 [![Downloads](https://static.pepy.tech/badge/git-sim)](https://pepy.tech/project/git-sim)
 [![Contributors](https://img.shields.io/github/contributors/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/graphs/contributors)
 [![Share](https://img.shields.io/twitter/url?label=Share&url=https%3A%2F%2Ftwitter.com%2Finitcommit)](https://twitter.com/intent/tweet?text=Check%20out%20%23gitsim%20%2D%20a%20tool%20to%20visualize%20%23Git%20operations%20in%20your%20local%20repos%20with%20a%20single%20terminal%20command,%20by%20%40initcommit!%20https%3A%2F%2Fgithub%2Ecom%2Finitialcommit%2Dcom%2Fgit%2Dsim)
 
 Visually simulate Git operations in your own repos with a single terminal command.
@@ -31,23 +33,23 @@
 Example: `$ git-sim merge <branch>`
 
 ![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210939840-1d51493a-6cac-43fd-9d12-3d2948d32c61.jpg)
 
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
-- Share visualizations (jpg image or mp4 video) of your Git commands with your team, or the world
+- Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
-- Create static Git diagrams (jpg) or dynamic animated videos (mp4) to speed up content creation
+- Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
-- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`
+- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
 - Color commits by parameter, such as author the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
@@ -139,15 +141,15 @@
 
 ## Requirements
 * Python 3.7 or greater
 * Pip (Package manager for Python)
 * [Manim (Community version)](https://www.manim.community/)
 
 ## Commands
-Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", along with corresponding options.
+Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", "rm", "mv", "clean" along with corresponding options.
 
 ```console
 $ git-sim [global options] <subcommand> [subcommand options]
 ```
 
 The `[global options]` apply to the overarching `git-sim` simulation itself, including:
 
@@ -161,15 +163,16 @@
 `-d`: Disable the automatic opening of the image/video file after generation. Useful to avoid errors in console mode with no GUI.  
 `--light-mode`: Use a light mode color scheme instead of default dark mode.  
 `--reverse, -r`: Display commit history in the reverse direction.  
 `--img-format`: Output format for the image file, i.e. `jpg` or `png`. Default output format is `jpg`.  
 `--stdout`: Write raw image data to stdout while suppressing all other program output.  
 `--output-only-path`: Only output the path to the generated media file to stdout. Useful for other programs to ingest.  
 `--quiet, -q`: Suppress all output except errors.  
-`--highlight-commit-messages`: Make commit message text bigger and bold, and hide commit ids.
+`--highlight-commit-messages`: Make commit message text bigger and bold, and hide commit ids.  
+`--style`: Graphical style of the output image or animated video, i.e. `clean` (default) or `thick`.
 
 Animation-only global options (to be used in conjunction with `--animate`):
 
 `--video-format`: Output format for the video file, i.e. `mp4` or `webm`. Default output format is `mp4`.  
 `--speed=n`: Set the multiple of animation speed of the output simulation, `n` can be an integer or float, default is 1.5.  
 `--low-quality`: Render the animation in low quality to speed up creation time, recommended for non-presentation use.  
 `--show-intro`: Add an intro sequence with custom logo and title.  
@@ -302,45 +305,85 @@
 
 ### git switch
 Usage: `git-sim switch [-c] <branch>`
 
 - Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
 - The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
 
+![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
+
 ### git checkout
 Usage: `git-sim checkout [-b] <branch>`
 
 - Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
 - The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
 
+![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
+
 ### git fetch
 Usage: `git-sim fetch <remote> <branch>`
 
 - Fetches the specified `<branch>` from the specified `<remote>` to the local repo
 
+![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
+
 ### git pull
 Usage: `git-sim pull [<remote> <branch>]`
 
 - Pulls the specified `<branch>` from the specified `<remote>` to the local repo
 - If `<remote>` and `<branch>` are not specified, the active branch is pulled from the default remote
 - If merge conflicts occur, they are displayed in a table
 
+![git-sim-pull_04-09-23_21-50-15](https://user-images.githubusercontent.com/49353917/230828298-455c0a9d-cf94-499e-9e35-623e7b218772.jpg)
+
 ### git push
 Usage: `git-sim push [<remote> <branch>]`
 
 - Pushes the specified `<branch>` to the specified `<remote>` and displays the local result
 - If `<remote>` and `<branch>` are not specified, the active branch is pushed to the default remote
 - If the push fails due to remote changes that don't exist in the local repo, a message is included telling the user to pull first, along with color coding which commits need to be pulled
 
+![git-sim-push_04-21-23_13-41-57](https://user-images.githubusercontent.com/49353917/233731005-51fd7887-ae14-4ceb-a5d5-e5aed79e9fd8.jpg)
+
 ### git clone
 Usage: `git-sim clone <url>`
 
 - Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
 - Output will report if clone operation is successful and show log of local clone
 
+![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
+
+### git rm
+Usage: `git-sim rm <file 1> <file 2> ... <file n>`
+
+- Specify one or more `<file>` as a *tracked* file
+- Simulated output will show files being removed from Git tracking
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-rm_04-09-23_22-01-29](https://user-images.githubusercontent.com/49353917/230829899-f5d688ea-bc8e-46f9-a54a-55d251c8915d.jpg)
+
+### git mv
+Usage: `git-sim mv <file> <new file>`
+
+- Specify `<file>` as file to update name/path
+- Specify `<new file>` as new name/path of file 
+- Simulated output will show the name/path of the file being updated 
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
+
+### git clean
+Usage: `git-sim clean`
+
+- Simulated output will show untracked files being deleted
+- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+
 ## Video animation examples
 ```console
 $ git-sim --animate reset HEAD^
 ```
 
 https://user-images.githubusercontent.com/49353917/210943230-f38d879b-bb0d-4d42-a196-f24efb9e351a.mp4
```

### Comparing `git-sim-0.2.9/README.md` & `git-sim-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # git-sim
+![git-sim-logo-with-tagline-1440x376p45](https://user-images.githubusercontent.com/49353917/232990611-58d0693f-69c0-45c8-b51d-cd540793d18c.gif)
+
 [![GitHub license](https://img.shields.io/github/license/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/blob/main/LICENSE)
 [![GitHub tag](https://img.shields.io/github/v/release/initialcommit-com/git-sim)](https://img.shields.io/github/v/release/initialcommit-com/git-sim)
 [![Downloads](https://static.pepy.tech/badge/git-sim)](https://pepy.tech/project/git-sim)
 [![Contributors](https://img.shields.io/github/contributors/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/graphs/contributors)
 [![Share](https://img.shields.io/twitter/url?label=Share&url=https%3A%2F%2Ftwitter.com%2Finitcommit)](https://twitter.com/intent/tweet?text=Check%20out%20%23gitsim%20%2D%20a%20tool%20to%20visualize%20%23Git%20operations%20in%20your%20local%20repos%20with%20a%20single%20terminal%20command,%20by%20%40initcommit!%20https%3A%2F%2Fgithub%2Ecom%2Finitialcommit%2Dcom%2Fgit%2Dsim)
 
 Visually simulate Git operations in your own repos with a single terminal command.
@@ -14,23 +16,23 @@
 Example: `$ git-sim merge <branch>`
 
 ![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210939840-1d51493a-6cac-43fd-9d12-3d2948d32c61.jpg)
 
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
-- Share visualizations (jpg image or mp4 video) of your Git commands with your team, or the world
+- Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
-- Create static Git diagrams (jpg) or dynamic animated videos (mp4) to speed up content creation
+- Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
-- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`
+- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
 - Color commits by parameter, such as author the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
@@ -122,15 +124,15 @@
 
 ## Requirements
 * Python 3.7 or greater
 * Pip (Package manager for Python)
 * [Manim (Community version)](https://www.manim.community/)
 
 ## Commands
-Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", along with corresponding options.
+Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", "rm", "mv", "clean" along with corresponding options.
 
 ```console
 $ git-sim [global options] <subcommand> [subcommand options]
 ```
 
 The `[global options]` apply to the overarching `git-sim` simulation itself, including:
 
@@ -144,15 +146,16 @@
 `-d`: Disable the automatic opening of the image/video file after generation. Useful to avoid errors in console mode with no GUI.  
 `--light-mode`: Use a light mode color scheme instead of default dark mode.  
 `--reverse, -r`: Display commit history in the reverse direction.  
 `--img-format`: Output format for the image file, i.e. `jpg` or `png`. Default output format is `jpg`.  
 `--stdout`: Write raw image data to stdout while suppressing all other program output.  
 `--output-only-path`: Only output the path to the generated media file to stdout. Useful for other programs to ingest.  
 `--quiet, -q`: Suppress all output except errors.  
-`--highlight-commit-messages`: Make commit message text bigger and bold, and hide commit ids.
+`--highlight-commit-messages`: Make commit message text bigger and bold, and hide commit ids.  
+`--style`: Graphical style of the output image or animated video, i.e. `clean` (default) or `thick`.
 
 Animation-only global options (to be used in conjunction with `--animate`):
 
 `--video-format`: Output format for the video file, i.e. `mp4` or `webm`. Default output format is `mp4`.  
 `--speed=n`: Set the multiple of animation speed of the output simulation, `n` can be an integer or float, default is 1.5.  
 `--low-quality`: Render the animation in low quality to speed up creation time, recommended for non-presentation use.  
 `--show-intro`: Add an intro sequence with custom logo and title.  
@@ -285,45 +288,85 @@
 
 ### git switch
 Usage: `git-sim switch [-c] <branch>`
 
 - Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
 - The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
 
+![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
+
 ### git checkout
 Usage: `git-sim checkout [-b] <branch>`
 
 - Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
 - The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
 
+![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
+
 ### git fetch
 Usage: `git-sim fetch <remote> <branch>`
 
 - Fetches the specified `<branch>` from the specified `<remote>` to the local repo
 
+![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
+
 ### git pull
 Usage: `git-sim pull [<remote> <branch>]`
 
 - Pulls the specified `<branch>` from the specified `<remote>` to the local repo
 - If `<remote>` and `<branch>` are not specified, the active branch is pulled from the default remote
 - If merge conflicts occur, they are displayed in a table
 
+![git-sim-pull_04-09-23_21-50-15](https://user-images.githubusercontent.com/49353917/230828298-455c0a9d-cf94-499e-9e35-623e7b218772.jpg)
+
 ### git push
 Usage: `git-sim push [<remote> <branch>]`
 
 - Pushes the specified `<branch>` to the specified `<remote>` and displays the local result
 - If `<remote>` and `<branch>` are not specified, the active branch is pushed to the default remote
 - If the push fails due to remote changes that don't exist in the local repo, a message is included telling the user to pull first, along with color coding which commits need to be pulled
 
+![git-sim-push_04-21-23_13-41-57](https://user-images.githubusercontent.com/49353917/233731005-51fd7887-ae14-4ceb-a5d5-e5aed79e9fd8.jpg)
+
 ### git clone
 Usage: `git-sim clone <url>`
 
 - Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
 - Output will report if clone operation is successful and show log of local clone
 
+![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
+
+### git rm
+Usage: `git-sim rm <file 1> <file 2> ... <file n>`
+
+- Specify one or more `<file>` as a *tracked* file
+- Simulated output will show files being removed from Git tracking
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-rm_04-09-23_22-01-29](https://user-images.githubusercontent.com/49353917/230829899-f5d688ea-bc8e-46f9-a54a-55d251c8915d.jpg)
+
+### git mv
+Usage: `git-sim mv <file> <new file>`
+
+- Specify `<file>` as file to update name/path
+- Specify `<new file>` as new name/path of file 
+- Simulated output will show the name/path of the file being updated 
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
+
+### git clean
+Usage: `git-sim clean`
+
+- Simulated output will show untracked files being deleted
+- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+
 ## Video animation examples
 ```console
 $ git-sim --animate reset HEAD^
 ```
 
 https://user-images.githubusercontent.com/49353917/210943230-f38d879b-bb0d-4d42-a196-f24efb9e351a.mp4
```

### Comparing `git-sim-0.2.9/git_sim/__main__.py` & `git-sim-0.3.0/git_sim/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-import pathlib
-import typer
+import datetime
 import os
+import pathlib
 import sys
-import datetime
 import time
 
-import git_sim.commands
+import typer
 
-from git_sim.settings import ImgFormat, VideoFormat, settings
+import git_sim.commands
+from git_sim.settings import (
+    ColorByOptions,
+    StyleOptions,
+    ImgFormat,
+    VideoFormat,
+    settings,
+)
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
 
+def version_callback(value: bool) -> None:
+    if value:
+        print(f"git-sim version {git_sim.__version__}")
+        raise typer.Exit()
+
+
 @app.callback(no_args_is_help=True)
 def main(
     ctx: typer.Context,
     animate: bool = typer.Option(
         settings.animate,
         help="Animate the simulation and output as an mp4 video",
     ),
@@ -122,25 +134,36 @@
         settings.hide_merged_branches,
         help="Hide commits from merged branches, i.e. only display mainline commits",
     ),
     all: bool = typer.Option(
         settings.all,
         help="Display all local branches in the log output",
     ),
-    color_by: str = typer.Option(
+    color_by: ColorByOptions = typer.Option(
         settings.color_by,
-        help="Color commits by parameter, such as author",
+        help="Color commits by parameter",
     ),
     highlight_commit_messages: bool = typer.Option(
         settings.highlight_commit_messages,
         help="Make the displayed commit messages more prominent",
     ),
+    version: bool = typer.Option(
+        False,
+        "--version",
+        "-v",
+        help="Show the version of git-sim and exit",
+        callback=version_callback,
+    ),
+    style: StyleOptions = typer.Option(
+        settings.style.value,
+        help="Graphical style of the output image or animated video",
+    ),
 ):
     import git
-    from manim import config, WHITE
+    from manim import WHITE, config
 
     settings.animate = animate
     settings.n = n
     settings.auto_open = auto_open
     settings.img_format = img_format
     settings.light_mode = light_mode
     settings.transparent_bg = transparent_bg
@@ -161,14 +184,15 @@
     settings.output_only_path = output_only_path
     settings.quiet = quiet
     settings.invert_branches = invert_branches
     settings.hide_merged_branches = hide_merged_branches
     settings.all = all
     settings.color_by = color_by
     settings.highlight_commit_messages = highlight_commit_messages
+    settings.style = style
 
     try:
         if sys.platform == "linux" or sys.platform == "darwin":
             repo_name = git.repo.Repo(
                 search_parent_directories=True
             ).working_tree_dir.split("/")[-1]
         elif sys.platform == "win32":
@@ -186,35 +210,38 @@
     if settings.low_quality:
         config.quality = "low_quality"
 
     if settings.light_mode:
         config.background_color = WHITE
 
     if settings.transparent_bg:
-        settings.img_format = ImgFormat.png
+        settings.img_format = ImgFormat.PNG
 
     t = datetime.datetime.fromtimestamp(time.time()).strftime("%m-%d-%y_%H-%M-%S")
     config.output_file = "git-sim-" + ctx.invoked_subcommand + "_" + t + ".mp4"
 
 
 app.command()(git_sim.commands.add)
 app.command()(git_sim.commands.branch)
 app.command()(git_sim.commands.checkout)
 app.command()(git_sim.commands.cherry_pick)
+app.command()(git_sim.commands.clean)
 app.command()(git_sim.commands.clone)
 app.command()(git_sim.commands.commit)
 app.command()(git_sim.commands.fetch)
 app.command()(git_sim.commands.log)
 app.command()(git_sim.commands.merge)
+app.command()(git_sim.commands.mv)
 app.command()(git_sim.commands.pull)
 app.command()(git_sim.commands.push)
 app.command()(git_sim.commands.rebase)
 app.command()(git_sim.commands.reset)
 app.command()(git_sim.commands.restore)
 app.command()(git_sim.commands.revert)
+app.command()(git_sim.commands.rm)
 app.command()(git_sim.commands.stash)
 app.command()(git_sim.commands.status)
 app.command()(git_sim.commands.switch)
 app.command()(git_sim.commands.tag)
 
 
 if __name__ == "__main__":
```

### Comparing `git-sim-0.2.9/git_sim/add.py` & `git-sim-0.3.0/git_sim/add.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/animations.py` & `git-sim-0.3.0/git_sim/animations.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 
 import cv2
 import git.repo
 from manim import WHITE, Scene
 from manim.utils.file_ops import open_file
 
 from git_sim.settings import settings
+from git_sim.enums import VideoFormat
 
 
 def handle_animations(scene: Scene) -> None:
     scene.render()
 
-    if settings.video_format == "webm":
+    if settings.video_format == VideoFormat.WEBM:
         webm_file_path = str(scene.renderer.file_writer.movie_file_path)[:-3] + "webm"
         cmd = f"ffmpeg -y -i {scene.renderer.file_writer.movie_file_path} -hide_banner -loglevel error -c:v libvpx-vp9 -crf 50 -b:v 0 -b:a 128k -c:a libopus {webm_file_path}"
         print("Converting video output to .webm format...")
         # Start ffmpeg conversion
         p = subprocess.Popen(cmd, shell=True)
         p.wait()
         # if the conversion is successful, delete the .mp4
```

### Comparing `git-sim-0.2.9/git_sim/branch.py` & `git-sim-0.3.0/git_sim/branch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/checkout.py` & `git-sim-0.3.0/git_sim/checkout.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/cherrypick.py` & `git-sim-0.3.0/git_sim/cherrypick.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/clone.py` & `git-sim-0.3.0/git_sim/clone.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/commands.py` & `git-sim-0.3.0/git_sim/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,22 @@
 ):
     from git_sim.cherrypick import CherryPick
 
     scene = CherryPick(commit=commit, edit=edit)
     handle_animations(scene=scene)
 
 
+def clean():
+    from git_sim.clean import Clean
+
+    settings.hide_first_tag = True
+    scene = Clean()
+    handle_animations(scene=scene)
+
+
 def clone(
     url: str = typer.Argument(
         ...,
         help="The web URL or filesystem path of the Git repo to clone",
     ),
 ):
     from git_sim.clone import Clone
@@ -162,14 +170,31 @@
 ):
     from git_sim.merge import Merge
 
     scene = Merge(branch=branch, no_ff=no_ff, message=message)
     handle_animations(scene=scene)
 
 
+def mv(
+    file: str = typer.Argument(
+        default=None,
+        help="The name of the file to change the name/path of",
+    ),
+    new_file: str = typer.Argument(
+        default=None,
+        help="The new name/path of the file",
+    ),
+):
+    from git_sim.mv import Mv
+
+    settings.hide_first_tag = True
+    scene = Mv(file=file, new_file=new_file)
+    handle_animations(scene=scene)
+
+
 def pull(
     remote: str = typer.Argument(
         default=None,
         help="The name of the remote to pull from",
     ),
     branch: str = typer.Argument(
         default=None,
@@ -261,14 +286,27 @@
     from git_sim.revert import Revert
 
     settings.hide_first_tag = True
     scene = Revert(commit=commit)
     handle_animations(scene=scene)
 
 
+def rm(
+    files: List[str] = typer.Argument(
+        default=None,
+        help="The names of one or more files to remove from Git's index",
+    )
+):
+    from git_sim.rm import Rm
+
+    settings.hide_first_tag = True
+    scene = Rm(files=files)
+    handle_animations(scene=scene)
+
+
 def stash(
     command: StashSubCommand = typer.Argument(
         default=None,
         help="Stash subcommand (push, pop, apply)",
     ),
     files: List[str] = typer.Argument(
         default=None,
```

### Comparing `git-sim-0.2.9/git_sim/commit.py` & `git-sim-0.3.0/git_sim/commit.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/fetch.py` & `git-sim-0.3.0/git_sim/fetch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/git_sim_base_command.py` & `git-sim-0.3.0/git_sim/git_sim_base_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import platform
-import sys
 import os
-import tempfile
+import platform
 import shutil
 import stat
+import sys
+import tempfile
 
 import git
 import manim as m
 import numpy
 from git.exc import GitCommandError, InvalidGitRepositoryError
 from git.repo import Repo
 
+from git_sim.enums import ColorByOptions, StyleOptions
 from git_sim.settings import settings
 
 
 class GitSimBaseCommand(m.MovingCameraScene):
     def __init__(self):
         super().__init__()
         self.init_repo()
@@ -57,14 +58,25 @@
 
         self.fill_opacity = 0.25
         self.ref_fill_opacity = 0.25
         if settings.transparent_bg:
             self.fill_opacity = 0.5
             self.ref_fill_opacity = 1.0
 
+        if settings.style == StyleOptions.CLEAN:
+            self.commit_stroke_width = 5
+            self.arrow_stroke_width = 5
+            self.arrow_tip_shape = m.ArrowTriangleFilledTip
+            self.font_weight = m.NORMAL
+        elif settings.style == StyleOptions.THICK:
+            self.commit_stroke_width = 30
+            self.arrow_stroke_width = 10
+            self.arrow_tip_shape = m.StealthTip
+            self.font_weight = m.BOLD
+
     def init_repo(self):
         try:
             self.repo = Repo(search_parent_directories=True)
             repo_name = os.path.basename(self.repo.working_dir)
             new_dir = os.path.join(tempfile.gettempdir(), "git_sim", repo_name)
             new_dir2 = os.path.join(tempfile.gettempdir(), "git_sim", repo_name + "2")
             try:
@@ -238,14 +250,15 @@
         elif len(commit.parents) <= 1:
             commit_fill = m.RED
         else:
             commit_fill = m.GRAY
 
         circle = m.Circle(
             stroke_color=commit_fill,
+            stroke_width=self.commit_stroke_width,
             fill_color=commit_fill,
             fill_opacity=self.fill_opacity,
         )
         circle.height = 1
 
         if shift.any():
             circle.shift(shift)
@@ -275,15 +288,22 @@
             start = (
                 prevCircle.get_center()
                 if prevCircle
                 else (m.LEFT if settings.reverse else m.RIGHT)
             )
             end = self.drawnCommits[commit.hexsha].get_center()
 
-        arrow = m.Arrow(start, end, color=self.fontColor)
+        arrow = m.Arrow(
+            start,
+            end,
+            color=self.fontColor,
+            stroke_width=self.arrow_stroke_width,
+            tip_shape=self.arrow_tip_shape,
+            max_stroke_width_to_length_ratio=1000,
+        )
 
         if commit == "dark":
             arrow = m.Arrow(
                 start, end, color=m.WHITE if settings.light_mode else m.BLACK
             )
 
         length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
@@ -294,15 +314,21 @@
             .move_to(arrow.get_center())
             .rotate(angle)
         )
 
         for commitCircle in self.drawnCommits.values():
             inter = m.Intersection(lineRect, commitCircle)
             if inter.has_points():
-                arrow = m.CurvedArrow(start, end, color=self.fontColor)
+                arrow = m.CurvedArrow(
+                    start,
+                    end,
+                    color=self.fontColor,
+                    stroke_width=self.arrow_stroke_width,
+                    tip_shape=self.arrow_tip_shape,
+                )
                 if start[1] == end[1]:
                     arrow.shift(m.UP * 1.25)
                 if start[0] < end[0] and start[1] == end[1]:
                     arrow.flip(m.RIGHT).shift(m.UP)
 
         commitId, commitMessage, commit, hide_refs = self.build_commit_id_and_message(
             commit, i
@@ -315,15 +341,18 @@
         message = m.Text(
             "\n".join(
                 commitMessage[j : j + 20] for j in range(0, len(commitMessage), 20)
             )[:100],
             font="Monospace",
             font_size=20 if settings.highlight_commit_messages else 14,
             color=self.fontColor,
-            weight=m.BOLD if settings.highlight_commit_messages else m.NORMAL,
+            weight=m.BOLD
+            if settings.highlight_commit_messages
+            or settings.style == StyleOptions.THICK
+            else m.NORMAL,
         ).next_to(circle, m.DOWN)
 
         if settings.animate and commit != "dark" and isNewCommit:
             self.play(
                 self.camera.frame.animate.move_to(circle.get_center()),
                 m.Create(circle),
                 m.Text("")
@@ -368,22 +397,29 @@
                     if self.repo.is_ancestor(b1.commit, b2.commit):
                         exclude.append(b1.name)
         return [b for b in branches if b.name not in exclude]
 
     def build_commit_id_and_message(self, commit, i):
         hide_refs = False
         if commit == "dark":
-            commitId = m.Text("", font="Monospace", font_size=20, color=self.fontColor)
+            commitId = m.Text(
+                "",
+                font="Monospace",
+                font_size=20,
+                color=self.fontColor,
+                weight=self.font_weight,
+            )
             commitMessage = ""
         else:
             commitId = m.Text(
                 commit.hexsha[0:6],
                 font="Monospace",
                 font_size=20,
                 color=self.fontColor,
+                weight=self.font_weight,
             )
             commitMessage = commit.message.split("\n")[0][:40].replace("\n", " ")
         return commitId, commitMessage, commit, hide_refs
 
     def draw_head(self, commit, i, commitId):
         if commit.hexsha == self.repo.head.commit.hexsha:
             headbox = m.Rectangle(
@@ -392,15 +428,19 @@
             headbox.width = 1
             headbox.height = 0.4
             if settings.highlight_commit_messages:
                 headbox.next_to(self.drawnCommits[commit.hexsha], m.UP)
             else:
                 headbox.next_to(commitId, m.UP)
             headText = m.Text(
-                "HEAD", font="Monospace", font_size=20, color=self.fontColor
+                "HEAD",
+                font="Monospace",
+                font_size=20,
+                color=self.fontColor,
+                weight=self.font_weight,
             ).move_to(headbox.get_center())
 
             head = m.VGroup(headbox, headText)
 
             if settings.animate:
                 self.play(m.Create(head), run_time=1 / settings.speed)
             else:
@@ -439,15 +479,19 @@
                         make_branches_remote
                         and not self.is_remote_tracking_branch(branch)
                     )
                     else branch
                 )
 
                 branchText = m.Text(
-                    text, font="Monospace", font_size=20, color=self.fontColor
+                    text,
+                    font="Monospace",
+                    font_size=20,
+                    color=self.fontColor,
+                    weight=self.font_weight,
                 )
                 branchRec = m.Rectangle(
                     color=m.GREEN,
                     fill_color=m.GREEN,
                     fill_opacity=self.ref_fill_opacity,
                     height=0.4,
                     width=branchText.width + 0.25,
@@ -485,14 +529,15 @@
             try:
                 if commit.hexsha == tag.commit.hexsha:
                     tagText = m.Text(
                         tag.name,
                         font="Monospace",
                         font_size=20,
                         color=self.fontColor,
+                        weight=self.font_weight,
                     )
                     tagRec = m.Rectangle(
                         color=m.YELLOW,
                         fill_color=m.YELLOW,
                         fill_opacity=self.ref_fill_opacity,
                         height=0.4,
                         width=tagText.width + 0.25,
@@ -648,34 +693,37 @@
 
         firstColumnTitle = (
             m.Text(
                 first_column_name,
                 font="Monospace",
                 font_size=28,
                 color=self.fontColor,
+                weight=m.BOLD,
             )
             .move_to((vert1.get_center()[0] - 4, 0, 0))
             .shift(m.UP * self.zone_title_offset)
         )
         secondColumnTitle = (
             m.Text(
                 second_column_name,
                 font="Monospace",
                 font_size=28,
                 color=self.fontColor,
+                weight=m.BOLD,
             )
             .move_to(self.camera.frame.get_center())
             .align_to(firstColumnTitle, m.UP)
         )
         thirdColumnTitle = (
             m.Text(
                 third_column_name,
                 font="Monospace",
                 font_size=28,
                 color=self.fontColor,
+                weight=m.BOLD,
             )
             .move_to((vert2.get_center()[0] + 4, 0, 0))
             .align_to(firstColumnTitle, m.UP)
         )
 
         self.toFadeOut.add(
             horizontal,
@@ -837,14 +885,18 @@
                 self.play(m.Create(thirdColumnArrowMap[filename]))
             else:
                 self.add(thirdColumnArrowMap[filename])
             self.toFadeOut.add(thirdColumnArrowMap[filename])
 
         self.toFadeOut.add(firstColumnFiles, secondColumnFiles, thirdColumnFiles)
 
+        self.firstColumnFiles = firstColumnFiles
+        self.secondColumnFiles = secondColumnFiles
+        self.thirdColumnFiles = thirdColumnFiles
+
     def populate_zones(
         self,
         firstColumnFileNames,
         secondColumnFileNames,
         thirdColumnFileNames,
         firstColumnArrowMap={},
         secondColumnArrowMap={},
@@ -976,43 +1028,58 @@
         child,
         commitMessage="New commit",
         shift=numpy.array([0.0, 0.0, 0.0]),
         draw_arrow=True,
         color=m.RED,
     ):
         circle = m.Circle(
-            stroke_color=color, fill_color=color, fill_opacity=self.ref_fill_opacity
+            stroke_color=color,
+            stroke_width=self.commit_stroke_width,
+            fill_color=color,
+            fill_opacity=self.ref_fill_opacity,
         )
         circle.height = 1
         circle.next_to(
             self.drawnCommits[child.hexsha],
             m.LEFT if settings.reverse else m.RIGHT,
             buff=1.5,
         )
         circle.shift(shift)
 
         start = circle.get_center()
         end = self.drawnCommits[child.hexsha].get_center()
-        arrow = m.Arrow(start, end, color=self.fontColor)
+        arrow = m.Arrow(
+            start,
+            end,
+            color=self.fontColor,
+            stroke_width=self.arrow_stroke_width,
+            tip_shape=self.arrow_tip_shape,
+            max_stroke_width_to_length_ratio=1000,
+        )
         length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
         arrow.set_length(length)
 
         commitId = m.Text(
-            "abcdef", font="Monospace", font_size=20, color=self.fontColor
+            "abcdef",
+            font="Monospace",
+            font_size=20,
+            color=self.fontColor,
+            weight=self.font_weight,
         ).next_to(circle, m.UP)
         self.toFadeOut.add(commitId)
 
         commitMessage = commitMessage.split("\n")[0][:40].replace("\n", " ")
         message = m.Text(
             "\n".join(
                 commitMessage[j : j + 20] for j in range(0, len(commitMessage), 20)
             )[:100],
             font="Monospace",
             font_size=14,
             color=self.fontColor,
+            weight=self.font_weight,
         ).next_to(circle, m.DOWN)
         self.toFadeOut.add(message)
 
         if settings.animate:
             self.play(
                 self.camera.frame.animate.move_to(circle.get_center()),
                 m.Create(circle),
@@ -1052,15 +1119,21 @@
         return "dark"
 
     def get_nondark_commits(self):
         nondark_commits = []
         return nondark_commits
 
     def draw_ref(self, commit, top, i=0, text="HEAD", color=m.BLUE):
-        refText = m.Text(text, font="Monospace", font_size=20, color=self.fontColor)
+        refText = m.Text(
+            text,
+            font="Monospace",
+            font_size=20,
+            color=self.fontColor,
+            weight=self.font_weight,
+        )
         refbox = m.Rectangle(
             color=color,
             fill_color=color,
             fill_opacity=self.ref_fill_opacity,
             height=0.4,
             width=refText.width + 0.25,
         )
@@ -1175,26 +1248,27 @@
                 )
                 .shift(m.DOWN * 0.5 * (h + 1))
             )
             thirdColumnFiles.add(text)
             thirdColumnFilesDict[f] = text
 
     def color_by(self, offset=0):
-        if settings.color_by == "author":
+        if settings.color_by == ColorByOptions.AUTHOR:
             sorted_authors = sorted(
                 self.author_groups.keys(),
                 key=lambda k: len(self.author_groups[k]),
                 reverse=True,
             )
             for i, author in enumerate(sorted_authors):
                 authorText = m.Text(
                     f"{author[:15]} ({str(len(self.author_groups[author]))})",
                     font="Monospace",
                     font_size=36,
                     color=self.colors[int(i % 11)],
+                    weight=self.font_weight,
                 )
                 authorText.move_to(
                     [(-5 - offset) if settings.reverse else (5 + offset), -i, 0]
                 )
                 self.toFadeOut.add(authorText)
                 if i == 0:
                     self.recenter_frame()
@@ -1204,25 +1278,25 @@
                 else:
                     self.add(authorText)
                 for g in self.author_groups[author]:
                     g[0].set_color(self.colors[int(i % 11)])
             self.recenter_frame()
             self.scale_frame()
 
-        elif settings.color_by == "branch":
+        elif settings.color_by == ColorByOptions.BRANCH:
             pass
 
-        elif settings.color_by == "notlocal1":
+        elif settings.color_by == ColorByOptions.NOTLOCAL1:
             for commit_id in self.drawnCommits:
                 try:
                     self.orig_repo.commit(commit_id)
                 except ValueError:
                     self.drawnCommits[commit_id].set_color(m.GOLD)
 
-        elif settings.color_by == "notlocal2":
+        elif settings.color_by == ColorByOptions.NOTLOCAL2:
             for commit_id in self.drawnCommits:
                 if not self.orig_repo.is_ancestor(commit_id, "HEAD"):
                     self.drawnCommits[commit_id].set_color(m.GOLD)
 
     def add_group_to_author_groups(self, author, group):
         if author not in self.author_groups:
             self.author_groups[author] = [group]
```

### Comparing `git-sim-0.2.9/git_sim/log.py` & `git-sim-0.3.0/git_sim/log.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/logo.png` & `git-sim-0.3.0/git_sim/logo.png`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/merge.py` & `git-sim-0.3.0/git_sim/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,21 @@
                 self.center_frame_on_commit(branch_commit)
                 commitId = self.setup_and_draw_parent(branch_commit, self.message)
 
                 # If pre-merge HEAD is on screen, drawn an arrow to it as 2nd parent
                 if head_commit.hexsha in self.drawnCommits:
                     start = self.drawnCommits["abcdef"].get_center()
                     end = self.drawnCommits[head_commit.hexsha].get_center()
-                    arrow = m.CurvedArrow(start, end, color=self.fontColor)
+                    arrow = m.CurvedArrow(
+                        start,
+                        end,
+                        color=self.fontColor,
+                        stroke_width=self.arrow_stroke_width,
+                        tip_shape=self.arrow_tip_shape,
+                    )
                     self.draw_arrow(True, arrow)
 
                 reset_head_to = "abcdef"
                 shift = numpy.array([0.0, 0.0, 0.0])
 
             self.recenter_frame()
             self.scale_frame()
@@ -148,15 +154,18 @@
         self.fadeout()
         self.show_outro()
 
         # Unlink the program from the filesystem
         self.repo.git.clear_cache()
 
         # Delete the local clone
-        shutil.rmtree(new_dir, onerror=self.del_rw)
+        try:
+            shutil.rmtree(new_dir, onerror=self.del_rw)
+        except (FileNotFoundError, UnboundLocalError):
+            pass
 
     def check_merge_conflict(self, branch1, branch2):
         git_root = self.repo.git.rev_parse("--show-toplevel")
         repo_name = os.path.basename(self.repo.working_dir)
         new_dir = os.path.join(tempfile.gettempdir(), "git_sim", repo_name)
 
         orig_repo = self.repo
```

### Comparing `git-sim-0.2.9/git_sim/pull.py` & `git-sim-0.3.0/git_sim/pull.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/push.py` & `git-sim-0.3.0/git_sim/push.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import tempfile
 import shutil
 import stat
 import re
 
 from git_sim.git_sim_base_command import GitSimBaseCommand
 from git_sim.settings import settings
+from git_sim.enums import ColorByOptions
 
 
 class Push(GitSimBaseCommand):
     def __init__(self, remote: str = None, branch: str = None):
         super().__init__()
         self.remote = remote
         self.branch = branch
@@ -72,20 +73,20 @@
             self.repo.git.push(self.remote, self.branch)
         # If push fails...
         except git.GitCommandError as e:
             if "rejected" in e.stderr and ("fetch first" in e.stderr):
                 push_result = 1
                 self.orig_repo = self.repo
                 self.repo = self.remote_repo
-                settings.color_by = "notlocal1"
+                settings.color_by = ColorByOptions.NOTLOCAL1
             elif "rejected" in e.stderr and ("non-fast-forward" in e.stderr):
                 push_result = 2
                 self.orig_repo = self.repo
                 self.repo = self.remote_repo
-                settings.color_by = "notlocal2"
+                settings.color_by = ColorByOptions.NOTLOCAL2
             else:
                 print(f"git-sim error: git push failed: {e.stderr}")
                 return
 
         head_commit = self.get_commit()
         if push_result > 0:
             self.parse_commits(
@@ -169,15 +170,15 @@
                 font_size=20,
                 color=self.fontColor,
                 weight=m.BOLD,
             )
             text2.move_to(text1.get_center()).shift(m.DOWN / 2)
 
             text3 = m.Text(
-                f"Gold commits exist are ahead of your current branch tip (need to be pulled).",
+                f"Gold commits are ahead of your current branch tip (need to be pulled).",
                 font="Monospace",
                 font_size=20,
                 color=m.GOLD,
                 weight=m.BOLD,
             )
             text3.move_to(text2.get_center()).shift(m.DOWN / 2)
```

### Comparing `git-sim-0.2.9/git_sim/rebase.py` & `git-sim-0.3.0/git_sim/rebase.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,26 +107,38 @@
     def setup_and_draw_parent(
         self,
         child,
         commitMessage="New commit",
         shift=numpy.array([0.0, 0.0, 0.0]),
         draw_arrow=True,
     ):
-        circle = m.Circle(stroke_color=m.RED, fill_color=m.RED, fill_opacity=0.25)
+        circle = m.Circle(
+            stroke_color=m.RED,
+            stroke_width=self.commit_stroke_width,
+            fill_color=m.RED,
+            fill_opacity=0.25,
+        )
         circle.height = 1
         circle.next_to(
             self.drawnCommits[child],
             m.LEFT if settings.reverse else m.RIGHT,
             buff=1.5,
         )
         circle.shift(shift)
 
         start = circle.get_center()
         end = self.drawnCommits[child].get_center()
-        arrow = m.Arrow(start, end, color=self.fontColor)
+        arrow = m.Arrow(
+            start,
+            end,
+            color=self.fontColor,
+            stroke_width=self.arrow_stroke_width,
+            tip_shape=self.arrow_tip_shape,
+            max_stroke_width_to_length_ratio=1000,
+        )
         length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
         arrow.set_length(length)
 
         sha = "".join(
             chr(ord(letter) + 1)
             if (
                 (chr(ord(letter) + 1).isalpha() and letter < "f")
```

### Comparing `git-sim-0.2.9/git_sim/reset.py` & `git-sim-0.3.0/git_sim/reset.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/restore.py` & `git-sim-0.3.0/git_sim/restore.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/revert.py` & `git-sim-0.3.0/git_sim/revert.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,25 +87,37 @@
                 font_size=20,
                 color=self.fontColor,
             )
             commitMessage = commit.message.split("\n")[0][:40].replace("\n", " ")
         return commitId, commitMessage, commit, hide_refs
 
     def setup_and_draw_revert_commit(self):
-        circle = m.Circle(stroke_color=m.RED, fill_color=m.RED, fill_opacity=0.25)
+        circle = m.Circle(
+            stroke_color=m.RED,
+            stroke_width=self.commit_stroke_width,
+            fill_color=m.RED,
+            fill_opacity=0.25,
+        )
         circle.height = 1
         circle.next_to(
             self.drawnCommits[self.get_commit().hexsha],
             m.LEFT if settings.reverse else m.RIGHT,
             buff=1.5,
         )
 
         start = circle.get_center()
         end = self.drawnCommits[self.get_commit().hexsha].get_center()
-        arrow = m.Arrow(start, end, color=self.fontColor)
+        arrow = m.Arrow(
+            start,
+            end,
+            color=self.fontColor,
+            stroke_width=self.arrow_stroke_width,
+            tip_shape=self.arrow_tip_shape,
+            max_stroke_width_to_length_ratio=1000,
+        )
         length = numpy.linalg.norm(start - end) - (1.5 if start[1] == end[1] else 3)
         arrow.set_length(length)
 
         commitId = m.Text(
             "abcdef", font="Monospace", font_size=20, color=self.fontColor
         ).next_to(circle, m.UP)
         self.toFadeOut.add(commitId)
```

### Comparing `git-sim-0.2.9/git_sim/settings.py` & `git-sim-0.3.0/git_sim/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 import pathlib
-
-from enum import Enum
 from typing import List, Union
-from pydantic import BaseSettings
-
-
-class VideoFormat(str, Enum):
-    mp4 = "mp4"
-    webm = "webm"
 
+from pydantic import BaseSettings
 
-class ImgFormat(str, Enum):
-    jpg = "jpg"
-    png = "png"
+from git_sim.enums import StyleOptions, ColorByOptions, ImgFormat, VideoFormat
 
 
 class Settings(BaseSettings):
     allow_no_commits = False
     animate = False
     auto_open = True
     n_default = 5
     n = 5
     files: Union[List[pathlib.Path], None] = None
     hide_first_tag = False
-    img_format: ImgFormat = ImgFormat.jpg
+    img_format: ImgFormat = ImgFormat.JPG
     INFO_STRING = "Simulating: git"
     light_mode = False
     transparent_bg = False
     logo = pathlib.Path(__file__).parent.resolve() / "logo.png"
     low_quality = False
     max_branches_per_commit = 1
     max_tags_per_commit = 1
@@ -35,22 +26,23 @@
     outro_bottom_text = "Learn more at initialcommit.com"
     outro_top_text = "Thanks for using Initial Commit!"
     reverse = False
     show_intro = False
     show_outro = False
     speed = 1.5
     title = "Git-Sim, by initialcommit.com"
-    video_format: VideoFormat = VideoFormat.mp4
+    video_format: VideoFormat = VideoFormat.MP4
     stdout = False
     output_only_path = False
     quiet = False
     invert_branches = False
     hide_merged_branches = False
     all = False
-    color_by: Union[str, None] = None
+    color_by: Union[ColorByOptions, None] = None
     highlight_commit_messages = False
+    style: Union[StyleOptions, None] = StyleOptions.CLEAN
 
     class Config:
         env_prefix = "git_sim_"
 
 
 settings = Settings()
```

### Comparing `git-sim-0.2.9/git_sim/stash.py` & `git-sim-0.3.0/git_sim/stash.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/status.py` & `git-sim-0.3.0/git_sim/status.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/switch.py` & `git-sim-0.3.0/git_sim/switch.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim/tag.py` & `git-sim-0.3.0/git_sim/tag.py`

 * *Files identical despite different names*

### Comparing `git-sim-0.2.9/git_sim.egg-info/PKG-INFO` & `git-sim-0.3.0/git_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-sim
-Version: 0.2.9
+Version: 0.3.0
 Summary: Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.
 Home-page: https://initialcommit.com/tools/git-sim
 Author: Jacob Stopak
 Author-email: jacob@initialcommit.io
 Project-URL: Homepage, https://initialcommit.com/tools/git-sim
 Project-URL: Source, https://github.com/initialcommit-com/git-sim
 Keywords: git sim simulation simulate git-simulate git-simulation git-sim manim animation gitanimation image video dryrun dry-run
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # git-sim
+![git-sim-logo-with-tagline-1440x376p45](https://user-images.githubusercontent.com/49353917/232990611-58d0693f-69c0-45c8-b51d-cd540793d18c.gif)
+
 [![GitHub license](https://img.shields.io/github/license/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/blob/main/LICENSE)
 [![GitHub tag](https://img.shields.io/github/v/release/initialcommit-com/git-sim)](https://img.shields.io/github/v/release/initialcommit-com/git-sim)
 [![Downloads](https://static.pepy.tech/badge/git-sim)](https://pepy.tech/project/git-sim)
 [![Contributors](https://img.shields.io/github/contributors/initialcommit-com/git-sim)](https://github.com/initialcommit-com/git-sim/graphs/contributors)
 [![Share](https://img.shields.io/twitter/url?label=Share&url=https%3A%2F%2Ftwitter.com%2Finitcommit)](https://twitter.com/intent/tweet?text=Check%20out%20%23gitsim%20%2D%20a%20tool%20to%20visualize%20%23Git%20operations%20in%20your%20local%20repos%20with%20a%20single%20terminal%20command,%20by%20%40initcommit!%20https%3A%2F%2Fgithub%2Ecom%2Finitialcommit%2Dcom%2Fgit%2Dsim)
 
 Visually simulate Git operations in your own repos with a single terminal command.
@@ -31,23 +33,23 @@
 Example: `$ git-sim merge <branch>`
 
 ![git-sim-merge_01-05-23_09-44-46](https://user-images.githubusercontent.com/49353917/210939840-1d51493a-6cac-43fd-9d12-3d2948d32c61.jpg)
 
 ## Use cases
 - Visualize Git commands to understand their effects on your repo before actually running them
 - Prevent unexpected working directory and repository states by simulating before running
-- Share visualizations (jpg image or mp4 video) of your Git commands with your team, or the world
+- Share visualizations (jpg/png image or mp4/webm video) of your Git commands with your team, or the world
 - Save visualizations as a part of your team documentation to document workflow and prevent recurring issues
-- Create static Git diagrams (jpg) or dynamic animated videos (mp4) to speed up content creation
+- Create static Git diagrams (jpg/png) or dynamic animated videos (mp4/webm) to speed up content creation
 - Help visual learners understand how Git commands work
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 
 ## Features
 - Run a one-liner git-sim command in the terminal to generate a custom Git command visualization (.jpg) from your repo
-- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`
+- Supported commands: `log`, `status`, `add`, `restore`, `commit`, `stash`, `branch`, `tag`, `reset`, `revert`, `merge`, `rebase`, `cherry-pick`, `switch`, `checkout`, `fetch`, `pull`, `push`, `clone`, `rm`, `mv`, `clean`
 - Generate an animated video (.mp4) instead of a static image using the `--animate` flag (note: significant performance slowdown, it is recommended to use `--low-quality` to speed up testing and remove when ready to generate presentation-quality video)
 - Color commits by parameter, such as author the `--color-by=author` option
 - Choose between dark mode (default) and light mode
 - Specify output formats of either jpg, png, mp4, or webm
 - Combine with bundled command [git-dummy](https://github.com/initialcommit-com/git-dummy) to generate a dummy Git repo and then simulate operations on it
 - Animation only: Add custom branded intro/outro sequences if desired
 - Animation only: Speed up or slow down animation speed as desired
@@ -139,15 +141,15 @@
 
 ## Requirements
 * Python 3.7 or greater
 * Pip (Package manager for Python)
 * [Manim (Community version)](https://www.manim.community/)
 
 ## Commands
-Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", along with corresponding options.
+Basic usage is similar to Git itself - `git-sim` takes a familiar set of subcommands including "log", "status", "add", "restore", "commit", "stash", "branch", "tag", "reset", "revert", "merge", "rebase", "cherry-pick", "switch", "checkout", "fetch", "pull", "push", "clone", "rm", "mv", "clean" along with corresponding options.
 
 ```console
 $ git-sim [global options] <subcommand> [subcommand options]
 ```
 
 The `[global options]` apply to the overarching `git-sim` simulation itself, including:
 
@@ -161,15 +163,16 @@
 `-d`: Disable the automatic opening of the image/video file after generation. Useful to avoid errors in console mode with no GUI.  
 `--light-mode`: Use a light mode color scheme instead of default dark mode.  
 `--reverse, -r`: Display commit history in the reverse direction.  
 `--img-format`: Output format for the image file, i.e. `jpg` or `png`. Default output format is `jpg`.  
 `--stdout`: Write raw image data to stdout while suppressing all other program output.  
 `--output-only-path`: Only output the path to the generated media file to stdout. Useful for other programs to ingest.  
 `--quiet, -q`: Suppress all output except errors.  
-`--highlight-commit-messages`: Make commit message text bigger and bold, and hide commit ids.
+`--highlight-commit-messages`: Make commit message text bigger and bold, and hide commit ids.  
+`--style`: Graphical style of the output image or animated video, i.e. `clean` (default) or `thick`.
 
 Animation-only global options (to be used in conjunction with `--animate`):
 
 `--video-format`: Output format for the video file, i.e. `mp4` or `webm`. Default output format is `mp4`.  
 `--speed=n`: Set the multiple of animation speed of the output simulation, `n` can be an integer or float, default is 1.5.  
 `--low-quality`: Render the animation in low quality to speed up creation time, recommended for non-presentation use.  
 `--show-intro`: Add an intro sequence with custom logo and title.  
@@ -302,45 +305,85 @@
 
 ### git switch
 Usage: `git-sim switch [-c] <branch>`
 
 - Switches the checked-out branch to `<branch>`, i.e. moves `HEAD` to the specified `<branch>`
 - The `-c` flag creates a new branch with the specified name `<branch>` and switches to it, assuming it doesn't already exist
 
+![git-sim-switch_04-09-23_21-42-43](https://user-images.githubusercontent.com/49353917/230827783-a8740ace-b66f-4cac-b94e-5d101d27e0b5.jpg)
+
 ### git checkout
 Usage: `git-sim checkout [-b] <branch>`
 
 - Checks out `<branch>` into the working directory, i.e. moves `HEAD` to the specified `<branch>`
 - The `-b` flag creates a new branch with the specified name `<branch>` and checks it out, assuming it doesn't already exist
 
+![git-sim-checkout_04-09-23_21-46-04](https://user-images.githubusercontent.com/49353917/230827836-e9f23a0e-2576-4716-b2fb-6327d3cf9b22.jpg)
+
 ### git fetch
 Usage: `git-sim fetch <remote> <branch>`
 
 - Fetches the specified `<branch>` from the specified `<remote>` to the local repo
 
+![git-sim-fetch_04-09-23_21-47-59](https://user-images.githubusercontent.com/49353917/230828090-acae8979-4097-43a8-96ea-525890e0e0a8.jpg)
+
 ### git pull
 Usage: `git-sim pull [<remote> <branch>]`
 
 - Pulls the specified `<branch>` from the specified `<remote>` to the local repo
 - If `<remote>` and `<branch>` are not specified, the active branch is pulled from the default remote
 - If merge conflicts occur, they are displayed in a table
 
+![git-sim-pull_04-09-23_21-50-15](https://user-images.githubusercontent.com/49353917/230828298-455c0a9d-cf94-499e-9e35-623e7b218772.jpg)
+
 ### git push
 Usage: `git-sim push [<remote> <branch>]`
 
 - Pushes the specified `<branch>` to the specified `<remote>` and displays the local result
 - If `<remote>` and `<branch>` are not specified, the active branch is pushed to the default remote
 - If the push fails due to remote changes that don't exist in the local repo, a message is included telling the user to pull first, along with color coding which commits need to be pulled
 
+![git-sim-push_04-21-23_13-41-57](https://user-images.githubusercontent.com/49353917/233731005-51fd7887-ae14-4ceb-a5d5-e5aed79e9fd8.jpg)
+
 ### git clone
 Usage: `git-sim clone <url>`
 
 - Clone the remote repo from `<url>` (web URL or filesystem path) to a new folder in the current directory
 - Output will report if clone operation is successful and show log of local clone
 
+![git-sim-clone_04-09-23_21-51-53](https://user-images.githubusercontent.com/49353917/230828521-80c8d2d1-2a31-46bb-aeed-746f0441c86e.jpg)
+
+### git rm
+Usage: `git-sim rm <file 1> <file 2> ... <file n>`
+
+- Specify one or more `<file>` as a *tracked* file
+- Simulated output will show files being removed from Git tracking
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-rm_04-09-23_22-01-29](https://user-images.githubusercontent.com/49353917/230829899-f5d688ea-bc8e-46f9-a54a-55d251c8915d.jpg)
+
+### git mv
+Usage: `git-sim mv <file> <new file>`
+
+- Specify `<file>` as file to update name/path
+- Specify `<new file>` as new name/path of file 
+- Simulated output will show the name/path of the file being updated 
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-mv_04-09-23_22-05-13](https://user-images.githubusercontent.com/49353917/230829978-0a64dbe2-d974-4cef-9c6e-ed26e987342f.jpg)
+
+### git clean
+Usage: `git-sim clean`
+
+- Simulated output will show untracked files being deleted
+- Since this is just a simulation, no need to specify `-i`, `-n`, `-f` as in regular Git
+- Note that simulated output will also show the most recent 5 commits on the active branch
+
+![git-sim-clean_04-09-23_22-05-54](https://user-images.githubusercontent.com/49353917/230830043-779e7230-f439-461a-a408-b19b263e86e4.jpg)
+
 ## Video animation examples
 ```console
 $ git-sim --animate reset HEAD^
 ```
 
 https://user-images.githubusercontent.com/49353917/210943230-f38d879b-bb0d-4d42-a196-f24efb9e351a.mp4
```

### Comparing `git-sim-0.2.9/git_sim.egg-info/SOURCES.txt` & `git-sim-0.3.0/git_sim.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 git_sim/__init__.py
 git_sim/__main__.py
 git_sim/add.py
 git_sim/animations.py
 git_sim/branch.py
 git_sim/checkout.py
 git_sim/cherrypick.py
+git_sim/clean.py
 git_sim/clone.py
 git_sim/commands.py
 git_sim/commit.py
 git_sim/enums.py
 git_sim/fetch.py
 git_sim/git_sim_base_command.py
 git_sim/log.py
 git_sim/logo.png
 git_sim/merge.py
+git_sim/mv.py
 git_sim/pull.py
 git_sim/push.py
 git_sim/rebase.py
 git_sim/reset.py
 git_sim/restore.py
 git_sim/revert.py
+git_sim/rm.py
 git_sim/settings.py
 git_sim/stash.py
 git_sim/status.py
 git_sim/switch.py
 git_sim/tag.py
 git_sim.egg-info/PKG-INFO
 git_sim.egg-info/SOURCES.txt
```

### Comparing `git-sim-0.2.9/setup.py` & `git-sim-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import setuptools
 
+from git_sim import __version__
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="git-sim",
-    version="0.2.9",
+    version=__version__,
     author="Jacob Stopak",
     author_email="jacob@initialcommit.io",
     description="Simulate Git commands on your own repos by generating an image (default) or video visualization depicting the command's behavior.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://initialcommit.com/tools/git-sim",
     packages=setuptools.find_packages(),
```

