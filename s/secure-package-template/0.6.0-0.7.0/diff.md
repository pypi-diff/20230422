# Comparing `tmp/secure_package_template-0.6.0.tar.gz` & `tmp/secure_package_template-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jan 10 15:36:16 2023, max compression
+gzip compressed data, last modified: Sat Apr 22 19:15:07 2023, max compression
```

## Comparing `secure_package_template-0.6.0.tar` & `secure_package_template-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1431 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0       63 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/src/secure_package_template/__init__.py
--rw-r--r--   0        0        0       22 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/src/secure_package_template/_version.py
--rw-r--r--   0        0        0        0 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/src/secure_package_template/py.typed
--rw-r--r--   0        0        0     3079 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/.gitignore
--rw-r--r--   0        0        0     1147 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/LICENSE
--rw-r--r--   0        0        0    13024 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/README.md
--rw-r--r--   0        0        0      895 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    14636 2023-01-10 15:36:16.000000 secure_package_template-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1756 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0       63 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/src/secure_package_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/src/secure_package_template/_version.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/src/secure_package_template/py.typed
+-rw-r--r--   0        0        0     3079 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1147 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/LICENSE
+-rw-r--r--   0        0        0    15497 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/README.md
+-rw-r--r--   0        0        0      895 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    17109 2023-04-22 19:15:07.000000 secure_package_template-0.7.0/PKG-INFO
```

### Comparing `secure_package_template-0.6.0/CHANGELOG.md` & `secure_package_template-0.7.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # Changelog
 <!-- scriv-insert-here -->
 
+<a id='changelog-0.7.0'></a>
+## 0.7.0 (2023-04-22)
+
+### Added
+
+- Added instructions on how to configure a Trusted Publisher.
+
 <a id='changelog-0.6.0'></a>
 ## 0.6.0 (2023-01-10)
 
 ### Added
 
 - Added the `repo_token` parameter to the `ossf/scorecard-action` GitHub Action.
 
 - Added documentation on how to upgrade dependencies in lock files manually with `pip-compile` and the `--upgrade-package` option.
 
 ### Changed
 
 - Changed Dependabot configuration to reduce the total number of opened pull requests without sacrificing timely security fixes or upgrades signalling a new major version.
 
-- Changed the build job to forward `PYPI_TOKEN` to the publish job
-  via `GITHUB_OUTPUT` to avoid needing to approve multiple environment
-  runs in one release.
+- Changed the `publish` job to only use the `publish` GitHub Environment, rather than both `publish` and `build` jobs.
+  This means that there will only be one approval required to publish to PyPI since all other steps before can either be
+  rolled back without harming users (ie deleting GitHub releases, git tags) or are idempotent (provenance attestation).
 
 <a id='changelog-0.5.0'></a>
 ## 0.5.0 (2022-12-10)
 
 ### Added
 
 - Added instructions for configuring signed commits and tags automatically from git.
