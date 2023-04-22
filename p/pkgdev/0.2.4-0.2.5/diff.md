# Comparing `tmp/pkgdev-0.2.4.tar.gz` & `tmp/pkgdev-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkgdev-0.2.4.tar", last modified: Sun Nov 27 17:09:37 2022, max compression
+gzip compressed data, was "pkgdev-0.2.5.tar", last modified: Sat Mar 11 17:35:13 2023, max compression
```

## Comparing `pkgdev-0.2.4.tar` & `pkgdev-0.2.5.tar`

### file list

```diff
@@ -1,42 +1,48 @@
--rw-r--r--   0        0        0     1493 2022-11-27 17:08:25.745561 pkgdev-0.2.4/LICENSE
--rw-r--r--   0        0        0      279 2022-11-27 17:08:25.745561 pkgdev-0.2.4/Makefile
--rw-r--r--   0        0        0     5990 2022-11-27 17:08:25.745561 pkgdev-0.2.4/NEWS.rst
--rw-r--r--   0        0        0     1442 2022-11-27 17:08:25.745561 pkgdev-0.2.4/README.rst
--rw-r--r--   0        0        0    15783 2022-11-27 17:09:25.593231 pkgdev-0.2.4/build/sphinx/man/pkgdev.1
--rw-r--r--   0        0        0     5420 2022-11-27 17:08:25.745561 pkgdev-0.2.4/data/share/bash-completion/completions/pkgdev
--rw-r--r--   0        0        0     4044 2022-11-27 17:08:25.745561 pkgdev-0.2.4/data/share/zsh/site-functions/_pkgdev
--rw-r--r--   0        0        0     9894 2022-11-27 17:08:25.745561 pkgdev-0.2.4/doc/conf.py
--rw-r--r--   0        0        0      237 2022-11-27 17:08:25.745561 pkgdev-0.2.4/doc/index.rst
--rw-r--r--   0        0        0     1953 2022-11-27 17:08:25.745561 pkgdev-0.2.4/doc/man/config.rst
--rw-r--r--   0        0        0      297 2022-11-27 17:08:25.745561 pkgdev-0.2.4/doc/man/pkgdev.rst
--rw-r--r--   0        0        0     1479 2022-11-27 17:08:25.745561 pkgdev-0.2.4/py_build.py
--rw-r--r--   0        0        0     1476 2022-11-27 17:08:25.745561 pkgdev-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       43 2022-11-27 17:08:25.745561 pkgdev-0.2.4/src/pkgdev/__init__.py
--rw-r--r--   0        0        0       52 2022-11-27 17:08:25.745561 pkgdev-0.2.4/src/pkgdev/_vendor/__init__.py
--rw-r--r--   0        0        0    59322 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/_vendor/tabulate.py
--rw-r--r--   0        0        0       17 2022-11-27 17:09:37.389910 pkgdev-0.2.4/src/pkgdev/_verinfo.py
--rw-r--r--   0        0        0     5775 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/cli.py
--rw-r--r--   0        0        0     1235 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/const.py
--rw-r--r--   0        0        0      741 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/git.py
--rw-r--r--   0        0        0     5948 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/mangle.py
--rwxr-xr-x   0        0        0     1520 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/__init__.py
--rw-r--r--   0        0        0     1243 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/argparsers.py
--rw-r--r--   0        0        0      272 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/pkgdev.py
--rw-r--r--   0        0        0    32606 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_commit.py
--rw-r--r--   0        0        0     4390 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_manifest.py
--rw-r--r--   0        0        0     9909 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_mask.py
--rw-r--r--   0        0        0     2433 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_push.py
--rw-r--r--   0        0        0     9323 2022-11-27 17:08:25.749561 pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_showkw.py
--rw-r--r--   0        0        0        0 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      521 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/__init__.py
--rw-r--r--   0        0        0     3518 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_cli.py
--rw-r--r--   0        0        0     1889 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_pkgdev.py
--rw-r--r--   0        0        0    43601 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_pkgdev_commit.py
--rw-r--r--   0        0        0     7615 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_pkgdev_manifest.py
--rw-r--r--   0        0        0    13545 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_pkgdev_mask.py
--rw-r--r--   0        0        0     4932 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_pkgdev_push.py
--rw-r--r--   0        0        0     8798 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/scripts/test_pkgdev_showkw.py
--rw-r--r--   0        0        0      909 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/test_git.py
--rw-r--r--   0        0        0     3455 2022-11-27 17:08:25.749561 pkgdev-0.2.4/tests/test_mangle.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 pkgdev-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1493 2023-03-11 17:34:25.225924 pkgdev-0.2.5/LICENSE
+-rw-r--r--   0        0        0      325 2023-03-11 17:34:25.225924 pkgdev-0.2.5/Makefile
+-rw-r--r--   0        0        0     6593 2023-03-11 17:34:25.225924 pkgdev-0.2.5/NEWS.rst
+-rw-r--r--   0        0        0     1442 2023-03-11 17:34:25.225924 pkgdev-0.2.5/README.rst
+-rw-r--r--   0        0        0    23010 2023-03-11 17:35:07.298920 pkgdev-0.2.5/build/sphinx/man/pkgdev.1
+-rw-r--r--   0        0        0     7107 2023-03-11 17:34:25.225924 pkgdev-0.2.5/data/share/bash-completion/completions/pkgdev
+-rw-r--r--   0        0        0     4044 2023-03-11 17:34:25.225924 pkgdev-0.2.5/data/share/zsh/site-functions/_pkgdev
+-rw-r--r--   0        0        0    10034 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/conf.py
+-rw-r--r--   0        0        0      380 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/index.rst
+-rw-r--r--   0        0        0     1953 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/man/config.rst
+-rw-r--r--   0        0        0      297 2023-03-11 17:34:25.225924 pkgdev-0.2.5/doc/man/pkgdev.rst
+-rw-r--r--   0        0        0     1494 2023-03-11 17:34:25.225924 pkgdev-0.2.5/py_build.py
+-rw-r--r--   0        0        0     1541 2023-03-11 17:34:25.225924 pkgdev-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/__init__.py
+-rw-r--r--   0        0        0       71 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/__main__.py
+-rw-r--r--   0        0        0       52 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/_vendor/__init__.py
+-rw-r--r--   0        0        0    59090 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/_vendor/tabulate.py
+-rw-r--r--   0        0        0       17 2023-03-11 17:35:13.035061 pkgdev-0.2.5/src/pkgdev/_verinfo.py
+-rw-r--r--   0        0        0     5912 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/cli.py
+-rw-r--r--   0        0        0     1243 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/const.py
+-rw-r--r--   0        0        0      741 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/git.py
+-rw-r--r--   0        0        0     5948 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/mangle.py
+-rwxr-xr-x   0        0        0     1527 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/__init__.py
+-rw-r--r--   0        0        0     1230 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/argparsers.py
+-rw-r--r--   0        0        0      273 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev.py
+-rw-r--r--   0        0        0    15135 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_bugs.py
+-rw-r--r--   0        0        0    33449 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_commit.py
+-rw-r--r--   0        0        0     4473 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_manifest.py
+-rw-r--r--   0        0        0    10261 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_mask.py
+-rw-r--r--   0        0        0     2445 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_push.py
+-rw-r--r--   0        0        0     9314 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_showkw.py
+-rw-r--r--   0        0        0    11822 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_tatt.py
+-rw-r--r--   0        0        0        0 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/tatt/__init__.py
+-rw-r--r--   0        0        0     4099 2023-03-11 17:34:25.225924 pkgdev-0.2.5/src/pkgdev/tatt/template.sh.jinja
+-rw-r--r--   0        0        0        0 2023-03-11 17:34:25.225924 pkgdev-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      521 2023-03-11 17:34:25.225924 pkgdev-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     3885 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_cli.py
+-rw-r--r--   0        0        0     1888 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev.py
+-rw-r--r--   0        0        0     3957 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_bugs.py
+-rw-r--r--   0        0        0    45229 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_commit.py
+-rw-r--r--   0        0        0     7585 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_manifest.py
+-rw-r--r--   0        0        0    13461 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_mask.py
+-rw-r--r--   0        0        0     4939 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_push.py
+-rw-r--r--   0        0        0     8963 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/scripts/test_pkgdev_showkw.py
+-rw-r--r--   0        0        0      908 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/test_git.py
+-rw-r--r--   0        0        0     3454 2023-03-11 17:34:25.229924 pkgdev-0.2.5/tests/test_mangle.py
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 pkgdev-0.2.5/PKG-INFO
```

### Comparing `pkgdev-0.2.4/LICENSE` & `pkgdev-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.4/NEWS.rst` & `pkgdev-0.2.5/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 =============
 Release Notes
 =============
 
