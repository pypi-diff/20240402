# Comparing `tmp/redpic-1.0.0.1.tar.gz` & `tmp/redpic-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redpic-1.0.0.1.tar", last modified: Thu Aug 24 08:04:43 2023, max compression
+gzip compressed data, was "redpic-1.0.0.2.tar", last modified: Thu Aug 24 08:11:28 2023, max compression
```

## Comparing `redpic-1.0.0.1.tar` & `redpic-1.0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fuodorov   (501) staff       (20)        0 2023-08-24 08:04:43.055368 redpic-1.0.0.1/
--rw-r--r--   0 fuodorov   (501) staff       (20)     1075 2023-08-24 07:25:28.000000 redpic-1.0.0.1/LICENSE
--rw-r--r--   0 fuodorov   (501) staff       (20)        0 2023-08-24 07:25:28.000000 redpic-1.0.0.1/MANIFEST.in
--rw-r--r--   0 fuodorov   (501) staff       (20)     4910 2023-08-24 08:04:43.055061 redpic-1.0.0.1/PKG-INFO
--rw-r--r--   0 fuodorov   (501) staff       (20)     4367 2023-08-24 07:25:28.000000 redpic-1.0.0.1/README.md
--rw-r--r--   0 fuodorov   (501) staff       (20)       62 2023-08-24 07:25:28.000000 redpic-1.0.0.1/pyproject.toml
-drwxr-xr-x   0 fuodorov   (501) staff       (20)        0 2023-08-24 08:04:43.051725 redpic-1.0.0.1/redpic/
--rw-r--r--   0 fuodorov   (501) staff       (20)      363 2023-08-24 07:25:28.000000 redpic-1.0.0.1/redpic/__init__.py
--rw-r--r--   0 fuodorov   (501) staff       (20)      146 2023-08-24 07:25:28.000000 redpic-1.0.0.1/redpic/accelerator.py
--rw-r--r--   0 fuodorov   (501) staff       (20)     6582 2023-08-24 07:25:28.000000 redpic-1.0.0.1/redpic/beam.py
--rw-r--r--   0 fuodorov   (501) staff       (20)     1893 2023-08-24 07:25:28.000000 redpic-1.0.0.1/redpic/constants.py
--rw-r--r--   0 fuodorov   (501) staff       (20)     9246 2023-08-24 07:25:28.000000 redpic-1.0.0.1/redpic/solver.py
-drwxr-xr-x   0 fuodorov   (501) staff       (20)        0 2023-08-24 08:04:43.054577 redpic-1.0.0.1/redpic.egg-info/
--rw-r--r--   0 fuodorov   (501) staff       (20)     4910 2023-08-24 08:04:42.000000 redpic-1.0.0.1/redpic.egg-info/PKG-INFO
--rw-r--r--   0 fuodorov   (501) staff       (20)      266 2023-08-24 08:04:42.000000 redpic-1.0.0.1/redpic.egg-info/SOURCES.txt
--rw-r--r--   0 fuodorov   (501) staff       (20)        1 2023-08-24 08:04:42.000000 redpic-1.0.0.1/redpic.egg-info/dependency_links.txt
--rw-r--r--   0 fuodorov   (501) staff       (20)        7 2023-08-24 08:04:42.000000 redpic-1.0.0.1/redpic.egg-info/top_level.txt
--rw-r--r--   0 fuodorov   (501) staff       (20)       38 2023-08-24 08:04:43.055483 redpic-1.0.0.1/setup.cfg
--rw-r--r--   0 fuodorov   (501) staff       (20)      754 2023-08-24 07:47:41.000000 redpic-1.0.0.1/setup.py
+drwxr-xr-x   0 fuodorov   (501) staff       (20)        0 2023-08-24 08:11:28.613943 redpic-1.0.0.2/
+-rw-r--r--   0 fuodorov   (501) staff       (20)     1075 2023-08-24 07:25:28.000000 redpic-1.0.0.2/LICENSE
+-rw-r--r--   0 fuodorov   (501) staff       (20)        0 2023-08-24 07:25:28.000000 redpic-1.0.0.2/MANIFEST.in
+-rw-r--r--   0 fuodorov   (501) staff       (20)     5911 2023-08-24 08:11:28.613579 redpic-1.0.0.2/PKG-INFO
+-rw-r--r--   0 fuodorov   (501) staff       (20)     4367 2023-08-24 07:25:28.000000 redpic-1.0.0.2/README.md
+-rw-r--r--   0 fuodorov   (501) staff       (20)       62 2023-08-24 07:25:28.000000 redpic-1.0.0.2/pyproject.toml
+drwxr-xr-x   0 fuodorov   (501) staff       (20)        0 2023-08-24 08:11:28.610425 redpic-1.0.0.2/redpic/
+-rw-r--r--   0 fuodorov   (501) staff       (20)      363 2023-08-24 08:08:13.000000 redpic-1.0.0.2/redpic/__init__.py
+-rw-r--r--   0 fuodorov   (501) staff       (20)      146 2023-08-24 07:25:28.000000 redpic-1.0.0.2/redpic/accelerator.py
+-rw-r--r--   0 fuodorov   (501) staff       (20)     6582 2023-08-24 07:25:28.000000 redpic-1.0.0.2/redpic/beam.py
+-rw-r--r--   0 fuodorov   (501) staff       (20)     1893 2023-08-24 07:25:28.000000 redpic-1.0.0.2/redpic/constants.py
+-rw-r--r--   0 fuodorov   (501) staff       (20)     9246 2023-08-24 07:25:28.000000 redpic-1.0.0.2/redpic/solver.py
+drwxr-xr-x   0 fuodorov   (501) staff       (20)        0 2023-08-24 08:11:28.612287 redpic-1.0.0.2/redpic.egg-info/
+-rw-r--r--   0 fuodorov   (501) staff       (20)     5911 2023-08-24 08:11:28.000000 redpic-1.0.0.2/redpic.egg-info/PKG-INFO
+-rw-r--r--   0 fuodorov   (501) staff       (20)      266 2023-08-24 08:11:28.000000 redpic-1.0.0.2/redpic.egg-info/SOURCES.txt
+-rw-r--r--   0 fuodorov   (501) staff       (20)        1 2023-08-24 08:11:28.000000 redpic-1.0.0.2/redpic.egg-info/dependency_links.txt
+-rw-r--r--   0 fuodorov   (501) staff       (20)        7 2023-08-24 08:11:28.000000 redpic-1.0.0.2/redpic.egg-info/top_level.txt
+-rw-r--r--   0 fuodorov   (501) staff       (20)       38 2023-08-24 08:11:28.614077 redpic-1.0.0.2/setup.cfg
+-rw-r--r--   0 fuodorov   (501) staff       (20)      754 2023-08-24 07:47:41.000000 redpic-1.0.0.2/setup.py
```

### Comparing `redpic-1.0.0.1/LICENSE` & `redpic-1.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redpic-1.0.0.1/PKG-INFO` & `redpic-1.0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: redpic
-Version: 1.0.0.1
-Summary: Relativictic Difference Scheme Particle-in-Cell code (REDPIC)
-Home-page: https://github.com/fuodorov/redpic
-Author: Vyacheslav Fedorov
-Author-email: slava@fuodorov.ru
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Relativistic Difference Scheme Particles-In-Cell (REDPIC)
 [![PyPI version](https://badge.fury.io/py/redpic.svg)](https://badge.fury.io/py/redpic)
 
 This PIC code has been developed since 2020 at the Budker Institute of Nuclear Physics as an alternative to 
 [ASTRA](https://www.desy.de/~mpyflo/), 
 [WARP](https://bitbucket.org/berkeleylab/warp/), 
 [XTRACK](https://xsuite.readthedocs.io/en/latest/) 
@@ -131,8 +116,8 @@
 Use `make lint` to run only linters for current python version
 
 ### Maintaining
 If pull request consists of several meaningful commits, that should be preserved, 
 then use "Rebase and merge" option. Otherwise use "Squash and merge". 
 
 New release (changelog, tag and pypi upload) will be automatically created 
-on each push to master via Github Actions workflow.
+on each push to master via Github Actions workflow.
```

### Comparing `redpic-1.0.0.1/README.md` & `redpic-1.0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,138 @@
-# Relativistic Difference Scheme Particles-In-Cell (REDPIC)
-[![PyPI version](https://badge.fury.io/py/redpic.svg)](https://badge.fury.io/py/redpic)
-
-This PIC code has been developed since 2020 at the Budker Institute of Nuclear Physics as an alternative to 
-[ASTRA](https://www.desy.de/~mpyflo/), 
-[WARP](https://bitbucket.org/berkeleylab/warp/), 
-[XTRACK](https://xsuite.readthedocs.io/en/latest/) 
-and other codes. 
-
-For particle dynamics simulation using finite difference scheme relativistic.
-
-## Table of content 
-
--   [Getting Started](#getting-started)
-    -   [Local build and launch](#local-build-and-launch)
-    -   [Documentation](#documentation)
-        -   [Adding a new section](#adding-a-new-section)
-    -   [Additional resources](#additional-resources)
--   [Prerequisites](#prerequisites)
-    -   [Latex](#latex)
--   [Useful Resources](#useful-resources)
-    -   [IDE](#ide)
--   [Authors](#authors)
--   [Licence](#license)
--   [Contributing](#contributing)
-    -   [Dependencies](#dependencies)
-    -   [Formatting](#formatting)
-    -   [Tests](#tests)
-    -   [Maintaining](#maintaining)
-
-## Getting Started
-
-### Local build and launch
-
-To build our application and create a Docker image, it will be enough to run the following command:
-
-`docker build -t redpic .`
-
-To launch the application, use the command:
-
-`docker run -it redpic`
-
-### Documentation
-
-The documentation contains all the Latex files needed to generate documentation. 
-The main source files are located in the `docs/src`.
-
-* [main.tex](/docs/src/main.tex) is documentation source file. 
-The final PDF can be found [here](/docs/out/main.pdf).
-
-[main.tex](/docs/src/main.tex) is the source file that Latex compiler will use to generate the paper. 
-However, in order to keep the code cleaner, the main sections of the paper are all located in the [sections](/docs/src/sections). 
-In this way you will experience less merging issues when two or more people are working on the same doc.
-
-Just edit the text in the relative Latex file (e.g., introduction, methodology, etc.) and you should be ready to go. 
-No need to change any other file.
-
-#### Adding a new section
-
-Just copy a section file (e.g., [introduction.tex](/docs/src/sections/introduction.tex)) paste it in the same directory. 
-Rename the pasted file (e.g. first_chapter.tex) and add this file to [main.tex](/docs/src/main.tex).
-
-### Additional Resources
-
-Alternatively you can find great resources on the 
-[Overleaf Tutorial website](https://www.overleaf.com/learn/latex/Tutorials) or on 
-[Latex wikibooks](https://en.wikibooks.org/wiki/LaTeX).
-
-## Prerequisites
-
-#### Latex
-
-Latex IDE and compiler installed locally on your machine. 
-We recommend using a PyCharm plugin called [TeXiFy IDEA](https://plugins.jetbrains.com/plugin/9473-texify-idea) as IDE and 
-[miktex](https://miktex.org) as Latex compiler  
-
-Alternatively you can push your code to Overleaf using git and only use Overleaf. 
-We would discourage you from doing this! Overleaf should only be used for the review.
-
-## Useful Resources
-
-### IDE
-
-You may want to take advantage of the power of IDEs. 
-For Python We would recommend using [PyCharm](https://www.jetbrains.com/pycharm/). 
-
-Alternatives are:
-
-* [Visual Studio](https://code.visualstudio.com)
-* [Atom](https://atom.io/)
-
-### Git
-
-You should install [git](https://git-scm.com) on your computer. And have [GitHub](https://github.com) account.
-
-## Authors
-
-* **[Vyacheslav Fedorov](https://github.com/fuodorov)** - *Initial work*
-* **[Danila Nikiforov](https://github.com/Danila-Nikiforov)** - *Initial work*
-
-See also the list of [contributors](https://github.com/binp-dev/redpic/contributors) who participated in this project.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-## Contributing
-
-### Dependencies
-Use `make deps` command to install library, its production and development dependencies.
-
-### Formatting
-Use `make format` to autoformat code with black tool. 
-
-### Tests
-Use `make lint` to run only linters for current python version
-
-### Maintaining
-If pull request consists of several meaningful commits, that should be preserved, 
-then use "Rebase and merge" option. Otherwise use "Squash and merge". 
-
-New release (changelog, tag and pypi upload) will be automatically created 
-on each push to master via Github Actions workflow.
+Metadata-Version: 2.1
+Name: redpic
+Version: 1.0.0.2
+Summary: Relativictic Difference Scheme Particle-in-Cell code (REDPIC)
+Home-page: https://github.com/fuodorov/redpic
+Author: Vyacheslav Fedorov
+Author-email: slava@fuodorov.ru
+License: UNKNOWN
+Description: # Relativistic Difference Scheme Particles-In-Cell (REDPIC)
+        [![PyPI version](https://badge.fury.io/py/redpic.svg)](https://badge.fury.io/py/redpic)
+        
+        This PIC code has been developed since 2020 at the Budker Institute of Nuclear Physics as an alternative to 
+        [ASTRA](https://www.desy.de/~mpyflo/), 
+        [WARP](https://bitbucket.org/berkeleylab/warp/), 
+        [XTRACK](https://xsuite.readthedocs.io/en/latest/) 
+        and other codes. 
+        
+        For particle dynamics simulation using finite difference scheme relativistic.
+        
+        ## Table of content 
+        
+        -   [Getting Started](#getting-started)
+            -   [Local build and launch](#local-build-and-launch)
+            -   [Documentation](#documentation)
+                -   [Adding a new section](#adding-a-new-section)
+            -   [Additional resources](#additional-resources)
+        -   [Prerequisites](#prerequisites)
+            -   [Latex](#latex)
+        -   [Useful Resources](#useful-resources)
+            -   [IDE](#ide)
+        -   [Authors](#authors)
+        -   [Licence](#license)
+        -   [Contributing](#contributing)
+            -   [Dependencies](#dependencies)
+            -   [Formatting](#formatting)
+            -   [Tests](#tests)
+            -   [Maintaining](#maintaining)
+        
+        ## Getting Started
+        
+        ### Local build and launch
+        
+        To build our application and create a Docker image, it will be enough to run the following command:
+        
+        `docker build -t redpic .`
+        
+        To launch the application, use the command:
+        
+        `docker run -it redpic`
+        
+        ### Documentation
+        
+        The documentation contains all the Latex files needed to generate documentation. 
+        The main source files are located in the `docs/src`.
+        
+        * [main.tex](/docs/src/main.tex) is documentation source file. 
+        The final PDF can be found [here](/docs/out/main.pdf).
+        
+        [main.tex](/docs/src/main.tex) is the source file that Latex compiler will use to generate the paper. 
+        However, in order to keep the code cleaner, the main sections of the paper are all located in the [sections](/docs/src/sections). 
+        In this way you will experience less merging issues when two or more people are working on the same doc.
+        
+        Just edit the text in the relative Latex file (e.g., introduction, methodology, etc.) and you should be ready to go. 
+        No need to change any other file.
+        
+        #### Adding a new section
+        
+        Just copy a section file (e.g., [introduction.tex](/docs/src/sections/introduction.tex)) paste it in the same directory. 
+        Rename the pasted file (e.g. first_chapter.tex) and add this file to [main.tex](/docs/src/main.tex).
+        
+        ### Additional Resources
+        
+        Alternatively you can find great resources on the 
+        [Overleaf Tutorial website](https://www.overleaf.com/learn/latex/Tutorials) or on 
+        [Latex wikibooks](https://en.wikibooks.org/wiki/LaTeX).
+        
+        ## Prerequisites
+        
+        #### Latex
+        
+        Latex IDE and compiler installed locally on your machine. 
+        We recommend using a PyCharm plugin called [TeXiFy IDEA](https://plugins.jetbrains.com/plugin/9473-texify-idea) as IDE and 
+        [miktex](https://miktex.org) as Latex compiler  
+        
+        Alternatively you can push your code to Overleaf using git and only use Overleaf. 
+        We would discourage you from doing this! Overleaf should only be used for the review.
+        
+        ## Useful Resources
+        
+        ### IDE
+        
+        You may want to take advantage of the power of IDEs. 
+        For Python We would recommend using [PyCharm](https://www.jetbrains.com/pycharm/). 
+        
+        Alternatives are:
+        
+        * [Visual Studio](https://code.visualstudio.com)
+        * [Atom](https://atom.io/)
+        
+        ### Git
+        
+        You should install [git](https://git-scm.com) on your computer. And have [GitHub](https://github.com) account.
+        
+        ## Authors
+        
+        * **[Vyacheslav Fedorov](https://github.com/fuodorov)** - *Initial work*
+        * **[Danila Nikiforov](https://github.com/Danila-Nikiforov)** - *Initial work*
+        
+        See also the list of [contributors](https://github.com/binp-dev/redpic/contributors) who participated in this project.
+        
+        ## License
+        
+        This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+        
+        ## Contributing
+        
+        ### Dependencies
+        Use `make deps` command to install library, its production and development dependencies.
+        
+        ### Formatting
+        Use `make format` to autoformat code with black tool. 
+        
+        ### Tests
+        Use `make lint` to run only linters for current python version
+        
+        ### Maintaining
+        If pull request consists of several meaningful commits, that should be preserved, 
+        then use "Rebase and merge" option. Otherwise use "Squash and merge". 
+        
+        New release (changelog, tag and pypi upload) will be automatically created 
+        on each push to master via Github Actions workflow.
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
```

### Comparing `redpic-1.0.0.1/redpic/beam.py` & `redpic-1.0.0.2/redpic/beam.py`

 * *Files identical despite different names*

### Comparing `redpic-1.0.0.1/redpic/constants.py` & `redpic-1.0.0.2/redpic/constants.py`

 * *Files identical despite different names*

### Comparing `redpic-1.0.0.1/redpic/solver.py` & `redpic-1.0.0.2/redpic/solver.py`

 * *Files identical despite different names*

### Comparing `redpic-1.0.0.1/redpic.egg-info/PKG-INFO` & `redpic-1.0.0.2/redpic.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,138 @@
 Metadata-Version: 2.1
 Name: redpic
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: Relativictic Difference Scheme Particle-in-Cell code (REDPIC)
 Home-page: https://github.com/fuodorov/redpic
 Author: Vyacheslav Fedorov
 Author-email: slava@fuodorov.ru
+License: UNKNOWN
+Description: # Relativistic Difference Scheme Particles-In-Cell (REDPIC)
+        [![PyPI version](https://badge.fury.io/py/redpic.svg)](https://badge.fury.io/py/redpic)
+        
+        This PIC code has been developed since 2020 at the Budker Institute of Nuclear Physics as an alternative to 
+        [ASTRA](https://www.desy.de/~mpyflo/), 
+        [WARP](https://bitbucket.org/berkeleylab/warp/), 
+        [XTRACK](https://xsuite.readthedocs.io/en/latest/) 
+        and other codes. 
+        
+        For particle dynamics simulation using finite difference scheme relativistic.
+        
+        ## Table of content 
+        
+        -   [Getting Started](#getting-started)
+            -   [Local build and launch](#local-build-and-launch)
+            -   [Documentation](#documentation)
+                -   [Adding a new section](#adding-a-new-section)
+            -   [Additional resources](#additional-resources)
+        -   [Prerequisites](#prerequisites)
+            -   [Latex](#latex)
+        -   [Useful Resources](#useful-resources)
+            -   [IDE](#ide)
+        -   [Authors](#authors)
+        -   [Licence](#license)
+        -   [Contributing](#contributing)
+            -   [Dependencies](#dependencies)
+            -   [Formatting](#formatting)
+            -   [Tests](#tests)
+            -   [Maintaining](#maintaining)
+        
+        ## Getting Started
+        
+        ### Local build and launch
+        
+        To build our application and create a Docker image, it will be enough to run the following command:
+        
+        `docker build -t redpic .`
+        
+        To launch the application, use the command:
+        
+        `docker run -it redpic`
+        
+        ### Documentation
+        
+        The documentation contains all the Latex files needed to generate documentation. 
+        The main source files are located in the `docs/src`.
+        
+        * [main.tex](/docs/src/main.tex) is documentation source file. 
+        The final PDF can be found [here](/docs/out/main.pdf).
+        
+        [main.tex](/docs/src/main.tex) is the source file that Latex compiler will use to generate the paper. 
+        However, in order to keep the code cleaner, the main sections of the paper are all located in the [sections](/docs/src/sections). 
+        In this way you will experience less merging issues when two or more people are working on the same doc.
+        
+        Just edit the text in the relative Latex file (e.g., introduction, methodology, etc.) and you should be ready to go. 
+        No need to change any other file.
+        
+        #### Adding a new section
+        
+        Just copy a section file (e.g., [introduction.tex](/docs/src/sections/introduction.tex)) paste it in the same directory. 
+        Rename the pasted file (e.g. first_chapter.tex) and add this file to [main.tex](/docs/src/main.tex).
+        
+        ### Additional Resources
+        
+        Alternatively you can find great resources on the 
+        [Overleaf Tutorial website](https://www.overleaf.com/learn/latex/Tutorials) or on 
+        [Latex wikibooks](https://en.wikibooks.org/wiki/LaTeX).
+        
+        ## Prerequisites
+        
+        #### Latex
+        
+        Latex IDE and compiler installed locally on your machine. 
+        We recommend using a PyCharm plugin called [TeXiFy IDEA](https://plugins.jetbrains.com/plugin/9473-texify-idea) as IDE and 
+        [miktex](https://miktex.org) as Latex compiler  
+        
+        Alternatively you can push your code to Overleaf using git and only use Overleaf. 
+        We would discourage you from doing this! Overleaf should only be used for the review.
+        
+        ## Useful Resources
+        
+        ### IDE
+        
+        You may want to take advantage of the power of IDEs. 
+        For Python We would recommend using [PyCharm](https://www.jetbrains.com/pycharm/). 
+        
+        Alternatives are:
+        
+        * [Visual Studio](https://code.visualstudio.com)
+        * [Atom](https://atom.io/)
+        
+        ### Git
+        
+        You should install [git](https://git-scm.com) on your computer. And have [GitHub](https://github.com) account.
+        
+        ## Authors
+        
+        * **[Vyacheslav Fedorov](https://github.com/fuodorov)** - *Initial work*
+        * **[Danila Nikiforov](https://github.com/Danila-Nikiforov)** - *Initial work*
+        
+        See also the list of [contributors](https://github.com/binp-dev/redpic/contributors) who participated in this project.
+        
+        ## License
+        
+        This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+        
+        ## Contributing
+        
+        ### Dependencies
+        Use `make deps` command to install library, its production and development dependencies.
+        
+        ### Formatting
+        Use `make format` to autoformat code with black tool. 
+        
+        ### Tests
+        Use `make lint` to run only linters for current python version
+        
+        ### Maintaining
+        If pull request consists of several meaningful commits, that should be preserved, 
+        then use "Rebase and merge" option. Otherwise use "Squash and merge". 
+        
+        New release (changelog, tag and pypi upload) will be automatically created 
+        on each push to master via Github Actions workflow.
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Relativistic Difference Scheme Particles-In-Cell (REDPIC)
-[![PyPI version](https://badge.fury.io/py/redpic.svg)](https://badge.fury.io/py/redpic)
-
-This PIC code has been developed since 2020 at the Budker Institute of Nuclear Physics as an alternative to 
-[ASTRA](https://www.desy.de/~mpyflo/), 
-[WARP](https://bitbucket.org/berkeleylab/warp/), 
-[XTRACK](https://xsuite.readthedocs.io/en/latest/) 
-and other codes. 
-
-For particle dynamics simulation using finite difference scheme relativistic.
-
-## Table of content 
-
--   [Getting Started](#getting-started)
-    -   [Local build and launch](#local-build-and-launch)
-    -   [Documentation](#documentation)
-        -   [Adding a new section](#adding-a-new-section)
-    -   [Additional resources](#additional-resources)
--   [Prerequisites](#prerequisites)
-    -   [Latex](#latex)
--   [Useful Resources](#useful-resources)
-    -   [IDE](#ide)
--   [Authors](#authors)
--   [Licence](#license)
--   [Contributing](#contributing)
-    -   [Dependencies](#dependencies)
-    -   [Formatting](#formatting)
-    -   [Tests](#tests)
-    -   [Maintaining](#maintaining)
-
-## Getting Started
-
-### Local build and launch
-
-To build our application and create a Docker image, it will be enough to run the following command:
-
-`docker build -t redpic .`
-
-To launch the application, use the command:
-
-`docker run -it redpic`
-
-### Documentation
-
-The documentation contains all the Latex files needed to generate documentation. 
-The main source files are located in the `docs/src`.
-
-* [main.tex](/docs/src/main.tex) is documentation source file. 
-The final PDF can be found [here](/docs/out/main.pdf).
-
-[main.tex](/docs/src/main.tex) is the source file that Latex compiler will use to generate the paper. 
-However, in order to keep the code cleaner, the main sections of the paper are all located in the [sections](/docs/src/sections). 
-In this way you will experience less merging issues when two or more people are working on the same doc.
-
-Just edit the text in the relative Latex file (e.g., introduction, methodology, etc.) and you should be ready to go. 
-No need to change any other file.
-
-#### Adding a new section
-
-Just copy a section file (e.g., [introduction.tex](/docs/src/sections/introduction.tex)) paste it in the same directory. 
-Rename the pasted file (e.g. first_chapter.tex) and add this file to [main.tex](/docs/src/main.tex).
-
-### Additional Resources
-
-Alternatively you can find great resources on the 
-[Overleaf Tutorial website](https://www.overleaf.com/learn/latex/Tutorials) or on 
-[Latex wikibooks](https://en.wikibooks.org/wiki/LaTeX).
-
-## Prerequisites
-
-#### Latex
-
-Latex IDE and compiler installed locally on your machine. 
-We recommend using a PyCharm plugin called [TeXiFy IDEA](https://plugins.jetbrains.com/plugin/9473-texify-idea) as IDE and 
-[miktex](https://miktex.org) as Latex compiler  
-
-Alternatively you can push your code to Overleaf using git and only use Overleaf. 
-We would discourage you from doing this! Overleaf should only be used for the review.
-
-## Useful Resources
-
-### IDE
-
-You may want to take advantage of the power of IDEs. 
-For Python We would recommend using [PyCharm](https://www.jetbrains.com/pycharm/). 
-
-Alternatives are:
-
-* [Visual Studio](https://code.visualstudio.com)
-* [Atom](https://atom.io/)
-
-### Git
-
-You should install [git](https://git-scm.com) on your computer. And have [GitHub](https://github.com) account.
-
-## Authors
-
-* **[Vyacheslav Fedorov](https://github.com/fuodorov)** - *Initial work*
-* **[Danila Nikiforov](https://github.com/Danila-Nikiforov)** - *Initial work*
-
-See also the list of [contributors](https://github.com/binp-dev/redpic/contributors) who participated in this project.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-## Contributing
-
-### Dependencies
-Use `make deps` command to install library, its production and development dependencies.
-
-### Formatting
-Use `make format` to autoformat code with black tool. 
-
-### Tests
-Use `make lint` to run only linters for current python version
-
-### Maintaining
-If pull request consists of several meaningful commits, that should be preserved, 
-then use "Rebase and merge" option. Otherwise use "Squash and merge". 
-
-New release (changelog, tag and pypi upload) will be automatically created 
-on each push to master via Github Actions workflow.
```

### Comparing `redpic-1.0.0.1/setup.py` & `redpic-1.0.0.2/setup.py`

 * *Files identical despite different names*