```

### Comparing `secure_package_template-0.6.0/.gitignore` & `secure_package_template-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.6.0/LICENSE` & `secure_package_template-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.6.0/README.md` & `secure_package_template-0.7.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,20 @@
   - Automated publishing to PyPI
   - Code quality and vulnerability scanning
   - Build reproducibility
   - Releases with provenance attestation
 - Obtain a perfect rating from [OpenSSF Scorecard](https://github.com/ossf/scorecard)
 - [SLSA Level 3](https://slsa.dev) using GitHub OIDC
 
-## Configuring git
+## Configuring git for commit and tag signing
+
+> **Info**
+> Commit and tag signing is a practice that's recommended to avoid commit author spoofing
+> but isn't strictly required for a secure project configuration.
+> If you'd like to skip this step, you can jump ahead to [creating a GitHub repository](https://github.com/sethmlarson/secure-python-package-template/#creating-the-github-repository).
 
 Git needs to be configured to be able to sign commits and tags. Git uses GPG for signing, so you need to
 [create a GPG key](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)
 if you don't have one already. Make sure you use a [email address associated with your GitHub account](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)
 as the email address for the key. If you wish to keep your email address private you should use GitHub's provided `noreply` email address.
 
 ```sh
@@ -146,34 +151,14 @@
 Total 25 (delta 0), reused 0 (delta 0), pack-reused 0
 To ssh://github.com/sethmlarson/package-name
  * [new branch]      main -> main
 ```
 
 Success! You should now see the commit and all files on your GitHub repository.
 
-## Configuring PyPI
-
-PyPI is increasing the minimum requirements for account security and credential management to make consuming packages on PyPI more secure. This includes [eventually requiring 2FA for all users and requiring API tokens to publish packages](https://pyfound.blogspot.com/2020/01/start-using-2fa-and-api-tokens-on-pypi.html). Instead of waiting for these best practices to become required we can opt-in to them now.
-
-### Obtain an API token
-
-API tokens will eventually be required for all packages to publish to PyPI.
-
-- Upload a dummy v0.0 package under the desired package name using your PyPI username and password.
-- Create an API token that is scoped to only the package
-- Copy the value into your clipboard, it will be used later (see `PYPI_TOKEN` in the GitHub Environments section below)
-
-### Opt-in to required 2FA
-
-If you don't have 2FA enabled on PyPI already there's a section in the [PyPI Help page](https://pypi.org/help) about how to enable 2FA for your account. To make 2FA required for the new project:
-
-- Open "Your projects" on PyPI
-- Select "Manage" for the project
-- Settings > Enable 2FA requirement for project
-
 ## Configuring the GitHub repository
 
 ### Dependabot
 
 [Dependabot](https://docs.github.com/en/code-security/dependabot) is a service provided by GitHub that keeps your dependencies up-to-date automatically by creating
 pull requests updating individually dependencies on your behalf. Unfortunately, when using Dependabot with any non-trivial number
 of dependencies the number of pull requests quickly becomes too much to handle, especially
@@ -271,14 +256,81 @@
 ### Private vulnerability reporting
 
 - Settings > Code security and analysis
 - Select "Enable" for "Private vulnerability reporting". This will allow
   users to privately submit vulnerability reports directly to the repository.
 - Update the URL in the `SECURITY.md` file to the URL of your own repository.
 
+## Configuring PyPI
+
+PyPI is increasing the minimum requirements for account security and credential management to make consuming packages on PyPI more secure. This includes [eventually requiring 2FA for all users and requiring API tokens to publish packages](https://pyfound.blogspot.com/2020/01/start-using-2fa-and-api-tokens-on-pypi.html). Instead of waiting for these best practices to become required we can opt-in to them now.
+
+### Opt-in to required 2FA
+
+If you don't have 2FA enabled on PyPI already there's a section in the [PyPI Help page](https://pypi.org/help) about how to enable 2FA for your account. To make 2FA required for the new project:
+
+- Open "Your projects" on PyPI
+- Select "Manage" for the project
+- Settings > Enable 2FA requirement for project
+
+### Configuring a Trusted Publisher
+
+If your project is hosted on GitHub you can take advantage of a new PyPI feature called "[Trusted Publishers](https://docs.pypi.org/trusted-publishers/)".
+It's recommended to use a Trusted Publisher over an API key or password because it provides an additional layer of security
+by requiring the package to originate from a pre-configured GitHub repository, workflow, and environment.
+
+There's a [short guide on how to add a Trusted Publisher to the project](https://docs.pypi.org/trusted-publishers/adding-a-publisher/).
+Below is an example of how to map the publishing GitHub Workflow definition to the PyPI Trusted Publisher.
+
+> **Warning**
+> Care should be taken that the publishing workflow can only be triggered
+> by the GitHub accounts that you intend. Remember that git tags (without Protected Tags enabled)
+> only require write access to the repository. This is why GitHub Environments with
+> a set of required reviewers is highly recommended to have an explicit list of
+> people who are allowed to completely execute the publish job.
+
+Configuring the Trusted Publisher requires 4 values:
+
+- GitHub repository owner
+- GitHub repository name
+- GitHub workflow filename
+- GitHub environment name (optional, but highly recommended!)
+
+Using this repository ([https://github.com/sethmlarson/secure-python-package-template](https://github.com/sethmlarson/secure-python-package-template)) as an example, the values to set up a Trusted Publisher would be:
+
+- GitHub repository owner: `sethmlarson`
+- GitHub repository name: `secure-python-package-template`
+- GitHub workflow filename: `publish.yml`
+- GitHub environment name: `publish`
+
+Below is the minimum configurations required from the GitHub Workflow:
+
+```yaml
+# Filename: '.github/workflows/publish.yml'
+# Note that the 'publish.yml' filename doesn't need the '.github/workflows' prefix.
+jobs:
+  publish:
+    # ...
+    permissions:
+      # This permission allows for the gh-action-pypi-publish
+      # step to access GitHub OpenID Connect tokens.
+      id-token: write
+
+    # This job requires the 'publish' GitHub Environment to run.
+    # This value is also set in the Trusted Publisher.
+    environment:
+      name: "publish"
+
+    steps:
+    # - ...
+    # The 'pypa/gh-action-pypi-publish' action reads OpenID Connect
+    # Note that there's zero config below, it's all magically handled!
+    - uses: "pypa/gh-action-pypi-publish@0bf742be3ebe032c25dd15117957dc15d0cfc38d"
+```
+
 ## Verifying configurations
 
 ### Verifying reproducible builds
 
 Find the latest release that was done via the publish GitHub Environment, I used [v0.1.0](https://github.com/sethmlarson/python-package-template/runs/7163956796?check_suite_focus=true)
 for this example.
 
@@ -294,15 +346,15 @@
 
 Check out the corresponding git tag.
 
 ```sh
 git checkout v0.1.0
 ```
 
-Run below command and export the stored value into `SOURCE_DATE_EPOCH`..
+Run below command and export the stored value into `SOURCE_DATE_EPOCH`:
 
 ```sh
 $ git log -1 --pretty=%ct
 1656789393
 
 $ export SOURCE_DATE_EPOCH=1656789393
 ```
```

### Comparing `secure_package_template-0.6.0/pyproject.toml` & `secure_package_template-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `secure_package_template-0.6.0/PKG-INFO` & `secure_package_template-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_package_template
-Version: 0.6.0
+Version: 0.7.0
 Summary: Template for a Python package with a secure project host and package repository configuration.
 Project-URL: Source, https://github.com/sethmlarson/secure-python-package-template
 Author-email: Seth Michael Larson <sethmichaellarson@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.
         
@@ -30,15 +30,20 @@
   - Automated publishing to PyPI
   - Code quality and vulnerability scanning
   - Build reproducibility
   - Releases with provenance attestation
 - Obtain a perfect rating from [OpenSSF Scorecard](https://github.com/ossf/scorecard)
 - [SLSA Level 3](https://slsa.dev) using GitHub OIDC
 
-## Configuring git
+## Configuring git for commit and tag signing
+
+> **Info**
+> Commit and tag signing is a practice that's recommended to avoid commit author spoofing
+> but isn't strictly required for a secure project configuration.
+> If you'd like to skip this step, you can jump ahead to [creating a GitHub repository](https://github.com/sethmlarson/secure-python-package-template/#creating-the-github-repository).
 
 Git needs to be configured to be able to sign commits and tags. Git uses GPG for signing, so you need to
 [create a GPG key](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)
 if you don't have one already. Make sure you use a [email address associated with your GitHub account](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)
 as the email address for the key. If you wish to keep your email address private you should use GitHub's provided `noreply` email address.
 
 ```sh
@@ -163,34 +168,14 @@
 Total 25 (delta 0), reused 0 (delta 0), pack-reused 0
 To ssh://github.com/sethmlarson/package-name
  * [new branch]      main -> main
 ```
 
 Success! You should now see the commit and all files on your GitHub repository.
 
-## Configuring PyPI
-
-PyPI is increasing the minimum requirements for account security and credential management to make consuming packages on PyPI more secure. This includes [eventually requiring 2FA for all users and requiring API tokens to publish packages](https://pyfound.blogspot.com/2020/01/start-using-2fa-and-api-tokens-on-pypi.html). Instead of waiting for these best practices to become required we can opt-in to them now.
-
-### Obtain an API token
-
-API tokens will eventually be required for all packages to publish to PyPI.
-
-- Upload a dummy v0.0 package under the desired package name using your PyPI username and password.
-- Create an API token that is scoped to only the package
-- Copy the value into your clipboard, it will be used later (see `PYPI_TOKEN` in the GitHub Environments section below)
-
-### Opt-in to required 2FA
-
-If you don't have 2FA enabled on PyPI already there's a section in the [PyPI Help page](https://pypi.org/help) about how to enable 2FA for your account. To make 2FA required for the new project:
-
-- Open "Your projects" on PyPI
-- Select "Manage" for the project
-- Settings > Enable 2FA requirement for project
-
 ## Configuring the GitHub repository
 
 ### Dependabot
 
 [Dependabot](https://docs.github.com/en/code-security/dependabot) is a service provided by GitHub that keeps your dependencies up-to-date automatically by creating
 pull requests updating individually dependencies on your behalf. Unfortunately, when using Dependabot with any non-trivial number
 of dependencies the number of pull requests quickly becomes too much to handle, especially
@@ -288,14 +273,81 @@
 ### Private vulnerability reporting
 
 - Settings > Code security and analysis
 - Select "Enable" for "Private vulnerability reporting". This will allow
   users to privately submit vulnerability reports directly to the repository.
 - Update the URL in the `SECURITY.md` file to the URL of your own repository.
 
+## Configuring PyPI
+
+PyPI is increasing the minimum requirements for account security and credential management to make consuming packages on PyPI more secure. This includes [eventually requiring 2FA for all users and requiring API tokens to publish packages](https://pyfound.blogspot.com/2020/01/start-using-2fa-and-api-tokens-on-pypi.html). Instead of waiting for these best practices to become required we can opt-in to them now.
+
+### Opt-in to required 2FA
+
+If you don't have 2FA enabled on PyPI already there's a section in the [PyPI Help page](https://pypi.org/help) about how to enable 2FA for your account. To make 2FA required for the new project:
+
+- Open "Your projects" on PyPI
+- Select "Manage" for the project
+- Settings > Enable 2FA requirement for project
+
+### Configuring a Trusted Publisher
+
+If your project is hosted on GitHub you can take advantage of a new PyPI feature called "[Trusted Publishers](https://docs.pypi.org/trusted-publishers/)".
+It's recommended to use a Trusted Publisher over an API key or password because it provides an additional layer of security
+by requiring the package to originate from a pre-configured GitHub repository, workflow, and environment.
+
+There's a [short guide on how to add a Trusted Publisher to the project](https://docs.pypi.org/trusted-publishers/adding-a-publisher/).
+Below is an example of how to map the publishing GitHub Workflow definition to the PyPI Trusted Publisher.
+
+> **Warning**
+> Care should be taken that the publishing workflow can only be triggered
+> by the GitHub accounts that you intend. Remember that git tags (without Protected Tags enabled)
+> only require write access to the repository. This is why GitHub Environments with
+> a set of required reviewers is highly recommended to have an explicit list of
+> people who are allowed to completely execute the publish job.
+
+Configuring the Trusted Publisher requires 4 values:
+
+- GitHub repository owner
+- GitHub repository name
+- GitHub workflow filename
+- GitHub environment name (optional, but highly recommended!)
+
+Using this repository ([https://github.com/sethmlarson/secure-python-package-template](https://github.com/sethmlarson/secure-python-package-template)) as an example, the values to set up a Trusted Publisher would be:
+
+- GitHub repository owner: `sethmlarson`
+- GitHub repository name: `secure-python-package-template`
+- GitHub workflow filename: `publish.yml`
+- GitHub environment name: `publish`
+
+Below is the minimum configurations required from the GitHub Workflow:
+
+```yaml
+# Filename: '.github/workflows/publish.yml'
+# Note that the 'publish.yml' filename doesn't need the '.github/workflows' prefix.
+jobs:
+  publish:
+    # ...
+    permissions:
+      # This permission allows for the gh-action-pypi-publish
+      # step to access GitHub OpenID Connect tokens.
+      id-token: write
+
+    # This job requires the 'publish' GitHub Environment to run.
+    # This value is also set in the Trusted Publisher.
+    environment:
+      name: "publish"
+
+    steps:
+    # - ...
+    # The 'pypa/gh-action-pypi-publish' action reads OpenID Connect
+    # Note that there's zero config below, it's all magically handled!
+    - uses: "pypa/gh-action-pypi-publish@0bf742be3ebe032c25dd15117957dc15d0cfc38d"
+```
+
 ## Verifying configurations
 
 ### Verifying reproducible builds
 
 Find the latest release that was done via the publish GitHub Environment, I used [v0.1.0](https://github.com/sethmlarson/python-package-template/runs/7163956796?check_suite_focus=true)
 for this example.
 
@@ -311,15 +363,15 @@
 
 Check out the corresponding git tag.
 
 ```sh
 git checkout v0.1.0
 ```
 
-Run below command and export the stored value into `SOURCE_DATE_EPOCH`..
+Run below command and export the stored value into `SOURCE_DATE_EPOCH`:
 
 ```sh
 $ git log -1 --pretty=%ct
 1656789393
 
 $ export SOURCE_DATE_EPOCH=1656789393
 ```
```

