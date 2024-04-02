# Comparing `tmp/os2024-0.4.0.tar.gz` & `tmp/os2024-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2024-0.4.0.tar", max compression
+gzip compressed data, was "os2024-0.5.0.tar", max compression
```

## Comparing `os2024-0.4.0.tar` & `os2024-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
--rw-r--r--   0        0        0    18656 2024-03-26 19:30:43.604751 os2024-0.4.0/LICENSE
--rw-r--r--   0        0        0     3892 2024-03-26 19:30:43.604751 os2024-0.4.0/README.md
--rw-r--r--   0        0        0     3573 2024-03-26 19:31:02.577043 os2024-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2311 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/__cli__.py
--rw-r--r--   0        0        0      338 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/__init__.py
--rw-r--r--   0        0        0       22 2024-03-26 19:31:02.537043 os2024-0.4.0/src/os2024/_version.py
--rw-r--r--   0        0        0     3968 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/_config.yml
--rw-r--r--   0        0        0     1792 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/_toc.yml
--rw-r--r--   0        0        0    22523 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/about/images/yjlee.jpeg
--rw-r--r--   0        0        0     1476 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/about/index.md
--rw-r--r--   0        0        0        0 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/assets/assets/extra/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/assets/extra/.gitkeep
--rw-r--r--   0        0        0     3949 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/index.md
--rw-r--r--   0        0        0     7547 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/references/ostep/index.md
--rw-r--r--   0        0        0     1967 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/references/ostep-code/index.md
--rw-r--r--   0        0        0    11719 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/references/ostep-homework/index.md
--rw-r--r--   0        0        0     3977 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/references/ostep-projects/index.md
--rw-r--r--   0        0        0        9 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/references.bib
--rw-r--r--   0        0        0      205 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/requirements.txt
--rw-r--r--   0        0        0     6229 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/syllabus/index.md
--rw-r--r--   0        0        0     2770 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week01/index.md
--rw-r--r--   0        0        0    26095 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week01/intro.md
--rw-r--r--   0        0        0     9466 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/cpu-api.md
--rw-r--r--   0        0        0    16683 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/cpu-intro.md
--rw-r--r--   0        0        0    20945 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/cpu-mechanisms.md
--rw-r--r--   0        0        0     2830 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/index.md
--rw-r--r--   0        0        0     4976 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/lab.md
--rw-r--r--   0        0        0     4284 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/shells.md
--rw-r--r--   0        0        0     2795 2024-03-26 19:30:43.608751 os2024-0.4.0/src/os2024/book/week02/tip.md
--rw-r--r--   0        0        0    19638 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week03/cpu-scheduling.md
--rw-r--r--   0        0        0    49905 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week03/figs/fcfs.png
--rw-r--r--   0        0        0       53 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week03/index.md
--rw-r--r--   0        0        0    15505 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week03/lab.md
--rw-r--r--   0        0        0     3518 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week03/wsl-setup.md
--rw-r--r--   0        0        0     3501 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week04/index.md
--rw-r--r--   0        0        0     6608 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week04/lab-lottery.md
--rw-r--r--   0        0        0     3127 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week04/lab-sched.md
--rw-r--r--   0        0        0    10353 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week04/lottery.md
--rw-r--r--   0        0        0    28602 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week04/mlfq.md
--rw-r--r--   0        0        0   202834 2024-03-26 19:30:43.612751 os2024-0.4.0/src/os2024/book/week05/figs/os_img_1.png
--rw-r--r--   0        0        0   475305 2024-03-26 19:30:43.616751 os2024-0.4.0/src/os2024/book/week05/figs/os_img_2.png
--rw-r--r--   0        0        0    87376 2024-03-26 19:30:43.616751 os2024-0.4.0/src/os2024/book/week05/figs/os_img_3.png
--rw-r--r--   0        0        0     3581 2024-03-26 19:30:43.616751 os2024-0.4.0/src/os2024/book/week05/index.md
--rw-r--r--   0        0        0    10505 2024-03-26 19:30:43.616751 os2024-0.4.0/src/os2024/book/week05/vm-intro.md
--rw-r--r--   0        0        0      172 2024-03-26 19:30:43.616751 os2024-0.4.0/src/os2024/conf/about/os2024.yaml
--rw-r--r--   0        0        0        0 2024-03-26 19:30:43.616751 os2024-0.4.0/src/os2024/py.typed
--rw-r--r--   0        0        0     5191 1970-01-01 00:00:00.000000 os2024-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    18656 2024-04-02 21:03:49.262368 os2024-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3892 2024-04-02 21:03:49.262368 os2024-0.5.0/README.md
+-rw-r--r--   0        0        0     3573 2024-04-02 21:04:07.682755 os2024-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2311 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/__cli__.py
+-rw-r--r--   0        0        0      338 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-02 21:04:07.642754 os2024-0.5.0/src/os2024/_version.py
+-rw-r--r--   0        0        0     3806 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/_config.yml
+-rw-r--r--   0        0        0     1930 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/_toc.yml
+-rw-r--r--   0        0        0    22523 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/about/images/yjlee.jpeg
+-rw-r--r--   0        0        0     1476 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/about/index.md
+-rw-r--r--   0        0        0        0 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/assets/assets/extra/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/assets/extra/.gitkeep
+-rw-r--r--   0        0        0     3949 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/index.md
+-rw-r--r--   0        0        0     7547 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep/index.md
+-rw-r--r--   0        0        0     1967 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep-code/index.md
+-rw-r--r--   0        0        0    11719 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep-homework/index.md
+-rw-r--r--   0        0        0     3977 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references/ostep-projects/index.md
+-rw-r--r--   0        0        0        9 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/references.bib
+-rw-r--r--   0        0        0      205 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/requirements.txt
+-rw-r--r--   0        0        0     6229 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/syllabus/index.md
+-rw-r--r--   0        0        0     2770 2024-04-02 21:03:49.262368 os2024-0.5.0/src/os2024/book/week01/index.md
+-rw-r--r--   0        0        0    26071 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week01/intro.md
+-rw-r--r--   0        0        0     9466 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/cpu-api.md
+-rw-r--r--   0        0        0    16683 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/cpu-intro.md
+-rw-r--r--   0        0        0    20945 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/cpu-mechanisms.md
+-rw-r--r--   0        0        0     2830 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/index.md
+-rw-r--r--   0        0        0     4976 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/lab.md
+-rw-r--r--   0        0        0     4284 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/shells.md
+-rw-r--r--   0        0        0     2795 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week02/tip.md
+-rw-r--r--   0        0        0    19638 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/cpu-scheduling.md
+-rw-r--r--   0        0        0    49905 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/figs/fcfs.png
+-rw-r--r--   0        0        0       53 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/index.md
+-rw-r--r--   0        0        0    15505 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/lab.md
+-rw-r--r--   0        0        0     3518 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week03/wsl-setup.md
+-rw-r--r--   0        0        0     3501 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/index.md
+-rw-r--r--   0        0        0     6608 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/lab-lottery.md
+-rw-r--r--   0        0        0     9209 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/lab-sched.md
+-rw-r--r--   0        0        0    24596 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/lottery.md
+-rw-r--r--   0        0        0    28602 2024-04-02 21:03:49.266368 os2024-0.5.0/src/os2024/book/week04/mlfq.md
+-rw-r--r--   0        0        0   202834 2024-04-02 21:03:49.270368 os2024-0.5.0/src/os2024/book/week05/figs/os_img_1.png
+-rw-r--r--   0        0        0   475305 2024-04-02 21:03:49.270368 os2024-0.5.0/src/os2024/book/week05/figs/os_img_2.png
+-rw-r--r--   0        0        0    87376 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/figs/os_img_3.png
+-rw-r--r--   0        0        0     3581 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/index.md
+-rw-r--r--   0        0        0     3753 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/lab.md
+-rw-r--r--   0        0        0     5279 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/tip-linux-cmd.md
+-rw-r--r--   0        0        0    13121 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/vm-api.md
+-rw-r--r--   0        0        0    15887 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/vm-intro.md
+-rw-r--r--   0        0        0    12644 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/book/week05/vm-mechanism.md
+-rw-r--r--   0        0        0      172 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/conf/about/os2024.yaml
+-rw-r--r--   0        0        0        0 2024-04-02 21:03:49.274368 os2024-0.5.0/src/os2024/py.typed
+-rw-r--r--   0        0        0     5191 1970-01-01 00:00:00.000000 os2024-0.5.0/PKG-INFO
```

### Comparing `os2024-0.4.0/LICENSE` & `os2024-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/README.md` & `os2024-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/pyproject.toml` & `os2024-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "os2024"
-version = "0.4.0"
+version = "0.5.0"
 description = "Operating Systems 2024 Class"
 authors = ["Young Joon Lee <yj.lee@chu.ac.kr>"]
 license = "CC-BY-4.0"
 homepage = "https://os2024.halla.ai"
 repository = "https://github.com/chu-aie/os-2024"
 readme = "README.md"
 packages = [{ include = "os2024", from = "src" }]
