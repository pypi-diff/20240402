# Comparing `tmp/psyplot-1.4.3.tar.gz` & `tmp/psyplot-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyplot-1.4.3.tar", last modified: Fri Aug 26 20:44:58 2022, max compression
+gzip compressed data, was "psyplot-1.5.0.tar", last modified: Tue Apr  2 08:15:01 2024, max compression
```

## Comparing `psyplot-1.4.3.tar` & `psyplot-1.5.0.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.416386 psyplot-1.4.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-08-26 20:34:04.000000 psyplot-1.4.3/COPYING
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7652 2022-08-26 20:34:04.000000 psyplot-1.4.3/COPYING.LESSER
--rw-r--r--   0 circleci  (3434) circleci  (3434)      204 2022-08-26 20:34:04.000000 psyplot-1.4.3/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9633 2022-08-26 20:44:58.416386 psyplot-1.4.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8337 2022-08-26 20:34:04.000000 psyplot-1.4.3/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.416386 psyplot-1.4.3/psyplot/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5876 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17602 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2022-08-26 20:44:58.416386 psyplot-1.4.3/psyplot/_version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.412387 psyplot-1.4.3/psyplot/compat/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      963 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/compat/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3301 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/compat/pycompat.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.412387 psyplot-1.4.3/psyplot/config/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1582 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/config/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3504 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/config/logsetup.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    42268 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/config/rcsetup.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   193583 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/data.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     3305 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/docstring.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6193 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/gdal_store.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    90052 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plotter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.412387 psyplot-1.4.3/psyplot/plugin-template-files/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/COPYING
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7652 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/COPYING.LESSER
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      646 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.412387 psyplot-1.4.3/psyplot/plugin-template-files/plugin_template/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1013 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/plugin_template/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1825 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/plugin_template/plotters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3894 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/plugin_template/plugin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin-template-files/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2884 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/plugin_template.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)   103422 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/project.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.412387 psyplot-1.4.3/psyplot/sphinxext/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      976 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/sphinxext/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6571 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/sphinxext/extended_napoleon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11454 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/utils.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     4336 2022-08-26 20:34:04.000000 psyplot-1.4.3/psyplot/warning.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-26 20:44:58.412387 psyplot-1.4.3/psyplot.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9633 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2022-08-26 20:44:58.000000 psyplot-1.4.3/psyplot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      201 2022-08-26 20:44:58.416386 psyplot-1.4.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3754 2022-08-26 20:34:04.000000 psyplot-1.4.3/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    69726 2022-08-26 20:34:04.000000 psyplot-1.4.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.424055 psyplot-1.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.416055 psyplot-1.5.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-04-02 08:14:33.000000 psyplot-1.5.0/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-02 08:14:33.000000 psyplot-1.5.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    42098 2024-04-02 08:14:33.000000 psyplot-1.5.0/LICENSES/LGPL-3.0-only.txt
+-rw-rw-rw-   0 root         (0) root         (0)      308 2024-04-02 08:14:33.000000 psyplot-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10287 2024-04-02 08:15:01.424055 psyplot-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2024-04-02 08:14:33.000000 psyplot-1.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.420055 psyplot-1.5.0/psyplot/
+-rwxrwxrwx   0 root         (0) root         (0)     5173 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20740 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-02 08:15:01.424055 psyplot-1.5.0/psyplot/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.420055 psyplot-1.5.0/psyplot/config/
+-rwxrwxrwx   0 root         (0) root         (0)      892 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2790 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/config/logsetup.py
+-rwxrwxrwx   0 root         (0) root         (0)    42725 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/config/rcsetup.py
+-rwxrwxrwx   0 root         (0) root         (0)   209438 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2627 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/docstring.py
+-rwxrwxrwx   0 root         (0) root         (0)     5572 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/gdal_store.py
+-rwxrwxrwx   0 root         (0) root         (0)    92095 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/plotter.py
+-rwxrwxrwx   0 root         (0) root         (0)   106121 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/project.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.420055 psyplot-1.5.0/psyplot/sphinxext/
+-rwxrwxrwx   0 root         (0) root         (0)      288 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/sphinxext/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5915 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/sphinxext/extended_napoleon.py
+-rw-rw-rw-   0 root         (0) root         (0)    10939 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     4119 2024-04-02 08:14:33.000000 psyplot-1.5.0/psyplot/warning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.420055 psyplot-1.5.0/psyplot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10287 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      825 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-02 08:15:01.000000 psyplot-1.5.0/psyplot.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-02 08:14:33.000000 psyplot-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 08:15:01.424055 psyplot-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      283 2024-04-02 08:14:33.000000 psyplot-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 08:15:01.420055 psyplot-1.5.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    72398 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_gdalstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8428 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    35532 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_plotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    78242 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     7690 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_rcsetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2024-04-02 08:14:33.000000 psyplot-1.5.0/tests/test_utils.py
```

### Comparing `psyplot-1.4.3/COPYING` & `psyplot-1.5.0/LICENSES/LGPL-3.0-only.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,674 +1,304 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+GNU LESSER GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the terms and conditions of version 3 of the GNU General Public License, supplemented by the additional permissions listed below.
+
+0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser General Public License, and the "GNU GPL" refers to version 3 of the GNU General Public License.
+
+"The Library" refers to a covered work governed by this License, other than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided by the Library, but which is not otherwise based on the Library. Defining a subclass of a class defined by the Library is deemed a mode of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an Application with the Library.  The particular version of the Library with which the Combined Work was made is also called the "Linked Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the Corresponding Source for the Combined Work, excluding any source code for portions of the Combined Work that, considered in isolation, are based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the object code and/or source code for the Application, including any data and utility programs needed for reproducing the Combined Work from the Application, but excluding the System Libraries of the Combined Work.
+
+1. Exception to Section 3 of the GNU GPL.
+You may convey a covered work under sections 3 and 4 of this License without being bound by section 3 of the GNU GPL.
+
+2. Conveying Modified Versions.
+If you modify a copy of the Library, and, in your modifications, a facility refers to a function or data to be supplied by an Application that uses the facility (other than as an argument passed when the facility is invoked), then you may convey a copy of the modified version:
+
+     a) under this License, provided that you make a good faith effort to ensure that, in the event an Application does not supply the function or data, the facility still operates, and performs whatever part of its purpose remains meaningful, or
+
+     b) under the GNU GPL, with none of the additional permissions of this License applicable to that copy.
+
+3. Object Code Incorporating Material from Library Header Files.
+The object code form of an Application may incorporate material from a header file that is part of the Library.  You may convey such object code under terms of your choice, provided that, if the incorporated material is not limited to numerical parameters, data structure layouts and accessors, or small macros, inline functions and templates (ten or fewer lines in length), you do both of the following:
+
+     a) Give prominent notice with each copy of the object code that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the object code with a copy of the GNU GPL and this license document.
+
+4. Combined Works.
+You may convey a Combined Work under terms of your choice that, taken together, effectively do not restrict modification of the portions of the Library contained in the Combined Work and reverse engineering for debugging such modifications, if you also do each of the following:
+
+     a) Give prominent notice with each copy of the Combined Work that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the Combined Work with a copy of the GNU GPL and this license document.
+
+     c) For a Combined Work that displays copyright notices during execution, include the copyright notice for the Library among these notices, as well as a reference directing the user to the copies of the GNU GPL and this license document.
+
+     d) Do one of the following:
+
+           0) Convey the Minimal Corresponding Source under the terms of this License, and the Corresponding Application Code in a form suitable for, and under terms that permit, the user to recombine or relink the Application with a modified version of the Linked Version to produce a modified Combined Work, in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.
+
+          1) Use a suitable shared library mechanism for linking with the Library.  A suitable mechanism is one that (a) uses at run time a copy of the Library already present on the user's computer system, and (b) will operate properly with a modified version of the Library that is interface-compatible with the Linked Version.
+
+     e) Provide Installation Information, but only if you would otherwise be required to provide such information under section 6 of the GNU GPL, and only to the extent that such information is necessary to install and execute a modified version of the Combined Work produced by recombining or relinking the Application with a modified version of the Linked Version. (If you use option 4d0, the Installation Information must accompany the Minimal Corresponding Source and Corresponding Application Code. If you use option 4d1, you must provide the Installation Information in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.)
+
+5. Combined Libraries.
+You may place library facilities that are a work based on the Library side by side in a single library together with other library facilities that are not Applications and are not covered by this License, and convey such a combined library under terms of your choice, if you do both of the following:
+
+     a) Accompany the combined library with a copy of the same work based on the Library, uncombined with any other library facilities, conveyed under the terms of this License.
+
+     b) Give prominent notice with the combined library that part of it is a work based on the Library, and explaining where to find the accompanying uncombined form of the same work.
+
+6. Revised Versions of the GNU Lesser General Public License.
+The Free Software Foundation may publish revised and/or new versions of the GNU Lesser General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
+
+GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+Preamble
+
+The GNU General Public License is a free, copyleft license for software and other kinds of works.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
+
+For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
+
+Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
+
+Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and modification follow.
+
+TERMS AND CONDITIONS
+
+0. Definitions.
+
+“This License” refers to version 3 of the GNU General Public License.
+
+“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
+
+To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
+
+A “covered work” means either the unmodified Program or a work based on the Program.
+
+To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
+
+A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+
+2. Basic Permissions.
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+
+4. Conveying Verbatim Copies.
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+     a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+
+     b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
+
+     c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+
+     d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+     a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+
+     b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+
+     c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+
+     d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+
+     e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+
+7. Additional Terms.
+“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+     a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+
+     b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+
+     c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+
+     d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+
+     e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+
+     f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+
+8. Termination.
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+
+11. Patents.
+A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
+
+A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+
+13. Use with the GNU Affero General Public License.
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
+
+14. Revised Versions of this License.
+The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+
+15. Disclaimer of Warranty.
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest possible use to the public, the best way to achieve this is to make it free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest to attach them to the start of each source file to most effectively state the exclusion of warranty; and each file should have at least the “copyright” line and a pointer to where the full notice is found.
+
+     <one line to give the program's name and a brief idea of what it does.>
+     Copyright (C) <year>  <name of author>
+
+     This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
+If the program does terminal interaction, make it output a short notice like this when it starts in an interactive mode:
+
+     <program>  Copyright (C) <year>  <name of author>
+     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+     This is free software, and you are welcome to redistribute it under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
+
+You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
 
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psyplot-1.4.3/README.rst` & `psyplot-1.5.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,25 @@
+.. SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 ===============================================
 The psyplot interactive visualization framework
 ===============================================
 
 .. start-badges
 
-.. list-table::
-    :stub-columns: 1
-    :widths: 10 90
-
-    * - docs
-      - |docs| |joss| |zenodo|
-    * - tests
-      - |circleci| |appveyor| |codecov|
-    * - package
-      - |version| |conda| |github|
-    * - implementations
-      - |supported-versions| |supported-implementations|
-    * - get in touch
-      - |mattermost| |mailing-list| |issues|
-
-.. |docs| image:: https://img.shields.io/github/deployments/psyplot/psyplot/github-pages
-    :alt: Documentation
-    :target: http://psyplot.github.io/psyplot/
-
-.. |circleci| image:: https://circleci.com/gh/psyplot/psyplot/tree/master.svg?style=svg
-    :alt: CircleCI
-    :target: https://circleci.com/gh/psyplot/psyplot/tree/master
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/4nt6qrw66iw65w33/branch/master?svg=true
-    :alt: AppVeyor
-    :target: https://ci.appveyor.com/project/psyplot/psyplot/branch/master
-
-.. |codecov| image:: https://codecov.io/gh/psyplot/psyplot/branch/master/graph/badge.svg
-    :alt: Coverage
-    :target: https://codecov.io/gh/psyplot/psyplot
-
-.. |version| image:: https://img.shields.io/pypi/v/psyplot.svg?style=flat
-    :alt: PyPI Package latest release
-    :target: https://pypi.python.org/pypi/psyplot
-
-.. |conda| image:: https://anaconda.org/conda-forge/psyplot/badges/version.svg
-    :alt: conda
-    :target: https://anaconda.org/conda-forge/psyplot
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/psyplot.svg?style=flat
-    :alt: Supported versions
-    :target: https://pypi.python.org/pypi/psyplot
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/psyplot.svg?style=flat
-    :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/psyplot
-
-.. |joss| image:: http://joss.theoj.org/papers/3535c28017003f0b5fb63b1b64118b60/status.svg
-    :alt: Journal of Open Source Software
-    :target: http://joss.theoj.org/papers/3535c28017003f0b5fb63b1b64118b60
-
-.. |zenodo| image:: https://zenodo.org/badge/87944102.svg
-    :alt: Zenodo
-    :target: https://zenodo.org/badge/latestdoi/87944102
-
-.. |github| image:: https://img.shields.io/github/release/psyplot/psyplot.svg
-    :target: https://github.com/psyplot/psyplot/releases/latest
-    :alt: Latest github release
-
-.. |mattermost| image:: https://img.shields.io/badge/chat-on%20mattermost-success?logo=mattermost
-    :target: https://mattermost.hzdr.de/psyplot/
-    :alt: Mattermost
-
-.. |mailing-list| image:: https://img.shields.io/badge/join-mailing%20list-brightgreen.svg?style=flat
-    :target: https://www.listserv.dfn.de/sympa/subscribe/psyplot
-    :alt: DFN mailing list
-
-.. |issues| image:: https://img.shields.io/github/issues-raw/psyplot/psyplot.svg?style=flat
-    :target: https://github.com/psyplot/psyplot/issues
-    :alt: GitHub issues
+|CI|
+|Code coverage|
+|Latest Release|
+|PyPI version|
+|Code style: black|
+|Imports: isort|
+|PEP8|
+|REUSE status|
 
 .. end-badges
 
 Welcome! **psyplot** is an open source python project that mainly combines the
 plotting utilities of matplotlib_ and the data management of the xarray_
 package. The main purpose is to have a framework that allows a  fast,
 attractive, flexible, easily applicable, easily reproducible and especially
@@ -87,15 +29,15 @@
 developers in their daily work by providing a flexible visualization tool that
 can be enhanced by their own visualization scripts. ``psyplot`` can be used
 through the python command line and through the psyplot-gui_ module which
 provides a graphical user interface for an easier interactive usage.
 
 The package is very new and there are many features that will be included in
 the future. So we are very pleased for feedback! Please simply raise an issue
-on `GitHub <https://github.com/psyplot/psyplot>`__ (see also
+on `GitHub <https://codebase.helmholtz.cloud/psyplot/psyplot>`__ (see also
 `How to contribute`_ in the docs).
 
 .. _psyplot-gui: http://psyplot.github.io/psyplot-gui/
 .. _How to contribute: http://psyplot.github.io/psyplot/contribute.html
 
 You can see the full documentation on
 `psyplot.github.io/psyplot <http://psyplot.github.io/psyplot/>`__.
@@ -109,19 +51,19 @@
 - Chat with the developers in out `team on mattermost`_
 - Subscribe to the `mailing list`_ and ask for support
 - Sent a mail to psyplot@hzg.de
 
 See also the `code of conduct`_, and our `contribution guide`_ for more
 information and a guide about good bug reports.
 
-.. _bug tracker: https://github.com/psyplot/psyplot
+.. _bug tracker: https://codebase.helmholtz.cloud/psyplot/psyplot
 .. _team on mattermost: https://mattermost.hzdr.de/psyplot/
 .. _mailing list: https://www.listserv.dfn.de/sympa/subscribe/psyplot
-.. _code of conduct: https://github.com/psyplot/psyplot/blob/master/CODE_OF_CONDUCT.md
-.. _contribution guide: https://github.com/psyplot/psyplot/blob/master/CONTRIBUTING.md
+.. _code of conduct: https://codebase.helmholtz.cloud/psyplot/psyplot/blob/master/CODE_OF_CONDUCT.md
+.. _contribution guide: https://codebase.helmholtz.cloud/psyplot/psyplot/blob/master/CONTRIBUTING.md
 
 
 How to cite psyplot
 -------------------
 
 When using psyplot, you should at least cite the publication in
 `the Journal of Open Source Software`_:
@@ -139,15 +81,15 @@
 version or plugin, please refer to the `releases page of psyplot` or the
 releases page of the corresponding subproject.
 
 
 .. _the Journal of Open Source Software: http://joss.theoj.org/
 .. _subprojects: https://psyplot.github.io/
 .. _zenodo.org: https://zenodo.org/
-.. _releases page of psyplot: https://github.com/psyplot/psyplot/releases/
+.. _releases page of psyplot: https://codebase.helmholtz.cloud/psyplot/psyplot/-/releases
 
 
 Acknowledgment
 --------------
 This package is being developed by Philipp S. Sommer at the
 `Helmholtz Coastal Data Center (HCDC)`_ of the `Helmholtz-Zentrum Hereon`_.
 
@@ -201,7 +143,25 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU LGPL-3.0 license for more details.
 
 You should have received a copy of the GNU LGPL-3.0 license
 along with this program.  If not, see https://www.gnu.org/licenses/.
+
+
+.. |CI| image:: https://codebase.helmholtz.cloud/psyplot/psyplot/badges/master/pipeline.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psyplot/-/pipelines?page=1&scope=all&ref=master
+.. |Code coverage| image:: https://codebase.helmholtz.cloud/psyplot/psyplot/badges/master/coverage.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psyplot/-/graphs/develop/charts
+.. |Latest Release| image:: https://codebase.helmholtz.cloud/psyplot/psyplot/-/badges/release.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psyplot
+.. |PyPI version| image:: https://img.shields.io/pypi/v/psyplot.svg
+   :target: https://pypi.python.org/pypi/psyplot/
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Imports: isort| image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+   :target: https://pycqa.github.io/isort/
+.. |PEP8| image:: https://img.shields.io/badge/code%20style-pep8-orange.svg
+   :target: https://www.python.org/dev/peps/pep-0008/
+.. |REUSE status| image:: https://api.reuse.software/badge/codebase.helmholtz.cloud/psyplot/psyplot
+   :target: https://api.reuse.software/info/codebase.helmholtz.cloud/psyplot/psyplot
```

### Comparing `psyplot-1.4.3/psyplot/__init__.py` & `psyplot-1.5.0/psyplot/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 """psyplot visualization framework."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
 import datetime as dt
 import logging as _logging
-from psyplot.warning import warn, critical, disable_warnings
-from psyplot.config.rcsetup import rcParams
+import sys
+
 import psyplot.config as config
-from psyplot.data import (
-    ArrayList, InteractiveArray, InteractiveList, open_dataset, open_mfdataset)
+from psyplot.config.rcsetup import rcParams
+from psyplot.data import (  # noqa: F401
+    ArrayList,
+    InteractiveArray,
+    InteractiveList,
+    open_dataset,
+    open_mfdataset,
+)
+from psyplot.warning import critical, disable_warnings, warn  # noqa: F401
 
 from ._version import get_versions
-__version__ = get_versions()['version']
+
+__version__ = get_versions()["version"]
 del get_versions
 
 
 __author__ = "Philipp S. Sommer"
 __copyright__ = """
-Copyright (C) 2021 Helmholtz-Zentrum Hereon
-Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-Copyright (C) 2016-2021 University of Lausanne
+2016-2024 University of Lausanne
+2020-2021 Helmholtz-Zentrum Geesthacht
+2021-2024 Helmholtz-Zentrum hereon GmbH
 """
 __credits__ = ["Philipp S. Sommer"]
 __license__ = "LGPL-3.0-only"
 
 __maintainer__ = "Philipp S. Sommer"
 __email__ = "psyplot@hereon.de"
 
 __status__ = "Production"
 
 
 logger = _logging.getLogger(__name__)
 logger.debug(
     "%s: Initializing psyplot, version %s",
-    dt.datetime.now().isoformat(), __version__)
+    dt.datetime.now().isoformat(),
+    __version__,
+)
 logger.debug("Logging configuration file: %s", config.logcfg_path)
 logger.debug("Configuration file: %s", config.config_path)
 
 
 rcParams.HEADER += "\n\npsyplot version: " + __version__
 rcParams.load_plugins()
 rcParams.load_from_file()
@@ -97,82 +89,87 @@
     Examples
     --------
     Using the built-in JSON module, we get something like
 
     .. code-block:: python
 
         import json
+
         print(json.dumps(psyplot.get_versions(), indent=4))
         {
-            "psy_simple.plugin": {
-                "version": "1.0.0.dev0"
-            },
+            "psy_simple.plugin": {"version": "1.0.0.dev0"},
             "psyplot": {
                 "version": "1.0.0.dev0",
                 "requirements": {
                     "matplotlib": "1.5.3",
                     "numpy": "1.11.3",
                     "pandas": "0.19.2",
-                    "xarray": "0.9.1"
-                }
+                    "xarray": "0.9.1",
+                },
             },
             "psy_maps.plugin": {
                 "version": "1.0.0.dev0",
-                "requirements": {
-                    "cartopy": "0.15.0"
-                }
-            }
+                "requirements": {"cartopy": "0.15.0"},
+            },
         }
     """
     from psyplot.utils import plugin_entrypoints
+
     eps = plugin_entrypoints("psyplot", "plugin")
 
-    ret = {'psyplot': _get_versions(requirements)}
+    ret = {"psyplot": _get_versions(requirements)}
     for ep in eps:
         if str(ep) in rcParams._plugins:
-            logger.debug('Loading entrypoint %s', ep)
+            logger.debug("Loading entrypoint %s", ep)
 
             try:
                 ep.module
             except AttributeError:  # python<3.10
                 ep.module = ep.pattern.match(ep.value).group("module")
 
             if key is not None and not key(ep.module):
                 continue
             try:
                 mod = ep.load()
-            except (ImportError, ModuleNotFoundError) as e:
-                logger.debug("Could not import %s" % (ep, ), exc_info=True)
-                logger.warning("Could not import %s" % (ep, ), exc_info=True)
+            except (ImportError, ModuleNotFoundError):
+                logger.debug("Could not import %s" % (ep,), exc_info=True)
+                logger.warning("Could not import %s" % (ep,), exc_info=True)
             else:
                 try:
                     ret[str(ep.module)] = mod.get_versions(requirements)
                 except AttributeError:
                     ret[str(ep.module)] = {
-                        'version': getattr(
-                            mod, 'plugin_version',
-                            getattr(mod, '__version__', ''))
-                        }
+                        "version": getattr(
+                            mod,
+                            "plugin_version",
+                            getattr(mod, "__version__", ""),
+                        )
+                    }
     if key is None:
         try:
             import psyplot_gui
         except ImportError:
             pass
         else:
-            ret['psyplot_gui'] = psyplot_gui.get_versions(requirements)
+            ret["psyplot_gui"] = psyplot_gui.get_versions(requirements)
     return ret
 
 
 def _get_versions(requirements=True):
     if requirements:
         import matplotlib as mpl
-        import xarray as xr
-        import pandas as pd
         import numpy as np
-        return {'version': __version__,
-                'requirements': {'matplotlib': mpl.__version__,
-                                 'xarray': xr.__version__,
-                                 'pandas': pd.__version__,
-                                 'numpy': np.__version__,
-                                 'python': ' '.join(sys.version.splitlines())}}
+        import pandas as pd
+        import xarray as xr
+
+        return {
+            "version": __version__,
+            "requirements": {
+                "matplotlib": mpl.__version__,
+                "xarray": xr.__version__,
+                "pandas": pd.__version__,
+                "numpy": np.__version__,
+                "python": " ".join(sys.version.splitlines()),
+            },
+        }
     else:
-        return {'version': __version__}
+        return {"version": __version__}
```

### Comparing `psyplot-1.4.3/psyplot/__main__.py` & `psyplot-1.5.0/psyplot/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,37 @@
 # -*- coding: utf-8 -*-
 """Main commandline entrypoint for psyplot."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import os
-import os.path as osp
-import sys
 import argparse
-import pickle
-import six
 import glob
-from itertools import chain
+import json
+import logging
+import os.path as osp
+import pickle
+import sys
 from collections import defaultdict
-import yaml
+from itertools import chain
+
+import six
 import xarray as xr
+import yaml
+from funcargparse import FuncArgParser
+
 import psyplot
+from psyplot.config.rcsetup import rcParams, safe_list
 from psyplot.docstring import docstrings
+from psyplot.utils import get_default_value
 from psyplot.warning import warn
-from psyplot.compat.pycompat import get_default_value
-from funcargparse import FuncArgParser
-import logging
-
-rcParams = psyplot.rcParams
-
 
 logger = logging.getLogger(__name__)
 
 
 def main(args=None):
     """Main function for usage of psyplot from the command line
 
@@ -57,34 +41,48 @@
 
     Returns
     -------
     psyplot.parser.FuncArgParser
         The parser that has been used from the command line"""
     try:
         from psyplot_gui import get_parser as _get_parser
-    except (ImportError, ModuleNotFoundError) as e:
-        logger.debug('Failed to import gui', exc_info=True)
+    except (ImportError, ModuleNotFoundError):
+        logger.debug("Failed to import gui", exc_info=True)
         parser = get_parser(create=False)
-        parser.update_arg('output', required=True)
+        parser.update_arg("output", required=True)
         parser.create_arguments()
         parser.parse2func(args)
     else:
         parser = _get_parser(create=False)
         parser.create_arguments()
         parser.parse_known2func(args)
 
 
-@docstrings.get_sections(base='make_plot')
+@docstrings.get_sections(base="make_plot")
 @docstrings.dedent
-def make_plot(fnames=[], name=[], dims=None, plot_method=None,
-              output=None, project=None, engine=None, formatoptions=None,
-              tight=False, rc_file=None, encoding=None, enable_post=False,
-              seaborn_style=None, output_project=None,
-              concat_dim=get_default_value(xr.open_mfdataset, 'concat_dim'),
-              chname={}, preset=None):
+def make_plot(
+    fnames=[],
+    name=[],
+    dims=None,
+    plot_method=None,
+    output=None,
+    project=None,
+    engine=None,
+    formatoptions=None,
+    tight=False,
+    rc_file=None,
+    encoding=None,
+    enable_post=False,
+    seaborn_style=None,
+    output_project=None,
+    concat_dim=get_default_value(xr.open_mfdataset, "concat_dim"),
+    chname={},
+    preset=None,
+    decoder=None,
+):
     """
     Eventually start the QApplication or only make a plot
 
     Parameters
     ----------
     fnames: list of str
         Either the filenames to show, or, if the `project` parameter is set,
@@ -135,62 +133,83 @@
         A mapping from variable names in the project to variable names in the
         datasets that should be used instead
     preset: str
         The filename or identifier of a preset. If the given `preset` is
         the path to an existing yaml file, it will be loaded. Otherwise we
         look up the `preset` in the psyplot configuration directory (see
         :func:`~psyplot.config.rcsetup.get_configdir`).
+    decoder: str
+        Keyword arguments for the decoder.
     """
     if project is not None and (name != [] or dims is not None):
-        warn('The `name` and `dims` parameter are ignored if the `project`'
-             ' parameter is set!')
+        warn(
+            "The `name` and `dims` parameter are ignored if the `project`"
+            " parameter is set!"
+        )
     if rc_file is not None:
         rcParams.load_from_file(rc_file)
 
     if dims is not None and not isinstance(dims, dict):
         dims = dict(chain(*map(six.iteritems, dims)))
 
     if len(output) == 1:
         output = output[0]
     if not fnames and not project:
         raise ValueError(
             "Either a filename or a project file must be provided if "
-            "the output parameter is set!")
+            "the output parameter is set!"
+        )
     elif project is None and plot_method is None:
         raise ValueError(
             "A plotting method must be provided if the output parameter "
-            "is set and not the project!")
+            "is set and not the project!"
+        )
     if seaborn_style is not None:
         import seaborn as sns
+
         sns.set_style(seaborn_style)
     import psyplot.project as psy
+
     if project is not None:
-        fnames = [s.split(',') for s in fnames]
+        fnames = [s.split(",") for s in fnames]
         chname = dict(chname)
-        single_files = (l[0] for l in fnames if len(l) == 1)
+        single_files = (fn_list[0] for fn_list in fnames if len(fn_list) == 1)
         alternative_paths = defaultdict(lambda: next(single_files, None))
-        alternative_paths.update([l for l in fnames if len(l) == 2])
+        alternative_paths.update(
+            (fn_list for fn_list in fnames if len(fn_list) == 2)
+        )
         p = psy.Project.load_project(
-            project, alternative_paths=alternative_paths,
-            engine=engine, encoding=encoding, enable_post=enable_post,
-            chname=chname)
+            project,
+            alternative_paths=alternative_paths,
+            engine=engine,
+            encoding=encoding,
+            enable_post=enable_post,
+            chname=chname,
+        )
         if preset:
             p.load_preset(preset)
         if formatoptions is not None:
             p.update(fmt=formatoptions)
         p.export(output, tight=tight)
     else:
         pm = getattr(psy.plot, plot_method, None)
         if pm is None:
             raise ValueError("Unknown plot method %s!" % plot_method)
-        kwargs = {'name': name} if name else {}
+        kwargs = {"name": name} if name else {}
         p = pm(
-            fnames, dims=dims or {}, engine=engine, preset=preset,
-            fmt=formatoptions or {}, mf_mode=True, concat_dim=concat_dim,
-            **kwargs)
+            fnames,
+            dims=dims or {},
+            engine=engine,
+            preset=preset,
+            fmt=formatoptions or {},
+            mf_mode=True,
+            concat_dim=concat_dim,
+            decoder=decoder,
+            **kwargs,
+        )
         p.export(output, tight=tight)
     if output_project is not None:
         p.save_project(output_project)
     return
 
 
 def get_parser(create=True):
@@ -198,15 +217,17 @@
     from the command line
 
     Returns
     -------
     psyplot.parser.FuncArgParser
         The :class:`argparse.ArgumentParser` instance"""
     #: The parse that is used to parse arguments from the command line
-    epilog = docstrings.get_sections(docstrings.dedent("""
+    epilog = docstrings.get_sections(
+        docstrings.dedent(
+            """
         Examples
         --------
 
         Here are some examples on how to use psyplot from the command line.
 
         Plot the variable ``'t2m'`` in a netCDF file ``'myfile.nc'`` and save
         the plot to ``'plot.pdf'``::
@@ -233,226 +254,423 @@
 
             $ psyplot old_ds.nc,other_ds.nc -p project.pkl -o test.pdf
 
         You can also load formatoptions from a configuration file, e.g.::
 
             $ echo 'title: my title' > fmt.yaml
             $ psyplot myfile.nc -n t2m  -pm mapplot -fmt fmt.yaml -o test.pdf
-        """), 'parser', ['Examples'])
+        """
+        ),
+        "parser",
+        ["Examples"],
+    )
 
-    epilog = '.. rubric:: Examples\n' + '\n'.join(epilog.splitlines()[2:])
+    epilog = ".. rubric:: Examples\n" + "\n".join(epilog.splitlines()[2:])
 
     parser = FuncArgParser(
         description="""
         Load a dataset, make the plot and save the result to a file""",
         epilog=epilog,
-        formatter_class=argparse.RawDescriptionHelpFormatter)
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
 
     info_grp = parser.add_argument_group(
-        'Info options',
-        'Options that print informations and quit afterwards')
+        "Info options", "Options that print informations and quit afterwards"
+    )
+
+    parser.update_arg(
+        "version",
+        short="V",
+        long="version",
+        action="version",
+        version=psyplot.__version__,
+        if_existent=False,
+        group=info_grp,
+    )
 
-    parser.update_arg('version', short='V', long='version', action='version',
-                      version=psyplot.__version__, if_existent=False,
-                      group=info_grp)
+    parser.update_arg(
+        "all_versions",
+        short="aV",
+        long="all-versions",
+        action=AllVersionsAction,
+        if_existent=False,
+        group=info_grp,
+    )
 
-    parser.update_arg('all_versions', short='aV', long='all-versions',
-                      action=AllVersionsAction, if_existent=False,
-                      group=info_grp)
+    parser.update_arg(
+        "info",
+        short="i",
+        long="info",
+        action=ShowGridInfo,
+        if_existent=False,
+        group=info_grp,
+    )
 
-    parser.update_arg('list_plugins', short='lp', long='list-plugins',
-                      action=ListPluginsAction, if_existent=False,
-                      group=info_grp)
     parser.update_arg(
-        'list_plot_methods', short='lpm', long='list-plot-methods',
-        action=ListPlotMethodsAction, if_existent=False, group=info_grp)
+        "list_plugins",
+        short="lp",
+        long="list-plugins",
+        action=ListPluginsAction,
+        if_existent=False,
+        group=info_grp,
+    )
     parser.update_arg(
-        'list_datasets', short='lds', long='list-datasets',
-        action=ListDsNamesAction, if_existent=False, group=info_grp,
-        help="""List the used dataset names in the given `project`.""")
+        "list_plot_methods",
+        short="lpm",
+        long="list-plot-methods",
+        action=ListPlotMethodsAction,
+        if_existent=False,
+        group=info_grp,
+    )
+    parser.update_arg(
+        "list_datasets",
+        short="lds",
+        long="list-datasets",
+        action=ListDsNamesAction,
+        if_existent=False,
+        group=info_grp,
+        help="""List the used dataset names in the given `project`.""",
+    )
 
     parser.update_arg(
-        'list_presets', short='lps', long='list-presets',
-        action=ListPresetsAction, if_existent=False, group=info_grp)
+        "list_presets",
+        short="lps",
+        long="list-presets",
+        action=ListPresetsAction,
+        if_existent=False,
+        group=info_grp,
+    )
 
     parser.setup_args(make_plot)
 
     output_grp = parser.add_argument_group(
-        'Output options',
-        'Options that only have an effect if the `-o` option is set.')
-
-    parser.update_arg('fnames', positional=True, nargs='*')
+        "Output options",
+        "Options that only have an effect if the `-o` option is set.",
+    )
 
-    parser.update_arg('name', short='n', nargs='*', metavar='variable_name',
-                      const=None)
+    parser.update_arg("fnames", positional=True, nargs="*")
 
-    parser.update_arg('dims', short='d', nargs='+', type=_load_dims,
-                      metavar='dim,val1[,val2[,...]]')
+    parser.update_arg(
+        "name", short="n", nargs="*", metavar="variable_name", const=None
+    )
 
-    pm_choices = {pm for pm, d in filter(
-                      lambda t: t[1].get('plot_func', True),
-                      six.iteritems(rcParams['project.plotters']))}
+    parser.update_arg(
+        "dims",
+        short="d",
+        nargs="+",
+        type=_load_dims,
+        metavar="dim,val1[,val2[,...]]",
+    )
+
+    pm_choices = {
+        pm
+        for pm, d in filter(
+            lambda t: t[1].get("plot_func", True),
+            six.iteritems(rcParams["project.plotters"]),
+        )
+    }
     if psyplot._project_imported:
         import psyplot.project as psy
+
         pm_choices.update(set(psy.plot._plot_methods))
-    parser.update_arg('plot_method', short='pm', choices=pm_choices,
-                      metavar='{%s}' % ', '.join(map(repr, pm_choices)))
+    parser.update_arg(
+        "plot_method",
+        short="pm",
+        choices=pm_choices,
+        metavar="{%s}" % ", ".join(map(repr, pm_choices)),
+    )
 
-    parser.update_arg('output', short='o', group=output_grp)
-    parser.update_arg('output_project', short='op', group=output_grp)
+    parser.update_arg("output", short="o", group=output_grp)
+    parser.update_arg("output_project", short="op", group=output_grp)
 
-    parser.update_arg('project', short='p')
+    parser.update_arg("project", short="p")
 
     parser.update_arg(
-        'formatoptions', short='fmt', type=_load_dict, help="""
-        The path to a yaml (``'.yml'`` or ``'.yaml'``) or pickle file
-        defining a dictionary of formatoption that is applied to the data
-        visualized by the chosen `plot_method`""", metavar='FILENAME')
+        "formatoptions",
+        short="fmt",
+        type=_load_dict,
+        help="""
+        YAML-formatted formatoption (e.g. 'cmap: Reds'), or the path to a yaml
+        (``'.yml'`` or ``'.yaml'``), JSON (``'.json'``) or  pickle file
+        defining a dictionary of formatoption that is applied to the
+        data visualized by the chosen `plot_method`""",
+        metavar="FILENAME_OR_YAML",
+    )
 
     parser.update_arg(
-        'chname', type=lambda s: s.split(','), nargs='*', help="""
+        "decoder",
+        long="decoder",
+        short=None,
+        type=_load_decoder,
+        help="""
+        YAML-formatted decoder options (e.g. 'x: x-coordinate'), or the path to
+        a yaml (``'.yml'`` or ``'.yaml'``), JSON (``'.json'``) or  pickle file
+        defining a dictionary of formatoption that is applied to the
+        data visualized by the chosen `plot_method`""",
+        metavar="FILENAME_OR_YAML",
+    )
+
+    parser.update_arg(
+        "chname",
+        type=lambda s: s.split(","),
+        nargs="*",
+        help="""
         A mapping from variable names in the project to variable names in the
         datasets that should be used instead. Variable names should be
-        separated by a comma.""", metavar='project-variable,variable-to-use')
+        separated by a comma.""",
+        metavar="project-variable,variable-to-use",
+    )
 
-    parser.update_arg('tight', short='t', group=output_grp)
+    parser.update_arg("tight", short="t", group=output_grp)
 
-    parser.update_arg('rc_file', short='rc')
-    parser.pop_key('rc_file', 'metavar')
+    parser.update_arg("rc_file", short="rc")
+    parser.pop_key("rc_file", "metavar")
 
-    parser.update_arg('encoding', short='e')
+    parser.update_arg("encoding", short="e")
 
-    parser.pop_key('enable_post', 'short')
+    parser.pop_key("enable_post", "short")
 
-    parser.update_arg('seaborn_style', short='sns')
+    parser.update_arg("seaborn_style", short="sns")
 
-    parser.update_arg('concat_dim', short='cd')
+    parser.update_arg("concat_dim", short="cd")
 
     if create:
         parser.create_arguments()
 
     return parser
 
 
 def _load_dict(fname):
-    with open(fname) as f:
-        if fname.endswith('.yml') or fname.endswith('.yaml'):
-            return yaml.load(f, Loader=yaml.SafeLoader)
-        return pickle.load(f)
+    data = yaml.safe_load(fname)
+    if isinstance(data, str):  # assume a file and load from disc
+        with open(data) as f:
+            if data.endswith(".yml") or data.endswith(".yaml"):
+                return yaml.safe_load(f)
+            elif data.endswith(".json"):
+                return json.load(f)
+            return pickle.load(f)
+    return data
+
+
+def _load_decoder(fname):
+    data = _load_dict(fname)
+    for key in "xyzt":
+        if key in data:
+            data[key] = set(safe_list(data[key]))
+    return data
 
 
 def _load_dims(s):
-    s = s.split(',')
+    s = s.split(",")
     if len(s) > 1:
         return {s[0]: list(map(int, s[1:]))}
     return {}
 
 
 class AllVersionsAction(argparse.Action):
-
-    def __init__(self, option_strings, dest=argparse.SUPPRESS, nargs=None,
-                 default=argparse.SUPPRESS, **kwargs):
+    def __init__(
+        self,
+        option_strings,
+        dest=argparse.SUPPRESS,
+        nargs=None,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        kwargs['help'] = ("Print the versions of all plugins and requirements "
-                          "and exit")
-        kwargs['default'] = default
+        kwargs["help"] = (
+            "Print the versions of all plugins and requirements " "and exit"
+        )
+        kwargs["default"] = default
         super(AllVersionsAction, self).__init__(
-            option_strings, nargs=0, dest=dest,
-            **kwargs)
+            option_strings, nargs=0, dest=dest, **kwargs
+        )
 
     def __call__(self, parser, namespace, values, option_string=None):
         print(yaml.dump(psyplot.get_versions(), default_flow_style=False))
         sys.exit(0)
 
 
 class ListPresetsAction(argparse.Action):
-
-    def __init__(self, option_strings, dest=argparse.SUPPRESS, nargs=None,
-                 default=argparse.SUPPRESS, **kwargs):
+    def __init__(
+        self,
+        option_strings,
+        dest=argparse.SUPPRESS,
+        nargs=None,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        kwargs['help'] = ("Print available presets and exit")
-        kwargs['default'] = default
+        kwargs["help"] = "Print available presets and exit"
+        kwargs["default"] = default
         super().__init__(option_strings, nargs=0, dest=dest, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         from psyplot.config.rcsetup import get_configdir
-        presets_dir = osp.join(get_configdir(), 'presets')
+
+        presets_dir = osp.join(get_configdir(), "presets")
         if not osp.exists(presets_dir):
             sys.exit(0)
         else:
-            presets = {osp.splitext(osp.basename(fname))[0]: fname
-                       for fname in glob.glob(osp.join(presets_dir, '*.yml'))}
-            print('\n'.join(map(': '.join, presets.items())))
+            presets = {
+                osp.splitext(osp.basename(fname))[0]: fname
+                for fname in glob.glob(osp.join(presets_dir, "*.yml"))
+            }
+            print("\n".join(map(": ".join, presets.items())))
             sys.exit(0)
 
-class ListPluginsAction(argparse.Action):
 
-    def __init__(self, option_strings, dest=argparse.SUPPRESS, nargs=None,
-                 default=argparse.SUPPRESS, **kwargs):
+class ListPluginsAction(argparse.Action):
+    def __init__(
+        self,
+        option_strings,
+        dest=argparse.SUPPRESS,
+        nargs=None,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        kwargs['help'] = ("Print the names of the plugins and exit")
-        kwargs['default'] = default
+        kwargs["help"] = "Print the names of the plugins and exit"
+        kwargs["default"] = default
         super(ListPluginsAction, self).__init__(
-            option_strings, nargs=0, dest=dest, **kwargs)
+            option_strings, nargs=0, dest=dest, **kwargs
+        )
 
     def __call__(self, parser, namespace, values, option_string=None):
         print(yaml.dump(psyplot.rcParams._plugins, default_flow_style=False))
         sys.exit(0)
 
 
-class ListPlotMethodsAction(argparse.Action):
+class ShowGridInfo(argparse.Action):
+    """Action to show the grid info on a variable"""
 
-    def __init__(self, option_strings, dest=argparse.SUPPRESS, nargs=None,
-                 default=argparse.SUPPRESS, **kwargs):
+    def __init__(
+        self,
+        option_strings,
+        nargs=None,
+        dest=argparse.SUPPRESS,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        kwargs['help'] = "List the available plot methods and what they do"
-        kwargs['default'] = default
+        kwargs.setdefault(
+            "help", "Show grid information on the specified variables."
+        )
+        super().__init__(
+            option_strings, nargs=0, dest=dest, default=default, **kwargs
+        )
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        from psyplot.data import CFDecoder, open_dataset, open_mfdataset
+
+        if not namespace.fnames:
+            print("Please specify a dataset for the info option.")
+        fnames = namespace.fnames
+        engine = namespace.engine
+        concat_dim = namespace.concat_dim
+        mf_mode = len(fnames) > 1
+        if mf_mode:
+            ds = open_mfdataset(fnames, engine=engine, concat_dim=concat_dim)
+        else:
+            ds = open_dataset(fnames[0], engine=engine)
+
+        data = {}
+
+        names = namespace.name or list(ds.variables)
+
+        if not names:
+            print("No variables found in the given dataset.")
+            sys.exit(1)
+
+        decoder_kwargs = namespace.decoder or {}
+
+        for name in names:
+            if name not in ds.variables:
+                data[name] = {
+                    "error": f"Variable {name} could not be found in the dataset."
+                }
+                continue
+            decoder = CFDecoder.get_decoder(ds, ds[name], **decoder_kwargs)
+            data[name] = decoder.get_metadata_for_variable(ds[name])
+        print(yaml.dump(data, default_flow_style=False))
+        sys.exit(0)
+
+
+class ListPlotMethodsAction(argparse.Action):
+    def __init__(
+        self,
+        option_strings,
+        dest=argparse.SUPPRESS,
+        nargs=None,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
+        if nargs is not None:
+            raise ValueError("nargs not allowed")
+        kwargs["help"] = "List the available plot methods and what they do"
+        kwargs["default"] = default
         super(ListPlotMethodsAction, self).__init__(
-            option_strings, nargs=0, dest=dest, **kwargs)
+            option_strings, nargs=0, dest=dest, **kwargs
+        )
 
     def __call__(self, parser, namespace, values, option_string=None):
         pm_choices = {}
-        for pm, d in filter(lambda t: t[1].get('plot_func', True),
-                            six.iteritems(rcParams['project.plotters'])):
-            pm_choices[pm] = d.get('summary') or (
-                'Open and plot data via :class:`%s.%s` plotters' % (
-                    d['module'], d['plotter_name']))
+        for pm, d in filter(
+            lambda t: t[1].get("plot_func", True),
+            six.iteritems(rcParams["project.plotters"]),
+        ):
+            pm_choices[pm] = d.get("summary") or (
+                "Open and plot data via :class:`%s.%s` plotters"
+                % (d["module"], d["plotter_name"])
+            )
         if psyplot._project_imported:
             import psyplot.project as psy
+
             pm_choices.update(psy.plot._plot_methods)
         print(yaml.dump(pm_choices, default_flow_style=False))
         sys.exit(0)
 
 
 class ListDsNamesAction(argparse.Action):
     """An action to list the used file names in a project"""
 
-    def __init__(self, option_strings, dest=argparse.SUPPRESS, nargs=None,
-                 default=argparse.SUPPRESS, **kwargs):
+    def __init__(
+        self,
+        option_strings,
+        dest=argparse.SUPPRESS,
+        nargs=None,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        kwargs['default'] = default
+        kwargs["default"] = default
         super(ListDsNamesAction, self).__init__(
-            option_strings, nargs=0, dest=dest, **kwargs)
+            option_strings, nargs=0, dest=dest, **kwargs
+        )
 
     def __call__(self, parser, namespace, values, option_string=None):
         if namespace.project is None:
-            print('A project is required before this argument! Call syntax:\n'
-                  '%s -p <project-file>.pkl %s' % (parser.prog, option_string))
+            print(
+                "A project is required before this argument! Call syntax:\n"
+                "%s -p <project-file>.pkl %s" % (parser.prog, option_string)
+            )
             sys.exit(1)
-        import psyplot.data as psyd
         import pickle
-        with open(namespace.project, 'rb') as f:
-            d = pickle.load(f)['arrays']
-        names = list(filter(None, (
-            t[0] for t in psyd.ArrayList._get_dsnames(d))))
+
+        import psyplot.data as psyd
+
+        with open(namespace.project, "rb") as f:
+            d = pickle.load(f)["arrays"]
+        names = list(
+            filter(None, (t[0] for t in psyd.ArrayList._get_dsnames(d)))
+        )
         if names:
             print(yaml.dump(names, default_flow_style=False))
         sys.exit(0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `psyplot-1.4.3/psyplot/config/logsetup.py` & `psyplot-1.5.0/psyplot/config/logsetup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,60 @@
 """Logging configuration module of the psyplot package
 
 This module defines the essential functions for setting up the
 :class:`logging.Logger` instances that are used by the psyplot package."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import os
-import six
-import sys
 import logging
 import logging.config
+import os
+import sys
+
+import six
 import yaml
+
 from psyplot.docstring import dedent
 
 
 def _get_home():
     """Find user's home directory if possible.
     Otherwise, returns None.
 
     :see:  http://mail.python.org/pipermail/python-list/2005-February/325395.html
 
     This function is copied from matplotlib version 1.4.3, Jan 2016
     """
     try:
-        if six.PY2 and sys.platform == 'win32':
+        if six.PY2 and sys.platform == "win32":
             path = os.path.expanduser(b"~").decode(sys.getfilesystemencoding())
         else:
             path = os.path.expanduser("~")
     except ImportError:
         # This happens on Google App Engine (pwd module is not present).
         pass
     else:
         if os.path.isdir(path):
             return path
-    for evar in ('HOME', 'USERPROFILE', 'TMP'):
+    for evar in ("HOME", "USERPROFILE", "TMP"):
         path = os.environ.get(evar)
         if path is not None and os.path.isdir(path):
             return path
     return None
 
 
 @dedent
-def setup_logging(default_path=None, default_level=logging.INFO,
-                  env_key='LOG_PSYPLOT'):
+def setup_logging(
+    default_path=None, default_level=logging.INFO, env_key="LOG_PSYPLOT"
+):
     """
     Setup logging configuration
 
     Parameters
     ----------
     default_path: str
         Default path of the yaml logging configuration file. If None, it
@@ -85,24 +72,24 @@
         Path to the logging configuration file
 
     Notes
     -----
     Function taken from
     http://victorlin.me/posts/2012/08/26/good-logging-practice-in-python"""
     path = default_path or os.path.join(
-        os.path.dirname(__file__), 'logging.yml')
+        os.path.dirname(__file__), "logging.yml"
+    )
     value = os.getenv(env_key, None)
     home = _get_home()
     if value:
         path = value
     if os.path.exists(path):
-        with open(path, 'rt') as f:
+        with open(path, "rt") as f:
             config = yaml.load(f.read(), Loader=yaml.SafeLoader)
-        for handler in config.get('handlers', {}).values():
-            if '~' in handler.get('filename', ''):
-                handler['filename'] = handler['filename'].replace(
-                    '~', home)
+        for handler in config.get("handlers", {}).values():
+            if "~" in handler.get("filename", ""):
+                handler["filename"] = handler["filename"].replace("~", home)
         logging.config.dictConfig(config)
     else:
         path = None
         logging.basicConfig(level=default_level)
     return path
```

### Comparing `psyplot-1.4.3/psyplot/config/rcsetup.py` & `psyplot-1.5.0/psyplot/config/rcsetup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,123 +3,109 @@
 This module defines the necessary classes, data and functions for the default
 configuration of the module.
 The structure is motivated and to larger parts taken from the matplotlib_
 package.
 
 .. _matplotlib: http://matplotlib.org/api/"""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
+import contextlib
+import inspect
+import logging
 import os
+import re
 import sys
+from collections import UserDict, defaultdict
+from itertools import chain
+
 import six
-import logging
-import re
-import inspect
 import yaml
-import contextlib
-from itertools import chain
-from collections import defaultdict
-from psyplot.warning import warn
-from psyplot.compat.pycompat import (
-    UserDict, DictMethods, getcwd, zip, isstring, map)
-from psyplot.docstring import docstrings, dedent, safe_modulo
+
 from psyplot.config.logsetup import _get_home
+from psyplot.docstring import dedent, docstrings, safe_modulo
+from psyplot.utils import isstring
+from psyplot.warning import warn
 
 
-@docstrings.get_sections(base='safe_list')
+@docstrings.get_sections(base="safe_list")
 @dedent
-def safe_list(l):
+def safe_list(iterable):
     """Function to create a list
 
     Parameters
     ----------
-    l: iterable or anything else
+    iterable: iterable or anything else
         Parameter that shall be converted to a list.
 
         - If string or any non-iterable, it will be put into a list
         - if iterable, it will be converted to a list
 
     Returns
     -------
     list
         `l` put (or converted) into a list"""
-    if isstring(l):
-        return [l]
+    if isstring(iterable):
+        return [iterable]
     try:
-        return list(l)
+        return list(iterable)
     except TypeError:
-        return [l]
+        return [iterable]
 
 
-class SubDict(UserDict, dict):
+class SubDict(UserDict, dict):  # type: ignore
     """Class that keeps week reference to the base dictionary
 
-This class is used by the :meth:`RcParams.find_and_replace` method
-to provide an easy handable instance that keeps reference to the
-base rcParams dictionary."""
+    This class is used by the :meth:`RcParams.find_and_replace` method
+    to provide an easy handable instance that keeps reference to the
+    base rcParams dictionary."""
 
     @property
     def data(self):
         """Dictionary representing this :class:`SubDict` instance
 
         See Also
         --------
         iteritems
         """
-        return dict(self.iteritems())
+        return dict(list(self.iteritems()))
 
     @property
     def replace(self):
         """:class:`bool`. If True, matching strings in the :attr:`base_str`
         attribute are replaced with an empty string."""
         return self._replace
 
     @replace.setter
     def replace(self, value):
         def replace_base(key):
             for pattern in self.patterns:
                 try:
-                    return pattern.match(key).group('key')
+                    return pattern.match(key).group("key")
                 except AttributeError:  # if match is None
                     pass
             raise KeyError(
                 "Could not find any matching key for %s in the base "
-                "dictionary!" % key)
+                "dictionary!" % key
+            )
 
         value = bool(value)
-        if hasattr(self, '_replace') and value == self._replace:
+        if hasattr(self, "_replace") and value == self._replace:
             return
-        if not hasattr(self, '_replace'):
+        if not hasattr(self, "_replace"):
             self._replace = value
             return
         # if the value has changed, we change the key in the SubDict instance
         # to match the ones in the base dictionary (if they exist)
-        for key, val in DictMethods.iteritems(self):
+        for key, val in iter(dict.items(self)):
             try:
                 if value:
                     new_key = replace_base(key)
                 else:
                     new_key = self._get_val_and_base(key)[0]
             except KeyError:
                 continue
@@ -137,19 +123,20 @@
     #: list of compiled patterns from the :attr:`base_str` attribute, that
     #: are used to look for the matching keys in :attr:`base`
     patterns = []
 
     #: :class:`bool`. If True, changes are traced back to the :attr:`base` dict
     trace = False
 
-    @docstrings.get_sections(base='SubDict.add_base_str')
+    @docstrings.get_sections(base="SubDict.add_base_str")
     @dedent
-    def add_base_str(self, base_str, pattern='.+', pattern_base=None,
-                     append=True):
-        """
+    def add_base_str(
+        self, base_str, pattern=".+", pattern_base=None, append=True
+    ):
+        r"""
         Add further base string to this instance
 
         Parameters
         ----------
         base_str: str or list of str
             Strings that are used as to look for keys to get and set keys in
             the :attr:`base` dictionary. If a string does not contain
@@ -172,33 +159,48 @@
         append: bool
             If True, the given `base_str` are appended (i.e. it is first
             looked for them in the :attr:`base` dictionary), otherwise they are
             put at the beginning"""
         base_str = safe_list(base_str)
         pattern_base = safe_list(pattern_base or [])
         for i, s in enumerate(base_str):
-            if '%(key)s' not in s:
-                base_str[i] += '%(key)s'
+            if "%(key)s" not in s:
+                base_str[i] += "%(key)s"
         if pattern_base:
             for i, s in enumerate(pattern_base):
-                if '%(key)s' not in s:
-                    pattern_base[i] += '%(key)s'
+                if "%(key)s" not in s:
+                    pattern_base[i] += "%(key)s"
         else:
             pattern_base = base_str
         self.base_str = base_str + self.base_str
-        self.patterns = list(map(lambda s: re.compile(s.replace(
-            '%(key)s', '(?P<key>%s)' % pattern)), pattern_base)) + \
-            self.patterns
+        self.patterns = (
+            list(
+                map(
+                    lambda s: re.compile(
+                        s.replace("%(key)s", "(?P<key>%s)" % pattern)
+                    ),
+                    pattern_base,
+                )
+            )
+            + self.patterns
+        )
 
-    docstrings.delete_params('SubDict.add_base_str.parameters', 'append')
+    docstrings.delete_params("SubDict.add_base_str.parameters", "append")
 
-    @docstrings.get_sections(base='SubDict')
+    @docstrings.get_sections(base="SubDict")
     @docstrings.dedent
-    def __init__(self, base, base_str, pattern='.+', pattern_base=None,
-                 trace=False, replace=True):
+    def __init__(
+        self,
+        base,
+        base_str,
+        pattern=".+",
+        pattern_base=None,
+        trace=False,
+        replace=True,
+    ):
         """
         Parameters
         ----------
         base: dict
             base dictionary
         %(SubDict.add_base_str.parameters.no_append)s
         trace: bool
@@ -267,19 +269,20 @@
         --------
         RcParams.find_and_replace"""
         self.base = base
         self.base_str = []
         self.patterns = []
         self.replace = bool(replace)
         self.trace = bool(trace)
-        self.add_base_str(base_str, pattern=pattern, pattern_base=pattern_base,
-                          append=False)
+        self.add_base_str(
+            base_str, pattern=pattern, pattern_base=pattern_base, append=False
+        )
 
     def __getitem__(self, key):
-        if key in DictMethods.iterkeys(self):
+        if key in iter(dict.keys(self)):
             return dict.__getitem__(self, key)
         if not self.replace:
             return self.base[key]
         return self._get_val_and_base(key)[1]
 
     def __setitem__(self, key, val):
         # set it in the SubDict instance if trace is False
@@ -308,44 +311,44 @@
             found = True
             try:
                 m = patt.match(s)
                 if m:
                     return m.group(), self.base[m.group()]
                 else:
                     raise KeyError(
-                        "{0} does not match the specified pattern!".format(
-                            s))
-            except KeyError as e:
+                        "{0} does not match the specified pattern!".format(s)
+                    )
+            except KeyError:
                 pass
         if not found:
             if e is not None:
                 raise
-        raise KeyError("{0} does not match the specified pattern!".format(
-                            key))
+        raise KeyError("{0} does not match the specified pattern!".format(key))
 
     def _iter_base_and_pattern(self, key):
         return zip(
-            map(lambda s: safe_modulo(s, {'key': key}), self.base_str),
-            self.patterns)
+            map(lambda s: safe_modulo(s, {"key": key}), self.base_str),
+            self.patterns,
+        )
 
     def iterkeys(self):
         """Unsorted iterator over keys"""
         patterns = self.patterns
         replace = self.replace
         seen = set()
         for key in six.iterkeys(self.base):
             for pattern in patterns:
                 m = pattern.match(key)
                 if m:
-                    ret = m.group('key') if replace else m.group()
+                    ret = m.group("key") if replace else m.group()
                     if ret not in seen:
                         seen.add(ret)
                         yield ret
                     break
-        for key in DictMethods.iterkeys(self):
+        for key in iter(dict.keys(self)):
             if key not in seen:
                 yield key
 
     def iteritems(self):
         """Unsorted iterator over items"""
         return ((key, self[key]) for key in self.iterkeys())
 
@@ -355,15 +358,15 @@
 
     def update(self, *args, **kwargs):
         """Update the dictionary"""
         for k, v in six.iteritems(dict(*args, **kwargs)):
             self[k] = v
 
 
-docstrings.delete_params('SubDict.parameters', 'base')
+docstrings.delete_params("SubDict.parameters", "base")
 
 
 class RcParams(dict):
     """A dictionary object including validation
 
     validating functions are defined and associated with rc parameters in
     :data:`defaultParams`
@@ -372,23 +375,28 @@
     :class:`~matplotlib.RcParams` but has the additional
     :meth:`find_and_replace` method."""
 
     @property
     def validate(self):
         """Dictionary with validation methods as values"""
         depr = self._all_deprecated
-        return dict((key, val[1]) for key, val in
-                    six.iteritems(self.defaultParams)
-                    if key not in depr)
+        return dict(
+            (key, val[1])
+            for key, val in six.iteritems(self.defaultParams)
+            if key not in depr
+        )
 
     @property
     def descriptions(self):
         """The description of each keyword in the rcParams dictionary"""
-        return {key: val[2] for key, val in six.iteritems(self.defaultParams)
-                if len(val) >= 3}
+        return {
+            key: val[2]
+            for key, val in six.iteritems(self.defaultParams)
+            if len(val) >= 3
+        }
 
     HEADER = """Configuration parameters of the psyplot module
 
 You can copy this file (or parts of it) to another path and save it as
 psyplotrc.yml. The directory should then be stored in the PSYPLOTCONFIGDIR
 environment variable."""
 
@@ -404,15 +412,15 @@
 
     @property
     def _all_deprecated(self):
         return set(chain(self._deprecated_ignore_map, self._deprecated_map))
 
     @property
     def defaultParams(self):
-        return getattr(self, '_defaultParams', defaultParams)
+        return getattr(self, "_defaultParams", defaultParams)
 
     @defaultParams.setter
     def defaultParams(self, value):
         self._defaultParams = value
 
     @defaultParams.deleter
     def defaultParams(self):
@@ -429,26 +437,29 @@
             dictionary is used
 
         Other Parameters
         ----------------
         *args, **kwargs
             Any key-value pair for the initialization of the dictionary
         """
-        defaultParams = kwargs.pop('defaultParams', None)
+        defaultParams = kwargs.pop("defaultParams", None)
         if defaultParams is not None:
             self.defaultParams = defaultParams
         self._deprecated_map = {}
         self._deprecated_ignore_map = {}
         for k, v in six.iteritems(dict(*args, **kwargs)):
             try:
                 self[k] = v
             except (ValueError, RuntimeError):
                 # force the issue
-                warn(_rcparam_warn_str.format(key=repr(k), value=repr(v),
-                                              func='__init__'))
+                warn(
+                    _rcparam_warn_str.format(
+                        key=repr(k), value=repr(v), func="__init__"
+                    )
+                )
                 dict.__setitem__(self, k, v)
 
     def __setitem__(self, key, val):
         key, val = self._get_depreceated(key, val)
         if key is None:
             return
         try:
@@ -467,16 +478,17 @@
             return key, alt_val(args[0]) if args else None
         elif key in self._deprecated_ignore_map:
             alt = self._deprecated_ignore_map[key]
             warn(self.msg_depr_ignore % (key, alt))
             return None, None
         elif key not in self.defaultParams:
             raise KeyError(
-                '%s is not a valid rc parameter. See rcParams.keys() for a '
-                'list of valid parameters.' % (key,))
+                "%s is not a valid rc parameter. See rcParams.keys() for a "
+                "list of valid parameters." % (key,)
+            )
         return key, args[0] if args else None
 
     def __getitem__(self, key):
         key = self._get_depreceated(key)[0]
         if key is not None:
             return dict.__getitem__(self, key)
 
@@ -528,46 +540,56 @@
     # through __setitem__
     def update(self, *args, **kwargs):
         for k, v in six.iteritems(dict(*args, **kwargs)):
             try:
                 self[k] = v
             except (ValueError, RuntimeError):
                 # force the issue
-                warn(_rcparam_warn_str.format(key=repr(k), value=repr(v),
-                                              func='update'))
+                warn(
+                    _rcparam_warn_str.format(
+                        key=repr(k), value=repr(v), func="update"
+                    )
+                )
                 dict.__setitem__(self, k, v)
 
-    def update_from_defaultParams(self, defaultParams=None,
-                                  plotters=True):
+    def update_from_defaultParams(self, defaultParams=None, plotters=True):
         """Update from the a dictionary like the :attr:`defaultParams`
 
         Parameters
         ----------
         defaultParams: dict
             The :attr:`defaultParams` like dictionary. If None, the
             :attr:`defaultParams` attribute will be updated
         plotters: bool
             If True, ``'project.plotters'`` will be updated too"""
         if defaultParams is None:
             defaultParams = self.defaultParams
-        self.update({key: val[0] for key, val in defaultParams.items()
-                     if plotters or key != 'project.plotters'})
+        self.update(
+            {
+                key: val[0]
+                for key, val in defaultParams.items()
+                if plotters or key != "project.plotters"
+            }
+        )
 
     def __repr__(self):
         import pprint
+
         class_name = self.__class__.__name__
         indent = len(class_name) + 1
-        repr_split = pprint.pformat(dict(self), indent=1,
-                                    width=80 - indent).split('\n')
-        repr_indented = ('\n' + ' ' * indent).join(repr_split)
-        return '{0}({1})'.format(class_name, repr_indented)
+        repr_split = pprint.pformat(
+            dict(self), indent=1, width=80 - indent
+        ).split("\n")
+        repr_indented = ("\n" + " " * indent).join(repr_split)
+        return "{0}({1})".format(class_name, repr_indented)
 
     def __str__(self):
-        return '\n'.join('{0}: {1}'.format(k, v)
-                         for k, v in sorted(self.items()))
+        return "\n".join(
+            "{0}: {1}".format(k, v) for k, v in sorted(self.items())
+        )
 
     def keys(self):
         """
         Return sorted list of keys.
         """
         k = list(dict.keys(self))
         k.sort()
@@ -602,16 +624,19 @@
 
         See Also
         --------
         find_and_replace"""
         pattern_re = re.compile(pattern)
         ret = RcParams()
         ret.defaultParams = self.defaultParams
-        ret.update((key, value) for key, value in self.items()
-                   if pattern_re.search(key))
+        ret.update(
+            (key, value)
+            for key, value in self.items()
+            if pattern_re.search(key)
+        )
         return ret
 
     @docstrings.dedent
     def find_and_replace(self, *args, **kwargs):
         """
         Like :meth:`find_all` but the given strings are replaced
 
@@ -668,21 +693,29 @@
         --------
         dump_to_file, psyplot_fname"""
         fname = fname or psyplot_fname()
         if fname and os.path.exists(fname):
             with open(fname) as f:
                 d = yaml.load(f, Loader=yaml.SafeLoader)
                 self.update(d)
-                if (d.get('project.plotters.user') and
-                        'project.plotters' in self):
-                    self['project.plotters'].update(d['project.plotters.user'])
-
-    def dump(self, fname=None, overwrite=True, include_keys=None,
-             exclude_keys=['project.plotters'], include_descriptions=True,
-             **kwargs):
+                if (
+                    d.get("project.plotters.user")
+                    and "project.plotters" in self
+                ):
+                    self["project.plotters"].update(d["project.plotters.user"])
+
+    def dump(
+        self,
+        fname=None,
+        overwrite=True,
+        include_keys=None,
+        exclude_keys=["project.plotters"],
+        include_descriptions=True,
+        **kwargs,
+    ):
         """Dump this instance to a yaml file
 
         Parameters
         ----------
         fname: str or None
             file name to write to. If None, the string that would be written
             to a file is returned
@@ -711,91 +744,97 @@
             If `fname` already exists and `overwrite` is False
 
         See Also
         --------
         load_from_file"""
         if fname is not None and not overwrite and os.path.exists(fname):
             raise IOError(
-                '%s already exists! Set overwrite=True to overwrite it!' % (
-                    fname))
+                "%s already exists! Set overwrite=True to overwrite it!"
+                % (fname)
+            )
         if six.PY2:
-            kwargs.setdefault('encoding', 'utf-8')
-        d = {key: val for key, val in six.iteritems(self) if (
-                include_keys is None or key in include_keys) and
-             key not in exclude_keys}
-        kwargs['default_flow_style'] = False
+            kwargs.setdefault("encoding", "utf-8")
+        d = {
+            key: val
+            for key, val in six.iteritems(self)
+            if (include_keys is None or key in include_keys)
+            and key not in exclude_keys
+        }
+        kwargs["default_flow_style"] = False
         if include_descriptions:
             s = yaml.dump(d, **kwargs)
             desc = self.descriptions
             i = 2
-            header = self.HEADER.splitlines() + [
-                '', 'Created with python', ''] + sys.version.splitlines() + [
-                    '', '']
-            lines = ['# ' + l for l in header] + s.splitlines()
-            for l in lines[2:]:
-                key = l.split(':')[0]
+            header = (
+                self.HEADER.splitlines()
+                + ["", "Created with python", ""]
+                + sys.version.splitlines()
+                + ["", ""]
+            )
+            lines = ["# " + line for line in header] + s.splitlines()
+            for line in lines[2:]:
+                key = line.split(":")[0]
                 if key in desc:
-                    lines.insert(i, '# ' + '\n# '.join(desc[key].splitlines()))
+                    lines.insert(i, "# " + "\n# ".join(desc[key].splitlines()))
                     i += 1
                 i += 1
-            s = '\n'.join(lines)
+            s = "\n".join(lines)
             if fname is None:
                 return s
             else:
-                with open(fname, 'w') as f:
+                with open(fname, "w") as f:
                     f.write(s)
         else:
             if fname is None:
                 return yaml.dump(d, **kwargs)
-            with open(fname, 'w') as f:
+            with open(fname, "w") as f:
                 yaml.dump(d, f, **kwargs)
         return None
 
     def _load_plugin_entrypoints(self):
         """Load the modules for the psyplot plugins
 
         Yields
         ------
         importlib.metadata.EntryPoint
             The entry point for the psyplot plugin module"""
         from psyplot.utils import plugin_entrypoints
 
         def load_plugin(ep):
-
             try:
                 ep.module
             except AttributeError:  # python<3.10
                 try:
                     ep.module = ep.pattern.match(ep.value).group("module")
-                except AttributeError: # python<3.8
+                except AttributeError:  # python<3.8
                     ep.module = ep.module_name
 
-            if plugins_env == ['no']:
+            if plugins_env == ["no"]:
                 return False
             elif ep.module in exclude_plugins:
                 return False
             elif include_plugins and ep.module not in include_plugins:
                 return False
             return True
 
         self._plugins = self._plugins or []
 
-        plugins_env = os.getenv('PSYPLOT_PLUGINS', '').split('::')
-        include_plugins = [s[4:] for s in plugins_env if s.startswith('yes:')]
-        exclude_plugins = [s[3:] for s in plugins_env if s.startswith('no:')]
+        plugins_env = os.getenv("PSYPLOT_PLUGINS", "").split("::")
+        include_plugins = [s[4:] for s in plugins_env if s.startswith("yes:")]
+        exclude_plugins = [s[3:] for s in plugins_env if s.startswith("no:")]
 
         logger = logging.getLogger(__name__)
 
         eps = plugin_entrypoints("psyplot", "plugin")
         for ep in eps:
             if not load_plugin(ep):
-                logger.debug('Skipping entrypoint %s', ep)
+                logger.debug("Skipping entrypoint %s", ep)
                 continue
             self._plugins.append(str(ep))
-            logger.debug('Loading entrypoint %s', ep)
+            logger.debug("Loading entrypoint %s", ep)
             yield ep
 
     def load_plugins(self, raise_error=False):
         """
         Load the plotters and defaultParams from the plugins
 
         This method loads the `plotters` attribute and `defaultParams`
@@ -805,91 +844,116 @@
 
         Parameters
         ----------
         raise_error: bool
             If True, an error is raised when multiple plugins define the same
             plotter or rcParams key. Otherwise only a warning is raised"""
 
-        pm_env = os.getenv('PSYPLOT_PLOTMETHODS', '').split('::')
-        include_pms = [s[4:] for s in pm_env if s.startswith('yes:')]
-        exclude_pms = [s[3:] for s in pm_env if s.startswith('no:')]
+        pm_env = os.getenv("PSYPLOT_PLOTMETHODS", "").split("::")
+        include_pms = [s[4:] for s in pm_env if s.startswith("yes:")]
+        exclude_pms = [s[3:] for s in pm_env if s.startswith("no:")]
 
         logger = logging.getLogger(__name__)
 
-        plotters = self['project.plotters']
-        def_plots = {'default': list(plotters)}
+        plotters = self["project.plotters"]
+        def_plots = {"default": list(plotters)}
         defaultParams = self.defaultParams
-        def_keys = {'default': defaultParams}
+        def_keys = {"default": defaultParams}
 
         def register_pm(ep, name):
-            full_name = '%s:%s' % (ep.module, name)
+            full_name = "%s:%s" % (ep.module, name)
             ret = True
-            if pm_env == ['no']:
+            if pm_env == ["no"]:
                 ret = False
             elif name in exclude_pms or full_name in exclude_pms:
                 ret = False
-            elif include_pms and (name not in include_pms and
-                                  full_name not in include_pms):
+            elif include_pms and (
+                name not in include_pms and full_name not in include_pms
+            ):
                 ret = False
             if not ret:
-                logger.debug('Skipping plot method %s', full_name)
+                logger.debug("Skipping plot method %s", full_name)
             return ret
 
         for ep in self._load_plugin_entrypoints():
             try:
                 plugin_mod = ep.load()
             except (ModuleNotFoundError, ImportError):
-                logger.debug("Failed to import %s!" % (ep, ), exc_info=True)
-                logger.warning("Failed to import %s!" % (ep, ))
+                logger.debug("Failed to import %s!" % (ep,), exc_info=True)
+                logger.warning("Failed to import %s!" % (ep,))
                 continue
             rc = plugin_mod.rcParams
 
             # load the plotters
             plugin_plotters = {
-                key: val for key, val in rc.get('project.plotters', {}).items()
-                if register_pm(ep, key)}
+                key: val
+                for key, val in rc.get("project.plotters", {}).items()
+                if register_pm(ep, key)
+            }
             already_defined = set(plotters).intersection(plugin_plotters)
             if already_defined:
-                msg = ("Error while loading psyplot plugin %s! The "
-                       "following plotters have already been "
-                       "defined") % ep
-                msg += 'and will be overwritten:' if not raise_error else ':'
-                msg += '\n' + '\n'.join(chain.from_iterable(
-                    (('%s by %s' % (key, plugin)
-                      for plugin, keys in def_plots.items() if key in keys)
-                     for key in already_defined)))
+                msg = (
+                    "Error while loading psyplot plugin %s! The "
+                    "following plotters have already been "
+                    "defined"
+                ) % ep
+                msg += "and will be overwritten:" if not raise_error else ":"
+                msg += "\n" + "\n".join(
+                    chain.from_iterable(
+                        (
+                            (
+                                "%s by %s" % (key, plugin)
+                                for plugin, keys in def_plots.items()
+                                if key in keys
+                            )
+                            for key in already_defined
+                        )
+                    )
+                )
                 if raise_error:
                     raise ImportError(msg)
                 else:
                     warn(msg)
             for d in plugin_plotters.values():
-                d['plugin'] = ep.module
+                d["plugin"] = ep.module
             plotters.update(plugin_plotters)
             def_plots[ep] = list(plugin_plotters)
 
             # load the defaultParams keys
             plugin_defaultParams = rc.defaultParams
             already_defined = set(defaultParams).intersection(
-                plugin_defaultParams) - {'project.plotters'}
+                plugin_defaultParams
+            ) - {"project.plotters"}
             if already_defined:
-                msg = ("Error while loading psyplot plugin %s! The "
-                       "following default keys have already been "
-                       "defined:") % ep
-                msg += '\n' + '\n'.join(chain.from_iterable(
-                    (('%s by %s' % (key, plugin)
-                      for plugin, keys in def_keys.items() if key in keys)
-                     for key in already_defined)))
+                msg = (
+                    "Error while loading psyplot plugin %s! The "
+                    "following default keys have already been "
+                    "defined:"
+                ) % ep
+                msg += "\n" + "\n".join(
+                    chain.from_iterable(
+                        (
+                            (
+                                "%s by %s" % (key, plugin)
+                                for plugin, keys in def_keys.items()
+                                if key in keys
+                            )
+                            for key in already_defined
+                        )
+                    )
+                )
                 if raise_error:
                     raise ImportError(msg)
                 else:
                     warn(msg)
-            update_keys = set(plugin_defaultParams) - {'project.plotters'}
+            update_keys = set(plugin_defaultParams) - {"project.plotters"}
             def_keys[ep] = update_keys
             self.defaultParams.update(
-                {key: plugin_defaultParams[key] for key in update_keys})
+                {key: plugin_defaultParams[key] for key in update_keys}
+            )
 
             # load the rcParams (without validation)
             super(RcParams, self).update({key: rc[key] for key in update_keys})
 
             # add the deprecated keys
             self._deprecated_ignore_map.update(rc._deprecated_ignore_map)
             self._deprecated_map.update(rc._deprecated_map)
@@ -911,16 +975,15 @@
             assert rcParams['some_key'] == 0
         """
         save = dict(self)
         yield
         super().update(save)  # reset settings
 
 
-def psyplot_fname(env_key='PSYPLOTRC', fname='psyplotrc.yml',
-                  if_exists=True):
+def psyplot_fname(env_key="PSYPLOTRC", fname="psyplotrc.yml", if_exists=True):
     """
     Get the location of the config file.
 
     The file location is determined in the following order
 
     - `$PWD/psyplotrc.yml`
 
@@ -956,15 +1019,15 @@
         None, if no file could be found and `if_exists` is True, else the path
         to the psyplot configuration file
 
     Notes
     -----
     This function is motivated by the :func:`matplotlib.matplotlib_fname`
     function"""
-    cwd = getcwd()
+    cwd = os.getcwd()
     full_fname = os.path.join(cwd, fname)
     if os.path.exists(full_fname):
         return full_fname
 
     if env_key in os.environ:
         path = os.environ[env_key]
         if os.path.exists(path):
@@ -980,15 +1043,15 @@
         full_fname = os.path.join(configdir, fname)
         if os.path.exists(full_fname) or not if_exists:
             return full_fname
 
     return None
 
 
-def get_configdir(name='psyplot', env_key='PSYPLOTCONFIGDIR'):
+def get_configdir(name="psyplot", env_key="PSYPLOTCONFIGDIR"):
     """
     Return the string representing the configuration directory.
 
     The directory is chosen as follows:
 
     1. If the `env_key` environment variable is supplied, choose that.
 
@@ -1014,19 +1077,20 @@
     function"""
     configdir = os.environ.get(env_key)
     if configdir is not None:
         return os.path.abspath(configdir)
 
     p = None
     h = _get_home()
-    if ((sys.platform.startswith('linux') or sys.platform == 'darwin') and
-            h is not None):
-        p = os.path.join(h, '.config/' + name)
+    if (
+        sys.platform.startswith("linux") or sys.platform == "darwin"
+    ) and h is not None:
+        p = os.path.join(h, ".config/" + name)
     elif h is not None:
-        p = os.path.join(h, '.' + name)
+        p = os.path.join(h, "." + name)
 
     if not os.path.exists(p):
         os.makedirs(p, exist_ok=True)
     return p
 
 
 def validate_path_exists(s):
@@ -1035,18 +1099,17 @@
         return None
     if os.path.exists(s):
         return s
     else:
         raise ValueError('"%s" should be a path but it does not exist' % s)
 
 
-def validate_files_exist(l):
+def validate_files_exist(files):
     """Validate if all pathnames in a given list exists"""
-    return [validate_str(s) and validate_path_exists(s)
-            for s in l]
+    return [validate_str(fn) and validate_path_exists(fn) for fn in files]
 
 
 def validate_dict(d):
     """Validate a dictionary
 
     Parameters
     ----------
@@ -1068,29 +1131,29 @@
             with open(d) as f:
                 return dict(yaml.load(f, Loader=yaml.SafeLoader))
         except Exception:
             raise ValueError("Could not convert {} to dictionary!".format(d))
 
 
 def validate_bool_maybe_none(b):
-    'Convert b to a boolean or raise'
+    "Convert b to a boolean or raise"
     if isinstance(b, six.string_types):
         b = b.lower()
-    if b is None or b == 'none':
+    if b is None or b == "none":
         return None
     return validate_bool(b)
 
 
 def validate_bool(b):
     """Convert b to a boolean or raise"""
     if isinstance(b, six.string_types):
         b = b.lower()
-    if b in ('t', 'y', 'yes', 'on', 'true', '1', 1, True):
+    if b in ("t", "y", "yes", "on", "true", "1", 1, True):
         return True
-    elif b in ('f', 'n', 'no', 'off', 'false', '0', 0, False):
+    elif b in ("f", "n", "no", "off", "false", "0", 0, False):
         return False
     else:
         raise ValueError('Could not convert "%s" to boolean' % b)
 
 
 def validate_str(s):
     """Validate a string
@@ -1123,15 +1186,15 @@
     list
         list of str
 
     Raises
     ------
     ValueError"""
     if isinstance(s, six.string_types):
-        return [six.text_type(v.strip()) for v in s.split(',') if v.strip()]
+        return [six.text_type(v.strip()) for v in s.split(",") if v.strip()]
     else:
         try:
             return list(map(validate_str, s))
         except TypeError as e:
             raise ValueError(e.message)
 
 
@@ -1152,103 +1215,144 @@
     ValueError"""
     return set(validate_stringlist(*args, **kwargs))
 
 
 #: :class:`dict` with default values and validation functions
 defaultParams = {
     # user defined plotter keys
-    'plotter.user': [
-        {}, validate_dict,
-        inspect.cleandoc("""
+    "plotter.user": [
+        {},
+        validate_dict,
+        inspect.cleandoc(
+            """
         formatoption keys and values that are defined by the user to be used by
         the specified plotters. For example to modify the title of all
         :class:`psyplot.plotter.maps.FieldPlotter` instances, set
-        ``{'plotter.fieldplotter.title': 'my title'}``""")],
-
-    'gridweights.use_cdo': [
-        None, validate_bool_maybe_none,
-        'Boolean flag to control whether CDOs (Climate Data Operators) should '
-        'be used to calculate grid weights. If None, they are tried to be '
-        'used.'],
-
+        ``{'plotter.fieldplotter.title': 'my title'}``"""
+        ),
+    ],
+    "gridweights.use_cdo": [
+        None,
+        validate_bool_maybe_none,
+        "Boolean flag to control whether CDOs (Climate Data Operators) should "
+        "be used to calculate grid weights. If None, they are tried to be "
+        "used.",
+    ],
     # decoder
-    'decoder.x': [set(), validate_stringset,
-                  'names that shall be interpreted as the longitudinal x dim'],
-    'decoder.y': [set(), validate_stringset,
-                  'names that shall be interpreted as the latitudinal y dim'],
-    'decoder.z': [set(), validate_stringset,
-                  'names that shall be interpreted as the vertical z dim'],
-    'decoder.t': [{'time'}, validate_stringset,
-                  'names that shall be interpreted as the time dimension'],
-    'decoder.interp_kind': [
-        'linear', validate_str,
-        'interpolation method to calculate 2D-bounds (see the `kind` parameter'
-        'in the :meth:`psyplot.data.CFDecoder.get_plotbounds` method)'],
-
+    "decoder.x": [
+        set(),
+        validate_stringset,
+        "names that shall be interpreted as the longitudinal x dim",
+    ],
+    "decoder.y": [
+        set(),
+        validate_stringset,
+        "names that shall be interpreted as the latitudinal y dim",
+    ],
+    "decoder.z": [
+        set(),
+        validate_stringset,
+        "names that shall be interpreted as the vertical z dim",
+    ],
+    "decoder.t": [
+        {"time"},
+        validate_stringset,
+        "names that shall be interpreted as the time dimension",
+    ],
+    "decoder.interp_kind": [
+        "linear",
+        validate_str,
+        "interpolation method to calculate 2D-bounds (see the `kind` parameter"
+        "in the :meth:`psyplot.data.CFDecoder.get_plotbounds` method)",
+    ],
     # specify automatic drawing and showing of figures
-    'auto_draw': [True, validate_bool,
-                  ('Automatically draw the figures if the draw keyword in the '
-                   'update and start_update methods is None')],
-    'auto_show': [False, validate_bool,
-                  ('Automatically show the figures after the update and'
-                   'start_update methods')],
-
+    "auto_draw": [
+        True,
+        validate_bool,
+        (
+            "Automatically draw the figures if the draw keyword in the "
+            "update and start_update methods is None"
+        ),
+    ],
+    "auto_show": [
+        False,
+        validate_bool,
+        (
+            "Automatically show the figures after the update and"
+            "start_update methods"
+        ),
+    ],
     # data
-    'datapath': [None, validate_path_exists, 'path for supplementary data'],
-
+    "datapath": [None, validate_path_exists, "path for supplementary data"],
     # list settings
-    'lists.auto_update': [True, validate_bool,
-                          'default value (boolean) for the auto_update '
-                          'parameter in the initialization of Plotter, '
-                          'Project, etc. instances'],
-
+    "lists.auto_update": [
+        True,
+        validate_bool,
+        "default value (boolean) for the auto_update "
+        "parameter in the initialization of Plotter, "
+        "Project, etc. instances",
+    ],
     # project settings
     # auto_import: If True the plotters in project,plotters are automatically
     # imported
-    'project.auto_import': [False, validate_bool,
-                            'boolean controlling whether all plotters '
-                            'specified in the project.plotters item will be '
-                            'automatically imported when importing the '
-                            'psyplot.project module'],
-    'project.import_seaborn': [
-        None, validate_bool_maybe_none,
-        'boolean controlling whether the seaborn module shall be imported '
-        'when importing the project module. If None, it is only tried to '
-        'import the module.'],
-    'project.plotters': [
-        {}, validate_dict,
-        'mapping from identifier to plotter definitions for the Project class.'
-        ' See the :func:`psyplot.project.register_plotter` function for '
-        'possible keywords and values. See '
-        ':attr:`psyplot.project.registered_plotters` for examples.'],
-
-    'project.plotters.user': [
-        {}, validate_dict,
+    "project.auto_import": [
+        False,
+        validate_bool,
+        "boolean controlling whether all plotters "
+        "specified in the project.plotters item will be "
+        "automatically imported when importing the "
+        "psyplot.project module",
+    ],
+    "project.import_seaborn": [
+        None,
+        validate_bool_maybe_none,
+        "boolean controlling whether the seaborn module shall be imported "
+        "when importing the project module. If None, it is only tried to "
+        "import the module.",
+    ],
+    "project.plotters": [
+        {},
+        validate_dict,
+        "mapping from identifier to plotter definitions for the Project class."
+        " See the :func:`psyplot.project.register_plotter` function for "
+        "possible keywords and values. See "
+        ":attr:`psyplot.project.registered_plotters` for examples.",
+    ],
+    "project.plotters.user": [
+        {},
+        validate_dict,
         "Plot methods that are defined by the user and overwrite those in the"
         "``'project.plotters'`` key. Use this if you want to define your own "
-        "plotters without writing a plugin"],
-
+        "plotters without writing a plugin",
+    ],
     # presets
-    'presets.trusted': [
-        [], validate_files_exist,
-        "A list of filenames with trusted presets"]
-    }
-
-
-_rcparam_warn_str = ("Trying to set {key} to {value} via the {func} "
-                     "method of RcParams which does not validate cleanly. ")
-
-
-_seq_err_msg = ('You must supply exactly {n:d} values, you provided '
-                '{num:d} values: {s}')
-
-
-_str_err_msg = ('You must supply exactly {n:d} comma-separated values, '
-                'you provided '
-                '{num:d} comma-separated values: {s}')
+    "presets.trusted": [
+        [],
+        validate_files_exist,
+        "A list of filenames with trusted presets",
+    ],
+}
+
+
+_rcparam_warn_str = (
+    "Trying to set {key} to {value} via the {func} "
+    "method of RcParams which does not validate cleanly. "
+)
+
+
+_seq_err_msg = (
+    "You must supply exactly {n:d} values, you provided " "{num:d} values: {s}"
+)
+
+
+_str_err_msg = (
+    "You must supply exactly {n:d} comma-separated values, "
+    "you provided "
+    "{num:d} comma-separated values: {s}"
+)
 
 #: :class:`~psyplot.config.rcsetup.RcParams` instance that stores default
 #: formatoptions and configuration settings.
 rcParams = RcParams()
 rcParams.update_from_defaultParams()
 
 defaultParams_orig = defaultParams.copy()
```

### Comparing `psyplot-1.4.3/psyplot/data.py` & `psyplot-1.5.0/psyplot/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,52 @@
 """Data management core routines of psyplot."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from __future__ import division
+
+import datetime as dt
+import inspect
+import io
+import logging
 import os
 import os.path as osp
-import inspect
-from threading import Thread
+import re
+import traceback as tb
+from collections import defaultdict
 from functools import partial
 from glob import glob
 from importlib import import_module
-import re
+from itertools import chain, count, cycle, islice, product, repeat, starmap
+from queue import Queue
+from threading import Thread
+from typing import Dict, List, Optional
+
+import numpy as np
 import six
-from collections import defaultdict
-from itertools import chain, product, repeat, starmap, count, cycle, islice
 import xarray as xr
-from xarray.core.utils import NDArrayMixin
-from xarray.core.formatting import first_n_items, format_item
-
 import xarray.backends.api as xarray_api
 from pandas import to_datetime
-import numpy as np
-import datetime as dt
-import logging
+from xarray.core.formatting import first_n_items, format_item
+from xarray.core.utils import NDArrayMixin
+
+import psyplot.utils as utils
 from psyplot.config.rcsetup import rcParams, safe_list
 from psyplot.docstring import dedent, docstrings
-from psyplot.compat.pycompat import (
-    zip, map, isstring, OrderedDict, filter, range, getcwd,
-    Queue)
-from psyplot.warning import PsyPlotRuntimeWarning
-from warnings import warn
-import psyplot.utils as utils
+from psyplot.utils import isstring
+from psyplot.warning import PsyPlotRuntimeWarning, warn
 
 try:
-    import dask
+    import dask  # noqa: F401
+
     with_dask = True
 except ImportError:
     with_dask = False
 
 try:
     import xarray.backends.plugins as xr_plugins
 except ImportError:
@@ -66,23 +54,23 @@
 
 
 # No data variable. This is used for filtering if an attribute could not have
 # been accessed
 _NODATA = object
 
 
-VARIABLELABEL = 'variable'
+VARIABLELABEL = "variable"
 
 
 logger = logging.getLogger(__name__)
 
 
 _ds_counter = count(1)
 
-xr_version = tuple(map(int, xr.__version__.split('.')[:2]))
+xr_version = tuple(map(int, xr.__version__.split(".")[:2]))
 
 
 def _no_auto_update_getter(self):
     """:class:`bool`. Boolean controlling whether the :meth:`start_update`
     method is automatically called by the :meth:`update` method
 
 
@@ -95,15 +83,15 @@
         ...     data.start_update()
 
     To permanently disable the automatic update, simply set
 
         >>> data.no_auto_update = True
         >>> data.update(time=1)
         >>> data.no_auto_update = False  # reenable automatical update"""
-    if getattr(self, '_no_auto_update', None) is not None:
+    if getattr(self, "_no_auto_update", None) is not None:
         return self._no_auto_update
     else:
         self._no_auto_update = utils._TempBool()
     return self._no_auto_update
 
 
 def _infer_interval_breaks(coord):
@@ -144,15 +132,15 @@
     # xarray 0.16 fails with pandas 1.1.0 for datetime, see
     # https://github.com/pydata/xarray/issues/4283
     for key, val in dims.items():
         if np.issubdtype(np.asarray(val).dtype, np.datetime64):
             dims[key] = to_datetime([val])[0]
 
 
-@docstrings.get_sections(base='setup_coords')
+@docstrings.get_sections(base="setup_coords")
 @dedent
 def setup_coords(arr_names=None, sort=[], dims={}, **kwargs):
     """
     Sets up the arr_names dictionary for the plot
 
     Parameters
     ----------
@@ -162,20 +150,20 @@
 
         - if string: same as list of strings (see below). Strings may
           include {0} which will be replaced by a counter.
         - list of strings: those will be used for the array names. The final
           number of dictionaries in the return depend in this case on the
           `dims` and ``**furtherdims``
         - dictionary:
-          Then nothing happens and an :class:`OrderedDict` version of
+          Then nothing happens and an :class:`dict` version of
           `arr_names` is returned.
     sort: list of strings
         This parameter defines how the dictionaries are ordered. It has no
         effect if `arr_names` is a dictionary (use a
-        :class:`~collections.OrderedDict` for that). It can be a list of
+        :class:`dict` for that). It can be a list of
         dimension strings matching to the dimensions in `dims` for the
         variable.
     dims: dict
         Keys must be variable names of dimensions (e.g. time, level, lat or
         lon) or 'name' for the variable name you want to choose.
         Values must be values of that dimension or iterables of the values
         (e.g. lists). Note that strings will be put into a list.
@@ -184,51 +172,54 @@
         will result in two plots, one for the first (time == 0) and one for the
         second (time == 1) time step.
     ``**kwargs``
         The same as `dims` (those will update what is specified in `dims`)
 
     Returns
     -------
-    ~collections.OrderedDict
+    dict
         A mapping from the keys in `arr_names` and to dictionaries. Each
         dictionary corresponds defines the coordinates of one data array to
         load"""
     try:
-        return OrderedDict(arr_names)
+        return dict(arr_names)
     except (ValueError, TypeError):
-        # ValueError for cyordereddict, TypeError for collections.OrderedDict
+        # ValueError for cydict, TypeError for dic
         pass
     if arr_names is None:
-        arr_names = repeat('arr{0}')
+        arr_names = repeat("arr{0}")
     elif isstring(arr_names):
         arr_names = repeat(arr_names)
-    dims = OrderedDict(dims)
+    dims = dict(dims)
     for key, val in six.iteritems(kwargs):
         dims.setdefault(key, val)
-    sorted_dims = OrderedDict()
+    sorted_dims = dict()
     if sort:
         for key in sort:
             sorted_dims[key] = dims.pop(key)
         for key, val in six.iteritems(dims):
             sorted_dims[key] = val
     else:
         # make sure, it is first sorted for the variable names
-        if 'name' in dims:
-            sorted_dims['name'] = None
+        if "name" in dims:
+            sorted_dims["name"] = None
         for key, val in sorted(dims.items()):
             sorted_dims[key] = val
         for key, val in six.iteritems(kwargs):
             sorted_dims.setdefault(key, val)
     for key, val in six.iteritems(sorted_dims):
         sorted_dims[key] = iter(safe_list(val))
-    return OrderedDict([
-        (arr_name.format(i), dict(zip(sorted_dims.keys(), dim_tuple)))
-        for i, (arr_name, dim_tuple) in enumerate(zip(
-            arr_names, product(
-                *map(list, sorted_dims.values()))))])
+    return dict(
+        [
+            (arr_name.format(i), dict(zip(sorted_dims.keys(), dim_tuple)))
+            for i, (arr_name, dim_tuple) in enumerate(
+                zip(arr_names, product(*map(list, sorted_dims.values())))
+            )
+        ]
+    )
 
 
 def to_slice(arr):
     """Test whether `arr` is an integer array that can be replaced by a slice
 
     Parameters
     ----------
@@ -274,33 +265,37 @@
         `base_index`
     """
     try:
         values = coord.values
     except AttributeError:
         values = coord
     if values.ndim == 0:
-        return base_index.get_loc(values[()])
+        try:
+            return base_index.get_loc(values[()])
+        except KeyError:
+            # the location does not exactly match, so we try a nearest match
+            return base_index.get_indexer([values[()]], "nearest")[0]
     if len(values) == len(base_index) and (values == base_index).all():
         return slice(None)
     values = np.array(list(map(lambda i: base_index.get_loc(i), values)))
     return to_slice(values) or values
 
 
 #: mapping that translates datetime format strings to regex patterns
 t_patterns = {
-        '%Y': '[0-9]{4}',
-        '%m': '[0-9]{1,2}',
-        '%d': '[0-9]{1,2}',
-        '%H': '[0-9]{1,2}',
-        '%M': '[0-9]{1,2}',
-        '%S': '[0-9]{1,2}',
-    }
+    "%Y": "[0-9]{4}",
+    "%m": "[0-9]{1,2}",
+    "%d": "[0-9]{1,2}",
+    "%H": "[0-9]{1,2}",
+    "%M": "[0-9]{1,2}",
+    "%S": "[0-9]{1,2}",
+}
 
 
-@docstrings.get_sections(base='get_tdata')
+@docstrings.get_sections(base="get_tdata")
 @dedent
 def get_tdata(t_format, files):
     """
     Get the time information from file names
 
     Parameters
     ----------
@@ -318,35 +313,49 @@
         The time coordinate
     list of str
         The file names as they are sorten in the returned index
 
     References
     ----------
     .. [1] https://docs.python.org/2/library/datetime.html"""
+
     def median(arr):
-        return arr.min() + (arr.max() - arr.min())/2
+        return arr.min() + (arr.max() - arr.min()) / 2
+
     import re
+
     from pandas import Index
+
     t_pattern = t_format
     for fmt, patt in t_patterns.items():
         t_pattern = t_pattern.replace(fmt, patt)
     t_pattern = re.compile(t_pattern)
     time = list(range(len(files)))
     for i, f in enumerate(files):
-        time[i] = median(np.array(list(map(
-            lambda s: np.datetime64(dt.datetime.strptime(s, t_format)),
-            t_pattern.findall(f)))))
+        time[i] = median(
+            np.array(
+                list(
+                    map(
+                        lambda s: np.datetime64(
+                            dt.datetime.strptime(s, t_format)
+                        ),
+                        t_pattern.findall(f),
+                    )
+                )
+            )
+        )
     ind = np.argsort(time)  # sort according to time
     files = np.array(files)[ind]
     time = np.array(time)[ind]
-    return to_datetime(Index(time, name='time')), files
+    return to_datetime(Index(time, name="time")), files
 
 
-docstrings.get_sections(xr.Dataset.to_netcdf.__doc__,
-                        'xarray.Dataset.to_netcdf')
+docstrings.get_sections(
+    xr.Dataset.to_netcdf.__doc__, "xarray.Dataset.to_netcdf"
+)
 
 
 @docstrings.dedent
 def to_netcdf(ds, *args, **kwargs):
     """
     Store the given dataset as a netCDF file
 
@@ -358,30 +367,34 @@
     ----------
     ds: xarray.Dataset
         The dataset to store
     %(xarray.Dataset.to_netcdf.parameters)s
     """
     to_update = {}
     for v, obj in six.iteritems(ds.variables):
-        units = obj.attrs.get('units', obj.encoding.get('units', None))
-        if units == 'day as %Y%m%d.%f' and np.issubdtype(
-                obj.dtype, np.datetime64):
+        units = obj.attrs.get("units", obj.encoding.get("units", None))
+        if units == "day as %Y%m%d.%f" and np.issubdtype(
+            obj.dtype, np.datetime64
+        ):
             to_update[v] = xr.Variable(
-                obj.dims, AbsoluteTimeEncoder(obj), attrs=obj.attrs.copy(),
-                encoding=obj.encoding)
-            to_update[v].attrs['units'] = units
+                obj.dims,
+                AbsoluteTimeEncoder(obj),
+                attrs=obj.attrs.copy(),
+                encoding=obj.encoding,
+            )
+            to_update[v].attrs["units"] = units
     if to_update:
         ds = ds.copy()
         ds.update(to_update)
     return xarray_api.to_netcdf(ds, *args, **kwargs)
 
 
 def _get_fname_netCDF4(store):
     """Try to get the file name from the NetCDF4DataStore store"""
-    return getattr(store, '_filename', None)
+    return getattr(store, "_filename", None)
 
 
 def _get_fname_scipy(store):
     """Try to get the file name from the ScipyDataStore store"""
     try:
         return store.ds.filename
     except AttributeError:
@@ -416,19 +429,20 @@
         self._connections = []
 
     def connect(self, func):
         if func not in self._connections:
             self._connections.append(func)
 
     def emit(self, *args, **kwargs):
-        if (not getattr(self.owner, 'block_signals', False) and
-                not getattr(self.instance, 'block_signals', False)):
-            logger.debug('Emitting signal %s', self.name)
+        if not getattr(self.owner, "block_signals", False) and not getattr(
+            self.instance, "block_signals", False
+        ):
+            logger.debug("Emitting signal %s", self.name)
             for func in self._connections[:]:
-                logger.debug('Calling %s', func)
+                logger.debug("Calling %s", func)
                 func(*args, **kwargs)
 
     def disconnect(self, func=None):
         """Disconnect a function call to the signal. If None, all connections
         are disconnected"""
         if func is None:
             self._connections = []
@@ -447,15 +461,15 @@
         return ret
 
 
 #: functions to use to extract the file name from a data store
 get_fname_funcs = [_get_fname_netCDF4, _get_fname_scipy, _get_fname_nio]
 
 
-@docstrings.get_sections(base='get_filename_ds')
+@docstrings.get_sections(base="get_filename_ds")
 @docstrings.dedent
 def get_filename_ds(ds, dump=True, paths=None, **kwargs):
     """
     Return the filename of the corresponding to a dataset
 
     This method returns the path to the `ds` or saves the dataset
     if there exists no filename
@@ -498,79 +512,44 @@
     if ds.psy._filename is not None:
         return tuple([ds.psy._filename] + list(ds.psy.data_store))
 
     def dump_nc():
         # make sure that the data store is not closed by providing a
         # write argument
         if xr_version < (0, 11):
-            kwargs.setdefault('writer', xarray_api.ArrayWriter())
+            kwargs.setdefault("writer", xarray_api.ArrayWriter())
             store = to_netcdf(ds, fname, **kwargs)
         else:
             # `writer` parameter was removed by
             # https://github.com/pydata/xarray/pull/2261
-            kwargs.setdefault('multifile', True)
+            kwargs.setdefault("multifile", True)
             store = to_netcdf(ds, fname, **kwargs)[1]
         store_mod = store.__module__
         store_cls = store.__class__.__name__
         ds._file_obj = store
         return store_mod, store_cls
 
     def tmp_it():
         while True:
-            yield NamedTemporaryFile(suffix='.nc').name
-
-    def _legacy_get_filename_ds(ds):
-        # try to get the filename from the data store of the obj
-        #
-        # Outdated possibility since the backend plugin methodology of
-        # xarray 0.18
-        if store_mod is not None:
-            store = ds._file_obj
-            # try several engines
-            if hasattr(store, 'file_objs'):
-                fname = []
-                store_mod = []
-                store_cls = []
-                for obj in store.file_objs:  # mfdataset
-                    _fname = None
-                    for func in get_fname_funcs:
-                        if _fname is None:
-                            _fname = func(obj)
-                            if _fname is not None:
-                                fname.append(_fname)
-                                store_mod.append(obj.__module__)
-                                store_cls.append(obj.__class__.__name__)
-                fname = tuple(fname)
-                store_mod = tuple(store_mod)
-                store_cls = tuple(store_cls)
-            else:
-                for func in get_fname_funcs:
-                    fname = func(store)
-                    if fname is not None:
-                        break
-
-        return fname, store_mod, store_cls
+            yield NamedTemporaryFile(suffix=".nc").name
 
     fname = None
     if paths is True or (dump and paths is None):
         paths = tmp_it()
     elif paths is not None:
         if isstring(paths):
             paths = iter([paths])
         else:
             paths = iter(paths)
     store_mod, store_cls = ds.psy.data_store
-    if xr_plugins is None:
-        fname, store_mod, store_cls = _legacy_get_filename_ds(ds)
-    elif "source" in ds.encoding:
+    if "source" in ds.encoding:
         fname = ds.encoding["source"]
         store_mod = None
         store_cls = None
 
-
     # check if paths is provided and if yes, save the file
     if fname is None and paths is not None:
         fname = next(paths, None)
         if dump and fname is not None:
             store_mod, store_cls = dump_nc()
 
     ds.psy.filename = fname
@@ -582,35 +561,39 @@
 class CFDecoder(object):
     """
     Class that interpretes the coordinates and attributes accordings to
     cf-conventions"""
 
     _registry = []
 
+    #: True if the data of the CFDecoder supports the extraction of a subset of
+    #: the data based on the indices.
+    supports_spatial_slicing = True
+
     @property
     def logger(self):
         """:class:`logging.Logger` of this instance"""
         try:
             return self._logger
         except AttributeError:
-            name = '%s.%s' % (self.__module__, self.__class__.__name__)
+            name = "%s.%s" % (self.__module__, self.__class__.__name__)
             self._logger = logging.getLogger(name)
-            self.logger.debug('Initializing...')
+            self.logger.debug("Initializing...")
             return self._logger
 
     @logger.setter
     def logger(self, value):
         self._logger = value
 
     def __init__(self, ds=None, x=None, y=None, z=None, t=None):
         self.ds = ds
-        self.x = rcParams['decoder.x'].copy() if x is None else set(x)
-        self.y = rcParams['decoder.y'].copy() if y is None else set(y)
-        self.z = rcParams['decoder.z'].copy() if z is None else set(z)
-        self.t = rcParams['decoder.t'].copy() if t is None else set(t)
+        self.x = rcParams["decoder.x"].copy() if x is None else set(x)
+        self.y = rcParams["decoder.y"].copy() if y is None else set(y)
+        self.z = rcParams["decoder.z"].copy() if z is None else set(z)
+        self.t = rcParams["decoder.t"].copy() if t is None else set(t)
 
     @staticmethod
     def register_decoder(decoder_class, pos=0):
         """Register a new decoder
 
         This function registeres a decoder class to use
 
@@ -620,16 +603,17 @@
             The class inherited from the :class:`CFDecoder`
         pos: int
             The position where to register the decoder (by default: the first
             position"""
         CFDecoder._registry.insert(pos, decoder_class)
 
     @classmethod
-    @docstrings.get_sections(base='CFDecoder.can_decode', sections=['Parameters',
-                                                                'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.can_decode", sections=["Parameters", "Returns"]
+    )
     def can_decode(cls, ds, var):
         """
         Class method to determine whether the object can be decoded by this
         decoder class.
 
         Parameters
         ----------
@@ -648,14 +632,15 @@
         -----
         The default implementation returns True for any argument. Subclass this
         method to be specific on what type of data your decoder can decode
         """
         return True
 
     @classmethod
+    @docstrings.get_sections(base="CFDecoder.get_decoder")
     @docstrings.dedent
     def get_decoder(cls, ds, var, *args, **kwargs):
         """
         Class method to get the right decoder class that can decode the
         given dataset and variable
 
         Parameters
@@ -669,16 +654,17 @@
             `var`"""
         for decoder_cls in cls._registry:
             if decoder_cls.can_decode(ds, var):
                 return decoder_cls(ds, *args, **kwargs)
         return CFDecoder(ds, *args, **kwargs)
 
     @staticmethod
-    @docstrings.get_sections(base='CFDecoder.decode_coords', sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.decode_coords", sections=["Parameters", "Returns"]
+    )
     def decode_coords(ds, gridfile=None):
         """
         Sets the coordinates and bounds in a dataset
 
         This static method sets those coordinates and bounds that are marked
         marked in the netCDF attributes as coordinates in :attr:`ds` (without
         deleting them from the variable attributes because this information is
@@ -692,46 +678,55 @@
             The path to a separate grid file or a xarray.Dataset instance which
             may store the coordinates used in `ds`
 
         Returns
         -------
         xarray.Dataset
             `ds` with additional coordinates"""
+
         def add_attrs(obj):
-            if 'coordinates' in obj.attrs:
-                extra_coords.update(obj.attrs['coordinates'].split())
-                obj.encoding['coordinates'] = obj.attrs.pop('coordinates')
-            if 'grid_mapping' in obj.attrs:
-                extra_coords.add(obj.attrs['grid_mapping'])
-            if 'bounds' in obj.attrs:
-                extra_coords.add(obj.attrs['bounds'])
+            if "coordinates" in obj.attrs:
+                extra_coords.update(obj.attrs["coordinates"].split())
+                obj.encoding["coordinates"] = obj.attrs.pop("coordinates")
+            if "grid_mapping" in obj.attrs:
+                extra_coords.add(obj.attrs["grid_mapping"])
+            if "bounds" in obj.attrs:
+                extra_coords.add(obj.attrs["bounds"])
+
         if gridfile is not None and not isinstance(gridfile, xr.Dataset):
             gridfile = open_dataset(gridfile)
         extra_coords = set(ds.coords)
         for k, v in six.iteritems(ds.variables):
             add_attrs(v)
         add_attrs(ds)
         if gridfile is not None:
-            ds.update({k: v for k, v in six.iteritems(gridfile.variables)
-                       if k in extra_coords})
+            ds.update(
+                {
+                    k: v
+                    for k, v in six.iteritems(gridfile.variables)
+                    if k in extra_coords
+                }
+            )
         if xr_version < (0, 11):
-            ds.set_coords(extra_coords.intersection(ds.variables),
-                          inplace=True)
+            ds.set_coords(
+                extra_coords.intersection(ds.variables), inplace=True
+            )
         else:
             ds._coord_names.update(extra_coords.intersection(ds.variables))
         return ds
 
-    @docstrings.get_sections(base='CFDecoder.is_unstructured', sections=[
-        'Parameters', 'Returns'])
-
-    @docstrings.get_sections(base=
-        'CFDecoder.get_cell_node_coord',
-        sections=['Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.is_unstructured", sections=["Parameters", "Returns"]
+    )
+    @docstrings.get_sections(
+        base="CFDecoder.get_cell_node_coord",
+        sections=["Parameters", "Returns"],
+    )
     @dedent
-    def get_cell_node_coord(self, var, coords=None, axis='x', nans=None):
+    def get_cell_node_coord(self, var, coords=None, axis="x", nans=None):
         """
         Checks whether the bounds in the variable attribute are triangular
 
         Parameters
         ----------
         var: xarray.Variable or xarray.DataArray
             The variable to check
@@ -747,119 +742,144 @@
         Returns
         -------
         xarray.DataArray or None
             the bounds corrdinate (if existent)"""
         if coords is None:
             coords = self.ds.coords
         axis = axis.lower()
-        get_coord = self.get_x if axis == 'x' else self.get_y
+        get_coord = self.get_x if axis == "x" else self.get_y
         coord = get_coord(var, coords=coords)
         if coord is not None:
-            bounds = self._get_coord_cell_node_coord(coord, coords, nans,
-                                                     var=var)
+            bounds = self._get_coord_cell_node_coord(
+                coord, coords, nans, var=var
+            )
             if bounds is None:
                 bounds = self.get_plotbounds(coord)
                 if bounds.ndim == 1:
                     dim0 = coord.dims[-1]
                     bounds = xr.DataArray(
                         np.dstack([bounds[:-1], bounds[1:]])[0],
-                        dims=(dim0, '_bnds'),  attrs=coord.attrs.copy(),
-                        name=coord.name + '_bnds')
+                        dims=(dim0, "_bnds"),
+                        attrs=coord.attrs.copy(),
+                        name=coord.name + "_bnds",
+                    )
                 elif bounds.ndim == 2:
                     warn("2D bounds are not yet sufficiently tested!")
                     bounds = xr.DataArray(
-                        np.dstack([bounds[1:, 1:].ravel(),
-                                   bounds[1:, :-1].ravel(),
-                                   bounds[:-1, :-1].ravel(),
-                                   bounds[:-1, 1:].ravel()])[0],
-                        dims=(''.join(var.dims[-2:]), '_bnds'),
+                        np.dstack(
+                            [
+                                bounds[1:, 1:].ravel(),
+                                bounds[1:, :-1].ravel(),
+                                bounds[:-1, :-1].ravel(),
+                                bounds[:-1, 1:].ravel(),
+                            ]
+                        )[0],
+                        dims=("".join(var.dims[-2:]), "_bnds"),
                         attrs=coord.attrs.copy(),
-                        name=coord.name + '_bnds')
+                        name=coord.name + "_bnds",
+                    )
                 else:
                     raise NotImplementedError(
-                        "More than 2D-bounds are not supported")
+                        "More than 2D-bounds are not supported"
+                    )
             if bounds is not None and bounds.shape[-1] == 2:
                 # normal CF-Conventions for rectangular grids
                 arr = bounds.values
-                if axis == 'y':
-                    stacked = np.c_[arr[..., :1], arr[..., :1],
-                                    arr[..., 1:], arr[..., 1:]]
+                if axis == "y":
+                    stacked = np.c_[
+                        arr[..., :1], arr[..., :1], arr[..., 1:], arr[..., 1:]
+                    ]
                     if bounds.ndim == 2:
                         stacked = np.repeat(
                             stacked.reshape((-1, 4)),
-                            len(self.get_x(var, coords)), axis=0)
+                            len(self.get_x(var, coords)),
+                            axis=0,
+                        )
                     else:
                         stacked = stacked.reshape((-1, 4))
                 else:
                     stacked = np.c_[arr, arr[..., ::-1]]
                     if bounds.ndim == 2:
                         stacked = np.tile(
-                            stacked, (len(self.get_y(var, coords)), 1))
+                            stacked, (len(self.get_y(var, coords)), 1)
+                        )
                     else:
                         stacked = stacked.reshape((-1, 4))
                 bounds = xr.DataArray(
                     stacked,
-                    dims=('cell', bounds.dims[1]), name=bounds.name,
-                    attrs=bounds.attrs)
+                    dims=("cell", bounds.dims[1]),
+                    name=bounds.name,
+                    attrs=bounds.attrs,
+                )
 
             return bounds
         return None
 
-    docstrings.delete_params('CFDecoder.get_cell_node_coord.parameters',
-                             'var', 'axis')
+    docstrings.delete_params(
+        "CFDecoder.get_cell_node_coord.parameters", "var", "axis"
+    )
 
     @docstrings.dedent
-    def _get_coord_cell_node_coord(self, coord, coords=None, nans=None,
-                                   var=None):
+    def _get_coord_cell_node_coord(
+        self, coord, coords=None, nans=None, var=None
+    ):
         """
         Get the boundaries of an unstructed coordinate
 
         Parameters
         ----------
         coord: xr.Variable
             The coordinate whose bounds should be returned
         %(CFDecoder.get_cell_node_coord.parameters.no_var|axis)s
 
         Returns
         -------
         %(CFDecoder.get_cell_node_coord.returns)s
         """
-        bounds = coord.attrs.get('bounds')
+        bounds = coord.attrs.get("bounds")
         if bounds is not None:
             bounds = self.ds.coords.get(bounds)
         if bounds is not None:
             if coords is not None:
-                bounds = bounds.sel(**{
-                    key: coords[key]
-                    for key in set(coords).intersection(bounds.dims)})
+                bounds = bounds.sel(
+                    **{
+                        key: coords[key]
+                        for key in set(coords).intersection(bounds.dims)
+                    }
+                )
             if nans is not None and var is None:
                 raise ValueError("Need the variable to deal with NaN!")
             elif nans is None:
                 pass
-            elif nans == 'skip':
+            elif nans == "skip":
                 dims = [dim for dim in set(var.dims) - set(bounds.dims)]
                 mask = var.notnull().all(list(dims)) if dims else var.notnull()
                 try:
                     bounds = bounds[mask.values]
                 except IndexError:  # 3D bounds
                     bounds = bounds.where(mask)
-            elif nans == 'only':
+            elif nans == "only":
                 dims = [dim for dim in set(var.dims) - set(bounds.dims)]
                 mask = var.isnull().all(list(dims)) if dims else var.isnull()
                 bounds = bounds[mask.values]
             else:
                 raise ValueError(
                     "`nans` must be either None, 'skip', or 'only'! "
-                    "Not {0}!".format(str(nans)))
+                    "Not {0}!".format(str(nans))
+                )
             return bounds
 
-    @docstrings.get_sections(base='CFDecoder._check_unstructured_bounds', sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder._check_unstructured_bounds",
+        sections=["Parameters", "Returns"],
+    )
     @docstrings.dedent
-    def _check_unstructured_bounds(self, var, coords=None, axis='x', nans=None):
+    def _check_unstructured_bounds(
+        self, var, coords=None, axis="x", nans=None
+    ):
         """
         Checks whether the bounds in the variable attribute are triangular
 
         Parameters
         ----------
         %(CFDecoder.get_cell_node_coord.parameters)s
 
@@ -889,20 +909,24 @@
         -------
         %(CFDecoder.is_unstructured.returns)s
 
         Notes
         -----
         Currently this is the same as :meth:`is_unstructured` method, but may
         change in the future to support hexagonal grids"""
-        if str(var.attrs.get('grid_type')) == 'unstructured':
+        if str(var.attrs.get("grid_type")) == "unstructured":
             return True
         xcoord = self.get_x(var)
         if xcoord is not None:
             bounds = self._get_coord_cell_node_coord(xcoord)
-            if bounds is not None and bounds.ndim == 2 and bounds.shape[-1] > 2:
+            if (
+                bounds is not None
+                and bounds.ndim == 2
+                and bounds.shape[-1] > 2
+            ):
                 return True
 
     @docstrings.dedent
     def is_circumpolar(self, var):
         """
         Test if a variable is on a circumpolar grid
 
@@ -969,81 +993,106 @@
                         raise
                     return None
                 ret = self.ds.coords[cname]
                 try:
                     idims = var.psy.idims
                 except AttributeError:  # got xarray.Variable
                     idims = {}
-                return ret.isel(**{d: sl for d, sl in idims.items()
-                                   if d in ret.dims})
+                return ret.isel(
+                    **{d: sl for d, sl in idims.items() if d in ret.dims}
+                )
+
+        def guess_x(cname):
+            cname = cname.lower()
+            return (
+                "lon" in cname or cname.endswith("x") or cname.startswith("x")
+            )
+
+        def guess_y(cname):
+            cname = cname.lower()
+            return (
+                "lat" in cname or cname.endswith("y") or cname.startswith("y")
+            )
 
         axis = axis.lower()
-        if axis not in list('xyzt'):
-            raise ValueError("Axis must be one of X, Y, Z, T, not {0}".format(
-                axis))
+        if axis not in list("xyzt"):
+            raise ValueError(
+                "Axis must be one of X, Y, Z, T, not {0}".format(axis)
+            )
         # we first check for the dimensions and then for the coordinates
         # attribute
         coords = coords or self.ds.coords
-        coord_names = var.attrs.get('coordinates', var.encoding.get(
-            'coordinates', '')).split()
+        coord_names = var.attrs.get(
+            "coordinates", var.encoding.get("coordinates", "")
+        ).split()
         if not coord_names:
             return
         ret = []
         matched = []
-        for coord in map(lambda dim: coords[dim], filter(
-                lambda dim: dim in coords, chain(
-                    coord_names, var.dims))):
+        for coord in map(
+            lambda dim: coords[dim],
+            filter(lambda dim: dim in coords, chain(coord_names, var.dims)),
+        ):
             # check for the axis attribute or whether the coordinate is in the
             # list of possible coordinate names
             if coord.name not in (c.name for c in ret):
                 if coord.name in getattr(self, axis):
                     matched.append(coord)
-                elif coord.attrs.get('axis', '').lower() == axis:
+                elif coord.attrs.get("axis", "").lower() == axis:
                     ret.append(coord)
         if matched:
             if len(set([c.name for c in matched])) > 1:
-                warn("Found multiple matches for %s coordinate in the "
-                     "coordinates: %s. I use %s" % (
-                         axis, ', '.join([c.name for c in matched]),
-                         matched[0].name),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for %s coordinate in the "
+                    "coordinates: %s. I use %s"
+                    % (
+                        axis,
+                        ", ".join([c.name for c in matched]),
+                        matched[0].name,
+                    ),
+                    PsyPlotRuntimeWarning,
+                )
             return matched[0]
         elif ret:
             return None if len(ret) > 1 else ret[0]
         # If the coordinates attribute is specified but the coordinate
         # variables themselves have no 'axis' attribute, we interpret the
         # coordinates such that x: -1, y: -2, z: -3
         # Since however the CF Conventions do not determine the order on how
         # the coordinates shall be saved, we try to use a pattern matching
         # for latitude and longitude. This is not very nice, hence it is
         # better to specify the :attr:`x` and :attr:`y` attribute
         tnames = self.t.intersection(coord_names)
-        if axis == 'x':
-            for cname in filter(lambda cname: re.search('lon', cname),
-                                coord_names):
+        if axis == "x":
+            for cname in filter(guess_x, coord_names):
                 return get_coord(cname)
             return get_coord(coord_names[-1], raise_error=False)
-        elif axis == 'y' and len(coord_names) >= 2:
-            for cname in filter(lambda cname: re.search('lat', cname),
-                                coord_names):
+        elif axis == "y" and len(coord_names) >= 2:
+            for cname in filter(guess_y, coord_names):
                 return get_coord(cname)
             return get_coord(coord_names[-2], raise_error=False)
-        elif (axis == 'z' and len(coord_names) >= 3 and
-              coord_names[-3] not in tnames):
+        elif (
+            axis == "z"
+            and len(coord_names) >= 3
+            and coord_names[-3] not in tnames
+        ):
             return get_coord(coord_names[-3], raise_error=False)
-        elif axis == 't' and tnames:
+        elif axis == "t" and tnames:
             tname = next(iter(tnames))
             if len(tnames) > 1:
-                warn("Found multiple matches for time coordinate in the "
-                     "coordinates: %s. I use %s" % (', '.join(tnames), tname),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for time coordinate in the "
+                    "coordinates: %s. I use %s" % (", ".join(tnames), tname),
+                    PsyPlotRuntimeWarning,
+                )
             return get_coord(tname, raise_error=False)
 
-    @docstrings.get_sections(base="CFDecoder.get_x", sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.get_x", sections=["Parameters", "Returns"]
+    )
     @dedent
     def get_x(self, var, coords=None):
         """
         Get the x-coordinate of a variable
 
         This method searches for the x-coordinate in the :attr:`ds`. It first
         checks whether there is one dimension that holds an ``'axis'``
@@ -1060,15 +1109,15 @@
             :attr:`ds` attribute are used.
 
         Returns
         -------
         xarray.Coordinate or None
             The y-coordinate or None if it could be found"""
         coords = coords or self.ds.coords
-        coord = self.get_variable_by_axis(var, 'x', coords)
+        coord = self.get_variable_by_axis(var, "x", coords)
         if coord is not None:
             return coord
         return coords.get(self.get_xname(var))
 
     def get_xname(self, var, coords=None):
         """Get the name of the x-dimension
 
@@ -1088,30 +1137,33 @@
         str
             The coordinate name
 
         See Also
         --------
         get_x"""
         if coords is not None:
-            coord = self.get_variable_by_axis(var, 'x', coords)
+            coord = self.get_variable_by_axis(var, "x", coords)
             if coord is not None and coord.name in var.dims:
                 return coord.name
         dimlist = list(self.x.intersection(var.dims))
         if dimlist:
             if len(dimlist) > 1:
-                warn("Found multiple matches for x coordinate in the variable:"
-                     "%s. I use %s" % (', '.join(dimlist), dimlist[0]),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for x coordinate in the variable:"
+                    "%s. I use %s" % (", ".join(dimlist), dimlist[0]),
+                    PsyPlotRuntimeWarning,
+                )
             return dimlist[0]
         # otherwise we return the coordinate in the last position
         if var.dims:
             return var.dims[-1]
 
-    @docstrings.get_sections(base="CFDecoder.get_y", sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.get_y", sections=["Parameters", "Returns"]
+    )
     @dedent
     def get_y(self, var, coords=None):
         """
         Get the y-coordinate of a variable
 
         This method searches for the y-coordinate in the :attr:`ds`. It first
         checks whether there is one dimension that holds an ``'axis'``
@@ -1129,15 +1181,15 @@
             :attr:`ds` attribute are used.
 
         Returns
         -------
         xarray.Coordinate or None
             The y-coordinate or None if it could be found"""
         coords = coords or self.ds.coords
-        coord = self.get_variable_by_axis(var, 'y', coords)
+        coord = self.get_variable_by_axis(var, "y", coords)
         if coord is not None:
             return coord
         return coords.get(self.get_yname(var))
 
     def get_yname(self, var, coords=None):
         """Get the name of the y-dimension
 
@@ -1157,33 +1209,36 @@
         str
             The coordinate name
 
         See Also
         --------
         get_y"""
         if coords is not None:
-            coord = self.get_variable_by_axis(var, 'y', coords)
+            coord = self.get_variable_by_axis(var, "y", coords)
             if coord is not None and coord.name in var.dims:
                 return coord.name
         dimlist = list(self.y.intersection(var.dims))
         if dimlist:
             if len(dimlist) > 1:
-                warn("Found multiple matches for y coordinate in the variable:"
-                     "%s. I use %s" % (', '.join(dimlist), dimlist[0]),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for y coordinate in the variable:"
+                    "%s. I use %s" % (", ".join(dimlist), dimlist[0]),
+                    PsyPlotRuntimeWarning,
+                )
             return dimlist[0]
         # otherwise we return the coordinate in the last or second last
         # position
         if var.dims:
             if self.is_unstructured(var):
                 return var.dims[-1]
             return var.dims[-2 if var.ndim > 1 else -1]
 
-    @docstrings.get_sections(base="CFDecoder.get_z", sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.get_z", sections=["Parameters", "Returns"]
+    )
     @dedent
     def get_z(self, var, coords=None):
         """
         Get the vertical (z-) coordinate of a variable
 
         This method searches for the z-coordinate in the :attr:`ds`. It first
         checks whether there is one dimension that holds an ``'axis'``
@@ -1201,15 +1256,15 @@
             :attr:`ds` attribute are used.
 
         Returns
         -------
         xarray.Coordinate or None
             The z-coordinate or None if no z coordinate could be found"""
         coords = coords or self.ds.coords
-        coord = self.get_variable_by_axis(var, 'z', coords)
+        coord = self.get_variable_by_axis(var, "z", coords)
         if coord is not None:
             return coord
         zname = self.get_zname(var)
         if zname is not None:
             return coords.get(zname)
         return None
 
@@ -1233,36 +1288,42 @@
             The coordinate name or None if no vertical coordinate could be
             found
 
         See Also
         --------
         get_z"""
         if coords is not None:
-            coord = self.get_variable_by_axis(var, 'z', coords)
+            coord = self.get_variable_by_axis(var, "z", coords)
             if coord is not None and coord.name in var.dims:
                 return coord.name
         dimlist = list(self.z.intersection(var.dims))
         if dimlist:
             if len(dimlist) > 1:
-                warn("Found multiple matches for z coordinate in the variable:"
-                     "%s. I use %s" % (', '.join(dimlist), dimlist[0]),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for z coordinate in the variable:"
+                    "%s. I use %s" % (", ".join(dimlist), dimlist[0]),
+                    PsyPlotRuntimeWarning,
+                )
             return dimlist[0]
         # otherwise we return the coordinate in the third last position
         if var.dims:
             is_unstructured = self.is_unstructured(var)
             icheck = -2 if is_unstructured else -3
-            min_dim = abs(icheck) if 'variable' not in var.dims else abs(icheck-1)
+            min_dim = (
+                abs(icheck) if "variable" not in var.dims else abs(icheck - 1)
+            )
             if var.ndim >= min_dim and var.dims[icheck] != self.get_tname(
-                    var, coords):
+                var, coords
+            ):
                 return var.dims[icheck]
         return None
 
-    @docstrings.get_sections(base="CFDecoder.get_t", sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.get_t", sections=["Parameters", "Returns"]
+    )
     @dedent
     def get_t(self, var, coords=None):
         """
         Get the time coordinate of a variable
 
         This method searches for the time coordinate in the :attr:`ds`. It
         first checks whether there is one dimension that holds an ``'axis'``
@@ -1279,24 +1340,26 @@
             :attr:`ds` attribute are used.
 
         Returns
         -------
         xarray.Coordinate or None
             The time coordinate or None if no time coordinate could be found"""
         coords = coords or self.ds.coords
-        coord = self.get_variable_by_axis(var, 't', coords)
+        coord = self.get_variable_by_axis(var, "t", coords)
         if coord is not None:
             return coord
         dimlist = list(self.t.intersection(var.dims).intersection(coords))
         if dimlist:
             if len(dimlist) > 1:
-                warn("Found multiple matches for time coordinate in the "
-                     "variable: %s. I use %s" % (
-                         ', '.join(dimlist), dimlist[0]),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for time coordinate in the "
+                    "variable: %s. I use %s"
+                    % (", ".join(dimlist), dimlist[0]),
+                    PsyPlotRuntimeWarning,
+                )
             return coords[dimlist[0]]
         tname = self.get_tname(var)
         if tname is not None:
             return coords.get(tname)
         return None
 
     def get_tname(self, var, coords=None):
@@ -1317,23 +1380,25 @@
         str or None
             The coordinate name or None if no time coordinate could be found
 
         See Also
         --------
         get_t"""
         if coords is not None:
-            coord = self.get_variable_by_axis(var, 't', coords)
+            coord = self.get_variable_by_axis(var, "t", coords)
             if coord is not None and coord.name in var.dims:
                 return coord.name
         dimlist = list(self.t.intersection(var.dims))
         if dimlist:
             if len(dimlist) > 1:
-                warn("Found multiple matches for t coordinate in the variable:"
-                     "%s. I use %s" % (', '.join(dimlist), dimlist[0]),
-                     PsyPlotRuntimeWarning)
+                warn(
+                    "Found multiple matches for t coordinate in the variable:"
+                    "%s. I use %s" % (", ".join(dimlist), dimlist[0]),
+                    PsyPlotRuntimeWarning,
+                )
             return dimlist[0]
         # otherwise we return None
         return None
 
     def get_idims(self, arr, coords=None):
         """Get the coordinates in the :attr:`ds` dataset as int or slice
 
@@ -1359,22 +1424,27 @@
         See Also
         --------
         xarray.Dataset.isel, InteractiveArray.idims"""
         if coords is None:
             coords = arr.coords
         else:
             coords = {
-                label: coord for label, coord in six.iteritems(arr.coords)
-                if label in coords}
+                label: coord
+                for label, coord in six.iteritems(arr.coords)
+                if label in coords
+            }
         ret = self.get_coord_idims(coords)
         # handle the coordinates that are not in the dataset
         missing = set(arr.dims).difference(ret)
         if missing:
-            warn('Could not get slices for the following dimensions: %r' % (
-                missing, ), PsyPlotRuntimeWarning)
+            warn(
+                "Could not get slices for the following dimensions: %r"
+                % (missing,),
+                PsyPlotRuntimeWarning,
+            )
         return ret
 
     def get_coord_idims(self, coords):
         """Get the slicers for the given coordinates from the base dataset
 
         This method converts `coords` to slicers (list of
         integers or ``slice`` objects)
@@ -1389,19 +1459,21 @@
         -------
         dict
             Mapping from coordinate name to integer, list of integer or slice
         """
         ret = dict(
             (label, get_index_from_coord(coord, self.ds.indexes[label]))
             for label, coord in six.iteritems(coords)
-            if label in self.ds.indexes)
+            if label in self.ds.indexes
+        )
         return ret
 
-    @docstrings.get_sections(base='CFDecoder.get_plotbounds', sections=[
-        'Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="CFDecoder.get_plotbounds", sections=["Parameters", "Returns"]
+    )
     @dedent
     def get_plotbounds(self, coord, kind=None, ignore_shape=False):
         """
         Get the bounds of a coordinate
 
         This method first checks the ``'bounds'`` attribute of the given
         `coord` and if it fails, it calculates them.
@@ -1422,25 +1494,27 @@
         Returns
         -------
         bounds: np.ndarray
             The bounds with the same number of dimensions as `coord` but one
             additional array (i.e. if `coord` has shape (4, ), `bounds` will
             have shape (5, ) and if `coord` has shape (4, 5), `bounds` will
             have shape (5, 6)"""
-        if 'bounds' in coord.attrs:
-            bounds = self.ds.coords[coord.attrs['bounds']]
+        if "bounds" in coord.attrs:
+            bounds = self.ds.coords[coord.attrs["bounds"]]
             if ignore_shape:
                 return bounds.values.ravel()
             if not bounds.shape[:-1] == coord.shape:
                 bounds = self.ds.isel(**self.get_idims(coord))
             try:
                 return self._get_plotbounds_from_cf(coord, bounds)
             except ValueError as e:
-                warn((e.message if six.PY2 else str(e)) +
-                     " Bounds are calculated automatically!")
+                warn(
+                    (e.message if six.PY2 else str(e))
+                    + " Bounds are calculated automatically!"
+                )
         return self._infer_interval_breaks(coord, kind=kind)
 
     @staticmethod
     @docstrings.dedent
     def _get_plotbounds_from_cf(coord, bounds):
         """
         Get plot bounds from the bounds stored as defined by CFConventions
@@ -1460,30 +1534,42 @@
         -----
         this currently only works for rectilinear grids"""
 
         if bounds.shape[:-1] != coord.shape or bounds.shape[-1] != 2:
             raise ValueError(
                 "Cannot interprete bounds with shape {0} for {1} "
                 "coordinate with shape {2}.".format(
-                    bounds.shape, coord.name, coord.shape))
-        ret = np.zeros(tuple(map(lambda i: i+1, coord.shape)))
+                    bounds.shape, coord.name, coord.shape
+                )
+            )
+        ret = np.zeros(tuple(map(lambda i: i + 1, coord.shape)))
         ret[tuple(map(slice, coord.shape))] = bounds[..., 0]
         last_slices = tuple(slice(-1, None) for _ in coord.shape)
         ret[last_slices] = bounds[tuple(chain(last_slices, [1]))]
         return ret
 
-    docstrings.keep_params('CFDecoder._check_unstructured_bounds.parameters',
-                           'nans')
-
-    @docstrings.get_sections(base='CFDecoder.get_triangles', sections=[
-        'Parameters', 'Returns'])
+    docstrings.keep_params(
+        "CFDecoder._check_unstructured_bounds.parameters", "nans"
+    )
+
+    @docstrings.get_sections(
+        base="CFDecoder.get_triangles", sections=["Parameters", "Returns"]
+    )
     @docstrings.dedent
-    def get_triangles(self, var, coords=None, convert_radian=True,
-                      copy=False, src_crs=None, target_crs=None,
-                      nans=None, stacklevel=1):
+    def get_triangles(
+        self,
+        var,
+        coords=None,
+        convert_radian=True,
+        copy=False,
+        src_crs=None,
+        target_crs=None,
+        nans=None,
+        stacklevel=1,
+    ):
         """
         Get the triangles for the variable
 
         Parameters
         ----------
         var: xarray.Variable or xarray.DataArray
             The variable to use
@@ -1508,49 +1594,55 @@
         matplotlib.tri.Triangulation
             The spatial triangles of the variable
 
         Raises
         ------
         ValueError
             If `src_crs` is not None and `target_crs` is None"""
-        warn("The 'get_triangles' method is depreceated and will be removed "
-             "soon! Use the 'get_cell_node_coord' method!",
-             DeprecationWarning, stacklevel=stacklevel)
+        warn(
+            "The 'get_triangles' method is depreceated and will be removed "
+            "soon! Use the 'get_cell_node_coord' method!",
+            DeprecationWarning,
+            stacklevel=stacklevel,
+        )
         from matplotlib.tri import Triangulation
 
         def get_vertices(axis):
-            bounds = self._check_unstructured_bounds(var, coords=coords,
-                                                   axis=axis, nans=nans)[1]
+            bounds = self._check_unstructured_bounds(
+                var, coords=coords, axis=axis, nans=nans
+            )[1]
             if coords is not None:
                 bounds = coords.get(bounds.name, bounds)
             vertices = bounds.values.ravel()
             if convert_radian:
-                coord = getattr(self, 'get_' + axis)(var)
-                if coord.attrs.get('units') == 'radian':
-                    vertices = vertices * 180. / np.pi
+                coord = getattr(self, "get_" + axis)(var)
+                if coord.attrs.get("units") == "radian":
+                    vertices = vertices * 180.0 / np.pi
             return vertices if not copy else vertices.copy()
 
         if coords is None:
             coords = self.ds.coords
 
-        xvert = get_vertices('x')
-        yvert = get_vertices('y')
+        xvert = get_vertices("x")
+        yvert = get_vertices("y")
         if src_crs is not None and src_crs != target_crs:
             if target_crs is None:
                 raise ValueError(
                     "Found %s for the source crs but got None for the "
-                    "target_crs!" % (src_crs, ))
+                    "target_crs!" % (src_crs,)
+                )
             arr = target_crs.transform_points(src_crs, xvert, yvert)
             xvert = arr[:, 0]
             yvert = arr[:, 1]
         triangles = np.reshape(range(len(xvert)), (len(xvert) // 3, 3))
         return Triangulation(xvert, yvert, triangles)
 
     docstrings.delete_params(
-        'CFDecoder.get_plotbounds.parameters', 'ignore_shape')
+        "CFDecoder.get_plotbounds.parameters", "ignore_shape"
+    )
 
     @staticmethod
     def _infer_interval_breaks(coord, kind=None):
         """
         Interpolate the bounds from the data in coord
 
         Parameters
@@ -1564,25 +1656,27 @@
         Notes
         -----
         this currently only works for rectilinear grids"""
         if coord.ndim == 1:
             return _infer_interval_breaks(coord)
         elif coord.ndim == 2:
             from scipy.interpolate import interp2d
-            kind = kind or rcParams['decoder.interp_kind']
+
+            kind = kind or rcParams["decoder.interp_kind"]
             y, x = map(np.arange, coord.shape)
             new_x, new_y = map(_infer_interval_breaks, [x, y])
             coord = np.asarray(coord)
             return interp2d(x, y, coord, kind=kind, copy=False)(new_x, new_y)
 
     @classmethod
-    @docstrings.get_sections(base='CFDecoder._decode_ds')
+    @docstrings.get_sections(base="CFDecoder._decode_ds")
     @docstrings.dedent
-    def _decode_ds(cls, ds, gridfile=None, decode_coords=True,
-                   decode_times=True):
+    def _decode_ds(
+        cls, ds, gridfile=None, decode_coords=True, decode_times=True
+    ):
         """
         Static method to decode coordinates and time informations
 
         This method interpretes absolute time informations (stored with units
         ``'day as %Y%m%d.%f'``) and coordinates
 
         Parameters
@@ -1597,19 +1691,23 @@
             in the resulting dataset."""
         if decode_coords:
             ds = cls.decode_coords(ds, gridfile=gridfile)
         if decode_times:
             for k, v in six.iteritems(ds.variables):
                 # check for absolute time units and make sure the data is not
                 # already decoded via dtype check
-                if v.attrs.get('units', '') == 'day as %Y%m%d.%f' and (
-                        np.issubdtype(v.dtype, np.float64)):
+                if v.attrs.get("units", "") == "day as %Y%m%d.%f" and (
+                    np.issubdtype(v.dtype, np.float64)
+                ):
                     decoded = xr.Variable(
-                        v.dims, AbsoluteTimeDecoder(v), attrs=v.attrs,
-                        encoding=v.encoding)
+                        v.dims,
+                        AbsoluteTimeDecoder(v),
+                        attrs=v.attrs,
+                        encoding=v.encoding,
+                    )
                     ds.update({k: decoded})
         return ds
 
     @classmethod
     @docstrings.dedent
     def decode_ds(cls, ds, *args, **kwargs):
         """
@@ -1638,21 +1736,24 @@
         var: xarray.Variable
             The variable to get the data for
         dims: dict
             a mapping from dimension to the slices
         remove: bool
             If True, dimensions in `dims` that are not in the dimensions of
             `var` are removed"""
-        method_mapping = {'x': self.get_xname,
-                          'z': self.get_zname, 't': self.get_tname}
+        method_mapping = {
+            "x": self.get_xname,
+            "z": self.get_zname,
+            "t": self.get_tname,
+        }
         dims = dict(dims)
         if self.is_unstructured(var):  # we assume a one-dimensional grid
-            method_mapping['y'] = self.get_xname
+            method_mapping["y"] = self.get_xname
         else:
-            method_mapping['y'] = self.get_yname
+            method_mapping["y"] = self.get_yname
         for key in six.iterkeys(dims.copy()):
             if key in method_mapping and key not in var.dims:
                 dim_name = method_mapping[key](var, self.ds.coords)
                 if dim_name in dims:
                     dims.pop(key)
                 else:
                     new_name = method_mapping[key](var)
@@ -1660,15 +1761,17 @@
                         dims[new_name] = dims.pop(key)
         # now remove the unnecessary dimensions
         if remove:
             for key in set(dims).difference(var.dims):
                 dims.pop(key)
                 self.logger.debug(
                     "Could not find a dimensions matching %s in variable %s!",
-                    key, var)
+                    key,
+                    var,
+                )
         return dims
 
     def standardize_dims(self, var, dims={}):
         """Replace the coordinate names through x, y, z and t
 
         Parameters
         ----------
@@ -1678,32 +1781,379 @@
             The dictionary to use for replacing the original dimensions
 
         Returns
         -------
         dict
             The dictionary with replaced dimensions"""
         dims = dict(dims)
-        name_map = {self.get_xname(var, self.ds.coords): 'x',
-                    self.get_yname(var, self.ds.coords): 'y',
-                    self.get_zname(var, self.ds.coords): 'z',
-                    self.get_tname(var, self.ds.coords): 't'}
+        name_map = {
+            self.get_xname(var, self.ds.coords): "x",
+            self.get_yname(var, self.ds.coords): "y",
+            self.get_zname(var, self.ds.coords): "z",
+            self.get_tname(var, self.ds.coords): "t",
+        }
         dims = dict(dims)
         for dim in set(dims).intersection(name_map):
             dims[name_map[dim]] = dims.pop(dim)
         return dims
 
+    def clear_cache(self):
+        """Clear any cached data.
+        The default method does nothing but can be reimplemented by subclasses
+        to clear data has been computed."""
+        pass
+
+    # -------------------------------------------------------------------------
+    # --------------- Grid informations on a variable -------------------------
+    # -------------------------------------------------------------------------
+
+    @docstrings.get_sections(base="CFDecoder.get_metadata_for_variable")
+    @docstrings.dedent
+    def get_metadata_for_variable(
+        self,
+        var: xr.DataArray,
+        coords: Optional[Dict] = None,
+        fail_on_error: bool = False,
+        include_tracebacks: bool = False,
+    ) -> Dict[str, Dict[str, str]]:
+        """Get the metadata information on a variable.
+
+        Parameters
+        ----------
+        var : xarray.DataArray
+            The data array to get the metadata for
+        coords: Dict, optional
+            The coordinates to use. If none, we'll fallback to the coordinates
+            of the base dataset.
+        fail_on_error: bool, default False
+            If True, an error is raised when an error occurs. Otherwise it is
+            captured and entered as an attribute to the metadata.
+        include_tracebacks: bool, default False
+            If True, the full traceback of the error is included
+
+        Returns
+        -------
+        Dict[str, Dict[str, str]]
+            A mapping from meta data sections for meta data attributes on the
+            specific section.
+        """
+        sections = self.get_metadata_sections(var)
+        ret = {}
+        if coords is None:
+            coords = self.ds.coords
+        for section in sections:
+            try:
+                attrs = self.get_metadata_for_section(var, section, coords)
+            except Exception as e:
+                if fail_on_error:
+                    raise
+                else:
+                    attrs = {"error": str(e)}
+                    if include_tracebacks:
+                        s = io.StringIO()
+                        tb.print_exc(file=s)
+                        attrs["traceback"] = s.getvalue()
+            if attrs:
+                ret[section] = attrs
+        return ret
+
+    docstrings.keep_params(
+        "CFDecoder.get_metadata_for_variable.parameters", "var"
+    )
+
+    @docstrings.dedent
+    def get_metadata_sections(self, var: xr.DataArray) -> List[str]:
+        """Get the metadata sections for a variable.
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+
+        Returns
+        -------
+        List[str]
+            The sections for the metadata information
+        """
+        return [
+            "Attributes",
+            "Time information",
+            "Vertical information",
+            "X-Coordinate information",
+            "Y-Coordinate information",
+            "Other dimensions",
+            "Projection info",
+            "Grid type info",
+        ]
+
+    @docstrings.dedent
+    @docstrings.get_sections(
+        base="CFDecoder.get_metadata_for_section",
+        sections=["Parameters", "Returns"],
+    )
+    def get_metadata_for_section(
+        self, var: xr.DataArray, section: str, coords: Dict
+    ) -> Dict[str, str]:
+        """Get the metadata for a specific section
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        section : str
+            The section name
+        coords : Dict
+            Other coordinates in the dataset
+
+        Returns
+        -------
+        Dict[str, str]
+            A mapping from metadata name to section.
+        """
+        standard_dimensions = {
+            "Time information": self.get_t_metadata,
+            "Vertical information": self.get_z_metadata,
+            "X-Coordinate information": self.get_x_metadata,
+            "Y-Coordinate information": self.get_y_metadata,
+        }
+        if section in standard_dimensions:
+            return standard_dimensions[section](var, coords)
+        elif section == "Other dimensions":
+            xyzt = {
+                self.get_xname(var, self.ds.coords),
+                self.get_yname(var, self.ds.coords),
+                self.get_zname(var, self.ds.coords),
+                self.get_tname(var, self.ds.coords),
+            }
+            other_dims = list(map(str, set(var.dims) - xyzt))
+            if other_dims:
+                return {"Dimension names": ", ".join(other_dims)}
+        elif section == "Attributes":
+            return {key: str(val) for key, val in var.attrs.items()}
+        elif section == "Projection info":
+            if "grid_mapping" in var.attrs:
+                return self.get_projection_info(var, coords)
+        elif section == "Grid type info":
+            return self.get_grid_type_info(var, coords)
+
+        return {}
+
+    def get_grid_type_info(
+        self, var: xr.DataArray, coords: Dict
+    ) -> Dict[str, str]:
+        """Get info on the grid type
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        coords : Dict
+            Other coordinates in the dataset
+
+        Returns
+        -------
+        Dict[str, str]
+            The info on the grid type
+        """
+        return {
+            "unstructured": self.is_unstructured(var),
+            "curvilinear": self.is_circumpolar(var),
+        }
+
+    def get_projection_info(
+        self, var: xr.DataArray, coords: Dict
+    ) -> Dict[str, str]:
+        """Get info on the projection
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        coords : Dict
+            Other coordinates in the dataset
+
+        Returns
+        -------
+        Dict[str, str]
+            The grid mapping attributes
+
+        Raises
+        ------
+        KeyError
+            when the variable specified by the `grid_mapping` is not part of
+            the given `coords`
+        """
+        try:
+            grid_mapping = coords[var.attrs["grid_mapping"]]
+        except KeyError:
+            raise KeyError(
+                f"Grid mapping variable {repr(var.attrs['grid_mapping'])}"
+                f"could not be found in list of coordinates {tuple(coords)}"
+            )
+        else:
+            return {key: str(val) for key, val in grid_mapping.attrs.items()}
+
+    @docstrings.dedent
+    def get_coord_info(
+        self,
+        var: xr.DataArray,
+        dimname: str,
+        coord: xr.DataArray,
+        coords: Dict,
+        what: str,
+    ) -> Dict[str, str]:
+        """_summary_
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        dimname : str
+            The dimension in the dimension of `var`
+        coord : Union[xr.Variable, xr.DataArray]
+            The coordinate to get the info from
+        coords : Dict
+            Other coordinates in the dataset
+        what : str
+            The name on what this is all bout
+
+        Returns
+        -------
+        Dict[str, str]
+            The coordinate infos
+
+        Raises
+        ------
+        ValueError
+            When the coordinates specifies boundaries but they could not be
+            found in the given `coords`
+        """
+        ret: Dict[str, str] = {
+            "Dimension name": dimname,
+            "Coordinate": str(coord.name),
+            "Shape": f"{coord.dims} -> {coord.shape}",
+        }
+        if "bounds" in coord.attrs:
+            bounds = coord.attrs["bounds"]
+            ret["Boundary variable"] = bounds
+            try:
+                bc = coords[bounds]
+            except KeyError:
+                raise KeyError(
+                    f"{what} {repr(coord.name)} specifies a bounds "
+                    f"attribute, but {repr(bounds)} is not part of the given "
+                    f"coordinates {tuple(coords)}."
+                )
+            else:
+                ret["Boundary variable shape"] = f"{bc.dims} -> {bc.shape}"
+        return ret
+
+    @docstrings.dedent
+    def get_t_metadata(
+        self, var: xr.DataArray, coords: Dict
+    ) -> Dict[str, str]:
+        """Get the temporal metadata for a variable.
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        coords: Dict
+            The coordinates to use
+
+        Returns
+        -------
+        %(CFDecoder.get_metadata_for_section.returns)s
+        """
+        dimname = self.get_tname(var)
+        coord = self.get_t(var)
+        if not dimname or coord is None:
+            return {}
+        return self.get_coord_info(
+            var, dimname, coord, coords, "Time coordinate"
+        )
+
+    @docstrings.dedent
+    def get_z_metadata(
+        self, var: xr.DataArray, coords: Dict
+    ) -> Dict[str, str]:
+        """Get the vertical level metadata for a variable.
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        coords: Dict
+            The coordinates to use
+
+        Returns
+        -------
+        %(CFDecoder.get_metadata_for_section.returns)s
+        """
+        dimname = self.get_zname(var)
+        coord = self.get_z(var)
+        if not dimname or coord is None:
+            return {}
+        return self.get_coord_info(
+            var, dimname, coord, coords, "Vertical coordinate"
+        )
+
+    @docstrings.dedent
+    def get_x_metadata(
+        self, var: xr.DataArray, coords: Dict
+    ) -> Dict[str, str]:
+        """Get the metadata for spatial x-dimension.
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        coords: Dict
+            The coordinates to use
+
+        Returns
+        -------
+        %(CFDecoder.get_metadata_for_section.returns)s
+        """
+        dimname = self.get_xname(var)
+        coord = self.get_x(var)
+        if not dimname or coord is None:
+            return {}
+        return self.get_coord_info(var, dimname, coord, coords, "X-coordinate")
+
+    @docstrings.dedent
+    def get_y_metadata(
+        self, var: xr.DataArray, coords: Dict
+    ) -> Dict[str, str]:
+        """Get the metadata for spatial y-dimension.
+
+        Parameters
+        ----------
+        %(CFDecoder.get_metadata_for_variable.parameters.var)s
+        coords: Dict
+            The coordinates to use
+
+        Returns
+        -------
+        %(CFDecoder.get_metadata_for_section.returns)s
+        """
+        dimname = self.get_yname(var)
+        coord = self.get_y(var)
+        if not dimname or coord is None:
+            return {}
+        return self.get_coord_info(var, dimname, coord, coords, "X-coordinate")
+
 
 class UGridDecoder(CFDecoder):
     """
     Decoder for UGrid data sets
 
     Warnings
     --------
     Currently only triangles are supported."""
 
+    #: True if the data of the CFDecoder supports the extraction of a subset of
+    #: the data based on the indices.
+    #:
+    #: For UGRID conventions, this is not easily possible because the
+    #: extraction of a subset breaks the connectivity information of the mesh
+    supports_spatial_slicing: bool = False
+
     def is_unstructured(self, *args, **kwargs):
         """Reimpletemented to return always True. Any ``*args`` and ``**kwargs``
         are ignored"""
         return True
 
     def get_mesh(self, var, coords=None):
         """Get the mesh variable for the given `var`
@@ -1716,15 +2166,15 @@
             The coordinates to use. If None, the coordinates of the dataset of
             this decoder is used
 
         Returns
         -------
         xarray.Coordinate
             The mesh coordinate"""
-        mesh = var.attrs.get('mesh')
+        mesh = var.attrs.get("mesh")
         if mesh is None:
             return None
         if coords is None:
             coords = self.ds.coords
         return coords.get(mesh, self.ds.coords.get(mesh))
 
     @classmethod
@@ -1742,16 +2192,25 @@
 
         Returns
         -------
         %(CFDecoder.can_decode.returns)s"""
         return cls(ds).get_mesh(var) is not None
 
     @docstrings.dedent
-    def get_triangles(self, var, coords=None, convert_radian=True, copy=False,
-                      src_crs=None, target_crs=None, nans=None, stacklevel=1):
+    def get_triangles(
+        self,
+        var,
+        coords=None,
+        convert_radian=True,
+        copy=False,
+        src_crs=None,
+        target_crs=None,
+        nans=None,
+        stacklevel=1,
+    ):
         """
         Get the of the given coordinate.
 
         Parameters
         ----------
         %(CFDecoder.get_triangles.parameters)s
 
@@ -1764,17 +2223,20 @@
         If the ``'location'`` attribute is set to ``'node'``, a delaunay
         triangulation is performed using the
         :class:`matplotlib.tri.Triangulation` class.
 
         .. todo::
             Implement the visualization for UGrid data shown on the edge of the
             triangles"""
-        warn("The 'get_triangles' method is depreceated and will be removed "
-             "soon! Use the 'get_cell_node_coord' method!",
-             DeprecationWarning, stacklevel=stacklevel)
+        warn(
+            "The 'get_triangles' method is depreceated and will be removed "
+            "soon! Use the 'get_cell_node_coord' method!",
+            DeprecationWarning,
+            stacklevel=stacklevel,
+        )
         from matplotlib.tri import Triangulation
 
         if coords is None:
             coords = self.ds.coords
 
         def get_coord(coord):
             return coords.get(coord, self.ds.coords.get(coord))
@@ -1782,50 +2244,53 @@
         mesh = self.get_mesh(var, coords)
         nodes = self.get_nodes(mesh, coords)
         if any(n is None for n in nodes):
             raise ValueError("Could not find the nodes variables!")
         xvert, yvert = nodes
         xvert = xvert.values
         yvert = yvert.values
-        loc = var.attrs.get('location', 'face')
-        if loc == 'face':
+        loc = var.attrs.get("location", "face")
+        if loc == "face":
             triangles = get_coord(
-                mesh.attrs.get('face_node_connectivity', '')).values
+                mesh.attrs.get("face_node_connectivity", "")
+            ).values
             if triangles is None:
                 raise ValueError(
-                    "Could not find the connectivity information!")
-        elif loc == 'node':
+                    "Could not find the connectivity information!"
+                )
+        elif loc == "node":
             triangles = None
         else:
             raise ValueError(
                 "Could not interprete location attribute (%s) of mesh "
-                "variable %s!" % (loc, mesh.name))
+                "variable %s!" % (loc, mesh.name)
+            )
 
         if convert_radian:
             for coord in nodes:
-                if coord.attrs.get('units') == 'radian':
-                    coord = coord * 180. / np.pi
+                if coord.attrs.get("units") == "radian":
+                    coord = coord * 180.0 / np.pi
         if src_crs is not None and src_crs != target_crs:
             if target_crs is None:
                 raise ValueError(
                     "Found %s for the source crs but got None for the "
-                    "target_crs!" % (src_crs, ))
+                    "target_crs!" % (src_crs,)
+                )
             xvert = xvert[triangles].ravel()
             yvert = yvert[triangles].ravel()
             arr = target_crs.transform_points(src_crs, xvert, yvert)
             xvert = arr[:, 0]
             yvert = arr[:, 1]
-            if loc == 'face':
-                triangles = np.reshape(range(len(xvert)), (len(xvert) // 3,
-                                                           3))
+            if loc == "face":
+                triangles = np.reshape(range(len(xvert)), (len(xvert) // 3, 3))
 
         return Triangulation(xvert, yvert, triangles)
 
     @docstrings.dedent
-    def get_cell_node_coord(self, var, coords=None, axis='x', nans=None):
+    def get_cell_node_coord(self, var, coords=None, axis="x", nans=None):
         """
         Checks whether the bounds in the variable attribute are triangular
 
         Parameters
         ----------
         %(CFDecoder.get_cell_node_coord.parameters)s
 
@@ -1835,59 +2300,76 @@
         if coords is None:
             coords = self.ds.coords
 
         idims = self.get_coord_idims(coords)
 
         def get_coord(coord):
             coord = coords.get(coord, self.ds.coords.get(coord))
-            return coord.isel(**{d: sl for d, sl in idims.items()
-                                 if d in coord.dims})
+            return coord.isel(
+                **{d: sl for d, sl in idims.items() if d in coord.dims}
+            )
 
         mesh = self.get_mesh(var, coords)
         if mesh is None:
             return
         nodes = self.get_nodes(mesh, coords)
         if not len(nodes):
-            raise ValueError("Could not find the nodes variables for the %s "
-                             "coordinate!" % axis)
-        vert = nodes[0 if axis == 'x' else 1]
+            raise ValueError(
+                "Could not find the nodes variables for the %s "
+                "coordinate!" % axis
+            )
+        vert = nodes[0 if axis == "x" else 1]
         if vert is None:
-            raise ValueError("Could not find the nodes variables for the %s "
-                             "coordinate!" % axis)
-        loc = var.attrs.get('location', 'face')
-        if loc == 'node':
+            raise ValueError(
+                "Could not find the nodes variables for the %s "
+                "coordinate!" % axis
+            )
+        loc = var.attrs.get("location", "face")
+        if loc == "node":
             # we assume a triangular grid and use matplotlibs triangulation
             from matplotlib.tri import Triangulation
+
             xvert, yvert = nodes
             triangles = Triangulation(xvert, yvert)
-            if axis == 'x':
+            if axis == "x":
                 bounds = triangles.x[triangles.triangles]
             else:
                 bounds = triangles.y[triangles.triangles]
-        elif loc in ['edge', 'face']:
+        elif loc in ["edge", "face"]:
             connectivity = get_coord(
-                mesh.attrs.get('%s_node_connectivity' % loc, ''))
+                mesh.attrs.get("%s_node_connectivity" % loc, "")
+            )
             if connectivity is None:
                 raise ValueError(
-                    "Could not find the connectivity information!")
+                    "Could not find the connectivity information!"
+                )
             connectivity = connectivity.values
             bounds = vert.values[
-                np.where(np.isnan(connectivity), connectivity[:, :1],
-                         connectivity).astype(int)]
+                np.where(
+                    np.isnan(connectivity), connectivity[:, :1], connectivity
+                ).astype(int)
+            ]
         else:
             raise ValueError(
                 "Could not interprete location attribute (%s) of mesh "
-                "variable %s!" % (loc, mesh.name))
-        dim0 = '__face' if loc == 'node' else var.dims[-1]
+                "variable %s!" % (loc, mesh.name)
+            )
+        dim0 = "__face" if loc == "node" else var.dims[-1]
         return xr.DataArray(
             bounds,
-            coords={key: val for key, val in coords.items()
-                    if (dim0, ) == val.dims},
-            dims=(dim0, '__bnds', ),
-            name=vert.name + '_bnds',  attrs=vert.attrs.copy())
+            coords={
+                key: val for key, val in coords.items() if (dim0,) == val.dims
+            },
+            dims=(
+                dim0,
+                "__bnds",
+            ),
+            name=vert.name + "_bnds",
+            attrs=vert.attrs.copy(),
+        )
 
     @staticmethod
     @docstrings.dedent
     def decode_coords(ds, gridfile=None):
         """
         Reimplemented to set the mesh variables as coordinates
 
@@ -1896,53 +2378,64 @@
         %(CFDecoder.decode_coords.parameters)s
 
         Returns
         -------
         %(CFDecoder.decode_coords.returns)s"""
         extra_coords = set(ds.coords)
         for var in six.itervalues(ds.variables):
-            if 'mesh' in var.attrs:
-                mesh = var.attrs['mesh']
+            if "mesh" in var.attrs:
+                mesh = var.attrs["mesh"]
                 if mesh not in extra_coords:
                     extra_coords.add(mesh)
                     try:
                         mesh_var = ds.variables[mesh]
                     except KeyError:
-                        warn('Could not find mesh variable %s' % mesh)
+                        warn("Could not find mesh variable %s" % mesh)
                         continue
-                    if 'node_coordinates' in mesh_var.attrs:
+                    if "node_coordinates" in mesh_var.attrs:
                         extra_coords.update(
-                            mesh_var.attrs['node_coordinates'].split())
-                    if 'face_node_connectivity' in mesh_var.attrs:
+                            mesh_var.attrs["node_coordinates"].split()
+                        )
+                    if "face_node_connectivity" in mesh_var.attrs:
                         extra_coords.add(
-                            mesh_var.attrs['face_node_connectivity'])
+                            mesh_var.attrs["face_node_connectivity"]
+                        )
         if gridfile is not None and not isinstance(gridfile, xr.Dataset):
             gridfile = open_dataset(gridfile)
-            ds.update({k: v for k, v in six.iteritems(gridfile.variables)
-                       if k in extra_coords})
+            ds.update(
+                {
+                    k: v
+                    for k, v in six.iteritems(gridfile.variables)
+                    if k in extra_coords
+                }
+            )
         if xr_version < (0, 11):
-            ds.set_coords(extra_coords.intersection(ds.variables),
-                          inplace=True)
+            ds.set_coords(
+                extra_coords.intersection(ds.variables), inplace=True
+            )
         else:
             ds._coord_names.update(extra_coords.intersection(ds.variables))
         return ds
 
     def get_nodes(self, coord, coords):
         """Get the variables containing the definition of the nodes
 
         Parameters
         ----------
         coord: xarray.Coordinate
             The mesh variable
         coords: dict
             The coordinates to use to get node coordinates"""
+
         def get_coord(coord):
             return coords.get(coord, self.ds.coords.get(coord))
-        return list(map(get_coord,
-                        coord.attrs.get('node_coordinates', '').split()[:2]))
+
+        return list(
+            map(get_coord, coord.attrs.get("node_coordinates", "").split()[:2])
+        )
 
     @docstrings.dedent
     def get_x(self, var, coords=None):
         """
         Get the centers of the triangles in the x-dimension
 
         Parameters
@@ -1954,17 +2447,20 @@
         %(CFDecoder.get_y.returns)s"""
         if coords is None:
             coords = self.ds.coords
         # first we try the super class
         ret = super(UGridDecoder, self).get_x(var, coords)
         # but if that doesn't work because we get the variable name in the
         # dimension of `var`, we use the means of the triangles
-        if ret is None or ret.name in var.dims or (hasattr(var, 'mesh') and
-                                                   ret.name == var.mesh):
-            bounds = self.get_cell_node_coord(var, axis='x', coords=coords)
+        if (
+            ret is None
+            or ret.name in var.dims
+            or (hasattr(var, "mesh") and ret.name == var.mesh)
+        ):
+            bounds = self.get_cell_node_coord(var, axis="x", coords=coords)
             if bounds is not None:
                 centers = bounds.mean(axis=-1)
                 x = self.get_nodes(self.get_mesh(var, coords), coords)[0]
                 try:
                     cls = xr.IndexVariable
                 except AttributeError:  # xarray < 0.9
                     cls = xr.Coordinate
@@ -1986,17 +2482,20 @@
         %(CFDecoder.get_y.returns)s"""
         if coords is None:
             coords = self.ds.coords
         # first we try the super class
         ret = super(UGridDecoder, self).get_y(var, coords)
         # but if that doesn't work because we get the variable name in the
         # dimension of `var`, we use the means of the triangles
-        if ret is None or ret.name in var.dims or (hasattr(var, 'mesh') and
-                                                   ret.name == var.mesh):
-            bounds = self.get_cell_node_coord(var, axis='y', coords=coords)
+        if (
+            ret is None
+            or ret.name in var.dims
+            or (hasattr(var, "mesh") and ret.name == var.mesh)
+        ):
+            bounds = self.get_cell_node_coord(var, axis="y", coords=coords)
             if bounds is not None:
                 centers = bounds.mean(axis=-1)
                 y = self.get_nodes(self.get_mesh(var, coords), coords)[1]
                 try:
                     cls = xr.IndexVariable
                 except AttributeError:  # xarray < 0.9
                     cls = xr.Coordinate
@@ -2004,25 +2503,33 @@
         else:
             return ret
 
 
 # register the UGridDecoder
 CFDecoder.register_decoder(UGridDecoder)
 
-docstrings.keep_params('CFDecoder.decode_coords.parameters', 'gridfile')
-docstrings.get_sections(inspect.cleandoc(
-    xr.open_dataset.__doc__.split('\n', 1)[1]),
-    'xarray.open_dataset')
-docstrings.delete_params('xarray.open_dataset.parameters', 'engine')
+docstrings.keep_params("CFDecoder.decode_coords.parameters", "gridfile")
+docstrings.get_sections(
+    inspect.cleandoc(xr.open_dataset.__doc__.split("\n", 1)[1]),
+    "xarray.open_dataset",
+)
+docstrings.delete_params("xarray.open_dataset.parameters", "engine")
 
 
-@docstrings.get_sections(base='open_dataset')
+@docstrings.get_sections(base="open_dataset")
 @docstrings.dedent
-def open_dataset(filename_or_obj, decode_cf=True, decode_times=True,
-                 decode_coords=True, engine=None, gridfile=None, **kwargs):
+def open_dataset(
+    filename_or_obj,
+    decode_cf=True,
+    decode_times=True,
+    decode_coords=True,
+    engine=None,
+    gridfile=None,
+    **kwargs,
+):
     """
     Open an instance of :class:`xarray.Dataset`.
 
     This method has the same functionality as the :func:`xarray.open_dataset`
     method except that is supports an additional 'gdal' engine to open
     gdal Rasters (e.g. GeoTiffs) and that is supports absolute time units like
     ``'day as %Y%m%d.%f'`` (if `decode_cf` and `decode_times` are True).
@@ -2039,49 +2546,67 @@
     Returns
     -------
     xarray.Dataset
         The dataset that contains the variables from `filename_or_obj`"""
     # use the absolute path name (is saver when saving the project)
     if isstring(filename_or_obj) and osp.exists(filename_or_obj):
         filename_or_obj = osp.abspath(filename_or_obj)
-    if engine == 'gdal':
+    if engine == "gdal":
         from psyplot.gdal_store import GdalStore
+
         filename_or_obj = GdalStore(filename_or_obj)
         engine = None
-    ds = xr.open_dataset(filename_or_obj, decode_cf=decode_cf,
-                         decode_coords=False, engine=engine,
-                         decode_times=decode_times, **kwargs)
+    ds = xr.open_dataset(
+        filename_or_obj,
+        decode_cf=decode_cf,
+        decode_coords=False,
+        engine=engine,
+        decode_times=decode_times,
+        **kwargs,
+    )
     if isstring(filename_or_obj):
         ds.psy.filename = filename_or_obj
     if decode_cf:
         ds = CFDecoder.decode_ds(
-            ds, decode_coords=decode_coords, decode_times=decode_times,
-            gridfile=gridfile)
+            ds,
+            decode_coords=decode_coords,
+            decode_times=decode_times,
+            gridfile=gridfile,
+        )
     return ds
 
 
 docstrings.get_sections(
-    inspect.cleandoc(xr.open_mfdataset.__doc__.split('\n', 1)[1]),
-    'xarray.open_mfdataset')
-docstrings.delete_params('xarray.open_mfdataset.parameters', 'engine')
-docstrings.keep_params('get_tdata.parameters', 't_format')
-
-docstrings.params['xarray.open_mfdataset.parameters.no_engine'] = \
-    docstrings.params['xarray.open_mfdataset.parameters.no_engine'].replace(
-        '**kwargs', '``**kwargs``').replace('"path/to/my/files/*.nc"',
-                                            '``"path/to/my/files/*.nc"``')
+    inspect.cleandoc(xr.open_mfdataset.__doc__.split("\n", 1)[1]),
+    "xarray.open_mfdataset",
+)
+docstrings.delete_params("xarray.open_mfdataset.parameters", "engine")
+docstrings.keep_params("get_tdata.parameters", "t_format")
+
+docstrings.params["xarray.open_mfdataset.parameters.no_engine"] = (
+    docstrings.params["xarray.open_mfdataset.parameters.no_engine"]
+    .replace("**kwargs", "``**kwargs``")
+    .replace('"path/to/my/files/*.nc"', '``"path/to/my/files/*.nc"``')
+)
 
 
-docstrings.keep_params('open_dataset.parameters', 'engine')
+docstrings.keep_params("open_dataset.parameters", "engine")
 
 
 @docstrings.dedent
-def open_mfdataset(paths, decode_cf=True, decode_times=True,
-                   decode_coords=True, engine=None, gridfile=None,
-                   t_format=None, **kwargs):
+def open_mfdataset(
+    paths,
+    decode_cf=True,
+    decode_times=True,
+    decode_coords=True,
+    engine=None,
+    gridfile=None,
+    t_format=None,
+    **kwargs,
+):
     """
     Open multiple files as a single dataset.
 
     This function is essentially the same as the :func:`xarray.open_mfdataset`
     function but (as the :func:`open_dataset`) supports additional decoding
     and the ``'gdal'`` engine.
     You can further specify the `t_format` parameter to get the time
@@ -2094,47 +2619,56 @@
     %(get_tdata.parameters.t_format)s
     %(CFDecoder.decode_coords.parameters.gridfile)s
 
     Returns
     -------
     xarray.Dataset
         The dataset that contains the variables from `filename_or_obj`"""
-    if t_format is not None or engine == 'gdal':
+    if t_format is not None or engine == "gdal":
         if isinstance(paths, six.string_types):
             paths = sorted(glob(paths))
         if not paths:
-            raise IOError('no files to open')
+            raise IOError("no files to open")
     if t_format is not None:
         time, paths = get_tdata(t_format, paths)
-        kwargs['concat_dim'] = 'time'
+        kwargs["concat_dim"] = "time"
         if xr_version > (0, 11):
-            kwargs['combine'] = 'nested'
+            kwargs["combine"] = "nested"
     if all(map(isstring, paths)):
         filenames = list(paths)
     else:
         filenames = None
-    if engine == 'gdal':
+    if engine == "gdal":
         from psyplot.gdal_store import GdalStore
+
         paths = list(map(GdalStore, paths))
         engine = None
         if xr_version < (0, 18):
-            kwargs['lock'] = False
+            kwargs["lock"] = False
 
     ds = xr.open_mfdataset(
-        paths, decode_cf=decode_cf, decode_times=decode_times, engine=engine,
-        decode_coords=False, **kwargs)
+        paths,
+        decode_cf=decode_cf,
+        decode_times=decode_times,
+        engine=engine,
+        decode_coords=False,
+        **kwargs,
+    )
     ds.psy.filename = filenames
     if decode_cf:
-        ds = CFDecoder.decode_ds(ds, gridfile=gridfile,
-                                 decode_coords=decode_coords,
-                                 decode_times=decode_times)
-    ds.psy._concat_dim = kwargs.get('concat_dim')
-    ds.psy._combine = kwargs.get('combine')
+        ds = CFDecoder.decode_ds(
+            ds,
+            gridfile=gridfile,
+            decode_coords=decode_coords,
+            decode_times=decode_times,
+        )
+    ds.psy._concat_dim = kwargs.get("concat_dim")
+    ds.psy._combine = kwargs.get("combine")
     if t_format is not None:
-        ds['time'] = time
+        ds["time"] = time
     return ds
 
 
 class InteractiveBase(object):
     """Class for the communication of a data object with a suitable plotter
 
     This class serves as an interface for data objects (in particular as a
@@ -2155,16 +2689,17 @@
     def plotter(self, value):
         self._plotter = value
 
     @plotter.deleter
     def plotter(self):
         self._plotter = None
 
-    no_auto_update = property(_no_auto_update_getter,
-                              doc=_no_auto_update_getter.__doc__)
+    no_auto_update = property(
+        _no_auto_update_getter, doc=_no_auto_update_getter.__doc__
+    )
 
     @property
     def plot(self):
         """An object to visualize this data object
 
         To make a 2D-plot with the :mod:`psy-simple <psy_simple.plugin>`
         plugin, you can just type
@@ -2177,14 +2712,15 @@
         extracted and visualized data.
 
         See Also
         --------
         psyplot.project.DataArrayPlotter: for the different plot methods"""
         if self._plot is None:
             import psyplot.project as psy
+
             self._plot = psy.DataArrayPlotter(self)
         return self._plot
 
     @no_auto_update.setter
     def no_auto_update(self, value):
         if self.plotter is not None:
             self.plotter.no_auto_update = value
@@ -2192,18 +2728,21 @@
 
     @property
     def logger(self):
         """:class:`logging.Logger` of this instance"""
         try:
             return self._logger
         except AttributeError:
-            name = '%s.%s.%s' % (self.__module__, self.__class__.__name__,
-                                 self.arr_name)
+            name = "%s.%s.%s" % (
+                self.__module__,
+                self.__class__.__name__,
+                self.arr_name,
+            )
             self._logger = logging.getLogger(name)
-            self.logger.debug('Initializing...')
+            self.logger.debug("Initializing...")
             return self._logger
 
     @logger.setter
     def logger(self, value):
         self._logger = value
 
     @property
@@ -2211,32 +2750,34 @@
         """The matplotlib axes the plotter of this data object plots on"""
         return None if self.plotter is None else self.plotter.ax
 
     @ax.setter
     def ax(self, value):
         if self.plotter is None:
             raise ValueError(
-                'Cannot set the axes because the plotter attribute is None!')
+                "Cannot set the axes because the plotter attribute is None!"
+            )
         self.plotter.ax = value
 
     block_signals = utils._temp_bool_prop(
-        'block_signals', "Block the emitting of signals of this instance")
+        "block_signals", "Block the emitting of signals of this instance"
+    )
 
     # -------------------------------------------------------------------------
     # -------------------------------- SIGNALS --------------------------------
     # -------------------------------------------------------------------------
 
     #: :class:`Signal` to be emitted when the object has been updated
-    onupdate = Signal('_onupdate')
+    onupdate = Signal("_onupdate")
     _onupdate = None
 
     _plotter = None
 
     @property
-    @docstrings.get_docstring(base='InteractiveBase._njobs')
+    @docstrings.get_docstring(base="InteractiveBase._njobs")
     @dedent
     def _njobs(self):
         """
         The number of jobs taken from the queue during an update process
 
         Returns
         -------
@@ -2260,17 +2801,17 @@
             pass
         self.onupdate.emit()
 
     _arr_name = None
 
     _no_auto_update = None
 
-    @docstrings.get_sections(base='InteractiveBase')
+    @docstrings.get_sections(base="InteractiveBase")
     @dedent
-    def __init__(self, plotter=None, arr_name='arr0', auto_update=None):
+    def __init__(self, plotter=None, arr_name="arr0", auto_update=None):
         """
         Parameters
         ----------
         plotter: Plotter
             Default: None. Interactive plotter that makes the plot via
             formatoption keywords.
         arr_name: str
@@ -2280,28 +2821,29 @@
             automatically update the contained arrays when calling the
             :meth:`update` method or not. See also the :attr:`no_auto_update`
             attribute. If None, the value from the ``'lists.auto_update'``
             key in the :attr:`psyplot.rcParams` dictionary is used."""
         self.plotter = plotter
         self.arr_name = arr_name
         if auto_update is None:
-            auto_update = rcParams['lists.auto_update']
+            auto_update = rcParams["lists.auto_update"]
         self.no_auto_update = not bool(auto_update)
         self.replot = False
 
     def _finish_all(self, queues):
         for n, queue in zip(safe_list(self._njobs), safe_list(queues)):
             if queue is not None:
                 for i in range(n):
                     queue.task_done()
 
-    @docstrings.get_sections(base='InteractiveBase._register_update')
+    @docstrings.get_sections(base="InteractiveBase._register_update")
     @dedent
-    def _register_update(self, replot=False, fmt={}, force=False,
-                         todefault=False):
+    def _register_update(
+        self, replot=False, fmt={}, force=False, todefault=False
+    ):
         """
         Register new formatoptions for updating
 
         Parameters
         ----------
         replot: bool
             Boolean that determines whether the data specific formatoptions
@@ -2322,19 +2864,21 @@
             :attr:`~psyplot.plotter.Plotter.rc` attribute
 
         See Also
         --------
         start_update"""
         self.replot = self.replot or replot
         if self.plotter is not None:
-            self.plotter._register_update(replot=self.replot, fmt=fmt,
-                                          force=force, todefault=todefault)
-
-    @docstrings.get_sections(base='InteractiveBase.start_update',
-                              sections=['Parameters', 'Returns'])
+            self.plotter._register_update(
+                replot=self.replot, fmt=fmt, force=force, todefault=todefault
+            )
+
+    @docstrings.get_sections(
+        base="InteractiveBase.start_update", sections=["Parameters", "Returns"]
+    )
     @dedent
     def start_update(self, draw=None, queues=None):
         """
         Conduct the formerly registered updates
 
         This method conducts the updates that have been registered via the
         :meth:`update` method. You can call this method if the
@@ -2364,21 +2908,30 @@
         See Also
         --------
         :attr:`no_auto_update`, update
         """
         if self.plotter is not None:
             return self.plotter.start_update(draw=draw, queues=queues)
 
-    docstrings.keep_params('InteractiveBase.start_update.parameters', 'draw')
+    docstrings.keep_params("InteractiveBase.start_update.parameters", "draw")
 
-    @docstrings.get_sections(base='InteractiveBase.update',
-                              sections=['Parameters', 'Notes'])
+    @docstrings.get_sections(
+        base="InteractiveBase.update", sections=["Parameters", "Notes"]
+    )
     @docstrings.dedent
-    def update(self, fmt={}, replot=False, draw=None, auto_update=False,
-               force=False, todefault=False, **kwargs):
+    def update(
+        self,
+        fmt={},
+        replot=False,
+        draw=None,
+        auto_update=False,
+        force=False,
+        todefault=False,
+        **kwargs,
+    ):
         """
         Update the coordinates and the plot
 
         This method updates all arrays in this list with the given coordinate
         values and formatoptions.
 
         Parameters
@@ -2400,57 +2953,63 @@
         registered and conducted at the next call of the :meth:`start_update`
         method or the next call of this method (if the `auto_update` parameter
         is then True).
         """
         fmt = dict(fmt)
         fmt.update(kwargs)
 
-        self._register_update(replot=replot, fmt=fmt, force=force,
-                              todefault=todefault)
+        self._register_update(
+            replot=replot, fmt=fmt, force=force, todefault=todefault
+        )
 
         if not self.no_auto_update or auto_update:
             self.start_update(draw=draw)
 
     def to_interactive_list(self):
         """Return a :class:`InteractiveList` that contains this object"""
-        raise NotImplementedError('Not implemented for the %s class' % (
-            self.__class__.__name__, ))
+        raise NotImplementedError(
+            "Not implemented for the %s class" % (self.__class__.__name__,)
+        )
 
 
-@xr.register_dataarray_accessor('psy')
+@xr.register_dataarray_accessor("psy")
 class InteractiveArray(InteractiveBase):
     """Interactive psyplot accessor for the data array
 
     This class keeps reference to the base :class:`xarray.Dataset` where the
     :class:`array.DataArray` originates from and enables to switch between the
     coordinates in the array. Furthermore it has a :attr:`plotter` attribute to
     enable interactive plotting via an :class:`psyplot.plotter.Plotter`
     instance."""
 
     @property
     def base(self):
         """Base dataset this instance gets its data from"""
         if self._base is None:
-            if 'variable' in self.arr.dims:
+            if "variable" in self.arr.dims:
+
                 def to_dataset(i):
                     ret = self.isel(variable=i).to_dataset(
-                        name=self.arr.coords['variable'].values[i])
+                        name=self.arr.coords["variable"].values[i]
+                    )
                     try:
-                        return ret.drop_vars('variable')
+                        return ret.drop_vars("variable")
                     except ValueError:  # 'variable' Variable not defined
                         pass
                     return ret
+
                 ds = to_dataset(0)
-                if len(self.arr.coords['variable']) > 1:
-                    for i in range(1, len(self.arr.coords['variable'])):
+                if len(self.arr.coords["variable"]) > 1:
+                    for i in range(1, len(self.arr.coords["variable"])):
                         ds.update(ds.merge(to_dataset(i)))
                 self._base = ds
             else:
                 self._base = self.arr.to_dataset(
-                    name=self.arr.name or self.arr_name)
+                    name=self.arr.name or self.arr_name
+                )
             self.onbasechange.emit()
         return self._base
 
     @base.setter
     def base(self, value):
         self._base = value
         self.onbasechange.emit()
@@ -2493,15 +3052,15 @@
 
     logger = InteractiveBase.logger
     _idims = None
     _base = None
 
     # -------------- SIGNALS --------------------------------------------------
     #: :class:`Signal` to be emiited when the base of the object changes
-    onbasechange = Signal('_onbasechange')
+    onbasechange = Signal("_onbasechange")
     _onbasechange = None
 
     @docstrings.dedent
     def __init__(self, xarray_obj, *args, **kwargs):
         """
         The ``*args`` and ``**kwargs`` are essentially the same as for the
         :class:`xarray.DataArray` method, additional ``**kwargs`` are
@@ -2524,16 +3083,17 @@
         """
         self.arr = xarray_obj
         super(InteractiveArray, self).__init__(*args, **kwargs)
         self._registered_updates = {}
         self._new_dims = {}
         self.method = None
 
-    def init_accessor(self, base=None, idims=None, decoder=None,
-                      *args, **kwargs):
+    def init_accessor(
+        self, base=None, idims=None, decoder=None, *args, **kwargs
+    ):
         """
         Initialize the accessor instance
 
         This method initializes the accessor
 
         Parameters
         ----------
@@ -2553,16 +3113,20 @@
             self.decoder = decoder
         super(InteractiveArray, self).__init__(*args, **kwargs)
 
     @property
     def iter_base_variables(self):
         """An iterator over the base variables in the :attr:`base` dataset"""
         if VARIABLELABEL in self.arr.coords:
-            return (self._get_base_var(name) for name in safe_list(
-                self.arr.coords[VARIABLELABEL].values.tolist()))
+            return (
+                self._get_base_var(name)
+                for name in safe_list(
+                    self.arr.coords[VARIABLELABEL].values.tolist()
+                )
+            )
         name = self.arr.name
         if name is None:
             return iter([self.arr._variable])
         return iter([self.base.variables[name]])
 
     def _get_base_var(self, name):
         try:
@@ -2571,29 +3135,41 @@
             return self.arr.sel(**{VARIABLELABEL: name}).rename(name)
 
     @property
     def base_variables(self):
         """A mapping from the variable name to the variablein the :attr:`base`
         dataset."""
         if VARIABLELABEL in self.arr.coords:
-            return OrderedDict([
-                (name, self._get_base_var(name)) for name in safe_list(
-                    self.arr.coords[VARIABLELABEL].values.tolist())])
+            return dict(
+                [
+                    (name, self._get_base_var(name))
+                    for name in safe_list(
+                        self.arr.coords[VARIABLELABEL].values.tolist()
+                    )
+                ]
+            )
         name = self.arr.name
         if name is None:
             return {name: self.arr._variable}
         else:
             return {self.arr.name: self.base.variables[self.arr.name]}
 
-    docstrings.keep_params('setup_coords.parameters', 'dims')
+    docstrings.keep_params("setup_coords.parameters", "dims")
 
-    @docstrings.get_sections(base='InteractiveArray._register_update')
+    @docstrings.get_sections(base="InteractiveArray._register_update")
     @docstrings.dedent
-    def _register_update(self, method='isel', replot=False, dims={}, fmt={},
-                         force=False, todefault=False):
+    def _register_update(
+        self,
+        method="isel",
+        replot=False,
+        dims={},
+        fmt={},
+        force=False,
+        todefault=False,
+    ):
         """
         Register new dimensions and formatoptions for updating
 
         Parameters
         ----------
         method: {'isel', None, 'nearest', ...}
             Selection method of the xarray.Dataset to be used for setting the
@@ -2606,30 +3182,35 @@
 
         See Also
         --------
         start_update"""
         if self._new_dims and self.method != method:
             raise ValueError(
                 "New dimensions were already specified for with the %s method!"
-                " I can not choose a new method %s" % (self.method, method))
+                " I can not choose a new method %s" % (self.method, method)
+            )
         else:
             self.method = method
-        if 'name' in dims:
-            self._new_dims['name'] = dims.pop('name')
-        if 'name' in self._new_dims:
-            name = self._new_dims['name']
+        if "name" in dims:
+            self._new_dims["name"] = dims.pop("name")
+        if "name" in self._new_dims:
+            name = self._new_dims["name"]
             if not isstring(name):
                 name = name[0]  # concatenated array
             arr = self.base[name]
         else:
-            arr= next(six.itervalues(self.base_variables))
+            arr = next(six.itervalues(self.base_variables))
         self._new_dims.update(self.decoder.correct_dims(arr, dims))
         InteractiveBase._register_update(
-            self, fmt=fmt, replot=replot or bool(self._new_dims), force=force,
-            todefault=todefault)
+            self,
+            fmt=fmt,
+            replot=replot or bool(self._new_dims),
+            force=force,
+            todefault=todefault,
+        )
 
     def _update_concatenated(self, dims, method):
         """Updates a concatenated array to new dimensions"""
 
         def is_unequal(v1, v2):
             try:
                 return bool(v1 != v2)
@@ -2637,55 +3218,59 @@
                 try:
                     (v1 == v2).all()
                 except AttributeError:
                     return False
 
         def filter_attrs(item):
             """Checks whether the attribute is from the base variable"""
-            return (item[0] not in self.base.attrs or
-                    is_unequal(item[1], self.base.attrs[item[0]]))
+            return item[0] not in self.base.attrs or is_unequal(
+                item[1], self.base.attrs[item[0]]
+            )
+
         saved_attrs = list(filter(filter_attrs, six.iteritems(self.arr.attrs)))
         saved_name = self.arr.name
-        self.arr.name = 'None'
-        if 'name' in dims:
-            name = dims.pop('name')
+        self.arr.name = "None"
+        if "name" in dims:
+            name = dims.pop("name")
         else:
-            name = list(self.arr.coords['variable'].values)
+            name = list(self.arr.coords["variable"].values)
         base_dims = self.base[name].dims
-        if method == 'isel':
+        if method == "isel":
             self.idims.update(dims)
             dims = self.idims
             for dim in set(base_dims) - set(dims):
                 dims[dim] = slice(None)
             for dim in set(dims) - set(self.base[name].dims):
                 del dims[dim]
             res = self.base[name].isel(**dims).to_array()
         else:
             self._idims = None
             for key, val in six.iteritems(self.arr.coords):
-                if key in base_dims and key != 'variable':
+                if key in base_dims and key != "variable":
                     dims.setdefault(key, val)
             kws = dims.copy()
             # the sel method does not work with slice objects
             if not any(isinstance(idx, slice) for idx in dims.values()):
-                kws['method'] = method
+                kws["method"] = method
             try:
                 res = self.base[name].sel(**kws)
             except KeyError:
                 _fix_times(kws)
                 res = self.base[name].sel(**kws)
             res = res.to_array()
-        if 'coordinates' in self.base[name[0]].encoding:
-            res.encoding['coordinates'] = self.base[name[0]].encoding[
-                'coordinates']
+        if "coordinates" in self.base[name[0]].encoding:
+            res.encoding["coordinates"] = self.base[name[0]].encoding[
+                "coordinates"
+            ]
         self.arr._variable = res._variable
         self.arr._coords = res._coords
         try:
             self.arr._indexes = (
-                res._indexes.copy() if res._indexes is not None else None)
+                res._indexes.copy() if res._indexes is not None else None
+            )
         except AttributeError:  # res.indexes not existent for xr<0.12
             pass
         self.arr.name = saved_name
         for key, val in saved_attrs:
             self.arr.attrs[key] = val
 
     def _update_array(self, dims, method):
@@ -2698,26 +3283,27 @@
                 try:
                     (v1 == v2).all()
                 except AttributeError:
                     return False
 
         def filter_attrs(item):
             """Checks whether the attribute is from the base variable"""
-            return (item[0] not in base_var.attrs or
-                    is_unequal(item[1], base_var.attrs[item[0]]))
+            return item[0] not in base_var.attrs or is_unequal(
+                item[1], base_var.attrs[item[0]]
+            )
 
         base_var = self.base.variables[self.arr.name]
-        if 'name' in dims:
-            name = dims.pop('name')
+        if "name" in dims:
+            name = dims.pop("name")
             self.arr.name = name
         else:
             name = self.arr.name
         # save attributes that have been changed by the user
         saved_attrs = list(filter(filter_attrs, six.iteritems(self.arr.attrs)))
-        if method == 'isel':
+        if method == "isel":
             self.idims.update(dims)
             dims = self.idims
             for dim in set(self.base[name].dims) - set(dims):
                 dims[dim] = slice(None)
             for dim in set(dims) - set(self.base[name].dims):
                 del dims[dim]
             res = self.base[name].isel(**dims)
@@ -2726,29 +3312,34 @@
             old_dims = self.arr.dims[:]
             for key, val in six.iteritems(self.arr.coords):
                 if key in base_var.dims:
                     dims.setdefault(key, val)
             kws = dims.copy()
             # the sel method does not work with slice objects
             if not any(isinstance(idx, slice) for idx in dims.values()):
-                kws['method'] = method
+                kws["method"] = method
             try:
                 res = self.base[name].sel(**kws)
             except KeyError:
                 _fix_times(kws)
                 res = self.base[name].sel(**kws)
             # squeeze the 0-dimensional dimensions
-            res = res.isel(**{
-                dim: 0 for i, dim in enumerate(res.dims) if (
-                    res.shape[i] == 1 and dim not in old_dims)})
+            res = res.isel(
+                **{
+                    dim: 0
+                    for i, dim in enumerate(res.dims)
+                    if (res.shape[i] == 1 and dim not in old_dims)
+                }
+            )
         self.arr._variable = res._variable
         self.arr._coords = res._coords
         try:
             self.arr._indexes = (
-                res._indexes.copy() if res._indexes is not None else None)
+                res._indexes.copy() if res._indexes is not None else None
+            )
         except AttributeError:  # res.indexes not existent for xr<0.12
             pass
         # update to old attributes
         for key, val in saved_attrs:
             self.arr.attrs[key] = val
 
     def shiftlon(self, central_longitude):
@@ -2767,74 +3358,81 @@
         ----------
         This function is copied and taken from the
         :class:`mpl_toolkits.basemap.Basemap` class. The only difference is
         that we do not mask values outside the map projection region
         """
         if xr_version < (0, 10):
             raise NotImplementedError(
-                "xarray>=0.10 is required for the shiftlon method!")
+                "xarray>=0.10 is required for the shiftlon method!"
+            )
         arr = self.arr
         ret = arr.copy(True, arr.values.copy())
         if arr.ndim > 2:
-            xname = self.get_dim('x')
-            yname = self.get_dim('y')
-            shapes = OrderedDict(
-                [(dim, range(i)) for dim, i in zip(arr.dims, arr.shape)
-                 if dim not in [xname, yname]])
+            xname = self.get_dim("x")
+            yname = self.get_dim("y")
+            shapes = dict(
+                [
+                    (dim, range(i))
+                    for dim, i in zip(arr.dims, arr.shape)
+                    if dim not in [xname, yname]
+                ]
+            )
             dims = list(shapes)
             for indexes in product(*shapes.values()):
                 d = dict(zip(dims, indexes))
                 shifted = ret[d].psy.shiftlon(central_longitude)
                 ret[d] = shifted.values
 
-            x = shifted.psy.get_coord('x')
+            x = shifted.psy.get_coord("x")
             ret[x.name] = shifted[x.name].variable
 
             return ret
 
-        lon = self.get_coord('x').variable
-        xname = self.get_dim('x')
+        lon = self.get_coord("x").variable
+        xname = self.get_dim("x")
         ix = arr.dims.index(xname)
         lon = lon.copy(True, lon.values.copy())
         lonsin = lon.values
         datain = arr.values.copy()
 
         clon = np.asarray(central_longitude)
 
         if lonsin.ndim not in [1]:
-            raise ValueError('1D longitudes required')
+            raise ValueError("1D longitudes required")
         elif clon.ndim:
-            raise ValueError("Central longitude must be a scalar, not "
-                             "%i-dimensional!" % clon.ndim)
-
-        lonsin = np.where(lonsin > clon+180, lonsin-360, lonsin)
-        lonsin = np.where(lonsin < clon-180, lonsin+360, lonsin)
-        londiff = np.abs(lonsin[0:-1]-lonsin[1:])
+            raise ValueError(
+                "Central longitude must be a scalar, not "
+                "%i-dimensional!" % clon.ndim
+            )
+
+        lonsin = np.where(lonsin > clon + 180, lonsin - 360, lonsin)
+        lonsin = np.where(lonsin < clon - 180, lonsin + 360, lonsin)
+        londiff = np.abs(lonsin[0:-1] - lonsin[1:])
         londiff_sort = np.sort(londiff)
-        thresh = 360.-londiff_sort[-2]
+        thresh = 360.0 - londiff_sort[-2]
         itemindex = len(lonsin) - np.where(londiff >= thresh)[0]
         if itemindex.size:
             # check to see if cyclic (wraparound) point included
             # if so, remove it.
-            if np.abs(lonsin[0]-lonsin[-1]) < 1.e-4:
+            if np.abs(lonsin[0] - lonsin[-1]) < 1.0e-4:
                 hascyclic = True
                 lonsin_save = lonsin.copy()
                 lonsin = lonsin[1:]
                 if datain is not None:
                     datain_save = datain.copy()
                     datain = datain[1:]
             else:
                 hascyclic = False
-            lonsin = np.roll(lonsin, itemindex-1)
+            lonsin = np.roll(lonsin, itemindex - 1)
             if datain is not None:
-                datain = np.roll(datain, itemindex-1, [ix])
+                datain = np.roll(datain, itemindex - 1, [ix])
             # add cyclic point back at beginning.
             if hascyclic:
                 lonsin_save[1:] = lonsin
-                lonsin_save[0] = lonsin[-1]-360.
+                lonsin_save[0] = lonsin[-1] - 360.0
                 lonsin = lonsin_save
                 if datain is not None:
                     datain_save[1:] = datain
                     datain_save[0] = datain[-1]
                     datain = datain_save
         ret = ret.copy(True, datain)
         lon.values[:] = lonsin
@@ -2860,43 +3458,58 @@
         -------
         %(InteractiveBase.start_update.returns)s
 
         See Also
         --------
         :attr:`no_auto_update`, update
         """
+
         def filter_attrs(item):
-            return (item[0] not in self.base.attrs or
-                    item[1] != self.base.attrs[item[0]])
+            return (
+                item[0] not in self.base.attrs
+                or item[1] != self.base.attrs[item[0]]
+            )
+
         if queues is not None:
             # make sure that no plot is updated during gathering the data
             queues[0].get()
         try:
             dims = self._new_dims
             method = self.method
             if dims:
+                self.decoder.clear_cache()
                 if VARIABLELABEL in self.arr.coords:
                     self._update_concatenated(dims, method)
                 else:
                     self._update_array(dims, method)
             if queues is not None:
                 queues[0].task_done()
             self._new_dims = {}
             self.onupdate.emit()
         except Exception:
             self._finish_all(queues)
             raise
         return InteractiveBase.start_update(self, draw=draw, queues=queues)
 
-    @docstrings.get_sections(base='InteractiveArray.update',
-                              sections=['Parameters', 'Notes'])
+    @docstrings.get_sections(
+        base="InteractiveArray.update", sections=["Parameters", "Notes"]
+    )
     @docstrings.dedent
-    def update(self, method='isel', dims={}, fmt={}, replot=False,
-               auto_update=False, draw=None, force=False, todefault=False,
-               **kwargs):
+    def update(
+        self,
+        method="isel",
+        dims={},
+        fmt={},
+        replot=False,
+        auto_update=False,
+        draw=None,
+        force=False,
+        todefault=False,
+        **kwargs,
+    ):
         """
         Update the coordinates and the plot
 
         This method updates all arrays in this list with the given coordinate
         values and formatoptions.
 
         Parameters
@@ -2919,57 +3532,80 @@
             da.psy.update(name='new_name', dims={'new_dim': 3})
 
         if ``'new_dim'`` is not yet a dimension of this array
 
         %(InteractiveBase.update.notes)s"""
         dims = dict(dims)
         fmt = dict(fmt)
-        vars_and_coords = set(chain(
-            self.arr.dims, self.arr.coords, ['name', 'x', 'y', 'z', 't']))
+        vars_and_coords = set(
+            chain(self.arr.dims, self.arr.coords, ["name", "x", "y", "z", "t"])
+        )
         furtherdims, furtherfmt = utils.sort_kwargs(kwargs, vars_and_coords)
         dims.update(furtherdims)
         fmt.update(furtherfmt)
 
-        self._register_update(method=method, replot=replot, dims=dims,
-                              fmt=fmt, force=force, todefault=todefault)
+        self._register_update(
+            method=method,
+            replot=replot,
+            dims=dims,
+            fmt=fmt,
+            force=force,
+            todefault=todefault,
+        )
 
         if not self.no_auto_update or auto_update:
             self.start_update(draw=draw)
 
     def _short_info(self, intend=0, maybe=False):
-        str_intend = ' ' * intend
-        if 'variable' in self.arr.coords:
-            name = ', '.join(self.arr.coords['variable'].values)
+        str_intend = " " * intend
+        if "variable" in self.arr.coords:
+            name = ", ".join(self.arr.coords["variable"].values)
         else:
             name = self.arr.name
         if self.arr.ndim > 0:
-            dims = ', with (%s)=%s' % (', '.join(self.arr.dims),
-                                       self.arr.shape)
+            dims = ", with (%s)=%s" % (
+                ", ".join(self.arr.dims),
+                self.arr.shape,
+            )
         else:
-            dims = ''
+            dims = ""
         return str_intend + "%s: %i-dim %s of %s%s, %s" % (
-            self.arr_name, self.arr.ndim, self.arr.__class__.__name__, name,
-            dims, ", ".join(
+            self.arr_name,
+            self.arr.ndim,
+            self.arr.__class__.__name__,
+            name,
+            dims,
+            ", ".join(
                 "%s=%s" % (coord, format_item(val.values))
                 for coord, val in six.iteritems(self.arr.coords)
-                if val.ndim == 0))
+                if val.ndim == 0
+            ),
+        )
 
     def __getitem__(self, key):
         ret = self.arr.__getitem__(key)
         ret.psy._base = self.base
         return ret
 
     def isel(self, *args, **kwargs):
-        # reimplemented to keep the base. The doc is set below
+        """Select a subset of the array based on position.
+
+        Same method as :meth:`xarray.DataArray.isel` but keeps information on
+        the base dataset.
+        """
         ret = self.arr.isel(*args, **kwargs)
         ret.psy._base = self._base
         return ret
 
     def sel(self, *args, **kwargs):
-        # reimplemented to keep the base. The doc is set below
+        """Select a subset of the array based on indexes.
+
+        Same method as :meth:`xarray.DataArray.sel` but keeps information on
+        the base dataset.
+        """
         ret = self.arr.sel(*args, **kwargs)
         ret.psy._base = self._base
         return ret
 
     def copy(self, deep=False):
         """Copy the array
 
@@ -2981,85 +3617,93 @@
         except AttributeError:  # attribute is read-only for xarray >=0.13
             pass
         return arr
 
     def to_interactive_list(self):
         return InteractiveList([self], arr_name=self.arr_name)
 
-    @docstrings.get_sections(base='InteractiveArray.get_coord')
+    @docstrings.get_sections(base="InteractiveArray.get_coord")
     @docstrings.dedent
     def get_coord(self, what, base=False):
         """
         The x-coordinate of this data array
 
         Parameters
         ----------
         what: {'t', 'x', 'y', 'z'}
             The letter of the axis
         base: bool
             If True, use the base variable in the :attr:`base` dataset."""
         what = what.lower()
-        return getattr(self.decoder, 'get_' + what)(
+        return getattr(self.decoder, "get_" + what)(
             next(six.itervalues(self.base_variables)) if base else self.arr,
-            self.arr.coords)
+            self.arr.coords,
+        )
 
     @docstrings.dedent
     def get_dim(self, what, base=False):
         """
         The name of the x-dimension of this data array
 
         Parameters
         ----------
         %(InteractiveArray.get_coord.parameters)s"""
         what = what.lower()
-        return getattr(self.decoder, 'get_%sname' % what)(
-            next(six.itervalues(self.base_variables)) if base else self.arr)
+        return getattr(self.decoder, "get_%sname" % what)(
+            next(six.itervalues(self.base_variables)) if base else self.arr
+        )
 
     # ------------------ Calculations -----------------------------------------
 
     def _gridweights(self):
         """Calculate the gridweights with a simple rectangular approximation"""
         arr = self.arr
-        xcoord = self.get_coord('x')
-        ycoord = self.get_coord('y')
+        xcoord = self.get_coord("x")
+        ycoord = self.get_coord("y")
         # convert the units
         xcoord_orig = xcoord
         ycoord_orig = ycoord
-        units = xcoord.attrs.get('units', '')
+        units = xcoord.attrs.get("units", "")
         in_metres = False
         in_degree = False
-        if 'deg' in units or (
-                'rad' not in units and 'lon' in xcoord.name and
-                'lat' in ycoord.name):
+        if "deg" in units or (
+            "rad" not in units
+            and "lon" in xcoord.name
+            and "lat" in ycoord.name
+        ):
             xcoord = xcoord * np.pi / 180
             ycoord = ycoord * np.pi / 180
             in_degree = True
-        elif 'rad' in units:
+        elif "rad" in units:
             pass
         else:
             in_metres = True
 
         # calculate the gridcell boundaries
         xbounds = self.decoder.get_plotbounds(xcoord, arr.coords)
         ybounds = self.decoder.get_plotbounds(ycoord, arr.coords)
         if xbounds.ndim == 1:
             xbounds, ybounds = np.meshgrid(xbounds, ybounds)
 
         # calculate the weights based on the units
         if xcoord.ndim == 2 or self.decoder.is_unstructured(self.arr):
-            warn("[%s] - Curvilinear grids are not supported! "
-                 "Using constant grid cell area weights!" % self.logger.name,
-                 PsyPlotRuntimeWarning)
+            warn(
+                "[%s] - Curvilinear grids are not supported! "
+                "Using constant grid cell area weights!" % self.logger.name,
+                PsyPlotRuntimeWarning,
+            )
             weights = np.ones_like(xcoord.values)
         elif in_metres:
             weights = np.abs(xbounds[:-1, :-1] - xbounds[1:, 1:]) * (
-                np.abs(ybounds[:-1, :-1] - ybounds[1:, 1:]))
+                np.abs(ybounds[:-1, :-1] - ybounds[1:, 1:])
+            )
         else:
             weights = np.abs(xbounds[:-1, :-1] - xbounds[1:, 1:]) * (
-                np.sin(ybounds[:-1, :-1]) - np.sin(ybounds[1:, 1:]))
+                np.sin(ybounds[:-1, :-1]) - np.sin(ybounds[1:, 1:])
+            )
 
         # normalize the weights by dividing through the sum
         if in_degree:
             xmask = (xcoord_orig.values < -400) | (xcoord_orig.values > 400)
             ymask = (ycoord_orig.values < -200) | (ycoord_orig.values > 200)
             if xmask.any() or ymask.any():
                 if xmask.ndim == 1 and weights.ndim != 1:
@@ -3067,51 +3711,56 @@
                 weights[xmask | ymask] = np.nan
         if np.any(~np.isnan(weights)):
             weights /= np.nansum(weights)
         return weights
 
     def _gridweights_cdo(self):
         """Estimate the gridweights using CDOs"""
-        from cdo import Cdo
         from tempfile import NamedTemporaryFile
-        sdims = {self.get_dim('y'), self.get_dim('x')}
+
+        from cdo import Cdo
+
+        sdims = {self.get_dim("y"), self.get_dim("x")}
         cdo = Cdo()
-        fname = NamedTemporaryFile(prefix='psy', suffix='.nc').name
+        fname = NamedTemporaryFile(prefix="psy", suffix=".nc").name
         arr = self.arr
         base = arr.psy.base
         dims = arr.dims
         ds = arr.isel(**{d: 0 for d in set(dims) - sdims}).to_dataset()
         for coord in six.itervalues(ds.coords):
-            bounds = coord.attrs.get('bounds', coord.encoding.get('bounds'))
-            if (bounds and bounds in set(base.coords) - set(ds.coords) and
-                    sdims.intersection(base.coords[bounds].dims)):
+            bounds = coord.attrs.get("bounds", coord.encoding.get("bounds"))
+            if (
+                bounds
+                and bounds in set(base.coords) - set(ds.coords)
+                and sdims.intersection(base.coords[bounds].dims)
+            ):
                 ds[bounds] = base.sel(
                     **{d: arr.coords[d].values for d in sdims}
-                    ).coords[bounds]
-            ds = ds.drop_vars([c.name for c in six.itervalues(ds.coords)
-                               if not c.ndim])
+                ).coords[bounds]
+            ds = ds.drop_vars(
+                [c.name for c in six.itervalues(ds.coords) if not c.ndim]
+            )
         to_netcdf(ds, fname)
-        ret = cdo.gridweights(input=fname, returnArray='cell_weights')
+        ret = cdo.gridweights(input=fname, returnArray="cell_weights")
         try:
             os.remove(fname)
         except Exception:
             pass
         return ret
 
     def _weights_to_da(self, weights, keepdims=False, keepshape=False):
-        """Convert the 2D weights into a DataArray and potentially enlarge it
-        """
+        """Convert the 2D weights into a DataArray and potentially enlarge it"""
         arr = self.arr
-        xcoord = self.get_coord('x')
-        ycoord = self.get_coord('y')
-        sdims = (self.get_dim('y'), self.get_dim('x'))
-        if sdims[0] == sdims[1]:   # unstructured grids
+        xcoord = self.get_coord("x")
+        ycoord = self.get_coord("y")
+        sdims = (self.get_dim("y"), self.get_dim("x"))
+        if sdims[0] == sdims[1]:  # unstructured grids
             sdims = sdims[:1]
         if (ycoord.name, xcoord.name) != sdims:
-            attrs = dict(coordinates=ycoord.name + ' ' + xcoord.name)
+            attrs = dict(coordinates=ycoord.name + " " + xcoord.name)
         else:
             attrs = {}
 
         # reshape and expand if necessary
         if not keepdims and not keepshape:
             coords = {ycoord.name: ycoord, xcoord.name: xcoord}
             dims = sdims
@@ -3139,21 +3788,25 @@
                 summed_weights = weights.sum(
                     axis=tuple(map(dims.index, sdims))
                 )
             weights = weights / summed_weights
         else:
             dims = arr.dims
             coords = arr.isel(
-                **{d: 0 if d not in sdims else slice(None)
-                   for d in dims}).coords
+                **{d: 0 if d not in sdims else slice(None) for d in dims}
+            ).coords
             weights = weights.reshape(
-                tuple(1 if dim not in sdims else s
-                      for s, dim in zip(arr.shape, arr.dims)))
-        return xr.DataArray(weights, dims=dims, coords=coords,
-                            name='cell_weights', attrs=attrs)
+                tuple(
+                    1 if dim not in sdims else s
+                    for s, dim in zip(arr.shape, arr.dims)
+                )
+            )
+        return xr.DataArray(
+            weights, dims=dims, coords=coords, name="cell_weights", attrs=attrs
+        )
 
     def gridweights(self, keepdims=False, keepshape=False, use_cdo=None):
         """Calculate the cell weights for each grid cell
 
         Parameters
         ----------
         keepdims: bool
@@ -3168,56 +3821,59 @@
             item in the :attr:`psyplot.rcParams`.
 
         Returns
         -------
         xarray.DataArray
             The 2D-DataArray with the grid weights"""
         if use_cdo is None:
-            use_cdo = rcParams['gridweights.use_cdo']
+            use_cdo = rcParams["gridweights.use_cdo"]
         if not use_cdo and self.decoder.is_unstructured(self.arr):
             use_cdo = True
         if use_cdo is None or use_cdo:
             try:
                 weights = self._gridweights_cdo()
             except Exception:
                 if use_cdo:
                     raise
                 else:
                     weights = self._gridweights()
         else:
             weights = self._gridweights()
 
-        return self._weights_to_da(weights, keepdims=keepdims,
-                                   keepshape=keepshape)
+        return self._weights_to_da(
+            weights, keepdims=keepdims, keepshape=keepshape
+        )
 
     def _fldaverage_args(self):
         """Masked array, xname, yname and axis for calculating the average"""
         arr = self.arr
-        sdims = (self.get_dim('y'), self.get_dim('x'))
+        sdims = (self.get_dim("y"), self.get_dim("x"))
         if sdims[0] == sdims[1]:
             sdims = sdims[:1]
         axis = tuple(map(arr.dims.index, sdims))
         return arr, sdims, axis
 
     def _insert_fldmean_bounds(self, da, keepdims=False):
-        xcoord = self.get_coord('x')
-        ycoord = self.get_coord('y')
-        sdims = (self.get_dim('y'), self.get_dim('x'))
+        xcoord = self.get_coord("x")
+        ycoord = self.get_coord("y")
+        sdims = (self.get_dim("y"), self.get_dim("x"))
         xbounds = np.array([[xcoord.min(), xcoord.max()]])
         ybounds = np.array([[ycoord.min(), ycoord.max()]])
-        xdims = (sdims[-1], 'bnds') if keepdims else ('bnds', )
-        ydims = (sdims[0], 'bnds') if keepdims else ('bnds', )
+        xdims = (sdims[-1], "bnds") if keepdims else ("bnds",)
+        ydims = (sdims[0], "bnds") if keepdims else ("bnds",)
         xattrs = xcoord.attrs.copy()
-        xattrs.pop('bounds', None)
+        xattrs.pop("bounds", None)
         yattrs = ycoord.attrs.copy()
-        yattrs.pop('bounds', None)
-        da.psy.base.coords[xcoord.name + '_bnds'] = xr.Variable(
-            xdims, xbounds if keepdims else xbounds[0], attrs=xattrs)
-        da.psy.base.coords[ycoord.name + '_bnds'] = xr.Variable(
-            ydims, ybounds if keepdims else ybounds[0], attrs=yattrs)
+        yattrs.pop("bounds", None)
+        da.psy.base.coords[xcoord.name + "_bnds"] = xr.Variable(
+            xdims, xbounds if keepdims else xbounds[0], attrs=xattrs
+        )
+        da.psy.base.coords[ycoord.name + "_bnds"] = xr.Variable(
+            ydims, ybounds if keepdims else ybounds[0], attrs=yattrs
+        )
 
     def fldmean(self, keepdims=False):
         """Calculate the weighted mean over the x- and y-dimension
 
         This method calculates the weighted mean of the spatial dimensions.
         Weights are calculated using the :meth:`gridweights` method, missing
         values are ignored. x- and y-dimensions are identified using the
@@ -3240,31 +3896,34 @@
         --------
         fldstd: For calculating the weighted standard deviation
         fldpctl: For calculating weighted percentiles
         """
         gridweights = self.gridweights()
         arr, sdims, axis = self._fldaverage_args()
 
-        xcoord = self.decoder.get_x(next(six.itervalues(self.base_variables)),
-                                    arr.coords)
-        ycoord = self.decoder.get_y(next(six.itervalues(self.base_variables)),
-                                    arr.coords)
+        xcoord = self.decoder.get_x(
+            next(six.itervalues(self.base_variables)), arr.coords
+        )
+        ycoord = self.decoder.get_y(
+            next(six.itervalues(self.base_variables)), arr.coords
+        )
         means = ((arr * gridweights)).sum(axis=axis) * (
-            gridweights.size / arr.notnull().sum(axis=axis))
+            gridweights.size / arr.notnull().sum(axis=axis)
+        )
         if keepdims:
             means = means.expand_dims(sdims, axis=axis)
 
         if keepdims:
             means[xcoord.name] = xcoord.mean().expand_dims(xcoord.dims[0])
             means[ycoord.name] = ycoord.mean().expand_dims(ycoord.dims[0])
         else:
             means[xcoord.name] = xcoord.mean()
             means[ycoord.name] = ycoord.mean()
-        means.coords[xcoord.name].attrs['bounds'] = xcoord.name + '_bnds'
-        means.coords[ycoord.name].attrs['bounds'] = ycoord.name + '_bnds'
+        means.coords[xcoord.name].attrs["bounds"] = xcoord.name + "_bnds"
+        means.coords[ycoord.name].attrs["bounds"] = ycoord.name + "_bnds"
         self._insert_fldmean_bounds(means, keepdims)
         means.name = arr.name
         return means
 
     def fldstd(self, keepdims=False):
         """Calculate the weighted standard deviation over x- and y-dimension
 
@@ -3290,27 +3949,33 @@
         --------
         fldmean: For calculating the weighted mean
         fldpctl: For calculating weighted percentiles
         """
         arr, sdims, axis = self._fldaverage_args()
         means = self.fldmean(keepdims=True)
         weights = self.gridweights(keepshape=True)
-        variance = ((arr - means.values)**2 * weights).sum(axis=axis)
+        variance = ((arr - means.values) ** 2 * weights).sum(axis=axis)
         if keepdims:
             variance = variance.expand_dims(sdims, axis=axis)
         for key, coord in six.iteritems(means.coords):
             if key not in variance.coords:
                 dims = set(sdims).intersection(coord.dims)
-                variance[key] = coord if keepdims else coord.isel(
-                    **dict(zip(dims, repeat(0))))
+                variance[key] = (
+                    coord
+                    if keepdims
+                    else coord.isel(**dict(zip(dims, repeat(0))))
+                )
         for key, coord in six.iteritems(means.psy.base.coords):
             if key not in variance.psy.base.coords:
                 dims = set(sdims).intersection(coord.dims)
-                variance.psy.base[key] = coord if keepdims else coord.isel(
-                    **dict(zip(dims, repeat(0))))
+                variance.psy.base[key] = (
+                    coord
+                    if keepdims
+                    else coord.isel(**dict(zip(dims, repeat(0))))
+                )
         std = variance**0.5
         std.name = arr.name
         return std
 
     def fldpctl(self, q, keepdims=False):
         """Calculate the percentiles along the x- and y-dimensions
 
@@ -3343,133 +4008,152 @@
         Warnings
         --------
         This method does load the entire array into memory! So take care if you
         handle big data."""
         gridweights = self.gridweights(keepshape=True)
         arr = self.arr
 
-        q = np.asarray(q) / 100.
+        q = np.asarray(q) / 100.0
         if not (np.all(q >= 0) and np.all(q <= 100)):
-            raise ValueError('q should be in [0, 100]')
+            raise ValueError("q should be in [0, 100]")
         reduce_shape = False if keepdims else (not bool(q.ndim))
         if not q.ndim:
             q = q[np.newaxis]
         data = arr.values.copy()
         sdims, axis = self._fldaverage_args()[1:]
         weights = gridweights.values
         # flatten along the spatial axis
         for ax in axis:
             data = np.rollaxis(data, ax, 0)
             weights = np.rollaxis(weights, ax, 0)
         data = data.reshape(
-            (np.product(data.shape[:len(axis)]), ) + data.shape[len(axis):])
+            (np.product(data.shape[: len(axis)]),) + data.shape[len(axis) :]
+        )
         weights = weights.reshape(
-            (np.product(weights.shape[:len(axis)]), ) +
-            weights.shape[len(axis):])
+            (np.product(weights.shape[: len(axis)]),)
+            + weights.shape[len(axis) :]
+        )
 
         # sort the data
         sorter = np.argsort(data, axis=0)
         all_indices = map(tuple, product(*map(range, data.shape[1:])))
         for indices in all_indices:
-            indices = (slice(None), ) + indices
+            indices = (slice(None),) + indices
             data.__setitem__(
-                indices, data.__getitem__(indices)[
-                    sorter.__getitem__(indices)])
+                indices, data.__getitem__(indices)[sorter.__getitem__(indices)]
+            )
             weights.__setitem__(
-                indices, weights.__getitem__(indices)[
-                    sorter.__getitem__(indices)])
+                indices,
+                weights.__getitem__(indices)[sorter.__getitem__(indices)],
+            )
 
         # compute the percentiles
         try:
             weights = np.nancumsum(weights, axis=0) - 0.5 * weights
         except AttributeError:
             notnull = ~np.isnan(weights)
             weights[notnull] = np.cumsum(weights[notnull])
         all_indices = map(tuple, product(*map(range, data.shape[1:])))
-        pctl = np.zeros((len(q), ) + data.shape[1:])
+        pctl = np.zeros((len(q),) + data.shape[1:])
 
         for indices in all_indices:
-            indices = (slice(None), ) + indices
+            indices = (slice(None),) + indices
             mask = ~np.isnan(data.__getitem__(indices))
-            pctl.__setitem__(indices, np.interp(
-                q, weights.__getitem__(indices)[mask],
-                data.__getitem__(indices)[mask]))
+            pctl.__setitem__(
+                indices,
+                np.interp(
+                    q,
+                    weights.__getitem__(indices)[mask],
+                    data.__getitem__(indices)[mask],
+                ),
+            )
 
         # setup the data array and it's coordinates
-        xcoord = self.decoder.get_x(next(six.itervalues(self.base_variables)),
-                                    arr.coords)
-        ycoord = self.decoder.get_y(next(six.itervalues(self.base_variables)),
-                                    arr.coords)
+        xcoord = self.decoder.get_x(
+            next(six.itervalues(self.base_variables)), arr.coords
+        )
+        ycoord = self.decoder.get_y(
+            next(six.itervalues(self.base_variables)), arr.coords
+        )
         coords = dict(arr.coords)
         if keepdims:
             pctl = pctl.reshape(
-                (len(q), ) +
-                tuple(1 if i in axis else s for i, s in enumerate(arr.shape)))
+                (len(q),)
+                + tuple(1 if i in axis else s for i, s in enumerate(arr.shape))
+            )
             coords[xcoord.name] = xcoord.mean().expand_dims(xcoord.dims[0])
             coords[ycoord.name] = ycoord.mean().expand_dims(ycoord.dims[0])
             dims = arr.dims
         else:
             coords[xcoord.name] = xcoord.mean()
             coords[ycoord.name] = ycoord.mean()
             dims = tuple(d for d in arr.dims if d not in sdims)
         if reduce_shape:
             pctl = pctl[0]
-            coords['pctl'] = xr.Variable((), q[0] * 100.,
-                                         attrs={'long_name': 'Percentile'})
-        else:
-            coords['pctl'] = xr.Variable(('pctl', ), q * 100.,
-                                         attrs={'long_name': 'Percentile'})
-            dims = ('pctl', ) + dims
-        coords[xcoord.name].attrs['bounds'] = xcoord.name + '_bnds'
-        coords[ycoord.name].attrs['bounds'] = ycoord.name + '_bnds'
-        coords = {name: c for name, c in coords.items()
-                  if set(c.dims) <= set(dims)}
-        ret = xr.DataArray(pctl, name=arr.name, dims=dims, coords=coords,
-                           attrs=arr.attrs.copy())
+            coords["pctl"] = xr.Variable(
+                (), q[0] * 100.0, attrs={"long_name": "Percentile"}
+            )
+        else:
+            coords["pctl"] = xr.Variable(
+                ("pctl",), q * 100.0, attrs={"long_name": "Percentile"}
+            )
+            dims = ("pctl",) + dims
+        coords[xcoord.name].attrs["bounds"] = xcoord.name + "_bnds"
+        coords[ycoord.name].attrs["bounds"] = ycoord.name + "_bnds"
+        coords = {
+            name: c for name, c in coords.items() if set(c.dims) <= set(dims)
+        }
+        ret = xr.DataArray(
+            pctl,
+            name=arr.name,
+            dims=dims,
+            coords=coords,
+            attrs=arr.attrs.copy(),
+        )
         self._insert_fldmean_bounds(ret, keepdims)
         return ret
 
-    isel.__doc__ = xr.DataArray.isel.__doc__
-    sel.__doc__ = xr.DataArray.sel.__doc__
-
 
 class ArrayList(list):
     """Base class for creating a list of interactive arrays from a dataset
 
     This list contains and manages :class:`InteractiveArray` instances"""
 
-    docstrings.keep_params('InteractiveBase.parameters', 'auto_update')
+    docstrings.keep_params("InteractiveBase.parameters", "auto_update")
 
     @property
     def dims(self):
         """Dimensions of the arrays in this list"""
         return set(chain(*(arr.dims for arr in self)))
 
     @property
     def dims_intersect(self):
-        """Dimensions of the arrays in this list that are used in all arrays
-        """
-        return set.intersection(*map(
-            set, (getattr(arr, 'dims_intersect', arr.dims) for arr in self)))
+        """Dimensions of the arrays in this list that are used in all arrays"""
+        return set.intersection(
+            *map(
+                set, (getattr(arr, "dims_intersect", arr.dims) for arr in self)
+            )
+        )
 
     @property
     def arr_names(self):
         """Names of the arrays (!not of the variables!) in this list
 
         This attribute can be set with an iterable of unique names to change
         the array names of the data objects in this list."""
         return list(arr.psy.arr_name for arr in self)
 
     @arr_names.setter
     def arr_names(self, value):
         value = list(islice(value, 0, len(self)))
         if not len(set(value)) == len(self):
             raise ValueError(
-                "Got %i unique array names for %i data objects!" % (
-                    len(set(value)), len(self)))
+                "Got %i unique array names for %i data objects!"
+                % (len(set(value)), len(self))
+            )
         for arr, n in zip(self, value):
             arr.psy.arr_name = n
 
     @property
     def names(self):
         """Set of the variable in this list"""
         ret = set()
@@ -3480,89 +4164,103 @@
                 ret.add(arr.name)
         return ret
 
     @property
     def all_names(self):
         """The variable names for each of the arrays in this list"""
         return [
-            _get_variable_names(arr) if not isinstance(arr, ArrayList) else
-            arr.all_names
-            for arr in self]
+            _get_variable_names(arr)
+            if not isinstance(arr, ArrayList)
+            else arr.all_names
+            for arr in self
+        ]
 
     @property
     def all_dims(self):
         """The dimensions for each of the arrays in this list"""
         return [
-            _get_dims(arr) if not isinstance(arr, ArrayList) else
-            arr.all_dims
-            for arr in self]
+            _get_dims(arr) if not isinstance(arr, ArrayList) else arr.all_dims
+            for arr in self
+        ]
 
     @property
     def is_unstructured(self):
         """A boolean for each array whether it is unstructured or not"""
         return [
             arr.psy.decoder.is_unstructured(arr)
-            if not isinstance(arr, ArrayList) else
-            arr.is_unstructured
-            for arr in self]
+            if not isinstance(arr, ArrayList)
+            else arr.is_unstructured
+            for arr in self
+        ]
 
     @property
     def coords(self):
         """Names of the coordinates of the arrays in this list"""
         return set(chain(*(arr.coords for arr in self)))
 
     @property
     def coords_intersect(self):
-        """Coordinates of the arrays in this list that are used in all arrays
-        """
-        return set.intersection(*map(
-            set, (getattr(arr, 'coords_intersect', arr.coords) for arr in self)
-            ))
+        """Coordinates of the arrays in this list that are used in all arrays"""
+        return set.intersection(
+            *map(
+                set,
+                (getattr(arr, "coords_intersect", arr.coords) for arr in self),
+            )
+        )
 
     @property
     def with_plotter(self):
         """The arrays in this instance that are visualized with a plotter"""
         return self.__class__(
             (arr for arr in self if arr.psy.plotter is not None),
-            auto_update=bool(self.auto_update))
+            auto_update=bool(self.auto_update),
+        )
 
-    no_auto_update = property(_no_auto_update_getter,
-                              doc=_no_auto_update_getter.__doc__)
+    no_auto_update = property(
+        _no_auto_update_getter, doc=_no_auto_update_getter.__doc__
+    )
 
     @no_auto_update.setter
     def no_auto_update(self, value):
         for arr in self:
             arr.psy.no_auto_update = value
         self.no_auto_update.value = bool(value)
 
     @property
     def logger(self):
         """:class:`logging.Logger` of this instance"""
         try:
             return self._logger
         except AttributeError:
-            name = '%s.%s' % (self.__module__, self.__class__.__name__)
+            name = "%s.%s" % (self.__module__, self.__class__.__name__)
             self._logger = logging.getLogger(name)
-            self.logger.debug('Initializing...')
+            self.logger.debug("Initializing...")
             return self._logger
 
     @logger.setter
     def logger(self, value):
         self._logger = value
 
     @property
     def arrays(self):
-        """A list of all the :class:`xarray.DataArray` instances in this list
-        """
-        return list(chain.from_iterable(
-            ([arr] if not isinstance(arr, InteractiveList) else arr.arrays
-             for arr in self)))
+        """A list of all the :class:`xarray.DataArray` instances in this list"""
+        return list(
+            chain.from_iterable(
+                (
+                    [arr]
+                    if not isinstance(arr, InteractiveList)
+                    else arr.arrays
+                    for arr in self
+                )
+            )
+        )
 
-    @docstrings.get_sections(base='ArrayList.rename', sections=[
-        'Parameters', 'Raises'])
+    @docstrings.get_sections(
+        base="ArrayList.rename", sections=["Parameters", "Raises"]
+    )
     @dedent
     def rename(self, arr, new_name=True):
         """
         Rename an array to find a name that isn't already in the list
 
         Parameters
         ----------
@@ -3595,72 +4293,95 @@
         name_in_me = arr.psy.arr_name in self.arr_names
         if not name_in_me:
             return arr, False
         elif name_in_me and not self._contains_array(arr):
             if new_name is False:
                 raise ValueError(
                     "Array name %s is already in use! Set the `new_name` "
-                    "parameter to None for renaming!" % arr.psy.arr_name)
+                    "parameter to None for renaming!" % arr.psy.arr_name
+                )
             elif new_name is True:
-                new_name = new_name if isstring(new_name) else 'arr{0}'
+                new_name = new_name if isstring(new_name) else "arr{0}"
                 arr.psy.arr_name = self.next_available_name(new_name)
                 return arr, True
         return arr, None
 
-    docstrings.keep_params('ArrayList.rename.parameters', 'new_name')
-    docstrings.keep_params('InteractiveBase.parameters', 'auto_update')
+    docstrings.keep_params("ArrayList.rename.parameters", "new_name")
+    docstrings.keep_params("InteractiveBase.parameters", "auto_update")
 
-    @docstrings.get_sections(base='ArrayList')
+    @docstrings.get_sections(base="ArrayList")
     @docstrings.dedent
     def __init__(self, iterable=[], attrs={}, auto_update=None, new_name=True):
         """
         Parameters
         ----------
         iterable: iterable
             The iterable (e.g. another list) defining this list
         attrs: dict-like or iterable, optional
             Global attributes of this list
         %(InteractiveBase.parameters.auto_update)s
         %(ArrayList.rename.parameters.new_name)s"""
         super(ArrayList, self).__init__()
-        self.attrs = OrderedDict(attrs)
+        self.attrs = dict(attrs)
         if auto_update is None:
-            auto_update = rcParams['lists.auto_update']
+            auto_update = rcParams["lists.auto_update"]
         self.auto_update = not bool(auto_update)
         # append the data in order to set the correct names
-        self.extend(filter(
-            lambda arr: isinstance(getattr(arr, 'psy', None),
-                                   InteractiveBase),
-            iterable), new_name=new_name)
+        self.extend(
+            filter(
+                lambda arr: isinstance(
+                    getattr(arr, "psy", None), InteractiveBase
+                ),
+                iterable,
+            ),
+            new_name=new_name,
+        )
 
     def copy(self, deep=False):
         """Returns a copy of the list
 
         Parameters
         ----------
         deep: bool
             If False (default), only the list is copied and not the contained
             arrays, otherwise the contained arrays are deep copied"""
         if not deep:
-            return self.__class__(self[:], attrs=self.attrs.copy(),
-                                  auto_update=not bool(self.no_auto_update))
+            return self.__class__(
+                self[:],
+                attrs=self.attrs.copy(),
+                auto_update=not bool(self.no_auto_update),
+            )
         else:
             return self.__class__(
-                [arr.psy.copy(deep) for arr in self], attrs=self.attrs.copy(),
-                auto_update=not bool(self.auto_update))
+                [arr.psy.copy(deep) for arr in self],
+                attrs=self.attrs.copy(),
+                auto_update=not bool(self.auto_update),
+            )
 
-    docstrings.keep_params('InteractiveArray.update.parameters', 'method')
+    docstrings.keep_params("InteractiveArray.update.parameters", "method")
 
     @classmethod
-    @docstrings.get_sections(base='ArrayList.from_dataset', sections=[
-        'Parameters', 'Other Parameters', 'Returns'])
+    @docstrings.get_sections(
+        base="ArrayList.from_dataset",
+        sections=["Parameters", "Other Parameters", "Returns"],
+    )
     @docstrings.dedent
-    def from_dataset(cls, base, method='isel', default_slice=None,
-                     decoder=None, auto_update=None, prefer_list=False,
-                     squeeze=True, attrs=None, load=False, **kwargs):
+    def from_dataset(
+        cls,
+        base,
+        method="isel",
+        default_slice=None,
+        decoder=None,
+        auto_update=None,
+        prefer_list=False,
+        squeeze=True,
+        attrs=None,
+        load=False,
+        **kwargs,
+    ):
         """
         Construct an ArrayList instance from an existing base dataset
 
         Parameters
         ----------
         base: xarray.Dataset
             Dataset instance that is used as reference
@@ -3703,51 +4424,58 @@
         -------
         ArrayList
             The list with the specified :class:`InteractiveArray` instances
             that hold a reference to the given `base`"""
         try:
             load = dict(load)
         except (TypeError, ValueError):
+
             def maybe_load(arr):
                 return arr.load() if load else arr
+
         else:
+
             def maybe_load(arr):
                 return arr.load(**load)
 
         def iter_dims(dims):
             """Split the given dictionary into multiples and iterate over it"""
             if not dims:
                 while 1:
                     yield {}
             else:
-                dims = OrderedDict(dims)
+                dims = dict(dims)
                 keys = dims.keys()
                 for vals in zip(*map(cycle, map(safe_list, dims.values()))):
                     yield dict(zip(keys, vals))
 
         def recursive_selection(key, dims, names):
             names = safe_list(names)
             if len(names) > 1 and prefer_list:
-                keys = ('arr%i' % i for i in range(len(names)))
+                keys = ("arr%i" % i for i in range(len(names)))
                 return InteractiveList(
                     starmap(sel_method, zip(keys, iter_dims(dims), names)),
-                    auto_update=auto_update, arr_name=key)
+                    auto_update=auto_update,
+                    arr_name=key,
+                )
             elif len(names) > 1:
                 return sel_method(key, dims, tuple(names))
             else:
                 return sel_method(key, dims, names[0])
 
         def ds2arr(arr):
-            base_var = next(var for key, var in arr.variables.items()
-                            if key not in arr.coords)
+            base_var = next(
+                var
+                for key, var in arr.variables.items()
+                if key not in arr.coords
+            )
             attrs = base_var.attrs
             arr = arr.to_array()
-            if 'coordinates' in base_var.encoding:
-                arr.encoding['coordinates'] = base_var.encoding[
-                    'coordinates']
+            if "coordinates" in base_var.encoding:
+                arr.encoding["coordinates"] = base_var.encoding["coordinates"]
             arr.attrs.update(attrs)
             return arr
 
         decoder_input = decoder
 
         def get_decoder(arr):
             if decoder_input is None:
@@ -3759,79 +4487,110 @@
             else:
                 return decoder_input(base)
 
         def add_missing_dimensions(arr):
             # add the missing dimensions to the dataset. This is not anymore
             # done by default from xarray >= 0.9 but we need it to ensure the
             # interactive treatment of DataArrays
-            missing = set(arr.dims).difference(base.coords) - {'variable'}
+            missing = set(arr.dims).difference(base.coords) - {"variable"}
             for dim in missing:
-                base[dim] = arr.coords[dim] = np.arange(base.dims[dim])
+                try:
+                    size = base.sizes[dim]
+                except AttributeError:
+                    # old xarray version
+                    size = base.dims[dim]
+                base[dim] = arr.coords[dim] = np.arange(size)
 
         if squeeze:
+
             def squeeze_array(arr):
-                return arr.isel(**{dim: 0 for i, dim in enumerate(arr.dims)
-                                   if arr.shape[i] == 1})
+                return arr.isel(
+                    **{
+                        dim: 0
+                        for i, dim in enumerate(arr.dims)
+                        if arr.shape[i] == 1
+                    }
+                )
+
         else:
+
             def squeeze_array(arr):
                 return arr
-        if method == 'isel':
+
+        if method == "isel":
+
             def sel_method(key, dims, name=None):
                 if name is None:
-                    return recursive_selection(key, dims, dims.pop('name'))
-                elif (isinstance(name, six.string_types) or
-                      not utils.is_iterable(name)):
+                    return recursive_selection(key, dims, dims.pop("name"))
+                elif isinstance(
+                    name, six.string_types
+                ) or not utils.is_iterable(name):
                     arr = base[name]
                     decoder = get_decoder(arr)
                     dims = decoder.correct_dims(arr, dims)
                 else:
                     arr = base[list(name)]
                     decoder = get_decoder(base[name[0]])
                     dims = decoder.correct_dims(base[name[0]], dims)
-                def_slice = slice(None) if default_slice is None else \
-                    default_slice
-                dims.update({
-                    dim: def_slice for dim in set(arr.dims).difference(
-                        dims) if dim != 'variable'})
+                def_slice = (
+                    slice(None) if default_slice is None else default_slice
+                )
+                dims.update(
+                    {
+                        dim: def_slice
+                        for dim in set(arr.dims).difference(dims)
+                        if dim != "variable"
+                    }
+                )
                 add_missing_dimensions(arr)
                 ret = arr.isel(**dims)
                 if not isinstance(ret, xr.DataArray):
                     ret = ds2arr(ret)
                 ret = squeeze_array(ret)
                 # delete the variable dimension for the idims
-                dims.pop('variable', None)
-                ret.psy.init_accessor(arr_name=key, base=base, idims=dims,
-                                      decoder=decoder)
+                dims.pop("variable", None)
+                ret.psy.init_accessor(
+                    arr_name=key, base=base, idims=dims, decoder=decoder
+                )
                 return maybe_load(ret)
+
         else:
+
             def sel_method(key, dims, name=None):
                 if name is None:
-                    return recursive_selection(key, dims, dims.pop('name'))
-                elif (isinstance(name, six.string_types) or
-                      not utils.is_iterable(name)):
+                    return recursive_selection(key, dims, dims.pop("name"))
+                elif isinstance(
+                    name, six.string_types
+                ) or not utils.is_iterable(name):
                     arr = base[name]
                     decoder = get_decoder(arr)
                     dims = decoder.correct_dims(arr, dims)
                 else:
                     arr = base[list(name)]
                     decoder = get_decoder(base[name[0]])
                     dims = decoder.correct_dims(base[name[0]], dims)
                 if default_slice is not None:
                     if isinstance(default_slice, slice):
-                        dims.update({
-                            dim: default_slice
-                            for dim in set(arr.dims).difference(dims)
-                            if dim != 'variable'})
+                        dims.update(
+                            {
+                                dim: default_slice
+                                for dim in set(arr.dims).difference(dims)
+                                if dim != "variable"
+                            }
+                        )
                     else:
-                        dims.update({
-                            dim: arr.coords[dim][default_slice]
-                            for dim in set(arr.dims).difference(dims)
-                            if dim != 'variable'})
+                        dims.update(
+                            {
+                                dim: arr.coords[dim][default_slice]
+                                for dim in set(arr.dims).difference(dims)
+                                if dim != "variable"
+                            }
+                        )
                 kws = dims.copy()
-                kws['method'] = method
+                kws["method"] = method
                 # the sel method does not work with slice objects
                 for dim, val in dims.items():
                     if isinstance(val, slice):
                         if val == slice(None):
                             kws.pop(dim)  # the full slice is the default
                         else:
                             kws.pop("method", None)
@@ -3842,111 +4601,159 @@
                     _fix_times(kws)
                     ret = arr.sel(**kws)
                 if not isinstance(ret, xr.DataArray):
                     ret = ds2arr(ret)
                 ret = squeeze_array(ret)
                 ret.psy.init_accessor(arr_name=key, base=base, decoder=decoder)
                 return maybe_load(ret)
-        if 'name' not in kwargs:
+
+        if "name" not in kwargs:
             default_names = list(
-                key for key in base.variables if key not in base.coords)
+                key for key in base.variables if key not in base.coords
+            )
             try:
                 default_names.sort()
             except TypeError:
                 pass
-            kwargs['name'] = default_names
+            kwargs["name"] = default_names
         names = setup_coords(**kwargs)
         # check coordinates
-        possible_keys = ['t', 'x', 'y', 'z', 'name'] + list(base.dims)
+        possible_keys = ["t", "x", "y", "z", "name"] + list(base.dims)
         for key in set(chain(*six.itervalues(names))):
-            utils.check_key(key, possible_keys, name='dimension')
-        instance = cls(starmap(sel_method, six.iteritems(names)),
-                       attrs=base.attrs, auto_update=auto_update)
+            utils.check_key(key, possible_keys, name="dimension")
+        instance = cls(
+            starmap(sel_method, six.iteritems(names)),
+            attrs=base.attrs,
+            auto_update=auto_update,
+        )
         # convert to interactive lists if an instance is not
         if prefer_list and any(
-                not isinstance(arr, InteractiveList) for arr in instance):
+            not isinstance(arr, InteractiveList) for arr in instance
+        ):
             # if any instance is an interactive list, than convert the others
             if any(isinstance(arr, InteractiveList) for arr in instance):
                 for i, arr in enumerate(instance):
                     if not isinstance(arr, InteractiveList):
                         instance[i] = InteractiveList([arr])
             else:  # put everything into one single interactive list
-                instance = cls([InteractiveList(instance, attrs=base.attrs,
-                                                auto_update=auto_update)])
+                instance = cls(
+                    [
+                        InteractiveList(
+                            instance, attrs=base.attrs, auto_update=auto_update
+                        )
+                    ]
+                )
                 instance[0].psy.arr_name = instance[0][0].psy.arr_name
         if attrs is not None:
             for arr in instance:
                 arr.attrs.update(attrs)
         return instance
 
     @classmethod
-    def _get_dsnames(cls, data, ignore_keys=['attrs', 'plotter', 'ds'],
-                     concat_dim=False, combine=False):
+    def _get_dsnames(
+        cls,
+        data,
+        ignore_keys=["attrs", "plotter", "ds"],
+        concat_dim=False,
+        combine=False,
+    ):
         """Recursive method to get all the file names out of a dictionary
         `data` created with the :meth`array_info` method"""
+
         def filter_ignores(item):
             return item[0] not in ignore_keys and isinstance(item[1], dict)
-        if 'fname' in data:
-            return {tuple(
-                [data['fname'], data['store']] +
-                ([data.get('concat_dim')] if concat_dim else []) +
-                ([data.get('combine')] if combine else []))}
-        return set(chain(*map(partial(cls._get_dsnames, concat_dim=concat_dim,
-                                      combine=combine,
-                                      ignore_keys=ignore_keys),
-                              dict(filter(filter_ignores,
-                                          six.iteritems(data))).values())))
+
+        if "fname" in data:
+            return {
+                tuple(
+                    [data["fname"], data["store"]]
+                    + ([data.get("concat_dim")] if concat_dim else [])
+                    + ([data.get("combine")] if combine else [])
+                )
+            }
+        return set(
+            chain(
+                *map(
+                    partial(
+                        cls._get_dsnames,
+                        concat_dim=concat_dim,
+                        combine=combine,
+                        ignore_keys=ignore_keys,
+                    ),
+                    dict(filter(filter_ignores, six.iteritems(data))).values(),
+                )
+            )
+        )
 
     @classmethod
     def _get_ds_descriptions(
-            cls, data, ds_description={'ds', 'fname', 'arr'}, **kwargs):
+        cls, data, ds_description={"ds", "fname", "arr"}, **kwargs
+    ):
         def new_dict():
             return defaultdict(list)
+
         ret = defaultdict(new_dict)
         ds_description = set(ds_description)
         for d in cls._get_ds_descriptions_unsorted(data, **kwargs):
             try:
-                num = d.get('num') or d['ds'].psy.num
+                num = d.get("num") or d["ds"].psy.num
             except KeyError:
                 raise ValueError(
-                    'Could not find either the dataset number nor the dataset '
-                    'in the data! However one must be provided.')
+                    "Could not find either the dataset number nor the dataset "
+                    "in the data! However one must be provided."
+                )
             d_ret = ret[num]
             for key, val in six.iteritems(d):
-                if key == 'arr':
-                    d_ret['arr'].append(d['arr'])
+                if key == "arr":
+                    d_ret["arr"].append(d["arr"])
                 else:
                     d_ret[key] = val
         return ret
 
     @classmethod
     def _get_ds_descriptions_unsorted(
-            cls, data, ignore_keys=['attrs', 'plotter'], nums=None):
+        cls, data, ignore_keys=["attrs", "plotter"], nums=None
+    ):
         """Recursive method to get all the file names or datasets out of a
         dictionary `data` created with the :meth`array_info` method"""
-        ds_description = {'ds', 'fname', 'num', 'arr', 'store'}
-        if 'ds' in data:
+        ds_description = {"ds", "fname", "num", "arr", "store"}
+        if "ds" in data:
             # make sure that the data set has a number assigned to it
-            data['ds'].psy.num
+            data["ds"].psy.num
         keys_in_data = ds_description.intersection(data)
         if keys_in_data:
             return {key: data[key] for key in keys_in_data}
         for key in ignore_keys:
             data.pop(key, None)
-        func = partial(cls._get_ds_descriptions_unsorted,
-                       ignore_keys=ignore_keys, nums=nums)
-        return chain(*map(lambda d: [d] if isinstance(d, dict) else d,
-                          map(func, six.itervalues(data))))
+        func = partial(
+            cls._get_ds_descriptions_unsorted,
+            ignore_keys=ignore_keys,
+            nums=nums,
+        )
+        return chain(
+            *map(
+                lambda d: [d] if isinstance(d, dict) else d,
+                map(func, six.itervalues(data)),
+            )
+        )
 
     @classmethod
-    @docstrings.get_sections(base='ArrayList.from_dict')
+    @docstrings.get_sections(base="ArrayList.from_dict")
     @docstrings.dedent
-    def from_dict(cls, d, alternative_paths={}, datasets=None,
-                  pwd=None, ignore_keys=['attrs', 'plotter', 'ds'],
-                  only=None, chname={}, **kwargs):
+    def from_dict(
+        cls,
+        d,
+        alternative_paths={},
+        datasets=None,
+        pwd=None,
+        ignore_keys=["attrs", "plotter", "ds"],
+        only=None,
+        chname={},
+        **kwargs,
+    ):
         """
         Create a list from the dictionary returned by :meth:`array_info`
 
         This classmethod creates an :class:`~psyplot.data.ArrayList` instance
         from a dictionary containing filename, dimension infos and array names
 
         Parameters
@@ -3956,15 +4763,15 @@
         alternative_paths: dict or list or str
             A mapping from original filenames as used in `d` to filenames that
             shall be used instead. If `alternative_paths` is not None,
             datasets must be None. Paths must be accessible from the current
             working directory.
             If `alternative_paths` is a list (or any other iterable) is
             provided, the file names will be replaced as they appear in `d`
-            (note that this is very unsafe if `d` is not and OrderedDict)
+            (note that this is very unsafe if `d` is not and dict)
         datasets: dict or list or None
             A mapping from original filenames in `d` to the instances of
             :class:`xarray.Dataset` to use. If it is an iterable, the same
             holds as for the `alternative_paths` parameter
         pwd: str
             Path to the working directory from where the data can be imported.
             If None, use the current working directory.
@@ -4018,139 +4825,176 @@
         -------
         psyplot.data.ArrayList
             The list with the interactive objects
 
         See Also
         --------
         from_dataset, array_info"""
-        pwd = pwd or getcwd()
+        pwd = pwd or os.getcwd()
         if only is None:
+
             def only_filter(arr_name, info):
                 return True
+
         elif callable(only):
             only_filter = only
         elif isstring(only):
+
             def only_filter(arr_name, info):
                 return patt.search(arr_name) is not None
+
             patt = re.compile(only)
             only = None
         else:
+
             def only_filter(arr_name, info):
                 return arr_name in save_only
+
             save_only = only
             only = None
 
         def get_fname_use(fname):
             squeeze = isstring(fname)
             fname = safe_list(fname)
-            ret = tuple(f if utils.is_remote_url(f) or osp.isabs(f) else
-                        osp.join(pwd, f)
-                        for f in fname)
+            ret = tuple(
+                f
+                if utils.is_remote_url(f) or osp.isabs(f)
+                else osp.join(pwd, f)
+                for f in fname
+            )
             return ret[0] if squeeze else ret
 
         def get_name(name):
             if not isstring(name):
                 return list(map(get_name, name))
             else:
                 return chname.get(name, name)
 
         if not isinstance(alternative_paths, dict):
             it = iter(alternative_paths)
             alternative_paths = defaultdict(partial(next, it, None))
         # first open all datasets if not already done
         if datasets is None:
-            replace_concat_dim = 'concat_dim' not in kwargs
-            replace_combine = 'combine' not in kwargs
+            replace_concat_dim = "concat_dim" not in kwargs
+            replace_combine = "combine" not in kwargs
 
             names_and_stores = cls._get_dsnames(
-                d, concat_dim=True, combine=True)
+                d, concat_dim=True, combine=True
+            )
             datasets = {}
-            for fname, (store_mod, store_cls), concat_dim, combine in names_and_stores:
+            for (
+                fname,
+                (store_mod, store_cls),
+                concat_dim,
+                combine,
+            ) in names_and_stores:
                 fname_use = fname
                 got = True
                 if replace_concat_dim and concat_dim is not None:
-                    kwargs['concat_dim'] = concat_dim
+                    kwargs["concat_dim"] = concat_dim
                 elif replace_concat_dim and concat_dim is None:
-                    kwargs.pop('concat_dim', None)
+                    kwargs.pop("concat_dim", None)
                 if replace_combine and combine is not None:
-                    kwargs['combine'] = combine
+                    kwargs["combine"] = combine
                 elif replace_combine and combine is None:
-                    kwargs.pop('combine', None)
+                    kwargs.pop("combine", None)
                 try:
                     fname_use = alternative_paths[fname]
                 except KeyError:
                     got = False
                 if not got or not fname_use:
                     if fname is not None:
                         fname_use = get_fname_use(fname)
                 if fname_use is not None:
                     datasets[fname] = _open_ds_from_store(
-                        fname_use, store_mod, store_cls, **kwargs)
+                        fname_use, store_mod, store_cls, **kwargs
+                    )
             if alternative_paths is not None:
                 for fname in set(alternative_paths).difference(datasets):
                     datasets[fname] = _open_ds_from_store(fname, **kwargs)
         elif not isinstance(datasets, dict):
             it_datasets = iter(datasets)
             datasets = defaultdict(partial(next, it_datasets, None))
         arrays = [0] * len(d)
         i = 0
         for arr_name, info in six.iteritems(d):
             if arr_name in ignore_keys or not only_filter(arr_name, info):
                 arrays.pop(i)
                 continue
-            if not {'fname', 'ds', 'arr'}.intersection(info):
+            if not {"fname", "ds", "arr"}.intersection(info):
                 # the described object is an InteractiveList
                 arr = InteractiveList.from_dict(
-                    info, alternative_paths=alternative_paths,
-                    datasets=datasets, chname=chname)
+                    info,
+                    alternative_paths=alternative_paths,
+                    datasets=datasets,
+                    chname=chname,
+                )
                 if not arr:
                     warn("Skipping empty list %s!" % arr_name)
                     arrays.pop(i)
                     continue
             else:
-                if 'arr' in info:
-                    arr = info.pop('arr')
-                elif 'ds' in info:
+                if "arr" in info:
+                    arr = info.pop("arr")
+                elif "ds" in info:
                     arr = cls.from_dataset(
-                        info['ds'], dims=info['dims'],
-                        name=get_name(info['name']))[0]
+                        info["ds"],
+                        dims=info["dims"],
+                        name=get_name(info["name"]),
+                    )[0]
                 else:
-                    fname = info['fname']
+                    fname = info["fname"]
                     if fname is None:
-                        warn("Could not open array %s because no filename was "
-                             "specified!" % arr_name)
+                        warn(
+                            "Could not open array %s because no filename was "
+                            "specified!" % arr_name
+                        )
                         arrays.pop(i)
                         continue
                     try:  # in case, datasets is a defaultdict
                         datasets[fname]
                     except KeyError:
                         pass
                     if fname not in datasets:
-                        warn("Could not open array %s because %s was not in "
-                             "the list of datasets!" % (arr_name, fname))
+                        warn(
+                            "Could not open array %s because %s was not in "
+                            "the list of datasets!" % (arr_name, fname)
+                        )
                         arrays.pop(i)
                         continue
                     arr = cls.from_dataset(
-                        datasets[fname], dims=info['dims'],
-                        name=get_name(info['name']))[0]
-                for key, val in six.iteritems(info.get('attrs', {})):
+                        datasets[fname],
+                        dims=info["dims"],
+                        name=get_name(info["name"]),
+                    )[0]
+                for key, val in six.iteritems(info.get("attrs", {})):
                     arr.attrs.setdefault(key, val)
             arr.psy.arr_name = arr_name
             arrays[i] = arr
             i += 1
-        return cls(arrays, attrs=d.get('attrs', {}))
+        return cls(arrays, attrs=d.get("attrs", {}))
 
-    docstrings.delete_params('get_filename_ds.parameters', 'ds', 'dump')
+    docstrings.delete_params("get_filename_ds.parameters", "ds", "dump")
 
-    @docstrings.get_sections(base='ArrayList.array_info')
+    @docstrings.get_sections(base="ArrayList.array_info")
     @docstrings.dedent
-    def array_info(self, dump=None, paths=None, attrs=True,
-                   standardize_dims=True, pwd=None, use_rel_paths=True,
-                   alternative_paths={}, ds_description={'fname', 'store'},
-                   full_ds=True, copy=False, **kwargs):
+    def array_info(
+        self,
+        dump=None,
+        paths=None,
+        attrs=True,
+        standardize_dims=True,
+        pwd=None,
+        use_rel_paths=True,
+        alternative_paths={},
+        ds_description={"fname", "store"},
+        full_ds=True,
+        copy=False,
+        **kwargs,
+    ):
         """
         Get dimension informations on you arrays
 
         This method returns a dictionary containing informations on the
         array in this instance
 
         Parameters
@@ -4200,142 +5044,177 @@
 
         Other Parameters
         ----------------
         %(get_filename_ds.other_parameters)s
 
         Returns
         -------
-        OrderedDict
+        dict
             An ordered mapping from array names to dimensions and filename
             corresponding to the array
 
         See Also
         --------
         from_dict"""
-        saved_ds = kwargs.pop('_saved_ds', {})
+        saved_ds = kwargs.pop("_saved_ds", {})
 
         def get_alternative(f):
-            return next(filter(lambda t: osp.samefile(f, t[0]),
-                               six.iteritems(alternative_paths)), [False, f])
+            return next(
+                filter(
+                    lambda t: osp.samefile(f, t[0]),
+                    six.iteritems(alternative_paths),
+                ),
+                [False, f],
+            )
 
         if copy:
+
             def copy_obj(obj):
                 # try to get the number of the dataset and create only one copy
                 # copy for each dataset
                 try:
                     num = obj.psy.num
                 except AttributeError:
                     pass
                 else:
                     try:
                         return saved_ds[num]
                     except KeyError:
                         saved_ds[num] = obj.psy.copy(True)
                         return saved_ds[num]
                 return obj.psy.copy(True)
+
         else:
+
             def copy_obj(obj):
                 return obj
-        ret = OrderedDict()
-        if ds_description == 'all':
-            ds_description = {'fname', 'ds', 'num', 'arr', 'store'}
+
+        ret = dict()
+        if ds_description == "all":
+            ds_description = {"fname", "ds", "num", "arr", "store"}
         if paths is not None:
             if dump is None:
                 dump = True
             paths = iter(paths)
         elif dump is None:
             dump = False
         if pwd is None:
-            pwd = getcwd()
+            pwd = os.getcwd()
         for arr in self:
             if isinstance(arr, InteractiveList):
                 ret[arr.arr_name] = arr.array_info(
-                    dump, paths, pwd=pwd, attrs=attrs,
+                    dump,
+                    paths,
+                    pwd=pwd,
+                    attrs=attrs,
                     standardize_dims=standardize_dims,
-                    use_rel_paths=use_rel_paths, ds_description=ds_description,
-                    alternative_paths=alternative_paths, copy=copy,
-                    _saved_ds=saved_ds, **kwargs)
+                    use_rel_paths=use_rel_paths,
+                    ds_description=ds_description,
+                    alternative_paths=alternative_paths,
+                    copy=copy,
+                    _saved_ds=saved_ds,
+                    **kwargs,
+                )
             else:
                 if standardize_dims:
                     idims = arr.psy.decoder.standardize_dims(
-                        next(arr.psy.iter_base_variables), arr.psy.idims)
+                        next(arr.psy.iter_base_variables), arr.psy.idims
+                    )
                 else:
                     idims = arr.psy.idims
-                ret[arr.psy.arr_name] = d = {'dims': idims}
-                if 'variable' in arr.coords:
-                    d['name'] = [list(arr.coords['variable'].values)]
+                ret[arr.psy.arr_name] = d = {"dims": idims}
+                if "variable" in arr.coords:
+                    d["name"] = [list(arr.coords["variable"].values)]
                 else:
-                    d['name'] = arr.name
-                if 'fname' in ds_description or 'store' in ds_description:
+                    d["name"] = arr.name
+                if "fname" in ds_description or "store" in ds_description:
                     fname, store_mod, store_cls = get_filename_ds(
-                        arr.psy.base, dump=dump, paths=paths, **kwargs)
-                    if 'store' in ds_description:
-                        d['store'] = (store_mod, store_cls)
-                    if 'fname' in ds_description:
-                        d['fname'] = []
+                        arr.psy.base, dump=dump, paths=paths, **kwargs
+                    )
+                    if "store" in ds_description:
+                        d["store"] = (store_mod, store_cls)
+                    if "fname" in ds_description:
+                        d["fname"] = []
                         for i, f in enumerate(safe_list(fname)):
-                            if (f is None or utils.is_remote_url(f)):
-                                d['fname'].append(f)
+                            if f is None or utils.is_remote_url(f):
+                                d["fname"].append(f)
                             else:
                                 found, f = get_alternative(f)
                                 if use_rel_paths:
                                     f = osp.relpath(f, pwd)
                                 else:
                                     f = osp.abspath(f)
-                                d['fname'].append(f)
-                        if fname is None or isinstance(fname,
-                                                       six.string_types):
-                            d['fname'] = d['fname'][0]
+                                d["fname"].append(f)
+                        if fname is None or isinstance(
+                            fname, six.string_types
+                        ):
+                            d["fname"] = d["fname"][0]
                         else:
-                            d['fname'] = tuple(safe_list(fname))
+                            d["fname"] = tuple(safe_list(fname))
                         if arr.psy.base.psy._concat_dim is not None:
-                            d['concat_dim'] = arr.psy.base.psy._concat_dim
+                            d["concat_dim"] = arr.psy.base.psy._concat_dim
                         if arr.psy.base.psy._combine is not None:
-                            d['combine'] = arr.psy.base.psy._combine
-                if 'ds' in ds_description:
+                            d["combine"] = arr.psy.base.psy._combine
+                if "ds" in ds_description:
                     if full_ds:
-                        d['ds'] = copy_obj(arr.psy.base)
+                        d["ds"] = copy_obj(arr.psy.base)
                     else:
-                        d['ds'] = copy_obj(arr.to_dataset())
-                if 'num' in ds_description:
-                    d['num'] = arr.psy.base.psy.num
-                if 'arr' in ds_description:
-                    d['arr'] = copy_obj(arr)
+                        d["ds"] = copy_obj(arr.to_dataset())
+                if "num" in ds_description:
+                    d["num"] = arr.psy.base.psy.num
+                if "arr" in ds_description:
+                    d["arr"] = copy_obj(arr)
                 if attrs:
-                    d['attrs'] = arr.attrs
-        ret['attrs'] = self.attrs
+                    d["attrs"] = arr.attrs
+        ret["attrs"] = self.attrs
         return ret
 
     def _get_tnames(self):
         """Get the name of the time coordinate of the objects in this list"""
         tnames = set()
         for arr in self:
             if isinstance(arr, InteractiveList):
                 tnames.update(arr.get_tnames())
             else:
-                tnames.add(arr.psy.decoder.get_tname(
-                    next(arr.psy.iter_base_variables), arr.coords))
+                tnames.add(
+                    arr.psy.decoder.get_tname(
+                        next(arr.psy.iter_base_variables), arr.coords
+                    )
+                )
         return tnames - {None}
 
     @docstrings.dedent
-    def _register_update(self, method='isel', replot=False, dims={}, fmt={},
-                         force=False, todefault=False):
+    def _register_update(
+        self,
+        method="isel",
+        replot=False,
+        dims={},
+        fmt={},
+        force=False,
+        todefault=False,
+    ):
         """
         Register new dimensions and formatoptions for updating. The keywords
         are the same as for each single array
 
         Parameters
         ----------
         %(InteractiveArray._register_update.parameters)s"""
 
         for arr in self:
-            arr.psy._register_update(method=method, replot=replot, dims=dims,
-                                     fmt=fmt, force=force, todefault=todefault)
+            arr.psy._register_update(
+                method=method,
+                replot=replot,
+                dims=dims,
+                fmt=fmt,
+                force=force,
+                todefault=todefault,
+            )
 
-    @docstrings.get_sections(base='ArrayList.start_update')
+    @docstrings.get_sections(base="ArrayList.start_update")
     @dedent
     def start_update(self, draw=None):
         """
         Conduct the registered plot updates
 
         This method starts the updates from what has been registered by the
         :meth:`update` method. You can call this method if you did not set the
@@ -4348,53 +5227,71 @@
             If True, all the figures of the arrays contained in this list will
             be drawn at the end. If None, it defaults to the `'auto_draw'``
             parameter in the :attr:`psyplot.rcParams` dictionary
 
         See Also
         --------
         :attr:`no_auto_update`, update"""
+
         def worker(arr):
             results[arr.psy.arr_name] = arr.psy.start_update(
-                draw=False, queues=queues)
+                draw=False, queues=queues
+            )
+
         if len(self) == 0:
             return
 
         results = {}
-        threads = [Thread(target=worker, args=(arr,),
-                          name='update_%s' % arr.psy.arr_name)
-                   for arr in self]
+        threads = [
+            Thread(
+                target=worker, args=(arr,), name="update_%s" % arr.psy.arr_name
+            )
+            for arr in self
+        ]
         jobs = [arr.psy._njobs for arr in self]
         queues = [Queue() for _ in range(max(map(len, jobs)))]
         # populate the queues
         for i, arr in enumerate(self):
             for j, n in enumerate(jobs[i]):
                 for k in range(n):
                     queues[j].put(arr.psy.arr_name)
         for thread in threads:
             thread.setDaemon(True)
         for thread in threads:
             thread.start()
         for thread in threads:
             thread.join()
         if draw is None:
-            draw = rcParams['auto_draw']
+            draw = rcParams["auto_draw"]
         if draw:
-            self(arr_name=[name for name, adraw in six.iteritems(results)
-                           if adraw]).draw()
-            if rcParams['auto_show']:
+            self(
+                arr_name=[
+                    name for name, adraw in six.iteritems(results) if adraw
+                ]
+            ).draw()
+            if rcParams["auto_show"]:
                 self.show()
 
-    docstrings.keep_params('InteractiveArray.update.parameters',
-                           'auto_update')
+    docstrings.keep_params("InteractiveArray.update.parameters", "auto_update")
 
-    @docstrings.get_sections(base='ArrayList.update')
+    @docstrings.get_sections(base="ArrayList.update")
     @docstrings.dedent
-    def update(self, method='isel', dims={}, fmt={}, replot=False,
-               auto_update=False, draw=None, force=False, todefault=False,
-               enable_post=None, **kwargs):
+    def update(
+        self,
+        method="isel",
+        dims={},
+        fmt={},
+        replot=False,
+        auto_update=False,
+        draw=None,
+        force=False,
+        todefault=False,
+        enable_post=None,
+        **kwargs,
+    ):
         """
         Update the coordinates and the plot
 
         This method updates all arrays in this list with the given coordinate
         values and formatoptions.
 
         Parameters
@@ -4414,40 +5311,50 @@
         %(InteractiveArray.update.notes)s
 
         See Also
         --------
         no_auto_update, start_update"""
         dims = dict(dims)
         fmt = dict(fmt)
-        vars_and_coords = set(chain(
-            self.dims, self.coords, ['name', 'x', 'y', 'z', 't']))
+        vars_and_coords = set(
+            chain(self.dims, self.coords, ["name", "x", "y", "z", "t"])
+        )
         furtherdims, furtherfmt = utils.sort_kwargs(kwargs, vars_and_coords)
         dims.update(furtherdims)
         fmt.update(furtherfmt)
 
-        self._register_update(method=method, replot=replot, dims=dims, fmt=fmt,
-                              force=force, todefault=todefault)
+        self._register_update(
+            method=method,
+            replot=replot,
+            dims=dims,
+            fmt=fmt,
+            force=force,
+            todefault=todefault,
+        )
         if enable_post is not None:
             for arr in self.with_plotter:
                 arr.psy.plotter.enable_post = enable_post
         if not self.no_auto_update or auto_update:
             self.start_update(draw)
 
     def draw(self):
         """Draws all the figures in this instance"""
-        for fig in set(chain(*map(
-                lambda arr: arr.psy.plotter.figs2draw, self.with_plotter))):
+        for fig in set(
+            chain(
+                *map(lambda arr: arr.psy.plotter.figs2draw, self.with_plotter)
+            )
+        ):
             self.logger.debug("Drawing figure %s", fig.number)
             fig.canvas.draw()
         for arr in self:
             if arr.psy.plotter is not None:
                 arr.psy.plotter._figs2draw.clear()
         self.logger.debug("Done drawing.")
 
-    def __call__(self, types=None, method='isel', fmts=[], **attrs):
+    def __call__(self, types=None, method="isel", fmts=[], **attrs):
         """Get the arrays specified by their attributes
 
         Parameters
         ----------
         types: type or tuple of types
             Any class that shall be used for an instance check via
             :func:`isinstance`. If not None, the :attr:`plotter` attribute
@@ -4464,73 +5371,91 @@
         ``**attrs``
             Parameters may be any attribute of the arrays in this instance,
             including the matplotlib axes (``ax``), matplotlib figure
             (``fig``) and the array name (``arr_name``).
             Values may be iterables (e.g. lists) of the attributes to consider
             or callable functions that accept the attribute as a value. If the
             value is a string, it will be put into a list."""
+
         def safe_item_list(key, val):
             return key, val if callable(val) else safe_list(val)
 
         def filter_list(arr):
             other_attrs = attrs.copy()
-            arr_names = other_attrs.pop('arr_name', None)
-            return ((arr_names is None or (
-                        arr_names(arr.psy.arr_name) if callable(arr_names)
-                        else arr.psy.arr_name in arr_names)) and
-                    len(arr) == len(arr(types=types, method=method,
-                                        **other_attrs)))
+            arr_names = other_attrs.pop("arr_name", None)
+            return (
+                arr_names is None
+                or (
+                    arr_names(arr.psy.arr_name)
+                    if callable(arr_names)
+                    else arr.psy.arr_name in arr_names
+                )
+            ) and len(arr) == len(
+                arr(types=types, method=method, **other_attrs)
+            )
+
         if not attrs:
+
             def filter_by_attrs(arr):
                 return True
-        elif method == 'sel':
+
+        elif method == "sel":
+
             def filter_by_attrs(arr):
                 if isinstance(arr, InteractiveList):
                     return filter_list(arr)
                 tname = arr.psy.decoder.get_tname(
-                    next(six.itervalues(arr.psy.base_variables)))
+                    next(six.itervalues(arr.psy.base_variables))
+                )
 
                 def check_values(arr, key, vals):
-                    if key == 'arr_name':
+                    if key == "arr_name":
                         attr = arr.psy.arr_name
-                    elif key == 'ax':
+                    elif key == "ax":
                         attr = arr.psy.ax
-                    elif key == 'fig':
-                        attr = getattr(arr.psy.ax, 'figure', None)
+                    elif key == "fig":
+                        attr = getattr(arr.psy.ax, "figure", None)
                     else:
                         try:
                             attr = getattr(arr, key)
                         except AttributeError:
                             return False
                     if np.ndim(attr):  # do not filter for multiple items
                         return False
-                    if hasattr(arr.psy, 'decoder') and (
-                            arr.name == tname):
+                    if hasattr(arr.psy, "decoder") and (arr.name == tname):
                         try:
                             vals = np.asarray(vals, dtype=np.datetime64)
                         except ValueError:
                             pass
                         else:
                             return attr.values.astype(vals.dtype) in vals
                     if callable(vals):
                         return vals(attr)
-                    return getattr(attr, 'values', attr) in vals
+                    return getattr(attr, "values", attr) in vals
+
                 return all(
                     check_values(arr, key, val)
                     for key, val in six.iteritems(
-                        arr.psy.decoder.correct_dims(next(six.itervalues(
-                            arr.psy.base_variables)), attrs, remove=False)))
+                        arr.psy.decoder.correct_dims(
+                            next(six.itervalues(arr.psy.base_variables)),
+                            attrs,
+                            remove=False,
+                        )
+                    )
+                )
+
         else:
+
             def check_values(arr, key, vals):
-                if key == 'arr_name':
+                if key == "arr_name":
                     attr = arr.psy.arr_name
-                elif key == 'ax':
+                elif key == "ax":
                     attr = arr.psy.ax
-                elif key == 'fig':
-                    attr = getattr(arr.psy.ax, 'figure', None)
+                elif key == "fig":
+                    attr = getattr(arr.psy.ax, "figure", None)
                 elif key in arr.coords:
                     attr = arr.psy.idims[key]
                 else:
                     try:
                         attr = getattr(arr, key)
                     except AttributeError:
                         return False
@@ -4542,96 +5467,115 @@
 
             def filter_by_attrs(arr):
                 if isinstance(arr, InteractiveList):
                     return filter_list(arr)
                 return all(
                     check_values(arr, key, val)
                     for key, val in six.iteritems(
-                        arr.psy.decoder.correct_dims(next(six.itervalues(
-                            arr.psy.base_variables)), attrs, remove=False)))
+                        arr.psy.decoder.correct_dims(
+                            next(six.itervalues(arr.psy.base_variables)),
+                            attrs,
+                            remove=False,
+                        )
+                    )
+                )
+
         attrs = dict(starmap(safe_item_list, six.iteritems(attrs)))
         ret = self.__class__(
             # iterable
-            (arr for arr in self if
-             (types is None or isinstance(arr.psy.plotter, types)) and
-             filter_by_attrs(arr)),
+            (
+                arr
+                for arr in self
+                if (types is None or isinstance(arr.psy.plotter, types))
+                and filter_by_attrs(arr)
+            ),
             # give itself as base and the auto_update parameter
-            auto_update=bool(self.auto_update))
+            auto_update=bool(self.auto_update),
+        )
         # now filter for the formatoptions
         if fmts:
             fmts = set(safe_list(fmts))
             ret = self.__class__(
-                filter(lambda arr: (arr.psy.plotter and
-                                    fmts <= set(arr.psy.plotter)),
-                       ret))
+                filter(
+                    lambda arr: (
+                        arr.psy.plotter and fmts <= set(arr.psy.plotter)
+                    ),
+                    ret,
+                )
+            )
         return ret
 
     def __contains__(self, val):
         try:
             name = val if isstring(val) else val.psy.arr_name
         except AttributeError:
             return False
         else:
             return name in self.arr_names and (
-                isstring(val) or self._contains_array(val))
+                isstring(val) or self._contains_array(val)
+            )
 
     def _contains_array(self, val):
         """Checks whether exactly this array is in the list"""
         arr = self(arr_name=val.psy.arr_name)[0]
         is_not_list = any(
-            map(lambda a: not isinstance(a, InteractiveList),
-                [arr, val]))
-        is_list = any(map(lambda a: isinstance(a, InteractiveList),
-                          [arr, val]))
+            map(lambda a: not isinstance(a, InteractiveList), [arr, val])
+        )
+        is_list = any(
+            map(lambda a: isinstance(a, InteractiveList), [arr, val])
+        )
         # if one is an InteractiveList and the other not, they differ
         if is_list and is_not_list:
             return False
         # if both are interactive lists, check the lists
         if is_list:
             return all(a in arr for a in val) and all(a in val for a in arr)
         # else we check the shapes and values
         return arr is val
 
     def _short_info(self, intend=0, maybe=False):
         if maybe:
             intend = 0
-        str_intend = ' ' * intend
+        str_intend = " " * intend
         if len(self) == 1:
             return str_intend + "%s%s.%s([%s])" % (
-                '' if not hasattr(self, 'arr_name') else self.arr_name + ': ',
-                self.__class__.__module__, self.__class__.__name__,
-                self[0].psy._short_info(intend+4, maybe=True))
+                "" if not hasattr(self, "arr_name") else self.arr_name + ": ",
+                self.__class__.__module__,
+                self.__class__.__name__,
+                self[0].psy._short_info(intend + 4, maybe=True),
+            )
         return str_intend + "%s%s.%s([\n%s])" % (
-            '' if not hasattr(self, 'arr_name') else self.arr_name + ': ',
-            self.__class__.__module__, self.__class__.__name__,
+            "" if not hasattr(self, "arr_name") else self.arr_name + ": ",
+            self.__class__.__module__,
+            self.__class__.__name__,
             ",\n".join(
-                '%s' % (
-                    arr.psy._short_info(intend+4))
-                for arr in self))
+                "%s" % (arr.psy._short_info(intend + 4)) for arr in self
+            ),
+        )
 
     def __str__(self):
         return self._short_info()
 
     def __repr__(self):
         return self.__str__()
 
     def __getitem__(self, key):
         """Overwrites lists __getitem__ by returning an ArrayList if `key` is a
         slice"""
         if isinstance(key, slice):  # return a new ArrayList
-            return self.__class__(
-                super(ArrayList, self).__getitem__(key))
+            return self.__class__(super(ArrayList, self).__getitem__(key))
         else:  # return the item
             return super(ArrayList, self).__getitem__(key)
 
     if six.PY2:  # for compatibility to python 2.7
+
         def __getslice__(self, *args):
             return self[slice(*args)]
 
-    def next_available_name(self, fmt_str='arr{0}', counter=None):
+    def next_available_name(self, fmt_str="arr{0}", counter=None):
         """Create a new array out of the given format string
 
         Parameters
         ----------
         format_str: str
             The base string to use. ``'{0}'`` will be replaced by a counter
         counter: iterable
@@ -4642,19 +5586,18 @@
         -------
         str
             A possible name that is not in the current project"""
         names = self.arr_names
         counter = counter or iter(range(1000))
         try:
             new_name = next(
-                filter(lambda n: n not in names,
-                       map(fmt_str.format, counter)))
+                filter(lambda n: n not in names, map(fmt_str.format, counter))
+            )
         except StopIteration:
-            raise ValueError(
-                "{0} already in the list".format(fmt_str))
+            raise ValueError("{0} already in the list".format(fmt_str))
         return new_name
 
     @docstrings.dedent
     def append(self, value, new_name=False):
         """
         Append a new array to the list
 
@@ -4690,17 +5633,21 @@
         ------
         %(ArrayList.rename.raises)s
 
         See Also
         --------
         list.extend, append, rename"""
         # extend those arrays that aren't alredy in the list
-        super(ArrayList, self).extend(t[0] for t in filter(
-            lambda t: t[1] is not None, (
-                self.rename(arr, new_name) for arr in iterable)))
+        super(ArrayList, self).extend(
+            t[0]
+            for t in filter(
+                lambda t: t[1] is not None,
+                (self.rename(arr, new_name) for arr in iterable),
+            )
+        )
 
     def remove(self, arr):
         """Removes an array from the list
 
         Parameters
         ----------
         arr: str or :class:`InteractiveBase`
@@ -4708,25 +5655,23 @@
 
         Raises
         ------
         ValueError
             If no array with the specified array name is in the list"""
         name = arr if isinstance(arr, six.string_types) else arr.psy.arr_name
         if arr not in self:
-            raise ValueError(
-                "Array {0} not in the list".format(name))
+            raise ValueError("Array {0} not in the list".format(name))
         for i, arr in enumerate(self):
             if arr.psy.arr_name == name:
                 del self[i]
                 return
-        raise ValueError(
-            "No array found with name {0}".format(name))
+        raise ValueError("No array found with name {0}".format(name))
 
 
-@xr.register_dataset_accessor('psy')
+@xr.register_dataset_accessor("psy")
 class DatasetAccessor(object):
     """A dataset accessor to interface with the psyplot package"""
 
     _filename = None
     _data_store = None
     _num = None
     _plot = None
@@ -4766,14 +5711,15 @@
 
         See Also
         --------
         psyplot.project.DatasetPlotter: for the different plot methods
         """
         if self._plot is None:
             import psyplot.project as psy
+
             self._plot = psy.DatasetPlotter(self.ds)
         return self._plot
 
     @property
     def filename(self):
         """The name of the file that stores this dataset"""
         fname = self._filename
@@ -4787,15 +5733,15 @@
 
     @property
     def data_store(self):
         """The :class:`xarray.backends.common.AbstractStore` used to save the
         dataset"""
         store_info = self._data_store
         if store_info is None or any(s is None for s in store_info):
-            store = getattr(self.ds, '_file_obj', None)
+            store = getattr(self.ds, "_file_obj", None)
             store_mod = store.__module__ if store is not None else None
             store_cls = store.__class__.__name__ if store is not None else None
             return store_mod, store_cls
         return store_info
 
     @data_store.setter
     def data_store(self, value):
@@ -4835,21 +5781,22 @@
     def __getitem__(self, key):
         ret = self.ds[key]
         if isinstance(ret, xr.DataArray):
             ret.psy.base = self.ds
         return ret
 
     def __getattr__(self, attr):
-        if attr != 'ds' and attr in self.ds:
+        if attr != "ds" and attr in self.ds:
             ret = getattr(self.ds, attr)
             ret.psy.base = self.ds
             return ret
         else:
-            raise AttributeError("%s has not Attribute %s" % (
-                self.__class__.__name__, attr))
+            raise AttributeError(
+                "%s has not Attribute %s" % (self.__class__.__name__, attr)
+            )
 
     def copy(self, deep=False):
         """Copy the array
 
         This method returns a copy of the underlying array in the :attr:`arr`
         attribute. It is more stable because it creates a new `psy` accessor"""
         ds = self.ds.copy(deep)
@@ -4860,16 +5807,17 @@
 class InteractiveList(ArrayList, InteractiveBase):
     """List of :class:`InteractiveArray` instances that can be plotted itself
 
     This class combines the :class:`ArrayList` and the interactive plotting
     through :class:`psyplot.plotter.Plotter` classes. It is mainly used by the
     :mod:`psyplot.plotter.simple` module"""
 
-    no_auto_update = property(_no_auto_update_getter,
-                              doc=_no_auto_update_getter.__doc__)
+    no_auto_update = property(
+        _no_auto_update_getter, doc=_no_auto_update_getter.__doc__
+    )
 
     @no_auto_update.setter
     def no_auto_update(self, value):
         ArrayList.no_auto_update.fset(self, value)
         InteractiveBase.no_auto_update.fset(self, value)
 
     @property
@@ -4883,43 +5831,55 @@
     @property
     def psy(self):
         """Return the list itself"""
         return self
 
     logger = InteractiveBase.logger
 
-    docstrings.delete_params('InteractiveBase.parameters', 'auto_update')
+    docstrings.delete_params("InteractiveBase.parameters", "auto_update")
 
     @docstrings.dedent
     def __init__(self, *args, **kwargs):
         """
         Parameters
         ----------
         %(ArrayList.parameters)s
         %(InteractiveBase.parameters.no_auto_update)s"""
         ibase_kwargs, array_kwargs = utils.sort_kwargs(
-            kwargs, ['plotter', 'arr_name'])
+            kwargs, ["plotter", "arr_name"]
+        )
         self._registered_updates = {}
         InteractiveBase.__init__(self, **ibase_kwargs)
         with self.block_signals:
             ArrayList.__init__(self, *args, **kwargs)
 
     @docstrings.dedent
-    def _register_update(self, method='isel', replot=False, dims={}, fmt={},
-                         force=False, todefault=False):
+    def _register_update(
+        self,
+        method="isel",
+        replot=False,
+        dims={},
+        fmt={},
+        force=False,
+        todefault=False,
+    ):
         """
         Register new dimensions and formatoptions for updating
 
         Parameters
         ----------
         %(InteractiveArray._register_update.parameters)s"""
         ArrayList._register_update(self, method=method, dims=dims)
-        InteractiveBase._register_update(self, fmt=fmt, todefault=todefault,
-                                         replot=bool(dims) or replot,
-                                         force=force)
+        InteractiveBase._register_update(
+            self,
+            fmt=fmt,
+            todefault=todefault,
+            replot=bool(dims) or replot,
+            force=force,
+        )
 
     @docstrings.dedent
     def start_update(self, draw=None, queues=None):
         """
         Conduct the formerly registered updates
 
         This method conducts the updates that have been registered via the
@@ -4952,32 +5912,35 @@
         if queues is not None:
             queues[0].task_done()
         return InteractiveBase.start_update(self, draw=draw, queues=queues)
 
     def to_dataframe(self):
         def to_df(arr):
             df = arr.to_pandas()
-            if hasattr(df, 'to_frame'):
+            if hasattr(df, "to_frame"):
                 df = df.to_frame()
             if not keep_names:
                 return df.rename(columns={df.keys()[0]: arr.psy.arr_name})
             return df
+
         if len(self) == 1:
             return self[0].to_series().to_frame()
         else:
             keep_names = len(set(arr.name for arr in self)) == self
             df = to_df(self[0])
             for arr in self[1:]:
-                df = df.merge(to_df(arr), left_index=True, right_index=True,
-                              how='outer')
+                df = df.merge(
+                    to_df(arr), left_index=True, right_index=True, how="outer"
+                )
             return df
 
-    docstrings.delete_params('ArrayList.from_dataset.parameters', 'plotter')
-    docstrings.delete_kwargs('ArrayList.from_dataset.other_parameters',
-                             'args', 'kwargs')
+    docstrings.delete_params("ArrayList.from_dataset.parameters", "plotter")
+    docstrings.delete_kwargs(
+        "ArrayList.from_dataset.other_parameters", "args", "kwargs"
+    )
 
     @classmethod
     @docstrings.dedent
     def from_dataset(cls, *args, **kwargs):
         """
         Create an InteractiveList instance from the given base dataset
 
@@ -4996,16 +5959,16 @@
         ``**kwargs``
             Further keyword arguments may point to any of the dimensions of the
             data (see `dims`)
 
         Returns
         -------
         %(ArrayList.from_dataset.returns)s"""
-        plotter = kwargs.pop('plotter', None)
-        make_plot = kwargs.pop('make_plot', True)
+        plotter = kwargs.pop("plotter", None)
+        make_plot = kwargs.pop("make_plot", True)
         instance = super(InteractiveList, cls).from_dataset(*args, **kwargs)
         if plotter is not None:
             plotter.initialize_plot(instance, make_plot=make_plot)
         return instance
 
     def extend(self, *args, **kwargs):
         # reimplemented to emit onupdate
@@ -5021,14 +5984,15 @@
         return self
 
 
 class _MissingModule(object):
     """Class that can be used if an optional module is not avaible.
 
     This class raises an error if any attribute is accessed or it is called"""
+
     def __init__(self, error):
         """
         Parameters
         ----------
         error: ImportError
             The error that has been raised when tried to import the module"""
         self.error = error
@@ -5051,18 +6015,20 @@
             pass
         else:
             if store_mod is not None and store_cls is not None:
                 if isstring(store_mod):
                     store_mod = repeat(store_mod)
                 if isstring(store_cls):
                     store_cls = repeat(store_cls)
-                fname = [_open_store(sm, sc, f)
-                         for sm, sc, f in zip(store_mod, store_cls, fname)]
-                kwargs['engine'] = None
-                kwargs['lock'] = False
+                fname = [
+                    _open_store(sm, sc, f)
+                    for sm, sc, f in zip(store_mod, store_cls, fname)
+                ]
+                kwargs["engine"] = None
+                kwargs["lock"] = False
                 return open_mfdataset(fname, **kwargs)
             else:
                 # try guessing with open_dataset
                 return open_mfdataset(fname, **kwargs)
     if store_mod is not None and store_cls is not None:
         fname = _open_store(store_mod, store_cls, fname)
     return open_dataset(fname, **kwargs)
@@ -5072,60 +6038,62 @@
     def decode(t):
         day = np.floor(t).astype(int)
         sub = t - day
         rest = dt.timedelta(days=sub)
         # round microseconds
         if rest.microseconds:
             rest += dt.timedelta(microseconds=1e6 - rest.microseconds)
-        return np.datetime64(dt.datetime.strptime(
-            "%i" % day, "%Y%m%d") + rest)
+        return np.datetime64(dt.datetime.strptime("%i" % day, "%Y%m%d") + rest)
+
     return np.vectorize(decode, [np.datetime64])(times)
 
 
 def encode_absolute_time(times):
     def encode(t):
         t = to_datetime(t)
-        return float(t.strftime('%Y%m%d')) + (
-            t - dt.datetime(t.year, t.month, t.day)).total_seconds() / 86400.
+        return (
+            float(t.strftime("%Y%m%d"))
+            + (t - dt.datetime(t.year, t.month, t.day)).total_seconds()
+            / 86400.0
+        )
+
     return np.vectorize(encode, [float])(times)
 
 
 class AbsoluteTimeDecoder(NDArrayMixin):
-
     def __init__(self, array):
         self.array = array
         example_value = first_n_items(array, 1) or 0
         try:
             result = decode_absolute_time(example_value)
         except Exception:
             logger.error("Could not interprete absolute time values!")
             raise
         else:
-            self._dtype = getattr(result, 'dtype', np.dtype('object'))
+            self._dtype = getattr(result, "dtype", np.dtype("object"))
 
     @property
     def dtype(self):
         return self._dtype
 
     def __getitem__(self, key):
         return decode_absolute_time(self.array[key])
 
 
 class AbsoluteTimeEncoder(NDArrayMixin):
-
     def __init__(self, array):
         self.array = array
         example_value = first_n_items(array, 1) or 0
         try:
             result = encode_absolute_time(example_value)
         except Exception:
             logger.error("Could not interprete absolute time values!")
             raise
         else:
-            self._dtype = getattr(result, 'dtype', np.dtype('object'))
+            self._dtype = getattr(result, "dtype", np.dtype("object"))
 
     @property
     def dtype(self):
         return self._dtype
 
     def __getitem__(self, key):
         return encode_absolute_time(self.array[key])
```

### Comparing `psyplot-1.4.3/psyplot/gdal_store.py` & `psyplot-1.5.0/psyplot/gdal_store.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,75 +7,61 @@
 
 Examples
 --------
 to open a GeoTIFF file named ``'my_tiff.tiff'`` you can do::
 
     >>> from psyplot.gdal_store import GdalStore
     >>> from xarray import open_dataset
-    >>> ds = open_dataset(GdalStore('my_tiff'))
+    >>> ds = open_dataset(GdalStore("my_tiff"))
 
 Or you use the `engine` of the :func:`psyplot.open_dataset` function:
 
-    >>> ds = open_dataset('my_tiff.tiff', engine='gdal')
+    >>> ds = open_dataset("my_tiff.tiff", engine="gdal")
 """
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
+
 
 import six
-from numpy import arange, nan, dtype
+from numpy import arange, dtype, nan
 from xarray import Variable
-from collections import OrderedDict
+from xarray.backends.common import AbstractDataStore
+
+import psyplot.data as psyd
+from psyplot.warning import warn
+
 try:
     from xarray.core.utils import FrozenOrderedDict
 except ImportError:
     FrozenOrderedDict = dict
-from xarray.backends.common import AbstractDataStore
-from psyplot.compat.pycompat import range
-from psyplot.warning import warn
-import psyplot.data as psyd
 try:
     import gdal
     from osgeo import gdal_array
 except ImportError as e:
     gdal = psyd._MissingModule(e)
 try:
     from dask.array import Array
+
     with_dask = True
 except ImportError:
     with_dask = False
 
 
 class GdalStore(AbstractDataStore):
     """Datastore to read raster files suitable for the gdal package
 
     We recommend to use the :func:`psyplot.open_dataset` function to open
     a geotiff file::
 
-        >>> ds = psyplot.open_dataset('my_geotiff.tiff', engine='gdal')
+        >>> ds = psyplot.open_dataset("my_geotiff.tiff", engine="gdal")
 
     Notes
     -----
     The :class:`GdalStore` object is not as elaborate as, for example, the
     `gdal_translate` command. Many attributes, e.g. variable names or netCDF
     dimensions will not be interpreted. We only support two
     dimensional arrays and each band is saved into one variable named like
@@ -106,64 +92,76 @@
             no_data = band.GetNoDataValue()
             if no_data is not None:
                 try:
                     a[a == no_data] = a.dtype.type(nan)
                 except ValueError:
                     pass
             return a
+
         ds = self.ds
-        dims = ['lat', 'lon']
+        dims = ["lat", "lon"]
         chunks = ((ds.RasterYSize,), (ds.RasterXSize,))
         shape = (ds.RasterYSize, ds.RasterXSize)
-        variables = OrderedDict()
-        for iband in range(1, ds.RasterCount+1):
+        variables = dict()
+        for iband in range(1, ds.RasterCount + 1):
             band = ds.GetRasterBand(iband)
             dt = dtype(gdal_array.codes[band.DataType])
             if with_dask:
-                dsk = {('x', 0, 0): (load, iband)}
-                arr = Array(dsk, 'x', chunks, shape=shape, dtype=dt)
+                dsk = {("x", 0, 0): (load, iband)}
+                arr = Array(dsk, "x", chunks, shape=shape, dtype=dt)
             else:
                 arr = load(iband)
             attrs = band.GetMetadata_Dict()
             try:
                 dt.type(nan)
-                attrs['_FillValue'] = nan
+                attrs["_FillValue"] = nan
             except ValueError:
                 no_data = band.GetNoDataValue()
-                attrs.update({'_FillValue': no_data} if no_data else {})
-            variables['Band%i' % iband] = Variable(dims, arr, attrs)
-        variables['lat'], variables['lon'] = self._load_GeoTransform()
+                attrs.update({"_FillValue": no_data} if no_data else {})
+            variables["Band%i" % iband] = Variable(dims, arr, attrs)
+        variables["lat"], variables["lon"] = self._load_GeoTransform()
         return FrozenOrderedDict(variables)
 
     def _load_GeoTransform(self):
         """Calculate latitude and longitude variable calculated from the
         gdal.Open.GetGeoTransform method"""
+
         def load_lon():
-            return arange(ds.RasterXSize)*b[1]+b[0]
+            return arange(ds.RasterXSize) * b[1] + b[0]
 
         def load_lat():
-            return arange(ds.RasterYSize)*b[5]+b[3]
+            return arange(ds.RasterYSize) * b[5] + b[3]
+
         ds = self.ds
         b = self.ds.GetGeoTransform()  # bbox, interval
         if with_dask:
             lat = Array(
-                {('lat', 0): (load_lat,)}, 'lat', (self.ds.RasterYSize,),
-                shape=(self.ds.RasterYSize,), dtype=float)
+                {("lat", 0): (load_lat,)},
+                "lat",
+                (self.ds.RasterYSize,),
+                shape=(self.ds.RasterYSize,),
+                dtype=float,
+            )
             lon = Array(
-                {('lon', 0): (load_lon,)}, 'lon', (self.ds.RasterXSize,),
-                shape=(self.ds.RasterXSize,), dtype=float)
+                {("lon", 0): (load_lon,)},
+                "lon",
+                (self.ds.RasterXSize,),
+                shape=(self.ds.RasterXSize,),
+                dtype=float,
+            )
         else:
             lat = load_lat()
             lon = load_lon()
-        return Variable(('lat',), lat), Variable(('lon',), lon)
+        return Variable(("lat",), lat), Variable(("lon",), lon)
 
     def get_attrs(self):
         from osr import SpatialReference
+
         attrs = self.ds.GetMetadata()
         try:
             sp = SpatialReference(wkt=self.ds.GetProjection())
             proj4 = sp.ExportToProj4()
-        except:
-            warn('Could not identify projection')
+        except Exception:
+            warn("Could not identify projection")
         else:
-            attrs['proj4'] = proj4
+            attrs["proj4"] = proj4
         return FrozenOrderedDict(attrs)
```

### Comparing `psyplot-1.4.3/psyplot/plotter.py` & `psyplot-1.5.0/psyplot/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,77 +1,66 @@
 """Core package for interactive visualization in the psyplot package
 
 This package defines the :class:`Plotter` and :class:`Formatoption` classes,
 the core of the visualization in the :mod:`psyplot` package. Each
 :class:`Plotter` combines a set of formatoption keys where each formatoption
 key is represented by a :class:`Formatoption` subclass."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
+import logging
 import weakref
 from abc import ABCMeta, abstractmethod
-from textwrap import TextWrapper
-import logging
-from itertools import chain, groupby, tee, repeat, starmap
 from collections import defaultdict
-from threading import RLock
 from datetime import datetime, timedelta
-from numpy import datetime64, timedelta64, ndarray, inf
-from xarray.core.formatting import format_timestamp, format_timedelta
+from itertools import chain, groupby, repeat, starmap, tee
+from textwrap import TextWrapper
+from threading import RLock
+
+import six
+from numpy import datetime64, inf, ndarray, timedelta64
+from xarray.core.formatting import format_timedelta, format_timestamp
+
 from psyplot import rcParams
-from psyplot.warning import warn, critical, PsyPlotRuntimeWarning
-from psyplot.compat.pycompat import map, filter, zip, range
 from psyplot.config.rcsetup import SubDict
-from psyplot.docstring import docstrings, dedent
-from psyplot.data import (
-    InteractiveList, _no_auto_update_getter, CFDecoder)
-from psyplot.utils import (DefaultOrderedDict, _TempBool, _temp_bool_prop,
-                           unique_everseen, check_key)
+from psyplot.data import CFDecoder, InteractiveList, _no_auto_update_getter
+from psyplot.docstring import dedent, docstrings
+from psyplot.utils import (
+    Defaultdict,
+    _temp_bool_prop,
+    _TempBool,
+    check_key,
+    unique_everseen,
+)
+from psyplot.warning import PsyPlotRuntimeWarning, warn
 
 #: the default function to use when printing formatoption infos (the default is
 #: use print or in the gui, use the help explorer)
 default_print_func = six.print_
 
 
 #: :class:`dict`. Mapping from group to group names
 groups = {
-    'data': 'Data manipulation formatoptions',
-    'axes': 'Axes formatoptions',
-    'labels': 'Label formatoptions',
-    'plotting': 'Plot formatoptions',
-    'post_processing': 'Post processing formatoptions',
-    'colors': 'Color coding formatoptions',
-    'misc': 'Miscallaneous formatoptions',
-    'ticks': 'Axis tick formatoptions',
-    'vector': 'Vector plot formatoptions',
-    'masking': 'Masking formatoptions',
-    'regression': 'Fitting formatoptions',
-    }
+    "data": "Data manipulation formatoptions",
+    "axes": "Axes formatoptions",
+    "labels": "Label formatoptions",
+    "plotting": "Plot formatoptions",
+    "post_processing": "Post processing formatoptions",
+    "colors": "Color coding formatoptions",
+    "misc": "Miscallaneous formatoptions",
+    "ticks": "Axis tick formatoptions",
+    "vector": "Vector plot formatoptions",
+    "masking": "Masking formatoptions",
+    "regression": "Fitting formatoptions",
+}
 
 
 def _identity(*args):
     """identity function to make no validation
 
     Returns
     -------
@@ -127,33 +116,40 @@
 
 
 def _child_property(childname):
     def get_x(self):
         return getattr(self.plotter, self._child_mapping[childname])
 
     return property(
-        get_x, doc=childname + " Formatoption instance in the plotter")
+        get_x, doc=childname + " Formatoption instance in the plotter"
+    )
 
 
 class FormatoptionMeta(ABCMeta):
     """Meta class for formatoptions
 
     This class serves as a meta class for formatoptions and allows a more
     efficient docstring generation by using the
     :attr:`psyplot.docstring.docstrings` when creating a new formatoption
     class"""
+
     def __new__(cls, clsname, bases, dct):
         """Assign an automatic documentation to the formatoption"""
-        doc = dct.get('__doc__')
+        doc = dct.get("__doc__")
         if doc is not None:
-            dct['__doc__'] = docstrings.dedent(doc)
-        new_cls = super(FormatoptionMeta, cls).__new__(cls, clsname, bases,
-                                                       dct)
-        for childname in chain(new_cls.children, new_cls.dependencies,
-                               new_cls.connections, new_cls.parents):
+            dct["__doc__"] = docstrings.dedent(doc)
+        new_cls = super(FormatoptionMeta, cls).__new__(
+            cls, clsname, bases, dct
+        )
+        for childname in chain(
+            new_cls.children,
+            new_cls.dependencies,
+            new_cls.connections,
+            new_cls.parents,
+        ):
             setattr(new_cls, childname, _child_property(childname))
         if new_cls.plot_fmt:
             new_cls.data_dependent = True
         return new_cls
 
 
 # priority values
@@ -226,15 +222,15 @@
 
     #: :class:`bool`. True if an update of this formatoption requires a
     #: clearing of the axes and reinitialization of the plot
     requires_clearing = False
 
     #: :class:`str`. Key of the group name in :data:`groups` of this
     #: formatoption keyword
-    group = 'misc'
+    group = "misc"
 
     #: :class:`bool` or a callable. This attribute indicates whether this
     #: :class:`Formatoption` depends on the data and should be updated if the
     #: data changes. If it is a callable, it must accept one argument: the
     #: new data. (Note: This is automatically set to True for plot
     #: formatoptions)
     data_dependent = False
@@ -293,35 +289,39 @@
 
     @property
     def groupname(self):
         """Long name of the group this formatoption belongs too."""
         try:
             return groups[self.group]
         except KeyError:
-            warn("Unknown formatoption group " + str(self.group),
-                 PsyPlotRuntimeWarning)
+            warn(
+                "Unknown formatoption group " + str(self.group),
+                PsyPlotRuntimeWarning,
+            )
             return self.group
 
     @property
     def raw_data(self):
         """The original data of the plotter of this formatoption"""
         if self.index_in_list is not None and isinstance(
-                self.plotter.data, InteractiveList):
+            self.plotter.data, InteractiveList
+        ):
             return self.plotter.data[self.index_in_list]
         else:
             return self.plotter.data
 
     @property
     def decoder(self):
         """The :class:`~psyplot.data.CFDecoder` instance that decodes the
         :attr:`raw_data`"""
         # If the decoder is modified by one of the formatoptions, use this one
         if self.plotter.plot_data_decoder is not None:
             if self.index_in_list is not None and isinstance(
-                    self.plotter.plot_data, InteractiveList):
+                self.plotter.plot_data, InteractiveList
+            ):
                 ret = self.plotter.plot_data_decoder[self.index_in_list]
                 if ret is not None:
                     return ret
             else:
                 return self.plotter.plot_data_decoder
         data = self.raw_data
         check = isinstance(data, InteractiveList)
@@ -342,15 +342,16 @@
             ret = ret[0]
         return ret
 
     @property
     def data(self):
         """The data that is plotted"""
         if self.index_in_list is not None and isinstance(
-                self.plotter.plot_data, InteractiveList):
+            self.plotter.plot_data, InteractiveList
+        ):
             return self.plotter.plot_data[self.index_in_list]
         else:
             return self.plotter.plot_data
 
     @data.setter
     def data(self, value):
         self.set_data(value, self.index_in_list)
@@ -376,17 +377,21 @@
         """Validation method of the formatoption"""
         try:
             return self._validate
         except AttributeError:
             try:
                 self._validate = self.plotter.get_vfunc(self.key)
             except KeyError:
-                warn("Could not find a validation function for %s "
-                     "formatoption keyword! No validation will be made!" % (
-                         self.key), PsyPlotRuntimeWarning, logger=self.logger)
+                warn(
+                    "Could not find a validation function for %s "
+                    "formatoption keyword! No validation will be made!"
+                    % (self.key),
+                    PsyPlotRuntimeWarning,
+                    logger=self.logger,
+                )
                 self._validate = _identity
         return self._validate
 
     @validate.setter
     def validate(self, value):
         self._validate = value
 
@@ -436,19 +441,25 @@
     @dedent
     def value2pickle(self):
         """
         The value that can be used when pickling the information of the project
         """
         return self.value
 
-    @docstrings.get_sections(base='Formatoption')
+    @docstrings.get_sections(base="Formatoption")
     @dedent
-    def __init__(self, key, plotter=None, index_in_list=None,
-                 additional_children=[], additional_dependencies=[],
-                 **kwargs):
+    def __init__(
+        self,
+        key,
+        plotter=None,
+        index_in_list=None,
+        additional_children=[],
+        additional_dependencies=[],
+        **kwargs,
+    ):
         """
         Parameters
         ----------
         key: str
             formatoption key in the `plotter`
         plotter: psyplot.plotter.Plotter
             Plotter instance that holds this formatoption. If None, it is
@@ -472,56 +483,73 @@
         self.plotter = plotter
         self.index_in_list = index_in_list
         self.shared = set()
         self.additional_children = additional_children
         self.additional_dependencies = additional_dependencies
         self.children = self.children + additional_children
         self.dependencies = self.dependencies + additional_dependencies
-        self._child_mapping = dict(zip(*tee(chain(
-            self.children, self.dependencies, self.connections,
-            self.parents), 2)))
+        self._child_mapping = dict(
+            zip(
+                *tee(
+                    chain(
+                        self.children,
+                        self.dependencies,
+                        self.connections,
+                        self.parents,
+                    ),
+                    2,
+                )
+            )
+        )
         # check kwargs
         for key in (key for key in kwargs if key not in self._child_mapping):
             raise TypeError(
-                '%s.__init__() got an unexpected keyword argument %r' % (
-                    self.__class__.__name__, key))
+                "%s.__init__() got an unexpected keyword argument %r"
+                % (self.__class__.__name__, key)
+            )
         # set up child mapping
         self._child_mapping.update(kwargs)
         # reset the dependency lists to match the current plotter setup
-        for attr in ['children', 'dependencies', 'connections', 'parents']:
-            setattr(self, attr,
-                    [self._child_mapping[key] for key in getattr(self, attr)])
+        for attr in ["children", "dependencies", "connections", "parents"]:
+            setattr(
+                self,
+                attr,
+                [self._child_mapping[key] for key in getattr(self, attr)],
+            )
 
     def __set__(self, instance, value):
         if isinstance(value, Formatoption):
-            setattr(instance, '_' + self.key, value)
+            setattr(instance, "_" + self.key, value)
         else:
             fmto = getattr(instance, self.key)
             fmto.set_value(value)
 
     def __get__(self, instance, owner):
         if instance is None:
             return self
         try:
-            return getattr(instance, '_' + self.key)
+            return getattr(instance, "_" + self.key)
         except AttributeError:
             fmto = self.__class__(
-                self.key, instance, self.index_in_list,
+                self.key,
+                instance,
+                self.index_in_list,
                 additional_children=self.additional_children,
                 additional_dependencies=self.additional_dependencies,
-                **self.init_kwargs)
-            setattr(instance, '_' + self.key, fmto)
+                **self.init_kwargs,
+            )
+            setattr(instance, "_" + self.key, fmto)
             return fmto
 
     def __delete__(self, instance, owner):
-        fmto = getattr(instance, '_' + self.key)
+        fmto = getattr(instance, "_" + self.key)
         with instance.no_validation:
             instance[self.key] = fmto.default
 
-    @docstrings.get_sections(base='Formatoption.set_value')
+    @docstrings.get_sections(base="Formatoption.set_value")
     @dedent
     def set_value(self, value, validate=True, todefault=False):
         """
         Set (and validate) the value in the plotter. This method is called by
         the plotter when it attempts to change the value of the formatoption.
 
         Parameters
@@ -532,16 +560,17 @@
             if True, validate the `value` before it is set
         todefault: bool
             True if the value is updated to the default value"""
         # do nothing if the key is shared
         if self.key in self.plotter._shared:
             return
         with self.plotter.no_validation:
-            self.plotter[self.key] = value if not validate else \
-                self.validate(value)
+            self.plotter[self.key] = (
+                value if not validate else self.validate(value)
+            )
 
     def set_data(self, data, i=None):
         """
         Replace the data to plot
 
         This method may be used to replace the data that is visualized by the
         plotter. It changes it's behaviour depending on whether an
@@ -558,16 +587,17 @@
 
         Notes
         -----
         This method uses the :attr:`Formatoption.data` attribute
         """
         if self.index_in_list is not None:
             i = self.index_in_list
-        if i is not None and isinstance(self.plotter.plot_data,
-                                        InteractiveList):
+        if i is not None and isinstance(
+            self.plotter.plot_data, InteractiveList
+        ):
             self.plotter.plot_data[i] = data
         else:
             self.plotter.plot_data = data
 
     def set_decoder(self, decoder, i=None):
         """
         Replace the data to plot
@@ -584,30 +614,33 @@
         i: int
             The position in the InteractiveList where to insert the data (if
             the plotter visualizes a list anyway)
         """
         # we do not modify the raw data but instead set it on the plotter
         # TODO: This is not safe for encapsulated InteractiveList instances!
         if i is not None and isinstance(
-                self.plotter.plot_data, InteractiveList):
+            self.plotter.plot_data, InteractiveList
+        ):
             n = len(self.plotter.plot_data)
             decoders = self.plotter.plot_data_decoder or [None] * n
             decoders[i] = decoder
             self.plotter.plot_data_decoder = decoders
         else:
-            if (isinstance(self.plotter.plot_data, InteractiveList) and
-                    isinstance(decoder, CFDecoder)):
+            if isinstance(
+                self.plotter.plot_data, InteractiveList
+            ) and isinstance(decoder, CFDecoder):
                 decoder = [decoder] * len(self.plotter.plot_data)
             self.plotter.plot_data_decoder = decoder
 
     def get_decoder(self, i=None):
         # we do not modify the raw data but instead set it on the plotter
         # TODO: This is not safe for encapsulated InteractiveList instances!
         if i is not None and isinstance(
-                self.plotter.plot_data, InteractiveList):
+            self.plotter.plot_data, InteractiveList
+        ):
             n = len(self.plotter.plot_data)
             decoders = self.plotter.plot_data_decoder or [None] * n
             return decoders[i] or self.plotter.plot_data[i].psy.decoder
         else:
             return self.decoder
 
     def check_and_set(self, value, todefault=False, validate=True):
@@ -751,15 +784,15 @@
         necessarily have to implement this formatoption if your plot results
         are removed by the usual :meth:`matplotlib.axes.Axes.clear` method."""
         pass
 
     @docstrings.get_extended_summary(base="Formatoption.convert_coordinate")
     @docstrings.get_sections(
         base="Formatoption.convert_coordinate",
-        sections=["Parameters", "Returns"]
+        sections=["Parameters", "Returns"],
     )
     def convert_coordinate(self, coord, *variables):
         """Convert a coordinate to units necessary for the plot.
 
         This method takes a single coordinate variable (e.g. the `bounds` of a
         coordinate, or the coordinate itself) and transforms the units that the
         plotter requires.
@@ -843,52 +876,58 @@
         Only run post processing scripts when the data changes or a replot
         is necessary
 
     See Also
     --------
     post: The post processing formatoption"""
 
-    default = 'never'
+    default = "never"
 
     priority = -inf
 
-    group = 'post_processing'
+    group = "post_processing"
 
-    name = 'Timing of the post processing'
+    name = "Timing of the post processing"
 
     @staticmethod
     def validate(value):
         value = six.text_type(value)
-        possible_values = ['never', 'always', 'replot']
+        possible_values = ["never", "always", "replot"]
         if value not in possible_values:
-            raise ValueError('String must be one of %s, not %r' % (
-                possible_values, value))
+            raise ValueError(
+                "String must be one of %s, not %r" % (possible_values, value)
+            )
         return value
 
     def update(self, value):
         pass
 
     def get_fmt_widget(self, parent, project):
         from psyplot_gui.compat.qtcompat import QComboBox
+
         combo = QComboBox(parent)
-        combo.addItems(['never', 'always', 'replot'])
+        combo.addItems(["never", "always", "replot"])
         combo.setCurrentText(
-            next((plotter[self.key] for plotter in project.plotters), 'never'))
+            next((plotter[self.key] for plotter in project.plotters), "never")
+        )
         combo.currentTextChanged.connect(parent.set_obj)
         return combo
 
 
 class PostProcDependencies(object):
     """The dependencies of this formatoption"""
 
     def __get__(self, instance, owner):
-        if (instance is None or instance.plotter is None or
-                not instance.plotter._initialized):
+        if (
+            instance is None
+            or instance.plotter is None
+            or not instance.plotter._initialized
+        ):
             return []
-        elif instance.post_timing.value == 'always':
+        elif instance.post_timing.value == "always":
             return list(set(instance.plotter) - {instance.key})
         else:
             return []
 
     def __set__(self, instance, value):
         pass
 
@@ -922,114 +961,121 @@
     Assume, you want to manually add the mean of the data to the title of the
     matplotlib axes. You can simply do this via
 
     .. code-block:: python
 
         from psyplot.plotter import Plotter
         from xarray import DataArray
+
         plotter = Plotter(DataArray([1, 2, 3]))
         # enable the post formatoption
         plotter.enable_post = True
         plotter.update(post="self.ax.set_title(str(self.data.mean()))")
         plotter.ax.get_title()
-        '2.0'
+        "2.0"
 
     By default, the ``post`` formatoption is only ran, when it is explicitly
     updated. However, you can use the :attr:`post_timing` formatoption, to
     run it automatically. E.g. for running it after every update of the
     plotter, you can set
 
     .. code-block:: python
 
-        plotter.update(post_timing='always')
+        plotter.update(post_timing="always")
 
     See Also
     --------
     post_timing: Determine the timing of this formatoption"""
 
-    children = ['post_timing']
+    children = ["post_timing"]
 
     default = None
 
     priority = -inf
 
-    group = 'post_processing'
+    group = "post_processing"
 
-    name = 'Custom post processing script'
+    name = "Custom post processing script"
 
     @staticmethod
     def validate(value):
         if value is None:
             return value
         elif not isinstance(value, six.string_types):
-            raise ValueError("Expected a string, not %s" % (type(value), ))
+            raise ValueError("Expected a string, not %s" % (type(value),))
         else:
             return six.text_type(value)
 
     @property
     def data_dependent(self):
         """True if the corresponding :class:`post_timing <PostTiming>`
         formatoption is set to ``'replot'`` to run the post processing script
         after every change of the data"""
-        return self.post_timing.value == 'replot'
+        return self.post_timing.value == "replot"
 
     dependencies = PostProcDependencies()
 
     def update(self, value):
         if value is None:
             return
         if not self.plotter.enable_post:
             warn(
                 "Post processing is disabled. Set the ``enable_post`` "
-                "attribute to True to run the script")
+                "attribute to True to run the script"
+            )
         else:
-            exec(value, {'self': self})
+            exec(value, {"self": self})
 
 
 class Plotter(dict):
     """Interactive plotting object for one or more data arrays
 
     This class is the base for the interactive plotting with the psyplot
     module. It capabilities are determined by it's descriptor classes that are
     derived from the :class:`Formatoption` class"""
 
     #: List of base strings in the :attr:`psyplot.rcParams` dictionary
     _rcparams_string = []
 
-    post_timing = PostTiming('post_timing')
-    post = PostProcessing('post')
+    post_timing = PostTiming("post_timing")
+    post = PostProcessing("post")
 
-    no_validation = _temp_bool_prop('no_validation', """
+    no_validation = _temp_bool_prop(
+        "no_validation",
+        """
         Temporarily disable the validation
 
         Examples
         --------
         Although it is not recommended to set a value with disabled validation,
         you can disable it via::
 
             >>> with plotter.no_validation:
-            ...     plotter['ticksize'] = 'x'
+            ...     plotter["ticksize"] = "x"
+            ...
 
         To permanently disable the validation, simply set
 
             >>> plotter.no_validation = True
-            >>> plotter['ticksize'] = 'x'
-            >>> plotter.no_validation = False  # reenable validation""")
+            >>> plotter["ticksize"] = "x"
+            >>> plotter.no_validation = False  # reenable validation""",
+    )
 
     #: Temporarily include links in the key descriptions from
     #: :meth:`show_keys`, :meth:`show_docs` and :meth:`show_summaries`.
     #: Note that this is a class attribute, so each change to the value of this
     #: attribute will affect all instances and subclasses
     include_links = _TempBool()
 
     @property
     def ax(self):
         """Axes instance of the plot"""
         if self._ax is None:
             import matplotlib.pyplot as plt
+
             plt.figure()
             self._ax = plt.axes(projection=self._get_sample_projection())
         return self._ax
 
     @ax.setter
     def ax(self, value):
         self._ax = value
@@ -1067,41 +1113,50 @@
             self._set_rc()
             return self._rc
 
     @property
     def base_variables(self):
         """A mapping from the base_variable names to the variables"""
         if isinstance(self.data, InteractiveList):
-            return dict(chain(*map(
-                lambda arr: six.iteritems(arr.psy.base_variables),
-                self.data)))
+            return dict(
+                chain(
+                    *map(
+                        lambda arr: six.iteritems(arr.psy.base_variables),
+                        self.data,
+                    )
+                )
+            )
         else:
             return self.data.psy.base_variables
 
     @property
     def iter_base_variables(self):
         """A mapping from the base_variable names to the variables"""
         if isinstance(self.data, InteractiveList):
             return chain(*(arr.psy.iter_base_variables for arr in self.data))
         else:
             return self.data.psy.iter_base_variables
 
-    no_auto_update = property(_no_auto_update_getter,
-                              doc=_no_auto_update_getter.__doc__)
+    no_auto_update = property(
+        _no_auto_update_getter, doc=_no_auto_update_getter.__doc__
+    )
 
     @no_auto_update.setter
     def no_auto_update(self, value):
         self.no_auto_update.value = bool(value)
 
     @property
     def changed(self):
         """:class:`dict` containing the key value pairs that are not the
         default"""
-        return {key: value for key, value in six.iteritems(self)
-                if getattr(self, key).changed}
+        return {
+            key: value
+            for key, value in six.iteritems(self)
+            if getattr(self, key).changed
+        }
 
     @property
     def figs2draw(self):
         """All figures that have been manipulated through sharing and the own
         figure.
 
         Notes
@@ -1151,15 +1206,15 @@
     @data.setter
     def data(self, value):
         self._data = value
 
     @property
     def plot_data(self):
         """The data that is used for plotting"""
-        return getattr(self, '_plot_data', self.data)
+        return getattr(self, "_plot_data", self.data)
 
     @plot_data.setter
     def plot_data(self, value):
         self._set_data(value)
 
     #: The decoder to use for the formatoptions. If None, the decoder of the
     #: raw data is used
@@ -1177,24 +1232,33 @@
 
     @property
     def logger(self):
         """:class:`logging.Logger` of this plotter"""
         try:
             return self.data.psy.logger.getChild(self.__class__.__name__)
         except AttributeError:
-            name = '%s.%s' % (self.__module__, self.__class__.__name__)
+            name = "%s.%s" % (self.__module__, self.__class__.__name__)
             return logging.getLogger(name)
 
-    docstrings.keep_params('InteractiveBase.parameters', 'auto_update')
+    docstrings.keep_params("InteractiveBase.parameters", "auto_update")
 
-    @docstrings.get_sections(base='Plotter')
+    @docstrings.get_sections(base="Plotter")
     @docstrings.dedent
-    def __init__(self, data=None, ax=None, auto_update=None, project=None,
-                 draw=False, make_plot=True, clear=False,
-                 enable_post=False, **kwargs):
+    def __init__(
+        self,
+        data=None,
+        ax=None,
+        auto_update=None,
+        project=None,
+        draw=False,
+        make_plot=True,
+        clear=False,
+        enable_post=False,
+        **kwargs,
+    ):
         """
         Parameters
         ----------
         data: InteractiveArray or ArrayList, optional
             Data object that shall be visualized. If given and `plot` is True,
             the :meth:`initialize_plot` method is called at the end. Otherwise
             you can call this method later by yourself
@@ -1215,15 +1279,15 @@
             Any formatoption key from the :attr:`formatoptions` attribute that
             shall be used"""
         self.project = project
         self.ax = ax
         self.data = data
         self.enable_post = enable_post
         if auto_update is None:
-            auto_update = rcParams['lists.auto_update']
+            auto_update = rcParams["lists.auto_update"]
         self.no_auto_update = not bool(auto_update)
         self._registered_updates = {}
         self._todefault = False
         self._old_fmt = []
         self._figs2draw = set()
         #: formatoptions that have to be updated by other plotters that share
         #: the given formatoption with this Plotter. :attr:`_to_update` is a
@@ -1253,16 +1317,17 @@
                 self[key] = None
         for key in self:  # then we set the default values
             fmto = getattr(self, key)
             self._try2set(fmto, fmto.default, validate=False)
         self._set_rc()
         for key, value in six.iteritems(kwargs):  # then the user values
             self[key] = value
-        self.initialize_plot(data, ax=ax, draw=draw, clear=clear,
-                             make_plot=make_plot)
+        self.initialize_plot(
+            data, ax=ax, draw=draw, clear=clear, make_plot=make_plot
+        )
 
     def _try2set(self, fmto, *args, **kwargs):
         """Sets the value in `fmto` and gives additional informations when fail
 
         Parameters
         ----------
         fmto: Formatoption
@@ -1286,15 +1351,15 @@
         getattr(self, key).lock.acquire()
         dict.__setitem__(self, key, value)
         getattr(self, key).lock.release()
 
     def __delitem__(self, key):
         self[key] = getattr(self, key).default
 
-    docstrings.delete_params('check_key.parameters', 'possible_keys', 'name')
+    docstrings.delete_params("check_key.parameters", "possible_keys", "name")
 
     @docstrings.dedent
     def check_key(self, key, raise_error=True, *args, **kwargs):
         """
         Checks whether the key is a valid formatoption
 
         Parameters
@@ -1305,20 +1370,26 @@
         -------
         %(check_key.returns)s
 
         Raises
         ------
         %(check_key.raises)s"""
         return check_key(
-            key, possible_keys=list(self), raise_error=raise_error,
-            name='formatoption keyword', *args, **kwargs)
+            key,
+            possible_keys=list(self),
+            raise_error=raise_error,
+            name="formatoption keyword",
+            *args,
+            **kwargs,
+        )
 
     @classmethod
-    @docstrings.get_sections(base='Plotter.check_data', sections=['Parameters',
-                                                              'Returns'])
+    @docstrings.get_sections(
+        base="Plotter.check_data", sections=["Parameters", "Returns"]
+    )
     @dedent
     def check_data(cls, name, dims, is_unstructured):
         """
         A validation method for the data shape
 
         The default method does nothing and should be subclassed to validate
         the results. If the plotter accepts a :class:`InteractiveList`, it
@@ -1345,24 +1416,33 @@
         if isinstance(name, six.string_types):
             name = [name]
             dims = [dims]
             is_unstructured = [is_unstructured]
         N = len(name)
         if len(dims) != N or len(is_unstructured) != N:
             return [False] * N, [
-                'Number of provided names (%i) and dimensions '
-                '(%i) or unstructured information (%i) are not the same' % (
-                    N, len(dims), len(is_unstructured))] * N
-        return [True] * N, [''] * N
+                "Number of provided names (%i) and dimensions "
+                "(%i) or unstructured information (%i) are not the same"
+                % (N, len(dims), len(is_unstructured))
+            ] * N
+        return [True] * N, [""] * N
 
-    docstrings.keep_params('Plotter.parameters', 'ax', 'make_plot', 'clear')
+    docstrings.keep_params("Plotter.parameters", "ax", "make_plot", "clear")
 
     @docstrings.dedent
-    def initialize_plot(self, data=None, ax=None, make_plot=True, clear=False,
-                        draw=False, remove=False, priority=None):
+    def initialize_plot(
+        self,
+        data=None,
+        ax=None,
+        make_plot=True,
+        clear=False,
+        draw=False,
+        remove=False,
+        priority=None,
+    ):
         """
         Initialize the plot for a data array
 
         Parameters
         ----------
         data: InteractiveArray or ArrayList, optional
             Data object that shall be visualized.
@@ -1385,62 +1465,71 @@
             data = self.data
         else:
             self.data = data
         self.ax = ax
         if data is None:  # nothing to do if no data is given
             return
         self.no_auto_update = not (
-            not self.no_auto_update or not data.psy.no_auto_update)
+            not self.no_auto_update or not data.psy.no_auto_update
+        )
         data.psy.plotter = self
         if not make_plot:  # stop here if we shall not plot
             return
         self.logger.debug("Initializing plot...")
         if remove:
             self.logger.debug("    Removing old formatoptions...")
             for fmto in self._fmtos:
                 try:
                     fmto.remove()
                 except Exception:
                     self.logger.debug(
-                        "Could not remove %s while initializing", fmto.key,
-                        exc_info=True)
+                        "Could not remove %s while initializing",
+                        fmto.key,
+                        exc_info=True,
+                    )
         if clear:
             self.logger.debug("    Clearing axes...")
             self.ax.clear()
             self.cleared = True
         # get the formatoptions. We sort them here by key to make sure that the
         # order always stays the same (easier for debugging)
-        fmto_groups = self._grouped_fmtos(self._sorted_by_priority(
-            sorted(self._fmtos, key=lambda fmto: fmto.key)))
+        fmto_groups = self._grouped_fmtos(
+            self._sorted_by_priority(
+                sorted(self._fmtos, key=lambda fmto: fmto.key)
+            )
+        )
         self.plot_data = self.data
         self._updating = True
         for fmto_priority, grouper in fmto_groups:
             if priority is None or fmto_priority == priority:
-                self._plot_by_priority(fmto_priority, grouper,
-                                       initializing=True)
+                self._plot_by_priority(
+                    fmto_priority, grouper, initializing=True
+                )
         self._release_all(True)  # finish the update
         self.cleared = False
         self.replot = False
         self._initialized = True
         self._updating = False
 
         if draw is None:
-            draw = rcParams['auto_draw']
+            draw = rcParams["auto_draw"]
         if draw:
             self.draw()
-            if rcParams['auto_show']:
+            if rcParams["auto_show"]:
                 self.show()
 
-    docstrings.keep_params('InteractiveBase._register_update.parameters',
-                           'force', 'todefault')
+    docstrings.keep_params(
+        "InteractiveBase._register_update.parameters", "force", "todefault"
+    )
 
-    @docstrings.get_sections(base='Plotter._register_update')
+    @docstrings.get_sections(base="Plotter._register_update")
     @docstrings.dedent
-    def _register_update(self, fmt={}, replot=False, force=False,
-                         todefault=False):
+    def _register_update(
+        self, fmt={}, replot=False, force=False, todefault=False
+    ):
         """
         Register formatoptions for the update
 
         Parameters
         ----------
         fmt: dict
             Keys can be any valid formatoptions with the corresponding values
@@ -1452,15 +1541,16 @@
         if self.disabled:
             return
         self.replot = self.replot or replot
         self._todefault = self._todefault or todefault
         if force is True:
             force = list(fmt)
         self._force.update(
-            [ret[0] for ret in map(self.check_key, force or [])])
+            [ret[0] for ret in map(self.check_key, force or [])]
+        )
         # check the keys
         list(map(self.check_key, fmt))
         self._registered_updates.update(fmt)
 
     def make_plot(self):
         """Method for making the plot
 
@@ -1485,35 +1575,41 @@
         Returns
         -------
         %(InteractiveBase.start_update.returns)s
 
         See Also
         --------
         :attr:`no_auto_update`, update"""
+
         def update_the_others():
             for fmto in fmtos:
                 for other_fmto in fmto.shared:
                     if not other_fmto.plotter._updating:
                         other_fmto.plotter._register_update(
-                            force=[other_fmto.key])
+                            force=[other_fmto.key]
+                        )
             for fmto in fmtos:
                 for other_fmto in fmto.shared:
                     if not other_fmto.plotter._updating:
                         other_draw = other_fmto.plotter.start_update(
-                            draw=False, update_shared=False)
+                            draw=False, update_shared=False
+                        )
                         if other_draw:
                             self._figs2draw.add(
-                                other_fmto.plotter.ax.get_figure())
+                                other_fmto.plotter.ax.get_figure()
+                            )
+
         if self.disabled:
             return False
 
         if queues is not None:
             queues[0].get()
-        self.logger.debug("Starting update of %r",
-                          self._registered_updates.keys())
+        self.logger.debug(
+            "Starting update of %r", self._registered_updates.keys()
+        )
         # update the formatoptions
         self._save_state()
         try:
             # get the formatoptions. We sort them here by key to make sure that
             # the order always stays the same (easier for debugging)
             fmtos = sorted(self._set_and_filter(), key=lambda fmto: fmto.key)
         except Exception:
@@ -1532,16 +1628,21 @@
                 fmto2.plotter._to_update[fmto2] = self
         if queues is not None:
             self._updating = True
             queues[0].task_done()
             # wait for the other tasks to finish
             queues[0].join()
             queues[1].get()
-        fmtos.extend([fmto for fmto in self._insert_additionals(list(
-            self._to_update)) if fmto not in fmtos])
+        fmtos.extend(
+            [
+                fmto
+                for fmto in self._insert_additionals(list(self._to_update))
+                if fmto not in fmtos
+            ]
+        )
         self._to_update.clear()
 
         fmto_groups = self._grouped_fmtos(self._sorted_by_priority(fmtos[:]))
         # if any formatoption requires a clearing of the axes is updated,
         # we reinitialize the plot
         try:
             if self.cleared:
@@ -1555,49 +1656,53 @@
                     arr_draw = True
                     self._plot_by_priority(priority, grouper)
                 update_the_others()
         except Exception:
             raise
         finally:
             # make sure that all locks are released
-            self._release_all(finish=True,
-                              queue=None if queues is None else queues[1])
+            self._release_all(
+                finish=True, queue=None if queues is None else queues[1]
+            )
         if draw is None:
-            draw = rcParams['auto_draw']
+            draw = rcParams["auto_draw"]
         if draw and arr_draw:
             self.draw()
-            if rcParams['auto_show']:
+            if rcParams["auto_show"]:
                 self.show()
         self.replot = False
         return arr_draw
 
     def _release_all(self, finish=False, queue=None):
         # make sure that all locks are released
         try:
             for fmto in self._fmtos:
                 if finish:
                     fmto.finish_update()
                 try:
                     fmto.lock.release()
                 except RuntimeError:
                     pass
-        except:
+        except Exception:
             raise
         finally:
             if queue is not None:
                 queue.task_done()
                 queue.join()
             self._updating = False
 
     def _plot_by_priority(self, priority, fmtos, initializing=False):
         def update(fmto):
             other_fmto = self._shared.get(fmto.key)
             if other_fmto:
-                self.logger.debug("%s is shared with %s", fmto.key,
-                                  other_fmto.plotter.logger.name)
+                self.logger.debug(
+                    "%s is shared with %s",
+                    fmto.key,
+                    other_fmto.plotter.logger.name,
+                )
                 other_fmto.share(fmto, initializing=initializing)
             # but if not, share them
             else:
                 if initializing:
                     self.logger.debug("Initializing %s", fmto.key)
                     fmto.initialize_plot(fmto.value)
                 else:
@@ -1608,15 +1713,17 @@
             except RuntimeError:
                 pass
 
         self._initializing = initializing
 
         self.logger.debug(
             "%s formatoptions with priority %i",
-            "Initializing" if initializing else "Updating", priority)
+            "Initializing" if initializing else "Updating",
+            priority,
+        )
 
         if priority >= START or priority == END:
             for fmto in fmtos:
                 update(fmto)
         elif priority == BEFOREPLOTTING:
             for fmto in fmtos:
                 update(fmto)
@@ -1639,17 +1746,20 @@
         --------
         The axes may be cleared when calling this method (even if `clear` is
         set to False)!"""
         # call the initialize_plot method. Note that clear can be set to
         # False if any fmto has requires_clearing attribute set to True,
         # because this then has been cleared before
         self.initialize_plot(
-            self.data, self._ax, draw=draw, clear=clear or any(
-                fmto.requires_clearing for fmto in self._fmtos),
-            remove=True)
+            self.data,
+            self._ax,
+            draw=draw,
+            clear=clear or any(fmto.requires_clearing for fmto in self._fmtos),
+            remove=True,
+        )
 
     def draw(self):
         """Draw the figures and those that are shared and have been changed"""
         for fig in self.figs2draw:
             fig.canvas.draw()
         self._figs2draw.clear()
 
@@ -1657,14 +1767,15 @@
         def key_func(fmto):
             if fmto.priority >= START:
                 return START
             elif fmto.priority >= BEFOREPLOTTING:
                 return BEFOREPLOTTING
             else:
                 return END
+
         return groupby(fmtos, key_func)
 
     def _set_and_filter(self):
         """Filters the registered updates and sort out what is not needed
 
         This method filters out the formatoptions that have not changed, sets
         the new value and returns an iterable that is sorted by the priority
@@ -1675,40 +1786,47 @@
         list
             list of :class:`Formatoption` objects that have to be updated"""
         fmtos = []
         seen = set()
         for key in self._force:
             self._registered_updates.setdefault(key, getattr(self, key).value)
         for key, value in chain(
-                six.iteritems(self._registered_updates),
-                six.iteritems(
-                    {key: getattr(self, key).default for key in self})
-                if self._todefault else ()):
+            six.iteritems(self._registered_updates),
+            six.iteritems({key: getattr(self, key).default for key in self})
+            if self._todefault
+            else (),
+        ):
             if key in seen:
                 continue
             seen.add(key)
             fmto = getattr(self, key)
             # if the key is shared, a warning will be printed as long as
             # this plotter is not also updating (for example due to a whole
             # project update)
             if key in self._shared and key not in self._force:
                 if not self._shared[key].plotter._updating:
-                    warn(("%s formatoption is shared with another plotter."
-                          " Use the unshare method to enable the updating") % (
-                              fmto.key),
-                         logger=self.logger)
+                    warn(
+                        (
+                            "%s formatoption is shared with another plotter."
+                            " Use the unshare method to enable the updating"
+                        )
+                        % (fmto.key),
+                        logger=self.logger,
+                    )
                 changed = False
             else:
                 try:
                     changed = fmto.check_and_set(
-                        value, todefault=self._todefault,
-                        validate=not self.no_validation)
+                        value,
+                        todefault=self._todefault,
+                        validate=not self.no_validation,
+                    )
                 except Exception as e:
                     self._registered_updates.pop(key, None)
-                    self.logger.debug('Failed to set %s', key)
+                    self.logger.debug("Failed to set %s", key)
                     raise e
             changed = changed or key in self._force
             if changed:
                 fmtos.append(fmto)
         fmtos = self._insert_additionals(fmtos, seen)
         for fmto in fmtos:
             fmto.lock.acquire()
@@ -1742,39 +1860,52 @@
             The initial `fmtos` plus further formatoptions
 
         Notes
         -----
         `fmtos` and `seen` are modified in place (except that any formatoption
         in the initial `fmtos` has :attr:`~Formatoption.requires_clearing`
         attribute set to True)"""
+
         def get_dependencies(fmto):
             if fmto is None:
                 return []
-            return fmto.dependencies + list(chain(*map(
-                lambda key: get_dependencies(getattr(self, key, None)),
-                fmto.dependencies)))
+            return fmto.dependencies + list(
+                chain(
+                    *map(
+                        lambda key: get_dependencies(getattr(self, key, None)),
+                        fmto.dependencies,
+                    )
+                )
+            )
+
         seen = seen or {fmto.key for fmto in fmtos}
         keys = {fmto.key for fmto in fmtos}
         self.replot = self.replot or any(
-            fmto.requires_replot for fmto in fmtos)
+            fmto.requires_replot for fmto in fmtos
+        )
         if self.replot or any(fmto.priority >= START for fmto in fmtos):
             self.replot = True
             self.plot_data = self.data
-            new_fmtos = dict((f.key, f) for f in self._fmtos
-                             if ((f not in fmtos and is_data_dependent(
-                                 f, self.data))))
+            new_fmtos = dict(
+                (f.key, f)
+                for f in self._fmtos
+                if ((f not in fmtos and is_data_dependent(f, self.data)))
+            )
             seen.update(new_fmtos)
             keys.update(new_fmtos)
             fmtos += list(new_fmtos.values())
 
         # insert the formatoptions that have to be updated if the plot is
         # changed
         if any(fmto.priority >= BEFOREPLOTTING for fmto in fmtos):
-            new_fmtos = dict((f.key, f) for f in self._fmtos
-                             if ((f not in fmtos and f.update_after_plot)))
+            new_fmtos = dict(
+                (f.key, f)
+                for f in self._fmtos
+                if ((f not in fmtos and f.update_after_plot))
+            )
             fmtos += list(new_fmtos.values())
         for fmto in set(self._fmtos).difference(fmtos):
             all_dependencies = get_dependencies(fmto)
             if keys.intersection(all_dependencies):
                 fmtos.append(fmto)
         if any(fmto.requires_clearing for fmto in fmtos):
             self.cleared = True
@@ -1795,31 +1926,35 @@
         ------
         Formatoption
             The next formatoption as it comes by the sorting
 
         Warnings
         --------
         The list `fmtos` is cleared by this method!"""
+
         def pop_fmto(key):
             idx = fmtos_keys.index(key)
             del fmtos_keys[idx]
             return fmtos.pop(idx)
 
         def get_children(fmto, parents_keys):
             all_fmtos = fmtos_keys + parents_keys
             for key in fmto.children + fmto.dependencies:
                 if key not in fmtos_keys:
                     continue
                 child_fmto = pop_fmto(key)
                 for childs_child in get_children(
-                        child_fmto, parents_keys + [child_fmto.key]):
+                    child_fmto, parents_keys + [child_fmto.key]
+                ):
                     yield childs_child
                 # filter out if parent is in update list
-                if (any(key in all_fmtos for key in child_fmto.parents) or
-                        fmto.key in child_fmto.parents):
+                if (
+                    any(key in all_fmtos for key in child_fmto.parents)
+                    or fmto.key in child_fmto.parents
+                ):
                     continue
                 yield child_fmto
 
         fmtos.sort(key=lambda fmto: fmto.priority, reverse=True)
         fmtos_keys = [fmto.key for fmto in fmtos]
         self._last_update = changed or fmtos_keys[:]
         self.logger.debug("Update the formatoptions %s", fmtos_keys)
@@ -1852,32 +1987,39 @@
             >>> list(plotter)
 
         to get the formatoptions.
 
         See Also
         --------
         _format_keys"""
+
         def base_fmtos(base):
             return filter(
                 lambda key: isinstance(getattr(cls, key), Formatoption),
-                getattr(base, '_get_formatoptions', empty)(False))
+                getattr(base, "_get_formatoptions", empty)(False),
+            )
 
         def empty(*args, **kwargs):
             return list()
-        fmtos = (attr for attr, obj in six.iteritems(cls.__dict__)
-                 if isinstance(obj, Formatoption))
+
+        fmtos = (
+            attr
+            for attr, obj in six.iteritems(cls.__dict__)
+            if isinstance(obj, Formatoption)
+        )
         if not include_bases:
             return fmtos
         return unique_everseen(chain(fmtos, *map(base_fmtos, cls.__mro__)))
 
-    docstrings.keep_types('check_key.parameters', 'kwargs',
-                          r'``\*args,\*\*kwargs``')
+    docstrings.keep_types(
+        "check_key.parameters", "kwargs", r"``\*args,\*\*kwargs``"
+    )
 
     @classmethod
-    @docstrings.get_sections(base='Plotter._enhance_keys')
+    @docstrings.get_sections(base="Plotter._enhance_keys")
     @docstrings.dedent
     def _enhance_keys(cls, keys=None, *args, **kwargs):
         """
         Enhance the given keys by groups
 
         Parameters
         ----------
@@ -1900,39 +2042,52 @@
         else:
             keys = list(keys or sorted(all_keys))
         fmto_groups = defaultdict(list)
         for key in all_keys:
             fmto_groups[getattr(cls, key).group].append(key)
         new_i = 0
         for i, key in enumerate(keys[:]):
-
             if key in fmto_groups:
                 del keys[new_i]
                 for key2 in fmto_groups[key]:
                     if key2 not in keys:
                         keys.insert(new_i, key2)
                         new_i += 1
             else:
                 valid, similar, message = check_key(
-                    key, all_keys, False, 'formatoption keyword', *args,
-                    **kwargs)
+                    key,
+                    all_keys,
+                    False,
+                    "formatoption keyword",
+                    *args,
+                    **kwargs,
+                )
                 if not valid:
                     keys.remove(key)
                     new_i -= 1
                     warn(message)
             new_i += 1
         return keys
 
     @classmethod
-    @docstrings.get_sections(base=
-        'Plotter.show_keys', sections=['Parameters', 'Returns',
-                                       'Other Parameters'])
+    @docstrings.get_sections(
+        base="Plotter.show_keys",
+        sections=["Parameters", "Returns", "Other Parameters"],
+    )
     @docstrings.dedent
-    def show_keys(cls, keys=None, indent=0, grouped=False, func=None,
-                  include_links=False, *args, **kwargs):
+    def show_keys(
+        cls,
+        keys=None,
+        indent=0,
+        grouped=False,
+        func=None,
+        include_links=False,
+        *args,
+        **kwargs,
+    ):
         """
         Classmethod to return a nice looking table with the given formatoptions
 
         Parameters
         ----------
         %(Plotter._enhance_keys.parameters)s
         indent: int
@@ -1957,65 +2112,94 @@
         -------
         results of `func`
             None if `func` is the print function, otherwise anything else
 
         See Also
         --------
         show_summaries, show_docs"""
+
         def titled_group(groupname):
-            bars = str_indent + '*' * len(groupname) + '\n'
-            return bars + str_indent + groupname + '\n' + bars
+            bars = str_indent + "*" * len(groupname) + "\n"
+            return bars + str_indent + groupname + "\n" + bars
 
         keys = cls._enhance_keys(keys, *args, **kwargs)
         str_indent = " " * indent
         func = func or default_print_func
         # call this function recursively when grouped is True
         if grouped:
-            grouped_keys = DefaultOrderedDict(list)
+            grouped_keys = Defaultdict(list)
             for fmto in map(lambda key: getattr(cls, key), keys):
                 grouped_keys[fmto.groupname].append(fmto.key)
             text = ""
             for group, keys in six.iteritems(grouped_keys):
-                text += titled_group(group) + cls.show_keys(
-                    keys, indent=indent, grouped=False, func=six.text_type,
-                    include_links=include_links) + '\n\n'
+                text += (
+                    titled_group(group)
+                    + cls.show_keys(
+                        keys,
+                        indent=indent,
+                        grouped=False,
+                        func=six.text_type,
+                        include_links=include_links,
+                    )
+                    + "\n\n"
+                )
             return func(text.rstrip())
 
         if not keys:
             return
         n = len(keys)
         ncols = min([4, n])  # number of columns
         # The number of cells in the table is one of the following cases:
         #     1. The number of columns and equal to the number of keys
         #     2. The number of keys
         #     3. The number of keys plus the empty cells in the last column
         ncells = n + ((ncols - (n % ncols)) if n != ncols else 0)
         if include_links or (include_links is None and cls.include_links):
-            long_keys = list(map(lambda key: ':attr:`~%s.%s.%s`' % (
-                cls.__module__, cls.__name__, key), keys))
+            long_keys = list(
+                map(
+                    lambda key: ":attr:`~%s.%s.%s`"
+                    % (cls.__module__, cls.__name__, key),
+                    keys,
+                )
+            )
         else:
             long_keys = keys
         maxn = max(map(len, long_keys))  # maximal lenght of the keys
         # extend with empty cells
-        long_keys.extend([' ' * maxn] * (ncells - n))
-        bars = (str_indent + '+-' + ("-"*(maxn) + "-+-")*ncols)[:-1]
-        lines = ('| %s |\n%s' % (' | '.join(
-            key.ljust(maxn) for key in long_keys[i:i+ncols]), bars)
-            for i in range(0, n, ncols))
-        text = bars + "\n" + str_indent + ("\n" + str_indent).join(
-            lines)
+        long_keys.extend([" " * maxn] * (ncells - n))
+        bars = (str_indent + "+-" + ("-" * (maxn) + "-+-") * ncols)[:-1]
+        lines = (
+            "| %s |\n%s"
+            % (
+                " | ".join(
+                    key.ljust(maxn) for key in long_keys[i : i + ncols]
+                ),
+                bars,
+            )
+            for i in range(0, n, ncols)
+        )
+        text = bars + "\n" + str_indent + ("\n" + str_indent).join(lines)
         if six.PY2:
-            text = text.encode('utf-8')
+            text = text.encode("utf-8")
 
         return func(text)
 
     @classmethod
     @docstrings.dedent
-    def _show_doc(cls, fmt_func, keys=None, indent=0, grouped=False,
-                  func=None, include_links=False, *args, **kwargs):
+    def _show_doc(
+        cls,
+        fmt_func,
+        keys=None,
+        indent=0,
+        grouped=False,
+        func=None,
+        include_links=False,
+        *args,
+        **kwargs,
+    ):
         """
         Classmethod to print the formatoptions and their documentation
 
         This function is the basis for the :meth:`show_summaries` and
         :meth:`show_docs` methods
 
         Parameters
@@ -2033,42 +2217,59 @@
         Returns
         -------
         %(Plotter.show_keys.returns)s
 
         See Also
         --------
         show_summaries, show_docs"""
+
         def titled_group(groupname):
-            bars = str_indent + '*' * len(groupname) + '\n'
-            return bars + str_indent + groupname + '\n' + bars
+            bars = str_indent + "*" * len(groupname) + "\n"
+            return bars + str_indent + groupname + "\n" + bars
 
         func = func or default_print_func
 
         keys = cls._enhance_keys(keys, *args, **kwargs)
         str_indent = " " * indent
         if grouped:
-            grouped_keys = DefaultOrderedDict(list)
+            grouped_keys = Defaultdict(list)
             for fmto in map(lambda key: getattr(cls, key), keys):
                 grouped_keys[fmto.groupname].append(fmto.key)
             text = "\n\n".join(
-                titled_group(group) + cls._show_doc(
-                    fmt_func, keys, indent=indent, grouped=False,
-                    func=str, include_links=include_links)
-                for group, keys in six.iteritems(grouped_keys))
+                titled_group(group)
+                + cls._show_doc(
+                    fmt_func,
+                    keys,
+                    indent=indent,
+                    grouped=False,
+                    func=str,
+                    include_links=include_links,
+                )
+                for group, keys in six.iteritems(grouped_keys)
+            )
             return func(text.rstrip())
 
         if include_links or (include_links is None and cls.include_links):
-            long_keys = list(map(lambda key: ':attr:`~%s.%s.%s`' % (
-                cls.__module__, cls.__name__, key), keys))
+            long_keys = list(
+                map(
+                    lambda key: ":attr:`~%s.%s.%s`"
+                    % (cls.__module__, cls.__name__, key),
+                    keys,
+                )
+            )
         else:
             long_keys = keys
 
-        text = '\n'.join(str_indent + long_key + '\n' + fmt_func(
-            key, long_key, getattr(cls, key).__doc__) for long_key, key in zip(
-                long_keys, keys))
+        text = "\n".join(
+            str_indent
+            + long_key
+            + "\n"
+            + fmt_func(key, long_key, getattr(cls, key).__doc__)
+            for long_key, key in zip(long_keys, keys)
+        )
         return func(text)
 
     @classmethod
     @docstrings.dedent
     def show_summaries(cls, keys=None, indent=0, *args, **kwargs):
         """
         Classmethod to print the summaries of the formatoptions
@@ -2084,21 +2285,27 @@
         Returns
         -------
         %(Plotter.show_keys.returns)s
 
         See Also
         --------
         show_keys, show_docs"""
+
         def find_summary(key, key_txt, doc):
-            return '\n'.join(wrapper.wrap(doc[:doc.find('\n\n')]))
+            return "\n".join(wrapper.wrap(doc[: doc.find("\n\n")]))
+
         str_indent = " " * indent
-        wrapper = TextWrapper(width=80, initial_indent=str_indent + ' ' * 4,
-                              subsequent_indent=str_indent + ' ' * 4)
-        return cls._show_doc(find_summary, keys=keys, indent=indent,
-                             *args, **kwargs)
+        wrapper = TextWrapper(
+            width=80,
+            initial_indent=str_indent + " " * 4,
+            subsequent_indent=str_indent + " " * 4,
+        )
+        return cls._show_doc(
+            find_summary, keys=keys, indent=indent, *args, **kwargs
+        )
 
     @classmethod
     @docstrings.dedent
     def show_docs(cls, keys=None, indent=0, *args, **kwargs):
         """
         Classmethod to print the full documentations of the formatoptions
 
@@ -2113,18 +2320,21 @@
         Returns
         -------
         %(Plotter.show_keys.returns)s
 
         See Also
         --------
         show_keys, show_docs"""
+
         def full_doc(key, key_txt, doc):
-            return ('=' * len(key_txt)) + '\n' + doc + '\n'
-        return cls._show_doc(full_doc, keys=keys, indent=indent,
-                             *args, **kwargs)
+            return ("=" * len(key_txt)) + "\n" + doc + "\n"
+
+        return cls._show_doc(
+            full_doc, keys=keys, indent=indent, *args, **kwargs
+        )
 
     @classmethod
     def _get_rc_strings(cls):
         """
         Recursive method to get the base strings in the rcParams dictionary.
 
         This method takes the :attr:`_rcparams_string` attribute from the given
@@ -2136,41 +2346,65 @@
         Returns
         -------
         list
             The first entry is the :attr:`_rcparams_string` of this class,
             the following the :attr:`_rcparams_string` attributes of the
             base classes according to the method resolution order of this
             class"""
-        return list(unique_everseen(chain(
-            *map(lambda base: getattr(base, '_rcparams_string', []),
-                 cls.__mro__))))
+        return list(
+            unique_everseen(
+                chain(
+                    *map(
+                        lambda base: getattr(base, "_rcparams_string", []),
+                        cls.__mro__,
+                    )
+                )
+            )
+        )
 
     def _set_rc(self):
         """Method to set the rcparams and defaultParams for this plotter"""
         base_str = self._get_rc_strings()
         # to make sure that the '.' is not interpreted as a regex pattern,
         # we specify the pattern_base by ourselves
-        pattern_base = map(lambda s: s.replace('.', r'\.'), base_str)
+        pattern_base = map(lambda s: s.replace(".", r"\."), base_str)
         # pattern for valid keys being all formatoptions in this plotter
-        pattern = '(%s)(?=$)' % '|'.join(self._get_formatoptions())
-        self._rc = rcParams.find_and_replace(base_str, pattern=pattern,
-                                             pattern_base=pattern_base)
-        user_rc = SubDict(rcParams['plotter.user'], base_str, pattern=pattern,
-                          pattern_base=pattern_base)
+        pattern = "(%s)(?=$)" % "|".join(self._get_formatoptions())
+        self._rc = rcParams.find_and_replace(
+            base_str, pattern=pattern, pattern_base=pattern_base
+        )
+        user_rc = SubDict(
+            rcParams["plotter.user"],
+            base_str,
+            pattern=pattern,
+            pattern_base=pattern_base,
+        )
         self._rc.update(user_rc.data)
 
-        self._defaultParams = SubDict(rcParams.defaultParams, base_str,
-                                      pattern=pattern,
-                                      pattern_base=pattern_base)
+        self._defaultParams = SubDict(
+            rcParams.defaultParams,
+            base_str,
+            pattern=pattern,
+            pattern_base=pattern_base,
+        )
 
-    docstrings.keep_params('InteractiveBase.update.parameters', 'auto_update')
+    docstrings.keep_params("InteractiveBase.update.parameters", "auto_update")
 
+    @docstrings.get_sections(base="Plotter.update")
     @docstrings.dedent
-    def update(self, fmt={}, replot=False, auto_update=False, draw=None,
-               force=False, todefault=False, **kwargs):
+    def update(
+        self,
+        fmt={},
+        replot=False,
+        auto_update=False,
+        draw=None,
+        force=False,
+        todefault=False,
+        **kwargs,
+    ):
         """
         Update the formatoptions and the plot
 
         If the :attr:`data` attribute of this plotter is None, the plotter is
         updated like a usual dictionary (see :meth:`dict.update`). Otherwise
         the update is registered and the plot is updated if `auto_update` is
         True or if the :meth:`start_update` method is called (see below).
@@ -2195,16 +2429,17 @@
         # if the data is None, update like a usual dictionary (but with
         # validation)
         if not self._initialized:
             for key, val in six.iteritems(fmt):
                 self[key] = val
             return
 
-        self._register_update(fmt=fmt, replot=replot, force=force,
-                              todefault=todefault)
+        self._register_update(
+            fmt=fmt, replot=replot, force=force, todefault=todefault
+        )
         if not self.no_auto_update or auto_update:
             self.start_update(draw=draw)
 
     def _set_sharing_keys(self, keys):
         """
         Set the keys to share or unshare
 
@@ -2220,20 +2455,26 @@
         -------
         set
             The set of formatoptions to share (or unshare)"""
         if isinstance(keys, str):
             keys = {keys}
         keys = set(self) if keys is None else set(keys)
         fmto_groups = self._fmto_groups
-        keys.update(chain(*(map(lambda fmto: fmto.key, fmto_groups[key])
-                            for key in keys.intersection(fmto_groups))))
+        keys.update(
+            chain(
+                *(
+                    map(lambda fmto: fmto.key, fmto_groups[key])
+                    for key in keys.intersection(fmto_groups)
+                )
+            )
+        )
         keys.difference_update(fmto_groups)
         return keys
 
-    @docstrings.get_sections(base='Plotter.share')
+    @docstrings.get_sections(base="Plotter.share")
     @docstrings.dedent
     def share(self, plotters, keys=None, draw=None, auto_update=False):
         """
         Share the formatoptions of this plotter with others
 
         This method shares the formatoptions of this :class:`Plotter` instance
         with others to make sure that, if the formatoption of this changes,
@@ -2270,24 +2511,24 @@
         for plotter in plotters:
             if not plotter._initialized:
                 continue
             old_registered = plotter._registered_updates.copy()
             plotter._registered_updates.clear()
             try:
                 plotter.update(force=keys, auto_update=auto_update, draw=draw)
-            except:
+            except Exception:
                 raise
             finally:
                 plotter._registered_updates.clear()
                 plotter._registered_updates.update(old_registered)
         if draw is None:
-            draw = rcParams['auto_draw']
+            draw = rcParams["auto_draw"]
         if draw:
             self.draw()
-            if rcParams['auto_show']:
+            if rcParams["auto_show"]:
                 self.show()
 
     @docstrings.dedent
     def unshare(self, plotters, keys=None, auto_update=False, draw=None):
         """
         Close the sharing connection of this plotter with others
 
@@ -2312,22 +2553,24 @@
         --------
         share, unshare_me"""
         auto_update = auto_update or not self.no_auto_update
         if isinstance(plotters, Plotter):
             plotters = [plotters]
         keys = self._set_sharing_keys(keys)
         for plotter in plotters:
-            plotter.unshare_me(keys, auto_update=auto_update, draw=draw,
-                               update_other=False)
+            plotter.unshare_me(
+                keys, auto_update=auto_update, draw=draw, update_other=False
+            )
         self.update(force=keys, auto_update=auto_update, draw=draw)
 
-    @docstrings.get_sections(base='Plotter.unshare_me')
+    @docstrings.get_sections(base="Plotter.unshare_me")
     @docstrings.dedent
-    def unshare_me(self, keys=None, auto_update=False, draw=None,
-                   update_other=True):
+    def unshare_me(
+        self, keys=None, auto_update=False, draw=None, update_other=True
+    ):
         """
         Close the sharing connection of this plotter with others
 
         This method undoes the sharing connections made by the :meth:`share`
         method and release this plotter again.
 
         Parameters
@@ -2351,16 +2594,15 @@
             try:
                 other_fmto = self._shared.pop(key)
             except KeyError:
                 pass
             else:
                 other_fmto.shared.remove(fmto)
                 if update_other:
-                    other_fmto.plotter._register_update(
-                        force=[other_fmto.key])
+                    other_fmto.plotter._register_update(force=[other_fmto.key])
                     to_update.append(other_fmto.plotter)
         self.update(force=keys, draw=draw, auto_update=auto_update)
         if update_other and auto_update:
             for plotter in to_update:
                 plotter.start_update(draw=draw)
 
     def get_vfunc(self, key):
@@ -2380,14 +2622,15 @@
     def _save_state(self):
         """Saves the current formatoptions"""
         self._old_fmt.append(self.changed)
 
     def show(self):
         """Shows all open figures"""
         import matplotlib.pyplot as plt
+
         plt.show(block=False)
 
     @dedent
     def has_changed(self, key, include_last=True):
         """
         Determine whether a formatoption changed in the last update
 
@@ -2410,53 +2653,65 @@
         if self._initializing or key not in self:
             return
         fmto = getattr(self, key)
         if self._old_fmt and key in self._old_fmt[-1]:
             old_val = self._old_fmt[-1][key]
         else:
             old_val = fmto.default
-        if (fmto.diff(old_val) or (include_last and
-                                   fmto.key in self._last_update)):
+        if fmto.diff(old_val) or (
+            include_last and fmto.key in self._last_update
+        ):
             return [old_val, fmto.value]
 
-    def get_enhanced_attrs(self, arr, axes=['x', 'y', 't', 'z']):
+    def get_enhanced_attrs(self, arr, axes=["x", "y", "t", "z"]):
         if isinstance(arr, InteractiveList):
-            all_attrs = list(starmap(self.get_enhanced_attrs, zip(
-                arr, repeat(axes))))
-            attrs = {key: val for key, val in six.iteritems(all_attrs[0])
-                     if all(key in attrs and attrs[key] == val
-                            for attrs in all_attrs[1:])}
+            all_attrs = list(
+                starmap(self.get_enhanced_attrs, zip(arr, repeat(axes)))
+            )
+            attrs = {
+                key: val
+                for key, val in six.iteritems(all_attrs[0])
+                if all(
+                    key in attrs and attrs[key] == val
+                    for attrs in all_attrs[1:]
+                )
+            }
             attrs.update(arr.attrs)
         else:
             attrs = arr.attrs.copy()
             base_variables = self.base_variables
             if len(base_variables) > 1:  # multiple variables
                 for name, base_var in six.iteritems(base_variables):
                     attrs.update(
-                        {six.text_type(name)+key: value
-                         for key, value in six.iteritems(base_var.attrs)})
+                        {
+                            six.text_type(name) + key: value
+                            for key, value in six.iteritems(base_var.attrs)
+                        }
+                    )
             else:
                 base_var = next(six.itervalues(base_variables))
-            attrs['name'] = arr.name
-            for dim, coord in six.iteritems(getattr(arr, 'coords', {})):
+            attrs["name"] = arr.name
+            for dim, coord in six.iteritems(getattr(arr, "coords", {})):
                 if coord.size == 1:
                     attrs[dim] = format_time(coord.values)
             if isinstance(self.data, InteractiveList):
-                decoder = self.data[0].psy.decoder
+                base = self.data[0].psy.base
             else:
-                decoder = self.data.psy.decoder
+                base = self.data.psy.base
             for dim in axes:
                 for obj in [base_var, arr]:
-                    coord = getattr(decoder, 'get_' + dim)(
-                        obj, coords=getattr(arr, 'coords', None))
+                    decoder = CFDecoder.get_decoder(base, obj)
+                    coord = getattr(decoder, "get_" + dim)(
+                        obj, coords=getattr(arr, "coords", None)
+                    )
                     if coord is None:
                         continue
                     if coord.size == 1:
                         attrs[dim] = format_time(coord.values)
-                    attrs[dim + 'name'] = coord.name
+                    attrs[dim + "name"] = coord.name
                     for key, val in six.iteritems(coord.attrs):
                         attrs[dim + key] = val
         self._enhanced_attrs = attrs
         return attrs
 
     def _make_plot(self):
         plot_fmtos = [fmto for fmto in self._fmtos if fmto.plot_fmt]
```

### Comparing `psyplot-1.4.3/psyplot/project.py` & `psyplot-1.5.0/psyplot/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,116 +4,120 @@
 part of the psyplot API. One instance of the :class:`Project` class serves as
 coordinator of multiple plots and can be distributed into subprojects that
 keep reference to the main project without holding all array instances
 
 Furthermore this module contains an easy pyplot-like API to the current
 subproject."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
+import logging
 import os
 import os.path as osp
-import yaml
+import pickle
 import sys
-import six
+from collections import defaultdict
 from copy import deepcopy as _deepcopy
-import logging
-import inspect
-import pickle
+from functools import partial, wraps
 from importlib import import_module
-from itertools import chain, repeat, cycle, count, islice
-from collections import defaultdict
-from functools import wraps, partial
-import xarray
-import pandas as pd
+from itertools import chain, count, cycle, islice, repeat
 
 import matplotlib as mpl
 import matplotlib.figure as mfig
 import numpy as np
+import pandas as pd
+import six
+import xarray
+import yaml
+from matplotlib.axes import SubplotBase
+
 import psyplot
-from psyplot import rcParams, get_versions
 import psyplot.utils as utils
+from psyplot import get_versions, rcParams
 from psyplot.config.rcsetup import get_configdir, psyplot_fname
-from psyplot.warning import warn, critical
-from psyplot.docstring import docstrings, dedent, safe_modulo
-import psyplot.data as psyd
 from psyplot.data import (
-    ArrayList, open_dataset, open_mfdataset, _MissingModule,
-    to_netcdf, Signal, CFDecoder, safe_list, InteractiveList)
-from psyplot.plotter import unique_everseen, Plotter
-from psyplot.compat.pycompat import (OrderedDict, range, getcwd,
-                                     get_default_value as _get_default_value)
+    ArrayList,
+    CFDecoder,
+    InteractiveList,
+    Signal,
+    _MissingModule,
+    open_dataset,
+    open_mfdataset,
+    safe_list,
+)
+from psyplot.docstring import dedent, docstrings, safe_modulo
+from psyplot.plotter import Plotter, unique_everseen
+from psyplot.utils import get_default_value as _get_default_value
+from psyplot.warning import critical, warn
+
 try:
-    from cdo import Cdo as _CdoBase, CDO_PY_VERSION as cdo_version
+    from cdo import CDO_PY_VERSION as cdo_version
+    from cdo import Cdo as _CdoBase
+
     with_cdo = True
-    cdo_version = tuple(map(int, cdo_version.split('.')[:2]))
+    cdo_version = tuple(map(int, cdo_version.split(".")[:2]))
 except ImportError as e:
     Cdo = _MissingModule(e)
     with_cdo = False
     cdo_version = None
 
 try:  # try import show_colormaps for convenience
-    from psy_simple.colors import show_colormaps, get_cmap
+    from psy_simple.colors import get_cmap, show_colormaps  # noqa: F401
 except ImportError:
     pass
 
-if rcParams['project.import_seaborn'] is not False:
+if rcParams["project.import_seaborn"] is not False:
     try:
         import seaborn as _sns
     except ImportError as e:
-        if rcParams['project.import_seaborn']:
+        if rcParams["project.import_seaborn"]:
             raise
         _sns = _MissingModule(e)
 
 _open_projects = []  # list of open projects
 _current_project = None  # current main project
 _current_subproject = None  # current subproject
 
 # the informations on the psyplot and plugin versions
 _versions = get_versions(requirements=False)
 
 
-_concat_dim_default = _get_default_value(xarray.open_mfdataset, 'concat_dim')
+_concat_dim_default = _get_default_value(xarray.open_mfdataset, "concat_dim")
 
 
 def _update_versions():
     """Update :attr:`_versions` with the registered plotter methods"""
     for pm_name in plot._plot_methods:
         pm = getattr(plot, pm_name)
         plugin = pm._plugin
-        if (plugin is not None and plugin not in _versions and
-                pm.module in sys.modules):
+        if (
+            plugin is not None
+            and plugin not in _versions
+            and pm.module in sys.modules
+        ):
             _versions.update(get_versions(key=lambda s: s == plugin))
 
 
-@docstrings.get_sections(base='multiple_subplots')
+@docstrings.get_sections(base="multiple_subplots")
 @docstrings.dedent
-def multiple_subplots(rows=1, cols=1, maxplots=None, n=1, delete=True,
-                      for_maps=False, *args, **kwargs):
+def multiple_subplots(
+    rows=1,
+    cols=1,
+    maxplots=None,
+    n=1,
+    delete=True,
+    for_maps=False,
+    *args,
+    **kwargs,
+):
     """
     Function to create subplots.
 
     This function creates so many subplots on so many figures until the
     specified number `n` is reached.
 
     Parameters
@@ -139,22 +143,23 @@
         function
 
     Returns
     -------
     list
         list of maplotlib.axes.SubplotBase instances"""
     import matplotlib.pyplot as plt
+
     axes = np.array([])
     maxplots = maxplots or rows * cols
-    kwargs.setdefault('figsize', [
-        min(8.*cols, 16), min(6.5*rows, 12)])
+    kwargs.setdefault("figsize", [min(8.0 * cols, 16), min(6.5 * rows, 12)])
     if for_maps:
         import cartopy.crs as ccrs
-        subplot_kw = kwargs.setdefault('subplot_kw', {})
-        subplot_kw['projection'] = ccrs.PlateCarree()
+
+        subplot_kw = kwargs.setdefault("subplot_kw", {})
+        subplot_kw["projection"] = ccrs.PlateCarree()
     for i in range(0, n, maxplots):
         fig, ax = plt.subplots(rows, cols, *args, **kwargs)
         try:
             axes = np.append(axes, ax.ravel()[:maxplots])
             if delete:
                 for iax in range(maxplots, rows * cols):
                     fig.delaxes(ax.ravel()[iax])
@@ -169,42 +174,46 @@
 
 def _is_slice(val):
     return isinstance(val, slice)
 
 
 def _only_main(func):
     """Call the given `func` only from the main project"""
+
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         if not self.is_main:
             return getattr(self.main, func.__name__)(*args, **kwargs)
         return func(self, *args, **kwargs)
+
     return wrapper
 
 
 def _first_main(func):
     """Call the given `func` with the same arguments but after the function
     of the main project"""
+
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         if not self.is_main:
             getattr(self.main, func.__name__)(*args, **kwargs)
         return func(self, *args, **kwargs)
+
     return wrapper
 
 
 class Project(ArrayList):
     """A manager of multiple interactive data projects"""
 
     _main = None
 
     _registered_plotters = {}  #: registered plotter identifiers
 
     #: signal to be emiitted when the current main and/or subproject changes
-    oncpchange = Signal(name='oncpchange', cls_signal=True)
+    oncpchange = Signal(name="oncpchange", cls_signal=True)
 
     # block the signals of this class
     block_signals = utils._TempBool()
 
     @property
     def main(self):
         """:class:`Project`. The main project of this subproject"""
@@ -230,16 +239,18 @@
         list"""
         plotters = self.plotters
         if len(plotters) == 0:
             return {}
         p0 = plotters[0]
         if len(plotters) == 1:
             return p0._fmtos
-        return (getattr(p0, key) for key in set(p0).intersection(
-            *map(set, plotters[1:])))
+        return (
+            getattr(p0, key)
+            for key in set(p0).intersection(*map(set, plotters[1:]))
+        )
 
     @property
     def is_csp(self):
         """Boolean that is True if the project is the current subproject"""
         return self is _current_subproject
 
     @property
@@ -247,47 +258,49 @@
         """Boolean that is True if the project is the current main project"""
         return self is _current_project
 
     @property
     def figs(self):
         """A mapping from figures to data objects with the plotter in this
         figure"""
-        ret = utils.DefaultOrderedDict(lambda: self[1:0])
+        ret = utils.Defaultdict(lambda: self[1:0])
         for arr in self:
             if arr.psy.plotter is not None:
                 ret[arr.psy.plotter.ax.get_figure()].append(arr)
-        return OrderedDict(ret)
+        return dict(ret)
 
     @property
     def axes(self):
-        """A mapping from axes to data objects with the plotter in this axes
-        """
-        ret = utils.DefaultOrderedDict(lambda: self[1:0])
+        """A mapping from axes to data objects with the plotter in this axes"""
+        ret = utils.Defaultdict(lambda: self[1:0])
         for arr in self:
             if arr.psy.plotter is not None:
                 ret[arr.psy.plotter.ax].append(arr)
-        return OrderedDict(ret)
+        return dict(ret)
 
     @property
     def is_main(self):
         """:class:`bool`. True if this :class:`Project` is a main project"""
         return self._main is None
 
     @property
     def logger(self):
         """:class:`logging.Logger` of this instance"""
         if not self.is_main:
             return self.main.logger
         try:
             return self._logger
         except AttributeError:
-            name = '%s.%s.%s' % (self.__module__, self.__class__.__name__,
-                                 self.num)
+            name = "%s.%s.%s" % (
+                self.__module__,
+                self.__class__.__name__,
+                self.num,
+            )
             self._logger = logging.getLogger(name)
-            self.logger.debug('Initializing...')
+            self.logger.debug("Initializing...")
             return self._logger
 
     @logger.setter
     def logger(self, value):
         self._logger = value
 
     def with_plotter(self):
@@ -306,78 +319,96 @@
         return list(arr.psy.arr_name for arr in self)
 
     @arr_names.setter
     def arr_names(self, value):
         value = list(islice(value, len(self)))
         if not len(set(value)) == len(self):
             raise ValueError(
-                "Got %i unique array names for %i data objects!" % (
-                    len(set(value)), len(self)))
+                "Got %i unique array names for %i data objects!"
+                % (len(set(value)), len(self))
+            )
         elif not self.is_main and set(value) & (
-                set(self.main.arr_names) - set(self.arr_names)):
+            set(self.main.arr_names) - set(self.arr_names)
+        ):
             raise ValueError(
                 "Cannot rename arrays because there are duplicates with the "
-                "main project: %s" % (
-                    set(value) & (
-                        set(self.main.arr_names) - set(self.arr_names)), ))
+                "main project: %s"
+                % (
+                    set(value)
+                    & (set(self.main.arr_names) - set(self.arr_names)),
+                )
+            )
         for arr, n in zip(self, value):
             arr.psy.arr_name = n
         if self.main is gcp(True):
             for arr in self:
                 arr.psy.onupdate.emit()
 
     @property
     def plotters(self):
         """A list of all the plotters in this instance"""
         return [arr.psy.plotter for arr in self.with_plotter]
 
     @property
     def datasets(self):
         """A mapping from dataset numbers to datasets in this list"""
-        return {key: val['ds'] for key, val in six.iteritems(
-            self._get_ds_descriptions(self.array_info(ds_description=['ds'])))}
+        return {
+            key: val["ds"]
+            for key, val in six.iteritems(
+                self._get_ds_descriptions(
+                    self.array_info(ds_description=["ds"])
+                )
+            )
+        }
 
     @property
     def dsnames_map(self):
         """A dictionary from the dataset numbers in this list to their
         filenames"""
-        return {key: val['fname'] for key, val in six.iteritems(
-            self._get_ds_descriptions(self.array_info(
-                ds_description=['num', 'fname']), ds_description={'fname'}))}
+        return {
+            key: val["fname"]
+            for key, val in six.iteritems(
+                self._get_ds_descriptions(
+                    self.array_info(ds_description=["num", "fname"]),
+                    ds_description={"fname"},
+                )
+            )
+        }
 
     @property
     def dsnames(self):
         """The set of dataset names in this instance"""
         return {t[0] for t in self._get_dsnames(self.array_info()) if t[0]}
 
-    @docstrings.get_sections(base='Project')
+    @docstrings.get_sections(base="Project")
     @docstrings.dedent
     def __init__(self, *args, **kwargs):
         """
         Parameters
         ----------
         %(ArrayList.parameters)s
         main: Project
             The main project this subproject belongs to (or None if this
             project is the main project)
         num: int
             The number of the project
         """
-        self.main = kwargs.pop('main', None)
+        self.main = kwargs.pop("main", None)
         self._plot = ProjectPlotter(self)
-        self.num = kwargs.pop('num', 1)
+        self.num = kwargs.pop("num", 1)
         self._ds_counter = count()
         with self.block_signals:
             super(Project, self).__init__(*args, **kwargs)
 
     @classmethod
-    @docstrings.get_sections(base='Project._register_plotter')
+    @docstrings.get_sections(base="Project._register_plotter")
     @dedent
-    def _register_plotter(cls, identifier, module, plotter_name,
-                          plotter_cls=None):
+    def _register_plotter(
+        cls, identifier, module, plotter_name, plotter_cls=None
+    ):
         """
         Register a plotter in the :class:`Project` class to easy access it
 
         Parameters
         ----------
         identifier: str
             Name of the attribute that is used to filter for the instances
@@ -387,22 +418,35 @@
         plotter_name: str
             The name of the plotter class in `module`
         plotter_cls: type
             The imported class of `plotter_name`. If None, it will be imported
             when it is needed
         """
         if plotter_cls is not None:  # plotter has already been imported
+
             def get_x(self):
                 return self(plotter_cls)
+
         else:
+
             def get_x(self):
                 return self(getattr(import_module(module), plotter_name))
-        setattr(cls, identifier, property(get_x, doc=(
-            "List of data arrays that are plotted by :class:`%s.%s`"
-            " plotters") % (module, plotter_name)))
+
+        setattr(
+            cls,
+            identifier,
+            property(
+                get_x,
+                doc=(
+                    "List of data arrays that are plotted by :class:`%s.%s`"
+                    " plotters"
+                )
+                % (module, plotter_name),
+            ),
+        )
         cls._registered_plotters[identifier] = (module, plotter_name)
 
     def disable(self):
         """Disables the plotters in this list"""
         for arr in self:
             if arr.psy.plotter:
                 arr.psy.plotter.disabled = True
@@ -420,16 +464,17 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close(True, True, True)
 
     @staticmethod
-    @docstrings.get_sections(base='Project._load_preset',
-                              sections=["Parameters", "Notes"])
+    @docstrings.get_sections(
+        base="Project._load_preset", sections=["Parameters", "Notes"]
+    )
     def _load_preset(preset: str):
         """Load a preset from disk
 
         Parameters
         ----------
         preset: str or dict
             The filename or identifier of a preset. If the given `preset` is
@@ -447,50 +492,51 @@
         -----
         An identifier is the filename without extension. If you want to list
         the available presets, run ``psyplot -lp`` from the command-line"""
         if isinstance(preset, dict):
             config = preset
         else:
             path = Project._resolve_preset_path(preset)
-            if path in rcParams['presets.trusted']:
+            if path in rcParams["presets.trusted"]:
                 loader = yaml.Loader
             else:
                 loader = yaml.SafeLoader
             with open(path) as f:
                 try:
                     config = yaml.load(f, loader)
                 except yaml.constructor.ConstructorError as e:
-                    e.note = (e.note or '') + (
-                        ' You might want to add it to the trusted presets '
+                    e.note = (e.note or "") + (
+                        " You might want to add it to the trusted presets "
                         'via\n\npsy.rcParams["presets.trusted"].append("{}")\n\n'
-                        'and run this method again. To permanently store '
-                        'this preset, edit the file at\n\n{} ').format(
-                            path, psyplot_fname())
+                        "and run this method again. To permanently store "
+                        "this preset, edit the file at\n\n{} "
+                    ).format(path, psyplot_fname())
                     raise
 
         return config
 
     @staticmethod
     def _resolve_preset_path(preset, if_exists=True):
         if osp.exists(preset):
             return preset
         else:
             confdir = get_configdir()
-            presets_dir = osp.join(confdir, 'presets')
+            presets_dir = osp.join(confdir, "presets")
             if osp.exists(osp.join(presets_dir, preset)):
                 return osp.join(presets_dir, preset)
-            elif osp.exists(osp.join(presets_dir, preset + '.yml')):
-                return osp.join(presets_dir, preset + '.yml')
+            elif osp.exists(osp.join(presets_dir, preset + ".yml")):
+                return osp.join(presets_dir, preset + ".yml")
             else:
                 if if_exists:
                     raise ValueError(
-                        f"Could not find a preset with name {preset}")
+                        f"Could not find a preset with name {preset}"
+                    )
                 else:
-                    if not preset.endswith('.yml'):
-                        return osp.join(presets_dir, preset + '.yml')
+                    if not preset.endswith(".yml"):
+                        return osp.join(presets_dir, preset + ".yml")
                     return preset
 
     @docstrings.dedent
     def load_preset(self, preset: str, **kwargs):
         """Load a preset from disk and apply it to the open project.
 
         This method loads a preset and updates the corresponding plots
@@ -512,16 +558,19 @@
         with self.no_auto_update:
             for pm in plotmethods:
                 method = getattr(self.plot, pm)
                 if method.is_imported:
                     sp = getattr(self, pm)
                     if sp:
                         valid = list(method.plotter_cls._get_formatoptions())
-                        fmts = {key: val for key, val in defaults.items()
-                                if key in valid}
+                        fmts = {
+                            key: val
+                            for key, val in defaults.items()
+                            if key in valid
+                        }
                         fmts.update(pm_config.get(pm, {}))
                         sp.update(fmt=fmts, **kwargs)
         self.start_update()
 
     @staticmethod
     def extract_fmts_from_preset(preset: str, plotmethod: str):
         """Extract the formatoptions for a plotmethod from a given preset
@@ -542,35 +591,33 @@
         else:
             method = plotmethod
             plotmethod = method._method
 
         plotmethods = plot._plot_methods
         pm_config, defaults = utils.sort_kwargs(preset, plotmethods)
         valid = list(method.plotter_cls._get_formatoptions())
-        fmts = {key: val for key, val in defaults.items()
-                if key in valid}
+        fmts = {key: val for key, val in defaults.items() if key in valid}
         fmts.update(pm_config.get(plotmethod, {}))
         return fmts
 
-
     def save_preset(self, fname=None, include_defaults=False, update=False):
         """Save the formatoptions of this project as a preset
 
         This method takes the formatoptions in the plotters of this project and
         saves it as a preset file"""
 
         def include(fmto, plotters):
             key = fmto.key
             for plotter in plotters:
                 if fmto.diff(plotter[key]):
                     return False
             return True if include_defaults else fmto.changed
 
         if update:
-            with open(f) as f:
+            with open(fname) as f:
                 preset = yaml.load(f, yaml.Loader)
         else:
             preset = {}
         plotters = self.plotters
 
         for fmto in self._fmtos:
             if include(fmto, plotters):
@@ -584,15 +631,15 @@
                 for fmto in sp._fmtos:
                     if fmto.key not in preset and include(fmto, plotters):
                         preset.setdefault(pm, {})
                         preset[pm][fmto.key] = fmto.value
         if fname is not None:
             fname = self._resolve_preset_path(fname, False)
             os.makedirs(osp.dirname(fname), exist_ok=True)
-            with open(fname, 'w') as f:
+            with open(fname, "w") as f:
                 yaml.dump(preset, f)
         else:
             return preset
 
     @_first_main
     def extend(self, *args, **kwargs):
         len0 = len(self)
@@ -619,15 +666,15 @@
             self.oncpchange.emit(self)
         return ret
 
     append.__doc__ = ArrayList.append.__doc__
 
     __call__.__doc__ = ArrayList.__call__.__doc__
 
-    @docstrings.get_sections(base='Project.close')
+    @docstrings.get_sections(base="Project.close")
     @dedent
     def close(self, figs=True, data=False, ds=False, remove_only=False):
         """
         Close this project instance
 
         Parameters
         ----------
@@ -637,14 +684,15 @@
             delete the arrays from the (main) project
         ds: bool
             If True, close the dataset as well
         remove_only: bool
             If True and `figs` is True, the figures are not closed but the
             plotters are removed"""
         import matplotlib.pyplot as plt
+
         close_ds = ds
         for arr in self[:]:
             if figs and arr.psy.plotter is not None:
                 if remove_only:
                     for fmto in arr.psy.plotter._fmtos:
                         try:
                             fmto.remove()
@@ -658,45 +706,68 @@
                 if not self.is_main:
                     try:
                         self.main.remove(arr)
                     except ValueError:  # arr not in list
                         pass
             if close_ds:
                 if isinstance(arr, InteractiveList):
-                    for ds in [val['ds'] for val in six.itervalues(
-                               arr._get_ds_descriptions(
-                                    arr.array_info(ds_description=['ds'],
-                                                   standardize_dims=False)))]:
+                    for ds in [
+                        val["ds"]
+                        for val in six.itervalues(
+                            arr._get_ds_descriptions(
+                                arr.array_info(
+                                    ds_description=["ds"],
+                                    standardize_dims=False,
+                                )
+                            )
+                        )
+                    ]:
                         ds.close()
                 else:
                     arr.psy.base.close()
         if self.is_main and self is gcp(True) and data:
             scp(None)
         elif self.is_main and self.is_cmp:
             self.oncpchange.emit(self)
         elif self.main.is_cmp:
             self.oncpchange.emit(self.main)
 
-    docstrings.keep_params('multiple_subplots.parameters', 'delete')
-    docstrings.delete_params('ArrayList.from_dataset.parameters', 'base')
-    docstrings.delete_kwargs('ArrayList.from_dataset.other_parameters',
-                             kwargs='kwargs')
-    docstrings.keep_params('xarray.open_mfdataset.parameters', 'concat_dim')
-    docstrings.keep_params('Project._load_preset.parameters', 'preset')
+    docstrings.keep_params("multiple_subplots.parameters", "delete")
+    docstrings.delete_params("ArrayList.from_dataset.parameters", "base")
+    docstrings.delete_kwargs(
+        "ArrayList.from_dataset.other_parameters", kwargs="kwargs"
+    )
+    docstrings.keep_params("xarray.open_mfdataset.parameters", "concat_dim")
+    docstrings.keep_params("Project._load_preset.parameters", "preset")
 
     @_only_main
-    @docstrings.get_sections(base='Project._add_data',
-                              sections=['Parameters', 'Other Parameters',
-                                        'Returns'])
-    @docstrings.dedent
-    def _add_data(self, plotter_cls, filename_or_obj, fmt={}, make_plot=True,
-                  draw=False, mf_mode=False, ax=None, engine=None, delete=True,
-                  share=False, clear=False, enable_post=None,
-                  concat_dim=_concat_dim_default, load=False,
-                  *args, **kwargs):
+    @docstrings.get_sections(
+        base="Project._add_data",
+        sections=["Parameters", "Other Parameters", "Returns"],
+    )
+    @docstrings.dedent
+    def _add_data(
+        self,
+        plotter_cls,
+        filename_or_obj,
+        fmt={},
+        make_plot=True,
+        draw=False,
+        mf_mode=False,
+        ax=None,
+        engine=None,
+        delete=True,
+        share=False,
+        clear=False,
+        enable_post=None,
+        concat_dim=_concat_dim_default,
+        load=False,
+        *args,
+        **kwargs,
+    ):
         """
         Extract data from a dataset and visualize it with the given plotter
 
         Parameters
         ----------
         plotter_cls: type
             The subclass of :class:`psyplot.plotter.Plotter` to use for
@@ -758,111 +829,125 @@
 
         Returns
         -------
         Project
             The subproject that contains the new (visualized) data array"""
         if not isinstance(filename_or_obj, xarray.Dataset):
             if mf_mode:
-                filename_or_obj = open_mfdataset(filename_or_obj,
-                                                 engine=engine,
-                                                 concat_dim=concat_dim)
+                filename_or_obj = open_mfdataset(
+                    filename_or_obj, engine=engine, concat_dim=concat_dim
+                )
             else:
-                filename_or_obj = open_dataset(filename_or_obj,
-                                               engine=engine)
+                filename_or_obj = open_dataset(filename_or_obj, engine=engine)
         if load:
             old = filename_or_obj
             filename_or_obj = filename_or_obj.load()
             old.close()
 
         fmt = dict(fmt)
         possible_fmts = list(plotter_cls._get_formatoptions())
-        additional_fmt, kwargs = utils.sort_kwargs(
-            kwargs, possible_fmts)
+        additional_fmt, kwargs = utils.sort_kwargs(kwargs, possible_fmts)
         fmt.update(additional_fmt)
         if enable_post is None:
-            enable_post = bool(fmt.get('post'))
+            enable_post = bool(fmt.get("post"))
         # create the subproject
         sub_project = self.from_dataset(filename_or_obj, **kwargs)
         sub_project.main = self
         sub_project.no_auto_update = not (
-            not sub_project.no_auto_update or not self.no_auto_update)
+            not sub_project.no_auto_update or not self.no_auto_update
+        )
         # create the subplots
         proj = plotter_cls._get_sample_projection()
         if isinstance(ax, tuple):
-            axes = iter(multiple_subplots(
-                *ax, n=len(sub_project), subplot_kw={'projection': proj}))
-        elif ax is None or isinstance(ax, (mpl.axes.SubplotBase,
-                                           mpl.axes.Axes)):
+            axes = iter(
+                multiple_subplots(
+                    *ax, n=len(sub_project), subplot_kw={"projection": proj}
+                )
+            )
+        elif ax is None or isinstance(
+            ax, (mpl.axes.SubplotBase, mpl.axes.Axes)
+        ):
             axes = repeat(ax)
         else:
             axes = iter(ax)
         clear = clear or (isinstance(ax, tuple) and proj is not None)
 
         for arr in sub_project:
-            plotter_cls(arr, make_plot=(not bool(share) and make_plot),
-                        draw=False, ax=next(axes), clear=clear,
-                        project=self, enable_post=enable_post, **fmt)
+            plotter_cls(
+                arr,
+                make_plot=(not bool(share) and make_plot),
+                draw=False,
+                ax=next(axes),
+                clear=clear,
+                project=self,
+                enable_post=enable_post,
+                **fmt,
+            )
         if share:
             if share is True:
                 share = possible_fmts
             elif isinstance(share, six.string_types):
                 share = [share]
             else:
                 share = list(share)
             sub_project[0].psy.plotter.share(
-                [arr.psy.plotter for arr in sub_project[1:]], keys=share,
-                draw=False)
+                [arr.psy.plotter for arr in sub_project[1:]],
+                keys=share,
+                draw=False,
+            )
             if make_plot:
                 for arr in sub_project:
                     arr.psy.plotter.reinit(draw=False, clear=clear)
         if draw is None:
-            draw = rcParams['auto_draw']
+            draw = rcParams["auto_draw"]
         if draw:
             sub_project.draw()
-            if rcParams['auto_show']:
+            if rcParams["auto_show"]:
                 self.show()
         self.extend(sub_project, new_name=True)
         if self is gcp(True):
             scp(sub_project)
         return sub_project
 
     def __getitem__(self, key):
         """Overwrites lists __getitem__ by returning subproject if `key` is a
         slice"""
         if isinstance(key, slice):  # return a new project
-            ret = self.__class__(
-                super(Project, self).__getitem__(key))
+            ret = self.__class__(super(Project, self).__getitem__(key))
             ret.main = self.main
         else:  # return the item
             ret = super(Project, self).__getitem__(key)
         return ret
 
     if six.PY2:  # for compatibility to python 2.7
+
         def __getslice__(self, *args):
             return self[slice(*args)]
 
     def __add__(self, other):
         # overwritte to return a subproject
         ret = self.__class__(super(Project, self).__add__(other))
         ret.main = self.main
         return ret
 
     @staticmethod
     def show():
         """Shows all open figures"""
         import matplotlib.pyplot as plt
+
         plt.show(block=False)
 
-    docstrings.keep_params('join_dicts.parameters', 'delimiter')
-    docstrings.keep_params('join_dicts.parameters', 'keep_all')
+    docstrings.keep_params("join_dicts.parameters", "delimiter")
+    docstrings.keep_params("join_dicts.parameters", "keep_all")
 
-    @docstrings.get_sections(base='Project.joined_attrs')
+    @docstrings.get_sections(base="Project.joined_attrs")
     @docstrings.with_indent(8)
-    def joined_attrs(self, delimiter=', ', enhanced=True, plot_data=False,
-                     keep_all=True):
+    def joined_attrs(
+        self, delimiter=", ", enhanced=True, plot_data=False, keep_all=True
+    ):
         """Join the attributes of the arrays in this project
 
         Parameters
         ----------
         %(join_dicts.parameters.delimiter)s
         enhanced: bool
             If True, the :meth:`psyplot.plotter.Plotter.get_enhanced_attrs`
@@ -878,29 +963,34 @@
         dict
             A mapping from the attribute to the joined attributes which are
             either strings or (if there is only one attribute value), the
             data type of the corresponding value"""
         if enhanced:
             all_attrs = [
                 plotter.get_enhanced_attrs(
-                    getattr(plotter, 'plot_data' if plot_data else 'data'))
-                for plotter in self.plotters]
+                    getattr(plotter, "plot_data" if plot_data else "data")
+                )
+                for plotter in self.plotters
+            ]
         else:
             if plot_data:
-                all_attrs = [plotter.plot_data.attrs
-                             for plotter in self.plotters]
+                all_attrs = [
+                    plotter.plot_data.attrs for plotter in self.plotters
+                ]
             else:
                 all_attrs = [arr.attrs for arr in self]
-        return utils.join_dicts(all_attrs, delimiter=delimiter,
-                                keep_all=keep_all)
+        return utils.join_dicts(
+            all_attrs, delimiter=delimiter, keep_all=keep_all
+        )
 
-    @docstrings.get_sections(base='Project.format_string')
+    @docstrings.get_sections(base="Project.format_string")
     @docstrings.with_indent(8)
-    def format_string(self, s, use_time=False, format_args=None, *args,
-                      **kwargs):
+    def format_string(
+        self, s, use_time=False, format_args=None, *args, **kwargs
+    ):
         """Format a string with the attributes in this project
 
         Parameters
         ----------
         s: str
             The string that is subject to be formatted
         use_time: bool
@@ -932,19 +1022,26 @@
         if format_args is not None:
             try:
                 s = safe_modulo(s, format_args, print_warning=False)
             except TypeError:
                 pass
         return safe_modulo(s, attrs)
 
-    docstrings.keep_params('Project.format_string.parameters', 'use_time')
+    docstrings.keep_params("Project.format_string.parameters", "use_time")
 
     @docstrings.with_indent(8)
-    def export(self, output, tight=False, concat=True, close_pdf=None,
-               use_time=False, **kwargs):
+    def export(
+        self,
+        output,
+        tight=False,
+        concat=True,
+        close_pdf=None,
+        use_time=False,
+        **kwargs,
+    ):
         """Exports the figures of the project to one or more image files
 
         Parameters
         ----------
         output: str, iterable or matplotlib.backends.backend_pdf.PdfPages
             if string or list of strings, those define the names of the output
             files. Otherwise you may provide an instance of
@@ -1002,60 +1099,64 @@
             >>> p.export('my_plots_%%i_%%(name)s.png')
 
         Specify the names for each figure directly via a list::
 
             >>> p.export(['my_plots1.pdf', 'my_plots2.pdf'])
         """
         from matplotlib.backends.backend_pdf import PdfPages
+
         if tight:
-            kwargs['bbox_inches'] = 'tight'
+            kwargs["bbox_inches"] = "tight"
 
         not_enough_files_warnings = (
             "Not enough output files specified! %i figures are open "
             "but only %i filenames have been given! This will cause "
             "that some figures may be overwritten after being "
             "exported! Use a pdf instead if you want to save all "
             "figures or include a '%%i' string in the filename to "
-            "avoid duplicates.")
+            "avoid duplicates."
+        )
 
         if isinstance(output, six.string_types):  # a single string
-            out_fmt = kwargs.pop('format', os.path.splitext(output))[1][1:]
-            if out_fmt.lower() == 'pdf' and concat:
-                output = self.format_string(output, use_time, delimiter='-')
+            out_fmt = kwargs.pop("format", os.path.splitext(output))[1][1:]
+            if out_fmt.lower() == "pdf" and concat:
+                output = self.format_string(output, use_time, delimiter="-")
                 pdf = PdfPages(output)
 
                 for fig in self.figs:
                     pdf.savefig(fig, **kwargs)
                 if close_pdf is None or close_pdf:
                     pdf.close()
                     return
                 else:
                     return pdf
             else:
                 output = [output] * len(self.figs)
 
         if utils.is_iterable(output):  # a list of strings
-            output = [sp.format_string(out, use_time, i, delimiter='-')
-                      for i, (out, sp) in enumerate(
-                          zip(output, self.figs.values()), 1)]
+            output = [
+                sp.format_string(out, use_time, i, delimiter="-")
+                for i, (out, sp) in enumerate(
+                    zip(output, self.figs.values()), 1
+                )
+            ]
             if len(set(output)) != len(output):
-                warn(not_enough_files_warnings % (
-                    len(output), len(self.figs)))
+                warn(not_enough_files_warnings % (len(output), len(self.figs)))
             output = iter(output)
 
             for fig, out in zip(self.figs, output):
                 fig.savefig(out, **kwargs)
         else:  # an instances of matplotlib.backends.backend_pdf.PdfPages
             for fig in self.figs:
                 output.savefig(fig, **kwargs)
             if close_pdf:
                 output.close()
 
-    docstrings.keep_params('Plotter.share.parameters', 'keys')
-    docstrings.delete_params('Plotter.share.parameters', 'keys', 'plotters')
+    docstrings.keep_params("Plotter.share.parameters", "keys")
+    docstrings.delete_params("Plotter.share.parameters", "keys", "plotters")
 
     @docstrings.dedent
     def share(self, base=None, keys=None, by=None, **kwargs):
         """
         Share the formatoptions of one plotter with all the others
 
         This method shares specified formatoptions from `base` with all the
@@ -1077,42 +1178,46 @@
         %(Plotter.share.parameters.no_keys|plotters)s
 
         See Also
         --------
         psyplot.plotter.share"""
         if by is not None:
             if base is not None:
-                if hasattr(base, 'psy') or isinstance(base, Plotter):
+                if hasattr(base, "psy") or isinstance(base, Plotter):
                     base = [base]
-                if by.lower() in ['ax', 'axes']:
-                    bases = {ax: p[0] for ax, p in six.iteritems(
-                        Project(base).axes)}
-                elif by.lower() in ['fig', 'figure']:
-                    bases = {fig: p[0] for fig, p in six.iteritems(
-                        Project(base).figs)}
+                if by.lower() in ["ax", "axes"]:
+                    bases = {
+                        ax: p[0] for ax, p in six.iteritems(Project(base).axes)
+                    }
+                elif by.lower() in ["fig", "figure"]:
+                    bases = {
+                        fig: p[0]
+                        for fig, p in six.iteritems(Project(base).figs)
+                    }
                 else:
                     raise ValueError(
                         "*by* must be out of {'fig', 'figure', 'ax', 'axes'}. "
-                        "Not %s" % (by, ))
+                        "Not %s" % (by,)
+                    )
             else:
                 bases = {}
-            projects = self.axes if by == 'axes' else self.figs
+            projects = self.axes if by == "axes" else self.figs
             for obj, p in projects.items():
                 p.share(bases.get(obj), keys, **kwargs)
         else:
             plotters = self.plotters
             if not plotters:
                 return
             if base is None:
                 if len(plotters) == 1:
                     return
                 base = plotters[0]
                 plotters = plotters[1:]
             elif not isinstance(base, Plotter):
-                base = getattr(getattr(base, 'psy', base), 'plotter', base)
+                base = getattr(getattr(base, "psy", base), "plotter", base)
             base.share(plotters, keys=keys, **kwargs)
 
     @docstrings.dedent
     def unshare(self, **kwargs):
         """
         Unshare the formatoptions of all the plotters in this instance
 
@@ -1125,17 +1230,17 @@
 
         See Also
         --------
         psyplot.plotter.Plotter.unshare, psyplot.plotter.Plotter.unshare_me"""
         for plotter in self.plotters:
             plotter.unshare_me(**kwargs)
 
-    docstrings.delete_params('ArrayList.array_info.parameters', 'pwd', 'copy')
+    docstrings.delete_params("ArrayList.array_info.parameters", "pwd", "copy")
 
-    @docstrings.get_sections(base='Project.save_project')
+    @docstrings.get_sections(base="Project.save_project")
     @docstrings.dedent
     def save_project(self, fname=None, pwd=None, pack=False, **kwargs):
         """
         Save this project to a file
 
         Parameters
         ----------
@@ -1163,87 +1268,112 @@
         if pack and fname is not None:
             target_dir = os.path.dirname(fname)
             if not os.path.exists(target_dir):
                 os.makedirs(target_dir, exist_ok=True)
 
             def tmp_it():
                 from tempfile import NamedTemporaryFile
+
                 while True:
-                    yield NamedTemporaryFile(
-                        dir=target_dir, suffix='.nc').name
+                    yield NamedTemporaryFile(dir=target_dir, suffix=".nc").name
 
-            kwargs.setdefault('paths', tmp_it())
+            kwargs.setdefault("paths", tmp_it())
         if fname is not None:
-            kwargs['copy'] = True
+            kwargs["copy"] = True
 
         _update_versions()
-        ret = {'figs': dict(map(_ProjectLoader.inspect_figure, self.figs)),
-               'arrays': self.array_info(pwd=pwd, **kwargs),
-               'versions': _deepcopy(_versions)}
+        ret = {
+            "figs": dict(map(_ProjectLoader.inspect_figure, self.figs)),
+            "arrays": self.array_info(pwd=pwd, **kwargs),
+            "versions": _deepcopy(_versions),
+        }
         if pack and fname is not None:
             # we get the filenames out of the results and copy the datasets
             # there. After that we check the filenames again and force them
             # to the desired directory
             from shutil import copyfile
-            fnames = (f[0] for f in self._get_dsnames(ret['arrays']))
-            alternative_paths = kwargs.pop('alternative_paths', {})
+
+            fnames = (f[0] for f in self._get_dsnames(ret["arrays"]))
+            alternative_paths = kwargs.pop("alternative_paths", {})
             counters = defaultdict(int)
-            if kwargs.get('use_rel_paths', True):
+            if kwargs.get("use_rel_paths", True):
                 get_path = partial(os.path.relpath, start=target_dir)
             else:
                 get_path = os.path.abspath
             for ds_fname in unique_everseen(chain(alternative_paths, fnames)):
                 if ds_fname is None or utils.is_remote_url(ds_fname):
                     continue
                 dst_file = alternative_paths.get(
-                    ds_fname, os.path.join(target_dir, os.path.basename(
-                        ds_fname)))
+                    ds_fname,
+                    os.path.join(target_dir, os.path.basename(ds_fname)),
+                )
                 orig_dst_file = dst_file
                 if counters[dst_file] and (
-                        not os.path.exists(dst_file) or
-                        not os.path.samefile(ds_fname, dst_file)):
+                    not os.path.exists(dst_file)
+                    or not os.path.samefile(ds_fname, dst_file)
+                ):
                     dst_file, ext = os.path.splitext(dst_file)
-                    dst_file += '-' + str(counters[orig_dst_file]) + ext
-                if (not os.path.exists(dst_file) or
-                        not os.path.samefile(ds_fname, dst_file)):
+                    dst_file += "-" + str(counters[orig_dst_file]) + ext
+                if not os.path.exists(dst_file) or not os.path.samefile(
+                    ds_fname, dst_file
+                ):
                     copyfile(ds_fname, dst_file)
                     counters[orig_dst_file] += 1
                 alternative_paths.setdefault(ds_fname, get_path(dst_file))
-            ret['arrays'] = self.array_info(
-                pwd=pwd, alternative_paths=alternative_paths, **kwargs)
+            ret["arrays"] = self.array_info(
+                pwd=pwd, alternative_paths=alternative_paths, **kwargs
+            )
         # store the plotter settings
-        for arr, d in zip(self, six.itervalues(ret['arrays'])):
+        for arr, d in zip(self, six.itervalues(ret["arrays"])):
             if arr.psy.plotter is None:
                 continue
             plotter = arr.psy.plotter
-            d['plotter'] = {
-                'ax': _ProjectLoader.inspect_axes(plotter.ax),
-                'fmt': {key: getattr(plotter, key).value2pickle
-                        for key in plotter},
-                'cls': (plotter.__class__.__module__,
-                        plotter.__class__.__name__),
-                'shared': {}}
-            d['plotter']['ax']['shared'] = set(
-                other.psy.arr_name for other in self
-                if other.psy.ax == plotter.ax)
+            d["plotter"] = {
+                "ax": _ProjectLoader.inspect_axes(plotter.ax),
+                "fmt": {
+                    key: getattr(plotter, key).value2pickle for key in plotter
+                },
+                "cls": (
+                    plotter.__class__.__module__,
+                    plotter.__class__.__name__,
+                ),
+                "shared": {},
+            }
+            d["plotter"]["ax"]["shared"] = set(
+                other.psy.arr_name
+                for other in self
+                if other.psy.ax == plotter.ax
+            )
             if plotter.ax._sharex:
-                d['plotter']['ax']['sharex'] = next(
-                    (other.psy.arr_name for other in self
-                     if other.psy.ax == plotter.ax._sharex), None)
+                d["plotter"]["ax"]["sharex"] = next(
+                    (
+                        other.psy.arr_name
+                        for other in self
+                        if other.psy.ax == plotter.ax._sharex
+                    ),
+                    None,
+                )
             if plotter.ax._sharey:
-                d['plotter']['ax']['sharey'] = next(
-                    (other.psy.arr_name for other in self
-                     if other.psy.ax == plotter.ax._sharey), None)
-            shared = d['plotter']['shared']
+                d["plotter"]["ax"]["sharey"] = next(
+                    (
+                        other.psy.arr_name
+                        for other in self
+                        if other.psy.ax == plotter.ax._sharey
+                    ),
+                    None,
+                )
+            shared = d["plotter"]["shared"]
             for fmto in plotter._fmtos:
                 if fmto.shared:
-                    shared[fmto.key] = [other_fmto.plotter.data.psy.arr_name
-                                        for other_fmto in fmto.shared]
+                    shared[fmto.key] = [
+                        other_fmto.plotter.data.psy.arr_name
+                        for other_fmto in fmto.shared
+                    ]
         if fname is not None:
-            with open(fname, 'wb') as f:
+            with open(fname, "wb") as f:
                 pickle.dump(ret, f)
             return None
 
         return ret
 
     @docstrings.dedent
     def keys(self, *args, **kwargs):
@@ -1260,14 +1390,15 @@
 
         Returns
         -------
         %(Plotter.show_keys.returns)s"""
 
         class TmpClass(Plotter):
             pass
+
         for fmto in self._fmtos:
             setattr(TmpClass, fmto.key, type(fmto)(fmto.key))
         return TmpClass.show_keys(*args, **kwargs)
 
     @docstrings.dedent
     def summaries(self, *args, **kwargs):
         """
@@ -1283,14 +1414,15 @@
 
         Returns
         -------
         %(Plotter.show_keys.returns)s"""
 
         class TmpClass(Plotter):
             pass
+
         for fmto in self._fmtos:
             setattr(TmpClass, fmto.key, type(fmto)(fmto.key))
         return TmpClass.show_summaries(*args, **kwargs)
 
     @docstrings.dedent
     def docs(self, *args, **kwargs):
         """
@@ -1306,14 +1438,15 @@
 
         Returns
         -------
         %(Plotter.show_keys.returns)s"""
 
         class TmpClass(Plotter):
             pass
+
         for fmto in self._fmtos:
             setattr(TmpClass, fmto.key, type(fmto)(fmto.key))
         return TmpClass.show_docs(*args, **kwargs)
 
     @classmethod
     @docstrings.with_indent(8)
     def from_dataset(cls, *args, **kwargs):
@@ -1330,32 +1463,42 @@
         %(ArrayList.from_dataset.other_parameters)s
 
         Returns
         -------
         Project
             The newly created project instance
         """
-        main = kwargs.pop('main', None)
+        main = kwargs.pop("main", None)
         ret = super(Project, cls).from_dataset(*args, **kwargs)
         if main is not None:
             ret.main = main
             main.extend(ret, new_name=False)
         return ret
 
-    docstrings.delete_params('ArrayList.from_dict.parameters', 'd', 'pwd')
-    docstrings.keep_params('Project._add_data.parameters', 'make_plot')
-    docstrings.keep_params('Project._add_data.parameters', 'clear')
+    docstrings.delete_params("ArrayList.from_dict.parameters", "d", "pwd")
+    docstrings.keep_params("Project._add_data.parameters", "make_plot")
+    docstrings.keep_params("Project._add_data.parameters", "clear")
 
     @classmethod
-    @docstrings.get_sections(base='Project.load_project')
+    @docstrings.get_sections(base="Project.load_project")
     @docstrings.dedent
-    def load_project(cls, fname, auto_update=None, make_plot=True,
-                     draw=False, alternative_axes=None, main=False,
-                     encoding=None, enable_post=False, new_fig=True,
-                     clear=None, **kwargs):
+    def load_project(
+        cls,
+        fname,
+        auto_update=None,
+        make_plot=True,
+        draw=False,
+        alternative_axes=None,
+        main=False,
+        encoding=None,
+        enable_post=False,
+        new_fig=True,
+        clear=None,
+        **kwargs,
+    ):
         """
         Load a project from a file or dict
 
         This classmethod allows to load a project that has been stored using
         the :meth:`save_project` method and reads all the data and creates the
         figures.
 
@@ -1421,128 +1564,161 @@
             ax_base = next(iter(obj(arr_name=name).axes), None)
             if ax_base is None:
                 ax_base = next(iter(obj(arr_name=alternatives).axes), None)
             if ax_base is not None:
                 alternatives.difference_update(obj(ax=ax_base).arr_names)
             return ax_base
 
-        pwd = kwargs.pop('pwd', None)
+        def join_axes(grouper_view, *axes):
+            """Join multiple axes together"""
+            try:
+                grouper = grouper_view._grouper
+            except AttributeError:  # matplotlib 3.5
+                grouper = grouper_view
+            grouper.join(*axes)
+
+        pwd = kwargs.pop("pwd", None)
         if isinstance(fname, six.string_types):
-            with open(fname, 'rb') as f:
-                pickle_kws = {} if not encoding else {'encoding': encoding}
+            with open(fname, "rb") as f:
+                pickle_kws = {} if not encoding else {"encoding": encoding}
                 d = pickle.load(f, **pickle_kws)
             pwd = pwd or os.path.dirname(fname)
         else:
             d = dict(fname)
-            pwd = pwd or getcwd()
+            pwd = pwd or os.getcwd()
         # check for patches of plugins
-        for ep in iter_entry_points('psyplot', name='patches'):
+        for ep in iter_entry_points("psyplot", name="patches"):
             patches = ep.load()
-            for arr_d in d.get('arrays').values():
-                plotter_cls = arr_d.get('plotter', {}).get('cls')
+            for arr_d in d.get("arrays").values():
+                plotter_cls = arr_d.get("plotter", {}).get("cls")
                 if plotter_cls is not None and plotter_cls in patches:
                     # apply the patch
-                    patches[plotter_cls](arr_d['plotter'],
-                                         d.get('versions', {}))
+                    patches[plotter_cls](
+                        arr_d["plotter"], d.get("versions", {})
+                    )
         fig_map = {}
         if alternative_axes is None:
-            for fig_dict in six.itervalues(d.get('figs', {})):
-                orig_num = fig_dict.get('num') or 1
+            for fig_dict in six.itervalues(d.get("figs", {})):
+                orig_num = fig_dict.get("num") or 1
                 fig_map[orig_num] = _ProjectLoader.load_figure(
-                    fig_dict, new_fig=new_fig).number
+                    fig_dict, new_fig=new_fig
+                ).number
         elif not isinstance(alternative_axes, dict):
             alternative_axes = cycle(iter(alternative_axes))
-        obj = cls.from_dict(d['arrays'], pwd=pwd, **kwargs)
+        obj = cls.from_dict(d["arrays"], pwd=pwd, **kwargs)
         if main:
             # we create a new project with the project factory to make sure
             # that everything is handled correctly
             obj = project(None, obj)
         axes = {}
         arr_names = obj.arr_names
         sharex = defaultdict(set)
         sharey = defaultdict(set)
         for arr, (arr_name, arr_dict) in zip(
-                obj, filter(lambda t: t[0] in arr_names,
-                            six.iteritems(d['arrays']))):
-            if not arr_dict.get('plotter'):
+            obj,
+            filter(lambda t: t[0] in arr_names, six.iteritems(d["arrays"])),
+        ):
+            if not arr_dict.get("plotter"):
                 continue
-            plot_dict = arr_dict['plotter']
+            plot_dict = arr_dict["plotter"]
             plotter_cls = getattr(
-                import_module(plot_dict['cls'][0]), plot_dict['cls'][1])
+                import_module(plot_dict["cls"][0]), plot_dict["cls"][1]
+            )
             ax = None
             if alternative_axes is not None:
                 if isinstance(alternative_axes, dict):
                     ax = alternative_axes.get(arr.arr_name)
                 else:
                     ax = next(alternative_axes, None)
-            if ax is None and 'ax' in plot_dict:
-                already_opened = plot_dict['ax'].get(
-                    'shared', set()).intersection(axes)
+            if ax is None and "ax" in plot_dict:
+                already_opened = (
+                    plot_dict["ax"].get("shared", set()).intersection(axes)
+                )
                 if already_opened:
                     ax = axes[next(iter(already_opened))]
                 else:
-                    plot_dict['ax'].pop('shared', None)
-                    plot_dict['ax']['fig'] = fig_map[
-                        plot_dict['ax'].get('fig') or 1]
-                    if plot_dict['ax'].get('sharex'):
-                        sharex[plot_dict['ax'].pop('sharex')].add(
-                            arr.psy.arr_name)
-                    if plot_dict['ax'].get('sharey'):
-                        sharey[plot_dict['ax'].pop('sharey')].add(
-                            arr.psy.arr_name)
+                    plot_dict["ax"].pop("shared", None)
+                    plot_dict["ax"]["fig"] = fig_map[
+                        plot_dict["ax"].get("fig") or 1
+                    ]
+                    if plot_dict["ax"].get("sharex"):
+                        sharex[plot_dict["ax"].pop("sharex")].add(
+                            arr.psy.arr_name
+                        )
+                    if plot_dict["ax"].get("sharey"):
+                        sharey[plot_dict["ax"].pop("sharey")].add(
+                            arr.psy.arr_name
+                        )
                     axes[arr.psy.arr_name] = ax = _ProjectLoader.load_axes(
-                        plot_dict['ax'])
+                        plot_dict["ax"]
+                    )
             plotter_cls(
-                arr, make_plot=False, draw=False, clear=False,
-                ax=ax, project=obj.main, enable_post=enable_post,
-                **plot_dict['fmt'])
+                arr,
+                make_plot=False,
+                draw=False,
+                clear=False,
+                ax=ax,
+                project=obj.main,
+                enable_post=enable_post,
+                **plot_dict["fmt"],
+            )
         # handle shared x and y-axes
         for key, names in sharex.items():
             ax_base = get_ax_base(key, names)
             if ax_base is not None:
-                ax_base.get_shared_x_axes().join(
-                    ax_base, *obj(arr_name=names).axes)
+                join_axes(
+                    ax_base.get_shared_x_axes(),
+                    ax_base,
+                    *obj(arr_name=names).axes,
+                )
                 for ax in obj(arr_name=names).axes:
                     ax._sharex = ax_base
         for key, names in sharey.items():
             ax_base = get_ax_base(key, names)
             if ax_base is not None:
-                ax_base.get_shared_y_axes().join(
-                    ax_base, *obj(arr_name=names).axes)
+                join_axes(
+                    ax_base.get_shared_y_axes(),
+                    ax_base,
+                    *obj(arr_name=names).axes,
+                )
                 for ax in obj(arr_name=names).axes:
                     ax._sharey = ax_base
         for arr in obj.with_plotter:
-            shared = d['arrays'][arr.psy.arr_name]['plotter'].get('shared', {})
+            shared = d["arrays"][arr.psy.arr_name]["plotter"].get("shared", {})
             for key, arr_names in six.iteritems(shared):
-                arr.psy.plotter.share(obj(arr_name=arr_names).plotters,
-                                      keys=[key])
+                arr.psy.plotter.share(
+                    obj(arr_name=arr_names).plotters, keys=[key]
+                )
         if make_plot:
             for plotter in obj.plotters:
                 plotter.reinit(
                     draw=False,
-                    clear=clear or (
-                        clear is None and
-                        plotter_cls._get_sample_projection() is not None))
+                    clear=clear
+                    or (
+                        clear is None
+                        and plotter_cls._get_sample_projection() is not None
+                    ),
+                )
             if draw is None:
-                draw = rcParams['auto_draw']
+                draw = rcParams["auto_draw"]
             if draw:
                 obj.draw()
-                if rcParams['auto_show']:
+                if rcParams["auto_show"]:
                     obj.show()
         if auto_update is None:
-            auto_update = rcParams['lists.auto_update']
+            auto_update = rcParams["lists.auto_update"]
         if not main:
             obj._main = gcp(True)
             obj.main.extend(obj, new_name=True)
         obj.no_auto_update = not auto_update
         scp(obj)
         return obj
 
     @classmethod
-    @docstrings.get_sections(base='Project.scp')
+    @docstrings.get_sections(base="Project.scp")
     @dedent
     def scp(cls, project):
         """
         Set the current project
 
         Parameters
         ----------
@@ -1569,15 +1745,15 @@
         else:
             _scp(project, True)
             cls.oncpchange.emit(project)
             sp = project[:]
             _scp(sp)
             cls.oncpchange.emit(sp)
 
-    docstrings.delete_params('Project.parameters', 'num')
+    docstrings.delete_params("Project.parameters", "num")
 
     @classmethod
     @docstrings.dedent
     def new(cls, num=None, *args, **kwargs):
         """
         Create a new main project
 
@@ -1599,109 +1775,121 @@
         gcp: Returns the current project
         """
         project = cls(*args, num=num, **kwargs)
         scp(project)
         return project
 
     def __str__(self):
-        return (('%i Main ' % self.num) if self.is_main else '') + super(
-            Project, self).__str__()
+        return (("%i Main " % self.num) if self.is_main else "") + super(
+            Project, self
+        ).__str__()
 
 
 class _ProjectLoader(object):
     """Class to inspect a project and reproduce it"""
 
     @staticmethod
     def inspect_figure(fig):
         """Get the parameters (heigth, width, etc.) to create a figure
 
         This method returns the number of the figure and a dictionary
         containing the necessary information for the
         :func:`matplotlib.pyplot.figure` function"""
         return fig.number, {
-            'num': fig.number,
-            'figsize': (fig.get_figwidth(), fig.get_figheight()),
-            'dpi': fig.get_dpi() / getattr(fig.canvas, '_dpi_ratio', 1),
-            'facecolor': fig.get_facecolor(),
-            'edgecolor': fig.get_edgecolor(),
-            'frameon': fig.get_frameon(),
-            'tight_layout': fig.get_tight_layout(),
-            'subplotpars': vars(fig.subplotpars)}
+            "num": fig.number,
+            "figsize": (fig.get_figwidth(), fig.get_figheight()),
+            "dpi": fig.get_dpi() / getattr(fig.canvas, "_dpi_ratio", 1),
+            "facecolor": fig.get_facecolor(),
+            "edgecolor": fig.get_edgecolor(),
+            "frameon": fig.get_frameon(),
+            "tight_layout": fig.get_tight_layout(),
+            "subplotpars": vars(fig.subplotpars),
+        }
 
     @staticmethod
     def load_figure(d, new_fig=True):
         """Create a figure from what is returned by :meth:`inspect_figure`"""
         import matplotlib.pyplot as plt
-        subplotpars = d.pop('subplotpars', None)
+
+        subplotpars = d.pop("subplotpars", None)
         if subplotpars is not None:
-            subplotpars.pop('validate', None)
-            subplotpars.pop('_validate', None)
+            subplotpars.pop("validate", None)
+            subplotpars.pop("_validate", None)
             subplotpars = mfig.SubplotParams(**subplotpars)
         if new_fig:
             nums = plt.get_fignums()
-            if d.get('num') in nums:
-                d['num'] = next(
-                    i for i in range(max(plt.get_fignums()) + 1, 0, -1)
-                    if i not in nums)
+            if d.get("num") in nums:
+                d["num"] = next(
+                    i
+                    for i in range(max(plt.get_fignums()) + 1, 0, -1)
+                    if i not in nums
+                )
         return plt.figure(subplotpars=subplotpars, **d)
 
     @staticmethod
     def inspect_axes(ax):
         """Inspect an axes or subplot to get the initialization parameters"""
-        ret = {'fig': ax.get_figure().number}
-        if mpl.__version__ < '2.0':
-            ret['axisbg'] = ax.get_axis_bgcolor()
+        ret = {"fig": ax.get_figure().number}
+        if mpl.__version__ < "2.0":
+            ret["axisbg"] = ax.get_axis_bgcolor()
         else:  # axisbg is depreceated
-            ret['facecolor'] = ax.get_facecolor()
-        proj = getattr(ax, 'projection', None)
+            ret["facecolor"] = ax.get_facecolor()
+        proj = getattr(ax, "projection", None)
         if proj is not None and not isinstance(proj, six.string_types):
             proj = (proj.__class__.__module__, proj.__class__.__name__)
-        ret['projection'] = proj
-        ret['visible'] = ax.get_visible()
-        ret['spines'] = {}
-        ret['zorder'] = ax.get_zorder()
-        ret['yaxis_inverted'] = ax.yaxis_inverted()
-        ret['xaxis_inverted'] = ax.xaxis_inverted()
+        ret["projection"] = proj
+        ret["visible"] = ax.get_visible()
+        ret["spines"] = {}
+        ret["zorder"] = ax.get_zorder()
+        ret["yaxis_inverted"] = ax.yaxis_inverted()
+        ret["xaxis_inverted"] = ax.xaxis_inverted()
         for key, val in ax.spines.items():
-            ret['spines'][key] = {}
-            for prop in ['linestyle', 'edgecolor', 'linewidth',
-                         'facecolor', 'visible']:
-                ret['spines'][key][prop] = getattr(val, 'get_' + prop)()
-        if isinstance(ax, mfig.SubplotBase):
+            ret["spines"][key] = {}
+            for prop in [
+                "linestyle",
+                "edgecolor",
+                "linewidth",
+                "facecolor",
+                "visible",
+            ]:
+                ret["spines"][key][prop] = getattr(val, "get_" + prop)()
+        if isinstance(ax, SubplotBase):
             sp = ax.get_subplotspec().get_topmost_subplotspec()
-            ret['grid_spec'] = sp.get_geometry()[:2]
-            ret['subplotspec'] = [sp.num1, sp.num2]
-            ret['is_subplot'] = True
+            ret["grid_spec"] = sp.get_geometry()[:2]
+            ret["subplotspec"] = [sp.num1, sp.num2]
+            ret["is_subplot"] = True
         else:
-            ret['args'] = [ax.get_position(True).bounds]
-            ret['is_subplot'] = False
+            ret["args"] = [ax.get_position(True).bounds]
+            ret["is_subplot"] = False
         return ret
 
     @staticmethod
     def load_axes(d):
         """Create an axes or subplot from what is returned by
         :meth:`inspect_axes`"""
         import matplotlib.pyplot as plt
-        fig = plt.figure(d.pop('fig', None))
-        proj = d.pop('projection', None)
-        spines = d.pop('spines', None)
-        invert_yaxis = d.pop('yaxis_inverted', None)
-        invert_xaxis = d.pop('xaxis_inverted', None)
-        if mpl.__version__ >= '2.0' and 'axisbg' in d:  # axisbg is depreceated
-            d['facecolor'] = d.pop('axisbg')
-        elif mpl.__version__ < '2.0' and 'facecolor' in d:
-            d['axisbg'] = d.pop('facecolor')
+
+        fig = plt.figure(d.pop("fig", None))
+        proj = d.pop("projection", None)
+        spines = d.pop("spines", None)
+        invert_yaxis = d.pop("yaxis_inverted", None)
+        invert_xaxis = d.pop("xaxis_inverted", None)
+        if mpl.__version__ >= "2.0" and "axisbg" in d:  # axisbg is depreceated
+            d["facecolor"] = d.pop("axisbg")
+        elif mpl.__version__ < "2.0" and "facecolor" in d:
+            d["axisbg"] = d.pop("facecolor")
         if proj is not None and not isinstance(proj, six.string_types):
             proj = getattr(import_module(proj[0]), proj[1])()
-        if d.pop('is_subplot', None):
-            grid_spec = mpl.gridspec.GridSpec(*d.pop('grid_spec', (1, 1)))
+        if d.pop("is_subplot", None):
+            grid_spec = mpl.gridspec.GridSpec(*d.pop("grid_spec", (1, 1)))
             subplotspec = mpl.gridspec.SubplotSpec(
-                grid_spec, *d.pop('subplotspec', (1, None)))
+                grid_spec, *d.pop("subplotspec", (1, None))
+            )
             return fig.add_subplot(subplotspec, projection=proj, **d)
-        ret = fig.add_axes(*d.pop('args', []), projection=proj, **d)
+        ret = fig.add_axes(*d.pop("args", []), projection=proj, **d)
         if spines is not None:
             for key, val in spines.items():
                 ret.spines[key].update(val)
         if invert_xaxis:
             if ret.get_xlim()[0] < ret.get_xlim()[1]:
                 ret.invert_xaxis()
         if invert_yaxis:
@@ -1720,16 +1908,17 @@
     @property
     def project(self):
         return self._project if self._project is not None else gcp(True)
 
     def __init__(self, project=None):
         self._project = project
 
-    docstrings.keep_params('ArrayList.from_dataset.parameters',
-                           'default_slice')
+    docstrings.keep_params(
+        "ArrayList.from_dataset.parameters", "default_slice"
+    )
 
     @property
     def _plot_methods(self):
         """A dictionary with mappings from plot method to their summary"""
         ret = {}
         for attr in filter(lambda s: not s.startswith("_"), dir(self)):
             obj = getattr(self, attr)
@@ -1739,20 +1928,22 @@
 
     def show_plot_methods(self):
         """Print the plotmethods of this instance"""
         print_func = PlotterInterface._print_func
         if print_func is None:
             print_func = six.print_
         s = "\n".join(
-            "%s\n    %s" % t for t in six.iteritems(self._plot_methods))
+            "%s\n    %s" % t for t in six.iteritems(self._plot_methods)
+        )
         return print_func(s)
 
-    @docstrings.get_sections(base='ProjectPlotter._add_data',
-                              sections=['Parameters', 'Other Parameters',
-                                        'Returns'])
+    @docstrings.get_sections(
+        base="ProjectPlotter._add_data",
+        sections=["Parameters", "Other Parameters", "Returns"],
+    )
     @docstrings.dedent
     def _add_data(self, *args, **kwargs):
         """
         Add new plots to the project
 
         Parameters
         ----------
@@ -1768,22 +1959,30 @@
         """
         # this method is just a shortcut to the :meth:`Project._add_data`
         # method but is reimplemented by subclasses as the
         # :class:`DatasetPlotter` or the :class:`DataArrayPlotter`
         return self.project._add_data(*args, **kwargs)
 
     @classmethod
-    @docstrings.get_sections(base='ProjectPlotter._register_plotter')
+    @docstrings.get_sections(base="ProjectPlotter._register_plotter")
     @docstrings.dedent
-    def _register_plotter(cls, identifier, module, plotter_name,
-                          plotter_cls=None, summary='', prefer_list=False,
-                          default_slice=None, default_dims={},
-                          show_examples=True,
-                          example_call="filename, name=['my_variable'], ...",
-                          plugin=None):
+    def _register_plotter(
+        cls,
+        identifier,
+        module,
+        plotter_name,
+        plotter_cls=None,
+        summary="",
+        prefer_list=False,
+        default_slice=None,
+        default_dims={},
+        show_examples=True,
+        example_call="filename, name=['my_variable'], ...",
+        plugin=None,
+    ):
         """
         Register a plotter for making plots
 
         This class method registeres a plot function for the :class:`Project`
         class under the name of the given `identifier`
 
         Parameters
@@ -1808,71 +2007,93 @@
             The arguments and keyword arguments that shall be included in the
             example of the generated plot method. This call will then appear as
             ``>>> psy.plot.%%(identifier)s(%%(example_call)s)`` in the
             documentation
         plugin: str
             The name of the plugin
         """
-        full_name = '%s.%s' % (module, plotter_name)
+        full_name = "%s.%s" % (module, plotter_name)
         if plotter_cls is not None:  # plotter has already been imported
-            docstrings.params['%s.formatoptions' % (full_name)] = \
-                plotter_cls.show_keys(
-                    indent=4, func=str,
-                    # include links in sphinx doc
-                    include_links=None)
-            doc_str = ('Possible formatoptions are\n\n'
-                       '%%(%s.formatoptions)s') % full_name
+            docstrings.params[
+                "%s.formatoptions" % (full_name)
+            ] = plotter_cls.show_keys(
+                indent=4,
+                func=str,
+                # include links in sphinx doc
+                include_links=None,
+            )
+            doc_str = (
+                "Possible formatoptions are\n\n" "%%(%s.formatoptions)s"
+            ) % full_name
         else:
-            doc_str = ''
+            doc_str = ""
 
         summary = summary or (
-            'Open and plot data via :class:`%s.%s` plotters' % (
-                module, plotter_name))
+            "Open and plot data via :class:`%s.%s` plotters"
+            % (module, plotter_name)
+        )
 
         if plotter_cls is not None:
             _versions.update(get_versions(key=lambda s: s == plugin))
 
         class PlotMethod(cls._plot_method_base_cls):
-            __doc__ = cls._gen_doc(summary, full_name, identifier,
-                                   example_call, doc_str, show_examples)
+            __doc__ = cls._gen_doc(
+                summary,
+                full_name,
+                identifier,
+                example_call,
+                doc_str,
+                show_examples,
+            )
 
             _default_slice = default_slice
             _default_dims = default_dims
             _plotter_cls = plotter_cls
             _prefer_list = prefer_list
             _plugin = plugin
 
             _summary = summary
 
         setattr(cls, identifier, PlotMethod(identifier, module, plotter_name))
 
     @classmethod
-    def _gen_doc(cls, summary, full_name, identifier, example_call, doc_str,
-                 show_examples):
+    def _gen_doc(
+        cls,
+        summary,
+        full_name,
+        identifier,
+        example_call,
+        doc_str,
+        show_examples,
+    ):
         """Generate the documentation docstring for a PlotMethod"""
-        ret = docstrings.dedent("""
+        ret = docstrings.dedent(
+            """
             %s
 
             This plotting method adds data arrays and plots them via
             :class:`%s` plotters
 
             To plot data from a netCDF file type::
 
                 >>> psy.plot.%s(%s)
 
-            %s""" % (summary, full_name, identifier, example_call, doc_str))
+            %s"""
+            % (summary, full_name, identifier, example_call, doc_str)
+        )
 
         if show_examples:
-            ret += '\n\n' + cls._gen_examples(identifier)
+            ret += "\n\n" + cls._gen_examples(identifier)
         return ret
 
     @classmethod
     def _gen_examples(cls, identifier):
         """Generate examples how to axes the formatoption docs"""
-        return docstrings.dedent("""
+        return docstrings.dedent(
+            """
             Examples
             --------
             To explore the formatoptions and their documentations, use the
             ``keys``, ``summaries`` and ``docs`` methods. For example::
 
                 >>> import psyplot.project as psy
 
@@ -1884,44 +2105,50 @@
                 # formatoption
                 >>> psy.plot.%(id)s.summaries('title')
 
                 # show the full documentation
                 >>> psy.plot.%(id)s.docs('plot')
 
                 # or access the documentation via the attribute
-                >>> psy.plot.%(id)s.plot""" % {'id': identifier})
+                >>> psy.plot.%(id)s.plot"""
+            % {"id": identifier}
+        )
 
 
 class PlotterInterface(object):
     """Base class for visualizing a data array from an predefined plotter
 
     See the :meth:`__call__` method for details on plotting."""
 
     @property
     def _logger(self):
-        name = '%s.%s.%s' % (self.__module__, self.__class__.__name__,
-                             self._method)
+        name = "%s.%s.%s" % (
+            self.__module__,
+            self.__class__.__name__,
+            self._method,
+        )
         return logging.getLogger(name)
 
     @property
     def is_imported(self):
         """True if the module for this plot method has been imported already"""
         return self.module in sys.modules
 
     @property
     def plotter_cls(self):
         """The plotter class"""
         ret = self._plotter_cls
         if ret is None:
-            self._logger.debug('importing %s', self.module)
+            self._logger.debug("importing %s", self.module)
             mod = import_module(self.module)
             plotter = self.plotter_name
             if plotter not in vars(mod):
-                raise ImportError("Module %r does not have a %r plotter!" % (
-                    mod, plotter))
+                raise ImportError(
+                    "Module %r does not have a %r plotter!" % (mod, plotter)
+                )
             ret = self._plotter_cls = getattr(mod, plotter)
             _versions.update(get_versions(key=lambda s: s == self._plugin))
         return ret
 
     _prefer_list = False
     _default_slice = None
     _default_dims = {}
@@ -1942,16 +2169,17 @@
 
     def __init__(self, methodname, module, plotter_name, project_plotter=None):
         self._method = methodname
         self._project_plotter = project_plotter
         self.module = module
         self.plotter_name = plotter_name
 
-    docstrings.delete_params('ProjectPlotter._add_data.parameters',
-                             'plotter_cls')
+    docstrings.delete_params(
+        "ProjectPlotter._add_data.parameters", "plotter_cls"
+    )
 
     @docstrings.dedent
     def __call__(self, *args, **kwargs):
         """
         Parameters
         ----------
         %(ProjectPlotter._add_data.parameters.no_plotter_cls)s
@@ -1962,64 +2190,84 @@
         %(ProjectPlotter._add_data.other_parameters)s
 
 
         Returns
         -------
         %(ProjectPlotter._add_data.returns)s
         """
-        preset = kwargs.pop('preset', None)
+        preset = kwargs.pop("preset", None)
         if preset:
             preset = self._project_plotter.project._load_preset(preset)
             if len(args) >= 2:
                 fmt = args[1]
             else:
-                fmt = kwargs.setdefault('fmt', {})
+                fmt = kwargs.setdefault("fmt", {})
             for key, val in preset.get(self._method, {}).items():
                 fmt.setdefault(key, val)
             valid = list(self.plotter_cls._get_formatoptions())
             for key, val in preset.items():
                 if key in valid:
                     fmt.setdefault(key, val)
 
         return self._project_plotter._add_data(
-            self.plotter_cls, *args, **dict(chain(
-                [('prefer_list', self._prefer_list),
-                 ('default_slice', self._default_slice)],
-                six.iteritems(self._default_dims), six.iteritems(kwargs))))
+            self.plotter_cls,
+            *args,
+            **dict(
+                chain(
+                    [
+                        ("prefer_list", self._prefer_list),
+                        ("default_slice", self._default_slice),
+                    ],
+                    six.iteritems(self._default_dims),
+                    six.iteritems(kwargs),
+                )
+            ),
+        )
 
     def __getattr__(self, attr):
         if attr in self.plotter_cls._get_formatoptions():
-            return partial(self.print_func,
-                           getattr(self.plotter_cls, attr).__doc__)
+            return partial(
+                self.print_func, getattr(self.plotter_cls, attr).__doc__
+            )
         else:
             raise AttributeError(
-                "%s instance does not have a %s attribute" % (
-                    self.__class__.__name__, attr))
+                "%s instance does not have a %s attribute"
+                % (self.__class__.__name__, attr)
+            )
 
     def __get__(self, instance, owner):
         if instance is None:
             return self
         else:
             try:
-                return getattr(instance, '_' + self._method)
+                return getattr(instance, "_" + self._method)
             except AttributeError:
-                setattr(instance, '_' + self._method, self.__class__(
-                    self._method, self.module, self.plotter_name,
-                    instance))
-                return getattr(instance, '_' + self._method)
+                setattr(
+                    instance,
+                    "_" + self._method,
+                    self.__class__(
+                        self._method, self.module, self.plotter_name, instance
+                    ),
+                )
+                return getattr(instance, "_" + self._method)
 
     def __set__(self, instance, value):
         """Actually not required. We just implement it to ensure the python
         "help" function works well"""
-        setattr(instance, '_' + self._method, value)
+        setattr(instance, "_" + self._method, value)
 
     def __dir__(self):
         try:
-            return sorted(chain(dir(self.__class__), self.__dict__,
-                                self.plotter_cls._get_formatoptions()))
+            return sorted(
+                chain(
+                    dir(self.__class__),
+                    self.__dict__,
+                    self.plotter_cls._get_formatoptions(),
+                )
+            )
         except Exception:
             return sorted(chain(dir(self.__class__), self.__dict__))
 
     @docstrings.dedent
     def keys(self, *args, **kwargs):
         """
         Classmethod to return a nice looking table with the given formatoptions
@@ -2122,48 +2370,62 @@
             decoders = [CFDecoder.get_decoder(ds, var) for var in variables]
         else:
             for i, (decoder, var) in enumerate(zip(decoders, variables)):
                 if decoder is None:
                     decoder = {}
                 if isinstance(decoder, dict):
                     decoders[i] = CFDecoder.get_decoder(ds, var, **decoder)
-        default_slice = slice(None) if self._default_slice is None else \
-            self._default_slice
-        for i, (dim_dict, var, decoder) in enumerate(zip(
-                dims, variables, decoders)):
-            corrected = decoder.correct_dims(var, dict(chain(
-                six.iteritems(self._default_dims),
-                dim_dict.items())))
+        default_slice = (
+            slice(None) if self._default_slice is None else self._default_slice
+        )
+        for i, (dim_dict, var, decoder) in enumerate(
+            zip(dims, variables, decoders)
+        ):
+            corrected = decoder.correct_dims(
+                var,
+                dict(
+                    chain(six.iteritems(self._default_dims), dim_dict.items())
+                ),
+            )
             # now use the default slice (we don't do this before because the
             # `correct_dims` method doesn't use 'x', 'y', 'z' and 't' (as used
             # for the _default_dims) if the real dimension name is already in
             # the dictionary)
             for dim in var.dims:
                 corrected.setdefault(dim, default_slice)
             dims[i] = [
-                dim for dim, val in map(lambda t: (t[0], safe_list(t[1])),
-                                        six.iteritems(corrected))
-                if val and (len(val) > 1 or _is_slice(val[0]))]
+                dim
+                for dim, val in map(
+                    lambda t: (t[0], safe_list(t[1])), six.iteritems(corrected)
+                )
+                if val and (len(val) > 1 or _is_slice(val[0]))
+            ]
         return self.plotter_cls.check_data(
-            name, dims, [decoder.is_unstructured(var) for decoder, var in zip(
-                decoders, variables)])
+            name,
+            dims,
+            [
+                decoder.is_unstructured(var)
+                for decoder, var in zip(decoders, variables)
+            ],
+        )
 
 
 # set the base class for the :class:`ProjectPlotter` plot methods
 ProjectPlotter._plot_method_base_cls = PlotterInterface
 
 
 class DatasetPlotterInterface(PlotterInterface):
     """Interface for the :class:`DatasetPlotter` to a plotter"""
 
     # there are not changes here compared to :class:`PlotterInterface`, except
     # for a different docstring for the __call__ method
 
-    docstrings.delete_params('ProjectPlotter._add_data.parameters',
-                             'plotter_cls', 'filename_or_obj')
+    docstrings.delete_params(
+        "ProjectPlotter._add_data.parameters", "plotter_cls", "filename_or_obj"
+    )
 
     @docstrings.dedent
     def __call__(self, *args, **kwargs):
         """
         Parameters
         ----------
         %(ProjectPlotter._add_data.parameters.no_plotter_cls|filename_or_obj)s
@@ -2189,20 +2451,22 @@
 
     _plot_method_base_cls = DatasetPlotterInterface
 
     def __init__(self, ds, *args, **kwargs):
         super(DatasetPlotter, self).__init__(*args, **kwargs)
         self._ds = ds
 
-    docstrings.delete_params('ProjectPlotter._add_data.parameters',
-                             'filename_or_obj')
-
-    @docstrings.get_sections(base='ProjectPlotter._add_data',
-                              sections=['Parameters', 'Other Parameters',
-                                        'Returns'])
+    docstrings.delete_params(
+        "ProjectPlotter._add_data.parameters", "filename_or_obj"
+    )
+
+    @docstrings.get_sections(
+        base="ProjectPlotter._add_data",
+        sections=["Parameters", "Other Parameters", "Returns"],
+    )
     @docstrings.dedent
     def _add_data(self, plotter_cls, *args, **kwargs):
         """
         Add new plots to the project
 
         Parameters
         ----------
@@ -2215,43 +2479,55 @@
         Returns
         -------
         %(ProjectPlotter._add_data.returns)s
         """
         # this method is just a shortcut to the :meth:`Project._add_data`
         # method but is reimplemented by subclasses as the
         # :class:`DatasetPlotter` or the :class:`DataArrayPlotter`
-        return super(DatasetPlotter, self)._add_data(plotter_cls, self._ds,
-                                                     *args, **kwargs)
+        return super(DatasetPlotter, self)._add_data(
+            plotter_cls, self._ds, *args, **kwargs
+        )
 
     @classmethod
-    def _gen_doc(cls, summary, full_name, identifier, example_call, doc_str,
-                 show_examples):
+    def _gen_doc(
+        cls,
+        summary,
+        full_name,
+        identifier,
+        example_call,
+        doc_str,
+        show_examples,
+    ):
         """Generate the documentation docstring for a PlotMethod"""
         # leave out the first argument
-        example_call = ', '.join(map(str.strip, example_call.split(',')[1:]))
-        ret = docstrings.dedent("""
+        example_call = ", ".join(map(str.strip, example_call.split(",")[1:]))
+        ret = docstrings.dedent(
+            """
             %s
 
             This plotting method adds data arrays and plots them via
             :class:`%s` plotters
 
             To plot a variable in this dataset, type::
 
                 >>> ds.psy.plot.%s(%s)
 
-            %s""" % (summary, full_name, identifier, example_call, doc_str))
+            %s"""
+            % (summary, full_name, identifier, example_call, doc_str)
+        )
 
         if show_examples:
-            ret += '\n\n' + cls._gen_examples(identifier)
+            ret += "\n\n" + cls._gen_examples(identifier)
         return ret
 
     @classmethod
     def _gen_examples(cls, identifier):
         """Generate examples how to axes the formatoption docs"""
-        return docstrings.dedent("""
+        return docstrings.dedent(
+            """
             Examples
             --------
             To explore the formatoptions and their documentations, use the
             ``keys``, ``summaries`` and ``docs`` methods. For example::
 
                 # show the keys corresponding to a group or multiple
                 # formatopions
@@ -2261,25 +2537,27 @@
                 # formatoption
                 >>> ds.psy.plot.%(id)s.summaries('title')
 
                 # show the full documentation
                 >>> ds.psy.plot.%(id)s.docs('plot')
 
                 # or access the documentation via the attribute
-                >>> ds.psy.plot.%(id)s.plot""" % {'id': identifier})
+                >>> ds.psy.plot.%(id)s.plot"""
+            % {"id": identifier}
+        )
 
 
 class DataArrayPlotterInterface(PlotterInterface):
     """Interface for the :class:`DataArrayPlotter` to a plotter"""
 
     # we reimplement the call method because we do not use the
     # prefer_list, etc. keywords. And we reimplment the check_data method
     # because we use the data array directly
 
-    docstrings.delete_params('Plotter.parameters', 'data')
+    docstrings.delete_params("Plotter.parameters", "data")
 
     @docstrings.dedent
     def __call__(self, *args, **kwargs):
         """
         Parameters
         ----------
         %(Plotter.parameters.no_data)s
@@ -2289,40 +2567,42 @@
         -------
         psyplot.plotter.Plotter
             The plotter that visualizes the data
         """
         checks, messages = self.check_data()
         if not all(checks):
             raise ValueError(
-                'Cannot visualize the data using %s! Reasons:\n    %s' % (
-                    self.plotter_name, '\n    '.join(filter(None, messages))))
+                "Cannot visualize the data using %s! Reasons:\n    %s"
+                % (self.plotter_name, "\n    ".join(filter(None, messages)))
+            )
         return self._project_plotter._add_data(
-            self.plotter_cls, *args, **kwargs)
+            self.plotter_cls, *args, **kwargs
+        )
 
     def check_data(self, *args, **kwargs):
-        """Check whether the plotter of this plot method can visualize the data
-        """
+        """Check whether the plotter of this plot method can visualize the data"""
         plotter_cls = self.plotter_cls
         da_list = self._project_plotter._da.psy.to_interactive_list()
         return plotter_cls.check_data(
-            da_list.all_names, da_list.all_dims, da_list.is_unstructured)
+            da_list.all_names, da_list.all_dims, da_list.is_unstructured
+        )
 
 
 class DataArrayPlotter(ProjectPlotter):
     """Interface between the :class:`xarray.Dataset` and the psyplot project
 
     This class can be used to make new plots from a given dataset and add them
     to the current :func:`psyplot.project`
     """
 
     _plot_method_base_cls = DataArrayPlotterInterface
 
     def __init__(self, da, *args, **kwargs):
         super(DataArrayPlotter, self).__init__(*args, **kwargs)
-        self._da = getattr(da, 'arr', da)
+        self._da = getattr(da, "arr", da)
 
     @docstrings.dedent
     def _add_data(self, plotter_cls, *args, **kwargs):
         """
         Visualize this data array
 
         Parameters
@@ -2336,39 +2616,50 @@
         """
         # this method is just a shortcut to the :meth:`Project._add_data`
         # method but is reimplemented by subclasses as the
         # :class:`DatasetPlotter` or the :class:`DataArrayPlotter`
         return plotter_cls(self._da, *args, **kwargs)
 
     @classmethod
-    def _gen_doc(cls, summary, full_name, identifier, example_call, doc_str,
-                 show_examples):
+    def _gen_doc(
+        cls,
+        summary,
+        full_name,
+        identifier,
+        example_call,
+        doc_str,
+        show_examples,
+    ):
         """Generate the documentation docstring for a PlotMethod"""
         # leave out the first argument
-        example_call = ', '.join(map(str.strip, example_call.split(',')[1:]))
-        ret = docstrings.dedent("""
+        example_call = ", ".join(map(str.strip, example_call.split(",")[1:]))
+        ret = docstrings.dedent(
+            """
             %s
 
             This plotting method visualizes the data via a
             :class:`%s` plotters
 
             To plot a variable in this dataset, type::
 
                 >>> da.psy.plot.%s()
 
-            %s""" % (summary, full_name, identifier, doc_str))
+            %s"""
+            % (summary, full_name, identifier, doc_str)
+        )
 
         if show_examples:
-            ret += '\n\n' + cls._gen_examples(identifier)
+            ret += "\n\n" + cls._gen_examples(identifier)
         return ret
 
     @classmethod
     def _gen_examples(cls, identifier):
         """Generate examples how to axes the formatoption docs"""
-        return docstrings.dedent("""
+        return docstrings.dedent(
+            """
             Examples
             --------
             To explore the formatoptions and their documentations, use the
             ``keys``, ``summaries`` and ``docs`` methods. For example::
 
                 # show the keys corresponding to a group or multiple
                 # formatopions
@@ -2378,25 +2669,32 @@
                 # formatoption
                 >>> da.psy.plot.%(id)s.summaries('title')
 
                 # show the full documentation
                 >>> da.psy.plot.%(id)s.docs('plot')
 
                 # or access the documentation via the attribute
-                >>> da.psy.plot.%(id)s.plot""" % {'id': identifier})
+                >>> da.psy.plot.%(id)s.plot"""
+            % {"id": identifier}
+        )
 
 
 if with_cdo:
-    CDF_MOD_NCREADER = 'xarray'
+    CDF_MOD_NCREADER = "xarray"
 
-    docstrings.keep_params('Project._add_data.parameters', 'dims',
-                           'fmt', 'ax', 'make_plot', 'method')
+    docstrings.keep_params(
+        "Project._add_data.parameters",
+        "dims",
+        "fmt",
+        "ax",
+        "make_plot",
+        "method",
+    )
 
     class Cdo(_CdoBase):
-
         __doc__ = docstrings.dedent(
             """
             Subclass of the original cdo.Cdo class in the cdo.py module
 
             Requirements are a working cdo binary and the installed cdo.py
             python module.
 
@@ -2446,69 +2744,80 @@
 
                 sp = cdo.timmean(input='ifile.nc', name='temperature',
                                  plot_method=psy.plot.mapplot)
                 # and
                 sp = psy.plot.mapplot(
                     cdo.timmean(input='ifile.nc', returnCdf=True),
                     name='temperature', plot_method=psy.plot.mapplot)
-            """)
+            """
+        )
 
         def __init__(self, *args, **kwargs):
             if cdo_version < (1, 5):
-                kwargs.setdefault('cdfMod', CDF_MOD_NCREADER)
+                kwargs.setdefault("cdfMod", CDF_MOD_NCREADER)
             super(Cdo, self).__init__(*args, **kwargs)
             if cdo_version < (1, 5):
                 self.loadCdf()
 
         def loadCdf(self, *args, **kwargs):
             """Load data handler as specified by self.cdfMod"""
             if cdo_version < (1, 5):
+
                 def open_nc(*args, **kwargs):
-                    kwargs.pop('mode', None)
+                    kwargs.pop("mode", None)
                     return open_dataset(*args, **kwargs)
+
                 if self.cdfMod == CDF_MOD_NCREADER:
                     self.cdf = open_nc
                 else:
                     super(Cdo, self).loadCdf(*args, **kwargs)
             else:
                 super(Cdo, self).readCdf(*args, **kwargs)
 
         def __getattr__(self, method_name):
             def my_get(get):
-                """Wrapper for get method of Cdo class to include several plotters
-                """
+                """Wrapper for get method of Cdo class to include several plotters"""
+
                 @wraps(get)
                 def wrapper(self, *args, **kwargs):
-                    added_kwargs = {'plot_method', 'name', 'dims', 'fmt'}
+                    added_kwargs = {"plot_method", "name", "dims", "fmt"}
                     if added_kwargs.intersection(kwargs):
-                        plot_method = kwargs.pop('plot_method', None)
-                        ax = kwargs.pop('ax', None)
-                        make_plot = kwargs.pop('make_plot', True)
-                        fmt = kwargs.pop('fmt', {})
-                        dims = kwargs.pop('dims', {})
-                        name = kwargs.pop('name', None)
-                        method = kwargs.pop('method', 'isel')
+                        plot_method = kwargs.pop("plot_method", None)
+                        ax = kwargs.pop("ax", None)
+                        make_plot = kwargs.pop("make_plot", True)
+                        fmt = kwargs.pop("fmt", {})
+                        dims = kwargs.pop("dims", {})
+                        name = kwargs.pop("name", None)
+                        method = kwargs.pop("method", "isel")
                         if cdo_version < (1, 5):
-                            kwargs['returnCdf'] = True
+                            kwargs["returnCdf"] = True
                         else:
-                            kwargs['returnXDataset'] = True
+                            kwargs["returnXDataset"] = True
                         ds = get(*args, **kwargs)
                         if isinstance(plot_method, six.string_types):
                             plot_method = getattr(plot, plot_method)
                         if plot_method is None:
                             ret = Project.from_dataset(
-                                ds, name=name, dims=dims, method=method)
+                                ds, name=name, dims=dims, method=method
+                            )
                             ret.main = gcp(True)
                             return ret
                         else:
                             return plot_method(
-                                ds, name=name, fmt=fmt, dims=dims, ax=ax,
-                                make_plot=make_plot, method=method)
+                                ds,
+                                name=name,
+                                fmt=fmt,
+                                dims=dims,
+                                ax=ax,
+                                make_plot=make_plot,
+                                method=method,
+                            )
                     else:
                         return get(*args, **kwargs)
+
                 return wrapper
 
             get = my_get(super(Cdo, self).__getattr__(method_name))
             setattr(self.__class__, method_name, get)
             return get.__get__(self)
 
 
@@ -2525,16 +2834,17 @@
     See Also
     --------
     scp: Sets the current project
     project: Creates a new project"""
     if main:
         return project() if _current_project is None else _current_project
     else:
-        return gcp(True) if _current_subproject is None else \
-            _current_subproject
+        return (
+            gcp(True) if _current_subproject is None else _current_subproject
+        )
 
 
 @dedent
 def scp(project):
     """
     Set the current project
 
@@ -2551,16 +2861,17 @@
 
 def _scp(p, main=False):
     """scp version that allows a bit more control over whether the project is a
     main project or not"""
     global _current_subproject
     global _current_project
     if p is None:
-        mp = project() if main or _current_project is None else \
-            _current_project
+        mp = (
+            project() if main or _current_project is None else _current_project
+        )
         _current_subproject = Project(main=mp)
     elif not main:
         _current_subproject = p
     else:
         _current_project = p
 
 
@@ -2617,46 +2928,54 @@
     kws = dict(figs=figs, data=data, ds=ds, remove_only=remove_only)
     cp_num = gcp(True).num
     got_cp = False
     if num is None:
         project = gcp()
         scp(None)
         project.close(**kws)
-    elif num == 'all':
+    elif num == "all":
         for project in _open_projects[:]:
             project.close(**kws)
             got_cp = got_cp or project.main.num == cp_num
             del _open_projects[0]
     else:
         if isinstance(num, Project):
             project = num
         else:
-            project = [project for project in _open_projects
-                       if project.num == num][0]
+            project = [
+                project for project in _open_projects if project.num == num
+            ][0]
         project.close(**kws)
         try:
             _open_projects.remove(project)
         except ValueError:
             pass
         got_cp = got_cp or project.main.num == cp_num
     if got_cp:
         if _open_projects:
             # set last opened project to the current
             scp(_open_projects[-1])
         else:
             _scp(None, True)  # set the current project to None
 
 
-docstrings.delete_params('Project._register_plotter.parameters', 'plotter_cls')
+docstrings.delete_params("Project._register_plotter.parameters", "plotter_cls")
 
 
 @docstrings.dedent
-def register_plotter(identifier, module, plotter_name, plotter_cls=None,
-                     sorter=True, plot_func=True, import_plotter=None,
-                     **kwargs):
+def register_plotter(
+    identifier,
+    module,
+    plotter_name,
+    plotter_cls=None,
+    sorter=True,
+    plot_func=True,
+    import_plotter=None,
+    **kwargs,
+):
     """
     Register a :class:`psyplot.plotter.Plotter` for the projects
 
     This function registers plotters for the :class:`Project` class to allow
     a dynamical handling of different plotter classes.
 
     Parameters
@@ -2678,42 +2997,58 @@
         item.
 
     Other Parameters
     ----------------
     %(ProjectPlotter._register_plotter.other_parameters)s
     """
     if plotter_cls is None:
-        if ((import_plotter is None and rcParams['project.auto_import']) or
-                import_plotter):
+        if (
+            import_plotter is None and rcParams["project.auto_import"]
+        ) or import_plotter:
             try:
                 plotter_cls = getattr(import_module(module), plotter_name)
             except Exception as e:
-                critical(("Could not import %s!\n" % module) +
-                         e.message if six.PY2 else str(e))
+                critical(
+                    ("Could not import %s!\n" % module) + e.message
+                    if six.PY2
+                    else str(e)
+                )
                 return
     if sorter:
         if hasattr(Project, identifier):
             raise ValueError(
-                "Project class already has a %s attribute" % identifier)
+                "Project class already has a %s attribute" % identifier
+            )
         Project._register_plotter(
-            identifier, module, plotter_name, plotter_cls)
+            identifier, module, plotter_name, plotter_cls
+        )
     if plot_func:
         if hasattr(ProjectPlotter, identifier):
             raise ValueError(
-                "Project class already has a %s attribute" % identifier)
+                "Project class already has a %s attribute" % identifier
+            )
         ProjectPlotter._register_plotter(
-            identifier, module, plotter_name, plotter_cls, **kwargs)
+            identifier, module, plotter_name, plotter_cls, **kwargs
+        )
         DatasetPlotter._register_plotter(
-            identifier, module, plotter_name, plotter_cls, **kwargs)
+            identifier, module, plotter_name, plotter_cls, **kwargs
+        )
         DataArrayPlotter._register_plotter(
-            identifier, module, plotter_name, plotter_cls, **kwargs)
+            identifier, module, plotter_name, plotter_cls, **kwargs
+        )
     if identifier not in registered_plotters:
-        kwargs.update(dict(
-            module=module, plotter_name=plotter_name, sorter=sorter,
-            plot_func=plot_func, import_plotter=import_plotter))
+        kwargs.update(
+            dict(
+                module=module,
+                plotter_name=plotter_name,
+                sorter=sorter,
+                plot_func=plot_func,
+                import_plotter=import_plotter,
+            )
+        )
         registered_plotters[identifier] = kwargs
     return
 
 
 def unregister_plotter(identifier, sorter=True, plot_func=True):
     """
     Unregister a :class:`psyplot.plotter.Plotter` for the projects
@@ -2729,37 +3064,38 @@
     plot_func: bool
         If True, the identifier will be unregistered from the
         :class:`ProjectPlotter` class
     """
     d = registered_plotters.get(identifier, {})
     if sorter and hasattr(Project, identifier):
         delattr(Project, identifier)
-        d['sorter'] = False
+        d["sorter"] = False
     if plot_func and hasattr(ProjectPlotter, identifier):
         for cls in [ProjectPlotter, DatasetPlotter, DataArrayPlotter]:
             delattr(cls, identifier)
         try:
-            delattr(plot, '_' + identifier)
+            delattr(plot, "_" + identifier)
         except AttributeError:
             pass
-        d['plot_func'] = False
+        d["plot_func"] = False
     if sorter and plot_func:
         registered_plotters.pop(identifier, None)
 
 
 registered_plotters = {}
 
-for _identifier, _plotter_settings in rcParams['project.plotters'].items():
+for _identifier, _plotter_settings in rcParams["project.plotters"].items():
     register_plotter(_identifier, **_plotter_settings)
 
 
 def get_project_nums():
     """Returns the project numbers of the open projects"""
     return [p.num for p in _open_projects]
 
+
 #: :class:`ProjectPlotter` of the current project. See the class documentation
 #: for available plotting methods
 plot = ProjectPlotter()
 
 #: The project class that is used for creating new projects
 PROJECT_CLS = Project
```

### Comparing `psyplot-1.4.3/psyplot/sphinxext/extended_napoleon.py` & `psyplot-1.5.0/psyplot/sphinxext/extended_napoleon.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,40 +6,25 @@
 
 Notes
 -----
 If you use this module as a sphinx extension, you should not list the
 :mod:`sphinx.ext.napoleon` module in the extensions variable of your conf.py.
 This module has been tested for sphinx 1.3.1."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from abc import ABCMeta, abstractmethod
-from sphinx.ext.napoleon import (
-    NumpyDocstring, GoogleDocstring, setup as napoleon_setup)
+
+from sphinx.ext.napoleon import GoogleDocstring, NumpyDocstring
+from sphinx.ext.napoleon import setup as napoleon_setup
 
 
 class DocstringExtension(object):
     """Class that introduces a "Possible Types" section
 
     This class serves as a base class for
     :class:`sphinx.ext.napoleon.NumpyDocstring` and
@@ -50,62 +35,64 @@
     --------
     The usage is the same as for the NumpyDocstring class, but it supports
     the `Possible types` section::
 
         >>> from sphinx.ext.napoleon import Config
 
         >>> from psyplot.sphinxext.extended_napoleon import (
-        ...     ExtendedNumpyDocstring)
-        >>> config = Config(napoleon_use_param=True,
-        ...                 napoleon_use_rtype=True)
+        ...     ExtendedNumpyDocstring,
+        ... )
+        >>> config = Config(napoleon_use_param=True, napoleon_use_rtype=True)
         >>> docstring = '''
         ... Possible types
         ... --------------
         ... type1
         ...     Description of `type1`
         ... type2
         ...     Description of `type2`'''
         >>> print(ExtendedNumpyDocstring(docstring, config))
         .. rubric:: Possible types
 
         * *type1* --
           Description of `type1`
         * *type2* --
           Description of `type2`"""
+
     __metaclass__ = ABCMeta
 
     def _parse_possible_types_section(self, section):
         fields = self._consume_fields(prefer_type=True)
-        lines = ['.. rubric:: %s' % section, '']
+        lines = [".. rubric:: %s" % section, ""]
         multi = len(fields) > 1
         for _name, _type, _desc in fields:
             field = self._format_field(_name, _type, _desc)
             if multi:
-                lines.extend(self._format_block('* ', field))
+                lines.extend(self._format_block("* ", field))
             else:
                 lines.extend(field)
-        return lines + ['']
+        return lines + [""]
 
     @abstractmethod
     def _parse(self):
         pass
 
 
 class ExtendedNumpyDocstring(NumpyDocstring, DocstringExtension):
     """:class:`sphinx.ext.napoleon.NumpyDocstring` with more sections"""
 
     def _parse(self, *args, **kwargs):
-        self._sections['possible types'] = self._parse_possible_types_section
+        self._sections["possible types"] = self._parse_possible_types_section
         return super(ExtendedNumpyDocstring, self)._parse(*args, **kwargs)
 
 
 class ExtendedGoogleDocstring(GoogleDocstring, DocstringExtension):
     """:class:`sphinx.ext.napoleon.GoogleDocstring` with more sections"""
+
     def _parse(self, *args, **kwargs):
-        self._sections['possible types'] = self._parse_possible_types_section
+        self._sections["possible types"] = self._parse_possible_types_section
         return super(ExtendedGoogleDocstring, self)._parse(*args, **kwargs)
 
 
 def process_docstring(app, what, name, obj, options, lines):
     """Process the docstring for a given python object.
 
     Called when autodoc has read and processed a docstring. `lines` is a list
@@ -143,19 +130,21 @@
     Notes
     -----
     This function is (to most parts) taken from the :mod:`sphinx.ext.napoleon`
     module, sphinx version 1.3.1, and adapted to the classes defined here"""
     result_lines = lines
     if app.config.napoleon_numpy_docstring:
         docstring = ExtendedNumpyDocstring(
-            result_lines, app.config, app, what, name, obj, options)
+            result_lines, app.config, app, what, name, obj, options
+        )
         result_lines = docstring.lines()
     if app.config.napoleon_google_docstring:
         docstring = ExtendedGoogleDocstring(
-            result_lines, app.config, app, what, name, obj, options)
+            result_lines, app.config, app, what, name, obj, options
+        )
         result_lines = docstring.lines()
 
     lines[:] = result_lines[:]
 
 
 def setup(app):
     """Sphinx extension setup function
@@ -170,12 +159,13 @@
         Application object representing the Sphinx process
 
     Notes
     -----
     This function uses the setup function of the :mod:`sphinx.ext.napoleon`
     module"""
     from sphinx.application import Sphinx
+
     if not isinstance(app, Sphinx):
         return  # probably called by tests
 
-    app.connect('autodoc-process-docstring', process_docstring)
+    app.connect("autodoc-process-docstring", process_docstring)
     return napoleon_setup(app)
```

### Comparing `psyplot-1.4.3/psyplot/utils.py` & `psyplot-1.5.0/psyplot/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,105 @@
 """Miscallaneous utility functions for the psyplot package."""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
+import inspect
 import re
-import six
+import sys
 from difflib import get_close_matches
-from itertools import chain
-from psyplot.compat.pycompat import OrderedDict, filterfalse
+from itertools import chain, filterfalse
+
+import six
+
 from psyplot.docstring import dedent, docstrings
 
 
+def get_default_value(func, arg):
+    argspec = inspect.getfullargspec(func)
+    return next(
+        default
+        for a, default in zip(reversed(argspec[0]), reversed(argspec.defaults))
+        if a == arg
+    )
+
+
+def isstring(s):
+    return isinstance(s, str)
+
+
 def plugin_entrypoints(group="psyplot", name="name"):
     """This utility function gets the entry points of the psyplot plugins"""
     if sys.version_info[:2] > (3, 7):
         from importlib.metadata import entry_points
+
         try:
             eps = entry_points(group=group, name=name)
         except TypeError:  # python<3.10
-            eps = [ep for ep in entry_points().get(group, [])
-                   if ep.name ==  name]
+            eps = [
+                ep for ep in entry_points().get(group, []) if ep.name == name
+            ]
     else:
         from pkg_resources import iter_entry_points
+
         eps = iter_entry_points(group=group, name=name)
     return eps
 
 
-class DefaultOrderedDict(OrderedDict):
+class Defaultdict(dict):
     """An ordered :class:`collections.defaultdict`
 
     Taken from http://stackoverflow.com/a/6190500/562769"""
+
     def __init__(self, default_factory=None, *a, **kw):
-        if (default_factory is not None and
-           not callable(default_factory)):
-            raise TypeError('first argument must be callable')
-        OrderedDict.__init__(self, *a, **kw)
+        if default_factory is not None and not callable(default_factory):
+            raise TypeError("first argument must be callable")
+        dict.__init__(self, *a, **kw)
         self.default_factory = default_factory
 
     def __getitem__(self, key):
         try:
-            return OrderedDict.__getitem__(self, key)
+            return dict.__getitem__(self, key)
         except KeyError:
             return self.__missing__(key)
 
     def __missing__(self, key):
         if self.default_factory is None:
             raise KeyError(key)
         self[key] = value = self.default_factory()
         return value
 
     def __reduce__(self):
         if self.default_factory is None:
             args = tuple()
         else:
-            args = self.default_factory,
+            args = (self.default_factory,)
         return type(self), args, None, None, self.items()
 
     def copy(self):
         """Return a shallow copy of the dictionary"""
         return self.__copy__()
 
     def __copy__(self):
         return type(self)(self.default_factory, self)
 
     def __deepcopy__(self, memo):
         import copy
-        return type(self)(self.default_factory,
-                          copy.deepcopy(self.items()))
+
+        return type(self)(self.default_factory, copy.deepcopy(self.items()))
 
     def __repr__(self):
-        return 'DefaultOrderedDict(%s, %s)' % (self.default_factory,
-                                               OrderedDict.__repr__(self))
+        return "Defaultdict(%s, %s)" % (
+            self.default_factory,
+            dict.__repr__(self),
+        )
 
 
 class _TempBool(object):
     """Wrapper around a boolean defining an __enter__ and __exit__ method
 
     Notes
     -----
@@ -125,17 +129,20 @@
 
     def __exit__(self, type, value, tb):
         self._entered.pop(-1)
         if not self._entered:
             self.value = self.default
 
     if six.PY2:
+
         def __nonzero__(self):
             return self.value
+
     else:
+
         def __bool__(self):
             return self.value
 
     def __repr__(self):
         return repr(bool(self))
 
     def __str__(self):
@@ -168,20 +175,21 @@
     propname: str
         The attribute name to use. The _TempBool instance will be stored in the
         ``'_' + propname`` attribute of the corresponding instance
     doc: str
         The documentation of the property
     default: bool
         The default value of the _TempBool class"""
+
     def getx(self):
-        if getattr(self, '_' + propname, None) is not None:
-            return getattr(self, '_' + propname)
+        if getattr(self, "_" + propname, None) is not None:
+            return getattr(self, "_" + propname)
         else:
-            setattr(self, '_' + propname, _TempBool(default))
-        return getattr(self, '_' + propname)
+            setattr(self, "_" + propname, _TempBool(default))
+        return getattr(self, "_" + propname)
 
     def setx(self, value):
         getattr(self, propname).value = bool(value)
 
     def delx(self):
         getattr(self, propname).value = default
 
@@ -205,28 +213,33 @@
             k = key(element)
             if k not in seen:
                 seen_add(k)
                 yield element
 
 
 def is_remote_url(path):
-    patt = re.compile(r'^https?\://')
+    patt = re.compile(r"^https?\://")
     if not isinstance(path, six.string_types):
-        return all(map(patt.search, (s or '' for s in path)))
-    return bool(re.search(r'^https?\://', path))
+        return all(map(patt.search, (s or "" for s in path)))
+    return bool(re.search(r"^https?\://", path))
 
 
-@docstrings.get_sections(base='check_key', sections=['Parameters', 'Returns',
-                                                 'Raises'])
+@docstrings.get_sections(
+    base="check_key", sections=["Parameters", "Returns", "Raises"]
+)
 @dedent
-def check_key(key, possible_keys, raise_error=True,
-              name='formatoption keyword',
-              msg=("See show_fmtkeys function for possible formatopion "
-                   "keywords"),
-              *args, **kwargs):
+def check_key(
+    key,
+    possible_keys,
+    raise_error=True,
+    name="formatoption keyword",
+    msg=("See show_fmtkeys function for possible formatopion " "keywords"),
+    *args,
+    **kwargs,
+):
     """
     Checks whether the key is in a list of possible keys
 
     This function checks whether the given `key` is in `possible_keys` and if
     not looks for similar sounding keys
 
     Parameters
@@ -259,23 +272,26 @@
     Raises
     ------
     KeyError
         If the key is not a valid formatoption and `raise_error` is True"""
     if key not in possible_keys:
         similarkeys = get_close_matches(key, possible_keys, *args, **kwargs)
         if similarkeys:
-            msg = ('Unknown %s %s! Possible similiar '
-                   'frasings are %s.') % (name, key, ', '.join(similarkeys))
+            msg = ("Unknown %s %s! Possible similiar " "frasings are %s.") % (
+                name,
+                key,
+                ", ".join(similarkeys),
+            )
         else:
             msg = ("Unknown %s %s! ") % (name, key) + msg
         if not raise_error:
-            return '', similarkeys, msg
+            return "", similarkeys, msg
         raise KeyError(msg)
     else:
-        return key, [key], ''
+        return key, [key], ""
 
 
 def sort_kwargs(kwargs, *param_lists):
     """Function to sort keyword arguments and sort them into dictionaries
 
     This function returns dictionaries that contain the keyword arguments
     from `kwargs` corresponding given iterables in ``*params``
@@ -290,16 +306,20 @@
     Returns
     -------
     list
         len(params) + 1 dictionaries. Each dictionary contains the items of
         `kwargs` corresponding to the specified list in ``*param_lists``. The
         last dictionary contains the remaining items"""
     return chain(
-        ({key: kwargs.pop(key) for key in params.intersection(kwargs)}
-         for params in map(set, param_lists)), [kwargs])
+        (
+            {key: kwargs.pop(key) for key in params.intersection(kwargs)}
+            for params in map(set, param_lists)
+        ),
+        [kwargs],
+    )
 
 
 def hashable(val):
     """Test if `val` is hashable and if not, get it's string representation
 
     Parameters
     ----------
@@ -316,15 +336,15 @@
         hash(val)
     except TypeError:
         return repr(val)
     else:
         return val
 
 
-@docstrings.get_sections(base='join_dicts')
+@docstrings.get_sections(base="join_dicts")
 def join_dicts(dicts, delimiter=None, keep_all=False):
     """Join multiple dictionaries into one
 
     Parameters
     ----------
     dicts: list of dict
         A list of dictionaries
```

### Comparing `psyplot-1.4.3/psyplot/warning.py` & `psyplot-1.5.0/psyplot/warning.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,89 +6,90 @@
 
 ..autosummay::
 
     PsPylotRuntimeWarning
     PsyPlotWarning
     PsyPlotCritical"""
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import warnings
 import logging
-
+import warnings
 
 # disable a warning about "comparison to 'None' in backend_pdf which occurs
 # in the matplotlib.backends.backend_pdf.PdfPages class
 warnings.filterwarnings(
-    'ignore', 'comparison', FutureWarning, 'matplotlib.backends.backend_pdf',
-    2264)
+    "ignore",
+    "comparison",
+    FutureWarning,
+    "matplotlib.backends.backend_pdf",
+    2264,
+)
 # disable a warning about "np.array_split" that occurs for certain numpy
 # versions
 warnings.filterwarnings(
-    'ignore', 'in the future np.array_split will retain', FutureWarning,
-    'numpy.lib.shape_base', 431)
+    "ignore",
+    "in the future np.array_split will retain",
+    FutureWarning,
+    "numpy.lib.shape_base",
+    431,
+)
 # disable a warning about "elementwise comparison of a string" in the
 # matplotlib.collection.Collection.get_edgecolor method that occurs for certain
 # matplotlib and numpy versions
 warnings.filterwarnings(
-    'ignore', 'elementwise comparison failed', FutureWarning,
-    'matplotlib.collections', 590)
+    "ignore",
+    "elementwise comparison failed",
+    FutureWarning,
+    "matplotlib.collections",
+    590,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 class PsyPlotRuntimeWarning(RuntimeWarning):
     """Runtime warning that appears only ones"""
+
     pass
 
 
 class PsyPlotWarning(UserWarning):
     """Normal UserWarning for psyplot module"""
+
     pass
 
 
 class PsyPlotCritical(UserWarning):
     """Critical UserWarning for psyplot module"""
+
     pass
 
 
-warnings.simplefilter('always', PsyPlotWarning, append=True)
-warnings.simplefilter('always', PsyPlotCritical, append=True)
+_issued_psyplot_warnings = []
+
+
+warnings.simplefilter("default", PsyPlotWarning)
+warnings.simplefilter("always", PsyPlotCritical)
 
 
 def disable_warnings(critical=False):
     """Function that disables all warnings and all critical warnings (if
     critical evaluates to True) related to the psyplot Module.
     Please note that you can also configure the warnings via the
     psyplot.warning logger (logging.getLogger(psyplot.warning))."""
-    warnings.filterwarnings('ignore', '\w', PsyPlotWarning, 'psyplot', 0)
+    warnings.filterwarnings("ignore", r"\w", PsyPlotWarning, "psyplot", 0)
     if critical:
-        warnings.filterwarnings('ignore', '\w', PsyPlotCritical, 'psyplot', 0)
+        warnings.filterwarnings("ignore", r"\w", PsyPlotCritical, "psyplot", 0)
 
 
 def warn(message, category=PsyPlotWarning, logger=None):
     """wrapper around the warnings.warn function for non-critical warnings.
     logger may be a logging.Logger instance"""
     if logger is not None:
         message = "[Warning by %s]\n%s" % (logger.name, message)
@@ -107,18 +108,30 @@
 
 
 def customwarn(message, category, filename, lineno, *args, **kwargs):
     """Use the psyplot.warning logger for categories being out of
     PsyPlotWarning and PsyPlotCritical and the default warnings.showwarning
     function for all the others."""
     if category is PsyPlotWarning:
-        logger.warning(warnings.formatwarning(
-            "\n%s" % message, category, filename, lineno))
+        # for whatever reason, the `default` warnings filter does not work
+        # when hovering over plots. This is why we implement a custom warning
+        # filter here
+        key = (str(message), filename, lineno)
+        if key not in _issued_psyplot_warnings:
+            logger.warning(
+                warnings.formatwarning(
+                    "\n%s" % message, category, filename, lineno
+                )
+            )
+            _issued_psyplot_warnings.append(key)
     elif category is PsyPlotCritical:
-        logger.critical(warnings.formatwarning(
-            "\n%s" % message, category, filename, lineno),
-            exc_info=True)
+        logger.critical(
+            warnings.formatwarning(
+                "\n%s" % message, category, filename, lineno
+            ),
+            exc_info=True,
+        )
     else:
         old_showwarning(message, category, filename, lineno, *args, **kwargs)
 
 
 warnings.showwarning = customwarn
```

