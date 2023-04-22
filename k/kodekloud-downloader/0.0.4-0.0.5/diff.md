# Comparing `tmp/kodekloud-downloader-0.0.4.tar.gz` & `tmp/kodekloud-downloader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodekloud-downloader-0.0.4.tar", max compression
+gzip compressed data, was "kodekloud-downloader-0.0.5.tar", max compression
```

## Comparing `kodekloud-downloader-0.0.4.tar` & `kodekloud-downloader-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13313 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/README.md
--rw-r--r--   0        0        0     1032 2023-04-18 14:19:06.454553 kodekloud-downloader-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/src/kodekloud_downloader/__init__.py
--rw-r--r--   0        0        0     1729 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/src/kodekloud_downloader/cli.py
--rw-r--r--   0        0        0      134 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/src/kodekloud_downloader/enums.py
--rw-r--r--   0        0        0     2144 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/src/kodekloud_downloader/helpers.py
--rw-r--r--   0        0        0     2273 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/src/kodekloud_downloader/main.py
--rw-r--r--   0        0        0     1976 2023-04-18 14:18:56.654408 kodekloud-downloader-0.0.4/src/kodekloud_downloader/models.py
--rw-r--r--   0        0        0    14597 2023-04-18 14:19:08.281249 kodekloud-downloader-0.0.4/setup.py
--rw-r--r--   0        0        0    14202 2023-04-18 14:19:08.282835 kodekloud-downloader-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    14008 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/README.md
+-rw-r--r--   0        0        0     1032 2023-04-22 06:52:58.409471 kodekloud-downloader-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/src/kodekloud_downloader/__init__.py
+-rw-r--r--   0        0        0     1748 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/src/kodekloud_downloader/cli.py
+-rw-r--r--   0        0        0      134 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/src/kodekloud_downloader/enums.py
+-rw-r--r--   0        0        0     2186 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/src/kodekloud_downloader/helpers.py
+-rw-r--r--   0        0        0     2275 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/src/kodekloud_downloader/main.py
+-rw-r--r--   0        0        0     1976 2023-04-22 06:52:49.537222 kodekloud-downloader-0.0.5/src/kodekloud_downloader/models.py
+-rw-r--r--   0        0        0    15291 2023-04-22 06:52:59.849115 kodekloud-downloader-0.0.5/setup.py
+-rw-r--r--   0        0        0    14897 2023-04-22 06:52:59.850437 kodekloud-downloader-0.0.5/PKG-INFO
```

### Comparing `kodekloud-downloader-0.0.4/README.md` & `kodekloud-downloader-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # KodeKloud Downloader
 
 ## Disclaimer
-Please use this only to keep your local copy. Please don't distribute the courses illegally. You will be responsible for the legal consequences. 
+Please read the following disclaimer carefully before using the Downloader CLI Tool.
+
+- The CLI Tool is intended for personal use only. By using this tool, you agree to use it at your own risk and assume full responsibility for any consequences that may arise from its use. The developers and contributors of this tool are not responsible for any damages or losses that may occur from its use.
+
+- The use of this tool to download premium courses is for educational purposes only. You must have the proper authorization or permission from the course provider to access the content legally.
+
+- It is strictly prohibited to distribute or share the downloaded content through any means, including but not limited to uploading to file-sharing platforms, torrent sites, or any other form of digital or physical distribution. Doing so is a violation of copyright laws and may result in legal consequences.
 
 ---
 
 ## Features
 
-- Download video lessons in selected quality
-- Download resources (PDFs, etc.) alongside video lessons
-- Organizes downloaded content in a structured folder hierarchy
+- [x] Download video lessons in selected quality
+- [x] Organizes downloaded content in a structured folder hierarchy
+- [ ] Download resources (PDFs, etc.) alongside video lessons
 
 ---
 
 ## Prerequisites
 
 - Python 3.8 or higher
 - ffmpeg
@@ -101,55 +107,50 @@
 
 </details>
 
 
 
 ## How to get cookie
 - Sign in to kodekloud.com