```

### Comparing `os2024-0.4.0/src/os2024/__cli__.py` & `os2024-0.5.0/src/os2024/__cli__.py`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/_config.yml` & `os2024-0.5.0/src/os2024/book/_config.yml`

 * *Files 10% similar despite different names*

```diff
@@ -47,16 +47,15 @@
       data-base-api-url="https://chat.entelecheia.app/api/embed"
       data-brand-image-url="https://assets.entelecheia.ai/favicon.png"
       data-chat-icon="magic"
       data-sponsor-text="OS 2024"
       data-sponsor-link="https://chat.entelecheia.app/workspace/os2024"
       src="https://chat.entelecheia.app/embed/anythingllm-chat-widget.min.js">
     </script>
-  announcement: |
-    4주차는 3주차에 다루지 못한 내용을 다룹니다. 따라서, 신규 내용은 없습니다. 기존 내용을 보강하는 것이 과제입니다.
+  announcement: ""
 
 sphinx:
   config:
     html_extra_path: ["assets"]
     bibtex_reference_style: author_year
     mathjax_path: https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
     intersphinx_mapping:
```

#### html2text {}

```diff
@@ -16,17 +16,15 @@
 your book, relative to the repository root branch: main # Which branch of the
 repository should be used when creating links (optional) # Add GitHub buttons
 to your book # See https://jupyterbook.org/customize/config.html#add-a-link-to-
 your-repository html: use_issues_button: true use_repository_button: true
 use_edit_page_button: true favicon: https://assets.entelecheia.ai/favicon.png #
 favicon: Path to the favicon image google_analytics_id: G-BQJE5V9RK2 #
 google_analytics_id: Google Analytics ID extra_footer: |
-announcement: | 4ì£¼ì°¨ë 3ì£¼ì°¨ì ë¤ë£¨ì§ ëª»í ë´ì©ì ë¤ë£¹ëë¤.
-ë°ë¼ì, ì ê· ë´ì©ì ììµëë¤. ê¸°ì¡´ ë´ì©ì ë³´ê°íë ê²ì´
-ê³¼ì ìëë¤. sphinx: config: html_extra_path: ["assets"]
+announcement: "" sphinx: config: html_extra_path: ["assets"]
 bibtex_reference_style: author_year mathjax_path: https://cdn.jsdelivr.net/npm/
 mathjax@3/es5/tex-mml-chtml.js intersphinx_mapping: ebp: - "https://
 executablebooks.org/en/latest/" - null myst-parser: - "https://myst-
 parser.readthedocs.io/en/latest/" - null myst-nb: - "https://myst-
 nb.readthedocs.io/en/latest/" - null sphinx: - "https://www.sphinx-doc.org/en/
 master" - null nbformat: - "https://nbformat.readthedocs.io/en/latest" - null
 sd: - "https://sphinx-design.readthedocs.io/en/latest" - null sphinxproof: -
```

