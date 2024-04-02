# Comparing `tmp/mercurial-testhelpers-0.6.0.tar.gz` & `tmp/mercurial-testhelpers-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercurial-testhelpers-0.6.0.tar", last modified: Thu Oct 21 20:04:33 2021, max compression
+gzip compressed data, was "mercurial-testhelpers-0.7.0.tar", last modified: Tue Apr  2 15:24:56 2024, max compression
```

## Comparing `mercurial-testhelpers-0.6.0.tar` & `mercurial-testhelpers-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      513 2021-10-21 20:03:39.000000 mercurial-testhelpers-0.6.0/CHANGELOG.md
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       54 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12447 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8835 2021-10-21 20:00:25.000000 mercurial-testhelpers-0.6.0/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/coverage_mercurial/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2021-10-21 20:00:25.000000 mercurial-testhelpers-0.6.0/coverage_mercurial/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/coverage_mercurial/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/coverage_mercurial/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1462 2021-10-21 20:00:25.000000 mercurial-testhelpers-0.6.0/coverage_mercurial/tests/test_regexps.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       19 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/install-requirements.txt
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/mercurial_testhelpers/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      356 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      883 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/command.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1904 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/datetime.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2781 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/extension.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    21309 2021-10-21 20:00:25.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/repo_wrapper.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1496 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_command.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1333 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_extension.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17239 2021-10-21 20:00:25.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_repo_wrapper.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2850 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_using_extensions.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2051 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/ui.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      657 2021-03-25 07:22:26.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers/util.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12447 2021-10-21 20:04:32.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      865 2021-10-21 20:04:32.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2021-10-21 20:04:32.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       19 2021-10-21 20:04:32.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       41 2021-10-21 20:04:32.000000 mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/top_level.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2021-10-21 20:04:33.084926 mercurial-testhelpers-0.6.0/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1413 2021-10-21 20:03:54.000000 mercurial-testhelpers-0.6.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-04-02 15:24:56.150153 mercurial-testhelpers-0.7.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      513 2024-04-02 14:52:13.000000 mercurial-testhelpers-0.7.0/CHANGELOG.md
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       54 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10253 2024-04-02 15:24:56.150153 mercurial-testhelpers-0.7.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     8835 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-04-02 15:24:56.147153 mercurial-testhelpers-0.7.0/coverage_mercurial/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/coverage_mercurial/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-04-02 15:24:56.147153 mercurial-testhelpers-0.7.0/coverage_mercurial/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/coverage_mercurial/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1462 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/coverage_mercurial/tests/test_regexps.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       19 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/install-requirements.txt
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-04-02 15:24:56.148153 mercurial-testhelpers-0.7.0/mercurial_testhelpers/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      356 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      883 2023-12-03 12:13:44.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/command.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1904 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/datetime.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2781 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/extension.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    21733 2024-04-02 14:52:13.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/repo_wrapper.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-04-02 15:24:56.149153 mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1496 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_command.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1333 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_extension.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17239 2024-01-02 11:41:59.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_repo_wrapper.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2850 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_using_extensions.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2051 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/ui.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      657 2023-12-01 16:35:53.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers/util.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-04-02 15:24:56.149153 mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10253 2024-04-02 15:24:56.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      865 2024-04-02 15:24:56.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-04-02 15:24:56.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       19 2024-04-02 15:24:56.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       41 2024-04-02 15:24:56.000000 mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/top_level.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-04-02 15:24:56.150153 mercurial-testhelpers-0.7.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1413 2024-04-02 15:24:14.000000 mercurial-testhelpers-0.7.0/setup.py
```

### Comparing `mercurial-testhelpers-0.6.0/CHANGELOG.md` & `mercurial-testhelpers-0.7.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/PKG-INFO` & `mercurial-testhelpers-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,290 +1,288 @@
 Metadata-Version: 2.1
 Name: mercurial-testhelpers
-Version: 0.6.0
+Version: 0.7.0
 Summary: Helpers to write Python tests involving Python internals of Mercurial
-Home-page: UNKNOWN
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Project-URL: Source, https://foss.heptapod.net/mercurial/testhelpers
 Project-URL: Tracker, https://foss.heptapod.net/mercurial/testhelpers/-/issues