-- Right Click -> Inspect -> Go to Network Tab -> Reload -> Select the first resource and copy the cookie:
+- Download extension such as [Get cookies.txt LOCALLY](https://chrome.google.com/webstore/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc/related)
+- Download the cookie and save it in some location (You can name it something like `cookie.txt`).
 
-![](https://i.imgur.com/MwkR9u6.png)
+![](/static/cookie-demo.png)
 
 ## 💻 Installation
 
 To install kodekloud-downloader, simply run the following command:
 
 ```css
 pip install -U kodekloud-downloader
 ```
 
 ## 📚 Usage
 
 After installing the package, you can use the `kodekloud dl` command to download shows from the command line.
 
 ```css
-kisskh dl --help
+kodekloud dl --help
 Usage: kodekloud dl [OPTIONS] [COURSE_URL]
 
 Options:
   -q, --quality [360p|480p|540p|720p|1080p]
                                   Quality of the video to be downloaded.
   -o, --output-dir TEXT           Output directory where downloaded files will
                                   be store.
   -c, --cookie TEXT               Cookie to download the courses.  [required]
   --help                          Show this message and exit.
 ```
 
-Here are some examples:
-
-### 🔗 Direct download entire course in highest quality available in current folder
-
-```css
-kodekloud dl "https://kodekloud.com/courses/amazon-elastic-container-service-aws-ecs/" -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>
-```
+Here is an example:
 
 ### 🔍 Download entire course from list of available course in current folder
 
 ```css
-kodekloud dl -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>
+kodekloud dl -o . -c /path/to/cookie.txt
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 | No. | Name                                                                        | Type    | Categories                                                 |
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 | 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |
 | 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |
 | 3   | 12 Factor App                                                               | Premium | Productivity                                               |
 | 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |
@@ -201,8 +202,10 @@
 | 50  | DevOps Pre-Requisite Course                                                 | Premium | Automation, Devops, IAC                                    |
 | 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |
 | 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |
 | 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |
 | 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 Enter the number of the course you want to select: 35
-```
+```
+
+![](static/demo-select-download.gif)
```

### Comparing `kodekloud-downloader-0.0.4/pyproject.toml` & `kodekloud-downloader-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodekloud-downloader"
-version = "v0.0.4"
+version = "v0.0.5"
 description = "Simple downloaded for https://kodekloud.com/"
 readme = "README.md"
 authors = ["Roy, Debakar <debakar.roy@outlook.com>"]
 repository = "https://github.com/debakarr/kodekloud-downloader"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kodekloud-downloader-0.0.4/src/kodekloud_downloader/cli.py` & `kodekloud-downloader-0.0.5/src/kodekloud_downloader/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     default=Path.home() / "Downloads",
     help="Output directory where downloaded files will be store.",
 )
 @click.option(
     "--cookie",
     "-c",
     required=True,
-    help="Cookie to download the courses.",
+    help="Cookie file. Course should be accessible via this.",
 )
 def dl(course_url, quality: str, output_dir: Union[Path, str], cookie):
     if course_url is None:
         courses = get_all_course()
         selected_course = select_course(courses)
         download_course(url=selected_course.link, cookie=cookie, quality=quality, output_dir=output_dir)
     elif validators.url(course_url):
```

### Comparing `kodekloud-downloader-0.0.4/src/kodekloud_downloader/helpers.py` & `kodekloud-downloader-0.0.5/src/kodekloud_downloader/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 
 def download_video(url: str, output_path: Path, cookie: str, quality: str) -> int:
     ydl_opts = {
         "format": f"bestvideo[height<={quality[:-1]}]+bestaudio/best[height<={quality[:-1]}]/best",
         "concurrent_fragment_downloads": 15,
         "outtmpl": f"{output_path}.%(ext)s",
         "verbose": logger.getEffectiveLevel() == logging.DEBUG,
-        "cookie": cookie,
+        "cookiefile": cookie,
+        "merge_output_format": "mkv",
     }
     logger.debug(f"Calling download with following options: {ydl_opts}")
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         ydl.download(url)
 
 
 def normalize_name(name: str) -> str:
```

### Comparing `kodekloud-downloader-0.0.4/src/kodekloud_downloader/main.py` & `kodekloud-downloader-0.0.5/src/kodekloud_downloader/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from kodekloud_downloader.helpers import download_all_pdf, download_video, is_normal_content, normalize_name
 from kodekloud_downloader.models import Topic
 
 logger = logging.getLogger(__name__)
 
 
 def download_course(url: str, cookie: str, quality: str, output_dir: Union[str, Path]) -> None:
-    page = requests.get(url, headers={"Cookie": cookie})
+    page = requests.get(url)
     soup = BeautifulSoup(page.content, "html.parser")
     course_name = soup.find("h1", class_="course_title").text.strip()
     main_lesson_content = soup.find("div", class_="lessons_main__content")
     topics = main_lesson_content.find_all("div", class_="w-dyn-item")
     items = []
     for topic in topics:
         items.append(Topic.make(topic))
@@ -29,17 +29,18 @@
                 / normalize_name(course_name)
                 / f"{i} - {normalize_name(item.name)}"
                 / f"{j} - {normalize_name(lesson.name)}"
             )
             if lesson.is_video:
                 logger.info(f"Writing video file... {file_path}...")
                 file_path.parent.mkdir(parents=True, exist_ok=True)