### Comparing `os2024-0.4.0/src/os2024/book/_toc.yml` & `os2024-0.5.0/src/os2024/book/_toc.yml`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,18 @@
           - file: week04/mlfq
           - file: week04/lottery
           - file: week04/lab-sched
           - file: week04/lab-lottery
       - file: week05/index
         sections:
           - file: week05/vm-intro
+          - file: week05/vm-api
+          - file: week05/vm-mechanism
+          - file: week05/lab
+          - file: week05/tip-linux-cmd
   - caption: References
     chapters:
       - file: references/ostep/index
       - file: references/ostep-code/index
       - file: references/ostep-homework/index
       - file: references/ostep-projects/index
       - url: https://kuleuven-diepenbeek.github.io/osc-course/
```

### Comparing `os2024-0.4.0/src/os2024/book/about/images/yjlee.jpeg` & `os2024-0.5.0/src/os2024/book/about/images/yjlee.jpeg`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/about/index.md` & `os2024-0.5.0/src/os2024/book/about/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/index.md` & `os2024-0.5.0/src/os2024/book/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/references/ostep/index.md` & `os2024-0.5.0/src/os2024/book/references/ostep/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/references/ostep-code/index.md` & `os2024-0.5.0/src/os2024/book/references/ostep-code/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/references/ostep-homework/index.md` & `os2024-0.5.0/src/os2024/book/references/ostep-homework/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/references/ostep-projects/index.md` & `os2024-0.5.0/src/os2024/book/references/ostep-projects/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/syllabus/index.md` & `os2024-0.5.0/src/os2024/book/syllabus/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week01/index.md` & `os2024-0.5.0/src/os2024/book/week01/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week01/intro.md` & `os2024-0.5.0/src/os2024/book/week01/intro.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 간단한 코드 예제는 다음과 같습니다:
 
 ```c
 #include <stdio.h>
 #include <stdlib.h>
 #include <sys/time.h>
 #include <assert.h>
-#include “common.h”
+#include "common.h"
 
 int main(int argc, char *argv[]) {
     if (argc != 2) {
-        fprintf(stderr, “사용법: cpu <문자열>\n”);
+        fprintf(stderr, "사용법: cpu <문자열>\n");
         exit(1);
     }
     char *str = argv[1];
     while (1) {
         Spin(1);
-        printf(“%s\n”, str);
+        printf("%s\n", str);
     }
     return 0;
 }
 ```
 
 이 코드는 사용자가 입력한 문자열을 1초마다 계속 출력합니다. 결과는 복잡하지 않지만, 프로그램이 어떻게 끊임없이 실행되는지 보여줍니다. 프로그램을 종료하려면 `Control-c`를 누르면 됩니다.
 
@@ -45,25 +45,25 @@
 
 아래는 메모리 접근과 관련된 프로그램의 예입니다. 이 프로그램은 메모리에 정수를 저장하고, 1초마다 그 값을 1씩 증가시킨 후 출력합니다. 각 프로그램은 고유한 메모리 주소를 가지며, 실행될 때마다 해당 주소에 있는 값이 어떻게 변하는지 보여줍니다.
 
 ```c
 #include <unistd.h>
 #include <stdio.h>
 #include <stdlib.h>
-#include “common.h”
+#include "common.h"
 
 int main(int argc, char *argv[]) {
     int *p = malloc(sizeof(int)); // 정수형 포인터 p에 메모리 할당
     assert(p != NULL); // p가 NULL이 아닌지 확인
-    printf(“(%d) p의 메모리 주소: %08x\n”, getpid(), (unsigned) p); // 프로세스 ID와 p의 메모리 주소 출력
+    printf("(%d) p의 메모리 주소: %08x\n", getpid(), (unsigned) p); // 프로세스 ID와 p의 메모리 주소 출력
     *p = 0; // p가 가리키는 값을 0으로 초기화
     while (1) {
         Spin(1); // 1초 대기
         *p = *p + 1; // p가 가리키는 값을 1 증가
-        printf(“(%d) p: %d\n”, getpid(), *p); // 프로세스 ID와 p가 가리키는 값 출력
+        printf("(%d) p: %d\n", getpid(), *p); // 프로세스 ID와 p가 가리키는 값 출력
     }
     return 0;
 }
 ```
 
 이 코드는 프로그램이 메모리를 어떻게 사용하는지와 프로세스마다 고유한 메모리 주소 공간을 가지고 있음을 보여줍니다.
```

### Comparing `os2024-0.4.0/src/os2024/book/week02/cpu-api.md` & `os2024-0.5.0/src/os2024/book/week02/cpu-api.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week02/cpu-intro.md` & `os2024-0.5.0/src/os2024/book/week02/cpu-intro.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week02/cpu-mechanisms.md` & `os2024-0.5.0/src/os2024/book/week02/cpu-mechanisms.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week02/index.md` & `os2024-0.5.0/src/os2024/book/week02/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week02/lab.md` & `os2024-0.5.0/src/os2024/book/week02/lab.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week02/shells.md` & `os2024-0.5.0/src/os2024/book/week02/shells.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week02/tip.md` & `os2024-0.5.0/src/os2024/book/week02/tip.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week03/cpu-scheduling.md` & `os2024-0.5.0/src/os2024/book/week03/cpu-scheduling.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week03/figs/fcfs.png` & `os2024-0.5.0/src/os2024/book/week03/figs/fcfs.png`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week03/lab.md` & `os2024-0.5.0/src/os2024/book/week03/lab.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week03/wsl-setup.md` & `os2024-0.5.0/src/os2024/book/week03/wsl-setup.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week04/index.md` & `os2024-0.5.0/src/os2024/book/week04/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week04/lab-lottery.md` & `os2024-0.5.0/src/os2024/book/week04/lab-lottery.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week04/mlfq.md` & `os2024-0.5.0/src/os2024/book/week04/mlfq.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week05/figs/os_img_1.png` & `os2024-0.5.0/src/os2024/book/week05/figs/os_img_1.png`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week05/figs/os_img_2.png` & `os2024-0.5.0/src/os2024/book/week05/figs/os_img_2.png`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week05/figs/os_img_3.png` & `os2024-0.5.0/src/os2024/book/week05/figs/os_img_3.png`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week05/index.md` & `os2024-0.5.0/src/os2024/book/week05/index.md`

 * *Files identical despite different names*