-Description: # Mercurial Test Helpers
-        ![test tube logo](https://foss.heptapod.net/mercurial/testhelpers/-/blob/branch/default/img/test_tube_icon_200.png)
-        
-        This is a collection of facilities to help writing integration tests
-        for Python code around Mercurial: core development and extensions or other
-        downstreams like forges and graphical user interfaces.
-        
-        It also provides a `coverage` plugin, allowing to check statements according to
-        the current Mercurial version.
-        
-        See the [Integration Tests Plan wiki page](https://www.mercurial-scm.org/wiki/IntegrationTestsPlan) for more details.
-        
-        This project is tested with its own helpers, so that many of the provided tests
-        can also be used as examples.
-        
-        It has a 100% coverage policy, enforced by pre-landing continuous integration.
-        
-        ## FAQ
-        
-        ### Goal of the project
-        
-        The goal is to include these test helpers in Mercurial core.
-        
-        Once that happens, this project will serve to provide backwards compatibility,
-        especially for extensions that need to be compatible with
-        Mercurial versions that predate inclusion in core.
-        
-        ### Is pytest mandatory?
-        
-        These helpers are just shortcuts to create setups easily and handle Mercurial
-        repositories. They don't depend themselves on a testing framework.
-        Only their own tests do.
-        
-        Tighter integration with pytest will be provided as a separate project:
-        [pytest-mercurial](https://pypi.org/project/pytest-mercurial)
-        
-        ### What are the Python and Mercurial versions supported?
-        
-        CPython 2.7, 3.7 and 3.8 are supported.
-        
-        PyPy should work if Mercurial does,
-        except maybe for the discovery of Mercurial extensions used for tests skips.
-        
-        Mercurial versions are those listed in [tox.ini](tox.ini).
-        As of this writing, these are Mercurial 4.3 to 5.9 on Python 2 and
-        5.3 to 5.9 on Python 3.
-        
-        ### Why not a generic Mercurial library?
-        
-        The choices made are oriented towards being efficient (in particular fast) for
-        the task of writing tests. Some features wouldn't be legitimate in a
-        general-purpose library, for example random commit messages and file content.
-        
-        On the other hand, some of the extra care about corner cases is not necessary:
-        users always have the option to go lower level if the helpers behave badly in
-        their case. This is much more acceptable in tests than in main application
-        code: it's better to add a missing test right away and reap the benefits
-        (non-regression, basis for main code refactors) than to postpone it for
-        breaking rules (not to say that technical debt does not exist in tests).
-        
-        ### Compatibility and stability
-        
-        This project is too young and simple to get a clear picture of what will
-        happen, but we have reasons to be optimistic.
-        
-        It was first started on Mercurial 5.2 and
-        turned out to easy to port down to 4.3. Forward compatibility won't be
-        a problem anyway once it's landed in Mercurial core.
-        The reason is that it calls Mercurial at a high level, actually often
-        through the functions that are right behind the command line interface.
-        
-        For the same reasons that compatibility seems to be easy, providing stability
-        to downstream users shouldn't be too hard once we're settled about the basic
-        names.
-        
-        Also, the fact that `bytes` are not mandatory in the API of the test helpers
-        is intended directly to help with the `bytes` vs `str` changes that
-        may happen after the final dismissal of Python 2 in Mercurial
-        (e.g `dict` keys and the like). While it's certain that such changes will be
-        painful for Mercurial developers, be it in the core or elsewhere,
-        at least if the tests setups keep working, we can hope that it will help a bit.
-        
-        ## Using the coverage plugin
-        
-        The plugin has to be [activated in `.coveragerc`](https://coverage.readthedocs.io/en/coverage-5.3/plugins.html#using-plug-ins):
-        
-        ```
-        [run]
-        plugins = coverage_mercurial
-        ```
-        
-        Statements can then annotated with comments describing the versions of Mercurial
-        that are expected to run it. Example:
-        
-        ```python
-        from mercurial import util
-        
-        if util.versiontuple() < (5, 4):
-           do_something()  # hg<5.4
-        ```
-        
-        With the comment above, the `do_something()` statement will be excluded from
-        coverage when running with, e.g, Mercurial 5.5.
-        
-        Details:
-        
-         - only simple comparisons with `<`, `>`, `=`, `<=`, and `>=` are supported.
-         - no whitespace is allowed anywhere in the annotation itself. Leading and
-           trailing words in the comment should be ignored.
-         - it's not possible to create more complex rules with and/or logical
-            connectors. Current behaviour when using several markers is unspecified
-            and will change in some future release – don't depend on it.
-         - supported Mercurial versions are of type `x.y`. Neither broader
-           specifications (e.g., `hg<5`) nor more precise ones (e.g., `hg>4.8.2`)
-           are understood. What happens with them is also unspecified, and can
-           change in any future version.
-        
-        ## Running the tests of these test helpers
-        
-        The quickest way to get a test run is to use
-        [tox](https://pypi.org/project/tox/), as this package comes with a
-        tox [configuration file](tox.ini) that defines a bunch of Python and Mercurial
-        combinations.
-        
-        0. Pre-requisites:
-           - target Python version, available on `$PATH` as `python2` or `python3`
-           - required dependencies to build Mercurial from source (Python development
-             files, usually in a package called `python$VERSION-dev` or
-             `python$VERSION-devel`)
-        
-        1. install tox
-        
-           Versions provided by package managers are usually fine.
-        
-           - Debian and derivatives: `apt install tox`
-           - Fedora: `dnf install python3-tox`
-           - MacPorts/HomeBrew: ?
-           - generic: `$somepython -m pip install tox`. This `$somepython` can be
-             completely different from those actually running the tests. Also tox is
-             among other things a `virtualenv` manager.
-        
-        2. run for a precise Python and Mercurial version: `tox -e py3-hg-5.6`.
-        
-           The first run will build Mercurial, the subsequent ones will be much
-           faster.
-        
-        3. run tox for all combinations: `tox`
-        
-           While the first run will be looong, as it will build Mercurial for all
-           version combinations, the subsequent ones are pretty reasonable:
-        
-           ```
-           $ time tox
-           (...)
-           ____________ summary ____________
-             py3-hg5.6: commands succeeded
-             py3-hg5.5: commands succeeded
-             py3-hg5.4: commands succeeded
-             py3-hg5.3: commands succeeded
-             py2-hg5.6: commands succeeded
-             py2-hg5.5: commands succeeded
-             py2-hg5.4: commands succeeded
-             py2-hg5.3: commands succeeded
-             py2-hg5.2: commands succeeded
-             py2-hg5.1: commands succeeded
-             py2-hg5.0: commands succeeded
-             py2-hg4.9: commands succeeded
-             py2-hg4.8: commands succeeded
-             py2-hg4.7: commands succeeded
-             py2-hg4.6: commands succeeded
-             py2-hg4.5: commands succeeded
-             py2-hg4.4: commands succeeded
-             py2-hg4.3: commands succeeded
-             congratulations :)
-           tox  39.53s user 5.27s system 99% cpu 45.044 total
-           ```
-        
-        ## Included examples, and how to run them
-        
-        ### examples/core
-        
-        These are actual tests from Mercurial core, translated (case of `.t` tests)
-        or not (Python tests).
-        
-        They are run as part of the main suite. If you already had a `tox` test run,
-        then you've tried them already.
-        
-        `tests/test_repo_wrapper.py` is also a source of examples to get an idea of
-        what can be done.
-        
-        ### examples/evolve
-        
-        These are toy examples of testing with the `evolve` and `topic` extensions,
-        and how the `hg-evolve` project could extend on these helpers.
-        
-        To run them, one has to use the `run-all-tests` script in a context where
-        Mercurial and hg-evolve are available. Example:
-        
-        ```
-        python3 -m venv venv_hg_evolve
-        venv_hg_evolve/bin/pip install Mercurial==5.5.2 hg-evolve
-        source venv_hg_evolve/bin/activate
-        pip install -r test-requirements.txt
-        ./run-all-tests
-        ```
-        
-        Remarks:
-        
-         - For Python 2, start with `virtualenv -p python2`, then it's the same.
-         - Often, `mercurial` is not importable right after installation in a
-           virtualenv. That's why the first `pip` above was before activation.
-         - It's also possible to run only the hg-evolve examples:
-        
-           ```
-           pytest examples/hg_evolve
-           ```
-        
-        ### examples/hg-git
-        Another toy example, this time with an additional integration need (Git itself).
-        
-        Prerequisite: `git` standard executable, available on `$PATH`.
-        
-        To run the tests, one has to use the `run-all-tests` script in a context where
-        Mercurial and hg-git are available. Example:
-        
-        ```
-        python3 -m venv venv_hg_git
-        venv_hg_git/bin/pip install Mercurial==5.6 hg-git
-        source venv_hg_git/bin/activate
-        pip install -r test-requirements.txt
-        ./run-all-tests
-        ```
-        
-        Remarks:
-        
-         - For Python 2, start with `virtualenv -p python2`, then it's the same.
-         - Often, `mercurial` is not importable right after installation in a
-           virtualenv. That's why the first `pip` above was before activation.
-         - It's also possible to run only the hg-git examples:
-        
-           ```
-           pytest examples/hg_git
-           ```
-        
-        ## Credits
-        
-        Test tube logo by User:Townie on Wikimedia Commons,
-        License Creative Commons by-sa international 4.0
-        
-        
-        ## Changelog
-        
-        ### version 0.6.0 (2021-10-21)
-        
-        - !11: new `RepoWrapper.reload()` method
-        - coverage plugin: support Mercurial versions 6.x
-        
-        ### version 0.5.0 (2021-02-17)
-        
-        - #2: options for `datetime` and timezones in methods creating commits
-        - #3: generic helper to call commands, even without repository
-        - #4: helper method to create merge commits
-        
-        ### version 0.4.0 (2020-12-20)
-        
-        - #5: keeping original path on `RepoWrapper`
-        - #6: helper methods for repository configuration (in-memory) and
-          `.hg/hgrc` writer.
-        
 Keywords: hg mercurial testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Version Control :: Mercurial
 Description-Content-Type: text/markdown
+
+# Mercurial Test Helpers
+![test tube logo](https://foss.heptapod.net/mercurial/testhelpers/-/blob/branch/default/img/test_tube_icon_200.png)
+
+This is a collection of facilities to help writing integration tests
+for Python code around Mercurial: core development and extensions or other
+downstreams like forges and graphical user interfaces.
+
+It also provides a `coverage` plugin, allowing to check statements according to
+the current Mercurial version.
+
+See the [Integration Tests Plan wiki page](https://www.mercurial-scm.org/wiki/IntegrationTestsPlan) for more details.
+
+This project is tested with its own helpers, so that many of the provided tests
+can also be used as examples.
+
+It has a 100% coverage policy, enforced by pre-landing continuous integration.
+
+## FAQ
+
+### Goal of the project
+
+The goal is to include these test helpers in Mercurial core.
+
+Once that happens, this project will serve to provide backwards compatibility,
+especially for extensions that need to be compatible with
+Mercurial versions that predate inclusion in core.
+
+### Is pytest mandatory?
+
+These helpers are just shortcuts to create setups easily and handle Mercurial
+repositories. They don't depend themselves on a testing framework.
+Only their own tests do.
+
+Tighter integration with pytest will be provided as a separate project:
+[pytest-mercurial](https://pypi.org/project/pytest-mercurial)
+
+### What are the Python and Mercurial versions supported?
+
+CPython 2.7, 3.7 and 3.8 are supported.
+
+PyPy should work if Mercurial does,
+except maybe for the discovery of Mercurial extensions used for tests skips.
+
+Mercurial versions are those listed in [tox.ini](tox.ini).
+As of this writing, these are Mercurial 4.3 to 5.9 on Python 2 and
+5.3 to 5.9 on Python 3.
+
+### Why not a generic Mercurial library?
+
+The choices made are oriented towards being efficient (in particular fast) for
+the task of writing tests. Some features wouldn't be legitimate in a
+general-purpose library, for example random commit messages and file content.
+
+On the other hand, some of the extra care about corner cases is not necessary:
+users always have the option to go lower level if the helpers behave badly in
+their case. This is much more acceptable in tests than in main application
+code: it's better to add a missing test right away and reap the benefits
+(non-regression, basis for main code refactors) than to postpone it for
+breaking rules (not to say that technical debt does not exist in tests).
+
+### Compatibility and stability
+
+This project is too young and simple to get a clear picture of what will
+happen, but we have reasons to be optimistic.
+
+It was first started on Mercurial 5.2 and
+turned out to easy to port down to 4.3. Forward compatibility won't be
+a problem anyway once it's landed in Mercurial core.
+The reason is that it calls Mercurial at a high level, actually often
+through the functions that are right behind the command line interface.
+
+For the same reasons that compatibility seems to be easy, providing stability
+to downstream users shouldn't be too hard once we're settled about the basic
+names.
+
+Also, the fact that `bytes` are not mandatory in the API of the test helpers
+is intended directly to help with the `bytes` vs `str` changes that
+may happen after the final dismissal of Python 2 in Mercurial
+(e.g `dict` keys and the like). While it's certain that such changes will be
+painful for Mercurial developers, be it in the core or elsewhere,
+at least if the tests setups keep working, we can hope that it will help a bit.
+
+## Using the coverage plugin
+
+The plugin has to be [activated in `.coveragerc`](https://coverage.readthedocs.io/en/coverage-5.3/plugins.html#using-plug-ins):
+
+```
+[run]
+plugins = coverage_mercurial
+```
+
+Statements can then annotated with comments describing the versions of Mercurial
+that are expected to run it. Example:
+
+```python
+from mercurial import util
+
+if util.versiontuple() < (5, 4):
+   do_something()  # hg<5.4
+```
+
+With the comment above, the `do_something()` statement will be excluded from
+coverage when running with, e.g, Mercurial 5.5.
+
+Details:
+
+ - only simple comparisons with `<`, `>`, `=`, `<=`, and `>=` are supported.
+ - no whitespace is allowed anywhere in the annotation itself. Leading and
+   trailing words in the comment should be ignored.
+ - it's not possible to create more complex rules with and/or logical
+    connectors. Current behaviour when using several markers is unspecified
+    and will change in some future release – don't depend on it.
+ - supported Mercurial versions are of type `x.y`. Neither broader
+   specifications (e.g., `hg<5`) nor more precise ones (e.g., `hg>4.8.2`)
+   are understood. What happens with them is also unspecified, and can
+   change in any future version.
+
+## Running the tests of these test helpers
+
+The quickest way to get a test run is to use
+[tox](https://pypi.org/project/tox/), as this package comes with a
+tox [configuration file](tox.ini) that defines a bunch of Python and Mercurial
+combinations.
+
+0. Pre-requisites:
+   - target Python version, available on `$PATH` as `python2` or `python3`
+   - required dependencies to build Mercurial from source (Python development
+     files, usually in a package called `python$VERSION-dev` or
+     `python$VERSION-devel`)
+
+1. install tox
+
+   Versions provided by package managers are usually fine.
+
+   - Debian and derivatives: `apt install tox`
+   - Fedora: `dnf install python3-tox`
+   - MacPorts/HomeBrew: ?
+   - generic: `$somepython -m pip install tox`. This `$somepython` can be
+     completely different from those actually running the tests. Also tox is
+     among other things a `virtualenv` manager.
+
+2. run for a precise Python and Mercurial version: `tox -e py3-hg-5.6`.
+
+   The first run will build Mercurial, the subsequent ones will be much
+   faster.
+
+3. run tox for all combinations: `tox`
+
+   While the first run will be looong, as it will build Mercurial for all
+   version combinations, the subsequent ones are pretty reasonable:
+
+   ```
+   $ time tox
+   (...)
+   ____________ summary ____________
+     py3-hg5.6: commands succeeded
+     py3-hg5.5: commands succeeded
+     py3-hg5.4: commands succeeded
+     py3-hg5.3: commands succeeded
+     py2-hg5.6: commands succeeded
+     py2-hg5.5: commands succeeded
+     py2-hg5.4: commands succeeded
+     py2-hg5.3: commands succeeded
+     py2-hg5.2: commands succeeded
+     py2-hg5.1: commands succeeded
+     py2-hg5.0: commands succeeded
+     py2-hg4.9: commands succeeded
+     py2-hg4.8: commands succeeded
+     py2-hg4.7: commands succeeded
+     py2-hg4.6: commands succeeded
+     py2-hg4.5: commands succeeded
+     py2-hg4.4: commands succeeded
+     py2-hg4.3: commands succeeded
+     congratulations :)
+   tox  39.53s user 5.27s system 99% cpu 45.044 total
+   ```
+
+## Included examples, and how to run them
+
+### examples/core
+
+These are actual tests from Mercurial core, translated (case of `.t` tests)
+or not (Python tests).
+
+They are run as part of the main suite. If you already had a `tox` test run,
+then you've tried them already.
+
+`tests/test_repo_wrapper.py` is also a source of examples to get an idea of
+what can be done.
+
+### examples/evolve
+
+These are toy examples of testing with the `evolve` and `topic` extensions,
+and how the `hg-evolve` project could extend on these helpers.
+
+To run them, one has to use the `run-all-tests` script in a context where
+Mercurial and hg-evolve are available. Example:
+
+```
+python3 -m venv venv_hg_evolve
+venv_hg_evolve/bin/pip install Mercurial==5.5.2 hg-evolve
+source venv_hg_evolve/bin/activate
+pip install -r test-requirements.txt
+./run-all-tests
+```
+
+Remarks:
+
+ - For Python 2, start with `virtualenv -p python2`, then it's the same.
+ - Often, `mercurial` is not importable right after installation in a
+   virtualenv. That's why the first `pip` above was before activation.
+ - It's also possible to run only the hg-evolve examples:
+
+   ```
+   pytest examples/hg_evolve
+   ```
+
+### examples/hg-git
+Another toy example, this time with an additional integration need (Git itself).
+
+Prerequisite: `git` standard executable, available on `$PATH`.
+
+To run the tests, one has to use the `run-all-tests` script in a context where
+Mercurial and hg-git are available. Example:
+
+```
+python3 -m venv venv_hg_git
+venv_hg_git/bin/pip install Mercurial==5.6 hg-git
+source venv_hg_git/bin/activate
+pip install -r test-requirements.txt
+./run-all-tests
+```
+
+Remarks:
+
+ - For Python 2, start with `virtualenv -p python2`, then it's the same.
+ - Often, `mercurial` is not importable right after installation in a
+   virtualenv. That's why the first `pip` above was before activation.
+ - It's also possible to run only the hg-git examples:
+
+   ```
+   pytest examples/hg_git
+   ```
+
+## Credits
+
+Test tube logo by User:Townie on Wikimedia Commons,
+License Creative Commons by-sa international 4.0
+
+
+## Changelog
+
+### version 0.6.0 (2021-10-21)
+
+- !11: new `RepoWrapper.reload()` method
+- coverage plugin: support Mercurial versions 6.x
+
+### version 0.5.0 (2021-02-17)
+
+- #2: options for `datetime` and timezones in methods creating commits
+- #3: generic helper to call commands, even without repository
+- #4: helper method to create merge commits
+
+### version 0.4.0 (2020-12-20)
+
+- #5: keeping original path on `RepoWrapper`
+- #6: helper methods for repository configuration (in-memory) and
+  `.hg/hgrc` writer.
```

### Comparing `mercurial-testhelpers-0.6.0/README.md` & `mercurial-testhelpers-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/coverage_mercurial/__init__.py` & `mercurial-testhelpers-0.7.0/coverage_mercurial/__init__.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/coverage_mercurial/tests/test_regexps.py` & `mercurial-testhelpers-0.7.0/coverage_mercurial/tests/test_regexps.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/command.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/command.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/datetime.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/datetime.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/extension.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/extension.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/repo_wrapper.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/repo_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Copyright 2019-2021 Georges Racinet <georges.racinet@octobus.net>
+# Copyright 2019-2023 Georges Racinet <georges.racinet@octobus.net>
+# Copyright 2024 Georges Racinet <georges.racinet@cloudcrane.io>
 #
 # This software may be used and distributed according to the terms of the
 # GNU General Public License version 2 or any later version.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 """Helpers for automatic tests.
 
@@ -15,14 +16,15 @@
 from mercurial import (
     cmdutil,
     hg,
     node,
     phases,
     pycompat,
 )
+from mercurial.util import versiontuple
 import random
 import time
 
 from .command import command
 from .datetime import (
     TimeZoneMissing,
     timestamp_offset,
@@ -36,14 +38,16 @@
 NULL_ID = node.nullid
 
 try:
     phase_names = phases.cmdphasenames
 except AttributeError:  # hg<4.8
     phase_names = phases.phasenames[:3]
 
+MERCURIAL_VERSION = versiontuple()
+
 
 def _config_key_args(args):
     """Convert arguments to bytes and take care of full dotted notation.
 
     :return: `(section, name)`, as :class:`bytes`
     """
     args = tuple(as_bytes(arg) for arg in args)
@@ -338,15 +342,20 @@
         if parent is not None:
             if isinstance(parent, bytes):
                 self.update_bin(parent)
             else:
                 self.update(parent.hex())
 
     def set_dirstate_branch(self, branch):
-        self.repo.dirstate.setbranch(as_bytes(branch))
+        if MERCURIAL_VERSION >= (6, 7):
+            # transaction argument of `setbranch` is used to register
+            # hooks for rollback, it is harmless to just pass `None`
+            self.repo.dirstate.setbranch(as_bytes(branch), None)  # hg>=6.7
+        else:
+            self.repo.dirstate.setbranch(as_bytes(branch))  # hg<6.7
 
     commit_option_handlers = dict(branch='set_dirstate_branch',
                                   )
 
     @classmethod
     def register_commit_option(cls, name, handler):
         super_registry = super(cls, cls).commit_option_handlers
```

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_command.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_extension.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_repo_wrapper.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_repo_wrapper.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/tests/test_using_extensions.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/tests/test_using_extensions.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/ui.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/ui.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers/util.py` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers/util.py`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/PKG-INFO` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,290 +1,288 @@
 Metadata-Version: 2.1
 Name: mercurial-testhelpers
-Version: 0.6.0
+Version: 0.7.0
 Summary: Helpers to write Python tests involving Python internals of Mercurial
-Home-page: UNKNOWN
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Project-URL: Source, https://foss.heptapod.net/mercurial/testhelpers
 Project-URL: Tracker, https://foss.heptapod.net/mercurial/testhelpers/-/issues
-Description: # Mercurial Test Helpers
-        ![test tube logo](https://foss.heptapod.net/mercurial/testhelpers/-/blob/branch/default/img/test_tube_icon_200.png)
-        
-        This is a collection of facilities to help writing integration tests
-        for Python code around Mercurial: core development and extensions or other
-        downstreams like forges and graphical user interfaces.
-        
-        It also provides a `coverage` plugin, allowing to check statements according to
-        the current Mercurial version.
-        
-        See the [Integration Tests Plan wiki page](https://www.mercurial-scm.org/wiki/IntegrationTestsPlan) for more details.
-        
-        This project is tested with its own helpers, so that many of the provided tests
-        can also be used as examples.
-        
-        It has a 100% coverage policy, enforced by pre-landing continuous integration.
-        
-        ## FAQ
-        
-        ### Goal of the project
-        
-        The goal is to include these test helpers in Mercurial core.
-        
-        Once that happens, this project will serve to provide backwards compatibility,
-        especially for extensions that need to be compatible with
-        Mercurial versions that predate inclusion in core.
-        
-        ### Is pytest mandatory?
-        
-        These helpers are just shortcuts to create setups easily and handle Mercurial
-        repositories. They don't depend themselves on a testing framework.
-        Only their own tests do.
-        
-        Tighter integration with pytest will be provided as a separate project:
-        [pytest-mercurial](https://pypi.org/project/pytest-mercurial)
-        
-        ### What are the Python and Mercurial versions supported?
-        
-        CPython 2.7, 3.7 and 3.8 are supported.
-        
-        PyPy should work if Mercurial does,
-        except maybe for the discovery of Mercurial extensions used for tests skips.
-        
-        Mercurial versions are those listed in [tox.ini](tox.ini).
-        As of this writing, these are Mercurial 4.3 to 5.9 on Python 2 and
-        5.3 to 5.9 on Python 3.
-        
-        ### Why not a generic Mercurial library?
-        
-        The choices made are oriented towards being efficient (in particular fast) for
-        the task of writing tests. Some features wouldn't be legitimate in a
-        general-purpose library, for example random commit messages and file content.
-        
-        On the other hand, some of the extra care about corner cases is not necessary:
-        users always have the option to go lower level if the helpers behave badly in
-        their case. This is much more acceptable in tests than in main application
-        code: it's better to add a missing test right away and reap the benefits
-        (non-regression, basis for main code refactors) than to postpone it for
-        breaking rules (not to say that technical debt does not exist in tests).
-        
-        ### Compatibility and stability
-        
-        This project is too young and simple to get a clear picture of what will
-        happen, but we have reasons to be optimistic.
-        
-        It was first started on Mercurial 5.2 and
-        turned out to easy to port down to 4.3. Forward compatibility won't be
-        a problem anyway once it's landed in Mercurial core.
-        The reason is that it calls Mercurial at a high level, actually often
-        through the functions that are right behind the command line interface.
-        
-        For the same reasons that compatibility seems to be easy, providing stability
-        to downstream users shouldn't be too hard once we're settled about the basic
-        names.
-        
-        Also, the fact that `bytes` are not mandatory in the API of the test helpers
-        is intended directly to help with the `bytes` vs `str` changes that
-        may happen after the final dismissal of Python 2 in Mercurial
-        (e.g `dict` keys and the like). While it's certain that such changes will be
-        painful for Mercurial developers, be it in the core or elsewhere,
-        at least if the tests setups keep working, we can hope that it will help a bit.
-        
-        ## Using the coverage plugin
-        
-        The plugin has to be [activated in `.coveragerc`](https://coverage.readthedocs.io/en/coverage-5.3/plugins.html#using-plug-ins):
-        
-        ```
-        [run]
-        plugins = coverage_mercurial
-        ```
-        
-        Statements can then annotated with comments describing the versions of Mercurial
-        that are expected to run it. Example:
-        
-        ```python
-        from mercurial import util
-        
-        if util.versiontuple() < (5, 4):
-           do_something()  # hg<5.4
-        ```
-        
-        With the comment above, the `do_something()` statement will be excluded from
-        coverage when running with, e.g, Mercurial 5.5.
-        
-        Details:
-        
-         - only simple comparisons with `<`, `>`, `=`, `<=`, and `>=` are supported.
-         - no whitespace is allowed anywhere in the annotation itself. Leading and
-           trailing words in the comment should be ignored.
-         - it's not possible to create more complex rules with and/or logical
-            connectors. Current behaviour when using several markers is unspecified
-            and will change in some future release – don't depend on it.
-         - supported Mercurial versions are of type `x.y`. Neither broader
-           specifications (e.g., `hg<5`) nor more precise ones (e.g., `hg>4.8.2`)
-           are understood. What happens with them is also unspecified, and can
-           change in any future version.
-        
-        ## Running the tests of these test helpers
-        
-        The quickest way to get a test run is to use
-        [tox](https://pypi.org/project/tox/), as this package comes with a
-        tox [configuration file](tox.ini) that defines a bunch of Python and Mercurial
-        combinations.
-        
-        0. Pre-requisites:
-           - target Python version, available on `$PATH` as `python2` or `python3`
-           - required dependencies to build Mercurial from source (Python development
-             files, usually in a package called `python$VERSION-dev` or
-             `python$VERSION-devel`)
-        
-        1. install tox
-        
-           Versions provided by package managers are usually fine.
-        
-           - Debian and derivatives: `apt install tox`
-           - Fedora: `dnf install python3-tox`
-           - MacPorts/HomeBrew: ?
-           - generic: `$somepython -m pip install tox`. This `$somepython` can be
-             completely different from those actually running the tests. Also tox is
-             among other things a `virtualenv` manager.
-        
-        2. run for a precise Python and Mercurial version: `tox -e py3-hg-5.6`.
-        
-           The first run will build Mercurial, the subsequent ones will be much
-           faster.
-        
-        3. run tox for all combinations: `tox`
-        
-           While the first run will be looong, as it will build Mercurial for all
-           version combinations, the subsequent ones are pretty reasonable:
-        
-           ```
-           $ time tox
-           (...)
-           ____________ summary ____________
-             py3-hg5.6: commands succeeded
-             py3-hg5.5: commands succeeded
-             py3-hg5.4: commands succeeded
-             py3-hg5.3: commands succeeded
-             py2-hg5.6: commands succeeded
-             py2-hg5.5: commands succeeded
-             py2-hg5.4: commands succeeded
-             py2-hg5.3: commands succeeded
-             py2-hg5.2: commands succeeded
-             py2-hg5.1: commands succeeded
-             py2-hg5.0: commands succeeded
-             py2-hg4.9: commands succeeded
-             py2-hg4.8: commands succeeded
-             py2-hg4.7: commands succeeded
-             py2-hg4.6: commands succeeded
-             py2-hg4.5: commands succeeded
-             py2-hg4.4: commands succeeded
-             py2-hg4.3: commands succeeded
-             congratulations :)
-           tox  39.53s user 5.27s system 99% cpu 45.044 total
-           ```
-        
-        ## Included examples, and how to run them
-        
-        ### examples/core
-        
-        These are actual tests from Mercurial core, translated (case of `.t` tests)
-        or not (Python tests).
-        
-        They are run as part of the main suite. If you already had a `tox` test run,
-        then you've tried them already.
-        
-        `tests/test_repo_wrapper.py` is also a source of examples to get an idea of
-        what can be done.
-        
-        ### examples/evolve
-        
-        These are toy examples of testing with the `evolve` and `topic` extensions,
-        and how the `hg-evolve` project could extend on these helpers.
-        
-        To run them, one has to use the `run-all-tests` script in a context where
-        Mercurial and hg-evolve are available. Example:
-        
-        ```
-        python3 -m venv venv_hg_evolve
-        venv_hg_evolve/bin/pip install Mercurial==5.5.2 hg-evolve
-        source venv_hg_evolve/bin/activate
-        pip install -r test-requirements.txt
-        ./run-all-tests
-        ```
-        
-        Remarks:
-        
-         - For Python 2, start with `virtualenv -p python2`, then it's the same.
-         - Often, `mercurial` is not importable right after installation in a
-           virtualenv. That's why the first `pip` above was before activation.
-         - It's also possible to run only the hg-evolve examples:
-        
-           ```
-           pytest examples/hg_evolve
-           ```
-        
-        ### examples/hg-git
-        Another toy example, this time with an additional integration need (Git itself).
-        
-        Prerequisite: `git` standard executable, available on `$PATH`.
-        
-        To run the tests, one has to use the `run-all-tests` script in a context where
-        Mercurial and hg-git are available. Example:
-        
-        ```
-        python3 -m venv venv_hg_git
-        venv_hg_git/bin/pip install Mercurial==5.6 hg-git
-        source venv_hg_git/bin/activate
-        pip install -r test-requirements.txt
-        ./run-all-tests
-        ```
-        
-        Remarks:
-        
-         - For Python 2, start with `virtualenv -p python2`, then it's the same.
-         - Often, `mercurial` is not importable right after installation in a
-           virtualenv. That's why the first `pip` above was before activation.
-         - It's also possible to run only the hg-git examples:
-        
-           ```
-           pytest examples/hg_git
-           ```
-        
-        ## Credits
-        
-        Test tube logo by User:Townie on Wikimedia Commons,
-        License Creative Commons by-sa international 4.0
-        
-        
-        ## Changelog
-        
-        ### version 0.6.0 (2021-10-21)
-        
-        - !11: new `RepoWrapper.reload()` method
-        - coverage plugin: support Mercurial versions 6.x
-        
-        ### version 0.5.0 (2021-02-17)
-        
-        - #2: options for `datetime` and timezones in methods creating commits
-        - #3: generic helper to call commands, even without repository
-        - #4: helper method to create merge commits
-        
-        ### version 0.4.0 (2020-12-20)
-        
-        - #5: keeping original path on `RepoWrapper`
-        - #6: helper methods for repository configuration (in-memory) and
-          `.hg/hgrc` writer.
-        
 Keywords: hg mercurial testing
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Version Control :: Mercurial
 Description-Content-Type: text/markdown
+
+# Mercurial Test Helpers
+![test tube logo](https://foss.heptapod.net/mercurial/testhelpers/-/blob/branch/default/img/test_tube_icon_200.png)
+
+This is a collection of facilities to help writing integration tests
+for Python code around Mercurial: core development and extensions or other
+downstreams like forges and graphical user interfaces.
+
+It also provides a `coverage` plugin, allowing to check statements according to
+the current Mercurial version.
+
+See the [Integration Tests Plan wiki page](https://www.mercurial-scm.org/wiki/IntegrationTestsPlan) for more details.
+
+This project is tested with its own helpers, so that many of the provided tests
+can also be used as examples.
+
+It has a 100% coverage policy, enforced by pre-landing continuous integration.
+
+## FAQ
+
+### Goal of the project
+
+The goal is to include these test helpers in Mercurial core.
+
+Once that happens, this project will serve to provide backwards compatibility,
+especially for extensions that need to be compatible with
+Mercurial versions that predate inclusion in core.
+
+### Is pytest mandatory?
+
+These helpers are just shortcuts to create setups easily and handle Mercurial
+repositories. They don't depend themselves on a testing framework.
+Only their own tests do.
+
+Tighter integration with pytest will be provided as a separate project:
+[pytest-mercurial](https://pypi.org/project/pytest-mercurial)
+
+### What are the Python and Mercurial versions supported?
+
+CPython 2.7, 3.7 and 3.8 are supported.
+
+PyPy should work if Mercurial does,
+except maybe for the discovery of Mercurial extensions used for tests skips.
+
+Mercurial versions are those listed in [tox.ini](tox.ini).
+As of this writing, these are Mercurial 4.3 to 5.9 on Python 2 and
+5.3 to 5.9 on Python 3.
+
+### Why not a generic Mercurial library?
+
+The choices made are oriented towards being efficient (in particular fast) for
+the task of writing tests. Some features wouldn't be legitimate in a
+general-purpose library, for example random commit messages and file content.
+
+On the other hand, some of the extra care about corner cases is not necessary:
+users always have the option to go lower level if the helpers behave badly in
+their case. This is much more acceptable in tests than in main application
+code: it's better to add a missing test right away and reap the benefits
+(non-regression, basis for main code refactors) than to postpone it for
+breaking rules (not to say that technical debt does not exist in tests).
+
+### Compatibility and stability
+
+This project is too young and simple to get a clear picture of what will
+happen, but we have reasons to be optimistic.
+
+It was first started on Mercurial 5.2 and
+turned out to easy to port down to 4.3. Forward compatibility won't be
+a problem anyway once it's landed in Mercurial core.
+The reason is that it calls Mercurial at a high level, actually often
+through the functions that are right behind the command line interface.
+
+For the same reasons that compatibility seems to be easy, providing stability
+to downstream users shouldn't be too hard once we're settled about the basic
+names.
+
+Also, the fact that `bytes` are not mandatory in the API of the test helpers
+is intended directly to help with the `bytes` vs `str` changes that
+may happen after the final dismissal of Python 2 in Mercurial
+(e.g `dict` keys and the like). While it's certain that such changes will be
+painful for Mercurial developers, be it in the core or elsewhere,
+at least if the tests setups keep working, we can hope that it will help a bit.
+
+## Using the coverage plugin
+
+The plugin has to be [activated in `.coveragerc`](https://coverage.readthedocs.io/en/coverage-5.3/plugins.html#using-plug-ins):
+
+```
+[run]
+plugins = coverage_mercurial
+```
+
+Statements can then annotated with comments describing the versions of Mercurial
+that are expected to run it. Example:
+
+```python
+from mercurial import util
+
+if util.versiontuple() < (5, 4):
+   do_something()  # hg<5.4
+```
+
+With the comment above, the `do_something()` statement will be excluded from
+coverage when running with, e.g, Mercurial 5.5.
+
+Details:
+
+ - only simple comparisons with `<`, `>`, `=`, `<=`, and `>=` are supported.
+ - no whitespace is allowed anywhere in the annotation itself. Leading and
+   trailing words in the comment should be ignored.
+ - it's not possible to create more complex rules with and/or logical
+    connectors. Current behaviour when using several markers is unspecified
+    and will change in some future release – don't depend on it.
+ - supported Mercurial versions are of type `x.y`. Neither broader
+   specifications (e.g., `hg<5`) nor more precise ones (e.g., `hg>4.8.2`)
+   are understood. What happens with them is also unspecified, and can
+   change in any future version.
+
+## Running the tests of these test helpers
+
+The quickest way to get a test run is to use
+[tox](https://pypi.org/project/tox/), as this package comes with a
+tox [configuration file](tox.ini) that defines a bunch of Python and Mercurial
+combinations.
+
+0. Pre-requisites:
+   - target Python version, available on `$PATH` as `python2` or `python3`
+   - required dependencies to build Mercurial from source (Python development
+     files, usually in a package called `python$VERSION-dev` or
+     `python$VERSION-devel`)
+
+1. install tox
+
+   Versions provided by package managers are usually fine.
+
+   - Debian and derivatives: `apt install tox`
+   - Fedora: `dnf install python3-tox`
+   - MacPorts/HomeBrew: ?
+   - generic: `$somepython -m pip install tox`. This `$somepython` can be
+     completely different from those actually running the tests. Also tox is
+     among other things a `virtualenv` manager.
+
+2. run for a precise Python and Mercurial version: `tox -e py3-hg-5.6`.
+
+   The first run will build Mercurial, the subsequent ones will be much
+   faster.
+
+3. run tox for all combinations: `tox`
+
+   While the first run will be looong, as it will build Mercurial for all
+   version combinations, the subsequent ones are pretty reasonable:
+
+   ```
+   $ time tox
+   (...)
+   ____________ summary ____________
+     py3-hg5.6: commands succeeded
+     py3-hg5.5: commands succeeded
+     py3-hg5.4: commands succeeded
+     py3-hg5.3: commands succeeded
+     py2-hg5.6: commands succeeded
+     py2-hg5.5: commands succeeded
+     py2-hg5.4: commands succeeded
+     py2-hg5.3: commands succeeded
+     py2-hg5.2: commands succeeded
+     py2-hg5.1: commands succeeded
+     py2-hg5.0: commands succeeded
+     py2-hg4.9: commands succeeded
+     py2-hg4.8: commands succeeded
+     py2-hg4.7: commands succeeded
+     py2-hg4.6: commands succeeded
+     py2-hg4.5: commands succeeded
+     py2-hg4.4: commands succeeded
+     py2-hg4.3: commands succeeded
+     congratulations :)
+   tox  39.53s user 5.27s system 99% cpu 45.044 total
+   ```
+
+## Included examples, and how to run them
+
+### examples/core
+
+These are actual tests from Mercurial core, translated (case of `.t` tests)
+or not (Python tests).
+
+They are run as part of the main suite. If you already had a `tox` test run,
+then you've tried them already.
+
+`tests/test_repo_wrapper.py` is also a source of examples to get an idea of
+what can be done.
+
+### examples/evolve
+
+These are toy examples of testing with the `evolve` and `topic` extensions,
+and how the `hg-evolve` project could extend on these helpers.
+
+To run them, one has to use the `run-all-tests` script in a context where
+Mercurial and hg-evolve are available. Example:
+
+```
+python3 -m venv venv_hg_evolve
+venv_hg_evolve/bin/pip install Mercurial==5.5.2 hg-evolve
+source venv_hg_evolve/bin/activate
+pip install -r test-requirements.txt
+./run-all-tests
+```
+
+Remarks:
+
+ - For Python 2, start with `virtualenv -p python2`, then it's the same.
+ - Often, `mercurial` is not importable right after installation in a
+   virtualenv. That's why the first `pip` above was before activation.
+ - It's also possible to run only the hg-evolve examples:
+
+   ```
+   pytest examples/hg_evolve
+   ```
+
+### examples/hg-git
+Another toy example, this time with an additional integration need (Git itself).
+
+Prerequisite: `git` standard executable, available on `$PATH`.
+
+To run the tests, one has to use the `run-all-tests` script in a context where
+Mercurial and hg-git are available. Example:
+
+```
+python3 -m venv venv_hg_git
+venv_hg_git/bin/pip install Mercurial==5.6 hg-git
+source venv_hg_git/bin/activate
+pip install -r test-requirements.txt
+./run-all-tests
+```
+
+Remarks:
+
+ - For Python 2, start with `virtualenv -p python2`, then it's the same.
+ - Often, `mercurial` is not importable right after installation in a
+   virtualenv. That's why the first `pip` above was before activation.
+ - It's also possible to run only the hg-git examples:
+
+   ```
+   pytest examples/hg_git
+   ```
+
+## Credits
+
+Test tube logo by User:Townie on Wikimedia Commons,
+License Creative Commons by-sa international 4.0
+
+
+## Changelog
+
+### version 0.6.0 (2021-10-21)
+
+- !11: new `RepoWrapper.reload()` method
+- coverage plugin: support Mercurial versions 6.x
+
+### version 0.5.0 (2021-02-17)
+
+- #2: options for `datetime` and timezones in methods creating commits
+- #3: generic helper to call commands, even without repository
+- #4: helper method to create merge commits
+
+### version 0.4.0 (2020-12-20)
+
+- #5: keeping original path on `RepoWrapper`
+- #6: helper methods for repository configuration (in-memory) and
+  `.hg/hgrc` writer.
```

### Comparing `mercurial-testhelpers-0.6.0/mercurial_testhelpers.egg-info/SOURCES.txt` & `mercurial-testhelpers-0.7.0/mercurial_testhelpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercurial-testhelpers-0.6.0/setup.py` & `mercurial-testhelpers-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('install-requirements.txt', 'r') as install_reqf:
     install_req = [req.strip() for req in install_reqf]
 
 
 setup(
     name='mercurial-testhelpers',
-    version='0.6.0',
+    version='0.7.0',
     author='Georges Racinet',
     author_email='georges.racinet@octobus.net',
     project_urls=dict(
         Source='https://foss.heptapod.net/mercurial/testhelpers',
         Tracker='https://foss.heptapod.net/mercurial/testhelpers/-/issues',
     ),
     description="Helpers to write Python tests involving "
```