+                logger.info(f"Parsing url: {lesson.url}")
                 download_video(url=lesson.url, output_path=file_path, cookie=cookie, quality=quality)
             else:
-                page = requests.get(lesson.url, headers={"Cookie": cookie})
+                page = requests.get(lesson.url)
                 soup = BeautifulSoup(page.content, "html.parser")
                 content = soup.find("div", class_="learndash_content_wrap")
                 # TODO: Fix this part. Most probably resources are not getting downloaded
                 if content and is_normal_content(content):
                     logger.info(f"Writing resource file... {file_path}...")
                     file_path.parent.mkdir(parents=True, exist_ok=True)
                     file_path.with_suffix(".md").write_text(
```

### Comparing `kodekloud-downloader-0.0.4/src/kodekloud_downloader/models.py` & `kodekloud-downloader-0.0.5/src/kodekloud_downloader/models.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.4/setup.py` & `kodekloud-downloader-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'yt-dlp>=2023.2.17,<2024.0.0']
 
 entry_points = \
 {'console_scripts': ['kodekloud = kodekloud_downloader.cli:kodekloud']}
 
 setup_kwargs = {
     'name': 'kodekloud-downloader',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Simple downloaded for https://kodekloud.com/',
-    'long_description': '# KodeKloud Downloader\n\n## Disclaimer\nPlease use this only to keep your local copy. Please don\'t distribute the courses illegally. You will be responsible for the legal consequences. \n\n---\n\n## Features\n\n- Download video lessons in selected quality\n- Download resources (PDFs, etc.) alongside video lessons\n- Organizes downloaded content in a structured folder hierarchy\n\n---\n\n## Prerequisites\n\n- Python 3.8 or higher\n- ffmpeg\n\n<details>\n    <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>\n\n# How to Install FFmpeg on Linux, Mac, and Windows\n\nFFmpeg is a powerful and flexible multimedia processing tool that can handle a wide range of tasks, such as video and audio conversion, streaming, and recording. In this guide, we will show you how to install FFmpeg on Linux, Mac, and Windows operating systems.\n\n## Linux\n\n### Ubuntu and Debian-based distributions\n\n1.  Update the package lists for upgrades and new package installations.\n\n`sudo apt update`\n\n1.  Install FFmpeg using the following command:\n\n`sudo apt install ffmpeg`\n\n### Fedora\n\n1.  Install FFmpeg using the following command:\n\n`sudo dnf install ffmpeg`\n\n### Arch Linux and Manjaro\n\n1.  Install FFmpeg using the following command:\n\n`sudo pacman -S ffmpeg`\n\n## Mac\n\n### Using Homebrew\n\nIf you don\'t have Homebrew installed, you can install it by following the instructions on the [official Homebrew website](https://brew.sh/).\n\nUpdate Homebrew to ensure you have the latest package information:\n\n`brew update`\n\n1.  Install FFmpeg using the following command:\n\n`brew install ffmpeg`\n\n### Using MacPorts\n\nIf you don\'t have MacPorts installed, you can install it by following the instructions on the [official MacPorts website](https://www.macports.org/install.php).\n\nUpdate MacPorts to ensure you have the latest package information:\n\n`sudo port selfupdate`\n\n1.  Install FFmpeg using the following command:\n\n`sudo port install ffmpeg`\n\n## Windows\n\n### Using Chocolatey\n\nIf you don\'t have Chocolatey installed, you can install it by following the instructions on the [official Chocolatey website](https://chocolatey.org/install).\n\nOpen an elevated Command Prompt (run as Administrator) and install FFmpeg using the following command:\n\n`choco install ffmpeg`\n\n### Using Scoop\n\nIf you don\'t have Scoop installed, you can install it by following the instructions on the [official Scoop website](https://scoop.sh/).\n\nOpen a PowerShell terminal and install FFmpeg using the following command:\n\n`scoop install ffmpeg`\n\nAfter following these steps, FFmpeg should be installed on your system. You can check the installation by running the following command in your terminal or command prompt:\n\n`ffmpeg -version`\n\nThis will display the FFmpeg version and build information, confirming that the installation was successful.\n\n</details>\n\n\n\n## How to get cookie\n- Sign in to kodekloud.com\n- Right Click -> Inspect -> Go to Network Tab -> Reload -> Select the first resource and copy the cookie:\n\n![](https://i.imgur.com/MwkR9u6.png)\n\n## 💻 Installation\n\nTo install kodekloud-downloader, simply run the following command:\n\n```css\npip install -U kodekloud-downloader\n```\n\n## 📚 Usage\n\nAfter installing the package, you can use the `kodekloud dl` command to download shows from the command line.\n\n```css\nkisskh dl --help\nUsage: kodekloud dl [OPTIONS] [COURSE_URL]\n\nOptions:\n  -q, --quality [360p|480p|540p|720p|1080p]\n                                  Quality of the video to be downloaded.\n  -o, --output-dir TEXT           Output directory where downloaded files will\n                                  be store.\n  -c, --cookie TEXT               Cookie to download the courses.  [required]\n  --help                          Show this message and exit.\n```\n\nHere are some examples:\n\n### 🔗 Direct download entire course in highest quality available in current folder\n\n```css\nkodekloud dl "https://kodekloud.com/courses/amazon-elastic-container-service-aws-ecs/" -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>\n```\n\n### 🔍 Download entire course from list of available course in current folder\n\n```css\nkodekloud dl -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| No. | Name                                                                        | Type    | Categories                                                 |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |\n| 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |\n| 3   | 12 Factor App                                                               | Premium | Productivity                                               |\n| 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |\n| 5   | Ultimate Certified Kubernetes Administrator (CKA) Mock Exam Series          | Free    | Container Orchestration, Kubernetes, Devops, Certification |\n| 6   | AWS Lambda                                                                  | Premium | AWS, Cloud                                                 |\n| 7   | Linux Professional Institute LPIC-1 Exam 101                                | Premium | Certification, Linux                                       |\n| 8   | Advanced Golang                                                             | Premium | Programming                                                |\n| 9   | Prometheus Certified Associate (PCA)                                        | Premium | Certification, Kubernetes, Monitoring                      |\n| 10  | GCP Cloud Digital Leader Certification                                      | Premium | Cloud, GCP, Certification                                  |\n| 11  | OpenShift 4                                                                 | Premium | Container Orchestration, Devops, Red Hat                   |\n| 12  | HashiCorp : Terraform Cloud                                                 | Premium | Cloud, Devops, HashiCorp                                   |\n| 13  | ArgoCD                                                                      | Premium | CI/CD, Devops, Kubernetes                                  |\n| 14  | Amazon Elastic Container Service (AWS ECS)                                  | Free    | AWS, Devops                                                |\n| 15  | Red Hat Certified System Administrator(RHCSA)                               | Premium | Devops, Linux, Red Hat, Certification                      |\n| 16  | Open Source for Beginners                                                   | Premium | Productivity                                               |\n| 17  | Kustomize                                                                   | Premium | Devops, Kubernetes                                         |\n| 18  | DevSecOps – Kubernetes DevOps & Security                                    | Premium | Devops, DevSecOps, Kubernetes                              |\n| 19  | AZ-104: Microsoft Azure Administrator                                       | Premium | Cloud, Devops, Certification                               |\n| 20  | DevOps Interview Preparation Course                                         | Premium | Devops                                                     |\n| 21  | Terraform Challenges                                                        | Free    | Challenges, Devops, IAC                                    |\n| 22  | HashiCorp Certified: Consul Associate Certification                         | Premium | Devops, HashiCorp                                          |\n| 23  | HashiCorp Certified: Vault Associate Certification                          | Premium | Devops, HashiCorp                                          |\n| 24  | Kubernetes Challenges                                                       | Free    | Challenges, Devops                                         |\n| 25  | Linux Challenges                                                            | Free    | Challenges, Devops, Linux                                  |\n| 26  | HashiCorp Certified: Vault Operations Professional 2022                     | Premium | Container Orchestration, Containers, Devops, HashiCorp     |\n| 27  | CKS – Challenges                                                            | Free    | Challenges, Container Orchestration, Containers, Devops    |\n| 28  | Linux Foundation Certified System Administrator (LFCS)                      | Premium | Devops, Linux, Certification                               |\n| 29  | Jenkins                                                                     | Premium | Automation, CI/CD, Devops                                  |\n| 30  | Golang                                                                      | Premium | Devops, Programming                                        |\n| 31  | Terraform Associate Certification: HashiCorp Certified                      | Premium | Container Orchestration, Devops, IAC, Certification        |\n| 32  | Helm for Beginners                                                          | Premium | Container Orchestration, Containers, Devops                |\n| 33  | PCAP – Python Certification Course                                          | Premium | Devops, Programming, Python, Certification                 |\n| 34  | Istio Service Mesh                                                          | Premium | Devops                                                     |\n| 35  | Jinja2 Basics (Mini Course)                                                 | Free    | Devops                                                     |\n| 36  | Certified Kubernetes Security Specialist (CKS)                              | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 37  | Certified Python Entry-Level Programmer: PCEP-30-02                         | Premium | Devops, Programming, Python, Certification                 |\n| 38  | JSON Path Test – Free Course                                                | Free    | Devops                                                     |\n| 39  | Docker Certified Associate Exam Course                                      | Premium | Containers, Devops, Certification                          |\n| 40  | Terraform Basics Training Course                                            | Premium | Automation, Devops, IAC                                    |\n| 41  | CKA Certification Course – Certified Kubernetes Administrator               | Premium | Container Orchestration, Containers, Devops                |\n| 42  | Certified Kubernetes Application Developer (CKAD)                           | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 43  | Kubernetes for the Absolute Beginners – Hands-on Tutorial                   | Premium | Container Orchestration, Containers, Kubernetes, Devops    |\n| 44  | Docker Training Course for the Absolute Beginner                            | Premium | Containers, Devops                                         |\n| 45  | Chef for the Absolute Beginners                                             | Premium | Automation, Devops                                         |\n| 46  | OpenShift 3 for the Absolute Beginners                                      | Premium | Container Orchestration, Containers, Devops                |\n| 47  | Ansible Advanced Course                                                     | Premium | Automation, Devops, IAC                                    |\n| 48  | Learn Ansible Basics – Beginners Course                                     | Premium | Automation, Devops, IAC                                    |\n| 49  | Docker – SWARM | SERVICES | STACKS – Hands-on                               | Premium | Containers, Devops                                         |\n| 50  | DevOps Pre-Requisite Course                                                 | Premium | Automation, Devops, IAC                                    |\n| 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |\n| 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |\n| 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |\n| 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\nEnter the number of the course you want to select: 35\n```',
+    'long_description': "# KodeKloud Downloader\n\n## Disclaimer\nPlease read the following disclaimer carefully before using the Downloader CLI Tool.\n\n- The CLI Tool is intended for personal use only. By using this tool, you agree to use it at your own risk and assume full responsibility for any consequences that may arise from its use. The developers and contributors of this tool are not responsible for any damages or losses that may occur from its use.\n\n- The use of this tool to download premium courses is for educational purposes only. You must have the proper authorization or permission from the course provider to access the content legally.\n\n- It is strictly prohibited to distribute or share the downloaded content through any means, including but not limited to uploading to file-sharing platforms, torrent sites, or any other form of digital or physical distribution. Doing so is a violation of copyright laws and may result in legal consequences.\n\n---\n\n## Features\n\n- [x] Download video lessons in selected quality\n- [x] Organizes downloaded content in a structured folder hierarchy\n- [ ] Download resources (PDFs, etc.) alongside video lessons\n\n---\n\n## Prerequisites\n\n- Python 3.8 or higher\n- ffmpeg\n\n<details>\n    <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>\n\n# How to Install FFmpeg on Linux, Mac, and Windows\n\nFFmpeg is a powerful and flexible multimedia processing tool that can handle a wide range of tasks, such as video and audio conversion, streaming, and recording. In this guide, we will show you how to install FFmpeg on Linux, Mac, and Windows operating systems.\n\n## Linux\n\n### Ubuntu and Debian-based distributions\n\n1.  Update the package lists for upgrades and new package installations.\n\n`sudo apt update`\n\n1.  Install FFmpeg using the following command:\n\n`sudo apt install ffmpeg`\n\n### Fedora\n\n1.  Install FFmpeg using the following command:\n\n`sudo dnf install ffmpeg`\n\n### Arch Linux and Manjaro\n\n1.  Install FFmpeg using the following command:\n\n`sudo pacman -S ffmpeg`\n\n## Mac\n\n### Using Homebrew\n\nIf you don't have Homebrew installed, you can install it by following the instructions on the [official Homebrew website](https://brew.sh/).\n\nUpdate Homebrew to ensure you have the latest package information:\n\n`brew update`\n\n1.  Install FFmpeg using the following command:\n\n`brew install ffmpeg`\n\n### Using MacPorts\n\nIf you don't have MacPorts installed, you can install it by following the instructions on the [official MacPorts website](https://www.macports.org/install.php).\n\nUpdate MacPorts to ensure you have the latest package information:\n\n`sudo port selfupdate`\n\n1.  Install FFmpeg using the following command:\n\n`sudo port install ffmpeg`\n\n## Windows\n\n### Using Chocolatey\n\nIf you don't have Chocolatey installed, you can install it by following the instructions on the [official Chocolatey website](https://chocolatey.org/install).\n\nOpen an elevated Command Prompt (run as Administrator) and install FFmpeg using the following command:\n\n`choco install ffmpeg`\n\n### Using Scoop\n\nIf you don't have Scoop installed, you can install it by following the instructions on the [official Scoop website](https://scoop.sh/).\n\nOpen a PowerShell terminal and install FFmpeg using the following command:\n\n`scoop install ffmpeg`\n\nAfter following these steps, FFmpeg should be installed on your system. You can check the installation by running the following command in your terminal or command prompt:\n\n`ffmpeg -version`\n\nThis will display the FFmpeg version and build information, confirming that the installation was successful.\n\n</details>\n\n\n\n## How to get cookie\n- Sign in to kodekloud.com\n- Download extension such as [Get cookies.txt LOCALLY](https://chrome.google.com/webstore/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc/related)\n- Download the cookie and save it in some location (You can name it something like `cookie.txt`).\n\n![](/static/cookie-demo.png)\n\n## 💻 Installation\n\nTo install kodekloud-downloader, simply run the following command:\n\n```css\npip install -U kodekloud-downloader\n```\n\n## 📚 Usage\n\nAfter installing the package, you can use the `kodekloud dl` command to download shows from the command line.\n\n```css\nkodekloud dl --help\nUsage: kodekloud dl [OPTIONS] [COURSE_URL]\n\nOptions:\n  -q, --quality [360p|480p|540p|720p|1080p]\n                                  Quality of the video to be downloaded.\n  -o, --output-dir TEXT           Output directory where downloaded files will\n                                  be store.\n  -c, --cookie TEXT               Cookie to download the courses.  [required]\n  --help                          Show this message and exit.\n```\n\nHere is an example:\n\n### 🔍 Download entire course from list of available course in current folder\n\n```css\nkodekloud dl -o . -c /path/to/cookie.txt\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| No. | Name                                                                        | Type    | Categories                                                 |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |\n| 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |\n| 3   | 12 Factor App                                                               | Premium | Productivity                                               |\n| 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |\n| 5   | Ultimate Certified Kubernetes Administrator (CKA) Mock Exam Series          | Free    | Container Orchestration, Kubernetes, Devops, Certification |\n| 6   | AWS Lambda                                                                  | Premium | AWS, Cloud                                                 |\n| 7   | Linux Professional Institute LPIC-1 Exam 101                                | Premium | Certification, Linux                                       |\n| 8   | Advanced Golang                                                             | Premium | Programming                                                |\n| 9   | Prometheus Certified Associate (PCA)                                        | Premium | Certification, Kubernetes, Monitoring                      |\n| 10  | GCP Cloud Digital Leader Certification                                      | Premium | Cloud, GCP, Certification                                  |\n| 11  | OpenShift 4                                                                 | Premium | Container Orchestration, Devops, Red Hat                   |\n| 12  | HashiCorp : Terraform Cloud                                                 | Premium | Cloud, Devops, HashiCorp                                   |\n| 13  | ArgoCD                                                                      | Premium | CI/CD, Devops, Kubernetes                                  |\n| 14  | Amazon Elastic Container Service (AWS ECS)                                  | Free    | AWS, Devops                                                |\n| 15  | Red Hat Certified System Administrator(RHCSA)                               | Premium | Devops, Linux, Red Hat, Certification                      |\n| 16  | Open Source for Beginners                                                   | Premium | Productivity                                               |\n| 17  | Kustomize                                                                   | Premium | Devops, Kubernetes                                         |\n| 18  | DevSecOps – Kubernetes DevOps & Security                                    | Premium | Devops, DevSecOps, Kubernetes                              |\n| 19  | AZ-104: Microsoft Azure Administrator                                       | Premium | Cloud, Devops, Certification                               |\n| 20  | DevOps Interview Preparation Course                                         | Premium | Devops                                                     |\n| 21  | Terraform Challenges                                                        | Free    | Challenges, Devops, IAC                                    |\n| 22  | HashiCorp Certified: Consul Associate Certification                         | Premium | Devops, HashiCorp                                          |\n| 23  | HashiCorp Certified: Vault Associate Certification                          | Premium | Devops, HashiCorp                                          |\n| 24  | Kubernetes Challenges                                                       | Free    | Challenges, Devops                                         |\n| 25  | Linux Challenges                                                            | Free    | Challenges, Devops, Linux                                  |\n| 26  | HashiCorp Certified: Vault Operations Professional 2022                     | Premium | Container Orchestration, Containers, Devops, HashiCorp     |\n| 27  | CKS – Challenges                                                            | Free    | Challenges, Container Orchestration, Containers, Devops    |\n| 28  | Linux Foundation Certified System Administrator (LFCS)                      | Premium | Devops, Linux, Certification                               |\n| 29  | Jenkins                                                                     | Premium | Automation, CI/CD, Devops                                  |\n| 30  | Golang                                                                      | Premium | Devops, Programming                                        |\n| 31  | Terraform Associate Certification: HashiCorp Certified                      | Premium | Container Orchestration, Devops, IAC, Certification        |\n| 32  | Helm for Beginners                                                          | Premium | Container Orchestration, Containers, Devops                |\n| 33  | PCAP – Python Certification Course                                          | Premium | Devops, Programming, Python, Certification                 |\n| 34  | Istio Service Mesh                                                          | Premium | Devops                                                     |\n| 35  | Jinja2 Basics (Mini Course)                                                 | Free    | Devops                                                     |\n| 36  | Certified Kubernetes Security Specialist (CKS)                              | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 37  | Certified Python Entry-Level Programmer: PCEP-30-02                         | Premium | Devops, Programming, Python, Certification                 |\n| 38  | JSON Path Test – Free Course                                                | Free    | Devops                                                     |\n| 39  | Docker Certified Associate Exam Course                                      | Premium | Containers, Devops, Certification                          |\n| 40  | Terraform Basics Training Course                                            | Premium | Automation, Devops, IAC                                    |\n| 41  | CKA Certification Course – Certified Kubernetes Administrator               | Premium | Container Orchestration, Containers, Devops                |\n| 42  | Certified Kubernetes Application Developer (CKAD)                           | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 43  | Kubernetes for the Absolute Beginners – Hands-on Tutorial                   | Premium | Container Orchestration, Containers, Kubernetes, Devops    |\n| 44  | Docker Training Course for the Absolute Beginner                            | Premium | Containers, Devops                                         |\n| 45  | Chef for the Absolute Beginners                                             | Premium | Automation, Devops                                         |\n| 46  | OpenShift 3 for the Absolute Beginners                                      | Premium | Container Orchestration, Containers, Devops                |\n| 47  | Ansible Advanced Course                                                     | Premium | Automation, Devops, IAC                                    |\n| 48  | Learn Ansible Basics – Beginners Course                                     | Premium | Automation, Devops, IAC                                    |\n| 49  | Docker – SWARM | SERVICES | STACKS – Hands-on                               | Premium | Containers, Devops                                         |\n| 50  | DevOps Pre-Requisite Course                                                 | Premium | Automation, Devops, IAC                                    |\n| 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |\n| 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |\n| 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |\n| 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\nEnter the number of the course you want to select: 35\n```\n\n![](static/demo-select-download.gif)\n",
     'author': 'Roy, Debakar',
     'author_email': 'debakar.roy@outlook.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/debakarr/kodekloud-downloader',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `kodekloud-downloader-0.0.4/PKG-INFO` & `kodekloud-downloader-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodekloud-downloader
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple downloaded for https://kodekloud.com/
 Home-page: https://github.com/debakarr/kodekloud-downloader
 Author: Roy, Debakar
 Author-email: debakar.roy@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -19,23 +19,29 @@
 Requires-Dist: yt-dlp (>=2023.2.17,<2024.0.0)
 Project-URL: Repository, https://github.com/debakarr/kodekloud-downloader
 Description-Content-Type: text/markdown
 
 # KodeKloud Downloader
 
 ## Disclaimer
-Please use this only to keep your local copy. Please don't distribute the courses illegally. You will be responsible for the legal consequences. 
+Please read the following disclaimer carefully before using the Downloader CLI Tool.
+
+- The CLI Tool is intended for personal use only. By using this tool, you agree to use it at your own risk and assume full responsibility for any consequences that may arise from its use. The developers and contributors of this tool are not responsible for any damages or losses that may occur from its use.
+
+- The use of this tool to download premium courses is for educational purposes only. You must have the proper authorization or permission from the course provider to access the content legally.
+
+- It is strictly prohibited to distribute or share the downloaded content through any means, including but not limited to uploading to file-sharing platforms, torrent sites, or any other form of digital or physical distribution. Doing so is a violation of copyright laws and may result in legal consequences.
 
 ---
 
 ## Features
 
-- Download video lessons in selected quality
-- Download resources (PDFs, etc.) alongside video lessons
-- Organizes downloaded content in a structured folder hierarchy
+- [x] Download video lessons in selected quality
+- [x] Organizes downloaded content in a structured folder hierarchy
+- [ ] Download resources (PDFs, etc.) alongside video lessons
 
 ---
 
 ## Prerequisites
 
 - Python 3.8 or higher
 - ffmpeg
@@ -123,55 +129,50 @@
 
 </details>
 
 
 
 ## How to get cookie
 - Sign in to kodekloud.com
-- Right Click -> Inspect -> Go to Network Tab -> Reload -> Select the first resource and copy the cookie:
+- Download extension such as [Get cookies.txt LOCALLY](https://chrome.google.com/webstore/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc/related)
+- Download the cookie and save it in some location (You can name it something like `cookie.txt`).
 
-![](https://i.imgur.com/MwkR9u6.png)
+![](/static/cookie-demo.png)
 
 ## 💻 Installation
 
 To install kodekloud-downloader, simply run the following command:
 
 ```css
 pip install -U kodekloud-downloader
 ```
 
 ## 📚 Usage
 
 After installing the package, you can use the `kodekloud dl` command to download shows from the command line.
 
 ```css
-kisskh dl --help
+kodekloud dl --help
 Usage: kodekloud dl [OPTIONS] [COURSE_URL]
 
 Options:
   -q, --quality [360p|480p|540p|720p|1080p]
                                   Quality of the video to be downloaded.
   -o, --output-dir TEXT           Output directory where downloaded files will
                                   be store.
   -c, --cookie TEXT               Cookie to download the courses.  [required]
   --help                          Show this message and exit.
 ```
 
-Here are some examples:
-
-### 🔗 Direct download entire course in highest quality available in current folder
-
-```css
-kodekloud dl "https://kodekloud.com/courses/amazon-elastic-container-service-aws-ecs/" -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>
-```
+Here is an example:
 
 ### 🔍 Download entire course from list of available course in current folder
 
 ```css
-kodekloud dl -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>
+kodekloud dl -o . -c /path/to/cookie.txt
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 | No. | Name                                                                        | Type    | Categories                                                 |
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 | 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |
 | 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |
 | 3   | 12 Factor App                                                               | Premium | Productivity                                               |
 | 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |
@@ -224,7 +225,10 @@
 | 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |
 | 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |
 | 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |
 | 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 Enter the number of the course you want to select: 35
 ```
+
+![](static/demo-select-download.gif)
+
```