### Comparing `os2024-0.4.0/src/os2024/book/week05/vm-intro.md` & `os2024-0.5.0/src/os2024/book/week05/vm-intro.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,171 +5,181 @@
 ## 초기 시스템
 
 ```{image} ./figs/os_img_1.png
 :width: 40%
 :align: center
 ```
 
-운영체제는 메모리에(그림에서는 물리주소 0부터) 상주하는 루틴(라이브러리)의 집합이였습니다. 물리 메모리에 하나의 실행 중인 프로그램(프로세스)이 존재하였고(그림에서는 물리 주소 64KB부터 시작하여) 나머지 메모리를 사용했습니다.
+메모리 관점에서 볼 때, 초기 컴퓨터 시스템의 운영체제는 사용자에게 그다지 많은 기능을 제공하지 않았습니다. 당시의 운영체제는 주로 메모리에 상주하는 루틴이나 라이브러리의 모음이었죠. 그림에서 볼 수 있듯이 운영체제는 물리 주소 0번지부터 메모리에 위치했습니다.
 
-```{admonition} 물리 주소
-물리 주소는 메모리 입장에서 바라본 주소, 말 그대로 정보가 실제로 저장된 하드웨어상의 주소를 의미합니다. 논리 주소는 CPU와 실행중인 프로그램 입장에서 바라본 주소로 실행 중인 프로그램 각각에게 부여된 0번지부터 시작하는 주소를 의미합니다.
+물리 메모리의 구성은 대략 그림과 같았습니다. 하나의 프로세스(실행 중인 프로그램)가 물리 메모리의 특정 영역을 독점적으로 사용하고, 나머지 공간은 다른 용도로 활용되었습니다. 예를 들면 그림에서는 64KB 주소부터 이런 방식으로 메모리가 할당된 것을 볼 수 있습니다.
+
+```{admonition} 주소 체계
+컴퓨터 시스템에서는 두 가지 주소 체계가 사용됩니다.
+
+- 논리 주소(Logical Address): 프로그램이 직접 다루는 주소로, 각 프로세스는 자신만의 독립된 논리 주소 공간을 가집니다. 보통 0번지부터 시작하죠.
+
+- 물리 주소(Physical Address): 실제 메모리 하드웨어의 주소입니다. 논리 주소는 물리 주소로 변환되어 메모리에 실제로 저장됩니다.
 ```
 
+초기 시스템에서는 특별한 가상화 기술이 거의 없었고, 사용자 역시 운영체제에 큰 기대를 하지 않았습니다.
+
+그 시절 운영체제 개발자들의 삶은 비교적 단순했다고 볼 수 있습니다. 지금처럼 복잡한 운영체제가 아니라 간단한 기능만 제공하면 되었고, 사용자와의 상호작용도 제한적이었거든요. 그런 환경에서 운영체제를 개발하고 관리하는 일은 오늘날에 비하면 상당히 쉬웠을 것입니다.
+
 ## 멀티프로그래밍과 시분할
 
-- CPU는 실제로 1개인데, 여러 개의 프로세스들은 마치 CPU가 여러개인 것과 같은 환상을 가집니다.
-- 그런 환상을 통해, 여러 프로세스가 동시에 실행되는 것 처럼 보이게 합니다.
+- CPU는 실제로는 하나지만, 여러 프로세스가 마치 자신만의 CPU를 가진 것처럼 느끼게 하는 것이 목표입니다.
+
+- 이를 통해 다수의 프로세스가 동시에 실행되는 것 같은 환상을 만들어냅니다.
+
+컴퓨터 가격이 비쌌던 시절, 한 대의 컴퓨터를 여러 사람이 함께 쓰는 것은 흔한 일이었습니다. 이는 컴퓨터 자원을 보다 효율적으로 사용하기 위한 방편이었고, 멀티프로그래밍의 등장으로 이어졌죠. 이때는 다수의 프로세스가 CPU를 할당받기를 기다리고, 운영체제가 이들을 번갈아 실행시켜 CPU를 최대한 활용하는 방식이 쓰였습니다.
 
-이러한 시분할을 구현하는 방법 중 하나는 하나의 프로세스를 짧은 시간동안 실행시키는데, 해당 기간동안 프로세스에게 모든 메모리를 접근할 권한을 주는 것이였습니다.
+그럼에도 컴퓨터 가격은 여전히 높았기에, 더 많은 사람이 동시에 사용할 수 있게 하고 자원 활용도를 극대화할 방법이 모색되었습니다. 그 결과 시분할 시스템이 개발되었죠. 이는 여러 사용자가 컴퓨터를 동시에 쓸 수 있게 함으로써, 기존의 일괄 처리 방식에 비해 결과를 더 빨리 받아볼 수 있게 했습니다. 프로그래머들 역시 자신의 프로그램을 즉시 실행해보고 수정할 수 있게 되었고요. 이런 요구에 부응해 대화형 사용 방식이 중요해졌습니다.
 
-그 후에, 이 프로세스를 중단하고 중단 시점의 모든 상태를 디스크 종류의 장치에 저장하고 다른 프로세스의 상태를 탑재하여 짧은 시간동안 실행시키는 것이였습니다.
+시분할을 구현하는 한 가지 방법은 프로세스를 아주 짧은 시간 동안만 실행시키되, 그 순간에는 메모리 전체에 대한 접근 권한을 부여하는 것이었습니다. 그 후 프로세스를 중단하고 그때의 모든 상태를 디스크 같은 곳에 저장한 뒤, 다른 프로세스의 정보를 불러와 또 잠깐 실행하는 식이었죠.
 
-이 방법에는 큰 문제가 있었는데, 레지스터 상태를 저장하고 복원하는 것은 빠르지만 메모리 내용 전체를 디스크에 저장하는 것이 느렸다는 것이였습니다.
+그러나 이 방식에는 큰 문제가 있었습니다. 레지스터 값을 저장하고 복원하는 건 빨랐지만, 메모리 전체를 디스크에 옮기는 건 너무 느렸던 거죠.
 
-→ 이것을 해결하기위해, 프로세스를 전환할 때 프로세스를 메모리에 그대로 유지하면서 OS가 시분할을 효율적으로 구현할 수 있게 하는 것이 메모리 가상화의 목표입니다.
+바로 이 문제를 해결하기 위해, 프로세스를 전환할 때도 메모리에 그대로 둔 채로 시분할을 구현하는 게 메모리 가상화의 주된 목표가 되었습니다.
 
 ```{image} ./figs/os_img_2.png
 :width: 40%
 :align: center
 ```
 
-그림에 세 개의 프로세스 A,B,C가 있습니다.
+그림을 보면 프로세스 A, B, C 세 개가 있습니다. 512KB짜리 물리 메모리에서 각자의 영역을 할당받은 것이죠. A는 현재 실행 중이고, B와 C는 실행 대기 중입니다. 중요한 건 프로세스들이 메모리를 공유하지 않고 각자의 공간을 가진다는 점입니다. 이는 프로세스 간 메모리 침범을 방지하기 위함입니다.
 
-각 프로세는 512KB의 물리 메모리에서 각자 작은 부분을 할당 받았고, A는 실행 중이며 B,C는 준비 큐에서 실행을 기다리고 있습니다.
-
-그런데, 이렇게 여러 프로세스들이 한 메모리에 존재하게 되면 서로 데이터를 침범할 수 있는 가능성이 존재합니다.
-
-그렇기에 보호 및 보안이 중요한 문제가 된 것입니다.
+시분할 시스템에서는 여러 프로세스가 동시에 돌아가므로, 이런 메모리 보호가 매우 중요합니다. 각 프로세스가 서로의 데이터나 코드를 함부로 건드리지 못하게 막아야 하는 거죠. 따라서 운영체제는 프로세스별로 할당된 메모리 영역을 엄격히 관리하고 지켜줘야 합니다. 그래야 시분할 시스템이 안전하고 안정적으로 작동할 수 있습니다.
 
 ## 주소 공간
 
-위와 같은 위험에 대비하기 위해 OS는 사용자에게 사용하기 쉬운 메모리 개념을 만들어야합니다.
+사용자가 의도치 않게 위험한 행동을 할 수 있다는 점을 고려하여, 운영체제는 메모리 개념을 사용하기 쉬운 형태로 제공해야 합니다. 바로 이 개념이 '주소 공간(address space)'입니다.
 
-이 개념이 주소 공간(address space)입니다.
+주소 공간은 실행 중인 프로그램이 메모리가 어떻게 구성되어 있다고 가정하는지를 나타냅니다. 운영체제의 메모리 가상화 방식을 이해하는 데 있어 핵심적인 개념이죠. 주소 공간은 프로그램이 사용하는 모든 메모리 영역을 포함하며, 운영체제는 이를 효율적이고 안전하게 관리할 책임이 있습니다. 따라서 주소 공간에 대한 이해는 운영체제가 메모리를 어떻게 다루는지 파악하는 데 있어 필수적입니다.
 
-주소 공간은 프로그램의 모든 메모리 상태를 갖고 있습니다.
-
-코드, 스택, 힙과 같이 프로그램을 실행시키기 위한 모든 상태를 주소공간이 가지고 있습니다.
+주소 공간에는 코드, 스택, 힙 등 프로그램을 실행하는 데 필요한 모든 상태 정보가 담겨 있습니다.
 
 ```{image} ./figs/os_img_3.png
 :width: 40%
 :align: center
 ```
 
-### Stack 영역:
+### 스택(Stack) 영역:
 
-- 함수의 호출과 관계되는 지역 변수와 매개변수가 저장되는 영역입니다.
-- Stack 영역의 값은 함수의 호출과 함께 할당되며, 함수의 호출이 완료되면 소멸합니다.
-- 메모리의 높은 주소에서 낮은 주소의 방향으로 할당됩니다.
-- 재귀 함수가 너무 깊게 호출되거나 함수가 지역변수를 너무 많이 가지고 있어 stack 영역을 초과하면 stack overflow 에러가 발생합니다.
+- 함수 호출과 관련된 지역 변수, 매개변수 등이 저장되는 공간입니다.
+- 함수가 호출될 때 할당되고, 함수가 종료되면 해제됩니다.
+- 메모리의 높은 주소에서 낮은 주소 방향으로 할당됩니다.
+- 재귀 호출이 너무 깊어지거나 지역 변수가 너무 많으면 스택 오버플로우 오류가 발생할 수 있습니다.
 
-### Heap 영역:
+### 힙(Heap) 영역:
 
-- 런타임에 크기가 결정되는 영역입니다.
-- 사용자에 의해 공간이 동적으로 할당 및 해제됩니다.
-- 주로 참조형 데이터 (ex. 클래스) 등의 데이터가 할당됩니다.
-- 메모리의 낮은 주소에서 높은 주소의 방향으로 할당됩니다.
+- 프로그램 실행 중에 크기가 결정되는 동적 메모리 영역입니다.
+- 사용자가 직접 공간을 할당하고 해제할 수 있습니다.
+- 주로 참조형 데이터(예: 객체)가 저장됩니다.
+- 메모리의 낮은 주소에서 높은 주소 방향으로 할당됩니다.
 
-### Data 영역:
+### 데이터(Data) 영역:
 
-- 전역 변수나 Static 변수 등 프로그램이 사용할 수 있는 데이터를 저장하는 영역입니다.
-- 어떤 프로그램에 전역/static 변수를 참조하는 코드가 존재한다면, 이 프로그램은 컴파일 된 후에 data 영역을 참조하게 됩니다.
-- 프로그램의 시작과 함께 할당되며, 프로그램이 종료되면 소멸합니다.
-- 단, 초기화 되지 않은 변수가 존재한다면, 이는 (그림에는 표현되지는 않았지만 BSS 영역에 저장됩니다.)
+- 전역 변수나 정적(static) 변수 등 프로그램에서 사용하는 데이터가 저장되는 영역입니다.
+- 전역/정적 변수를 참조하는 코드가 있다면, 컴파일 후 이 영역을 참조하게 됩니다.
+- 프로그램이 시작할 때 할당되고, 종료되면 해제됩니다.
+- 초기화되지 않은 변수는 그림에는 없지만 BSS 영역에 따로 저장됩니다.
 
-```{admonition} BSS 영역 (Block Started by Symbol)
-초기화되지 않은 전역 변수와 정적 변수를 저장하는 메모리 영역
-BSS 영역의 변수들은 프로그램 실행 시 0 또는 NULL 값으로 자동 초기화된다.
+```{admonition} BSS (Block Started by Symbol) 영역
+초기화되지 않은 전역 변수와 정적 변수가 저장되는 메모리 영역입니다. BSS 영역의 변수들은 프로그램 시작 시 자동으로 0이나 NULL로 초기화됩니다.
 ```
 