+pkgdev 0.2.5 (2023-03-11)
+-------------------------
+
+**New Features:**
+
+- pkgdev tatt: new tool for package testing (Arthur Zamarin, #109)
+
+- pkgdev bugs: new tool for filing stable bugs (Arthur Zamarin, #113)
+
+  This tool is currently *very experimental* and breakage should be expected.
+  Use very carefully and monitor created bugs!
+
+- commit: use same summary when matching across multiple ebuilds (Arthur
+  Zamarin, #116)
+
+**Fixed bugs:**
+
+- commit: enable ``-e`` usage with ``-M`` or ``-m`` (Arthur Zamarin)
+
+- commit: generate commit title for commit related files only (Arthur Zamarin,
+  #122)
+
 pkgdev 0.2.4 (2022-11-26)
 -------------------------
 
 - commit: don't show disable for python targets that are disabled (Arthur
   Zamarin)
 
 - commit: mention ``-e`` as nice option (Arthur Zamarin)
```

### Comparing `pkgdev-0.2.4/README.rst` & `pkgdev-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.4/build/sphinx/man/pkgdev.1` & `pkgdev-0.2.5/build/sphinx/man/pkgdev.1`

 * *Files 26% similar despite different names*

```diff
@@ -23,285 +23,376 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PKGDEV" "1" "Nov 27, 2022" "0.2.4" "pkgdev"
+.TH "PKGDEV" "1" "Mar 11, 2023" "0.2.5" "pkgdev"
 .SH NAME
 pkgdev \- Wrapper for running commandline scripts.
 .SH SYNOPSIS
 .sp
-pkgdev [\-h] [\-\-version] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] {commit,manifest,mask,push,showkw} ...
+pkgdev [\-h] [\-\-version] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] {bugs,commit,manifest,mask,push,showkw,tatt} ...
 .SH BASE OPTIONS
 .INDENT 0.0
 .TP
-.B  \-h\fP,\fB  \-\-help
+.B \fB\-h, \-\-help\fP
 show this help message and exit
 .TP
-.B  \-\-version
+.B \fB\-\-version\fP
 show this program\(aqs version info and exit
 .TP
-.B  \-\-debug
+.B \fB\-\-debug\fP
 enable debugging checks
 .TP
-.B  \-q\fP,\fB  \-\-quiet
+.B \fB\-q, \-\-quiet\fP
 suppress non\-error messages
 .TP
-.B  \-v\fP,\fB  \-\-verbose
+.B \fB\-v, \-\-verbose\fP
 show verbose output
 .TP
-.BI \-\-color \ BOOLEAN
+.B \fB\-\-color BOOLEAN\fP
 enable/disable color support
 .UNINDENT
 .SH SUBCOMMANDS
+.SS pkgdev bugs \- Automatic bugs filler
+.SS Synopsis
+.sp
+pkgdev bugs [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-\-color BOOLEAN] [\-\-api\-key KEY] [\-\-dot DOT] [\-\-auto\-cc\-arches AUTO_CC_ARCHES] [\-s | \-k] [\-a ARCH] [\-p PROFILE] target [target ...]
+.SS Positional Arguments
+.INDENT 0.0
+.TP
+.B \fBtarget\fP
+extended atom matching of packages
+.UNINDENT
+.SS Options
+.INDENT 0.0
+.TP
+.B \fB\-\-api\-key KEY\fP
+The Bugzilla API key to use for authentication. Used mainly to overcome
+rate limiting done by bugzilla server. This tool doesn\(aqt perform any
+bug editing, just fetching info for the bug.
+.TP
+.B \fB\-\-dot DOT\fP
+path file where to save the graph in dot format
+.TP
+.B \fB\-\-auto\-cc\-arches AUTO_CC_ARCHES\fP
+Comma separated list of email addresses, for which automatically add
+CC\-ARCHES if one of the maintainers matches the email address. If the
+package is maintainer\-needed, always add CC\-ARCHES.
+.TP
+.B \fB\-s, \-\-stablereq\fP
+File stable request bugs
+.TP
+.B \fB\-k, \-\-keywording\fP
+File rekeywording bugs
+.UNINDENT
+.SS Config Options
+.INDENT 0.0
+.TP
+.B \fB\-\-config CONFIG_FILE\fP
+Load custom pkgdev scan settings from a given file.
+.sp
+Note that custom user settings override all other system and repo\-level
+settings.
+.sp
+It\(aqs also possible to disable all types of settings loading by
+specifying an argument of \(aqfalse\(aq or \(aqno\(aq.
+.TP
+.B \fB\-\-domain DOMAIN\fP
+custom pkgcore domain to use for this operation
+.UNINDENT
+.SS Base Options
+.INDENT 0.0
+.TP
+.B \fB\-h, \-\-help\fP
+Show this help message and exit. To get more
+information see the related man page.
+.TP
+.B \fB\-\-debug\fP
+Enable debug checks and show verbose debug output.
+.TP
+.B \fB\-\-color BOOLEAN\fP
+Toggle colored output support. This can be used to forcibly
+enable color support when piping output or other situations
+where stdout is not a tty.
+.UNINDENT
+.SS Arches
+.INDENT 0.0
+.TP
+.B \fB\-a ARCH, \-\-arches ARCH\fP
+Comma separated list of arches to enable and disable.
+.sp
+To specify disabled arches prefix them with \(aq\-\(aq. Note that when
+starting the argument list with a disabled arch an equals sign
+must be used, e.g. \-a=\-arch, otherwise the disabled arch
+argument is treated as an option.
+.sp
+By default all repo defined arches are used; however,
+stable\-related checks (e.g. UnstableOnly) default to the set of
+arches having stable profiles in the target repo.
+.UNINDENT
+.SS Profiles
+.INDENT 0.0
+.TP
+.B \fB\-p PROFILE, \-\-profiles PROFILE\fP
+Comma separated list of profiles to enable and disable for
+scanning. Any profiles specified in this fashion will be the
+only profiles that get scanned, skipping any disabled profiles.
+In addition, if no profiles are explicitly enabled, all
+profiles defined in the target repo\(aqs profiles.desc file will be
+scanned except those marked as experimental (exp).
+.sp
+To specify disabled profiles prefix them with \fB\-\fP which
+removes the from the list of profiles to be considered. Note
+that when starting the argument list with a disabled profile an
+equals sign must be used, e.g.  \fB\-p=\-path/to/profile\fP,
+otherwise the disabled profile argument is treated as an
+option.
+.sp
+The special keywords of \fBstable\fP, \fBdev\fP, \fBexp\fP, and
+\fBdeprecated\fP correspond to the lists of stable, development,
+experimental, and deprecated profiles, respectively. Therefore,
+to only scan all stable profiles pass the \fBstable\fP argument
+to \-\-profiles. Additionally the keyword \fBall\fP can be used to
+scan all defined profiles in the target repo.
+.UNINDENT
 .SS pkgdev commit \- create git commit
 .SS Synopsis
 .sp
-pkgdev commit [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] [\-b BUG] [\-c CLOSES] [\-T NAME:VALUE] [\-n] [\-s [BOOLEAN]] [\-A [BOOLEAN]] [\-\-mangle [BOOLEAN]] [\-\-signoff [BOOLEAN]] [\-d DISTDIR] [\-m MSG | \-M FILE | \-e] [\-u | \-a]
+pkgdev commit [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] [\-b BUG] [\-c CLOSES] [\-T NAME:VALUE] [\-n] [\-s [BOOLEAN]] [\-A [BOOLEAN]] [\-\-mangle [BOOLEAN]] [\-\-signoff [BOOLEAN]] [\-d DISTDIR] [\-m MSG | \-M FILE] [\-e] [\-u | \-a]
 .SS Config Options
 .INDENT 0.0
 .TP
-.BI \-\-config \ CONFIG_FILE
+.B \fB\-\-config CONFIG_FILE\fP
 Load custom pkgdev scan settings from a given file.
 .sp
 Note that custom user settings override all other system and repo\-level
 settings.
 .sp
 It\(aqs also possible to disable all types of settings loading by
 specifying an argument of \(aqfalse\(aq or \(aqno\(aq.
 .TP
-.BI \-\-domain \ DOMAIN
+.B \fB\-\-domain DOMAIN\fP
 custom pkgcore domain to use for this operation
 .UNINDENT
 .SS Base Options
 .INDENT 0.0
 .TP
-.B  \-h\fP,\fB  \-\-help
+.B \fB\-h, \-\-help\fP
 Show this help message and exit. To get more
 information see the related man page.
 .TP
-.B  \-\-debug
+.B \fB\-\-debug\fP
 Enable debug checks and show verbose debug output.
 .TP
-.B  \-q\fP,\fB  \-\-quiet
+.B \fB\-q, \-\-quiet\fP
 Suppress non\-error, informational messages.
 .TP
-.B  \-v\fP,\fB  \-\-verbose
+.B \fB\-v, \-\-verbose\fP
 Increase the verbosity of various output.
 .TP
-.BI \-\-color \ BOOLEAN
+.B \fB\-\-color BOOLEAN\fP
 Toggle colored output support. This can be used to forcibly
-enable color support when piping output or other sitations
+enable color support when piping output or other situations
 where stdout is not a tty.
 .UNINDENT
 .SS Commit Options
 .INDENT 0.0
 .TP
-.BI \-b \ BUG\fR,\fB \ \-\-bug \ BUG
+.B \fB\-b BUG, \-\-bug BUG\fP
 add Bug tag for a given Gentoo or upstream bug
 .TP
-.BI \-c \ CLOSES\fR,\fB \ \-\-closes \ CLOSES
+.B \fB\-c CLOSES, \-\-closes CLOSES\fP
 add Closes tag for a given Gentoo bug or upstream PR URL
-.UNINDENT
-.INDENT 0.0
 .TP
-.B \-T NAME:VALUE, \-\-tag NAME:VALUE
+.B \fB\-T NAME:VALUE, \-\-tag NAME:VALUE\fP
 add commit tag
-.UNINDENT
-.INDENT 0.0
 .TP
-.B  \-n\fP,\fB  \-\-dry\-run
+.B \fB\-n, \-\-dry\-run\fP
 Perform all actions without creating a commit.
-.UNINDENT
-.INDENT 0.0
 .TP
-.B \-s [BOOLEAN], \-\-scan [BOOLEAN]
+.B \fB\-s [BOOLEAN], \-\-scan [BOOLEAN]\fP
 By default, \fBpkgdev commit\fP doesn\(aqt scan for QA errors. This option
 enables using pkgcheck to scan the staged changes for issues, erroring
 out if any failures are found.
 .TP
-.B \-A [BOOLEAN], \-\-ask [BOOLEAN]
+.B \fB\-A [BOOLEAN], \-\-ask [BOOLEAN]\fP
 When running with the \-s/\-\-scan option enabled, \fBpkgdev commit\fP will
 ask for confirmation before creating a commit if it detects failure
 results.
 .TP
-.B \-\-mangle [BOOLEAN]
+.B \fB\-\-mangle [BOOLEAN]\fP
 File mangling automatically modifies the content of relevant staged
 files including updating copyright headers and fixing EOF newlines.
 .sp
 This is performed by default for the gentoo repo, but can be forcibly
 disabled or enabled as required.
 .TP
-.B \-\-signoff [BOOLEAN]
+.B \fB\-\-signoff [BOOLEAN]\fP
 Add a Signed\-off\-by trailer by the committer at the end of the commit
 log message.
 .sp
 For committing to the Gentoo repository, under GLEP\-76, the committer
 shall certify agreement to the Certificate of Origin by adding
 Signed\-off\-by line containing the committer\(aqs legal name.
-.UNINDENT
-.INDENT 0.0
 .TP
-.BI \-d \ DISTDIR\fR,\fB \ \-\-distdir \ DISTDIR
+.B \fB\-d DISTDIR, \-\-distdir DISTDIR\fP
 Use a specified target directory for downloads instead of the
 configured DISTDIR.
 .TP
-.BI \-m \ MSG\fR,\fB \ \-\-message \ MSG
+.B \fB\-m MSG, \-\-message MSG\fP
 Use a given message as the commit message. If multiple \-m options are
 specified, their values are concatenated as separate paragraphs.
 .sp
 Note that the first value will be used for the commit summary and if
 it\(aqs empty then a generated summary will be used if available.
 .TP
-.BI \-M \ FILE\fR,\fB \ \-\-message\-template \ FILE
+.B \fB\-M FILE, \-\-message\-template FILE\fP
 Use content from the given file as a commit message template. The
 commit summary prefix \(aq
 .nf
 *
 .fi
 : \(aq is automatically replaced by a generated
 prefix if one exists for the related staged changes.
 .TP
-.B  \-e\fP,\fB  \-\-edit
-The message taken from command line with \-m, and from automatically
-generated one are usually used as the commit log message unmodified.
-This option lets you further edit the message taken from these sources.
+.B \fB\-e, \-\-edit\fP
+This option will ask git to open the commit message in an editor before
+commit. The git configuration is used to select the editor.
 .TP
-.B  \-u\fP,\fB  \-\-update
+.B \fB\-u, \-\-update\fP
 stage all changed files
 .TP
-.B  \-a\fP,\fB  \-\-all
+.B \fB\-a, \-\-all\fP
 stage all changed/new/removed files
 .UNINDENT
 .SS pkgdev manifest \- update package manifests
 .SS Synopsis
 .sp
 pkgdev manifest [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] [\-d DISTDIR] [\-f] [\-m] [\-\-if\-modified] [\-\-ignore\-fetch\-restricted] [target ...]
 .SS Positional Arguments
 .INDENT 0.0
 .TP
-.B target
+.B \fBtarget\fP
 Packages matching any of these restrictions will have their manifest
 entries updated. If no target is specified a path restriction is
 created based on the current working directory. In other words, if
 \fBpkgdev manifest\fP is run within an ebuild\(aqs directory, all the
 ebuilds within that directory will be manifested.
 .UNINDENT
 .SS Config Options
 .INDENT 0.0
 .TP
-.BI \-\-config \ CONFIG_FILE
+.B \fB\-\-config CONFIG_FILE\fP
 Load custom pkgdev scan settings from a given file.
 .sp
 Note that custom user settings override all other system and repo\-level
 settings.
 .sp
 It\(aqs also possible to disable all types of settings loading by
 specifying an argument of \(aqfalse\(aq or \(aqno\(aq.
 .TP
-.BI \-\-domain \ DOMAIN
+.B \fB\-\-domain DOMAIN\fP
 custom pkgcore domain to use for this operation
 .UNINDENT
 .SS Base Options
 .INDENT 0.0
 .TP
-.B  \-h\fP,\fB  \-\-help
+.B \fB\-h, \-\-help\fP
 Show this help message and exit. To get more
 information see the related man page.
 .TP
-.B  \-\-debug
+.B \fB\-\-debug\fP
 Enable debug checks and show verbose debug output.
 .TP
-.B  \-q\fP,\fB  \-\-quiet
+.B \fB\-q, \-\-quiet\fP
 Suppress non\-error, informational messages.
 .TP
-.B  \-v\fP,\fB  \-\-verbose
+.B \fB\-v, \-\-verbose\fP
 Increase the verbosity of various output.
 .TP
-.BI \-\-color \ BOOLEAN
+.B \fB\-\-color BOOLEAN\fP
 Toggle colored output support. This can be used to forcibly
-enable color support when piping output or other sitations
+enable color support when piping output or other situations
 where stdout is not a tty.
 .UNINDENT
 .SS Manifest Options
 .INDENT 0.0
 .TP
-.BI \-d \ DISTDIR\fR,\fB \ \-\-distdir \ DISTDIR
+.B \fB\-d DISTDIR, \-\-distdir DISTDIR\fP
 Use a specified target directory for downloads instead of the
 configured DISTDIR.
 .TP
-.B  \-f\fP,\fB  \-\-force
+.B \fB\-f, \-\-force\fP
 Force package manifest files to be rewritten. Note that this requires
 downloading all distfiles.
 .TP
-.B  \-m\fP,\fB  \-\-mirrors
+.B \fB\-m, \-\-mirrors\fP
 Enable checking Gentoo mirrors first for distfiles. This is disabled by
 default because manifest generation is often performed when adding new
 ebuilds with distfiles that aren\(aqt on Gentoo mirrors yet.
 .TP
-.B  \-\-if\-modified
+.B \fB\-\-if\-modified\fP
 In addition to matching the specified restriction, restrict to targets
 which are marked as modified by git, including untracked files.
 .TP
-.B  \-\-ignore\-fetch\-restricted
+.B \fB\-\-ignore\-fetch\-restricted\fP
 Ignore attempting to update manifest entries for ebuilds which are
 fetch restricted.
 .UNINDENT
 .SS pkgdev mask \- mask packages
 .SS Synopsis
 .sp
 pkgdev mask [\-h] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] [\-r [DAYS]] [\-b BUGS] [\-\-email] [TARGET ...]
 .SS Positional Arguments
 .INDENT 0.0
 .TP
-.B TARGET
+.B \fBTARGET\fP
 Packages matching any of these restrictions will have a mask entry in
 profiles/package.mask added for them. If no target is specified a path
 restriction is created based on the current working directory. In other
 words, if \fBpkgdev mask\fP is run within an ebuild\(aqs directory, all the
 ebuilds within that directory will be masked.
 .UNINDENT
 .SS Base Options
 .INDENT 0.0
 .TP
-.B  \-h\fP,\fB  \-\-help
+.B \fB\-h, \-\-help\fP
 Show this help message and exit. To get more
 information see the related man page.
 .TP
-.B  \-\-debug
+.B \fB\-\-debug\fP
 Enable debug checks and show verbose debug output.
 .TP
-.B  \-q\fP,\fB  \-\-quiet
+.B \fB\-q, \-\-quiet\fP
 Suppress non\-error, informational messages.
 .TP
-.B  \-v\fP,\fB  \-\-verbose
+.B \fB\-v, \-\-verbose\fP
 Increase the verbosity of various output.
 .TP
-.BI \-\-color \ BOOLEAN
+.B \fB\-\-color BOOLEAN\fP
 Toggle colored output support. This can be used to forcibly
-enable color support when piping output or other sitations
+enable color support when piping output or other situations
 where stdout is not a tty.
 .UNINDENT
 .SS Mask Options
 .INDENT 0.0
 .TP
-.B \-r [DAYS], \-\-rites [DAYS]
+.B \fB\-r [DAYS], \-\-rites [DAYS]\fP
 Mark a mask entry for last rites. This defaults to 30 days until
 package removal but accepts an optional argument for the number of
 days.
-.UNINDENT
-.INDENT 0.0
 .TP
-.BI \-b \ BUGS\fR,\fB \ \-\-bug \ BUGS
+.B \fB\-b BUGS, \-\-bug BUGS\fP
 Add a reference to a bug in the mask comment. May be specified multiple
 times to reference multiple bugs.
 .TP
-.B  \-\-email
+.B \fB\-\-email\fP
 Spawn user\(aqs preferred email composer with a prepared email for
 sending a last rites message to Gentoo\(aqs mailing list (\fBgentoo\-dev\fP
 and \fBgentoo\-dev\-announce\fP). The user should manually set the Reply\-to
 field for the message to be accepted by \fBgentoo\-dev\-announce\fP\&.
 .sp
 For spawning the preferred email composer, the \fBxdg\-email\fP tool from
 \fBx11\-misc/xdg\-utils\fP package.
@@ -309,143 +400,262 @@
 .SS pkgdev push \- run QA checks on commits and push them
 .SS Synopsis
 .sp
 pkgdev push [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] [\-A [BOOLEAN]] [\-n] [\-\-pull]
 .SS Config Options
 .INDENT 0.0
 .TP
-.BI \-\-config \ CONFIG_FILE
+.B \fB\-\-config CONFIG_FILE\fP
 Load custom pkgdev scan settings from a given file.
 .sp
 Note that custom user settings override all other system and repo\-level
 settings.
 .sp
 It\(aqs also possible to disable all types of settings loading by
 specifying an argument of \(aqfalse\(aq or \(aqno\(aq.
 .TP
-.BI \-\-domain \ DOMAIN
+.B \fB\-\-domain DOMAIN\fP
 custom pkgcore domain to use for this operation
 .UNINDENT
 .SS Base Options
 .INDENT 0.0
 .TP
-.B  \-h\fP,\fB  \-\-help
+.B \fB\-h, \-\-help\fP
 Show this help message and exit. To get more
 information see the related man page.
 .TP
-.B  \-\-debug
+.B \fB\-\-debug\fP
 Enable debug checks and show verbose debug output.
 .TP
-.B  \-q\fP,\fB  \-\-quiet
+.B \fB\-q, \-\-quiet\fP
 Suppress non\-error, informational messages.
 .TP
-.B  \-v\fP,\fB  \-\-verbose
+.B \fB\-v, \-\-verbose\fP
 Increase the verbosity of various output.
 .TP
-.BI \-\-color \ BOOLEAN
+.B \fB\-\-color BOOLEAN\fP
 Toggle colored output support. This can be used to forcibly
-enable color support when piping output or other sitations
+enable color support when piping output or other situations
 where stdout is not a tty.
 .UNINDENT
 .SS Push Options
 .INDENT 0.0
 .TP
-.B \-A [BOOLEAN], \-\-ask [BOOLEAN]
+.B \fB\-A [BOOLEAN], \-\-ask [BOOLEAN]\fP
 confirm pushing commits with QA errors
-.UNINDENT
-.INDENT 0.0
 .TP
-.B  \-n\fP,\fB  \-\-dry\-run
+.B \fB\-n, \-\-dry\-run\fP
 pretend to push the commits
 .TP
-.B  \-\-pull
+.B \fB\-\-pull\fP
 run \fIgit pull \-\-rebase\fP before scanning
 .UNINDENT
 .SS pkgdev showkw \- show package keywords
 .SS Synopsis
 .sp
 pkgdev showkw [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-q] [\-v] [\-\-color BOOLEAN] [\-f FORMAT] [\-c] [\-s] [\-u] [\-o] [\-p] [\-a ARCH] [\-r REPO] [target ...]
 .SS Positional Arguments
 .INDENT 0.0
 .TP
-.B target
+.B \fBtarget\fP
 extended atom matching of packages
 .UNINDENT
 .SS Config Options
 .INDENT 0.0
 .TP
-.BI \-\-config \ CONFIG_FILE
+.B \fB\-\-config CONFIG_FILE\fP
 Load custom pkgdev scan settings from a given file.
 .sp
 Note that custom user settings override all other system and repo\-level
 settings.
 .sp
 It\(aqs also possible to disable all types of settings loading by
 specifying an argument of \(aqfalse\(aq or \(aqno\(aq.
 .TP
-.BI \-\-domain \ DOMAIN
+.B \fB\-\-domain DOMAIN\fP
 custom pkgcore domain to use for this operation
 .UNINDENT
 .SS Base Options
 .INDENT 0.0
 .TP
-.B  \-h\fP,\fB  \-\-help
+.B \fB\-h, \-\-help\fP
 Show this help message and exit. To get more
 information see the related man page.
 .TP
-.B  \-\-debug
+.B \fB\-\-debug\fP
 Enable debug checks and show verbose debug output.
 .TP
-.B  \-q\fP,\fB  \-\-quiet
+.B \fB\-q, \-\-quiet\fP
 Suppress non\-error, informational messages.
 .TP
-.B  \-v\fP,\fB  \-\-verbose
+.B \fB\-v, \-\-verbose\fP
 Increase the verbosity of various output.
 .TP
-.BI \-\-color \ BOOLEAN
+.B \fB\-\-color BOOLEAN\fP
 Toggle colored output support. This can be used to forcibly
-enable color support when piping output or other sitations
+enable color support when piping output or other situations
 where stdout is not a tty.
 .UNINDENT
 .SS Output Options
 .INDENT 0.0
 .TP
-.BI \-f \ FORMAT\fR,\fB \ \-\-format \ FORMAT
+.B \fB\-f FORMAT, \-\-format FORMAT\fP
 Output table using specified tabular format (defaults to compressed,
 custom format).
 .sp
 Available formats: fancy_grid, fancy_outline, github, grid, html, jira, latex, latex_booktabs, latex_longtable, latex_raw, mediawiki, moinmoin, orgtbl, pipe, plain, presto, pretty, psql, rst, showkw, simple, textile, tsv, unsafehtml, youtrack
 .TP
-.B  \-c\fP,\fB  \-\-collapse
+.B \fB\-c, \-\-collapse\fP
 show collapsed list of arches
 .UNINDENT
 .SS Arch Options
 .INDENT 0.0
 .TP
-.B  \-s\fP,\fB  \-\-stable
+.B \fB\-s, \-\-stable\fP
 show stable arches
 .TP
-.B  \-u\fP,\fB  \-\-unstable
+.B \fB\-u, \-\-unstable\fP
 show unstable arches
 .TP
-.B  \-o\fP,\fB  \-\-only\-unstable
+.B \fB\-o, \-\-only\-unstable\fP
 show arches that only have unstable keywords
 .TP
-.B  \-p\fP,\fB  \-\-prefix
+.B \fB\-p, \-\-prefix\fP
 show prefix and non\-native arches
 .TP
-.BI \-a \ ARCH\fR,\fB \ \-\-arch \ ARCH
+.B \fB\-a ARCH, \-\-arch ARCH\fP
 select arches to display
 .UNINDENT
 .SS Target Options
 .INDENT 0.0
 .TP
-.BI \-r \ REPO\fR,\fB \ \-\-repo \ REPO
+.B \fB\-r REPO, \-\-repo REPO\fP
 repo to query (defaults to all ebuild repos)
 .UNINDENT
+.SS pkgdev tatt \- package testing tool
+.SS Synopsis
+.sp
+pkgdev tatt [\-\-config CONFIG_FILE] [\-\-domain DOMAIN] [\-h] [\-\-debug] [\-\-color BOOLEAN] [\-\-api\-key KEY] [\-j NAME] [\-b BUG] [\-t] [\-u NUMBER] [\-\-ignore\-prefixes IGNORE_PREFIXES] [\-\-use\-default | \-\-use\-random | \-\-use\-expand\-random] [\-p TARGET [TARGET ...]] [\-s | \-k] [\-\-template\-file TEMPLATE_FILE] [\-\-logs\-dir LOGS_DIR] [\-\-emerge\-opts EMERGE_OPTS]
+.SS Options
+.INDENT 0.0
+.TP
+.B \fB\-\-api\-key KEY\fP
+The Bugzilla API key to use for authentication. Used mainly to overcome
+rate limiting done by bugzilla server. This tool doesn\(aqt perform any
+bug editing, just fetching info for the bug.
+.TP
+.B \fB\-j NAME, \-\-job\-name NAME\fP
+The job name to use for the job script and report. The name can use
+the variables \fB{PN}\fP (package name) and \fB{BUGNO}\fP (bug number)
+to created variable names.
+.TP
+.B \fB\-b BUG, \-\-bug BUG\fP
+Single bug to take package list from
+.UNINDENT
+.SS Config Options
+.INDENT 0.0
+.TP
+.B \fB\-\-config CONFIG_FILE\fP
+Load custom pkgdev scan settings from a given file.
+.sp
+Note that custom user settings override all other system and repo\-level
+settings.
+.sp
+It\(aqs also possible to disable all types of settings loading by
+specifying an argument of \(aqfalse\(aq or \(aqno\(aq.
+.TP
+.B \fB\-\-domain DOMAIN\fP
+custom pkgcore domain to use for this operation
+.UNINDENT
+.SS Base Options
+.INDENT 0.0
+.TP
+.B \fB\-h, \-\-help\fP
+Show this help message and exit. To get more
+information see the related man page.
+.TP
+.B \fB\-\-debug\fP
+Enable debug checks and show verbose debug output.
+.TP
+.B \fB\-\-color BOOLEAN\fP
+Toggle colored output support. This can be used to forcibly
+enable color support when piping output or other situations
+where stdout is not a tty.
+.UNINDENT
+.SS Use Flags Options
+.INDENT 0.0
+.TP
+.B \fB\-t, \-\-test\fP
+Include a test run for packages which define \fBsrc_test\fP phase
+(in the ebuild or inherited from eclass).
+.TP
+.B \fB\-u NUMBER, \-\-use\-combos NUMBER\fP
+Maximal number USE combinations to be tested
+.TP
+.B \fB\-\-ignore\-prefixes IGNORE_PREFIXES\fP
+Comma separated USE flags prefixes that won\(aqt be randomized. This is
+useful for USE flags such as \fBpython_targets_\fP\&. Note that this
+doesn\(aqt affect preference, but because of specific REQUIRED_USE will
+still be changed from defaults.
+.TP
+.B \fB\-\-use\-default\fP
+Prefer to use default use flags configuration
+.TP
+.B \fB\-\-use\-random\fP
+Turn on random use flags, with default USE_EXPAND
+.TP
+.B \fB\-\-use\-expand\-random\fP
+Turn on random use flags, including USE_EXPAND
+.UNINDENT
+.SS Manual Packages Options
+.INDENT 0.0
+.TP
+.B \fB\-p TARGET [TARGET ...], \-\-packages TARGET [TARGET ...]\fP
+extended atom matching of packages
+.TP
+.B \fB\-s, \-\-stablereq\fP
+Test packages for stable keywording requests
+.TP
+.B \fB\-k, \-\-keywording\fP
+Test packages for keywording requests
+.UNINDENT
+.SS Template Options
+.INDENT 0.0
+.TP
+.B \fB\-\-template\-file TEMPLATE_FILE\fP
+Template file to use for the job script. The template file is a
+Jinja template file, which can use the following variables:
+.INDENT 7.0
+.TP
+.B \fBjobs\fP
+A list of jobs to be run. Each job is a tuple consisting of
+USE flags values, is a testing job, and the atom to build.
+.TP
+.B \fBreport_file\fP
+The path to the report file.
+.TP
+.B \fBemerge_opts\fP
+Options to be passed to emerge invocations. Taken from
+\fB\-\-emerge\-opts\fP\&.
+.TP
+.B \fBlog_dir\fP
+irectory to save build logs for failing tasks. Taken from
+\fB\-\-logs\-dir\fP\&.
+.TP
+.B \fBcleanup_files\fP
+A list of files to be removed after the job script is done.
+.UNINDENT
+.TP
+.B \fB\-\-logs\-dir LOGS_DIR\fP
+Directory to save build logs for failing tasks
+.TP
+.B \fB\-\-emerge\-opts EMERGE_OPTS\fP
+Space separated single argument, consisting og options to be passed
+to \fBemerge\fP invocations.
+.UNINDENT
 .SH CONFIG FILE SUPPORT
 .sp
 Config files are supported by most subcommands of \fBpkgdev\fP from any of three
 locations. Listed in order of increasing precedence these include the
 following:
 .INDENT 0.0
 .IP \(bu 2
```

### Comparing `pkgdev-0.2.4/data/share/bash-completion/completions/pkgdev` & `pkgdev-0.2.5/data/share/bash-completion/completions/pkgdev`

 * *Files 19% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 source "/usr/share/bash-completion/helpers/gentoo-common.sh"
 
 _pkgdev() {
     local i=1 cmd cur prev words cword split
     _init_completion || return
 
     local subcommands="
+        bugs
         commit
         manifest
         mask
         push
         showkw
+        tatt
     "
 
     local base_options="
         -h --help
         --version
         --debug
         -q --quiet
@@ -190,12 +192,67 @@
                     ;;
                 *)
                     COMPREPLY+=($(compgen -W "${subcmd_options}" -- "${cur}"))
                     COMPREPLY+=($(_list_repo_atoms))
                     ;;
             esac
             ;;
+        tatt)
+            subcmd_options="
+                --api-key
+                -j --job-name
+                -b --bug
+                -t --test
+                -u --use-combos
+                --ignore-prefixes
+                --use-default
+                --use-random
+                --use-expand-random
+                -p --package
+                -s --stablereq
+                -k --keywording
+                --template-file
+                --logs-dir
+                --emerge-opts
+            "
+
+            case "${prev}" in
+                -[jbup] | --api-key | --job-name | --bug | --use-combos | --package | --emerge-opts)
+                    COMPREPLY=()
+                    ;;
+                --template-file)
+                    COMPREPLY=($(compgen -f -- "${cur}"))
+                    ;;
+                --logs-dir)
+                    COMPREPLY=($(compgen -d -- "${cur}"))
+                    ;;
+                *)
+                    COMPREPLY+=($(compgen -W "${subcmd_options}" -- "${cur}"))
+                    ;;
+            esac
+            ;;
+        bugs)
+            subcmd_options="
+                --api-key
+                --auto-cc-arches
+                --dot
+                -s --stablereq
+                -k --keywording
+            "
+
+            case "${prev}" in
+                --api-key | --auto-cc-arches)
+                    COMPREPLY=()
+                    ;;
+                --dot)
+                    COMPREPLY=($(compgen -f -- "${cur}"))
+                    ;;
+                *)
+                    COMPREPLY+=($(compgen -W "${subcmd_options}" -- "${cur}"))
+                    ;;
+            esac
+            ;;
     esac
 }
 complete -F _pkgdev pkgdev
 
 # vim: set ft=bash sw=4 et sts=4 :
```

### Comparing `pkgdev-0.2.4/data/share/zsh/site-functions/_pkgdev` & `pkgdev-0.2.5/data/share/zsh/site-functions/_pkgdev`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.4/doc/conf.py` & `pkgdev-0.2.5/doc/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,312 +12,315 @@
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.autosectionlabel',
-    'sphinx.ext.doctest',
-    'sphinx.ext.extlinks',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.todo',
-    'sphinx.ext.coverage',
-    'sphinx.ext.ifconfig',
-    'sphinx.ext.viewcode',
-    'snakeoil.dist.sphinxext',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.autosectionlabel",
+    "sphinx.ext.doctest",
+    "sphinx.ext.extlinks",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.viewcode",
+    "snakeoil.dist.sphinxext",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-#templates_path = ['_templates']
+# templates_path = ['_templates']
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'pkgdev'
-authors = ''
-copyright = '2021-2022, pkgdev contributors'
+project = "pkgdev"
+authors = ""
+copyright = "2021-2022, pkgdev contributors"
 
 # version is set by snakeoil extension
-release = 'master'
+release = "master"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build', 'generated']
+exclude_patterns = ["_build", "generated"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = "default"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+# html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'pkgdevdoc'
+htmlhelp_basename = "pkgdevdoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  ('index', 'pkgdev.tex', 'pkgdev Documentation',
-   authors, 'manual'),
+    ("index", "pkgdev.tex", "pkgdev Documentation", authors, "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = []
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  ('index', 'pkgdev', 'pkgdev Documentation',
-   authors, 'pkgdev', 'One line description of project.',
-   'Miscellaneous'),
+    (
+        "index",
+        "pkgdev",
+        "pkgdev Documentation",
+        authors,
+        "pkgdev",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # -- Options for Epub output ----------------------------------------------
 
 # Bibliographic Dublin Core info.
 epub_title = project
 epub_author = authors
 epub_publisher = authors
 epub_copyright = copyright
 
 # The basename for the epub file. It defaults to the project name.
-#epub_basename = 'pkgdev'
+# epub_basename = 'pkgdev'
 
 # The HTML theme for the epub output. Since the default themes are not optimized
 # for small screen space, using the same theme for HTML and epub output is
 # usually not wise. This defaults to 'epub', a theme designed to save visual
 # space.
-#epub_theme = 'epub'
+# epub_theme = 'epub'
 
 # The language of the text. It defaults to the language option
 # or en if the language is not set.
-#epub_language = ''
+# epub_language = ''
 
 # The scheme of the identifier. Typical schemes are ISBN or URL.
-#epub_scheme = ''
+# epub_scheme = ''
 
 # The unique identifier of the text. This can be a ISBN number
 # or the project homepage.
-#epub_identifier = ''
+# epub_identifier = ''
 
 # A unique identification for the text.
-#epub_uid = ''
+# epub_uid = ''
 
 # A tuple containing the cover image and cover page html template filenames.
-#epub_cover = ()
+# epub_cover = ()
 
 # A sequence of (type, uri, title) tuples for the guide element of content.opf.
-#epub_guide = ()
+# epub_guide = ()
 
 # HTML files that should be inserted before the pages created by sphinx.
 # The format is a list of tuples containing the path and title.
-#epub_pre_files = []
+# epub_pre_files = []
 
 # HTML files shat should be inserted after the pages created by sphinx.
 # The format is a list of tuples containing the path and title.
-#epub_post_files = []
+# epub_post_files = []
 
 # A list of files that should not be packed into the epub file.
-epub_exclude_files = ['search.html']
+epub_exclude_files = ["search.html"]
 
 # The depth of the table of contents in toc.ncx.
-#epub_tocdepth = 3
+# epub_tocdepth = 3
 
 # Allow duplicate toc entries.
-#epub_tocdup = True
+# epub_tocdup = True
 
 # Choose between 'default' and 'includehidden'.
-#epub_tocscope = 'default'
+# epub_tocscope = 'default'
 
 # Fix unsupported image types using the PIL.
-#epub_fix_images = False
+# epub_fix_images = False
 
 # Scale large images.
-#epub_max_image_width = 0
+# epub_max_image_width = 0
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#epub_show_urls = 'inline'
+# epub_show_urls = 'inline'
 
 # If false, no index is generated.
-#epub_use_index = True
+# epub_use_index = True
```

### Comparing `pkgdev-0.2.4/doc/man/config.rst` & `pkgdev-0.2.5/doc/man/config.rst`

 * *Files identical despite different names*

### Comparing `pkgdev-0.2.4/py_build.py` & `pkgdev-0.2.5/py_build.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from functools import partial
 from pathlib import Path
 
 from flit_core import buildapi
 
 
 def write_verinfo(cleanup_files):
+    from snakeoil.version import get_git_version
+
     cleanup_files.append(path := Path.cwd() / "src/pkgdev/_verinfo.py")
     path.parent.mkdir(parents=True, exist_ok=True)
     print(f"generating version info: {path}")
-    from snakeoil.version import get_git_version
     path.write_text(f"version_info={get_git_version(Path.cwd())!r}")
 
 
 def prepare_pkgcore(callback):
     cleanup_files = []
     try:
         write_verinfo(cleanup_files)
@@ -30,15 +31,17 @@
     """Builds a wheel, places it in wheel_directory"""
     callback = partial(buildapi.build_wheel, wheel_directory, config_settings, metadata_directory)
     return prepare_pkgcore(callback)
 
 
 def build_editable(wheel_directory, config_settings=None, metadata_directory=None):
     """Builds an "editable" wheel, places it in wheel_directory"""
-    callback = partial(buildapi.build_editable, wheel_directory, config_settings, metadata_directory)
+    callback = partial(
+        buildapi.build_editable, wheel_directory, config_settings, metadata_directory
+    )
     return prepare_pkgcore(callback)
 
 
 def build_sdist(sdist_directory, config_settings=None):
     """Builds an sdist, places it in sdist_directory"""
     callback = partial(buildapi.build_sdist, sdist_directory, config_settings)
     return prepare_pkgcore(callback)
```

### Comparing `pkgdev-0.2.4/pyproject.toml` & `pkgdev-0.2.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -24,28 +24,32 @@
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 
 dependencies = [
-	"snakeoil~=0.10.3",
+	"snakeoil~=0.10.4",
 	"pkgcore~=0.12.16",
 	"pkgcheck~=0.10.16",
 ]
 
 [project.optional-dependencies]
 test = [
 	"pytest>=6.0",
 	"pytest-cov",
 ]
 doc = [
 	"sphinx",
 	"tomli; python_version < '3.11'"
 ]
+tatt = [
+	"nattka",
+	"Jinja2",
+]
 
 [project.urls]
 Homepage = "https://github.com/pkgcore/pkgdev"
 Documentation = "https://pkgcore.github.io/pkgdev/"
 Source = "https://github.com/pkgcore/pkgdev"
 
 [project.scripts]
@@ -61,11 +65,14 @@
 	"build/sphinx/man/*.1",
 ]
 exclude = [
 	".github/", ".gitignore",
 	"doc/api/", "doc/generated/", "doc/_build/",
 ]
 
+[tool.black]
+line-length = 100
+
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-vv -ra -l"
 testpaths = ["tests"]
```

### Comparing `pkgdev-0.2.4/src/pkgdev/_vendor/tabulate.py` & `pkgdev-0.2.5/src/pkgdev/_vendor/tabulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         "linebelow",
         "headerrow",
         "datarow",
         "padding",
         "with_header_hide",
         "vertical_headers",
     ],
-    defaults=(False,)
+    defaults=(False,),
 )
 
 
 def _pipe_segment_with_colons(align, colwidth):
     """Return a segment of a horizontal line with optional colons which
     indicate column's alignment (as in `pipe` output format)."""
     w = colwidth
@@ -401,15 +401,16 @@
     "showkw": TableFormat(
         lineabove=None,
         linebelowheader=Line("", "-", "-", ""),
         linebetweenrows=None,
         linebelow=None,
         headerrow=DataRow("", "", ""),
         datarow=DataRow("", "", ""),
-        padding=1, with_header_hide=None,
+        padding=1,
+        with_header_hide=None,
         vertical_headers=True,
     ),
     "mediawiki": TableFormat(
         lineabove=Line(
             '{| class="wikitable" style="text-align: left;"',
             "",
             "",
@@ -658,17 +659,15 @@
     >>> _type('\x1b[31m42\x1b[0m') is type(42)
     True
     >>> _type('\x1b[31m42\x1b[0m') is type(42)
     True
 
     """
 
-    if has_invisible and (
-        isinstance(string, _text_type) or isinstance(string, _binary_type)
-    ):
+    if has_invisible and (isinstance(string, _text_type) or isinstance(string, _binary_type)):
         string = _strip_invisible(string)
 
     if string is None:
         return _none_type
     elif hasattr(string, "isoformat"):  # datetime.datetime, date, and time
         return _text_type
     elif _isbool(string):
@@ -870,33 +869,29 @@
     minwidth=0,
     has_invisible=True,
     enable_widechars=False,
     is_multiline=False,
 ):
     """[string] -> [padded_string]"""
     strings, padfn = _align_column_choose_padfn(strings, alignment, has_invisible)
-    width_fn = _align_column_choose_width_fn(
-        has_invisible, enable_widechars, is_multiline
-    )
+    width_fn = _align_column_choose_width_fn(has_invisible, enable_widechars, is_multiline)
 
     s_widths = list(map(width_fn, strings))
     maxwidth = max(max(_flat_list(s_widths)), minwidth)
     # TODO: refactor column alignment in single-line and multiline modes
     if is_multiline:
         if not enable_widechars and not has_invisible:
             padded_strings = [
-                "\n".join([padfn(maxwidth, s) for s in ms.splitlines()])
-                for ms in strings
+                "\n".join([padfn(maxwidth, s) for s in ms.splitlines()]) for ms in strings
             ]
         else:
             # enable wide-character width corrections
             s_lens = [[len(s) for s in re.split("[\r\n]", ms)] for ms in strings]
             visible_widths = [
-                [maxwidth - (w - l) for w, l in zip(mw, ml)]
-                for mw, ml in zip(s_widths, s_lens)
+                [maxwidth - (w - l) for w, l in zip(mw, ml)] for mw, ml in zip(s_widths, s_lens)
             ]
             # wcswidth and _visible_width don't count invisible characters;
             # padfn doesn't need to apply another correction
             padded_strings = [
                 "\n".join([padfn(w, s) for s, w in zip((ms.splitlines() or ms), mw)])
                 for ms, mw in zip(strings, visible_widths)
             ]
@@ -979,36 +974,30 @@
         return "{0}".format(val)
     elif valtype is _binary_type:
         try:
             return _text_type(val, "ascii")
         except TypeError:
             return _text_type(val)
     elif valtype is float:
-        is_a_colored_number = has_invisible and isinstance(
-            val, (_text_type, _binary_type)
-        )
+        is_a_colored_number = has_invisible and isinstance(val, (_text_type, _binary_type))
         if is_a_colored_number:
             raw_val = _strip_invisible(val)
             formatted_val = format(float(raw_val), floatfmt)
             return val.replace(raw_val, formatted_val)
         else:
             return format(float(val), floatfmt)
     else:
         return "{0}".format(val)
 
 
-def _align_header(
-    header, alignment, width, visible_width, is_multiline=False, width_fn=None
-):
+def _align_header(header, alignment, width, visible_width, is_multiline=False, width_fn=None):
     "Pad string header to width chars given known visible_width of the header."
     if is_multiline:
         header_lines = re.split(_multiline_codes, header)
-        padded_lines = [
-            _align_header(h, alignment, width, width_fn(h)) for h in header_lines
-        ]
+        padded_lines = [_align_header(h, alignment, width, width_fn(h)) for h in header_lines]
         return "\n".join(padded_lines)
     # else: not multiline
     ninvisible = len(header) - visible_width
     width += ninvisible
     if alignment == "left":
         return _padright(width, header)
     elif alignment == "center":
@@ -1079,24 +1068,19 @@
 
     index = None
     if hasattr(tabular_data, "keys") and hasattr(tabular_data, "values"):
         # dict-like and pandas.DataFrame?
         if hasattr(tabular_data.values, "__call__"):
             # likely a conventional dict
             keys = tabular_data.keys()
-            rows = list(
-                zip_longest(*tabular_data.values())
-            )  # columns have to be transposed
+            rows = list(zip_longest(*tabular_data.values()))  # columns have to be transposed
         elif hasattr(tabular_data, "index"):
             # values is a property, has .index => it's likely a pandas.DataFrame (pandas 0.11.0)
             keys = list(tabular_data)
-            if (
-                showindex in ["default", "always", True]
-                and tabular_data.index.name is not None
-            ):
+            if showindex in ["default", "always", True] and tabular_data.index.name is not None:
                 if isinstance(tabular_data.index.name, list):
                     keys[:0] = tabular_data.index.name
                 else:
                     keys[:0] = [tabular_data.index.name]
             vals = tabular_data.values  # values matrix doesn't need to be transposed
             # for DataFrames add an index per default
             index = list(tabular_data.index)
@@ -1152,17 +1136,15 @@
             elif headers == "firstrow":
                 if len(rows) > 0:
                     headers = [firstdict.get(k, k) for k in keys]
                     headers = list(map(_text_type, headers))
                 else:
                     headers = []
             elif headers:
-                raise ValueError(
-                    "headers for a list of dicts is not a dict or a keyword"
-                )
+                raise ValueError("headers for a list of dicts is not a dict or a keyword")
             rows = [[row.get(k) for k in keys] for row in rows]
 
         elif (
             headers == "keys"
             and hasattr(tabular_data, "description")
             and hasattr(tabular_data, "fetchone")
             and hasattr(tabular_data, "rowcount")
@@ -1519,17 +1501,15 @@
     indices is used to disable number parsing only on those columns
     e.g. `disable_numparse=[0, 2]` would disable number parsing only on the
     first and third columns.
     """
 
     if tabular_data is None:
         tabular_data = []
-    list_of_lists, headers = _normalize_tabular_data(
-        tabular_data, headers, showindex=showindex
-    )
+    list_of_lists, headers = _normalize_tabular_data(tabular_data, headers, showindex=showindex)
 
     fmt = tablefmt
     if not isinstance(fmt, TableFormat):
         fmt = _table_formats.get(fmt, _table_formats["simple"])
 
     # empty values in the first column of RST tables should be escaped (issue #82)
     # "" should be escaped as "\\ " or ".."
@@ -1573,17 +1553,15 @@
     width_fn = _choose_width_fn(has_invisible, enable_widechars, is_multiline)
 
     # format rows and columns, convert numeric values to strings
     cols = list(zip_longest(*list_of_lists))
     numparses = _expand_numparse(disable_numparse, len(cols))
     coltypes = [_column_type(col, numparse=np) for col, np in zip(cols, numparses)]
     if isinstance(floatfmt, str):  # old version
-        float_formats = len(cols) * [
-            floatfmt
-        ]  # just duplicate the string to use in each column
+        float_formats = len(cols) * [floatfmt]  # just duplicate the string to use in each column
     else:  # if floatfmt is list, tuple etc we have one per column
         float_formats = list(floatfmt)
         if len(float_formats) < len(cols):
             float_formats.extend((len(cols) - len(float_formats)) * [_DEFAULT_FLOATFMT])
     if isinstance(missingval, str):
         missing_vals = len(cols) * [missingval]
     else:
@@ -1603,36 +1581,39 @@
             aligns[idx] = align
     if not headers:
         minwidths = [0] * len(cols)
     elif fmt.vertical_headers:
         minwidths = [1] * len(cols)
     else:
         minwidths = [width_fn(h) + MIN_PADDING for h in headers]
-    cols = [_align_column(c, a, minw, has_invisible, enable_widechars, is_multiline)
-            for c, a, minw in zip(cols, aligns, minwidths)]
+    cols = [
+        _align_column(c, a, minw, has_invisible, enable_widechars, is_multiline)
+        for c, a, minw in zip(cols, aligns, minwidths)
+    ]
 
     if headers:
         # align headers and add headers
         t_cols = cols or [[""]] * len(headers)
         t_aligns = aligns or [stralign] * len(headers)
-        minwidths = [
-            max(minw, max(width_fn(cl) for cl in c))
-            for minw, c in zip(minwidths, t_cols)]
+        minwidths = [max(minw, max(width_fn(cl) for cl in c)) for minw, c in zip(minwidths, t_cols)]
         if fmt.vertical_headers:
             max_len = max(len(x) for x in headers)
             headers = [x.rjust(max_len) for x in headers]
             headers = [
-                [_align_header(h[i], a, minw, width_fn(h[i])) for h, a, minw
-                 in zip(headers, t_aligns, minwidths)]
+                [
+                    _align_header(h[i], a, minw, width_fn(h[i]))
+                    for h, a, minw in zip(headers, t_aligns, minwidths)
+                ]
                 for i in range(max_len)
             ]
         else:
             headers = [
                 _align_header(h, a, minw, width_fn(h), is_multiline, width_fn)
-                for h, a, minw in zip(headers, t_aligns, minwidths)]
+                for h, a, minw in zip(headers, t_aligns, minwidths)
+            ]
         rows = list(zip(*cols))
     else:
         minwidths = [max(width_fn(cl) for cl in c) for c in cols]
         rows = list(zip(*cols))
 
     return _format_table(fmt, headers, rows, minwidths, aligns, is_multiline)
 
@@ -1683,24 +1664,20 @@
 
 
 def _append_basic_row(lines, padded_cells, colwidths, colaligns, rowfmt):
     lines.append(_build_row(padded_cells, colwidths, colaligns, rowfmt))
     return lines
 
 
-def _append_multiline_row(
-    lines, padded_multiline_cells, padded_widths, colaligns, rowfmt, pad
-):
+def _append_multiline_row(lines, padded_multiline_cells, padded_widths, colaligns, rowfmt, pad):
     colwidths = [w - 2 * pad for w in padded_widths]
     cells_lines = [c.splitlines() for c in padded_multiline_cells]
     nlines = max(map(len, cells_lines))  # number of lines in the row
     # vertically pad cells where some lines are missing
-    cells_lines = [
-        (cl + [" " * w] * (nlines - len(cl))) for cl, w in zip(cells_lines, colwidths)
-    ]
+    cells_lines = [(cl + [" " * w] * (nlines - len(cl))) for cl, w in zip(cells_lines, colwidths)]
     lines_cells = [[cl[i] for cl in cells_lines] for i in range(nlines)]
     for ln in lines_cells:
         padded_ln = _pad_row(ln, pad)
         _append_basic_row(lines, padded_ln, colwidths, colaligns, rowfmt)
     return lines
 
 
@@ -1741,15 +1718,15 @@
     pad = fmt.padding
     headerrow = fmt.headerrow
 
     if fmt.vertical_headers:
         colwidths[0] += 1
         padded_widths = colwidths
     else:
-        padded_widths = [(w + 2*pad) for w in colwidths]
+        padded_widths = [(w + 2 * pad) for w in colwidths]
 
     if is_multiline:
         pad_row = lambda row, _: row  # noqa do it later, in _append_multiline_row
         append_row = partial(_append_multiline_row, pad=pad)
     else:
         pad_row = _pad_row
         append_row = _append_basic_row
```

### Comparing `pkgdev-0.2.4/src/pkgdev/cli.py` & `pkgdev-0.2.5/src/pkgdev/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,25 @@
 from pkgcore.repository import errors as repo_errors
 from pkgcore.util.commandline import _mk_domain
 
 from . import const
 
 
 class Tool(commandline.Tool):
-
     def main(self):
         # suppress all pkgcore log messages
-        logging.getLogger('pkgcore').setLevel(100)
+        logging.getLogger("pkgcore").setLevel(100)
         return super().main()
 
 
 class ConfigArg(argparse._StoreAction):
     """Store config path string or False when explicitly disabled."""
 
     def __call__(self, parser, namespace, values, option_string=None):
-        if values.lower() in ('false', 'no', 'n'):
+        if values.lower() in ("false", "no", "n"):
             values = False
         setattr(namespace, self.dest, values)
 
 
 class ConfigParser(configparser.ConfigParser):
     """ConfigParser with case-sensitive keys (default forces lowercase)."""
 
@@ -58,25 +57,29 @@
         """Parse given config files."""
         configs = configs if configs else self.configs
         config = ConfigParser(default_section=None)
         try:
             for f in configs:
                 config.read(f)
         except configparser.ParsingError as e:
-            self.parser.error(f'parsing config file failed: {e}')
+            self.parser.error(f"parsing config file failed: {e}")
         return config
 
     def parse_config_sections(self, namespace, sections):
         """Parse options from a given iterable of config section names."""
-        assert self.parser.prog.startswith('pkgdev ')
-        module = self.parser.prog.split(' ', 1)[1] + '.'
-        with patch('snakeoil.cli.arghparse.ArgumentParser.error', self._config_error):
+        assert self.parser.prog.startswith("pkgdev ")
+        module = self.parser.prog.split(" ", 1)[1] + "."
+        with patch("snakeoil.cli.arghparse.ArgumentParser.error", self._config_error):
             for section in (x for x in sections if x in self.config):
-                config_args = ((k.split('.', 1)[1], v) for k, v in self.config.items(section) if k.startswith(module))
-                config_args = (f'--{k}={v}' if v else f'--{k}' for k, v in config_args)
+                config_args = (
+                    (k.split(".", 1)[1], v)
+                    for k, v in self.config.items(section)
+                    if k.startswith(module)
+                )
+                config_args = (f"--{k}={v}" if v else f"--{k}" for k, v in config_args)
                 namespace, args = self.parser.parse_known_optionals(config_args, namespace)
                 if args:
                     self.parser.error(f"unknown arguments: {'  '.join(args)}")
         return namespace
 
     def parse_config_options(self, namespace, configs=()):
         """Parse options from config if they exist."""
@@ -85,65 +88,71 @@
             return namespace
 
         self.configs.update(configs)
         # reset jit attr to force reparse
         self._config = None
 
         # load default options
-        namespace = self.parse_config_sections(namespace, ['DEFAULT'])
+        namespace = self.parse_config_sections(namespace, ["DEFAULT"])
 
         return namespace
 
     def _config_error(self, message, status=2):
         """Stub to replace error method that notes config failure."""
-        self.parser.exit(status, f'{self.parser.prog}: failed loading config: {message}\n')
+        self.parser.exit(status, f"{self.parser.prog}: failed loading config: {message}\n")
+
 
 class ArgumentParser(arghparse.ArgumentParser):
     """Parse all known arguments, from command line and config file."""
 
     def __init__(self, parents=(), **kwargs):
         self.config_argparser = arghparse.ArgumentParser(suppress=True)
-        config_options = self.config_argparser.add_argument_group('config options')
+        config_options = self.config_argparser.add_argument_group("config options")
         config_options.add_argument(
-            '--config', action=ConfigArg, dest='config_file',
-            help='use custom pkgdev settings file',
+            "--config",
+            action=ConfigArg,
+            dest="config_file",
+            help="use custom pkgdev settings file",
             docs="""
                 Load custom pkgdev scan settings from a given file.
 
                 Note that custom user settings override all other system and repo-level
                 settings.
 
                 It's also possible to disable all types of settings loading by
                 specifying an argument of 'false' or 'no'.
-            """)
+            """,
+        )
         _mk_domain(config_options)
         super().__init__(parents=[*parents, self.config_argparser], **kwargs)
 
     def parse_known_args(self, args=None, namespace=None):
         temp_namespace, _ = self.config_argparser.parse_known_args(args, namespace)
         # parser supporting config file options
         config_parser = ConfigFileParser(self)
         # always load settings from bundled config
-        namespace = config_parser.parse_config_options(
-            namespace, configs=[const.BUNDLED_CONF_FILE])
+        namespace = config_parser.parse_config_options(namespace, configs=[const.BUNDLED_CONF_FILE])
 
         # load default args from system/user configs if config-loading is allowed
         if temp_namespace.config_file is None:
             namespace = config_parser.parse_config_options(
-                namespace, configs=ConfigFileParser.default_configs)
+                namespace, configs=ConfigFileParser.default_configs
+            )
         elif temp_namespace.config_file is not False:
             namespace = config_parser.parse_config_options(
-                namespace, configs=(namespace.config_file, ))
+                namespace, configs=(namespace.config_file,)
+            )
 
         try:
             repo = temp_namespace.domain.find_repo(
-                os.getcwd(), config=temp_namespace.config, configure=False)
+                os.getcwd(), config=temp_namespace.config, configure=False
+            )
             if repo is not None:
                 namespace = config_parser.parse_config_sections(namespace, repo.aliases)
         except (repo_errors.InitializationError, IOError) as exc:
             self.error(str(exc))
 
-        if os.getenv('NOCOLOR'):
+        if os.getenv("NOCOLOR"):
             namespace.color = False
 
         # parse command line args to override config defaults
         return super().parse_known_args(args, namespace)
```

### Comparing `pkgdev-0.2.4/src/pkgdev/const.py` & `pkgdev-0.2.5/src/pkgdev/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,19 +21,22 @@
     consts = mappings.ProxiedAttrs(_module)
     default_value %= consts
     return getattr(_defaults, attr, default_value)
 
 
 # determine XDG compatible paths
 for xdg_var, var_name, fallback_dir in (
-        ('XDG_CONFIG_HOME', 'USER_CONFIG_PATH', '~/.config'),
-        ('XDG_DATA_HOME', 'USER_DATA_PATH', '~/.local/share')):
+    ("XDG_CONFIG_HOME", "USER_CONFIG_PATH", "~/.config"),
+    ("XDG_DATA_HOME", "USER_DATA_PATH", "~/.local/share"),
+):
     setattr(
-        _module, var_name,
-        os.path.join(os.environ.get(xdg_var, os.path.expanduser(fallback_dir)), 'pkgdev'))
+        _module,
+        var_name,
+        os.path.join(os.environ.get(xdg_var, os.path.expanduser(fallback_dir)), "pkgdev"),
+    )
 
-REPO_PATH = _GET_CONST('REPO_PATH', _reporoot)
-DATA_PATH = _GET_CONST('DATA_PATH', '%(REPO_PATH)s/data')
+REPO_PATH = _GET_CONST("REPO_PATH", _reporoot)
+DATA_PATH = _GET_CONST("DATA_PATH", "%(REPO_PATH)s/data")
 
-USER_CONF_FILE = os.path.join(getattr(_module, 'USER_CONFIG_PATH'), 'pkgdev.conf')
-SYSTEM_CONF_FILE = '/etc/pkgdev/pkgdev.conf'
-BUNDLED_CONF_FILE = os.path.join(DATA_PATH, 'pkgdev.conf')
+USER_CONF_FILE = os.path.join(getattr(_module, "USER_CONFIG_PATH"), "pkgdev.conf")
+SYSTEM_CONF_FILE = "/etc/pkgdev/pkgdev.conf"
+BUNDLED_CONF_FILE = os.path.join(DATA_PATH, "pkgdev.conf")
```

### Comparing `pkgdev-0.2.4/src/pkgdev/git.py` & `pkgdev-0.2.5/src/pkgdev/git.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 class GitError(SystemExit):
     """Generic error running a git command."""
 
 
 def run(*args, **kwargs):
     """Wrapper for running git via subprocess.run()."""
-    kwargs.setdefault('check', True)
-    kwargs.setdefault('text', True)
-    cmd = ['git'] + list(args)
+    kwargs.setdefault("check", True)
+    kwargs.setdefault("text", True)
+    cmd = ["git"] + list(args)
 
     # output git command that would be run to stderr
-    if '--dry-run' in args:
-        git_cmd = ' '.join(x for x in cmd if x != '--dry-run')
-        sys.stderr.write(f'{git_cmd}\n')
+    if "--dry-run" in args:
+        git_cmd = " ".join(x for x in cmd if x != "--dry-run")
+        sys.stderr.write(f"{git_cmd}\n")
 
     try:
         return subprocess.run(cmd, **kwargs)
     except FileNotFoundError as e:
         raise UserException(str(e))
     except subprocess.CalledProcessError as e:
         raise GitError(e.returncode)
```

### Comparing `pkgdev-0.2.4/src/pkgdev/mangle.py` & `pkgdev-0.2.5/src/pkgdev/mangle.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import traceback
 from datetime import datetime
 
 from snakeoil.cli.exceptions import UserException
 from snakeoil.mappings import OrderedSet
 
 copyright_regex = re.compile(
-    r'^# Copyright (?P<date>(?P<begin>\d{4}-)?(?P<end>\d{4})) (?P<holder>.+)$')
+    r"^# Copyright (?P<date>(?P<begin>\d{4}-)?(?P<end>\d{4})) (?P<holder>.+)$"
+)
 
 keywords_regex = re.compile(
-    r'^(?P<pre>[^#]*\bKEYWORDS=(?P<quote>[\'"]?))'
-    r'(?P<keywords>.*)'
-    r'(?P<post>(?P=quote).*)$')
+    r'^(?P<pre>[^#]*\bKEYWORDS=(?P<quote>[\'"]?))(?P<keywords>.*)(?P<post>(?P=quote).*)$'
+)
 
 
-def mangle(name):
+def mangle(name: str):
     """Decorator to register file mangling methods."""
 
     class decorator:
         """Decorator with access to the class of a decorated function."""
 
         def __init__(self, func):
             self.func = func
@@ -45,49 +45,50 @@
     def __init__(self, changes, skip_regex=None):
         self.jobs = os.cpu_count()
         if skip_regex is not None:
             changes = (c for c in changes if not skip_regex.match(c.full_path))
         self.changes = OrderedSet(changes)
 
         # setup for parallelizing the mangling procedure across files
-        self._mp_ctx = multiprocessing.get_context('fork')
+        self._mp_ctx = multiprocessing.get_context("fork")
         self._mangled_paths_q = self._mp_ctx.SimpleQueue()
         self._current_year = str(datetime.today().year)
 
         # initialize settings used by iterator support
         self._runner = self._mp_ctx.Process(target=self._run)
         signal.signal(signal.SIGINT, self._kill_pipe)
         self._mangled_paths = iter(self._mangled_paths_q.get, None)
 
         # construct composed mangling function
         self.composed_func = functools.reduce(
-            lambda f, g: lambda x: f(g(self, x)), self._mangle_funcs.values(), lambda x: x)
+            lambda f, g: lambda x: f(g(self, x)), self._mangle_funcs.values(), lambda x: x
+        )
 
-    @mangle('EOF')
+    @mangle("EOF")
     def _eof(self, change):
         """Drop EOF whitespace and forcibly add EOF newline."""
-        return change.update(change.data.rstrip() + '\n')
+        return change.update(change.data.rstrip() + "\n")
 
-    @mangle('keywords')
+    @mangle("keywords")
     def _keywords(self, change):
         """Fix keywords order."""
 
         def keywords_sort_key(kw):
-            return tuple(reversed(kw.lstrip('-~').partition('-')))
+            return tuple(reversed(kw.lstrip("-~").partition("-")))
 
         lines = change.data.splitlines()
         for i, line in enumerate(lines):
             if mo := keywords_regex.match(line):
-                kw = sorted(mo.group('keywords').split(), key=keywords_sort_key)
-                new_kw = ' '.join(kw)
-                if not mo.group('quote'):
+                kw = sorted(mo.group("keywords").split(), key=keywords_sort_key)
+                new_kw = " ".join(kw)
+                if not mo.group("quote"):
                     new_kw = f'"{new_kw}"'
                 lines[i] = f'{mo.group("pre")}{new_kw}{mo.group("post")}'
                 break
-        return change.update('\n'.join(lines) + '\n')
+        return change.update("\n".join(lines) + "\n")
 
     def _kill_pipe(self, *args, error=None):
         """Handle terminating the mangling process group."""
         if self._runner.is_alive():
             os.killpg(self._runner.pid, signal.SIGKILL)
         if error is not None:
             # propagate exception raised during parallelized mangling
@@ -153,21 +154,21 @@
 
 
 class GentooMangler(Mangler):
     """Gentoo repo specific file mangler."""
 
     _mangle_funcs = Mangler._mangle_funcs.copy()
 
-    @mangle('copyright')
+    @mangle("copyright")
     def _copyright(self, change):
         """Fix copyright headers and dates."""
         lines = change.data.splitlines()
         if mo := copyright_regex.match(lines[0]):
             groups = mo.groupdict()
-            if groups['begin'] is None and groups['date'] != self._current_year:
+            if groups["begin"] is None and groups["date"] != self._current_year:
                 # use old copyright date as the start of date range
                 date_range = f"{groups['date']}-{self._current_year}"
-                lines[0] = re.sub(groups['date'], date_range, lines[0])
+                lines[0] = re.sub(groups["date"], date_range, lines[0])
             else:
-                lines[0] = re.sub(mo.group('end'), self._current_year, lines[0])
-            lines[0] = re.sub('Gentoo Foundation', 'Gentoo Authors', lines[0])
-        return change.update('\n'.join(lines) + '\n')
+                lines[0] = re.sub(mo.group("end"), self._current_year, lines[0])
+            lines[0] = re.sub("Gentoo Foundation", "Gentoo Authors", lines[0])
+        return change.update("\n".join(lines) + "\n")
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/__init__.py` & `pkgdev-0.2.5/src/pkgdev/scripts/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,36 +15,38 @@
     try:
         sys.path.remove(os.getcwd())
     except ValueError:
         pass
 
     try:
         from pkgdev.cli import Tool
-        script_module = '.'.join(
-            os.path.realpath(__file__).split(os.path.sep)[-3:-1] +
-            [script_name.replace('-', '_')])
+
+        script_module = ".".join(
+            os.path.realpath(__file__).split(os.path.sep)[-3:-1] + [script_name.replace("-", "_")]
+        )
         script = import_module(script_module)
     except ImportError as e:
-        python_version = '.'.join(map(str, sys.version_info[:3]))
-        sys.stderr.write(f'Failed importing: {e}!\n')
+        python_version = ".".join(map(str, sys.version_info[:3]))
+        sys.stderr.write(f"Failed importing: {e}!\n")
         sys.stderr.write(
-            'Verify that pkgdev and its deps are properly installed '
-            f'and/or PYTHONPATH is set correctly for python {python_version}.\n')
-        if '--debug' in sys.argv[1:]:
+            "Verify that pkgdev and its deps are properly installed "
+            f"and/or PYTHONPATH is set correctly for python {python_version}.\n"
+        )
+        if "--debug" in sys.argv[1:]:
             raise
-        sys.stderr.write('Add --debug to the commandline for a traceback.\n')
+        sys.stderr.write("Add --debug to the commandline for a traceback.\n")
         sys.exit(1)
 
     tool = Tool(script.argparser)
     sys.exit(tool())
 
 
 def main():
     # We're in a git repo or tarball so add the src dir to the system path.
     # Note that this assumes a certain module layout.
     src_dir = os.path.realpath(__file__).rsplit(os.path.sep, 3)[0]
     sys.path.insert(0, src_dir)
     run(os.path.basename(sys.argv[0]))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/argparsers.py` & `pkgdev-0.2.5/src/pkgdev/scripts/argparsers.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,35 +10,34 @@
 git_repo_argparser = ArgumentParser(suppress=True)
 
 
 @cwd_repo_argparser.bind_final_check
 def _determine_cwd_repo(parser, namespace):
     namespace.cwd = os.getcwd()
     try:
-        repo = namespace.domain.find_repo(
-            namespace.cwd, config=namespace.config, configure=False)
+        repo = namespace.domain.find_repo(namespace.cwd, config=namespace.config, configure=False)
     except (repo_errors.InitializationError, IOError) as e:
         raise parser.error(str(e))
 
     if repo is None:
-        raise parser.error('not in ebuild repo')
+        raise parser.error("not in ebuild repo")
 
     namespace.repo = repo
 
 
 @git_repo_argparser.bind_final_check
 def _determine_git_repo(parser, namespace):
     try:
-        p = git.run('rev-parse', '--show-toplevel', stdout=subprocess.PIPE)
+        p = git.run("rev-parse", "--show-toplevel", stdout=subprocess.PIPE)
         path = p.stdout.strip()
     except git.GitError:
-        raise parser.error('not in git repo')
+        raise parser.error("not in git repo")
 
     # verify the git and ebuild repo roots match when using both
     try:
         if namespace.repo.location != path:
-            raise parser.error('not in ebuild git repo')
+            raise parser.error("not in ebuild git repo")
     except AttributeError:
         # ebuild repo parser not enabled
         pass
 
     namespace.git_repo = path
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_commit.py` & `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_commit.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,153 +36,203 @@
 
     def parse_known_args(self, args=None, namespace=None):
         namespace.footer = OrderedSet()
         namespace.git_add_files = []
         namespace, args = super().parse_known_args(args, namespace)
 
         if namespace.dry_run:
-            args.append('--dry-run')
+            args.append("--dry-run")
         if namespace.verbosity:
-            args.append('-v')
+            args.append("-v")
         if namespace.signoff:
-            args.append('--signoff')
+            args.append("--signoff")
         if namespace.edit:
-            args.append('--edit')
+            args.append("--edit")
         namespace.commit_args = args
+        namespace.git_args_paths = list(
+            filter(os.path.exists, (s for s in args if not s.startswith("-")))
+        )
         return namespace, []
 
 
 class BugTag(argparse.Action):
     """Register bug-related tag to inject into the commit message footer."""
 
     def __call__(self, parser, namespace, value, option_string=None):
         try:
-            url = f'https://bugs.gentoo.org/{int(value)}'
+            url = f"https://bugs.gentoo.org/{int(value)}"
         except ValueError:
             url = value
-            if not url.startswith(('https://', 'http://')):
-                raise argparse.ArgumentError(self, f'invalid URL: {url}')
+            if not url.startswith(("https://", "http://")):
+                raise argparse.ArgumentError(self, f"invalid URL: {url}")
         namespace.footer.add((self.dest.capitalize(), url))
 
 
 class CommitTag(argparse.Action):
     """Register commit tag to inject into the commit message footer."""
 
     def __call__(self, parser, namespace, value, option_string=None):
         try:
-            name, val = value.split(':', 1)
+            name, val = value.split(":", 1)
             if not (name and val):
-                raise ValueError('empty name or value')
+                raise ValueError("empty name or value")
         except ValueError:
-            raise argparse.ArgumentError(self, f'invalid commit tag: {value!r}')
+            raise argparse.ArgumentError(self, f"invalid commit tag: {value!r}")
         namespace.footer.add((name.capitalize(), val))
 
 
 commit = ArgumentParser(
-    prog='pkgdev commit', description='create git commit',
-    parents=(cwd_repo_argparser, git_repo_argparser))
+    prog="pkgdev commit",
+    description="create git commit",
+    parents=(cwd_repo_argparser, git_repo_argparser),
+)
 # custom `pkgcheck scan` args used for tests
-commit.add_argument('--pkgcheck-scan', help=argparse.SUPPRESS)
-commit_opts = commit.add_argument_group('commit options')
+commit.add_argument("--pkgcheck-scan", help=argparse.SUPPRESS)
+commit_opts = commit.add_argument_group("commit options")
 commit_opts.add_argument(
-    '-b', '--bug', action=BugTag,
-    help='add Bug tag for a given Gentoo or upstream bug')
+    "-b", "--bug", action=BugTag, help="add Bug tag for a given Gentoo or upstream bug"
+)
 commit_opts.add_argument(
-    '-c', '--closes', action=BugTag,
-    help='add Closes tag for a given Gentoo bug or upstream PR URL')
+    "-c", "--closes", action=BugTag, help="add Closes tag for a given Gentoo bug or upstream PR URL"
+)
 commit_opts.add_argument(
-    '-T', '--tag', action=CommitTag, metavar='NAME:VALUE',
-    help='add commit tag')
+    "-T", "--tag", action=CommitTag, metavar="NAME:VALUE", help="add commit tag"
+)
 commit_opts.add_argument(
-    '-n', '--dry-run', action='store_true',
-    help='pretend to create commit',
+    "-n",
+    "--dry-run",
+    action="store_true",
+    help="pretend to create commit",
     docs="""
         Perform all actions without creating a commit.
-    """)
+    """,
+)
 commit_opts.add_argument(
-    '-s', '--scan', nargs='?', const=True, action=arghparse.StoreBool,
-    help='run pkgcheck against staged changes',
+    "-s",
+    "--scan",
+    nargs="?",
+    const=True,
+    action=arghparse.StoreBool,
+    help="run pkgcheck against staged changes",
     docs="""
         By default, ``pkgdev commit`` doesn't scan for QA errors. This option
         enables using pkgcheck to scan the staged changes for issues, erroring
         out if any failures are found.
-    """)
+    """,
+)
 commit_opts.add_argument(
-    '-A', '--ask', nargs='?', const=True, action=arghparse.StoreBool,
-    help='confirm creating commit with QA errors',
+    "-A",
+    "--ask",
+    nargs="?",
+    const=True,
+    action=arghparse.StoreBool,
+    help="confirm creating commit with QA errors",
     docs="""
         When running with the -s/--scan option enabled, ``pkgdev commit`` will
         ask for confirmation before creating a commit if it detects failure
         results.
-    """)
+    """,
+)
 commit_opts.add_argument(
-    '--mangle', nargs='?', const=True, action=arghparse.StoreBool,
-    help='forcibly enable/disable file mangling',
+    "--mangle",
+    nargs="?",
+    const=True,
+    action=arghparse.StoreBool,
+    help="forcibly enable/disable file mangling",
     docs="""
         File mangling automatically modifies the content of relevant staged
         files including updating copyright headers and fixing EOF newlines.
 
         This is performed by default for the gentoo repo, but can be forcibly
         disabled or enabled as required.
-    """)
+    """,
+)
 commit_opts.add_argument(
-    '--signoff', nargs='?', const=True, action=arghparse.StoreBool,
-    help='Add a Signed-off-by at the end of the commit log message',
+    "--signoff",
+    nargs="?",
+    const=True,
+    action=arghparse.StoreBool,
+    help="Add a Signed-off-by at the end of the commit log message",
     docs="""
         Add a Signed-off-by trailer by the committer at the end of the commit
         log message.
 
         For committing to the Gentoo repository, under GLEP-76, the committer
         shall certify agreement to the Certificate of Origin by adding
         Signed-off-by line containing the committer's legal name.
-    """)
+    """,
+)
 commit_opts.add_argument(
-    '-d', '--distdir', type=arghparse.create_dir, help='target download directory',
+    "-d",
+    "--distdir",
+    type=arghparse.create_dir,
+    help="target download directory",
     docs="""
         Use a specified target directory for downloads instead of the
         configured DISTDIR.
-    """)
+    """,
+)
 
 msg_actions = commit_opts.add_mutually_exclusive_group()
 msg_actions.add_argument(
-    '-m', '--message', metavar='MSG', action='append',
-    help='specify commit message',
+    "-m",
+    "--message",
+    metavar="MSG",
+    action="append",
+    help="specify commit message",
     docs="""
         Use a given message as the commit message. If multiple -m options are
         specified, their values are concatenated as separate paragraphs.
 
         Note that the first value will be used for the commit summary and if
         it's empty then a generated summary will be used if available.
-    """)
+    """,
+)
 msg_actions.add_argument(
-    '-M', '--message-template', metavar='FILE', type=argparse.FileType('r'),
-    help='use commit message template from specified file',
+    "-M",
+    "--message-template",
+    metavar="FILE",
+    type=argparse.FileType("r"),
+    help="use commit message template from specified file",
     docs="""
         Use content from the given file as a commit message template. The
         commit summary prefix '*: ' is automatically replaced by a generated
         prefix if one exists for the related staged changes.
-    """)
-msg_actions.add_argument('-F', '--file', help=argparse.SUPPRESS)
-msg_actions.add_argument('-t', '--template', help=argparse.SUPPRESS)
-msg_actions.add_argument(
-    '-e', '--edit', action='store_true',
-    help='force edit of commit',
+    """,
+)
+msg_actions.add_argument("-F", "--file", help=argparse.SUPPRESS)
+msg_actions.add_argument("-t", "--template", help=argparse.SUPPRESS)
+commit_opts.add_argument(
+    "-e",
+    "--edit",
+    action="store_true",
+    help="force edit of commit",
     docs="""
-        The message taken from command line with -m, and from automatically
-        generated one are usually used as the commit log message unmodified.
-        This option lets you further edit the message taken from these sources.
-    """)
+        This option will ask git to open the commit message in an editor before
+        commit. The git configuration is used to select the editor.
+    """,
+)
 
 add_actions = commit_opts.add_mutually_exclusive_group()
 add_actions.add_argument(
-    '-u', '--update', dest='git_add_arg', const='--update', action='store_const',
-    help='stage all changed files')
+    "-u",
+    "--update",
+    dest="git_add_arg",
+    const="--update",
+    action="store_const",
+    help="stage all changed files",
+)
 add_actions.add_argument(
-    '-a', '--all', dest='git_add_arg', const='--all', action='store_const',
-    help='stage all changed/new/removed files')
+    "-a",
+    "--all",
+    dest="git_add_arg",
+    const="--all",
+    action="store_const",
+    help="stage all changed/new/removed files",
+)
 
 
 class HistoricalRepo(UnconfiguredTree):
     """Repository of historical packages stored in a temporary directory."""
 
     def __init__(self, parent_repo, tmpdir, *args, **kwargs):
         self.__parent_repo = parent_repo
@@ -197,21 +247,23 @@
         for pkg in pkgs:
             self.notify_add_package(pkg)
 
     def _populate(self, pkgs):
         """Populate the repo with a given sequence of historical packages."""
         paths = {pkg.key for pkg in pkgs}
         old_files = subprocess.Popen(
-            ['git', 'archive', 'HEAD'] + list(paths),
-            stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-            cwd=self.__parent_repo.location)
+            ["git", "archive", "HEAD"] + list(paths),
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            cwd=self.__parent_repo.location,
+        )
         if old_files.poll():  # pragma: no cover
             error = old_files.stderr.read().decode().strip()
-            raise Exception(f'failed populating archive repo: {error}')
-        with tarfile.open(mode='r|', fileobj=old_files.stdout) as tar:
+            raise Exception(f"failed populating archive repo: {error}")
+        with tarfile.open(mode="r|", fileobj=old_files.stdout) as tar:
             tar.extractall(path=self.location)
 
 
 def change(*statuses):
     """Decorator to register change status summary methods."""
 
     class decorator:
@@ -240,46 +292,46 @@
     @jit_attr
     def old_repo(self):
         """Create a repository of historical packages removed from git."""
         tmpdir = tempfile.TemporaryDirectory()
         repo_dir = tmpdir.name
 
         # set up some basic repo files so pkgcore doesn't complain
-        os.makedirs(pjoin(repo_dir, 'metadata'))
-        with open(pjoin(repo_dir, 'metadata', 'layout.conf'), 'w') as f:
+        os.makedirs(pjoin(repo_dir, "metadata"))
+        with open(pjoin(repo_dir, "metadata", "layout.conf"), "w") as f:
             f.write(f"masters = {' '.join(x.repo_id for x in self.repo.trees)}\n")
-        os.makedirs(pjoin(repo_dir, 'profiles'))
-        with open(pjoin(repo_dir, 'profiles', 'repo_name'), 'w') as f:
-            f.write(f'{self.repo.repo_id}-old\n')
+        os.makedirs(pjoin(repo_dir, "profiles"))
+        with open(pjoin(repo_dir, "profiles", "repo_name"), "w") as f:
+            f.write(f"{self.repo.repo_id}-old\n")
 
         repo_config = RepoConfig(repo_dir)
         tree_cls = partial(HistoricalRepo, self.repo, tmpdir)
         return tree(self.options.config, repo_config, tree_cls=tree_cls)
 
     def __str__(self):
         """Serialize git changes into commit summary strings."""
         statuses = frozenset(x.status for x in self.changes.values())
         try:
             if s := self.status_funcs[statuses](self):
                 return s
         except KeyError:  # pragma: no cover
             pass
-        return ''
+        return ""
 
 
 class MetadataSummary(ChangeSummary):
     """Summary generation support for metadata.xml changes."""
 
     status_funcs = {}
 
     def __init__(self, options, changes):
         super().__init__(options)
         self.changes = {x.atom: x for x in changes}
 
-    @change('M')
+    @change("M")
     def modify(self):
         """Generate summaries for modify actions."""
         atom = next(iter(self.changes))
         pkgs = self.repo.match(atom)
         self.old_repo.add_pkgs(pkgs)
         try:
             old_pkg = self.old_repo.match(atom)[0]
@@ -287,40 +339,40 @@
         except IndexError:  # pragma: no cover
             # broken ebuild should be caught during manifesting or scanning
             return
 
         if old_pkg.maintainers != new_pkg.maintainers:
             new = {x.email for x in new_pkg.maintainers}
             old = {x.email for x in old_pkg.maintainers}
-            p = git.run('config', 'user.email', stdout=subprocess.PIPE)
+            p = git.run("config", "user.email", stdout=subprocess.PIPE)
             git_email = p.stdout.strip()
             if git_email in new - old:
-                return 'add myself as a maintainer'
+                return "add myself as a maintainer"
             if git_email in old - new:
-                return 'drop myself as a maintainer'
+                return "drop myself as a maintainer"
             if old and not new:
-                return 'drop to maintainer-needed'
-            return 'update maintainers'
+                return "drop to maintainer-needed"
+            return "update maintainers"
         elif old_pkg.stabilize_allarches != new_pkg.stabilize_allarches:
-            status = 'mark' if new_pkg.stabilize_allarches else 'drop'
-            return f'{status} ALLARCHES'
+            status = "mark" if new_pkg.stabilize_allarches else "drop"
+            return f"{status} ALLARCHES"
         elif old_pkg.upstreams != new_pkg.upstreams:
             new = set(new_pkg.upstreams)
             old = set(old_pkg.upstreams)
             added = new - old
             removed = old - new
             msg = []
-            for action, data in (('add', added), ('remove', removed)):
+            for action, data in (("add", added), ("remove", removed)):
                 if data:
-                    upstreams = ', '.join(sorted(x.type for x in data))
+                    upstreams = ", ".join(sorted(x.type for x in data))
                     msg.append(f"{action} {upstreams} upstream metadata")
             # return action-specific shorter summary if a single type exists
             if len(msg) == 1 and len(msg[0]) <= 50:
                 return msg[0]
-            return 'update upstream metadata'
+            return "update upstream metadata"
 
 
 class PkgSummary(ChangeSummary):
     """Summary generation support for single package ebuild changes."""
 
     status_funcs = {}
 
@@ -339,214 +391,240 @@
         return any(x.revision for x in self.changes)
 
     @jit_attr
     def existing(self):
         """Existing packages in the tree related to the package."""
         return tuple(self.repo.match(next(iter(self.changes)).unversioned_atom))
 
-    @change('A')
+    @change("A")
     def add(self):
         """Generate summaries for add actions."""
         if len(self.existing) == len(self.changes):
             msg = f"new package, add {', '.join(self.versions)}"
             if len(self.versions) == 1 or len(msg) <= 50:
                 return msg
-            return 'new package'
+            return "new package"
         elif not self.revbump:
             msg = f"add {', '.join(self.versions)}"
             if len(self.versions) == 1 or len(msg) <= 50:
                 return msg
-            return 'add versions'
+            return "add versions"
         elif len(self.changes) == 1:
             # adding a new revbump
             atom = next(iter(self.changes))
             # assume revbump was based on the previous version
             pkgs = sorted(x for x in self.repo.match(atom.unversioned_atom) if x <= atom)
             try:
                 old_pkg, new_pkg = pkgs[-2:]
             except ValueError:  # pragma: no cover
                 # broken ebuild should be caught during manifesting or scanning
                 return
 
             if old_pkg.eapi in new_pkg.eapi.inherits[1:]:
-                return f'update EAPI {old_pkg.eapi} -> {new_pkg.eapi}'
+                return f"update EAPI {old_pkg.eapi} -> {new_pkg.eapi}"
 
-    @change('D')
+    @change("D")
     def remove(self):
         """Generate summaries for remove actions."""
         if self.existing:
             msg = f"drop {', '.join(self.versions)}"
             if len(self.versions) == 1 or len(msg) <= 50:
                 return msg
-            return 'drop versions'
-        return 'treeclean'
+            return "drop versions"
+        return "treeclean"
 
-    @change('R')
+    @change("R")
     def rename(self):
         """Generate summaries for rename actions."""
         if len(self.changes) == 1:
             if not self.revbump:
                 # single, non-revbump version rename
                 change = next(iter(self.changes.values()))
-                return f'add {change.atom.fullver}, drop {change.old.fullver}'
+                return f"add {change.atom.fullver}, drop {change.old.fullver}"
         elif len({x.key for x in self.changes}) == 1:
             change = next(iter(self.changes.values()))
             if change.atom.key != change.old.key:
                 # package rename
-                return f'rename {change.old.key}'
+                return f"rename {change.old.key}"
 
-    @change('M')
+    @change("M")
     def modify(self):
         """Generate summaries for modify actions."""
-        if len(self.changes) == 1:
-            atom = next(iter(self.changes))
+        summaries = set()
+        for atom in self.changes:
             pkgs = self.repo.match(atom)
             self.old_repo.add_pkgs(pkgs)
             try:
                 old_pkg = self.old_repo.match(atom)[0]
                 new_pkg = pkgs[0]
             except IndexError:  # pragma: no cover
                 # broken ebuild should be caught during manifesting or scanning
-                return
+                continue
 
             if old_pkg.eapi in new_pkg.eapi.inherits[1:]:
-                return f'update EAPI {old_pkg.eapi} -> {new_pkg.eapi}'
+                summaries.add(f"update EAPI {old_pkg.eapi} -> {new_pkg.eapi}")
             elif new_pkg.keywords != old_pkg.keywords:
-                repo_stable = set(self.repo.config.arches_desc['stable'])
+                repo_stable = set(self.repo.config.arches_desc["stable"])
                 new_keywords = set(new_pkg.keywords)
                 old_keywords = set(old_pkg.keywords)
                 added = new_keywords - old_keywords
                 removed = old_keywords - new_keywords
-                if removed == {f'~{x}' for x in added}:
-                    action = f'stabilize {atom.fullver}'
-                    if (new_pkg.stabilize_allarches and repo_stable and
-                            not repo_stable.intersection(x.lstrip('~') for x in new_keywords - removed if x[0] == '~')):
+                if removed == {f"~{x}" for x in added}:
+                    action = f"stabilize {atom.fullver}"
+                    if (
+                        new_pkg.stabilize_allarches
+                        and repo_stable
+                        and not repo_stable.intersection(
+                            x.lstrip("~") for x in new_keywords - removed if x[0] == "~"
+                        )
+                    ):
                         msg = f"{action} for ALLARCHES"
                     else:
                         msg = f"{action} for {', '.join(sorted(added))}"
-                elif removed == {x.lstrip('~') for x in added}:
-                    action = f'destabilize {atom.fullver}'
+                elif removed == {x.lstrip("~") for x in added}:
+                    action = f"destabilize {atom.fullver}"
                     msg = f"{action} for {', '.join(sorted(added))}"
                 elif added:
-                    action = f'keyword {atom.fullver}'
+                    action = f"keyword {atom.fullver}"
                     msg = f"{action} for {', '.join(sorted(added))}"
                 else:
-                    action = f'unkeyword {atom.fullver}'
+                    action = f"unkeyword {atom.fullver}"
                     msg = f"{action} for {', '.join(sorted(removed))}"
 
                 if len(msg) <= 50:
-                    return msg
-                return action
+                    summaries.add(msg)
+                else:
+                    summaries.add(action)
             else:
                 # use sourced bash env diffs to determine summaries
                 old_env = old_pkg.environment.data.splitlines()
                 new_env = new_pkg.environment.data.splitlines()
-                var_drop_re = re.compile(r'^-declare .+ (?P<name>\w+)=(?P<value>.+)$')
-                var_add_re = re.compile(r'^\+declare .+ (?P<name>\w+)=(?P<value>.+)$')
+                var_drop_re = re.compile(r"^-declare .+ (?P<name>\w+)=(?P<value>.+)$")
+                var_add_re = re.compile(r"^\+declare .+ (?P<name>\w+)=(?P<value>.+)$")
                 drop, add = {}, {}
 
                 for x in difflib.unified_diff(old_env, new_env):
                     if mo := var_drop_re.match(x):
-                        drop[mo.group('name')] = mo.group('value')
+                        drop[mo.group("name")] = mo.group("value")
                     elif mo := var_add_re.match(x):
-                        add[mo.group('name')] = mo.group('value')
+                        add[mo.group("name")] = mo.group("value")
 
-                watch_vars = {'HOMEPAGE', 'DESCRIPTION', 'LICENSE', 'SRC_URI'}
-                array_targets = {'PYTHON_COMPAT', 'LUA_COMPAT'}
-                string_targets = {'USE_RUBY'}
-                use_expand_mapping = {'PYTHON_COMPAT': 'python_targets', 'LUA_COMPAT': 'lua_targets', 'USE_RUBY': 'ruby_targets'}
+                watch_vars = {"HOMEPAGE", "DESCRIPTION", "LICENSE", "SRC_URI"}
+                array_targets = {"PYTHON_COMPAT", "LUA_COMPAT"}
+                string_targets = {"USE_RUBY"}
+                use_expand_mapping = {
+                    "PYTHON_COMPAT": "python_targets",
+                    "LUA_COMPAT": "lua_targets",
+                    "USE_RUBY": "ruby_targets",
+                }
                 targets = array_targets | string_targets
 
                 updated_vars = drop.keys() & add.keys()
                 if updated := sorted(watch_vars & updated_vars):
-                    return f"update {', '.join(updated)}"
+                    summaries.add(f"update {', '.join(updated)}")
                 elif (target := targets & updated_vars) and len(target) == 1:
                     target = next(iter(target))
-                    py_re = lambda x: re.sub(r'^python(\d+)_(\d+)$', r'py\1.\2', x)
-                    use_expand = {py_re(use[len(target)+2:])
-                        for use, _ in self.repo.use_expand_desc[use_expand_mapping[target]]}
+                    py_re = partial(re.sub, r"^python(\d+)_(\d+)$", r"py\1.\2")
+                    use_expand = {
+                        py_re(use[len(target) + 2 :])
+                        for use, _ in self.repo.use_expand_desc[use_expand_mapping[target]]
+                    }
                     if target in array_targets:
                         array_re = re.compile(r'\[\d+\]="(?P<val>.+?)"')
-                        old = {py_re(m.group('val')) for m in re.finditer(array_re, drop[target])}
-                        new = {py_re(m.group('val')) for m in re.finditer(array_re, add[target])}
+                        old = {py_re(m.group("val")) for m in re.finditer(array_re, drop[target])}
+                        new = {py_re(m.group("val")) for m in re.finditer(array_re, add[target])}
                     else:
                         old = set(drop[target].strip('"').split())
                         new = set(add[target].strip('"').split())
 
                     msg = []
                     if added := sorted(new - old):
                         msg.append(f"enable {', '.join(added)}")
                     if dropped := old - new:
                         if not msg or (dropped := dropped.intersection(use_expand)):
                             msg.append(f"disable {', '.join(sorted(dropped))}")
-                    msg = ' and '.join(msg)
+                    msg = " and ".join(msg)
                     if len(msg) <= 50:
-                        return msg
+                        summaries.add(msg)
                     else:
-                        return f'update {target} support'
+                        summaries.add(f"update {target} support")
+        if len(summaries) == 1:
+            return next(iter(summaries))
 
 
 class GitChanges(UserDict):
     """Mapping of change objects for staged git changes."""
 
     # ebuild path regex, validation is handled on instantiation
-    _ebuild_re = re.compile(r'^(?P<category>[^/]+)/[^/]+/(?P<package>[^/]+)\.ebuild$')
-    _eclass_re = re.compile(r'^eclass/(?P<name>[^/]+\.eclass)$')
+    _ebuild_re = re.compile(r"^(?P<category>[^/]+)/[^/]+/(?P<package>[^/]+)\.ebuild$")
+    _eclass_re = re.compile(r"^eclass/(?P<name>[^/]+\.eclass)$")
 
     def __init__(self, options):
         self._options = options
         self._repo = options.repo
         super().__init__(self._generate_mapping())
 
     def _generate_mapping(self):
         """Generate mapping for staged changes."""
         # stage changes as requested
         if self._options.git_add_arg:
-            git.run('add', self._options.git_add_arg, self._options.cwd)
+            git.run("add", self._options.git_add_arg, self._options.cwd)
 
         # determine staged changes forcing rename search
         p = git.run(
-            'diff-index', '--diff-filter=ARMD', '--find-renames',
-            '--name-status', '--cached', '-z', 'HEAD',
-            stdout=subprocess.PIPE)
+            "diff-index",
+            "--diff-filter=ARMD",
+            "--find-renames",
+            "--name-status",
+            "--cached",
+            "-z",
+            "HEAD",
+            *self._options.git_args_paths,
+            stdout=subprocess.PIPE,
+        )
 
         # if no changes exist, exit early
         if not p.stdout:
-            commit.error('no staged changes exist')
+            commit.error("no staged changes exist")
 
-        data = deque(p.stdout.strip('\x00').split('\x00'))
+        data = deque(p.stdout.strip("\x00").split("\x00"))
         changes = defaultdict(OrderedSet)
         while data:
             status = data.popleft()
             old_path = None
-            if status.startswith('R'):
-                status = 'R'
+            if status.startswith("R"):
+                status = "R"
                 old_path = data.popleft()
             path = data.popleft()
             path_components = path.split(os.sep)
             if path_components[0] in self._repo.categories and len(path_components) > 2:
                 if mo := self._ebuild_re.match(path):
                     # ebuild changes
                     try:
                         atom = atom_cls(f"={mo.group('category')}/{mo.group('package')}")
                         old = None
-                        if status == 'R' and (om := self._ebuild_re.match(old_path)):
+                        if status == "R" and (om := self._ebuild_re.match(old_path)):
                             old = atom_cls(f"={om.group('category')}/{om.group('package')}")
-                        changes[PkgChange].add(PkgChange(
-                            self._repo.location, status, path, atom=atom, ebuild=True, old=old))
+                        changes[PkgChange].add(
+                            PkgChange(
+                                self._repo.location, status, path, atom=atom, ebuild=True, old=old
+                            )
+                        )
                     except MalformedAtom:
                         continue
                 else:
                     # non-ebuild package level changes
                     atom = atom_cls(os.sep.join(path_components[:2]))
                     changes[PkgChange].add(
-                        PkgChange(self._repo.location, status, path, atom=atom, ebuild=False))
+                        PkgChange(self._repo.location, status, path, atom=atom, ebuild=False)
+                    )
             elif mo := self._eclass_re.match(path):
                 changes[EclassChange].add(
-                    EclassChange(self._repo.location, status, path, name=mo.group('name')))
+                    EclassChange(self._repo.location, status, path, name=mo.group("name"))
+                )
             else:
                 changes[path_components[0]].add(Change(self._repo.location, status, path))
 
         return changes
 
     @jit_attr
     def all(self):
@@ -567,16 +645,15 @@
     def prefix(self):
         """Determine commit message prefix using GLEP 66 as a guide.
 
         See https://www.gentoo.org/glep/glep-0066.html#commit-messages for
         details.
         """
         single = len(self.data) == 1
-        pkg_with_profile_update = (
-            len(self.data) == 2 and set(self.data) == {PkgChange, 'profiles'})
+        pkg_with_profile_update = len(self.data) == 2 and set(self.data) == {PkgChange, "profiles"}
 
         if single or pkg_with_profile_update:
             if single:
                 change_type, change_objs = next(iter(self.data.items()))
             else:
                 change_type = PkgChange
                 change_objs = self.data[PkgChange]
@@ -585,213 +662,222 @@
                 # changes limited to a single object
                 return change_objs[0].prefix
             else:
                 # multiple changes of the same object type
                 common_path = os.path.commonpath(x.path for x in change_objs)
                 if change_type is PkgChange:
                     if os.sep in common_path:
-                        return f'{common_path}: '
+                        return f"{common_path}: "
                     elif common_path:
-                        return f'{common_path}/*: '
-                    return '*/*: '
+                        return f"{common_path}/*: "
+                    return "*/*: "
                 elif common_path:
-                    return f'{common_path}: '
+                    return f"{common_path}: "
 
         # no prefix used for global changes
-        return ''
+        return ""
 
     @jit_attr
     def summary(self):
         """Determine commit message summary."""
         # all changes made on the same package
         if len({x.atom.key for x in self.pkg_changes}) == 1:
             if not self.ebuild_changes:
                 if len(self.pkg_changes) == 1:
-                    if self.pkg_changes[0].path.endswith('/Manifest'):
-                        return 'update Manifest'
-                    elif self.pkg_changes[0].path.endswith('/metadata.xml'):
+                    if self.pkg_changes[0].path.endswith("/Manifest"):
+                        return "update Manifest"
+                    elif self.pkg_changes[0].path.endswith("/metadata.xml"):
                         return str(MetadataSummary(self._options, self.pkg_changes))
             return str(PkgSummary(self._options, self.ebuild_changes))
-        return ''
+        return ""
 
 
 @dataclass(frozen=True)
 class Change:
     """Generic file change."""
+
     repo: str
     status: str
     path: str
 
     @property
     def full_path(self):
         return pjoin(self.repo, self.path)
 
     def read(self):
         """Read data from the change's file."""
         try:
-            with open(self.full_path, 'r', encoding='utf-8') as f:
+            with open(self.full_path, "r", encoding="utf-8") as f:
                 data = f.read()
         except (FileNotFoundError, UnicodeDecodeError):
             data = None
-        object.__setattr__(self, 'data', data)
+        object.__setattr__(self, "data", data)
         return data
 
     def update(self, data):
         """Update the change's cached file data."""
-        if data != getattr(self, 'data', None):
-            object.__setattr__(self, 'data', data)
+        if data != getattr(self, "data", None):
+            object.__setattr__(self, "data", data)
         return self
 
     def sync(self):
         """Write the change's cached file data back to its file."""
         try:
-            with open(self.full_path, 'w', encoding='utf-8') as f:
+            with open(self.full_path, "w", encoding="utf-8") as f:
                 f.write(self.data)
         except AttributeError:
             pass
 
     @property
     def prefix(self):
         if os.sep in self.path:
             # use change path's parent directory
-            return f'{os.path.dirname(self.path)}: '
+            return f"{os.path.dirname(self.path)}: "
         # use repo root file name
-        return f'{self.path}: '
+        return f"{self.path}: "
 
 
 @dataclass(frozen=True)
 class EclassChange(Change):
     """Eclass change."""
+
     name: str
 
     @property
     def prefix(self):
-        return f'{self.name}: '
+        return f"{self.name}: "
 
 
 @dataclass(frozen=True)
 class PkgChange(Change):
     """Package change."""
+
     atom: atom_cls
     ebuild: bool
     old: atom_cls = None
 
     @property
     def prefix(self):
-        return f'{self.atom.key}: '
+        return f"{self.atom.key}: "
 
 
 def determine_msg_args(options, changes):
     """Determine message-related arguments used with `git commit`."""
     args = []
     if options.file:
-        args.extend(['-F', options.file])
+        args.extend(["-F", options.file])
     elif options.template:
-        args.extend(['-t', options.template])
+        args.extend(["-t", options.template])
     else:
         if options.message_template:
-            message = options.message_template.read().splitlines()
+            message: list[str] = options.message_template.read().splitlines()
             try:
-                # TODO: replace with str.removeprefix when py3.8 support dropped
-                if message[0].startswith('*: '):
-                    message[0] = message[0][3:]
+                message[0] = message[0].removeprefix("*: ")
             except IndexError:
-                commit.error(f'empty message template: {options.message_template.name!r}')
+                commit.error(f"empty message template: {options.message_template.name!r}")
         else:
             message = [] if options.message is None else options.message
 
         # determine commit message
         if message:
             # ignore generated prefix when using custom prefix
-            if not re.match(r'^\S+: ', message[0]):
+            if not re.match(r"^\S+: ", message[0]):
                 message[0] = changes.prefix + message[0]
         elif changes.prefix:
             # use generated summary if a generated prefix exists
             message.append(changes.prefix + changes.summary)
         else:
             # use empty string to force user input
-            message.append('')
+            message.append("")
 
-        tmp = tempfile.NamedTemporaryFile(mode='w')
+        tmp = tempfile.NamedTemporaryFile(mode="w")
         tmp.write(message[0])
         if len(message) > 1:
             # wrap body paragraphs at 85 chars
-            body = ('\n'.join(textwrap.wrap(x, width=85)) for x in message[1:])
-            tmp.write('\n\n' + '\n\n'.join(body))
+            body = ("\n".join(textwrap.wrap(x, width=85)) for x in message[1:])
+            tmp.write("\n\n" + "\n\n".join(body))
 
         # add footer tags
         if options.footer:
-            tmp.write('\n\n')
+            tmp.write("\n\n")
             for tag, value in options.footer:
-                tmp.write(f'{tag}: {value}\n')
+                tmp.write(f"{tag}: {value}\n")
 
         tmp.flush()
 
         # force `git commit` to open an editor for uncompleted summary
-        if not message[0] or message[0].endswith(' '):
-            args.extend(['-t', tmp.name])
+        if not message[0] or message[0].endswith(" "):
+            args.extend(["-t", tmp.name])
         else:
-            args.extend(['-F', tmp.name])
+            args.extend(["-F", tmp.name])
 
         # Explicitly register tempfile removal so the object isn't garbage
         # collected and removed when leaving function scope.
         atexit.register(tmp.close)
 
     return args
 
 
 @commit.bind_final_check
 def _commit_validate(parser, namespace):
     # flag for testing if running under the gentoo repo
-    namespace.gentoo_repo = namespace.repo.repo_id == 'gentoo'
+    namespace.gentoo_repo = namespace.repo.repo_id == "gentoo"
 
     # mangle files in the gentoo repo by default
     if namespace.mangle is None and namespace.gentoo_repo:
         namespace.mangle = True
 
     # determine `pkgcheck scan` args
-    namespace.scan_args = ['-v'] * namespace.verbosity
+    namespace.scan_args = ["-v"] * namespace.verbosity
     if namespace.pkgcheck_scan:
         namespace.scan_args.extend(shlex.split(namespace.pkgcheck_scan))
-    namespace.scan_args.extend(['--exit', 'GentooCI', '--staged'])
+    namespace.scan_args.extend(["--exit", "GentooCI", "--staged"])
 
     if namespace.repo.config.sign_commits:
-        namespace.commit_args.append('--gpg-sign')
+        namespace.commit_args.append("--gpg-sign")
 
 
 def update_manifests(options, out, err, changes):
     """Update package manifests for any staged ebuild changes."""
     repo = options.repo
-    untracked_ebuild_re = re.compile(r'^\?\? (?P<category>[^/]+)/[^/]+/(?P<package>[^/]+)\.ebuild$')
+    untracked_ebuild_re = re.compile(r"^\?\? (?P<category>[^/]+)/[^/]+/(?P<package>[^/]+)\.ebuild$")
 
     # update manifests for existing packages
     if atoms := {x.atom.unversioned_atom for x in changes.ebuild_changes}:
         if pkgs := {x.versioned_atom for x in repo.itermatch(packages.OrRestriction(*atoms))}:
             # pull all matches and drop untracked ebuilds
             p = git.run(
-                'status', '--porcelain=v1', '-u', '-z', "*.ebuild",
-                cwd=repo.location, stdout=subprocess.PIPE)
-            for path in p.stdout.strip('\x00').split('\x00'):
+                "status",
+                "--porcelain=v1",
+                "-u",
+                "-z",
+                "*.ebuild",
+                cwd=repo.location,
+                stdout=subprocess.PIPE,
+            )
+            for path in p.stdout.strip("\x00").split("\x00"):
                 if mo := untracked_ebuild_re.match(path):
                     try:
                         untracked = atom_cls(f"={mo.group('category')}/{mo.group('package')}")
                         pkgs.discard(untracked)
                     except MalformedAtom:
                         continue
 
             # manifest all staged or committed packages
             failed = repo.operations.manifest(
-                options.domain, packages.OrRestriction(*pkgs),
+                options.domain,
+                packages.OrRestriction(*pkgs),
                 observer=observer_mod.formatter_output(out),
-                distdir=options.distdir)
+                distdir=options.distdir,
+            )
             if any(failed):
                 return 1
 
             # include existing Manifest files for staging
-            manifests = (pjoin(repo.location, f'{x.key}/Manifest') for x in pkgs)
+            manifests = (pjoin(repo.location, f"{x.key}/Manifest") for x in pkgs)
             options.git_add_files.extend(filter(os.path.exists, manifests))
 
     return 0
 
 
 @commit.bind_main_func
 def _commit(options, out, err):
@@ -803,37 +889,37 @@
     # update package manifests
     if update_manifests(options, out, err, changes):
         return 1
 
     # mangle files
     if options.mangle:
         # don't mangle FILESDIR content
-        skip_regex = re.compile(rf'^{repo.location}/[^/]+/[^/]+/files/.+$')
+        skip_regex = re.compile(rf"^{repo.location}/[^/]+/[^/]+/files/.+$")
         mangler = GentooMangler if options.gentoo_repo else Mangler
         files = mangler(changes.all, skip_regex=skip_regex)
         options.git_add_files.extend(files)
 
     # stage modified files
     if options.git_add_files:
-        git.run('add', *options.git_add_files, cwd=repo.location)
+        git.run("add", *options.git_add_files, cwd=repo.location)
 
     # scan staged changes for QA issues if requested
     if options.scan:
         pipe = scan(options.scan_args)
         with reporters.FancyReporter(out) as reporter:
             for result in pipe:
                 reporter.report(result)
         # fail on errors unless they're ignored
         if pipe.errors:
             with reporters.FancyReporter(out) as reporter:
-                out.write(out.bold, out.fg('red'), '\nFAILURES', out.reset)
+                out.write(out.bold, out.fg("red"), "\nFAILURES", out.reset)
                 for result in sorted(pipe.errors):
                     reporter.report(result)
-            if not (options.ask and userquery('Create commit anyway?', out, err)):
+            if not (options.ask and userquery("Create commit anyway?", out, err)):
                 return 1
 
     # determine message-related args
     args = determine_msg_args(options, changes)
     # create commit
-    git.run('commit', *args, *options.commit_args)
+    git.run("commit", *args, *options.commit_args)
 
     return 0
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_manifest.py` & `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_manifest.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,62 +7,80 @@
 from pkgcore.util.parserestrict import parse_match
 from snakeoil.cli import arghparse
 
 from .. import cli, git
 from .argparsers import cwd_repo_argparser
 
 manifest = cli.ArgumentParser(
-    prog='pkgdev manifest', description='update package manifests',
-    parents=(cwd_repo_argparser,))
+    prog="pkgdev manifest", description="update package manifests", parents=(cwd_repo_argparser,)
+)
 manifest.add_argument(
-    'target', nargs='*',
-    help='packages to target',
+    "target",
+    nargs="*",
+    help="packages to target",
     docs="""
         Packages matching any of these restrictions will have their manifest
         entries updated. If no target is specified a path restriction is
         created based on the current working directory. In other words, if
         ``pkgdev manifest`` is run within an ebuild's directory, all the
         ebuilds within that directory will be manifested.
-    """)
-manifest_opts = manifest.add_argument_group('manifest options')
+    """,
+)
+manifest_opts = manifest.add_argument_group("manifest options")
 manifest_opts.add_argument(
-    '-d', '--distdir', type=arghparse.create_dir, help='target download directory',
+    "-d",
+    "--distdir",
+    type=arghparse.create_dir,
+    help="target download directory",
     docs="""
         Use a specified target directory for downloads instead of the
         configured DISTDIR.
-    """)
+    """,
+)
 manifest_opts.add_argument(
-    '-f', '--force', help='forcibly remanifest packages',
-    action='store_true',
+    "-f",
+    "--force",
+    help="forcibly remanifest packages",
+    action="store_true",
     docs="""
         Force package manifest files to be rewritten. Note that this requires
         downloading all distfiles.
-    """)
+    """,
+)
 manifest_opts.add_argument(
-    '-m', '--mirrors', help='enable fetching from Gentoo mirrors',
-    action='store_true',
+    "-m",
+    "--mirrors",
+    help="enable fetching from Gentoo mirrors",
+    action="store_true",
     docs="""
         Enable checking Gentoo mirrors first for distfiles. This is disabled by
         default because manifest generation is often performed when adding new
         ebuilds with distfiles that aren't on Gentoo mirrors yet.
-    """)
+    """,
+)
 manifest_opts.add_argument(
-    '--if-modified', dest='if_modified', help='Only check packages that have uncommitted modifications',
-    action='store_true',
+    "--if-modified",
+    dest="if_modified",
+    help="Only check packages that have uncommitted modifications",
+    action="store_true",
     docs="""
         In addition to matching the specified restriction, restrict to targets
         which are marked as modified by git, including untracked files.
-    """)
+    """,
+)
 manifest_opts.add_argument(
-    '--ignore-fetch-restricted', dest='ignore_fetch_restricted', help='Ignore fetch restricted ebuilds',
-    action='store_true',
+    "--ignore-fetch-restricted",
+    dest="ignore_fetch_restricted",
+    help="Ignore fetch restricted ebuilds",
+    action="store_true",
     docs="""
         Ignore attempting to update manifest entries for ebuilds which are
         fetch restricted.
-    """)
+    """,
+)
 
 
 def _restrict_targets(repo, targets):
     restrictions = []
     for target in targets:
         if os.path.exists(target):
             try:
@@ -71,46 +89,50 @@
                 restrictions.append(repo.path_restrict(target))
             except ValueError as exc:
                 manifest.error(exc)
         else:
             try:
                 restrictions.append(parse_match(target))
             except ValueError:
-                manifest.error(f'invalid atom: {target!r}')
+                manifest.error(f"invalid atom: {target!r}")
     return packages.OrRestriction(*restrictions)
 
 
 def _restrict_modified_files(repo):
-    ebuild_re = re.compile(r'^[ MTARC?]{2} (?P<path>[^/]+/[^/]+/[^/]+\.ebuild)$')
-    p = git.run('status', '--porcelain=v1', '-z', "*.ebuild",
-                cwd=repo.location, stdout=subprocess.PIPE)
+    ebuild_re = re.compile(r"^[ MTARC?]{2} (?P<path>[^/]+/[^/]+/[^/]+\.ebuild)$")
+    p = git.run(
+        "status", "--porcelain=v1", "-z", "*.ebuild", cwd=repo.location, stdout=subprocess.PIPE
+    )
 
     restrictions = []
-    for line in p.stdout.strip('\x00').split('\x00'):
+    for line in p.stdout.strip("\x00").split("\x00"):
         if mo := ebuild_re.match(line):
-            restrictions.append(repo.path_restrict(mo.group('path')))
+            restrictions.append(repo.path_restrict(mo.group("path")))
     return packages.OrRestriction(*restrictions)
 
 
 @manifest.bind_final_check
 def _manifest_validate(parser, namespace):
     targets = namespace.target if namespace.target else [namespace.cwd]
 
     restrictions = [_restrict_targets(namespace.repo, targets)]
     if namespace.if_modified:
         restrictions.append(_restrict_modified_files(namespace.repo))
     if namespace.ignore_fetch_restricted:
-        restrictions.append(packages.PackageRestriction('restrict', values.ContainmentMatch('fetch', negate=True)))
+        restrictions.append(
+            packages.PackageRestriction("restrict", values.ContainmentMatch("fetch", negate=True))
+        )
     namespace.restriction = packages.AndRestriction(*restrictions)
 
 
 @manifest.bind_main_func
 def _manifest(options, out, err):
     failed = options.repo.operations.manifest(
         domain=options.domain,
         restriction=options.restriction,
         observer=observer_mod.formatter_output(out),
         mirrors=options.mirrors,
         force=options.force,
-        distdir=options.distdir)
+        distdir=options.distdir,
+    )
 
     return int(any(failed))
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_mask.py` & `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_mask.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,123 +19,142 @@
 from snakeoil.osutils import pjoin
 from snakeoil.strings import pluralism
 
 from .. import git
 from .argparsers import cwd_repo_argparser, git_repo_argparser
 
 mask = arghparse.ArgumentParser(
-    prog='pkgdev mask', description='mask packages',
-    parents=(cwd_repo_argparser, git_repo_argparser))
+    prog="pkgdev mask",
+    description="mask packages",
+    parents=(cwd_repo_argparser, git_repo_argparser),
+)
 mask.add_argument(
-    'targets', metavar='TARGET', nargs='*',
-    help='package to mask',
+    "targets",
+    metavar="TARGET",
+    nargs="*",
+    help="package to mask",
     docs="""
         Packages matching any of these restrictions will have a mask entry in
         profiles/package.mask added for them. If no target is specified a path
         restriction is created based on the current working directory. In other
         words, if ``pkgdev mask`` is run within an ebuild's directory, all the
         ebuilds within that directory will be masked.
-    """)
-mask_opts = mask.add_argument_group('mask options')
+    """,
+)
+mask_opts = mask.add_argument_group("mask options")
 mask_opts.add_argument(
-    '-r', '--rites', metavar='DAYS', nargs='?', const=30, type=arghparse.positive_int,
-    help='mark for last rites',
+    "-r",
+    "--rites",
+    metavar="DAYS",
+    nargs="?",
+    const=30,
+    type=arghparse.positive_int,
+    help="mark for last rites",
     docs="""
         Mark a mask entry for last rites. This defaults to 30 days until
         package removal but accepts an optional argument for the number of
         days.
-    """)
+    """,
+)
 mask_opts.add_argument(
-    '-b', '--bug', dest='bugs', action='append', type=arghparse.positive_int,
-    help='reference bug in the mask comment',
+    "-b",
+    "--bug",
+    dest="bugs",
+    action="append",
+    type=arghparse.positive_int,
+    help="reference bug in the mask comment",
     docs="""
         Add a reference to a bug in the mask comment. May be specified multiple
         times to reference multiple bugs.
-    """)
+    """,
+)
 mask_opts.add_argument(
-    '--email', action='store_true',
-    help='spawn email composer with prepared email for sending to mailing lists',
+    "--email",
+    action="store_true",
+    help="spawn email composer with prepared email for sending to mailing lists",
     docs="""
         Spawn user's preferred email composer with a prepared email for
         sending a last rites message to Gentoo's mailing list (``gentoo-dev``
         and ``gentoo-dev-announce``). The user should manually set the Reply-to
         field for the message to be accepted by ``gentoo-dev-announce``.
 
         For spawning the preferred email composer, the ``xdg-email`` tool from
         ``x11-misc/xdg-utils`` package.
-    """)
+    """,
+)
 
 
 @mask.bind_final_check
 def _mask_validate(parser, namespace):
     atoms = []
 
     if namespace.email and not namespace.rites:
-        mask.error('last rites required for email support')
+        mask.error("last rites required for email support")
 
     if namespace.targets:
         for x in namespace.targets:
-            if os.path.exists(x) and x.endswith('.ebuild'):
+            if os.path.exists(x) and x.endswith(".ebuild"):
                 restrict = namespace.repo.path_restrict(x)
                 pkg = next(namespace.repo.itermatch(restrict))
                 atom = pkg.versioned_atom
             else:
                 try:
                     atom = atom_cls(x)
                 except MalformedAtom:
-                    mask.error(f'invalid atom: {x!r}')
+                    mask.error(f"invalid atom: {x!r}")
                 if not namespace.repo.match(atom):
-                    mask.error(f'no repo matches: {x!r}')
+                    mask.error(f"no repo matches: {x!r}")
             atoms.append(atom)
     else:
         restrict = namespace.repo.path_restrict(os.getcwd())
         # repo, category, and package level restricts
         if len(restrict) != 3:
-            mask.error('not in a package directory')
+            mask.error("not in a package directory")
         pkg = next(namespace.repo.itermatch(restrict))
         atoms.append(pkg.unversioned_atom)
 
     namespace.atoms = sorted(atoms)
 
 
 @dataclass(frozen=True)
 class Mask:
     """Entry in package.mask file."""
+
     author: str
     email: str
     date: str
     comment: List[str]
     atoms: List[atom_cls]
 
-    _removal_re = re.compile(r'^Removal: (?P<date>\d{4}-\d{2}-\d{2})')
+    _removal_re = re.compile(r"^Removal: (?P<date>\d{4}-\d{2}-\d{2})")
 
     def __str__(self):
-        lines = [f'# {self.author} <{self.email}> ({self.date})']
-        lines.extend(f'# {x}' if x else '#' for x in self.comment)
+        lines = [f"# {self.author} <{self.email}> ({self.date})"]
+        lines.extend(f"# {x}" if x else "#" for x in self.comment)
         lines.extend(map(str, self.atoms))
-        return '\n'.join(lines)
+        return "\n".join(lines)
 
     @property
     def removal(self):
         """Pull removal date from comment."""
         if mo := self._removal_re.match(self.comment[-1]):
-            return mo.group('date')
+            return mo.group("date")
         return None
 
 
 def consecutive_groups(iterable, ordering=lambda x: x):
     """Return an iterable split into separate, consecutive groups."""
     for k, g in groupby(enumerate(iterable), key=lambda x: x[0] - ordering(x[1])):
         yield map(itemgetter(1), g)
 
 
 class MaskFile:
     """Object representing the contents of a package.mask file."""
 
-    attribution_re = re.compile(r'^(?P<author>.+) <(?P<email>.+)> \((?P<date>\d{4}-\d{2}-\d{2})\)$')
+    attribution_re = re.compile(r"^(?P<author>.+) <(?P<email>.+)> \((?P<date>\d{4}-\d{2}-\d{2})\)$")
 
     def __init__(self, path):
         self.path = path
         self.profile = ProfileNode(os.path.dirname(path))
         self.header = []
         self.masks = deque()
 
@@ -156,132 +175,143 @@
             # use profile's EAPI setting to coerce supported masks
             atoms = [self.profile.eapi_atom(mask_map[x]) for x in mask_lines]
 
             # pull comment lines above initial mask entry line
             comment = []
             i = mask_lines[0] - 2
             while i >= 0 and (line := lines[i].rstrip()):
-                if not line.startswith('# ') and line != '#':
-                    mask.error(f'invalid mask entry header, lineno {i + 1}: {line!r}')
+                if not line.startswith("# ") and line != "#":
+                    mask.error(f"invalid mask entry header, lineno {i + 1}: {line!r}")
                 comment.append(line[2:])
                 i -= 1
             if not self.header:
-                self.header = lines[:i + 1]
+                self.header = lines[: i + 1]
             comment = list(reversed(comment))
 
             # pull attribution data from first comment line
             if mo := self.attribution_re.match(comment[0]):
-                author, email, date = mo.group('author'), mo.group('email'), mo.group('date')
+                author, email, date = mo.group("author"), mo.group("email"), mo.group("date")
             else:
-                mask.error(f'invalid author, lineno {i + 2}: {comment[0]!r}')
+                mask.error(f"invalid author, lineno {i + 2}: {comment[0]!r}")
 
             self.masks.append(Mask(author, email, date, comment[1:], atoms))
 
     def add(self, mask):
         """Add a new mask to the file."""
         self.masks.appendleft(mask)
 
     def write(self):
         """Serialize the registered masks back to the related file."""
-        with open(self.path, 'w') as f:
-            f.write(f'{self}\n')
+        with open(self.path, "w") as f:
+            f.write(f"{self}\n")
 
     def __str__(self):
-        return ''.join(self.header) + '\n\n'.join(map(str, self.masks))
+        return "".join(self.header) + "\n\n".join(map(str, self.masks))
 
 
 def get_comment(bugs, rites: int):
     """Spawn editor to get mask comment."""
-    tmp = tempfile.NamedTemporaryFile(mode='w')
+    tmp = tempfile.NamedTemporaryFile(mode="w")
     summary = []
     if rites:
-        summary.append(f'Removal: {datetime.now(timezone.utc) + timedelta(days=rites):%Y-%m-%d}.')
+        summary.append(f"Removal: {datetime.now(timezone.utc) + timedelta(days=rites):%Y-%m-%d}.")
     if bugs:
         # Bug(s) #A, #B, #C
-        bug_list = ", ".join(f'#{b}' for b in bugs)
+        bug_list = ", ".join(f"#{b}" for b in bugs)
         s = pluralism(bugs)
-        summary.append(f'Bug{s} {bug_list}.')
-    if summary := '  '.join(summary):
-        tmp.write(f'\n{summary}')
-    tmp.write(textwrap.dedent("""
-
-        # Please enter the mask message. Lines starting with '#' will be ignored.
-        #
-        # - Best last rites (removal) practices -
-        #
-        # Include the following info:
-        # a) reason for masking
-        # b) bug # for the removal (and yes you should have one)
-        # c) date of removal (either the date or "in x days")
-        #
-        # Example:
-        #
-        # Masked for removal in 30 days.  Doesn't work
-        # with new libfoo. Upstream dead, gtk-1, smells
-        # funny.
-        # Bug #987654
-    """))
+        summary.append(f"Bug{s} {bug_list}.")
+    if summary := "  ".join(summary):
+        tmp.write(f"\n{summary}")
+    tmp.write(
+        textwrap.dedent(
+            """
+
+                # Please enter the mask message. Lines starting with '#' will be ignored.
+                #
+                # - Best last rites (removal) practices -
+                #
+                # Include the following info:
+                # a) reason for masking
+                # b) bug # for the removal (and yes you should have one)
+                # c) date of removal (either the date or "in x days")
+                #
+                # Example:
+                #
+                # Masked for removal in 30 days.  Doesn't work
+                # with new libfoo. Upstream dead, gtk-1, smells
+                # funny.
+                # Bug #987654
+            """
+        )
+    )
     tmp.flush()
 
-    editor = shlex.split(os.environ.get('VISUAL', os.environ.get('EDITOR', 'nano')))
+    editor = shlex.split(os.environ.get("VISUAL", os.environ.get("EDITOR", "nano")))
     try:
         subprocess.run(editor + [tmp.name], check=True)
     except subprocess.CalledProcessError:
-        mask.error('failed writing mask comment')
+        mask.error("failed writing mask comment")
     except FileNotFoundError:
-        mask.error(f'nonexistent editor: {editor[0]!r}')
+        mask.error(f"nonexistent editor: {editor[0]!r}")
 
     with open(tmp.name) as f:
         # strip trailing whitespace from lines
         comment = (x.rstrip() for x in f.readlines())
     # strip comments
-    comment = (x for x in comment if not x.startswith('#'))
+    comment = (x for x in comment if not x.startswith("#"))
     # strip leading/trailing newlines
-    comment = '\n'.join(comment).strip().splitlines()
+    comment = "\n".join(comment).strip().splitlines()
     if not comment:
-        mask.error('empty mask comment')
+        mask.error("empty mask comment")
 
     return comment
 
 
 def send_last_rites_email(m: Mask, subject_prefix: str):
     try:
-        atoms = ', '.join(map(str, m.atoms))
-        subprocess.run(args=[
-            'xdg-email', '--utf8',
-            '--cc', 'gentoo-dev@lists.gentoo.org',
-            '--subject', f'{subject_prefix}: {atoms}',
-            '--body', str(m),
-            'gentoo-dev-announce@lists.gentoo.org'
-        ], check=True)
+        atoms = ", ".join(map(str, m.atoms))
+        subprocess.run(
+            args=[
+                "xdg-email",
+                "--utf8",
+                "--cc",
+                "gentoo-dev@lists.gentoo.org",
+                "--subject",
+                f"{subject_prefix}: {atoms}",
+                "--body",
+                str(m),
+                "gentoo-dev-announce@lists.gentoo.org",
+            ],
+            check=True,
+        )
     except subprocess.CalledProcessError:
-        mask.error('failed opening email composer')
+        mask.error("failed opening email composer")
 
 
 @mask.bind_main_func
 def _mask(options, out, err):
-    mask_file = MaskFile(pjoin(options.repo.location, 'profiles/package.mask'))
+    mask_file = MaskFile(pjoin(options.repo.location, "profiles/package.mask"))
     today = datetime.now(timezone.utc)
 
     # pull name/email from git config
-    p = git.run('config', 'user.name', stdout=subprocess.PIPE)
+    p = git.run("config", "user.name", stdout=subprocess.PIPE)
     author = p.stdout.strip()
-    p = git.run('config', 'user.email', stdout=subprocess.PIPE)
+    p = git.run("config", "user.email", stdout=subprocess.PIPE)
     email = p.stdout.strip()
 
     # initial args for Mask obj
     mask_args = {
-        'author': author,
-        'email': email,
-        'date': today.strftime('%Y-%m-%d'),
-        'comment': get_comment(options.bugs, options.rites),
-        'atoms': options.atoms,
+        "author": author,
+        "email": email,
+        "date": today.strftime("%Y-%m-%d"),
+        "comment": get_comment(options.bugs, options.rites),
+        "atoms": options.atoms,
     }
 
     m = Mask(**mask_args)
     mask_file.add(m)
     mask_file.write()
 
     if options.email:
-        send_last_rites_email(m, 'Last rites')
+        send_last_rites_email(m, "Last rites")
 
     return 0
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_push.py` & `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_push.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,62 +11,67 @@
 
 class ArgumentParser(cli.ArgumentParser):
     """Parse all known arguments, passing unknown arguments to ``git push``."""
 
     def parse_known_args(self, args=None, namespace=None):
         namespace, args = super().parse_known_args(args, namespace)
         if namespace.dry_run:
-            args.append('--dry-run')
+            args.append("--dry-run")
         namespace.push_args = args
         return namespace, []
 
 
 push = ArgumentParser(
-    prog='pkgdev push', description='run QA checks on commits and push them',
-    parents=(cwd_repo_argparser, git_repo_argparser))
+    prog="pkgdev push",
+    description="run QA checks on commits and push them",
+    parents=(cwd_repo_argparser, git_repo_argparser),
+)
 # custom `pkgcheck scan` args used for tests
-push.add_argument('--pkgcheck-scan', help=argparse.SUPPRESS)
-push_opts = push.add_argument_group('push options')
+push.add_argument("--pkgcheck-scan", help=argparse.SUPPRESS)
+push_opts = push.add_argument_group("push options")
 push_opts.add_argument(
-    '-A', '--ask', nargs='?', const=True, action=arghparse.StoreBool,
-    help='confirm pushing commits with QA errors')
+    "-A",
+    "--ask",
+    nargs="?",
+    const=True,
+    action=arghparse.StoreBool,
+    help="confirm pushing commits with QA errors",
+)
+push_opts.add_argument("-n", "--dry-run", action="store_true", help="pretend to push the commits")
 push_opts.add_argument(
-    '-n', '--dry-run', action='store_true',
-    help='pretend to push the commits')
-push_opts.add_argument(
-    '--pull', action='store_true',
-    help='run `git pull --rebase` before scanning')
+    "--pull", action="store_true", help="run `git pull --rebase` before scanning"
+)
 
 
 @push.bind_final_check
 def _commit_validate(parser, namespace):
     # determine `pkgcheck scan` args
-    namespace.scan_args = ['-v'] * namespace.verbosity
+    namespace.scan_args = ["-v"] * namespace.verbosity
     if namespace.pkgcheck_scan:
         namespace.scan_args.extend(shlex.split(namespace.pkgcheck_scan))
-    namespace.scan_args.extend(['--exit', 'GentooCI', '--commits'])
+    namespace.scan_args.extend(["--exit", "GentooCI", "--commits"])
 
 
 @push.bind_main_func
 def _push(options, out, err):
     if options.pull:
-        git.run('pull', '--rebase', cwd=options.repo.location)
+        git.run("pull", "--rebase", cwd=options.repo.location)
 
     # scan commits for QA issues
     pipe = scan(options.scan_args)
     with reporters.FancyReporter(out) as reporter:
         for result in pipe:
             reporter.report(result)
 
     # fail on errors unless they're ignored
     if pipe.errors:
         with reporters.FancyReporter(out) as reporter:
-            out.write(out.bold, out.fg('red'), '\nFAILURES', out.reset)
+            out.write(out.bold, out.fg("red"), "\nFAILURES", out.reset)
             for result in sorted(pipe.errors):
                 reporter.report(result)
-        if not (options.ask and userquery('Push commits anyway?', out, err)):
+        if not (options.ask and userquery("Push commits anyway?", out, err)):
             return 1
 
     # push commits upstream
-    git.run('push', *options.push_args, cwd=options.repo.location)
+    git.run("push", *options.push_args, cwd=options.repo.location)
 
     return 0
```

### Comparing `pkgdev-0.2.4/src/pkgdev/scripts/pkgdev_showkw.py` & `pkgdev-0.2.5/src/pkgdev/scripts/pkgdev_showkw.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,157 +8,169 @@
 from pkgcore.util import packages as pkgutils
 from snakeoil.strings import pluralism
 
 from .. import cli
 from .._vendor.tabulate import tabulate, tabulate_formats
 
 
-showkw = cli.ArgumentParser(
-    prog='pkgdev showkw', description='show package keywords')
+showkw = cli.ArgumentParser(prog="pkgdev showkw", description="show package keywords")
 showkw.add_argument(
-    'targets', metavar='target', nargs='*',
+    "targets",
+    metavar="target",
+    nargs="*",
     action=commandline.StoreTarget,
-    help='extended atom matching of packages')
+    help="extended atom matching of packages",
+)
 
-output_opts = showkw.add_argument_group('output options')
+output_opts = showkw.add_argument_group("output options")
 output_opts.add_argument(
-    '-f', '--format', default='showkw', metavar='FORMAT',
+    "-f",
+    "--format",
+    default="showkw",
+    metavar="FORMAT",
     choices=tabulate_formats,
-    help='keywords table format',
+    help="keywords table format",
     docs=f"""
         Output table using specified tabular format (defaults to compressed,
         custom format).
 
         Available formats: {', '.join(tabulate_formats)}
-    """)
+    """,
+)
 output_opts.add_argument(
-    '-c', '--collapse', action='store_true',
-    help='show collapsed list of arches')
+    "-c", "--collapse", action="store_true", help="show collapsed list of arches"
+)
 
-arch_options = showkw.add_argument_group('arch options')
+arch_options = showkw.add_argument_group("arch options")
+arch_options.add_argument("-s", "--stable", action="store_true", help="show stable arches")
+arch_options.add_argument("-u", "--unstable", action="store_true", help="show unstable arches")
 arch_options.add_argument(
-    '-s', '--stable', action='store_true',
-    help='show stable arches')
+    "-o",
+    "--only-unstable",
+    action="store_true",
+    help="show arches that only have unstable keywords",
+)
 arch_options.add_argument(
-    '-u', '--unstable', action='store_true',
-    help='show unstable arches')
-arch_options.add_argument(
-    '-o', '--only-unstable', action='store_true',
-    help='show arches that only have unstable keywords')
-arch_options.add_argument(
-    '-p', '--prefix', action='store_true',
-    help='show prefix and non-native arches')
-arch_options.add_argument(
-    '-a', '--arch', action='csv_negations',
-    help='select arches to display')
+    "-p", "--prefix", action="store_true", help="show prefix and non-native arches"
+)
+arch_options.add_argument("-a", "--arch", action="csv_negations", help="select arches to display")
 
 # TODO: allow multi-repo comma-separated input
-target_opts = showkw.add_argument_group('target options')
+target_opts = showkw.add_argument_group("target options")
 target_opts.add_argument(
-    '-r', '--repo', dest='selected_repo', metavar='REPO', priority=29,
+    "-r",
+    "--repo",
+    dest="selected_repo",
+    metavar="REPO",
+    priority=29,
     action=commandline.StoreRepoObject,
-    repo_type='all-raw', allow_external_repos=True,
-    help='repo to query (defaults to all ebuild repos)')
-@showkw.bind_delayed_default(30, 'repos')
+    repo_type="all-raw",
+    allow_external_repos=True,
+    help="repo to query (defaults to all ebuild repos)",
+)
+
+
+@showkw.bind_delayed_default(30, "repos")
 def _setup_repos(namespace, attr):
     target_repo = namespace.selected_repo
     all_ebuild_repos = namespace.domain.all_ebuild_repos_raw
     namespace.cwd = os.getcwd()
 
     # TODO: move this to StoreRepoObject
     if target_repo is None:
         # determine target repo from the target directory
         for repo in all_ebuild_repos.trees:
             if namespace.cwd in repo:
                 target_repo = repo
                 break
         else:
             # determine if CWD is inside an unconfigured repo
-            target_repo = namespace.domain.find_repo(
-                namespace.cwd, config=namespace.config)
+            target_repo = namespace.domain.find_repo(namespace.cwd, config=namespace.config)
 
     # fallback to using all, unfiltered ebuild repos if no target repo can be found
     namespace.repo = target_repo if target_repo is not None else all_ebuild_repos
 
 
-@showkw.bind_delayed_default(40, 'arches')
+@showkw.bind_delayed_default(40, "arches")
 def _setup_arches(namespace, attr):
-    default_repo = namespace.config.get_default('repo')
+    default_repo = namespace.config.get_default("repo")
 
     try:
-        known_arches = {arch for r in namespace.repo.trees
-                        for arch in r.config.known_arches}
+        known_arches = {arch for r in namespace.repo.trees for arch in r.config.known_arches}
     except AttributeError:
         try:
             # binary/vdb repos use known arches from the default repo
             known_arches = default_repo.config.known_arches
         except AttributeError:
             # TODO: remove fallback for tests after fixing default repo pull
             # from faked config
             known_arches = set()
 
     arches = known_arches
     if namespace.arch is not None:
         disabled_arches, enabled_arches = namespace.arch
         disabled_arches = set(disabled_arches)
         enabled_arches = set(enabled_arches)
-        unknown_arches = disabled_arches.difference(known_arches) | enabled_arches.difference(known_arches)
+        unknown_arches = disabled_arches.difference(known_arches) | enabled_arches.difference(
+            known_arches
+        )
         if unknown_arches:
-            unknown = ', '.join(map(repr, sorted(unknown_arches)))
-            known = ', '.join(sorted(known_arches))
-            es = pluralism(unknown_arches, plural='es')
-            showkw.error(f'unknown arch{es}: {unknown} (choices: {known})')
+            unknown = ", ".join(map(repr, sorted(unknown_arches)))
+            known = ", ".join(sorted(known_arches))
+            es = pluralism(unknown_arches, plural="es")
+            showkw.error(f"unknown arch{es}: {unknown} (choices: {known})")
         if enabled_arches:
             arches = arches.intersection(enabled_arches)
         if disabled_arches:
             arches = arches - disabled_arches
 
-    prefix_arches = set(x for x in arches if '-' in x)
+    prefix_arches = set(x for x in arches if "-" in x)
     native_arches = arches.difference(prefix_arches)
     arches = native_arches
     if namespace.prefix:
         arches = arches.union(prefix_arches)
     if namespace.stable:
         try:
-            stable_arches = {arch for r in namespace.repo.trees
-                             for arch in r.config.profiles.arches('stable')}
+            stable_arches = {
+                arch for r in namespace.repo.trees for arch in r.config.profiles.arches("stable")
+            }
         except AttributeError:
             # binary/vdb repos use stable arches from the default repo
-            stable_arches = default_repo.config.profiles.arches('stable')
+            stable_arches = default_repo.config.profiles.arches("stable")
         arches = arches.intersection(stable_arches)
 
     namespace.known_arches = known_arches
     namespace.prefix_arches = prefix_arches
     namespace.native_arches = native_arches
     namespace.arches = arches
 
 
 def _colormap(colors, line):
     if colors is None:
         return line
-    return colors[line] + line + colors['reset']
+    return colors[line] + line + colors["reset"]
 
 
 @showkw.bind_final_check
 def _validate_args(parser, namespace):
     namespace.pkg_dir = False
 
     # disable colors when not using the native output format
-    if namespace.format != 'showkw':
+    if namespace.format != "showkw":
         namespace.color = False
 
     if namespace.color:
         # default colors to use for keyword types
         _COLORS = {
-            '+': '\u001b[32m',
-            '~': '\u001b[33m',
-            '-': '\u001b[31m',
-            '*': '\u001b[31m',
-            'o': '\u001b[90;1m',
-            'reset': '\u001b[0m',
+            "+": "\u001b[32m",
+            "~": "\u001b[33m",
+            "-": "\u001b[31m",
+            "*": "\u001b[31m",
+            "o": "\u001b[90;1m",
+            "reset": "\u001b[0m",
         }
     else:
         _COLORS = None
     namespace.colormap = partial(_colormap, _COLORS)
 
     if not namespace.targets:
         if namespace.selected_repo:
@@ -169,87 +181,87 @@
             # Use a path restriction if we're in a repo, obviously it'll work
             # faster if we're in an invididual ebuild dir but we're not that
             # restrictive.
             try:
                 restriction = namespace.repo.path_restrict(namespace.cwd)
                 token = namespace.cwd
             except (AttributeError, ValueError):
-                parser.error('missing target argument and not in a supported repo')
+                parser.error("missing target argument and not in a supported repo")
 
             # determine if we're grabbing the keywords for a single pkg in cwd
             namespace.pkg_dir = any(
-                isinstance(x, restricts.PackageDep)
-                for x in reversed(restriction.restrictions))
+                isinstance(x, restricts.PackageDep) for x in reversed(restriction.restrictions)
+            )
 
         namespace.targets = [(token, restriction)]
 
 
 def _collapse_arches(options, pkgs):
     """Collapse arches into a single set."""
     keywords = set()
     stable_keywords = set()
     unstable_keywords = set()
     for pkg in pkgs:
         for x in pkg.keywords:
-            if x[0] == '~':
+            if x[0] == "~":
                 unstable_keywords.add(x[1:])
             elif x in options.arches:
                 stable_keywords.add(x)
     if options.unstable:
         keywords.update(unstable_keywords)
     if options.only_unstable:
         keywords.update(unstable_keywords.difference(stable_keywords))
     if not keywords or options.stable:
         keywords.update(stable_keywords)
-    return (
-        sorted(keywords.intersection(options.native_arches)) +
-        sorted(keywords.intersection(options.prefix_arches)))
+    return sorted(keywords.intersection(options.native_arches)) + sorted(
+        keywords.intersection(options.prefix_arches)
+    )
 
 
 def _render_rows(options, pkgs, arches):
     """Build rows for tabular data output."""
     for pkg in sorted(pkgs):
         keywords = set(pkg.keywords)
         row = [pkg.fullver]
         for arch in arches:
             if arch in keywords:
-                line = '+'
-            elif f'~{arch}' in keywords:
-                line = '~'
-            elif f'-{arch}' in keywords:
-                line = '-'
-            elif '-*' in keywords:
-                line = '*'
+                line = "+"
+            elif f"~{arch}" in keywords:
+                line = "~"
+            elif f"-{arch}" in keywords:
+                line = "-"
+            elif "-*" in keywords:
+                line = "*"
             else:
-                line = 'o'
+                line = "o"
             row.append(options.colormap(line))
         row.extend([pkg.eapi, pkg.fullslot, pkg.repo.repo_id])
         yield row
 
 
 @showkw.bind_main_func
 def main(options, out, err):
     continued = False
     for token, restriction in options.targets:
         for pkgs in pkgutils.groupby_pkg(options.repo.itermatch(restriction, sorter=sorted)):
             if options.collapse:
-                out.write(' '.join(_collapse_arches(options, pkgs)))
+                out.write(" ".join(_collapse_arches(options, pkgs)))
             else:
                 arches = sorted(options.arches.intersection(options.native_arches))
                 if options.prefix:
                     arches += sorted(options.arches.intersection(options.prefix_arches))
-                headers = [''] + arches + ['eapi', 'slot', 'repo']
+                headers = [""] + arches + ["eapi", "slot", "repo"]
                 if continued:
                     out.write()
                 if not options.pkg_dir:
                     pkgs = list(pkgs)
-                    out.write(f'keywords for {pkgs[0].unversioned_atom}:')
+                    out.write(f"keywords for {pkgs[0].unversioned_atom}:")
                 data = _render_rows(options, pkgs, arches)
                 table = tabulate(
-                    data, headers=headers, tablefmt=options.format,
-                    disable_numparse=True)
+                    data, headers=headers, tablefmt=options.format, disable_numparse=True
+                )
                 out.write(table)
             continued = True
 
     if not continued:
         err.write(f"{options.prog}: no matches for {token!r}")
         return 1
```

### Comparing `pkgdev-0.2.4/tests/conftest.py` & `pkgdev-0.2.5/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from pkgdev.cli import Tool
 from pkgdev.scripts import pkgdev
 from snakeoil.cli import arghparse
 
-pytest_plugins = ['pkgcore']
+pytest_plugins = ["pkgcore"]
 
 
 @pytest.fixture(scope="session")
 def tool():
     """Generate a tool utility for running pkgdev."""
     return Tool(pkgdev.argparser)
```

### Comparing `pkgdev-0.2.4/tests/scripts/test_cli.py` & `pkgdev-0.2.5/tests/scripts/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,89 +2,104 @@
 
 import pytest
 from pkgdev import cli
 from snakeoil.cli import arghparse
 
 
 class TestConfigFileParser:
-
     @pytest.fixture(autouse=True)
     def _create_argparser(self, tmp_path):
-        self.config_file = str(tmp_path / 'config')
-        self.parser = arghparse.ArgumentParser(prog='pkgdev cli_test')
+        self.config_file = str(tmp_path / "config")
+        self.parser = arghparse.ArgumentParser(prog="pkgdev cli_test")
         self.namespace = arghparse.Namespace()
         self.config_parser = cli.ConfigFileParser(self.parser)
 
     def test_no_configs(self):
         config = self.config_parser.parse_config(())
         assert config.sections() == []
         namespace = self.config_parser.parse_config_options(self.namespace)
         assert vars(namespace) == {}
 
     def test_ignored_configs(self):
         # nonexistent config files are ignored
-        config = self.config_parser.parse_config(('foo', 'bar'))
+        config = self.config_parser.parse_config(("foo", "bar"))
         assert config.sections() == []
 
     def test_bad_config_format_no_section(self, capsys):
-        with open(self.config_file, 'w') as f:
-            f.write('foobar\n')
+        with open(self.config_file, "w") as f:
+            f.write("foobar\n")
         with pytest.raises(SystemExit) as excinfo:
             self.config_parser.parse_config((self.config_file,))
         out, err = capsys.readouterr()
         assert not out
-        assert 'parsing config file failed: File contains no section headers' in err
+        assert "parsing config file failed: File contains no section headers" in err
         assert self.config_file in err
         assert excinfo.value.code == 2
 
     def test_bad_config_format(self, capsys):
-        with open(self.config_file, 'w') as f:
-            f.write(textwrap.dedent("""
-                [DEFAULT]
-                foobar
-            """))
+        with open(self.config_file, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """
+                        [DEFAULT]
+                        foobar
+                    """
+                )
+            )
         with pytest.raises(SystemExit) as excinfo:
             self.config_parser.parse_config((self.config_file,))
         out, err = capsys.readouterr()
         assert not out
-        assert 'parsing config file failed: Source contains parsing errors' in err
+        assert "parsing config file failed: Source contains parsing errors" in err
         assert excinfo.value.code == 2
 
     def test_nonexistent_config_options(self, capsys):
         """Nonexistent parser arguments don't cause errors."""
-        with open(self.config_file, 'w') as f:
-            f.write(textwrap.dedent("""
-                [DEFAULT]
-                cli_test.foo=bar
-            """))
+        with open(self.config_file, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """
+                        [DEFAULT]
+                        cli_test.foo=bar
+                    """
+                )
+            )
         with pytest.raises(SystemExit) as excinfo:
             self.config_parser.parse_config_options(None, configs=(self.config_file,))
         out, err = capsys.readouterr()
         assert not out
-        assert 'failed loading config: unknown arguments: --foo=bar' in err
+        assert "failed loading config: unknown arguments: --foo=bar" in err
         assert excinfo.value.code == 2
 
     def test_config_options_other_prog(self):
-        self.parser.add_argument('--foo')
-        with open(self.config_file, 'w') as f:
-            f.write(textwrap.dedent("""
-                [DEFAULT]
-                other.foo=bar
-            """))
-        namespace = self.parser.parse_args(['--foo', 'foo'])
-        assert namespace.foo == 'foo'
+        self.parser.add_argument("--foo")
+        with open(self.config_file, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """
+                        [DEFAULT]
+                        other.foo=bar
+                    """
+                )
+            )
+        namespace = self.parser.parse_args(["--foo", "foo"])
+        assert namespace.foo == "foo"
         # config args don't override not matching namespace attrs
         namespace = self.config_parser.parse_config_options(namespace, configs=[self.config_file])
-        assert namespace.foo == 'foo'
+        assert namespace.foo == "foo"
 
     def test_config_options(self):
-        self.parser.add_argument('--foo')
-        with open(self.config_file, 'w') as f:
-            f.write(textwrap.dedent("""
-                [DEFAULT]
-                cli_test.foo=bar
-            """))
-        namespace = self.parser.parse_args(['--foo', 'foo'])
-        assert namespace.foo == 'foo'
+        self.parser.add_argument("--foo")
+        with open(self.config_file, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """
+                        [DEFAULT]
+                        cli_test.foo=bar
+                    """
+                )
+            )
+        namespace = self.parser.parse_args(["--foo", "foo"])
+        assert namespace.foo == "foo"
         # config args override matching namespace attrs
         namespace = self.config_parser.parse_config_options(namespace, configs=[self.config_file])
-        assert namespace.foo == 'bar'
+        assert namespace.foo == "bar"
```

### Comparing `pkgdev-0.2.4/tests/scripts/test_pkgdev.py` & `pkgdev-0.2.5/tests/scripts/test_pkgdev.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,46 +8,45 @@
 from pkgdev.scripts import run
 
 
 def test_script_run(capsys):
     """Test regular code path for running scripts."""
     script = partial(run, project)
 
-    with patch(f'{project}.scripts.import_module') as import_module:
+    with patch(f"{project}.scripts.import_module") as import_module:
         import_module.side_effect = ImportError("baz module doesn't exist")
 
         # default error path when script import fails
-        with patch('sys.argv', [project]):
+        with patch("sys.argv", [project]):
             with pytest.raises(SystemExit) as excinfo:
                 script()
             assert excinfo.value.code == 1
             out, err = capsys.readouterr()
-            err = err.strip().split('\n')
+            err = err.strip().split("\n")
             assert len(err) == 3
             assert err[0] == "Failed importing: baz module doesn't exist!"
             assert err[1].startswith(f"Verify that {project} and its deps")
             assert err[2] == "Add --debug to the commandline for a traceback."
 
         # running with --debug should raise an ImportError when there are issues
-        with patch('sys.argv', [project, '--debug']):
+        with patch("sys.argv", [project, "--debug"]):
             with pytest.raises(ImportError):
                 script()
             out, err = capsys.readouterr()
-            err = err.strip().split('\n')
+            err = err.strip().split("\n")
             assert len(err) == 2
             assert err[0] == "Failed importing: baz module doesn't exist!"
             assert err[1].startswith(f"Verify that {project} and its deps")
 
         import_module.reset_mock()
 
 
 class TestPkgdev:
-
     script = staticmethod(partial(run, project))
 
     def test_version(self, capsys):
-        with patch('sys.argv', [project, '--version']):
+        with patch("sys.argv", [project, "--version"]):
             with pytest.raises(SystemExit) as excinfo:
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
             assert out.startswith(project)
```

### Comparing `pkgdev-0.2.4/tests/scripts/test_pkgdev_commit.py` & `pkgdev-0.2.5/tests/scripts/test_pkgdev_commit.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,1034 +10,1090 @@
 from pkgdev.mangle import copyright_regex, keywords_regex
 from pkgdev.scripts import run
 from snakeoil.contexts import chdir, os_environ
 from snakeoil.osutils import pjoin
 
 
 class TestPkgdevCommitParseArgs:
-
     def test_non_repo_cwd(self, capsys, tool):
         with pytest.raises(SystemExit) as excinfo:
-            tool.parse_args(['commit'])
+            tool.parse_args(["commit"])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
-        assert err.strip() == 'pkgdev commit: error: not in ebuild repo'
+        assert err.strip() == "pkgdev commit: error: not in ebuild repo"
 
     def test_bad_repo_cwd(self, make_repo, capsys, tool):
-        repo = make_repo(masters=('nonexistent',))
-        with pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
-            tool.parse_args(['commit'])
+        repo = make_repo(masters=("nonexistent",))
+        with pytest.raises(SystemExit) as excinfo, chdir(repo.location):
+            tool.parse_args(["commit"])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
-        assert err.strip().startswith('pkgdev commit: error: repo init failed')
+        assert err.strip().startswith("pkgdev commit: error: repo init failed")
 
     def test_non_git_repo_cwd(self, repo, capsys, tool):
-        with pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
-            tool.parse_args(['commit'])
+        with pytest.raises(SystemExit) as excinfo, chdir(repo.location):
+            tool.parse_args(["commit"])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
-        assert err.strip() == 'pkgdev commit: error: not in git repo'
+        assert err.strip() == "pkgdev commit: error: not in git repo"
 
     def test_non_ebuild_git_repo_cwd(self, make_repo, git_repo, capsys, tool):
-        os.mkdir(pjoin(git_repo.path, 'repo'))
-        repo = make_repo(pjoin(git_repo.path, 'repo'))
-        with pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
-            tool.parse_args(['commit'])
+        os.mkdir(pjoin(git_repo.path, "repo"))
+        repo = make_repo(pjoin(git_repo.path, "repo"))
+        with pytest.raises(SystemExit) as excinfo, chdir(repo.location):
+            tool.parse_args(["commit"])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
-        assert err.strip() == 'pkgdev commit: error: not in ebuild git repo'
+        assert err.strip() == "pkgdev commit: error: not in ebuild git repo"
 
     def test_commit_signing(self, repo, make_git_repo, tool):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0', commit=False)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0", commit=False)
         # signed commits aren't enabled by default
         with chdir(repo.location):
-            options, _ = tool.parse_args(['commit', '-u'])
-            assert '--signoff' not in options.commit_args
-            assert '--gpg-sign' not in options.commit_args
-
-            options, _ = tool.parse_args(['commit', '-u', '--signoff'])
-            assert '--signoff' in options.commit_args
-            assert '--gpg-sign' not in options.commit_args
+            options, _ = tool.parse_args(["commit", "-u"])
+            assert "--signoff" not in options.commit_args
+            assert "--gpg-sign" not in options.commit_args
+
+            options, _ = tool.parse_args(["commit", "-u", "--signoff"])
+            assert "--signoff" in options.commit_args
+            assert "--gpg-sign" not in options.commit_args
         # signed commits enabled by layout.conf setting
-        with open(pjoin(git_repo.path, 'metadata/layout.conf'), 'a+') as f:
-            f.write('sign-commits = true\n')
+        with open(pjoin(git_repo.path, "metadata/layout.conf"), "a+") as f:
+            f.write("sign-commits = true\n")
         with chdir(repo.location):
-            options, _ = tool.parse_args(['commit', '-u'])
-            assert '--signoff' not in options.commit_args
-            assert '--gpg-sign' in options.commit_args
-
-            options, _ = tool.parse_args(['commit', '-u', '--signoff'])
-            assert '--signoff' in options.commit_args
-            assert '--gpg-sign' in options.commit_args
+            options, _ = tool.parse_args(["commit", "-u"])
+            assert "--signoff" not in options.commit_args
+            assert "--gpg-sign" in options.commit_args
+
+            options, _ = tool.parse_args(["commit", "-u", "--signoff"])
+            assert "--signoff" in options.commit_args
+            assert "--gpg-sign" in options.commit_args
 
     def test_git_commit_args(self, repo, make_git_repo, tool):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0', commit=False)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0", commit=False)
         with chdir(repo.location):
             for opt, expected in (
-                    ('-n', '--dry-run'),
-                    ('--dry-run', '--dry-run'),
-                    ('-v', '-v'),
-                    ('--verbose', '-v'),
-                    ('-e', '--edit'),
-                    ('--edit', '--edit'),
-                    ):
-                options, _ = tool.parse_args(['commit', opt])
+                ("-n", "--dry-run"),
+                ("--dry-run", "--dry-run"),
+                ("-v", "-v"),
+                ("--verbose", "-v"),
+                ("-e", "--edit"),
+                ("--edit", "--edit"),
+            ):
+                options, _ = tool.parse_args(["commit", opt])
                 assert expected in options.commit_args
 
     def test_git_commit_args_passthrough(self, repo, make_git_repo, tool):
         """Unknown arguments for ``pkgdev commit`` are passed to ``git commit``."""
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0', commit=False)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0", commit=False)
         with chdir(repo.location):
-            for opt in ('--author="A U Thor <author@example.com>"', '-p'):
-                options, _ = tool.parse_args(['commit', opt])
+            for opt in ('--author="A U Thor <author@example.com>"', "-p"):
+                options, _ = tool.parse_args(["commit", opt])
             assert options.commit_args == [opt]
 
     def test_scan_args(self, repo, make_git_repo, tool):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0', commit=False)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0", commit=False)
         # pkgcheck isn't run in verbose mode by default
         with chdir(repo.location):
-            options, _ = tool.parse_args(['commit'])
-        assert '-v' not in options.scan_args
+            options, _ = tool.parse_args(["commit"])
+        assert "-v" not in options.scan_args
         # verbosity level is passed down to pkgcheck
         with chdir(repo.location):
-            options, _ = tool.parse_args(['commit', '-v'])
-        assert '-v' in options.scan_args
+            options, _ = tool.parse_args(["commit", "-v"])
+        assert "-v" in options.scan_args
 
     def test_commit_tags(self, capsys, repo, make_git_repo, tool):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0', commit=False)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0", commit=False)
         with chdir(repo.location):
             # bug IDs
-            for opt in ('-b', '--bug'):
-                options, _ = tool.parse_args(['commit', opt, '1'])
-                assert options.footer == {('Bug', 'https://bugs.gentoo.org/1')}
+            for opt in ("-b", "--bug"):
+                options, _ = tool.parse_args(["commit", opt, "1"])
+                assert options.footer == {("Bug", "https://bugs.gentoo.org/1")}
 
             # bug URLs
-            for opt in ('-b', '--bug'):
-                options, _ = tool.parse_args(['commit', opt, 'https://bugs.gentoo.org/2'])
-                assert options.footer == {('Bug', 'https://bugs.gentoo.org/2')}
+            for opt in ("-b", "--bug"):
+                options, _ = tool.parse_args(["commit", opt, "https://bugs.gentoo.org/2"])
+                assert options.footer == {("Bug", "https://bugs.gentoo.org/2")}
 
             # bug IDs
-            for opt in ('-c', '--closes'):
-                options, _ = tool.parse_args(['commit', opt, '1'])
-                assert options.footer == {('Closes', 'https://bugs.gentoo.org/1')}
+            for opt in ("-c", "--closes"):
+                options, _ = tool.parse_args(["commit", opt, "1"])
+                assert options.footer == {("Closes", "https://bugs.gentoo.org/1")}
 
             # bug URLs
-            for opt in ('-c', '--closes'):
-                options, _ = tool.parse_args(['commit', opt, 'https://bugs.gentoo.org/2'])
-                assert options.footer == {('Closes', 'https://bugs.gentoo.org/2')}
+            for opt in ("-c", "--closes"):
+                options, _ = tool.parse_args(["commit", opt, "https://bugs.gentoo.org/2"])
+                assert options.footer == {("Closes", "https://bugs.gentoo.org/2")}
 
             # bad URL
-            for opt in ('-b', '-c'):
+            for opt in ("-b", "-c"):
                 with pytest.raises(SystemExit) as excinfo:
-                    tool.parse_args(['commit', opt, 'bugs.gentoo.org/1'])
+                    tool.parse_args(["commit", opt, "bugs.gentoo.org/1"])
                 assert excinfo.value.code == 2
                 out, err = capsys.readouterr()
                 assert not out
-                assert 'invalid URL: bugs.gentoo.org/1' in err
+                assert "invalid URL: bugs.gentoo.org/1" in err
 
             # generic tags
-            for opt in ('-T', '--tag'):
+            for opt in ("-T", "--tag"):
                 for value, expected in (
-                        ('tag:value', ('Tag', 'value')),
-                        ('tag:multiple values', ('Tag', 'multiple values')),
-                        ('tag:multiple:values', ('Tag', 'multiple:values')),
-                        ):
-                    options, _ = tool.parse_args(['commit', opt, value])
+                    ("tag:value", ("Tag", "value")),
+                    ("tag:multiple values", ("Tag", "multiple values")),
+                    ("tag:multiple:values", ("Tag", "multiple:values")),
+                ):
+                    options, _ = tool.parse_args(["commit", opt, value])
                     assert options.footer == {expected}
 
             # bad tags
-            for opt in ('-T', '--tag'):
-                for value in ('', ':', 'tag:', ':value', 'tag'):
+            for opt in ("-T", "--tag"):
+                for value in ("", ":", "tag:", ":value", "tag"):
                     with pytest.raises(SystemExit) as excinfo:
-                        tool.parse_args(['commit', opt, value])
+                        tool.parse_args(["commit", opt, value])
                     assert excinfo.value.code == 2
                     out, err = capsys.readouterr()
                     assert not out
-                    assert 'invalid commit tag' in err
+                    assert "invalid commit tag" in err
 
 
 class TestPkgdevCommit:
-
-    script = staticmethod(partial(run, 'pkgdev'))
+    script = staticmethod(partial(run, "pkgdev"))
 
     @pytest.fixture(autouse=True)
     def _setup(self, tmp_path):
         self.cache_dir = str(tmp_path)
-        self.scan_args = ['--pkgcheck-scan', f'--config no --cache-dir {self.cache_dir}']
+        self.scan_args = ["--pkgcheck-scan", f"--config no --cache-dir {self.cache_dir}"]
         # args for running pkgdev like a script
-        self.args = ['pkgdev', 'commit', '--config', 'no'] + self.scan_args
+        self.args = ["pkgdev", "commit", "--config", "no"] + self.scan_args
 
     def test_empty_repo(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location, commit=True)
-        with patch('sys.argv', self.args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        with patch("sys.argv", self.args), pytest.raises(SystemExit) as excinfo, chdir(
+            git_repo.path
+        ):
             self.script()
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
         assert not out
-        assert err.strip() == 'pkgdev commit: error: no staged changes exist'
+        assert err.strip() == "pkgdev commit: error: no staged changes exist"
 
     def test_git_message_opts(self, repo, make_git_repo, tmp_path):
         """Verify message-related options are passed through to `git commit`."""
         git_repo = make_git_repo(repo.location, commit=True)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0', commit=False)
-        path = str(tmp_path / 'msg')
-        with open(path, 'w') as f:
-            f.write('commit1')
-
-        with patch('sys.argv', self.args + ['-u', '-F', path]), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0", commit=False)
+        path = str(tmp_path / "msg")
+        with open(path, "w") as f:
+            f.write("commit1")
+
+        with patch("sys.argv", self.args + ["-u", "-F", path]), pytest.raises(
+            SystemExit
+        ) as excinfo, chdir(git_repo.path):
             self.script()
         assert excinfo.value.code == 0
-        commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-        assert commit_msg == ['commit1']
+        commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+        assert commit_msg == ["commit1"]
 
-        repo.create_ebuild('cat/pkg-1')
-        git_repo.add_all('cat/pkg-1', commit=False)
-        with os_environ(GIT_EDITOR="sed -i '1s/1/2/'"), \
-                patch('sys.argv', self.args + ['-u', '-t', path]), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        repo.create_ebuild("cat/pkg-1")
+        git_repo.add_all("cat/pkg-1", commit=False)
+        with os_environ(GIT_EDITOR="sed -i '1s/1/2/'"), patch(
+            "sys.argv", self.args + ["-u", "-t", path]
+        ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
             self.script()
         assert excinfo.value.code == 0
-        commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-        assert commit_msg == ['commit2']
+        commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+        assert commit_msg == ["commit2"]
 
     def test_message_template(self, capsys, repo, make_git_repo, tmp_path):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        path = str(tmp_path / 'msg')
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        path = str(tmp_path / "msg")
 
         # auto-generate prefix
-        with open(path, 'w') as f:
-            f.write(textwrap.dedent("""\
-                *: summary
-
-                body
-            """))
-
-        for i, opt in enumerate(['-M', '--message-template'], 1):
-            repo.create_ebuild(f'cat/pkg-{i}')
-            git_repo.add_all(f'cat/pkg-{i}', commit=False)
-            with patch('sys.argv', self.args + ['-u', opt, path]), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+        with open(path, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        *: summary
+
+                        body
+                    """
+                )
+            )
+
+        for i, opt in enumerate(["-M", "--message-template"], 1):
+            repo.create_ebuild(f"cat/pkg-{i}")
+            git_repo.add_all(f"cat/pkg-{i}", commit=False)
+            with patch("sys.argv", self.args + ["-u", opt, path]), pytest.raises(
+                SystemExit
+            ) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
-            commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-            assert commit_msg == ['cat/pkg: summary', '', 'body']
+            commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+            assert commit_msg == ["cat/pkg: summary", "", "body"]
 
         # override prefix
-        with open(path, 'w') as f:
-            f.write(textwrap.dedent("""\
-                prefix: summary
-
-                body
-            """))
-
-        for i, opt in enumerate(['-M', '--message-template'], 3):
-            repo.create_ebuild(f'cat/pkg-{i}')
-            git_repo.add_all(f'cat/pkg-{i}', commit=False)
-            with patch('sys.argv', self.args + ['-u', opt, path]), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+        with open(path, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        prefix: summary
+
+                        body
+                    """
+                )
+            )
+
+        for i, opt in enumerate(["-M", "--message-template"], 3):
+            repo.create_ebuild(f"cat/pkg-{i}")
+            git_repo.add_all(f"cat/pkg-{i}", commit=False)
+            with patch("sys.argv", self.args + ["-u", opt, path]), pytest.raises(
+                SystemExit
+            ) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
-            commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-            assert commit_msg == ['prefix: summary', '', 'body']
+            commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+            assert commit_msg == ["prefix: summary", "", "body"]
 
         # empty message
-        with open(path, 'w') as f:
-            f.write('')
+        with open(path, "w") as f:
+            f.write("")
 
-        for i, opt in enumerate(['-M', '--message-template'], 5):
-            repo.create_ebuild(f'cat/pkg-{i}')
-            git_repo.add_all(f'cat/pkg-{i}', commit=False)
-            with patch('sys.argv', self.args + ['-u', opt, path]), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+        for i, opt in enumerate(["-M", "--message-template"], 5):
+            repo.create_ebuild(f"cat/pkg-{i}")
+            git_repo.add_all(f"cat/pkg-{i}", commit=False)
+            with patch("sys.argv", self.args + ["-u", opt, path]), pytest.raises(
+                SystemExit
+            ) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 2
             out, err = capsys.readouterr()
             assert not out
-            assert err.strip().startswith('pkgdev commit: error: empty message template')
+            assert err.strip().startswith("pkgdev commit: error: empty message template")
 
     def test_custom_unprefixed_message(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        ebuild_path = repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        with open(ebuild_path, 'a+') as f:
-            f.write('# comment\n')
-
-        with patch('sys.argv', self.args + ['-u', '-m', 'msg']), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        ebuild_path = repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        with open(ebuild_path, "a+") as f:
+            f.write("# comment\n")
+
+        with patch("sys.argv", self.args + ["-u", "-m", "msg"]), pytest.raises(
+            SystemExit
+        ) as excinfo, chdir(git_repo.path):
             self.script()
         assert excinfo.value.code == 0
         out, err = capsys.readouterr()
-        assert err == out == ''
+        assert err == out == ""
 
-        commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-        assert commit_msg == ['cat/pkg: msg']
+        commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+        assert commit_msg == ["cat/pkg: msg"]
 
     def test_custom_prefixed_message(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        ebuild_path = repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        with open(ebuild_path, 'a+') as f:
-            f.write('# comment\n')
-
-        with patch('sys.argv', self.args + ['-u', '-m', 'prefix: msg']), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        ebuild_path = repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        with open(ebuild_path, "a+") as f:
+            f.write("# comment\n")
+
+        with patch("sys.argv", self.args + ["-u", "-m", "prefix: msg"]), pytest.raises(
+            SystemExit
+        ) as excinfo, chdir(git_repo.path):
             self.script()
         assert excinfo.value.code == 0
         out, err = capsys.readouterr()
-        assert err == out == ''
+        assert err == out == ""
 
-        commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-        assert commit_msg == ['prefix: msg']
+        commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+        assert commit_msg == ["prefix: msg"]
 
     def test_edited_commit_message(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        ebuild_path = repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        with open(ebuild_path, 'a+') as f:
-            f.write('# comment\n')
-
-        with os_environ(GIT_EDITOR="sed -i '1s/$/commit/'"), \
-                patch('sys.argv', self.args + ['-u']), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        ebuild_path = repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        with open(ebuild_path, "a+") as f:
+            f.write("# comment\n")
+
+        with os_environ(GIT_EDITOR="sed -i '1s/$/commit/'"), patch(
+            "sys.argv", self.args + ["-u"]
+        ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
             self.script()
         assert excinfo.value.code == 0
         out, err = capsys.readouterr()
-        assert err == out == ''
+        assert err == out == ""
 
-        commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-        assert commit_msg == ['cat/pkg: commit']
+        commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+        assert commit_msg == ["cat/pkg: commit"]
 
     def test_generated_commit_prefixes(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
         def commit():
-            with patch('sys.argv', self.args + ['-a', '-m', 'msg']), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with patch("sys.argv", self.args + ["-a", "-m", "msg"]), pytest.raises(
+                SystemExit
+            ) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
-            assert err == out == ''
-            message = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
+            assert err == out == ""
+            message = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
             return message[0]
 
         # single package change
-        repo.create_ebuild('cat/newpkg-0')
-        assert commit().startswith('cat/newpkg: ')
+        repo.create_ebuild("cat/newpkg-0")
+        assert commit().startswith("cat/newpkg: ")
 
         # multiple package changes in the same category
-        repo.create_ebuild('cat/newpkg-1')
-        repo.create_ebuild('cat/pkg-1')
-        assert commit().startswith('cat/*: ')
+        repo.create_ebuild("cat/newpkg-1")
+        repo.create_ebuild("cat/pkg-1")
+        assert commit().startswith("cat/*: ")
 
         # multiple package changes in various categories
-        repo.create_ebuild('cat/newpkg-2')
-        repo.create_ebuild('cat/pkg-2')
-        repo.create_ebuild('newcat/newpkg-1')
-        assert commit().startswith('*/*: ')
+        repo.create_ebuild("cat/newpkg-2")
+        repo.create_ebuild("cat/pkg-2")
+        repo.create_ebuild("newcat/newpkg-1")
+        assert commit().startswith("*/*: ")
 
         # single eclass change
-        with open(pjoin(repo.location, 'eclass', 'foo.eclass'), 'a+') as f:
-            f.write('# comment\n')
-        assert commit().startswith('foo.eclass: ')
+        with open(pjoin(repo.location, "eclass", "foo.eclass"), "a+") as f:
+            f.write("# comment\n")
+        assert commit().startswith("foo.eclass: ")
 
         # multiple eclass changes
-        for eclass in ('foo.eclass', 'bar.eclass'):
-            with open(pjoin(repo.location, 'eclass', eclass), 'a+') as f:
-                f.write('# comment\n')
-        assert commit().startswith('eclass: ')
+        for eclass in ("foo.eclass", "bar.eclass"):
+            with open(pjoin(repo.location, "eclass", eclass), "a+") as f:
+                f.write("# comment\n")
+        assert commit().startswith("eclass: ")
 
         # single profiles/package.mask change
-        with open(pjoin(repo.location, 'profiles', 'package.mask'), 'a+') as f:
-            f.write('# comment\n')
-        assert commit().startswith('profiles: ')
+        with open(pjoin(repo.location, "profiles", "package.mask"), "a+") as f:
+            f.write("# comment\n")
+        assert commit().startswith("profiles: ")
 
-        amd64 = pjoin(repo.location, 'profiles', 'arch', 'amd64')
+        amd64 = pjoin(repo.location, "profiles", "arch", "amd64")
         os.makedirs(amd64)
-        arm64 = pjoin(repo.location, 'profiles', 'arch', 'arm64')
+        arm64 = pjoin(repo.location, "profiles", "arch", "arm64")
         os.makedirs(arm64)
 
         # multiple profiles file changes in the same subdir
-        for file in ('package.mask', 'package.mask'):
-            with open(pjoin(amd64, file), 'a+') as f:
-                f.write('# comment\n')
-        assert commit().startswith('profiles/arch/amd64: ')
+        for file in ("package.mask", "package.mask"):
+            with open(pjoin(amd64, file), "a+") as f:
+                f.write("# comment\n")
+        assert commit().startswith("profiles/arch/amd64: ")
 
         # multiple profiles file changes in different subdirs
         for path in (amd64, arm64):
-            with open(pjoin(path, 'package.use'), 'a+') as f:
-                f.write('# comment\n')
-        assert commit().startswith('profiles/arch: ')
+            with open(pjoin(path, "package.use"), "a+") as f:
+                f.write("# comment\n")
+        assert commit().startswith("profiles/arch: ")
 
         # single repo root file change
-        with open(pjoin(repo.location, 'skel.ebuild'), 'a+') as f:
-            f.write('# comment\n')
-        assert commit().startswith('skel.ebuild: ')
+        with open(pjoin(repo.location, "skel.ebuild"), "a+") as f:
+            f.write("# comment\n")
+        assert commit().startswith("skel.ebuild: ")
 
         # multiple repo root file change (no commit message prefix)
-        for file in ('skel.ebuild', 'header.txt'):
-            with open(pjoin(repo.location, file), 'a+') as f:
-                f.write('# comment\n')
-        assert commit() == 'msg'
+        for file in ("skel.ebuild", "header.txt"):
+            with open(pjoin(repo.location, file), "a+") as f:
+                f.write("# comment\n")
+        assert commit() == "msg"
 
         # treewide changes (no commit message prefix)
-        repo.create_ebuild('foo/bar-1')
-        with open(pjoin(repo.location, 'eclass', 'foo.eclass'), 'a+') as f:
-            f.write('# comment\n')
-        with open(pjoin(repo.location, 'profiles', 'package.mask'), 'a+') as f:
-            f.write('# comment\n')
-        assert commit() == 'msg'
+        repo.create_ebuild("foo/bar-1")
+        with open(pjoin(repo.location, "eclass", "foo.eclass"), "a+") as f:
+            f.write("# comment\n")
+        with open(pjoin(repo.location, "profiles", "package.mask"), "a+") as f:
+            f.write("# comment\n")
+        assert commit() == "msg"
 
     def test_generated_commit_summaries(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
         def commit():
-            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), \
-                    patch('sys.argv', self.args + ['-a']), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), patch(
+                "sys.argv", self.args + ["-a"]
+            ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
-            assert err == out == ''
-            message = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
+            assert err == out == ""
+            message = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
             return message[0]
 
         # initial package import
-        repo.create_ebuild('cat/newpkg-0')
-        assert commit() == 'cat/newpkg: new package, add 0'
+        repo.create_ebuild("cat/newpkg-0")
+        assert commit() == "cat/newpkg: new package, add 0"
 
         # initial package import, overflowed title truncated
         for i in range(10):
-            repo.create_ebuild(f'cat/newpkg2-{i}.0.0')
-        assert commit() == 'cat/newpkg2: new package'
+            repo.create_ebuild(f"cat/newpkg2-{i}.0.0")
+        assert commit() == "cat/newpkg2: new package"
 
         # single addition
-        repo.create_ebuild('cat/pkg-1')
-        assert commit() == 'cat/pkg: add 1'
+        repo.create_ebuild("cat/pkg-1")
+        assert commit() == "cat/pkg: add 1"
 
         # multiple additions
-        repo.create_ebuild('cat/pkg-2')
-        repo.create_ebuild('cat/pkg-3')
-        repo.create_ebuild('cat/pkg-4', eapi=6)
-        assert commit() == 'cat/pkg: add 2, 3, 4'
+        repo.create_ebuild("cat/pkg-2")
+        repo.create_ebuild("cat/pkg-3", eapi=6)
+        repo.create_ebuild("cat/pkg-4", eapi=6)
+        assert commit() == "cat/pkg: add 2, 3, 4"
 
         # revbump updating EAPI
-        repo.create_ebuild('cat/pkg-4-r1', eapi=7)
-        assert commit() == 'cat/pkg: update EAPI 6 -> 7'
+        repo.create_ebuild("cat/pkg-4-r1", eapi=7)
+        assert commit() == "cat/pkg: update EAPI 6 -> 7"
 
         # single rename with no revisions
         git_repo.move(
-            pjoin(git_repo.path, 'cat/pkg/pkg-4.ebuild'),
-            pjoin(git_repo.path, 'cat/pkg/pkg-5.ebuild'),
-            commit=False
+            pjoin(git_repo.path, "cat/pkg/pkg-4.ebuild"),
+            pjoin(git_repo.path, "cat/pkg/pkg-5.ebuild"),
+            commit=False,
         )
-        assert commit() == 'cat/pkg: add 5, drop 4'
+        assert commit() == "cat/pkg: add 5, drop 4"
 
-        # bump EAPI
-        repo.create_ebuild('cat/pkg-6', eapi='6')
-        git_repo.add_all('cat/pkg-6')
-        repo.create_ebuild('cat/pkg-6', eapi='7')
-        assert commit() == 'cat/pkg: update EAPI 6 -> 7'
+        # bump EAPI for multiple versions, same summary
+        repo.create_ebuild("cat/pkg-6", eapi="6")
+        git_repo.add_all("cat/pkg-6")
+        repo.create_ebuild("cat/pkg-3", eapi="7")
+        repo.create_ebuild("cat/pkg-6", eapi="7")
+        assert commit() == "cat/pkg: update EAPI 6 -> 7"
 
         # update description
-        repo.create_ebuild('cat/pkg-7')
-        git_repo.add_all('cat/pkg-7')
-        repo.create_ebuild('cat/pkg-7', description='something')
-        assert commit() == 'cat/pkg: update DESCRIPTION'
+        repo.create_ebuild("cat/pkg-7")
+        git_repo.add_all("cat/pkg-7")
+        repo.create_ebuild("cat/pkg-7", description="something")
+        assert commit() == "cat/pkg: update DESCRIPTION"
 
         # update description & homepage
-        repo.create_ebuild('cat/pkg-7', description='another something', homepage='https://gentoo.org')
-        assert commit() == 'cat/pkg: update DESCRIPTION, HOMEPAGE'
+        repo.create_ebuild(
+            "cat/pkg-7", description="another something", homepage="https://gentoo.org"
+        )
+        assert commit() == "cat/pkg: update DESCRIPTION, HOMEPAGE"
 
         # update string_targets (USE_RUBY)
-        os.mkdir(pjoin(repo.location, 'profiles', 'desc'))
-        with open(pjoin(repo.path, 'profiles', 'desc', 'ruby_targets.desc'), 'w') as file:
-            file.write('\n'.join(f'ruby{ver} - stub' for ver in range(27, 40)))
-        repo.create_ebuild('cat/pkg-8', use_ruby='ruby27')
-        git_repo.add_all('cat/pkg-8')
-        repo.create_ebuild('cat/pkg-8', use_ruby='ruby27 ruby30')
-        assert commit() == 'cat/pkg: enable ruby30'
-        repo.create_ebuild('cat/pkg-8', use_ruby='ruby30')
-        assert commit() == 'cat/pkg: disable ruby27'
-        repo.create_ebuild('cat/pkg-8', use_ruby=' '.join(f'ruby{i}' for i in range(30, 40)))
-        assert commit() == 'cat/pkg: update USE_RUBY support'
+        os.mkdir(pjoin(repo.location, "profiles", "desc"))
+        with open(pjoin(repo.path, "profiles", "desc", "ruby_targets.desc"), "w") as file:
+            file.write("\n".join(f"ruby{ver} - stub" for ver in range(27, 40)))
+        repo.create_ebuild("cat/pkg-8", use_ruby="ruby27")
+        git_repo.add_all("cat/pkg-8")
+        repo.create_ebuild("cat/pkg-8", use_ruby="ruby27 ruby30")
+        assert commit() == "cat/pkg: enable ruby30"
+        repo.create_ebuild("cat/pkg-8", use_ruby="ruby30")
+        assert commit() == "cat/pkg: disable ruby27"
+        repo.create_ebuild("cat/pkg-8", use_ruby=" ".join(f"ruby{i}" for i in range(30, 40)))
+        assert commit() == "cat/pkg: update USE_RUBY support"
 
         # update array_targets (PYTHON_COMPAT)
-        with open(pjoin(repo.path, 'profiles', 'desc', 'python_targets.desc'), 'w') as file:
-            file.write('\n'.join(f'python3_{ver} - stub' for ver in (10, 11)))
-        repo.create_ebuild('cat/pkg-9', data='PYTHON_COMPAT=( python3_8 python3_9 )')
-        git_repo.add_all('cat/pkg-9')
-        repo.create_ebuild('cat/pkg-9', data='PYTHON_COMPAT=( python3_{8..10} )')
-        assert commit() == 'cat/pkg: enable py3.10'
-        repo.create_ebuild('cat/pkg-9', data='PYTHON_COMPAT=( python3_{9..10} )')
-        assert commit() == 'cat/pkg: disable py3.8'
-        repo.create_ebuild('cat/pkg-9', data='PYTHON_COMPAT=( python3_{10..11} )')
-        assert commit() == 'cat/pkg: enable py3.11'
-
+        with open(pjoin(repo.path, "profiles", "desc", "python_targets.desc"), "w") as file:
+            file.write("\n".join(f"python3_{ver} - stub" for ver in (10, 11)))
+        repo.create_ebuild("cat/pkg-9", data="PYTHON_COMPAT=( python3_8 python3_9 )")
+        git_repo.add_all("cat/pkg-9")
+        repo.create_ebuild("cat/pkg-9", data="PYTHON_COMPAT=( python3_{8..10} )")
+        assert commit() == "cat/pkg: enable py3.10"
+        repo.create_ebuild("cat/pkg-9", data="PYTHON_COMPAT=( python3_{9..10} )")
+        assert commit() == "cat/pkg: disable py3.8"
+        repo.create_ebuild("cat/pkg-9", data="PYTHON_COMPAT=( python3_{10..11} )")
+        assert commit() == "cat/pkg: enable py3.11"
 
         # multiple ebuild modifications don't get a generated summary
-        repo.create_ebuild('cat/pkg-5', keywords=['~amd64'])
-        repo.create_ebuild('cat/pkg-6', keywords=['~amd64'])
-        assert commit() == 'cat/pkg: summary'
+        repo.create_ebuild("cat/pkg-5", keywords=["~amd64"])
+        repo.create_ebuild("cat/pkg-6", keywords=["~amd64"])
+        assert commit() == "cat/pkg: summary"
 
         # large number of additions in a single commit
         for v in range(10000, 10010):
-            repo.create_ebuild(f'cat/pkg-{v}')
-        assert commit() == 'cat/pkg: add versions'
+            repo.create_ebuild(f"cat/pkg-{v}")
+        assert commit() == "cat/pkg: add versions"
 
         # create Manifest
-        with open(pjoin(git_repo.path, 'cat/pkg/Manifest'), 'w') as file:
-            file.write('DIST pkg-3.tar.gz 101 BLAKE2B deadbeef SHA512 deadbeef\n')
-        assert commit() == 'cat/pkg: update Manifest'
+        with open(pjoin(git_repo.path, "cat/pkg/Manifest"), "w") as file:
+            file.write("DIST pkg-3.tar.gz 101 BLAKE2B deadbeef SHA512 deadbeef\n")
+        assert commit() == "cat/pkg: update Manifest"
         # update Manifest
-        with open(pjoin(git_repo.path, 'cat/pkg/Manifest'), 'a+') as file:
-            file.write('DIST pkg-2.tar.gz 101 BLAKE2B deadbeef SHA512 deadbeef\n')
-        assert commit() == 'cat/pkg: update Manifest'
+        with open(pjoin(git_repo.path, "cat/pkg/Manifest"), "a+") as file:
+            file.write("DIST pkg-2.tar.gz 101 BLAKE2B deadbeef SHA512 deadbeef\n")
+        assert commit() == "cat/pkg: update Manifest"
         # remove Manifest
-        os.remove(pjoin(git_repo.path, 'cat/pkg/Manifest'))
-        assert commit() == 'cat/pkg: update Manifest'
+        os.remove(pjoin(git_repo.path, "cat/pkg/Manifest"))
+        assert commit() == "cat/pkg: update Manifest"
 
         # single removals
-        os.remove(pjoin(git_repo.path, 'cat/pkg/pkg-4-r1.ebuild'))
-        assert commit() == 'cat/pkg: drop 4-r1'
-        os.remove(pjoin(git_repo.path, 'cat/pkg/pkg-3.ebuild'))
-        assert commit() == 'cat/pkg: drop 3'
+        os.remove(pjoin(git_repo.path, "cat/pkg/pkg-4-r1.ebuild"))
+        assert commit() == "cat/pkg: drop 4-r1"
+        os.remove(pjoin(git_repo.path, "cat/pkg/pkg-3.ebuild"))
+        assert commit() == "cat/pkg: drop 3"
 
         # multiple removal
-        os.remove(pjoin(git_repo.path, 'cat/pkg/pkg-2.ebuild'))
-        os.remove(pjoin(git_repo.path, 'cat/pkg/pkg-1.ebuild'))
-        assert commit() == 'cat/pkg: drop 1, 2'
+        os.remove(pjoin(git_repo.path, "cat/pkg/pkg-2.ebuild"))
+        os.remove(pjoin(git_repo.path, "cat/pkg/pkg-1.ebuild"))
+        assert commit() == "cat/pkg: drop 1, 2"
 
         # large number of removals in a single commit
         for v in range(10000, 10010):
-            os.remove(pjoin(git_repo.path, f'cat/pkg/pkg-{v}.ebuild'))
-        assert commit() == 'cat/pkg: drop versions'
+            os.remove(pjoin(git_repo.path, f"cat/pkg/pkg-{v}.ebuild"))
+        assert commit() == "cat/pkg: drop versions"
 
         # package rename
-        shutil.copytree(pjoin(git_repo.path, 'cat/pkg'), pjoin(git_repo.path, 'newcat/pkg'))
-        shutil.rmtree(pjoin(git_repo.path, 'cat/pkg'))
-        assert commit() == 'newcat/pkg: rename cat/pkg'
+        shutil.copytree(pjoin(git_repo.path, "cat/pkg"), pjoin(git_repo.path, "newcat/pkg"))
+        shutil.rmtree(pjoin(git_repo.path, "cat/pkg"))
+        assert commit() == "newcat/pkg: rename cat/pkg"
 
         # treeclean
-        shutil.rmtree(pjoin(git_repo.path, 'newcat/pkg'))
-        assert commit() == 'newcat/pkg: treeclean'
+        shutil.rmtree(pjoin(git_repo.path, "newcat/pkg"))
+        assert commit() == "newcat/pkg: treeclean"
 
     def test_generated_commit_summaries_keywords(self, capsys, make_repo, make_git_repo):
-        repo = make_repo(arches=['amd64', 'arm64', 'ia64', 'x86'])
+        repo = make_repo(arches=["amd64", "arm64", "ia64", "x86"])
         git_repo = make_git_repo(repo.location)
-        pkgdir = os.path.dirname(repo.create_ebuild('cat/pkg-0'))
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <stabilize-allarches/>
-                </pkgmetadata>
-            """))
-        git_repo.add_all('cat/pkg-0')
+        pkgdir = os.path.dirname(repo.create_ebuild("cat/pkg-0"))
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <stabilize-allarches/>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        git_repo.add_all("cat/pkg-0")
 
         def commit():
-            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), \
-                    patch('sys.argv', self.args + ['-a']), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), patch(
+                "sys.argv", self.args + ["-a"]
+            ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
-            assert err == out == ''
-            message = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
+            assert err == out == ""
+            message = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
             return message[0]
 
         # keyword version
-        repo.create_ebuild('cat/pkg-0', keywords=['~amd64'])
-        assert commit() == 'cat/pkg: keyword 0 for ~amd64'
+        repo.create_ebuild("cat/pkg-0", keywords=["~amd64"])
+        assert commit() == "cat/pkg: keyword 0 for ~amd64"
 
         # stabilize version
-        repo.create_ebuild('cat/pkg-0', keywords=['amd64'])
-        assert commit() == 'cat/pkg: stabilize 0 for amd64'
+        repo.create_ebuild("cat/pkg-0", keywords=["amd64"])
+        assert commit() == "cat/pkg: stabilize 0 for amd64"
 
         # destabilize version
-        repo.create_ebuild('cat/pkg-0', keywords=['~amd64'])
-        assert commit() == 'cat/pkg: destabilize 0 for ~amd64'
+        repo.create_ebuild("cat/pkg-0", keywords=["~amd64"])
+        assert commit() == "cat/pkg: destabilize 0 for ~amd64"
 
         # unkeyword version
-        repo.create_ebuild('cat/pkg-0')
-        assert commit() == 'cat/pkg: unkeyword 0 for ~amd64'
+        repo.create_ebuild("cat/pkg-0")
+        assert commit() == "cat/pkg: unkeyword 0 for ~amd64"
 
-        with open(pjoin(repo.location, 'profiles', 'arches.desc'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                amd64 stable
-                arm64 stable
-                ia64  testing
-                x86   stable
-            """))
-        git_repo.add_all('set arches.desc')
+        with open(pjoin(repo.location, "profiles", "arches.desc"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        amd64 stable
+                        arm64 stable
+                        ia64  testing
+                        x86   stable
+                    """
+                )
+            )
+        git_repo.add_all("set arches.desc")
 
-        repo.create_ebuild('cat/pkg-0', keywords=['~amd64', '~arm64', '~ia64', '~x86'])
-        git_repo.add_all('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0", keywords=["~amd64", "~arm64", "~ia64", "~x86"])
+        git_repo.add_all("cat/pkg-0")
 
         # stabilize version
-        repo.create_ebuild('cat/pkg-0', keywords=['amd64', '~arm64', '~ia64', '~x86'])
-        assert commit() == 'cat/pkg: stabilize 0 for amd64'
+        repo.create_ebuild("cat/pkg-0", keywords=["amd64", "~arm64", "~ia64", "~x86"])
+        assert commit() == "cat/pkg: stabilize 0 for amd64"
 
         # stabilize version ALLARCHES
-        repo.create_ebuild('cat/pkg-0', keywords=['amd64', 'arm64', '~ia64', 'x86'])
-        assert commit() == 'cat/pkg: stabilize 0 for ALLARCHES'
+        repo.create_ebuild("cat/pkg-0", keywords=["amd64", "arm64", "~ia64", "x86"])
+        assert commit() == "cat/pkg: stabilize 0 for ALLARCHES"
 
         # stabilize version
-        repo.create_ebuild('cat/newpkg-0', keywords=['~amd64', '~arm64', '~ia64', '~x86'])
-        git_repo.add_all('cat/newpkg')
-        repo.create_ebuild('cat/newpkg-0', keywords=['amd64', 'arm64', '~ia64', 'x86'])
-        assert commit() == 'cat/newpkg: stabilize 0 for amd64, arm64, x86'
+        repo.create_ebuild("cat/newpkg-0", keywords=["~amd64", "~arm64", "~ia64", "~x86"])
+        git_repo.add_all("cat/newpkg")
+        repo.create_ebuild("cat/newpkg-0", keywords=["amd64", "arm64", "~ia64", "x86"])
+        assert commit() == "cat/newpkg: stabilize 0 for amd64, arm64, x86"
 
     def test_metadata_summaries(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        pkgdir = os.path.dirname(repo.create_ebuild('cat/pkg-0'))
+        pkgdir = os.path.dirname(repo.create_ebuild("cat/pkg-0"))
         # stub metadata
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                </pkgmetadata>
-            """))
-        git_repo.add_all('cat/pkg-0')
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        git_repo.add_all("cat/pkg-0")
 
         def commit():
-            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), \
-                    patch('sys.argv', self.args + ['-a']), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), patch(
+                "sys.argv", self.args + ["-a"]
+            ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
-            assert err == out == ''
-            message = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
+            assert err == out == ""
+            message = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
             return message[0]
 
         # add yourself
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                    <maintainer type="person">
-                        <email>first.last@email.com</email>
-                        <name>First Last</name>
-                    </maintainer>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: add myself as a maintainer'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                            <maintainer type="person">
+                                <email>first.last@email.com</email>
+                                <name>First Last</name>
+                            </maintainer>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: add myself as a maintainer"
 
         # drop yourself
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: drop myself as a maintainer'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: drop myself as a maintainer"
 
         # drop to maintainer-needed
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: drop to maintainer-needed'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: drop to maintainer-needed"
 
         # add random maintainer
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: update maintainers'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: update maintainers"
 
         # add allarches tag
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                    <stabilize-allarches/>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: mark ALLARCHES'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                            <stabilize-allarches/>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: mark ALLARCHES"
 
         # drop allarches tag
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: drop ALLARCHES'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: drop ALLARCHES"
 
         # add upstream metadata
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                    <upstream>
-                        <remote-id type="github">pkgcore/pkgdev</remote-id>
-                        <remote-id type="pypi">pkgdev</remote-id>
-                    </upstream>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: add github, pypi upstream metadata'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                            <upstream>
+                                <remote-id type="github">pkgcore/pkgdev</remote-id>
+                                <remote-id type="pypi">pkgdev</remote-id>
+                            </upstream>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: add github, pypi upstream metadata"
 
         # remove upstream metadata
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                    <upstream>
-                        <remote-id type="github">pkgcore/pkgdev</remote-id>
-                    </upstream>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: remove pypi upstream metadata'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                            <upstream>
+                                <remote-id type="github">pkgcore/pkgdev</remote-id>
+                            </upstream>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: remove pypi upstream metadata"
 
         # update upstream metadata
-        with open(pjoin(pkgdir, 'metadata.xml'), 'w') as f:
-            f.write(textwrap.dedent("""\
-                <?xml version="1.0" encoding="UTF-8"?>
-                <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
-                <pkgmetadata>
-                    <maintainer type="person">
-                        <email>person@email.com</email>
-                        <name>Person</name>
-                    </maintainer>
-                    <upstream>
-                        <remote-id type="github">pkgcore/pkgcheck</remote-id>
-                    </upstream>
-                </pkgmetadata>
-            """))
-        assert commit() == 'cat/pkg: update upstream metadata'
+        with open(pjoin(pkgdir, "metadata.xml"), "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """\
+                        <?xml version="1.0" encoding="UTF-8"?>
+                        <!DOCTYPE pkgmetadata SYSTEM "http://www.gentoo.org/dtd/metadata.dtd">
+                        <pkgmetadata>
+                            <maintainer type="person">
+                                <email>person@email.com</email>
+                                <name>Person</name>
+                            </maintainer>
+                            <upstream>
+                                <remote-id type="github">pkgcore/pkgcheck</remote-id>
+                            </upstream>
+                        </pkgmetadata>
+                    """
+                )
+            )
+        assert commit() == "cat/pkg: update upstream metadata"
 
     def test_no_summary(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
         def commit(args):
-            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), \
-                    patch('sys.argv', self.args + args), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with os_environ(GIT_EDITOR="sed -i '1s/$/summary/'"), patch(
+                "sys.argv", self.args + args
+            ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
-            assert err == out == ''
-            return git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
+            assert err == out == ""
+            return git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
 
         # no commit message content
         for i in range(10):
-            with open(pjoin(git_repo.path, f'file-a-{i}'), 'w') as f:
-                f.write('stub\n')
-        assert commit(['-a']) == ['summary']
+            with open(pjoin(git_repo.path, f"file-a-{i}"), "w") as f:
+                f.write("stub\n")
+        assert commit(["-a"]) == ["summary"]
 
         # footer exists with no generated summary
         for i in range(10):
-            with open(pjoin(git_repo.path, f'file-b-{i}'), 'w') as f:
-                f.write('stub\n')
-        assert commit(['-a', '-T', 'tag:value']) == ['summary', '', 'Tag: value']
+            with open(pjoin(git_repo.path, f"file-b-{i}"), "w") as f:
+                f.write("stub\n")
+        assert commit(["-a", "-T", "tag:value"]) == ["summary", "", "Tag: value"]
 
     def test_non_gentoo_file_mangling(self, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        ebuild_path = repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        ebuild_path = repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
         def commit(args):
-            with patch('sys.argv', self.args + args), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with patch("sys.argv", self.args + args), pytest.raises(SystemExit) as excinfo, chdir(
+                git_repo.path
+            ):
                 self.script()
             assert excinfo.value.code == 0
 
         # append line missing EOF newline to ebuild
-        with open(ebuild_path, 'a+') as f:
-            f.write('# comment')
+        with open(ebuild_path, "a+") as f:
+            f.write("# comment")
         # verify file doesn't end with newline
         with open(ebuild_path) as f:
-            assert f.read()[-1] != '\n'
+            assert f.read()[-1] != "\n"
 
         # non-gentoo repos aren't mangled by default
-        commit(['-u', '-m', 'mangling'])
+        commit(["-u", "-m", "mangling"])
         with open(ebuild_path) as f:
-            assert f.read()[-1] != '\n'
+            assert f.read()[-1] != "\n"
 
         # but they can be forcibly mangled
-        with open(ebuild_path, 'a+') as f:
-            f.write('# comment')
-        commit(['--mangle', '-u', '-m', 'mangling'])
+        with open(ebuild_path, "a+") as f:
+            f.write("# comment")
+        commit(["--mangle", "-u", "-m", "mangling"])
         # mangled pre-commit, file now ends with newline
         with open(ebuild_path) as f:
-            assert f.read()[-1] == '\n'
+            assert f.read()[-1] == "\n"
 
         # FILESDIR content is ignored even when forced
-        path = pjoin(os.path.dirname(ebuild_path), 'files', 'pkg.patch')
+        path = pjoin(os.path.dirname(ebuild_path), "files", "pkg.patch")
         os.makedirs(os.path.dirname(path))
-        with open(path, 'w') as f:
-            f.write('# comment')
+        with open(path, "w") as f:
+            f.write("# comment")
         # verify file doesn't end with newline
         with open(path) as f:
-            assert f.read()[-1] != '\n'
+            assert f.read()[-1] != "\n"
 
     def test_gentoo_file_mangling(self, make_repo, make_git_repo):
-        repo = make_repo(repo_id='gentoo')
+        repo = make_repo(repo_id="gentoo")
         git_repo = make_git_repo(repo.location)
-        ebuild_path = repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        ebuild_path = repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
         def commit(args):
-            with patch('sys.argv', self.args + args), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+            with patch("sys.argv", self.args + args), pytest.raises(SystemExit) as excinfo, chdir(
+                git_repo.path
+            ):
                 self.script()
             assert excinfo.value.code == 0
 
         # append line missing EOF newline to ebuild
-        with open(ebuild_path, 'a+') as f:
-            f.write('# comment')
+        with open(ebuild_path, "a+") as f:
+            f.write("# comment")
         # verify file doesn't end with newline
         with open(ebuild_path) as f:
-            assert f.read()[-1] != '\n'
+            assert f.read()[-1] != "\n"
 
         # gentoo repos are mangled by default
-        commit(['-n', '-u', '-m', 'mangling'])
+        commit(["-n", "-u", "-m", "mangling"])
         with open(ebuild_path) as f:
-            assert f.read()[-1] == '\n'
+            assert f.read()[-1] == "\n"
 
         # FILESDIR content is ignored
-        path = pjoin(os.path.dirname(ebuild_path), 'files', 'pkg.patch')
+        path = pjoin(os.path.dirname(ebuild_path), "files", "pkg.patch")
         os.makedirs(os.path.dirname(path))
-        with open(path, 'w') as f:
-            f.write('# comment')
+        with open(path, "w") as f:
+            f.write("# comment")
         # verify file doesn't end with newline
         with open(path) as f:
-            assert f.read()[-1] != '\n'
+            assert f.read()[-1] != "\n"
 
         for years, org in (
-                ('1999-2020', 'Gentoo Authors'),
-                ('1999-2020', 'Gentoo Foundation'),
-                ('2020', 'Gentoo Authors'),
-                ('2020', 'Gentoo Foundation'),
-                ):
+            ("1999-2020", "Gentoo Authors"),
+            ("1999-2020", "Gentoo Foundation"),
+            ("2020", "Gentoo Authors"),
+            ("2020", "Gentoo Foundation"),
+        ):
             # munge the copyright header
-            with open(ebuild_path, 'r+') as f:
+            with open(ebuild_path, "r+") as f:
                 lines = f.read().splitlines()
-                lines[0] = f'# Copyright {years} {org}\n'
+                lines[0] = f"# Copyright {years} {org}\n"
                 f.seek(0)
                 f.truncate()
-                f.write('\n'.join(lines) + '\n')
-            commit(['-n', '-u', '-m', 'mangling'])
+                f.write("\n".join(lines) + "\n")
+            commit(["-n", "-u", "-m", "mangling"])
             # verify the copyright header was updated
             with open(ebuild_path) as f:
                 lines = f.read().splitlines()
                 mo = copyright_regex.match(lines[0])
-                assert mo.group('end') == str(datetime.today().year)
-                assert mo.group('begin') == years[:4] + '-'
-                assert mo.group('holder') == 'Gentoo Authors'
+                assert mo.group("end") == str(datetime.today().year)
+                assert mo.group("begin") == years[:4] + "-"
+                assert mo.group("holder") == "Gentoo Authors"
 
         for original, expected in (
-                ('"arm64 amd64 x86"', 'amd64 arm64 x86'),
-                ('"arm64 amd64 ~x86"', 'amd64 arm64 ~x86'),
-                ('"arm64 ~x86 amd64"', 'amd64 arm64 ~x86'),
-                ('"arm64 ~x86 ~amd64"', '~amd64 arm64 ~x86'),
-                ('arm64 ~x86 ~amd64', '~amd64 arm64 ~x86'),
-                ):
+            ('"arm64 amd64 x86"', "amd64 arm64 x86"),
+            ('"arm64 amd64 ~x86"', "amd64 arm64 ~x86"),
+            ('"arm64 ~x86 amd64"', "amd64 arm64 ~x86"),
+            ('"arm64 ~x86 ~amd64"', "~amd64 arm64 ~x86"),
+            ("arm64 ~x86 ~amd64", "~amd64 arm64 ~x86"),
+        ):
             # munge the keywords
-            with open(ebuild_path, 'r+') as f:
+            with open(ebuild_path, "r+") as f:
                 lines = f.read().splitlines()
-                lines[-1] = f'KEYWORDS={original}'
+                lines[-1] = f"KEYWORDS={original}"
                 f.seek(0)
                 f.truncate()
-                f.write('\n'.join(lines) + '\n')
-            commit(['-n', '-u', '-m', 'mangling'])
+                f.write("\n".join(lines) + "\n")
+            commit(["-n", "-u", "-m", "mangling"])
             # verify the keywords were updated
             with open(ebuild_path) as f:
                 lines = f.read().splitlines()
                 mo = keywords_regex.match(lines[-1])
-                assert mo.group('keywords') == expected
+                assert mo.group("keywords") == expected
 
     def test_scan(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
-        for i, opt in enumerate(['-s', '--scan'], 1):
-            repo.create_ebuild(f'cat/pkg-{i}')
-            git_repo.add_all(f'cat/pkg-{i}', commit=False)
-            with patch('sys.argv', self.args + [opt]), \
-                    pytest.raises(SystemExit) as excinfo, \
-                    chdir(git_repo.path):
+        for i, opt in enumerate(["-s", "--scan"], 1):
+            repo.create_ebuild(f"cat/pkg-{i}")
+            git_repo.add_all(f"cat/pkg-{i}", commit=False)
+            with patch("sys.argv", self.args + [opt]), pytest.raises(SystemExit) as excinfo, chdir(
+                git_repo.path
+            ):
                 self.script()
             assert excinfo.value.code == 0
             out, err = capsys.readouterr()
-            assert err == out == ''
-            commit_msg = git_repo.log(['-1', '--pretty=tformat:%B', 'HEAD'])
-            assert commit_msg == [f'cat/pkg: add {i}']
+            assert err == out == ""
+            commit_msg = git_repo.log(["-1", "--pretty=tformat:%B", "HEAD"])
+            assert commit_msg == [f"cat/pkg: add {i}"]
 
     def test_failed_scan(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
 
         # verify staged changes via `pkgcheck scan` before creating commit
-        repo.create_ebuild('cat/pkg-1', license='')
-        git_repo.add_all('cat/pkg-1', commit=False)
-        with patch('sys.argv', self.args + ['--scan']), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        repo.create_ebuild("cat/pkg-1", license="")
+        git_repo.add_all("cat/pkg-1", commit=False)
+        with patch("sys.argv", self.args + ["--scan"]), pytest.raises(SystemExit) as excinfo, chdir(
+            git_repo.path
+        ):
             self.script()
         assert excinfo.value.code == 1
         out, err = capsys.readouterr()
         assert not err
-        assert out == textwrap.dedent("""\
-            cat/pkg
-              MissingLicense: version 1: no license defined
-
-            FAILURES
-            cat/pkg
-              MissingLicense: version 1: no license defined
-        """)
+        assert out == textwrap.dedent(
+            """\
+                cat/pkg
+                  MissingLicense: version 1: no license defined
+
+                FAILURES
+                cat/pkg
+                  MissingLicense: version 1: no license defined
+        """
+        )
 
         # ignore failures to create the commit
-        with patch('sys.argv', self.args + ['--scan', '--ask']), \
-                patch('sys.stdin', StringIO('y\n')), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        with patch("sys.argv", self.args + ["--scan", "--ask"]), patch(
+            "sys.stdin", StringIO("y\n")
+        ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
             self.script()
         assert excinfo.value.code == 0
 
     def test_config_opts(self, capsys, repo, make_git_repo, tmp_path):
-        config_file = str(tmp_path / 'config')
-        with open(config_file, 'w') as f:
-            f.write(textwrap.dedent("""
-                [DEFAULT]
-                commit.scan=
-            """))
-
-        git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        repo.create_ebuild('cat/pkg-1', license='')
-        git_repo.add_all('cat/pkg-1', commit=False)
-        with patch('sys.argv', ['pkgdev', 'commit', '--config', config_file] + self.scan_args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        config_file = str(tmp_path / "config")
+        with open(config_file, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """
+                        [DEFAULT]
+                        commit.scan=
+                    """
+                )
+            )
+
+        git_repo = make_git_repo(repo.location)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        repo.create_ebuild("cat/pkg-1", license="")
+        git_repo.add_all("cat/pkg-1", commit=False)
+        with patch(
+            "sys.argv", ["pkgdev", "commit", "--config", config_file] + self.scan_args
+        ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
             self.script()
         out, err = capsys.readouterr()
         assert excinfo.value.code == 1
         assert not err
-        assert 'MissingLicense' in out
+        assert "MissingLicense" in out
 
     def test_config_repo_opts(self, capsys, repo, make_git_repo, tmp_path):
-        config_file = str(tmp_path / 'config')
-        with open(config_file, 'w') as f:
-            f.write(textwrap.dedent("""
-                [fake]
-                commit.scan=
-            """))
-
-        git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        repo.create_ebuild('cat/pkg-1', license='')
-        git_repo.add_all('cat/pkg-1', commit=False)
-        with patch('sys.argv', ['pkgdev', 'commit', '--config', config_file] + self.scan_args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        config_file = str(tmp_path / "config")
+        with open(config_file, "w") as f:
+            f.write(
+                textwrap.dedent(
+                    """
+                        [fake]
+                        commit.scan=
+                    """
+                )
+            )
+
+        git_repo = make_git_repo(repo.location)
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        repo.create_ebuild("cat/pkg-1", license="")
+        git_repo.add_all("cat/pkg-1", commit=False)
+        with patch(
+            "sys.argv", ["pkgdev", "commit", "--config", config_file] + self.scan_args
+        ), pytest.raises(SystemExit) as excinfo, chdir(git_repo.path):
             self.script()
         out, err = capsys.readouterr()
         assert excinfo.value.code == 1
         assert not err
-        assert 'MissingLicense' in out
+        assert "MissingLicense" in out
 
     def test_failed_manifest(self, capsys, repo, make_git_repo):
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/pkg-0')
-        git_repo.add_all('cat/pkg-0')
-        repo.create_ebuild('cat/pkg-1', eapi='-1')
-        git_repo.add_all('cat/pkg-1', commit=False)
-        with patch('sys.argv', self.args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(git_repo.path):
+        repo.create_ebuild("cat/pkg-0")
+        git_repo.add_all("cat/pkg-0")
+        repo.create_ebuild("cat/pkg-1", eapi="-1")
+        git_repo.add_all("cat/pkg-1", commit=False)
+        with patch("sys.argv", self.args), pytest.raises(SystemExit) as excinfo, chdir(
+            git_repo.path
+        ):
             self.script()
         assert excinfo.value.code == 1
         out, err = capsys.readouterr()
         assert not err
         assert out == " * cat/pkg-1: invalid EAPI '-1'\n"
```

### Comparing `pkgdev-0.2.4/tests/scripts/test_pkgdev_manifest.py` & `pkgdev-0.2.5/tests/scripts/test_pkgdev_manifest.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,192 +5,191 @@
 import pytest
 from pkgdev.scripts import run
 from snakeoil.contexts import chdir
 from snakeoil.osutils import pjoin
 
 
 class TestPkgdevManifestParseArgs:
-
     def test_non_repo_cwd(self, capsys, tool):
         with pytest.raises(SystemExit) as excinfo:
-            tool.parse_args(['manifest'])
+            tool.parse_args(["manifest"])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
-        assert err.strip() == 'pkgdev manifest: error: not in ebuild repo'
+        assert err.strip() == "pkgdev manifest: error: not in ebuild repo"
 
     def test_repo_cwd(self, repo, capsys, tool):
-        repo.create_ebuild('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
         with chdir(repo.location):
-            options, _ = tool.parse_args(['manifest'])
+            options, _ = tool.parse_args(["manifest"])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert matches == ['cat/pkg-0']
+        assert matches == ["cat/pkg-0"]
 
     def test_repo_relative_pkg(self, repo, capsys, tool):
-        repo.create_ebuild('cat/pkg-0')
-        repo.create_ebuild('cat/newpkg-0')
-        with chdir(pjoin(repo.location, 'cat/pkg')):
-            options, _ = tool.parse_args(['manifest', '.'])
+        repo.create_ebuild("cat/pkg-0")
+        repo.create_ebuild("cat/newpkg-0")
+        with chdir(pjoin(repo.location, "cat/pkg")):
+            options, _ = tool.parse_args(["manifest", "."])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert matches == ['cat/pkg-0']
+        assert matches == ["cat/pkg-0"]
 
     def test_repo_relative_category(self, repo, capsys, tool):
-        repo.create_ebuild('cat/pkg-0')
-        repo.create_ebuild('cat/newpkg-0')
+        repo.create_ebuild("cat/pkg-0")
+        repo.create_ebuild("cat/newpkg-0")
 
-        with chdir(pjoin(repo.location, 'cat')):
-            options, _ = tool.parse_args(['manifest', 'pkg'])
+        with chdir(pjoin(repo.location, "cat")):
+            options, _ = tool.parse_args(["manifest", "pkg"])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert matches == ['cat/pkg-0']
+        assert matches == ["cat/pkg-0"]
 
-        with chdir(pjoin(repo.location, 'cat')):
-            options, _ = tool.parse_args(['manifest', '.'])
+        with chdir(pjoin(repo.location, "cat")):
+            options, _ = tool.parse_args(["manifest", "."])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert set(matches) == {'cat/pkg-0', 'cat/newpkg-0'}
+        assert set(matches) == {"cat/pkg-0", "cat/newpkg-0"}
 
     def test_repo_relative_outside(self, tmp_path, repo, capsys, tool):
-        repo.create_ebuild('cat/pkg-0')
-        (ebuild := tmp_path / 'pkg.ebuild').touch()
+        repo.create_ebuild("cat/pkg-0")
+        (ebuild := tmp_path / "pkg.ebuild").touch()
         with pytest.raises(SystemExit) as excinfo:
             with chdir(repo.location):
-                tool.parse_args(['manifest', str(ebuild)])
+                tool.parse_args(["manifest", str(ebuild)])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
-        assert err.strip() == f"pkgdev manifest: error: {repo.repo_id!r} repo doesn't contain: {str(ebuild)!r}"
+        assert (
+            err.strip()
+            == f"pkgdev manifest: error: {repo.repo_id!r} repo doesn't contain: {str(ebuild)!r}"
+        )
 
     def test_dir_target(self, repo, capsys, tool):
-        repo.create_ebuild('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
         with chdir(repo.location):
-            options, _ = tool.parse_args(['manifest', pjoin(repo.location, 'cat')])
+            options, _ = tool.parse_args(["manifest", pjoin(repo.location, "cat")])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert matches == ['cat/pkg-0']
+        assert matches == ["cat/pkg-0"]
 
     def test_ebuild_target(self, repo, capsys, tool):
-        path = repo.create_ebuild('cat/pkg-0')
+        path = repo.create_ebuild("cat/pkg-0")
         with chdir(repo.location):
-            options, _ = tool.parse_args(['manifest', path])
+            options, _ = tool.parse_args(["manifest", path])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert matches == ['cat/pkg-0']
+        assert matches == ["cat/pkg-0"]
 
     def test_atom_target(self, repo, capsys, tool):
-        repo.create_ebuild('cat/pkg-0')
+        repo.create_ebuild("cat/pkg-0")
         with chdir(repo.location):
-            options, _ = tool.parse_args(['manifest', 'cat/pkg'])
+            options, _ = tool.parse_args(["manifest", "cat/pkg"])
         matches = [x.cpvstr for x in repo.itermatch(options.restriction)]
-        assert matches == ['cat/pkg-0']
+        assert matches == ["cat/pkg-0"]
 
     def test_if_modified_target(self, repo, make_git_repo, tool):
         def manifest_matches() -> Set[str]:
             repo.sync()
             with chdir(repo.location):
-                options, _ = tool.parse_args(['manifest', '--if-modified'])
+                options, _ = tool.parse_args(["manifest", "--if-modified"])
             return {x.cpvstr for x in repo.itermatch(options.restriction)}
 
         git_repo = make_git_repo(repo.location)
-        repo.create_ebuild('cat/oldpkg-0')
-        git_repo.add_all('cat/oldpkg-0')
+        repo.create_ebuild("cat/oldpkg-0")
+        git_repo.add_all("cat/oldpkg-0")
 
         # New package
-        repo.create_ebuild('cat/newpkg-0')
-        assert manifest_matches() == {'cat/newpkg-0'}
-        git_repo.add_all('cat/newpkg-0')
+        repo.create_ebuild("cat/newpkg-0")
+        assert manifest_matches() == {"cat/newpkg-0"}
+        git_repo.add_all("cat/newpkg-0")
 
         # Untracked file
-        ebuild_path = repo.create_ebuild('cat/newpkg-1')
-        assert manifest_matches() == {'cat/newpkg-1'}
+        ebuild_path = repo.create_ebuild("cat/newpkg-1")
+        assert manifest_matches() == {"cat/newpkg-1"}
 
         # Staged file
         git_repo.add(ebuild_path, commit=False)
-        assert manifest_matches() == {'cat/newpkg-1'}
+        assert manifest_matches() == {"cat/newpkg-1"}
 
         # No modified files
-        git_repo.add_all('cat/newpkg-1')
+        git_repo.add_all("cat/newpkg-1")
         assert manifest_matches() == set()
 
         # Modified file
-        ebuild_path = repo.create_ebuild('cat/newpkg-1', eapi=8)
-        assert manifest_matches() == {'cat/newpkg-1'}
-        git_repo.add_all('cat/newpkg-1: eapi 8')
+        ebuild_path = repo.create_ebuild("cat/newpkg-1", eapi=8)
+        assert manifest_matches() == {"cat/newpkg-1"}
+        git_repo.add_all("cat/newpkg-1: eapi 8")
 
         # Renamed file
         git_repo.remove(ebuild_path, commit=False)
-        ebuild_path = repo.create_ebuild('cat/newpkg-2')
+        ebuild_path = repo.create_ebuild("cat/newpkg-2")
         git_repo.add(ebuild_path, commit=False)
-        assert manifest_matches() == {'cat/newpkg-2'}
-        git_repo.add_all('cat/newpkg-2: rename')
+        assert manifest_matches() == {"cat/newpkg-2"}
+        git_repo.add_all("cat/newpkg-2: rename")
 
         # Deleted file
         git_repo.remove(ebuild_path, commit=False)
         assert manifest_matches() == set()
 
         # Deleted package
-        ebuild_path = repo.create_ebuild('cat/newpkg-0')
+        ebuild_path = repo.create_ebuild("cat/newpkg-0")
         git_repo.remove(ebuild_path, commit=False)
         assert manifest_matches() == set()
 
     def test_ignore_fetch_restricted(self, repo, tool):
         def manifest_matches() -> List[str]:
             with chdir(repo.location):
-                options, _ = tool.parse_args(['manifest', '--ignore-fetch-restricted'])
+                options, _ = tool.parse_args(["manifest", "--ignore-fetch-restricted"])
             return [x.cpvstr for x in repo.itermatch(options.restriction)]
 
         # No RESTRICT
-        repo.create_ebuild('cat/pkg-0')
-        assert manifest_matches() == ['cat/pkg-0']
+        repo.create_ebuild("cat/pkg-0")
+        assert manifest_matches() == ["cat/pkg-0"]
 
         # Not fetch RESTRICT
-        repo.create_ebuild('cat/pkg-0', restrict=('mirror'))
-        assert manifest_matches() == ['cat/pkg-0']
+        repo.create_ebuild("cat/pkg-0", restrict=("mirror"))
+        assert manifest_matches() == ["cat/pkg-0"]
 
         # fetch RESTRICT
-        repo.create_ebuild('cat/pkg-0', restrict=('fetch'))
+        repo.create_ebuild("cat/pkg-0", restrict=("fetch"))
         assert manifest_matches() == []
 
         # Multiple RESTRICT
-        repo.create_ebuild('cat/pkg-0', restrict=('mirror', 'fetch'))
+        repo.create_ebuild("cat/pkg-0", restrict=("mirror", "fetch"))
         assert manifest_matches() == []
 
     def test_non_repo_dir_target(self, tmp_path, repo, capsys, tool):
-        with pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
-            tool.parse_args(['manifest', str(tmp_path)])
+        with pytest.raises(SystemExit) as excinfo, chdir(repo.location):
+            tool.parse_args(["manifest", str(tmp_path)])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
         assert err.startswith("pkgdev manifest: error: 'fake' repo doesn't contain:")
 
     def test_invalid_atom_target(self, repo, capsys, tool):
-        with pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
-            tool.parse_args(['manifest', '=cat/pkg'])
+        with pytest.raises(SystemExit) as excinfo, chdir(repo.location):
+            tool.parse_args(["manifest", "=cat/pkg"])
         assert excinfo.value.code == 2
         out, err = capsys.readouterr()
         assert err.startswith("pkgdev manifest: error: invalid atom: '=cat/pkg'")
 
 
 class TestPkgdevManifest:
-
-    script = staticmethod(partial(run, 'pkgdev'))
+    script = staticmethod(partial(run, "pkgdev"))
 
     @pytest.fixture(autouse=True)
     def _setup(self):
-        self.args = ['pkgdev', 'manifest']
+        self.args = ["pkgdev", "manifest"]
 
     def test_good_manifest(self, capsys, repo):
-        repo.create_ebuild('cat/pkg-0')
-        with patch('sys.argv', self.args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
+        repo.create_ebuild("cat/pkg-0")
+        with patch("sys.argv", self.args), pytest.raises(SystemExit) as excinfo, chdir(
+            repo.location
+        ):
             self.script()
         assert excinfo.value.code == 0
         out, err = capsys.readouterr()
-        assert out == err == ''
+        assert out == err == ""
 
     def test_bad_manifest(self, capsys, repo):
-        repo.create_ebuild('cat/pkg-0')
-        repo.create_ebuild('cat/pkg-1', eapi='-1')
-        with patch('sys.argv', self.args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
+        repo.create_ebuild("cat/pkg-0")
+        repo.create_ebuild("cat/pkg-1", eapi="-1")
+        with patch("sys.argv", self.args), pytest.raises(SystemExit) as excinfo, chdir(
+            repo.location
+        ):
             self.script()
         assert excinfo.value.code == 1
         out, err = capsys.readouterr()
         assert not err
         assert out == " * cat/pkg-1: invalid EAPI '-1'\n"
```

### Comparing `pkgdev-0.2.4/tests/scripts/test_pkgdev_showkw.py` & `pkgdev-0.2.5/tests/scripts/test_pkgdev_showkw.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,195 +7,217 @@
 from snakeoil.contexts import chdir, os_environ
 
 from pkgdev.scripts import run
 
 
 class Profile(NamedTuple):
     """Profile record used to create profiles in a repository."""
+
     path: str
     arch: str
-    status: str = 'stable'
+    status: str = "stable"
     deprecated: bool = False
     defaults: List[str] = None
-    eapi: str = '5'
+    eapi: str = "5"
+
 
 class TestPkgdevShowkwParseArgs:
-    args = ('showkw', '--config', 'no')
+    args = ("showkw", "--config", "no")
 
     def test_missing_target(self, capsys, tool):
         with pytest.raises(SystemExit):
             tool.parse_args(self.args)
         captured = capsys.readouterr()
         assert captured.err.strip() == (
-            'pkgdev showkw: error: missing target argument and not in a supported repo')
+            "pkgdev showkw: error: missing target argument and not in a supported repo"
+        )
 
     def test_unknown_arches(self, capsys, tool, make_repo):
-        repo = make_repo(arches=['amd64'])
+        repo = make_repo(arches=["amd64"])
         with pytest.raises(SystemExit):
-            tool.parse_args([*self.args, '-a', 'unknown', '-r', repo.location])
+            tool.parse_args([*self.args, "-a", "unknown", "-r", repo.location])
         captured = capsys.readouterr()
         assert captured.err.strip() == (
-            "pkgdev showkw: error: unknown arch: 'unknown' (choices: amd64)")
+            "pkgdev showkw: error: unknown arch: 'unknown' (choices: amd64)"
+        )
 
     def test_no_color(self, tool, make_repo, tmp_path):
-        repo = make_repo(arches=['amd64'])
-        repo.create_ebuild('foo/bar-0', keywords=('x86'))
+        repo = make_repo(arches=["amd64"])
+        repo.create_ebuild("foo/bar-0", keywords=("x86"))
 
-        (config_file := tmp_path / 'pkgcheck.conf').write_text(textwrap.dedent('''\
+        (config_file := tmp_path / "pkgcheck.conf").write_text(
+            textwrap.dedent(
+                """\
             [DEFAULT]
             showkw.color = true
-        '''))
+        """
+            )
+        )
 
         def parse(*args):
-            options, _ = tool.parse_args(['showkw', '-r', repo.location, 'foo/bar',
-                                          '--config', str(config_file), *args])
+            options, _ = tool.parse_args(
+                ["showkw", "-r", repo.location, "foo/bar", "--config", str(config_file), *args]
+            )
             return options
 
-        with os_environ('NOCOLOR'):
+        with os_environ("NOCOLOR"):
             assert parse().color is True
-        with os_environ(NOCOLOR='1'):
+        with os_environ(NOCOLOR="1"):
             # NOCOLOR overrides config file
             assert parse().color is False
             # cmd line option overrides NOCOLOR
-            assert parse('--color', 'n').color is False
-            assert parse('--color', 'y').color is True
+            assert parse("--color", "n").color is False
+            assert parse("--color", "y").color is True
 
-class TestPkgdevShowkw:
 
-    script = staticmethod(partial(run, 'pkgdev'))
-    base_args = ('pkgdev', 'showkw', '--config', 'n', '--color', 'n')
+class TestPkgdevShowkw:
+    script = staticmethod(partial(run, "pkgdev"))
+    base_args = ("pkgdev", "showkw", "--config", "n", "--color", "n")
 
     def _create_repo(self, make_repo):
-        repo = make_repo(arches=['amd64', 'ia64', 'mips', 'x86'])
-        repo.create_profiles([
-            Profile('default/linux/amd64', 'amd64'),
-            Profile('default/linux/x86', 'x86'),
-            Profile('default/linux/ia64', 'ia64', 'dev'),
-            Profile('default/linux/mips', 'mips', 'exp'),
-        ])
+        repo = make_repo(arches=["amd64", "ia64", "mips", "x86"])
+        repo.create_profiles(
+            [
+                Profile("default/linux/amd64", "amd64"),
+                Profile("default/linux/x86", "x86"),
+                Profile("default/linux/ia64", "ia64", "dev"),
+                Profile("default/linux/mips", "mips", "exp"),
+            ]
+        )
         return repo
 
     def _run_and_parse(self, capsys, *args):
-        with patch('sys.argv', [*self.base_args, "--format", "presto", *args]), \
-                pytest.raises(SystemExit) as excinfo:
+        with patch("sys.argv", [*self.base_args, "--format", "presto", *args]), pytest.raises(
+            SystemExit
+        ) as excinfo:
             self.script()
         assert excinfo.value.code is None
         out, err = capsys.readouterr()
         assert not err
-        lines = out.split('\n')
-        table_columns = [s.strip() for s in lines[1].split('|')][1:]
+        lines = out.split("\n")
+        table_columns = [s.strip() for s in lines[1].split("|")][1:]
         return {
             ver: dict(zip(table_columns, values))
-                for ver, *values in map(lambda s: map(str.strip, s.split('|')), lines[3:-1])
+            for ver, *values in map(lambda s: map(str.strip, s.split("|")), lines[3:-1])
         }
 
     def test_match(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0')
-        with patch('sys.argv', [*self.base_args, '-r', repo.location, 'foo/bar']), \
-                pytest.raises(SystemExit) as excinfo:
+        repo.create_ebuild("foo/bar-0")
+        with patch("sys.argv", [*self.base_args, "-r", repo.location, "foo/bar"]), pytest.raises(
+            SystemExit
+        ) as excinfo:
             self.script()
         assert excinfo.value.code is None
         out, err = capsys.readouterr()
         assert not err
-        assert out.split('\n')[0] == "keywords for foo/bar:"
+        assert out.split("\n")[0] == "keywords for foo/bar:"
 
     def test_match_short_name(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0')
-        with patch('sys.argv', [*self.base_args, '-r', repo.location, 'bar']), \
-                pytest.raises(SystemExit) as excinfo:
+        repo.create_ebuild("foo/bar-0")
+        with patch("sys.argv", [*self.base_args, "-r", repo.location, "bar"]), pytest.raises(
+            SystemExit
+        ) as excinfo:
             self.script()
         assert excinfo.value.code is None
         out, err = capsys.readouterr()
         assert not err
-        assert out.split('\n')[0] == "keywords for foo/bar:"
+        assert out.split("\n")[0] == "keywords for foo/bar:"
 
     def test_match_cwd_repo(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0')
-        with patch('sys.argv', [*self.base_args, 'foo/bar']), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location):
+        repo.create_ebuild("foo/bar-0")
+        with patch("sys.argv", [*self.base_args, "foo/bar"]), pytest.raises(
+            SystemExit
+        ) as excinfo, chdir(repo.location):
             self.script()
         assert excinfo.value.code is None
         out, err = capsys.readouterr()
         assert not err
-        assert out.split('\n')[0] == "keywords for foo/bar:"
+        assert out.split("\n")[0] == "keywords for foo/bar:"
 
     def test_match_cwd_pkg(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0')
-        with patch('sys.argv', self.base_args), \
-                pytest.raises(SystemExit) as excinfo, \
-                chdir(repo.location + '/foo/bar'):
+        repo.create_ebuild("foo/bar-0")
+        with patch("sys.argv", self.base_args), pytest.raises(SystemExit) as excinfo, chdir(
+            repo.location + "/foo/bar"
+        ):
             self.script()
         assert excinfo.value.code is None
         _, err = capsys.readouterr()
         assert not err
 
     def test_no_matches(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        with patch('sys.argv', [*self.base_args, '-r', repo.location, 'foo/bar']), \
-                pytest.raises(SystemExit) as excinfo:
+        with patch("sys.argv", [*self.base_args, "-r", repo.location, "foo/bar"]), pytest.raises(
+            SystemExit
+        ) as excinfo:
             self.script()
         assert excinfo.value.code == 1
         out, err = capsys.readouterr()
         assert not out
         assert err.strip() == "pkgdev showkw: no matches for 'foo/bar'"
 
     def test_match_stable(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0', keywords=('~amd64', '~ia64', '~mips', 'x86'))
-        res = self._run_and_parse(capsys, '-r', repo.location, 'foo/bar', '--stable')
-        assert set(res.keys()) == {'0'}
-        assert {'amd64', 'ia64', 'mips', 'x86'} & res['0'].keys() == {'amd64', 'x86'}
+        repo.create_ebuild("foo/bar-0", keywords=("~amd64", "~ia64", "~mips", "x86"))
+        res = self._run_and_parse(capsys, "-r", repo.location, "foo/bar", "--stable")
+        assert set(res.keys()) == {"0"}
+        assert {"amd64", "ia64", "mips", "x86"} & res["0"].keys() == {"amd64", "x86"}
 
     def test_match_unstable(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0', keywords=('~amd64', '~ia64', '~mips', 'x86'))
-        res = self._run_and_parse(capsys, '-r', repo.location, 'foo/bar', '--unstable')
-        assert set(res.keys()) == {'0'}
-        assert {'amd64', 'ia64', 'mips', 'x86'} <= res['0'].keys()
+        repo.create_ebuild("foo/bar-0", keywords=("~amd64", "~ia64", "~mips", "x86"))
+        res = self._run_and_parse(capsys, "-r", repo.location, "foo/bar", "--unstable")
+        assert set(res.keys()) == {"0"}
+        assert {"amd64", "ia64", "mips", "x86"} <= res["0"].keys()
 
     def test_match_specific_arch(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0', keywords=('~amd64', '~ia64', '~mips', 'x86'))
-        res = self._run_and_parse(capsys, '-r', repo.location, 'foo/bar', '--arch', 'amd64')
-        assert set(res.keys()) == {'0'}
-        assert {'amd64', 'ia64', 'mips', 'x86'} & res['0'].keys() == {'amd64'}
+        repo.create_ebuild("foo/bar-0", keywords=("~amd64", "~ia64", "~mips", "x86"))
+        res = self._run_and_parse(capsys, "-r", repo.location, "foo/bar", "--arch", "amd64")
+        assert set(res.keys()) == {"0"}
+        assert {"amd64", "ia64", "mips", "x86"} & res["0"].keys() == {"amd64"}
 
     def test_match_specific_multiple_arch(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0', keywords=('~amd64', '~ia64', '~mips', 'x86'))
-        res = self._run_and_parse(capsys, '-r', repo.location, 'foo/bar', '--arch', 'amd64,mips')
-        assert set(res.keys()) == {'0'}
-        assert {'amd64', 'ia64', 'mips', 'x86'} & res['0'].keys() == {'amd64', 'mips'}
+        repo.create_ebuild("foo/bar-0", keywords=("~amd64", "~ia64", "~mips", "x86"))
+        res = self._run_and_parse(capsys, "-r", repo.location, "foo/bar", "--arch", "amd64,mips")
+        assert set(res.keys()) == {"0"}
+        assert {"amd64", "ia64", "mips", "x86"} & res["0"].keys() == {"amd64", "mips"}
 
     def test_correct_keywords_status(self, capsys, make_repo):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0', keywords=('amd64', '~ia64', '~mips', 'x86'))
-        repo.create_ebuild('foo/bar-1', keywords=('~amd64', '-mips', '~x86'))
-        repo.create_ebuild('foo/bar-2', keywords=('-*', 'amd64', '-x86'), eapi=8, slot=2)
-        res = self._run_and_parse(capsys, '-r', repo.location, 'foo/bar')
-        assert set(res.keys()) == {'0', '1', '2'}
-        assert dict(amd64='+', ia64='~', mips='~', x86='+', slot='0').items() <= res['0'].items()
-        assert dict(amd64='~', ia64='o', mips='-', x86='~', slot='0').items() <= res['1'].items()
-        assert dict(amd64='+', ia64='*', mips='*', x86='-', slot='2', eapi='8').items() <= res['2'].items()
-
-    @pytest.mark.parametrize(('arg', 'expected'), (
-        pytest.param('--stable', {'amd64', 'x86'}, id='stable'),
-        pytest.param('--unstable', {'amd64', 'ia64', 'mips', 'x86'}, id='unstable'),
-        pytest.param('--only-unstable', {'ia64', 'mips'}, id='only-unstable'),
-    ))
+        repo.create_ebuild("foo/bar-0", keywords=("amd64", "~ia64", "~mips", "x86"))
+        repo.create_ebuild("foo/bar-1", keywords=("~amd64", "-mips", "~x86"))
+        repo.create_ebuild("foo/bar-2", keywords=("-*", "amd64", "-x86"), eapi=8, slot=2)
+        res = self._run_and_parse(capsys, "-r", repo.location, "foo/bar")
+        assert set(res.keys()) == {"0", "1", "2"}
+        assert dict(amd64="+", ia64="~", mips="~", x86="+", slot="0").items() <= res["0"].items()
+        assert dict(amd64="~", ia64="o", mips="-", x86="~", slot="0").items() <= res["1"].items()
+        assert (
+            dict(amd64="+", ia64="*", mips="*", x86="-", slot="2", eapi="8").items()
+            <= res["2"].items()
+        )
+
+    @pytest.mark.parametrize(
+        ("arg", "expected"),
+        (
+            pytest.param("--stable", {"amd64", "x86"}, id="stable"),
+            pytest.param("--unstable", {"amd64", "ia64", "mips", "x86"}, id="unstable"),
+            pytest.param("--only-unstable", {"ia64", "mips"}, id="only-unstable"),
+        ),
+    )
     def test_collapse(self, capsys, make_repo, arg, expected):
         repo = self._create_repo(make_repo)
-        repo.create_ebuild('foo/bar-0', keywords=('amd64', '~ia64', '~mips', '~x86'))
-        repo.create_ebuild('foo/bar-1', keywords=('~amd64', '~ia64', '~mips', 'x86'))
-        with patch('sys.argv', [*self.base_args, '-r', repo.location, 'foo/bar', "--collapse", arg]), \
-                pytest.raises(SystemExit) as excinfo:
+        repo.create_ebuild("foo/bar-0", keywords=("amd64", "~ia64", "~mips", "~x86"))
+        repo.create_ebuild("foo/bar-1", keywords=("~amd64", "~ia64", "~mips", "x86"))
+        with patch(
+            "sys.argv", [*self.base_args, "-r", repo.location, "foo/bar", "--collapse", arg]
+        ), pytest.raises(SystemExit) as excinfo:
             self.script()
         out, err = capsys.readouterr()
         assert excinfo.value.code is None
         assert not err
-        arches = set(out.split('\n')[0].split())
+        arches = set(out.split("\n")[0].split())
         assert arches == expected
```

### Comparing `pkgdev-0.2.4/tests/test_git.py` & `pkgdev-0.2.5/tests/test_git.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 import pytest
 from snakeoil.cli.exceptions import UserException
 from snakeoil.contexts import chdir
 from pkgdev import git
 
 
 class TestGitRun:
-
     def test_git_missing(self):
-        with patch('subprocess.run') as git_run:
+        with patch("subprocess.run") as git_run:
             git_run.side_effect = FileNotFoundError("no such file 'git'")
             with pytest.raises(UserException, match="no such file 'git'"):
-                git.run('commit')
+                git.run("commit")
 
     def test_failed_run(self):
-        with patch('subprocess.run') as git_run:
-            git_run.side_effect = subprocess.CalledProcessError(1, 'git commit')
+        with patch("subprocess.run") as git_run:
+            git_run.side_effect = subprocess.CalledProcessError(1, "git commit")
             with pytest.raises(git.GitError):
-                git.run('commit')
+                git.run("commit")
 
     def test_successful_run(self, git_repo):
         with chdir(git_repo.path):
-            p = git.run('rev-parse', '--abbrev-ref', 'HEAD', stdout=subprocess.PIPE)
-        assert p.stdout.strip() == 'main'
+            p = git.run("rev-parse", "--abbrev-ref", "HEAD", stdout=subprocess.PIPE)
+        assert p.stdout.strip() == "main"
```

### Comparing `pkgdev-0.2.4/tests/test_mangle.py` & `pkgdev-0.2.5/tests/test_mangle.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,96 +8,95 @@
 from pkgdev.mangle import Mangler
 from pkgdev.scripts.pkgdev_commit import Change
 import pytest
 from snakeoil.cli.exceptions import UserException
 
 
 def fake_change(s):
-    return Change('/repo', 'A', str(s))
+    return Change("/repo", "A", str(s))
 
 
 class TestMangler:
-
     def test_nonexistent_file(self, tmp_path):
-        path = tmp_path / 'nonexistent'
+        path = tmp_path / "nonexistent"
         assert list(Mangler([fake_change(path)])) == []
 
     def test_empty_file(self, tmp_path):
-        path = tmp_path / 'empty'
+        path = tmp_path / "empty"
         path.touch()
         assert list(Mangler([fake_change(path)])) == []
 
     def test_skipped_file(self, tmp_path):
-        paths = [(tmp_path / x) for x in ('file', 'file.patch')]
+        paths = [(tmp_path / x) for x in ("file", "file.patch")]
 
         for p in paths:
-            p.write_text('# comment')
+            p.write_text("# comment")
         # skip patch files
-        skip_regex = re.compile(r'.+\.patch$')
+        skip_regex = re.compile(r".+\.patch$")
         mangled_paths = set(Mangler(map(fake_change, paths), skip_regex=skip_regex))
-        assert mangled_paths == {str(tmp_path / 'file')}
+        assert mangled_paths == {str(tmp_path / "file")}
 
         for p in paths:
-            p.write_text('# comment')
+            p.write_text("# comment")
         # don't skip any files
         mangled_paths = set(Mangler(map(fake_change, paths)))
         assert mangled_paths == set(map(str, paths))
 
     def test_nonmangled_file(self, tmp_path):
-        path = tmp_path / 'file'
-        path.write_text('# comment\n')
+        path = tmp_path / "file"
+        path.write_text("# comment\n")
         assert list(Mangler([fake_change(path)])) == []
 
     def test_mangled_file(self, tmp_path):
-        path = tmp_path / 'file'
-        path.write_text('# comment')
+        path = tmp_path / "file"
+        path.write_text("# comment")
         assert list(Mangler([fake_change(path)])) == [str(path)]
-        assert path.read_text() == '# comment\n'
+        assert path.read_text() == "# comment\n"
 
     def test_iterator_exceptions(self, tmp_path):
         """Test parallelized iterator against unhandled exceptions."""
-        path = tmp_path / 'file'
-        path.write_text('# comment\n')
+        path = tmp_path / "file"
+        path.write_text("# comment\n")
 
         def _mangle_func(self, data):
-            raise Exception('func failed')
+            raise Exception("func failed")
 
-        with patch('pkgdev.mangle.Mangler._mangle', _mangle_func):
-            with pytest.raises(UserException, match='Exception: func failed'):
+        with patch("pkgdev.mangle.Mangler._mangle", _mangle_func):
+            with pytest.raises(UserException, match="Exception: func failed"):
                 list(Mangler([fake_change(path)]))
 
     def test_sigint_handling(self, tmp_path):
         """Verify SIGINT is properly handled by the parallelized pipeline."""
-        path = tmp_path / 'file'
-        path.write_text('# comment\n')
+        path = tmp_path / "file"
+        path.write_text("# comment\n")
 
         def run(queue):
             """Mangler run in a separate process that gets interrupted."""
             import sys
             import time
             from unittest.mock import patch
 
             from pkgdev.mangle import Mangler
 
             def sleep():
                 """Notify testing process then sleep."""
-                queue.put('ready')
+                queue.put("ready")
                 time.sleep(100)
 
-            with patch('pkgdev.mangle.Mangler.__iter__') as fake_iter:
+            with patch("pkgdev.mangle.Mangler.__iter__") as fake_iter:
                 fake_iter.side_effect = partial(sleep)
                 try:
                     iter(Mangler([fake_change(path)]))
                 except KeyboardInterrupt:
                     queue.put(None)
                     sys.exit(0)
                 queue.put(None)
                 sys.exit(1)
 
-        mp_ctx = multiprocessing.get_context('fork')
+        mp_ctx = multiprocessing.get_context("fork")
         queue = mp_ctx.SimpleQueue()
         p = mp_ctx.Process(target=run, args=(queue,))
         p.start()
         # wait for pipeline object to be fully initialized then send SIGINT
         for _ in iter(queue.get, None):
             os.kill(p.pid, signal.SIGINT)
             p.join()
```

### Comparing `pkgdev-0.2.4/PKG-INFO` & `pkgdev-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: pkgdev
-Version: 0.2.4
+Version: 0.2.5
 Summary: collection of tools for Gentoo development
 Author-email: Tim Harder <radhermit@gmail.com>, Arthur Zamarin <arthurzam@gentoo.org>
 Maintainer-email: Arthur Zamarin <arthurzam@gentoo.org>
 Requires-Python: ~=3.9
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: snakeoil~=0.10.3
+Requires-Dist: snakeoil~=0.10.4
 Requires-Dist: pkgcore~=0.12.16
 Requires-Dist: pkgcheck~=0.10.16
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: tomli ; extra == "doc" and ( python_version < '3.11')
+Requires-Dist: nattka ; extra == "tatt"
+Requires-Dist: Jinja2 ; extra == "tatt"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Documentation, https://pkgcore.github.io/pkgdev/
 Project-URL: Homepage, https://github.com/pkgcore/pkgdev
 Project-URL: Source, https://github.com/pkgcore/pkgdev
 Provides-Extra: doc
+Provides-Extra: tatt
 Provides-Extra: test
 
 |pypi| |test| |coverage|
 
 ======
 pkgdev
 ======
```

