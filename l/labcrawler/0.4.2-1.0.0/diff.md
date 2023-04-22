# Comparing `tmp/labcrawler-0.4.2.tar.gz` & `tmp/labcrawler-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-0.4.2.tar", last modified: Wed Apr 19 19:43:39 2023, max compression
+gzip compressed data, was "labcrawler-1.0.0.tar", last modified: Sat Apr 22 03:10:25 2023, max compression
```

## Comparing `labcrawler-0.4.2.tar` & `labcrawler-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:43:39.464167 labcrawler-0.4.2/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-0.4.2/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-19 19:25:24.000000 labcrawler-0.4.2/MANIFEST.in
--rw-r--r--   0 francispotter   (501) staff       (20)     9034 2023-04-19 19:43:39.463405 labcrawler-0.4.2/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     8752 2023-04-19 19:25:24.000000 labcrawler-0.4.2/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:43:39.454279 labcrawler-0.4.2/labcrawler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-0.4.2/labcrawler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/_legacy.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3509 2023-04-19 19:32:32.000000 labcrawler-0.4.2/labcrawler/analysis.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5354 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/cli.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-0.4.2/labcrawler/gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3040 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/gitlab_ci_data_loader.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-0.4.2/labcrawler/gitlab_repository_files_extractor.py
--rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/project_data_file.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:43:39.460314 labcrawler-0.4.2/labcrawler/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/templates/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/templates/labcrawler.json.template
--rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-19 19:25:24.000000 labcrawler-0.4.2/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:43:39.458184 labcrawler-0.4.2/labcrawler.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     9034 2023-04-19 19:43:39.000000 labcrawler-0.4.2/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-19 19:43:39.000000 labcrawler-0.4.2/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-19 19:43:39.000000 labcrawler-0.4.2/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-19 19:43:39.000000 labcrawler-0.4.2/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-19 19:43:39.000000 labcrawler-0.4.2/labcrawler.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-19 19:43:39.000000 labcrawler-0.4.2/labcrawler.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-19 19:25:24.000000 labcrawler-0.4.2/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-19 19:43:39.464314 labcrawler-0.4.2/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:43:39.461332 labcrawler-0.4.2/test/
--rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-0.4.2/test/test_gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-19 19:43:28.000000 labcrawler-0.4.2/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.270439 labcrawler-1.0.0/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-1.0.0/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-22 03:09:31.000000 labcrawler-1.0.0/MANIFEST.in
+-rw-r--r--   0 francispotter   (501) staff       (20)    13528 2023-04-22 03:10:25.269366 labcrawler-1.0.0/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)    13246 2023-04-22 03:09:31.000000 labcrawler-1.0.0/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.263841 labcrawler-1.0.0/labcrawler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-1.0.0/labcrawler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/_legacy.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3509 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/analysis.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5354 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/cli.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-1.0.0/labcrawler/gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3040 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/gitlab_ci_data_loader.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-1.0.0/labcrawler/gitlab_repository_files_extractor.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/project_data_file.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.268015 labcrawler-1.0.0/labcrawler/templates/
+-rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/templates/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/templates/labcrawler.json.template
+-rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-22 03:09:31.000000 labcrawler-1.0.0/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.266020 labcrawler-1.0.0/labcrawler.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)    13528 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-22 03:10:25.000000 labcrawler-1.0.0/labcrawler.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-22 03:09:31.000000 labcrawler-1.0.0/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-22 03:10:25.270633 labcrawler-1.0.0/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-22 03:10:25.268436 labcrawler-1.0.0/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-1.0.0/test/test_gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-22 03:10:05.000000 labcrawler-1.0.0/version
```

### Comparing `labcrawler-0.4.2/LICENSE` & `labcrawler-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/PKG-INFO` & `labcrawler-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: labcrawler
-Version: 0.4.2
-Summary: Analysis tool for GitLab project and CI configurations
-Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
-License: MIT
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 Summary
 -------
 
 LabCrawler by [Francis Potter](https://www.linkedin.com/in/francispotter/) using [Meltano](https://meltano.com/) and [Pandas](https://pandas.pydata.org/).
 
 Examine a set of GitLab projects for usage of governance processes such as CI/CD, merge requests, merge request approvals, security scanning, and code review. This tool pulls project and group configuration and recent history data from GitLab and returns it in a CSV that can be imported to a spreadsheet.
@@ -59,43 +49,98 @@
 
 The workspace should be good for the life of LabCrawler, though in rare cases a LabCrawler upgrade might require you to recreate it, so check the release notes when upgrading.
 
 The output from the `init` command includes the location of the LabCrawler config file (`labcrawler.json`). Edit the file with the following information:
 
 - `api_url` - URL to the root of the GitLab API, including `https://`.
 - `groups` - All the groups containing projects that you wish to examine. LabCrawler will not examine subgroups, so include them too.
-- `output_dir` - Directory to store the CSV files that are generated; the default is a logical location based on the OS and might be sufficient.
+- `output_dir` - Directory to store the CSV files that are generated; the default is based on the OS and might be sufficient.
+
+*TODO: Note about the GitLab private token*
+
+Meltano loading
+---------------
 
-Use
----
+LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in analyzer.
 
-LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in `labcrawler analyze` command.
+Generating the CSV files requires two phases: `melt` and `load`.
 
-Generating the CSV files requires two phases:
+To run the Meltano load, issue the following command:
+
+```
+labcrawler melt
+```
 
-- `labcrawler melt` - Load all the data that is handled directly by Meltano. The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation] to understand the fields. Data loaded includes:
+The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation](https://docs.gitlab.com/ee/api/api_resources.html) to understand the fields. Data loaded includes:
     - `groups`
     - `projects`
     - `branches`
     - `merge_requests`
     - `project_members`
     - `group_members`
     - `users`
-- `labcrawler load` - Load LabCrawler-specific data, include CI configuration includes and committers. Data loaded includes:
-    - `ci_config_committers` - Names and email addresses of developers who have committed changes to the main GitLab CI configuration file in each project's repo. The location of the CI configuration file might be from the `ci_config_path` setting on the project, or it's `.gitlab-ci.yml`. Committer information comes from the `git blame` command so only includes the last developer to touch each line of the configuration.
-    - `ci_config_includes` - 
 
-    *TODO: Leftoff here*
+CI configuration data loading
+-----------------------------
+
+To load LabCrawler-specific data, include CI configuration includes and committers, issue the following command:
+
+```
+labcrawler load
+```
+
+The `load` command includes queries specific to GitLab CI configuration files, which are not covered by the Meltano tap.
+
+LabCrawler looks at each project's main GitLab CI configuration file. The default file is at the repo root with the name `.gitlab-ci.yml`, but the location can be overridden by the project maintainers, in which case it's read from the `ci_config_path` setting at the project level. Since `ci_config_path` is now loaded by the Meltano tap, LabCrawler uses that information to query about the correct file.
+
+At this point, the main GitLab CI configuration file is the only file for which LabCrawler loads file-specific information.
+
+The `load` phase loads two specific types of information:
+
+- *includes* - Paths to other GitLab CI configuration files from the same repo that are loaded into the main CI configuration file using the `include:` key. Useful to know where all the CI configuration lives, so it can be easily inspected.
+- *committers* - Names and email addresses of developers who committed the most recent change to at least one line of the main CI configuration file, as per the `git blame` command. Useful to know who has touched CI configuratoin most recently, so they can be easily questioned.
+
+*Understanding includes*
+
+To list the "includes", LabCrawler downloads the CI configuration file itself from the default branch, parses the YAML, and identifies the `include:` key if it exists. The idea is to help understand where more CI configuration lives inside the project.
+
+[The `include:` key](https://docs.gitlab.com/ee/ci/yaml/includes.html) has some power, including the ability to include templates (shipped with GitLab itself) and CI configuration files from other projects and even from URLs outside of the GitLab instance. LabCrawler only lists local includes - that is, other CI configuration files in the same project that are used by the main CI configuration file.
+
+*Understanding committers*
+
+LabCralwer's "committers" list is based on the output from a [GitLab API call](https://docs.gitlab.com/ee/api/repository_files.html#get-file-blame-from-repository) that emulates the [`git blame`](https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-blame) command.
+
+Git differentiates between the author of a commit and the committer, both of which are stored by name and email address within the repo based on the developer's local configuration settings. Authors and committers are not authenticated by Git itself on the desktop.
+
+A push to GitLab might contain one or more commits. GitLab requires authentication and authorization for every push, and records the user who made the push in the database. Optionally, a pre-receive hook can be set up to confirm that the committers (inside the repo data) are authorized users. It's also possible to require signed commits. But GitLab has no way to authenticate the committers themselves, who might have committed code offline.
+
+So within the GitLab API, committer information comes from the Git repo itself, not from the users table. LabCrawler doesn't check other project-level configuration (such as push rules and the signed commit requirement) when reporting committer data. The discrepancy can result in surprises, such as commits by people not authorized to push to the repo, or even employees from other companies (or GitLab itself) showing up as committers.
+
+To investigate why an unknown committer appears in the committers data, use the GitLab web UI. Navigate to the project in question, identify the CI configuration file, and click the "Blame" button. You'll be able to see exactly which lines of code were touched by each committer, and with what commit message. It's also possible to use the "History" button to see the history of all commits to the file.
+
+Note that LabCrawler simply extracts the committers themselves from the API output, and discards the detailed information about which line each developer committed.
+
+*TODO: Note about only loading one project's data*
 
 Analysis
 --------
 
-Then you may examine the results using `pandas` in the Python shell. We've provided a useful way to do so with the `analyze` script. To run it, type:
+LabCrawler generates simple CSV files in the output directory, which can be opened using Microsoft Excel or any other CSV application. Also, LabCrawler offers an easy-to-use analysis prompt based on `pandas`. To use the analysis:
+
+```
+labcrawler analyze
+```
+
+The above command:
+
+1. Reads the CSV file data into Pandas DataFrames (called "raw)
+2. Joins raw DataFrames into slightly-more-useful DataFrames with specific names for each datatype
+3. Outputs how many rows are in each DataFrame, with the variable name for each
+4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
-The above command will run the `analyze` script, which loads the CSV file data into Pandas. It then starts the command-line Python interpreter so you may experiment with the values. Before opening the shell, it lists the objects that are present. Try some of these:
 
 ``` python
 
 # See what columns are available in any table
 projects.columns
 
 # View just certain columns from a table
@@ -131,59 +176,59 @@
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
 
 ``` python
 pandas.set_option('display.max_rows', None)
 ```
 
-Extracting CI Config information
---------------------------------
-
-There is a mechanism for extracting CI configuration information from GitLab which is separate from Meltano. The `run-extract` command uses it, but by calling it directly you can troubleshoot issues and read the CI config file itself.
-
-``` bash
-source .env
-python -m labcrawler.ci_config_extractor
-```
-
-There are two options for the above command:
-
-- `--project <id>` allows you to specify an individual project ID, so it won't pull all of the data if things are malfunctioning.
-- `--output file` will save the data to `output/ci_config_committers.csv` same as in the `./run-extract` command.
-- `--query content` will dump the content of the CI configuration file. Note that at present, it's not saving the content to a file anywhere, so `content` only works with `--output term`.
+Roadmap
+-------
 
-We're just starting to look at the CI config itself so we can crawl the `include` content. To list the `include` content from the base CI configuration files:
+We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
-```bash
-python -m labcrawler --query includes
-```
+- Put all these roadmap items into GitLab issues for visibility and sharing
+- Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
+- Fix everything to use the `logger` instead of `print()`.
+- Add a command (`labcrawler info`?) to get e.g. locations of config and output files.
+- Load information about [external main CI configuration files](https://docs.gitlab.com/ee/ci/pipelines/settings.html#specify-a-custom-cicd-configuration-file)
+- Load information about external included CI configuration files
+- Load CI configuration includes recursively, so if an included CI config includes another one, it's loaded also
+- Pull committer information for included and external CI configuration files
+- "Crawl" through subgroups at the beginning, to get all the groups and projects within a portfolio
+- Add one command to combine `crawl`, `melt`, and `load`
+- Enable designation of groups and/or projects as options in the CLI
+- Provide a Dockerfile for easy deployment
+- Set it up to run inside GitLab CI
+- Integrate with Jupyter Notebook to make querying easier
+- Generate useful reports (in GitLab Pages? Conflucence?)
+- Read the CI configuration and smartly explain what it includes
+- Add (in reports, analysis, Jupyter, etc) clear explanations of what each field means (so users new to GitLab can understand more quickly)
+- Provide a test bed for LabCrawler itself, including a GitLab instance with test groups/projects
+- Contribute some or all of LabCrawler's custom queries back to tap-gitlab
 
 Troubleshooting
 ---------------
 
-If some data isn't loading, you might have the wrong scope on your access token. Try this to see your token's scope(s):
+If the `load` command seems to fail, try querying the GitLab API directly. The shell commands below assume that your token is already in the `GITLAB_PRIVATE_TOKEN` environment variable.
+
+To make sure you can connect, and see the towen's user information:
 
 ``` bash
-source .env
 curl --request GET --header "PRIVATE-TOKEN: $GITLAB_PRIVATE_TOKEN" "$GITLAB_API_URL/api/v4/personal_access_tokens/self"
 ```
 
-Not getting any CI config committers? Seems like a bug. 
-
  Here's how to look up the raw blame data using CURL. You *might* need to replace `.gitlab-ci.yml` with the actual path to the CI configuration file, and you also might need to change the `ref` to the default branch.
 
 ``` bash
-source .env
 curl --request GET --header "PRIVATE-TOKEN: $GITLAB_PRIVATE_TOKEN" "$GITLAB_API_URL/api/v4/projects/<id>/repository/files/.gitlab-ci.yml/blame?ref=master"
 ```
 
-FInally, here's a crude API-driven way to list the files and directories at the root of a project:
+Finally, here's a crude API-driven way to list the files and directories at the root of a project:
 
 ``` bash
-source .env
 curl --request GET --header "PRIVATE-TOKEN: $GITLAB_PRIVATE_TOKEN" "$GITLAB_API_URL/api/v4/projects/<id>/repository/tree?per_page=999"
 ```
 
 Useful links
 ------------
 
 [Meltano tutorial](https://docs.meltano.com/getting-started/)
@@ -192,17 +237,7 @@
 
 [tap-gitlab on GitHub](https://github.com/MeltanoLabs/tap-gitlab)
 
 [GitLab API docs](https://docs.gitlab.com/ee/api/)
 
 [Pandas DataFrame reference](https://pandas.pydata.org/docs/reference/frame.html)
 
-
-Handy commands
---------------
-
-To uninstall everything installed by PIP (not Meltano plugins or `pipx` installs):
-
-```
-pip uninstall -y -r <(pip freeze)
-```
-
```

### Comparing `labcrawler-0.4.2/labcrawler/_legacy.py` & `labcrawler-1.0.0/labcrawler/_legacy.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler/analysis.py` & `labcrawler-1.0.0/labcrawler/analysis.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler/cli.py` & `labcrawler-1.0.0/labcrawler/cli.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler/gitlab_ci_config.py` & `labcrawler-1.0.0/labcrawler/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-1.0.0/labcrawler/gitlab_ci_data_loader.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler/gitlab_repository_files_extractor.py` & `labcrawler-1.0.0/labcrawler/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler/templates/meltano.yml` & `labcrawler-1.0.0/labcrawler/templates/meltano.yml`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/labcrawler.egg-info/PKG-INFO` & `labcrawler-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 0.4.2
+Version: 1.0.0
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -59,43 +59,98 @@
 
 The workspace should be good for the life of LabCrawler, though in rare cases a LabCrawler upgrade might require you to recreate it, so check the release notes when upgrading.
 
 The output from the `init` command includes the location of the LabCrawler config file (`labcrawler.json`). Edit the file with the following information:
 
 - `api_url` - URL to the root of the GitLab API, including `https://`.
 - `groups` - All the groups containing projects that you wish to examine. LabCrawler will not examine subgroups, so include them too.
-- `output_dir` - Directory to store the CSV files that are generated; the default is a logical location based on the OS and might be sufficient.
+- `output_dir` - Directory to store the CSV files that are generated; the default is based on the OS and might be sufficient.
 
-Use
----
+*TODO: Note about the GitLab private token*
 
-LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in `labcrawler analyze` command.
+Meltano loading
+---------------
+
+LabCrawler loads data from the GitLab API into CSV files, which can then be examined using a spreadsheet application, independent script, or LabCrawler's built-in analyzer.
+
+Generating the CSV files requires two phases: `melt` and `load`.
 
-Generating the CSV files requires two phases:
+To run the Meltano load, issue the following command:
+
+```
+labcrawler melt
+```
 
-- `labcrawler melt` - Load all the data that is handled directly by Meltano. The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation] to understand the fields. Data loaded includes:
+The CSV files generated by Meltano will contain the verbatim fields from the GitLab REST API, so refer to the [GitLab API Documentation](https://docs.gitlab.com/ee/api/api_resources.html) to understand the fields. Data loaded includes:
     - `groups`
     - `projects`
     - `branches`
     - `merge_requests`
     - `project_members`
     - `group_members`
     - `users`
-- `labcrawler load` - Load LabCrawler-specific data, include CI configuration includes and committers. Data loaded includes:
-    - `ci_config_committers` - Names and email addresses of developers who have committed changes to the main GitLab CI configuration file in each project's repo. The location of the CI configuration file might be from the `ci_config_path` setting on the project, or it's `.gitlab-ci.yml`. Committer information comes from the `git blame` command so only includes the last developer to touch each line of the configuration.
-    - `ci_config_includes` - 
 
-    *TODO: Leftoff here*
+CI configuration data loading
+-----------------------------
+
+To load LabCrawler-specific data, include CI configuration includes and committers, issue the following command:
+
+```
+labcrawler load
+```
+
+The `load` command includes queries specific to GitLab CI configuration files, which are not covered by the Meltano tap.
+
+LabCrawler looks at each project's main GitLab CI configuration file. The default file is at the repo root with the name `.gitlab-ci.yml`, but the location can be overridden by the project maintainers, in which case it's read from the `ci_config_path` setting at the project level. Since `ci_config_path` is now loaded by the Meltano tap, LabCrawler uses that information to query about the correct file.
+
+At this point, the main GitLab CI configuration file is the only file for which LabCrawler loads file-specific information.
+
+The `load` phase loads two specific types of information:
+
+- *includes* - Paths to other GitLab CI configuration files from the same repo that are loaded into the main CI configuration file using the `include:` key. Useful to know where all the CI configuration lives, so it can be easily inspected.
+- *committers* - Names and email addresses of developers who committed the most recent change to at least one line of the main CI configuration file, as per the `git blame` command. Useful to know who has touched CI configuratoin most recently, so they can be easily questioned.
+
+*Understanding includes*
+
+To list the "includes", LabCrawler downloads the CI configuration file itself from the default branch, parses the YAML, and identifies the `include:` key if it exists. The idea is to help understand where more CI configuration lives inside the project.
+
+[The `include:` key](https://docs.gitlab.com/ee/ci/yaml/includes.html) has some power, including the ability to include templates (shipped with GitLab itself) and CI configuration files from other projects and even from URLs outside of the GitLab instance. LabCrawler only lists local includes - that is, other CI configuration files in the same project that are used by the main CI configuration file.
+
+*Understanding committers*
+
+LabCralwer's "committers" list is based on the output from a [GitLab API call](https://docs.gitlab.com/ee/api/repository_files.html#get-file-blame-from-repository) that emulates the [`git blame`](https://www.atlassian.com/git/tutorials/inspecting-a-repository/git-blame) command.
+
+Git differentiates between the author of a commit and the committer, both of which are stored by name and email address within the repo based on the developer's local configuration settings. Authors and committers are not authenticated by Git itself on the desktop.
+
+A push to GitLab might contain one or more commits. GitLab requires authentication and authorization for every push, and records the user who made the push in the database. Optionally, a pre-receive hook can be set up to confirm that the committers (inside the repo data) are authorized users. It's also possible to require signed commits. But GitLab has no way to authenticate the committers themselves, who might have committed code offline.
+
+So within the GitLab API, committer information comes from the Git repo itself, not from the users table. LabCrawler doesn't check other project-level configuration (such as push rules and the signed commit requirement) when reporting committer data. The discrepancy can result in surprises, such as commits by people not authorized to push to the repo, or even employees from other companies (or GitLab itself) showing up as committers.
+
+To investigate why an unknown committer appears in the committers data, use the GitLab web UI. Navigate to the project in question, identify the CI configuration file, and click the "Blame" button. You'll be able to see exactly which lines of code were touched by each committer, and with what commit message. It's also possible to use the "History" button to see the history of all commits to the file.
+
+Note that LabCrawler simply extracts the committers themselves from the API output, and discards the detailed information about which line each developer committed.
+
+*TODO: Note about only loading one project's data*
 
 Analysis
 --------
 
-Then you may examine the results using `pandas` in the Python shell. We've provided a useful way to do so with the `analyze` script. To run it, type:
+LabCrawler generates simple CSV files in the output directory, which can be opened using Microsoft Excel or any other CSV application. Also, LabCrawler offers an easy-to-use analysis prompt based on `pandas`. To use the analysis:
+
+```
+labcrawler analyze
+```
+
+The above command:
+
+1. Reads the CSV file data into Pandas DataFrames (called "raw)
+2. Joins raw DataFrames into slightly-more-useful DataFrames with specific names for each datatype
+3. Outputs how many rows are in each DataFrame, with the variable name for each
+4. Starts a Python command-line Python interpreter for querying the resulting DataFrames using Pandas operations
 
-The above command will run the `analyze` script, which loads the CSV file data into Pandas. It then starts the command-line Python interpreter so you may experiment with the values. Before opening the shell, it lists the objects that are present. Try some of these:
 
 ``` python
 
 # See what columns are available in any table
 projects.columns
 
 # View just certain columns from a table
@@ -131,59 +186,59 @@
 
 If you want to see all of the rows when performing queries, rather than just a sample, try:
 
 ``` python
 pandas.set_option('display.max_rows', None)
 ```
 
-Extracting CI Config information
---------------------------------
-
-There is a mechanism for extracting CI configuration information from GitLab which is separate from Meltano. The `run-extract` command uses it, but by calling it directly you can troubleshoot issues and read the CI config file itself.
-
-``` bash
-source .env
-python -m labcrawler.ci_config_extractor
-```
-
-There are two options for the above command:
-
-- `--project <id>` allows you to specify an individual project ID, so it won't pull all of the data if things are malfunctioning.
-- `--output file` will save the data to `output/ci_config_committers.csv` same as in the `./run-extract` command.
-- `--query content` will dump the content of the CI configuration file. Note that at present, it's not saving the content to a file anywhere, so `content` only works with `--output term`.
+Roadmap
+-------
 
-We're just starting to look at the CI config itself so we can crawl the `include` content. To list the `include` content from the base CI configuration files:
+We maintain an informal roadmap of future functionality. Development of such functionality depends on contributions from the community, a generous donation, or us simply finding the time ;-).
 
-```bash
-python -m labcrawler --query includes
-```
+- Put all these roadmap items into GitLab issues for visibility and sharing
+- Fix the bug where users are being loaded into the CSV multiple times (possible Meltano tap-gitlab fix?)
+- Fix everything to use the `logger` instead of `print()`.
+- Add a command (`labcrawler info`?) to get e.g. locations of config and output files.
+- Load information about [external main CI configuration files](https://docs.gitlab.com/ee/ci/pipelines/settings.html#specify-a-custom-cicd-configuration-file)
+- Load information about external included CI configuration files
+- Load CI configuration includes recursively, so if an included CI config includes another one, it's loaded also
+- Pull committer information for included and external CI configuration files
+- "Crawl" through subgroups at the beginning, to get all the groups and projects within a portfolio
+- Add one command to combine `crawl`, `melt`, and `load`
+- Enable designation of groups and/or projects as options in the CLI
+- Provide a Dockerfile for easy deployment
+- Set it up to run inside GitLab CI
+- Integrate with Jupyter Notebook to make querying easier
+- Generate useful reports (in GitLab Pages? Conflucence?)
+- Read the CI configuration and smartly explain what it includes
+- Add (in reports, analysis, Jupyter, etc) clear explanations of what each field means (so users new to GitLab can understand more quickly)
+- Provide a test bed for LabCrawler itself, including a GitLab instance with test groups/projects
+- Contribute some or all of LabCrawler's custom queries back to tap-gitlab
 
 Troubleshooting
 ---------------
 
-If some data isn't loading, you might have the wrong scope on your access token. Try this to see your token's scope(s):
+If the `load` command seems to fail, try querying the GitLab API directly. The shell commands below assume that your token is already in the `GITLAB_PRIVATE_TOKEN` environment variable.
+
+To make sure you can connect, and see the towen's user information:
 
 ``` bash
-source .env
 curl --request GET --header "PRIVATE-TOKEN: $GITLAB_PRIVATE_TOKEN" "$GITLAB_API_URL/api/v4/personal_access_tokens/self"
 ```
 
-Not getting any CI config committers? Seems like a bug. 
-
  Here's how to look up the raw blame data using CURL. You *might* need to replace `.gitlab-ci.yml` with the actual path to the CI configuration file, and you also might need to change the `ref` to the default branch.
 
 ``` bash
-source .env
 curl --request GET --header "PRIVATE-TOKEN: $GITLAB_PRIVATE_TOKEN" "$GITLAB_API_URL/api/v4/projects/<id>/repository/files/.gitlab-ci.yml/blame?ref=master"
 ```
 
-FInally, here's a crude API-driven way to list the files and directories at the root of a project:
+Finally, here's a crude API-driven way to list the files and directories at the root of a project:
 
 ``` bash
-source .env
 curl --request GET --header "PRIVATE-TOKEN: $GITLAB_PRIVATE_TOKEN" "$GITLAB_API_URL/api/v4/projects/<id>/repository/tree?per_page=999"
 ```
 
 Useful links
 ------------
 
 [Meltano tutorial](https://docs.meltano.com/getting-started/)
@@ -192,17 +247,7 @@
 
 [tap-gitlab on GitHub](https://github.com/MeltanoLabs/tap-gitlab)
 
 [GitLab API docs](https://docs.gitlab.com/ee/api/)
 
 [Pandas DataFrame reference](https://pandas.pydata.org/docs/reference/frame.html)
 
-
-Handy commands
---------------
-
-To uninstall everything installed by PIP (not Meltano plugins or `pipx` installs):
-
-```
-pip uninstall -y -r <(pip freeze)
-```
-
```

### Comparing `labcrawler-0.4.2/labcrawler.egg-info/SOURCES.txt` & `labcrawler-1.0.0/labcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/pyproject.toml` & `labcrawler-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.2/test/test_gitlab_ci_config.py` & `labcrawler-1.0.0/test/test_gitlab_ci_config.py`

 * *Files identical despite different names*