-### Text (Code) 영역:
+### 텍스트(Text) 또는 코드(Code) 영역:
 
-- 프로그램이 실행될 수 있도록 CPU가 해석 가능한 기계어 코드가 저장되어 있는 공간으로, 프로그램이 수정되면 안 되므로 ReadOnly 상태로 저장 되어있습니다.
+- CPU가 실행할 수 있는 기계어 코드가 저장된 영역입니다.
+- 프로그램 코드는 변경되면 안 되므로 읽기 전용(read-only)으로 보호됩니다.
 
-코드는 정적이기 때문에, 프로그램이 실행되면서 추가적으로 메모리를 필요로하지 않습니다.
+코드는 정적이므로 실행 중에 추가 메모리를 요구하지 않습니다. 따라서 메모리에 쉽게 적재할 수 있어 주로 주소 공간의 상단에 위치합니다.
 
-따라서 메모리에 저장하기 쉬우며, 상단에 배치하게됩니다.
+그 아래로는 프로그램 실행에 따라 크기가 변할 수 있는 힙과 스택이 자리잡습니다. 힙은 위쪽에, 스택은 아래쪽에 배치되는데, 서로 반대 방향으로 확장될 수 있어야 하기 때문입니다. (이런 배치는 일반적인 관례일 뿐, 필요에 따라 얼마든지 다르게 구성할 수 있습니다.)
 
-다음으로 프로그램 실행과 더불어 확장되거나 축소될 수 있는 힙과 스택이 존재합니다.
+그림에서 데이터 영역이 0~16KB 주소를 사용하는 것처럼 보이지만, 실제 물리 메모리에서 해당 주소를 쓰는 건 아닙니다. 메모리 가상화 기법을 통해 임의의 물리 주소에 맵핑되기 때문이죠. (그림 13.2를 보면 각 프로세스가 64KB씩의 가상 주소 공간을 갖지만, 실제 물리 메모리에서는 그에 대응하는 0~64KB 영역이 아닌 다른 위치에 적재된 걸 확인할 수 있습니다.)
 
-힙은 상단에, 스택은 하단에 존재하게 됩니다.
+이처럼 운영체제가 가상 주소와 물리 주소의 매핑을 관리하는 것을 '메모리 가상화'라고 부릅니다. 프로그램 입장에서는 자신만의 거대하고 연속적인 메모리 공간을 독점하는 것처럼 보이지만, 사실은 운영체제가 뒤에서 교묘하게 주소를 변환하고 있는 셈이죠.
 
-두 메모리 영역은 확장 할 수 있어야하기 때문에, 각각 서로다른 방향으로 위치하게 되고 각 양 끝단에서 확장하게 됩니다.
+물론 최종적으로 프로그램을 실행할 때는 반드시 가상 주소가 아닌 진짜 물리 주소로 접근해야 합니다. 이 변환 과정을 투명하게 처리하는 것이 운영체제의 중요한 역할 중 하나입니다.
 
-( 이런한 배치는 관례일 뿐, 원한다면 다르게 배치할 수 있습니다. )
+## 가상 메모리 시스템의 목표
 
-위 그림에서는 0~16KB 사이에 데이터가 존재하게 되지만, 실제 메모리에서 0~16KB 사이의 물리주소를 사용하지 않습니다. ( 메모리 가상화 )
+가상 메모리 시스템은 다음 세 가지 주요 목표를 달성하기 위해 설계되었습니다: 투명성(Transparency), 효율성(Efficiency), 보호(Protection).
 
-실제로는 임의의 물리 주소에 탑재됩니다. ( 13.2 그림을 보면 각각 64KB의 공간을 가지지만 실제 공간은 0~64가 아닌 것을 볼 수 있습니다 )
+### 투명성(Transparency)
 
-이런일을 할 때, 우리는 OS가 메모리 가상화를한다고 이야기합니다.
+- 메모리 가상화의 핵심 목표 중 하나는 사용자와 응용 프로그램이 물리 메모리의 복잡성과 한계를 직접 다룰 필요가 없게 하는 것입니다.
+- 각 프로세스는 마치 자신이 시스템의 모든 메모리를 독점하고 있는 것처럼 동작할 수 있어야 합니다.
+- 운영체제는 이를 위해 각 프로세스에게 독립적인 가상 주소 공간을 제공합니다. 프로세스는 이 가상 공간 내에서 자유롭게 메모리를 사용할 수 있습니다.
 
-왜냐하면, 프로그램은 실제로 자신이 실제 물리주소에 저장된다고 생각하게되고 매우 큰 공간을 가지고 있다고 생각하기 때문입니다.
+### 효율성(Efficiency)
 
-실제로 프로그램이 실행될 때 OS는 가상주소( virtual address )가 아닌, 실제 물리 주소를 읽도록 보장해야합니다.
+- 메모리 가상화는 시간적으로나 공간적으로나 효율적으로 구현되어야 합니다.
+- 운영체제가 가상 주소를 실제 물리 주소로 변환하는 과정에서 발생하는 오버헤드를 최소화해야 합니다.
+- 이를 위해 페이지 테이블(page table)이나 TLB(Translation Lookaside Buffer)와 같은 하드웨어 지원 메커니즘이 필수적입니다.
 
-## 목표
+```{admonition} TLB(Translation Lookaside Buffer)
+TLB는 가장 최근에 사용된 가상-물리 주소 매핑 정보를 캐시로 저장하는 하드웨어 장치입니다. 주소 변환이 필요할 때 페이지 테이블을 탐색하기 전에 먼저 TLB를 확인함으로써, 주소 변환 속도를 크게 향상시킬 수 있습니다.
+```
 
-가상 메모리 시스템의 주요 목표는 **투명성 (Transparency), 효율성 (Efficiency), 보호 (Protection)** 이다.
+### 보호(Protection)
 
-### 투명성 (Transparency)
+- 메모리 가상화는 각 프로세스를 다른 프로세스와 운영체제로부터 보호하는 데 있어 필수적인 역할을 합니다.
+- 프로세스는 오직 자신의 가상 주소 공간 내에서만 메모리에 접근할 수 있어야 하며, 다른 프로세스의 메모리 영역에는 절대 접근할 수 없어야 합니다.
+  - 이는 각 메모리 영역에 대한 접근 권한을 철저히 관리함으로써 달성할 수 있습니다.
+- 가상 메모리 시스템은 각 페이지나 세그먼트 별로 읽기(read), 쓰기(write), 실행(execute) 권한을 설정할 수 있습니다. 이를 통해 잘못된 메모리 접근이나 악의적인 행위를 차단할 수 있습니다.
+- 이런 보호 기능을 활용하면 프로세스를 서로 완벽히 '격리(isolation)'시킬 수 있습니다. 한 프로세스의 오류가 다른 프로세스나 시스템 전체에 영향을 미치지 않도록 하는 거죠.
 
-- 메모리 가상화는 사용자 및 응용 프로그램이 실제 물리 메모리의 복잡성과 제한을 인식하지 않도록 설계되어야 한다.
-- 프로세스는 자신이 물리 메모리 전체를 독점적으로 사용하는 것처럼 동작할 수 있어야 한다.
-- 운영 체제는 가상 주소 공간을 제공하며, 각 프로세스는 자신만의 독립된 주소 공간에서 실행되는 것처럼 실행된다.
+이상의 세 가지 목표, 즉 사용자/프로그램 입장에서의 투명성, 구현 측면에서의 효율성, 그리고 시스템 안정성을 위한 보호 기능이 현대적인 가상 메모리 시스템의 핵심 설계 원칙이라 할 수 있겠습니다. 운영체제는 이 원칙에 입각하여 한정된 물리 메모리를 다수의 프로세스가 공유하면서도, 마치 각자 독립된 메모리를 가진 것처럼 사용할 수 있게 만듭니다.
 
-### 효율성 (Efficiency)
+## 요약
 
-- 메모리 가상화는 시간과 공간 측면에서 효율적으로 구현되어야 한다.
-- 운영 체제가 가상 메모리를 물리 메모리로 매핑하는 과정에서 최소한의 오버헤드로 수행되어야 한다.
-- 페이지 테이블, TLB(Translation Lookaside Buffer)와 같은 하드웨어 지원 메커니즘은 이 목표를 달성하기 위해 필수적이다.
+가상 메모리 시스템은 메모리 가상화 기술을 활용하여 물리 메모리의 복잡성을 프로세스로부터 숨기고, 각 프로세스에게 독립적이고 투명한 메모리 환경을 제공합니다.
 
-```{admonition} TLB(Translation Lookaside Buffer)
-TLB는 가장 자주 접근하는 가상 주소의 변환을 캐시하여 물리 주소 변환 과정을 가속화한다.
-```
+프로세스는 자신만의 가상 주소 공간에서 실행되는 것처럼 느끼게 됩니다. 이를 위해서는 가상 주소와 물리 주소 간의 효율적인 매핑과 접근 제어가 필수적이며, 페이지 테이블과 TLB와 같은 하드웨어적 지원이 중요한 역할을 합니다.
 
-### 보호 (Protection)
+또한 시스템의 안정성과 보안을 위해, 각 프로세스는 오직 자신에게 할당된 주소 공간 내에서만 메모리에 접근할 수 있어야 합니다. 운영체제는 메모리 접근 권한을 엄격히 통제함으로써 프로세스 간의 상호 격리를 유지합니다.
 
-- 메모리 가상화는 각 프로세스를 서로 및 운영 체제로부터 보호하는 데 필수적이다.
-- 프로세스는 자신의 가상 주소 공간 내에서만 메모리에 접근할 수 있으며, 다른 프로세스의 공간에는 접근할 수 없어야한다.
-  > (메모리 접근 권한을 철저히 관리함으로써 달성가능)
-- 가상 메모리 시스템은 각 페이지 또는 세그먼트에 대한 접근 권한(읽기, 쓰기, 실행)을 설정하여, 잘못된 접근 시도나 악의적인 활동을 방지한다.
-- 이러한 보호 성질을 이용하여, 프로세스를 격리 ( isolation ) 시켜야한다.
+### 메모리 관리의 변천사
 
-## 요약
+- 초기 운영체제에서는 한 번에 하나의 프로그램만 물리 메모리 상에서 실행되었습니다.
 
-가상 메모리 시스템은 메모리 가상화를 통해 프로세스에게 실제 물리 메모리의 복잡성을 숨기고, 투명성을 제공합니다.
-각 프로세스는 독립된 주소 공간에서 실행되는 것처럼 보여야 합니다. 이를 위해 효율적인 매핑 및 접근 제어가 필요하며,
-하드웨어 지원 기능인 페이지 테이블과 TLB가 중요합니다.
-또한, 보호를 위해 각 프로세스는 자신의 주소 공간 외에는 접근할 수 없어야 하며,
-메모리 접근 권한을 철저히 관리하여 프로세스 간 격리를 유지해야 합니다.
+- 그러나 멀티프로그래밍과 시분할 시스템의 등장으로, 여러 프로세스가 동시에 메모리에 상주하며 실행되는 환경이 도래했습니다.
 
-### 메모리 관리의 변천
+### 메모리 가상화의 도입
 
-- 초기 운영 체제는 **물리 메모리**에 단일 프로그램만 실행시키는 구조였다.
-- **멀티프로그래밍**과 **시분할 시스템**의 도입으로, 다수의 프로세스가 동시에 실행되는 환경이 마련되었다.
+- 메모리 가상화는 각 프로세스에게 독자적인 주소 공간을 부여함으로써, 마치 전체 메모리를 혼자 사용하는 것 같은 환상을 제공합니다.
 
-### 메모리 가상화의 도입
+- 이는 한정된 메모리 자원을 보다 효율적으로 활용하고, 프로세스 사이의 상호 보호를 가능케 하기 위한 목적으로 도입되었습니다.
+
+### 주소 공간의 구성 요소
+
+- 코드(텍스트) 영역: 기계어로 컴파일된 프로그램 코드가 저장되는 부분입니다.
+
+- 데이터 영역: 전역 변수나 정적 변수 등 프로그램의 데이터가 할당됩니다.
 
-- **메모리 가상화**는 각 프로세스에 독립된 주소 공간을 제공하여, 프로세스가 전체 메모리를 독점하는 것처럼 환상을 제공한다.
-- 가상화의 목적은 메모리의 효율적 사용과 프로세스 간의 보호다.
+- 힙 영역: 프로그램 실행 중에 동적으로 할당되고 해제되는 메모리 공간입니다.
 
-### 주소 공간 구성
+- 스택 영역: 함수 호출 시 전달되는 인자, 반환 주소, 지역 변수 등이 임시로 저장됩니다.
 
-- **코드(텍스트) 영역:** CPU가 실행할 기계어 코드를 저장한다.
-- **데이터 영역:** 전역 변수와 정적 변수를 저장한다.
-- **힙 영역:** 동적으로 할당되는 데이터를 저장한다.
-- **스택 영역:** 함수의 호출과 지역 변수를 저장한다.
-
-### 가상 메모리 시스템의 목표
-
-1. **투명성(Transparency):**
-   - 프로세스가 독립된 주소 공간을 가지고 있는 것처럼 느끼게 함으로써, 물리 메모리의 복잡성을 응용 프로그램으로부터 숨긴다.
-2. **효율성(Efficiency):**
-   - 가상 주소를 물리 주소로 변환하는 과정에서 발생하는 오버헤드를 최소화하여, 시스템 자원을 최적으로 활용한다.
-3. **보호(Protection):**
-   - 각 프로세스가 자신의 메모리 영역 안에서만 작동하도록 제한하여, 프로세스 간의 데이터 침범을 방지한다.
+### 가상 메모리 시스템의 세 가지 목표
+
+1. 투명성(Transparency):
+
+   - 프로세스는 자신만의 독립된 메모리 공간을 가진 것처럼 인식하며, 실제 물리 메모리의 복잡성은 운영체제에 의해 추상화됩니다.
+
+2. 효율성(Efficiency):
+
+   - 가상 주소에서 물리 주소로의 변환 과정에서 발생하는 오버헤드를 최소화함으로써 시스템 자원을 최적으로 활용합니다.
+
+3. 보호(Protection):
+   - 각 프로세스는 자신에게 할당된 메모리 영역 내에서만 작업할 수 있으며, 다른 프로세스의 메모리를 침범할 수 없습니다.
 
 ### 결론
 
-- 운영 체제의 메모리 관리와 가상화 기술은 멀티프로그래밍 환경에서 프로세스의 효율적 실행과 데이터의 안전한 관리를 가능하게 한다.
+현대 운영체제에서 메모리 관리와 가상화 기술은 다중 프로그래밍 환경에서 프로세스를 효과적으로 실행하고, 데이터를 안전하게 관리하는 데 있어 필수불가결한 요소라 할 수 있습니다.
+
+가상 메모리 시스템은 제한된 물리 메모리를 다수의 프로세스가 공유하면서도, 각자 독자적인 메모리 공간을 가진 것처럼 사용할 수 있게 해줍니다. 이를 통해 프로세스 간 간섭 없이 안정적으로 프로그램을 실행하고, 시스템 전체의 성능과 효율성을 높일 수 있게 되었습니다.
+
+운영체제가 제공하는 이런 가상화 기술 덕분에, 프로그래머들은 하드웨어적 제약에 구애받지 않고 더 자유롭고 창의적으로 소프트웨어를 개발할 수 있게 된 것이죠. 가상 메모리야말로 현대 컴퓨팅 시스템의 핵심 기반이라 해도 과언이 아닐 것입니다.
```

### Comparing `os2024-0.4.0/PKG-INFO` & `os2024-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2024
-Version: 0.4.0
+Version: 0.5.0
 Summary: Operating Systems 2024 Class
 Home-page: https://os2024.halla.ai
 License: CC-BY-4.0
 Author: Young Joon Lee
 Author-email: yj.lee@chu.ac.kr
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
```

