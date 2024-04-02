# Comparing `tmp/sedrila-0.6.0.tar.gz` & `tmp/sedrila-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sedrila-0.6.0.tar", max compression
+gzip compressed data, was "sedrila-0.7.0.tar", max compression
```

## Comparing `sedrila-0.6.0.tar` & `sedrila-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-0.6.0/LICENSE
--rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-0.6.0/README.md
--rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-0.6.0/baseresources/favicon-32x32.png
--rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-0.6.0/baseresources/local.css
--rwxr-xr-x   0        0        0     8057 2024-02-17 09:50:19.451320 sedrila-0.6.0/baseresources/sedrila.css
--rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-0.6.0/baseresources/sidebar.js
--rwxr-xr-x   0        0        0     6607 2024-03-26 13:35:47.411019 sedrila-0.6.0/py/base.py
--rwxr-xr-x   0        0        0     3343 2024-03-19 08:47:22.086143 sedrila-0.6.0/py/git.py
--rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-0.6.0/py/sdrl/__init__.py
--rwxr-xr-x   0        0        0    24154 2024-03-26 13:26:44.008028 sedrila-0.6.0/py/sdrl/course.py
--rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-0.6.0/py/sdrl/glossary.py
--rwxr-xr-x   0        0        0     1206 2024-01-30 14:55:30.878881 sedrila-0.6.0/py/sdrl/html.py
--rwxr-xr-x   0        0        0     3517 2024-03-25 11:31:55.720300 sedrila-0.6.0/py/sdrl/interactive.py
--rwxr-xr-x   0        0        0     8247 2024-03-14 17:40:27.632492 sedrila-0.6.0/py/sdrl/macros.py
--rwxr-xr-x   0        0        0     4604 2024-03-14 17:40:29.403549 sedrila-0.6.0/py/sdrl/markdown.py
--rwxr-xr-x   0        0        0     6059 2024-03-20 16:23:20.848908 sedrila-0.6.0/py/sdrl/part.py
--rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-0.6.0/py/sdrl/participant.py
--rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-0.6.0/py/sdrl/replacements.py
--rwxr-xr-x   0        0        0     8242 2024-03-26 12:39:08.144480 sedrila-0.6.0/py/sdrl/repo.py
--rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-0.6.0/py/sdrl/subcmd/__init__.py
--rwxr-xr-x   0        0        0    25884 2024-03-26 10:09:27.445758 sedrila-0.6.0/py/sdrl/subcmd/author.py
--rwxr-xr-x   0        0        0     8149 2024-03-26 13:05:54.176845 sedrila-0.6.0/py/sdrl/subcmd/instructor.py
--rwxr-xr-x   0        0        0     5959 2024-03-26 13:02:02.723848 sedrila-0.6.0/py/sdrl/subcmd/student.py
--rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-0.6.0/py/sedrila.py
--rwxr-xr-x   0        0        0     2329 2024-03-26 13:35:47.419554 sedrila-0.6.0/pyproject.toml
--rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-0.6.0/templates/base.html
--rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-0.6.0/templates/chapter.html
--rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-0.6.0/templates/glossary.html
--rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-0.6.0/templates/homepage.html
--rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-0.6.0/templates/task.html
--rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-0.6.0/templates/taskgroup.html
--rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-0.6.0/setup.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2022-11-04 08:14:04.746613 sedrila-0.7.0/LICENSE
+-rwxr-xr-x   0        0        0     4087 2024-03-25 11:31:56.923322 sedrila-0.7.0/README.md
+-rwxr-xr-x   0        0        0      622 2024-01-16 08:42:09.535422 sedrila-0.7.0/baseresources/favicon-32x32.png
+-rwxr-xr-x   0        0        0       79 2024-01-06 12:00:53.054430 sedrila-0.7.0/baseresources/local.css
+-rwxr-xr-x   0        0        0     8057 2024-02-17 09:50:19.451320 sedrila-0.7.0/baseresources/sedrila.css
+-rwxr-xr-x   0        0        0     1929 2023-12-21 08:14:44.888758 sedrila-0.7.0/baseresources/sidebar.js
+-rwxr-xr-x   0        0        0     6607 2024-04-02 17:14:14.148211 sedrila-0.7.0/py/base.py
+-rwxr-xr-x   0        0        0     3343 2024-03-19 08:47:22.086143 sedrila-0.7.0/py/git.py
+-rwxr-xr-x   0        0        0       34 2022-11-17 11:17:31.396262 sedrila-0.7.0/py/sdrl/__init__.py
+-rwxr-xr-x   0        0        0    24154 2024-03-26 13:26:44.008028 sedrila-0.7.0/py/sdrl/course.py
+-rwxr-xr-x   0        0        0     9777 2024-03-14 17:40:26.435091 sedrila-0.7.0/py/sdrl/glossary.py
+-rwxr-xr-x   0        0        0     1209 2024-03-28 09:55:55.453116 sedrila-0.7.0/py/sdrl/html.py
+-rwxr-xr-x   0        0        0     3901 2024-04-02 13:32:41.301782 sedrila-0.7.0/py/sdrl/interactive.py
+-rwxr-xr-x   0        0        0     8274 2024-03-27 15:01:39.014198 sedrila-0.7.0/py/sdrl/macros.py
+-rwxr-xr-x   0        0        0     4604 2024-03-14 17:40:29.403549 sedrila-0.7.0/py/sdrl/markdown.py
+-rwxr-xr-x   0        0        0     6059 2024-03-20 16:23:20.848908 sedrila-0.7.0/py/sdrl/part.py
+-rwxr-xr-x   0        0        0     1504 2024-02-23 11:01:27.759372 sedrila-0.7.0/py/sdrl/participant.py
+-rwxr-xr-x   0        0        0     1334 2023-11-22 14:11:46.025037 sedrila-0.7.0/py/sdrl/replacements.py
+-rwxr-xr-x   0        0        0     8344 2024-04-02 17:08:18.901707 sedrila-0.7.0/py/sdrl/repo.py
+-rwxr-xr-x   0        0        0       31 2024-01-24 12:48:05.392624 sedrila-0.7.0/py/sdrl/subcmd/__init__.py
+-rwxr-xr-x   0        0        0    26282 2024-04-02 16:56:24.340593 sedrila-0.7.0/py/sdrl/subcmd/author.py
+-rwxr-xr-x   0        0        0     8508 2024-04-02 13:32:41.354363 sedrila-0.7.0/py/sdrl/subcmd/instructor.py
+-rwxr-xr-x   0        0        0     5959 2024-03-26 13:02:02.723848 sedrila-0.7.0/py/sdrl/subcmd/student.py
+-rwxr-xr-x   0        0        0      975 2024-02-24 16:55:02.006852 sedrila-0.7.0/py/sedrila.py
+-rwxr-xr-x   0        0        0     2329 2024-04-02 17:14:14.141110 sedrila-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1546 2024-03-20 16:45:46.286389 sedrila-0.7.0/templates/base.html
+-rwxr-xr-x   0        0        0      198 2023-12-21 08:24:47.653800 sedrila-0.7.0/templates/chapter.html
+-rwxr-xr-x   0        0        0      154 2024-01-05 15:47:36.097811 sedrila-0.7.0/templates/glossary.html
+-rwxr-xr-x   0        0        0      158 2023-12-21 08:24:47.628801 sedrila-0.7.0/templates/homepage.html
+-rwxr-xr-x   0        0        0      312 2024-03-20 16:41:25.421337 sedrila-0.7.0/templates/task.html
+-rwxr-xr-x   0        0        0      159 2023-12-21 08:24:47.660799 sedrila-0.7.0/templates/taskgroup.html
+-rw-r--r--   0        0        0    11173 1970-01-01 00:00:00.000000 sedrila-0.7.0/setup.py
+-rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 sedrila-0.7.0/PKG-INFO
```

### Comparing `sedrila-0.6.0/LICENSE` & `sedrila-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/README.md` & `sedrila-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/baseresources/favicon-32x32.png` & `sedrila-0.7.0/baseresources/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/baseresources/sedrila.css` & `sedrila-0.7.0/baseresources/sedrila.css`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/baseresources/sidebar.js` & `sedrila-0.7.0/baseresources/sidebar.js`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/base.py` & `sedrila-0.7.0/py/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import requests
 import rich
 import rich.table
 import yaml
 
 
-SEDRILA_VERSION = "0.6.0"  # keep in sync with pyproject.toml
+SEDRILA_VERSION = "0.7.0"  # keep in sync with pyproject.toml
 CONFIG_FILENAME = "sedrila.yaml"  # at top-level of source dir
 GLOSSARY_BASENAME = "glossary"  # .md at top-level of chapterdir, .html in build directory
 METADATA_FILE = "course.json"  # at top-level of build directory
 CACHE_FILE = "course.pickle"  # at top-level of instructor build directory
 TEMPLATES_DIR = "templates"
 SEDRILA_COMMAND_ENV = "SEDRILA_COMMAND"
```

### Comparing `sedrila-0.6.0/py/git.py` & `sedrila-0.7.0/py/git.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/course.py` & `sedrila-0.7.0/py/sdrl/course.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/glossary.py` & `sedrila-0.7.0/py/sdrl/glossary.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/html.py` & `sedrila-0.7.0/py/sdrl/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def as_attribute(text: str) -> str:
     """Cleans text so that it can appear between double quotes in an HTML attribute."""
     return text.replace('"', "'").replace("\n", " ")  # no doublequotes, no line breaks
 
 
 def breadcrumb(*args):
     """Renders breadcrumb HTML fragment from list of items with breadcrumb_item property."""
-    SEPARATOR = " > "
+    SEPARATOR = " &gt; "
     return '<div><span class="breadcrumbs">%s</span></div>' % SEPARATOR.join([arg.breadcrumb_item for arg in args])
 
 
 def difficulty_symbol(level: int) -> str:
     difficulty_text = difficulty_levels[level - 1]
     diffclass = f"class='difficulty{level}'"
     circle = f"<span {diffclass} title='Difficulty: {difficulty_text}'>{DIFFICULTY_SIGN}</span>"
```

### Comparing `sedrila-0.6.0/py/sdrl/interactive.py` & `sedrila-0.7.0/py/sdrl/interactive.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from blessed import Terminal
 import typing as tg
+import webbrowser
 
 import base as b
 import sdrl.repo as r
 
 ACCEPT_SYMBOL = "✓"
 REJECT_SYMBOL = "X"
 
@@ -11,36 +12,40 @@
     if selected[entry[0]]:
         return ACCEPT_SYMBOL
     if not(rejected is None) and rejected[entry[0]]:
         return REJECT_SYMBOL
     return " "
 
 
-def redraw_filter_selection(term: Terminal, entries: tg.Sequence[r.ReportEntry], rowindex: int, selected: dict[str, bool], rejected: dict[str, bool]):
+def redraw_filter_selection(term: Terminal, entries: tg.Sequence[r.ReportEntry], rowindex: int, selected: dict[str, bool], rejected: dict[str, bool], course_url: str):
     print(term.home + term.clear, end="")
+    lines = term.height - 1
     print("Move with arrow keys, select/deselect with space/enter, exit with escape")
-    rangestart = max(0, rowindex - term.height / 2)
-    rangeend = min(len(entries), rowindex + term.height / 2)
+    if not(course_url is None):
+        print("Press 'o' to open task in browser")
+        lines = lines - 1
+    rangestart = max(0, rowindex - lines / 2)
+    rangeend = min(len(entries), rowindex + lines / 2)
     for i in range(rangestart, rangeend):
         if i == rowindex:
             print(term.reverse, end="")
         else:
             print(term.normal, end="")
         print(prefix(entries[i], selected, rejected) + " %4.2fh " % entries[i][1] + entries[i][0], end="")
         print(" " * (term.width - 9 - len(entries[i][0]))) #padding to end of line
     print(term.normal, end="") #if we end on the selection
 
 
-def filter_entries(entries: tg.Sequence[r.ReportEntry], selected: dict[str, bool], rejected: dict[str, bool]):
+def filter_entries(entries: tg.Sequence[r.ReportEntry], selected: dict[str, bool], rejected: dict[str, bool], course_url: str):
     term = Terminal()
     rowindex = 0
     with term.cbreak(), term.hidden_cursor():
         inp = None
         while not(inp) or not(str(inp) == "q" or str(inp.name) == "KEY_ESCAPE"):
-            redraw_filter_selection(term, entries, rowindex, selected, rejected)
+            redraw_filter_selection(term, entries, rowindex, selected, rejected, course_url)
             inp = term.inkey()
             if str(inp) == " " or str(inp.name) == "KEY_ENTER":
                 if rejected is None:
                     selected[entries[rowindex][0]] = not(selected[entries[rowindex][0]])
                 elif rejected[entries[rowindex][0]]:
                     rejected[entries[rowindex][0]] = False
                 elif selected[entries[rowindex][0]]:
@@ -50,28 +55,30 @@
                     selected[entries[rowindex][0]] = True
             elif str(inp) == "j" or str(inp.name) == "KEY_DOWN":
                 if rowindex < len(entries) - 1:
                     rowindex += 1
             elif str(inp) == "k" or str(inp.name) == "KEY_UP":
                 if rowindex > 0:
                     rowindex -= 1
+            elif not(course_url is None) and (str(inp) == "o" or str(inp) == "O"):
+                webbrowser.open(f"{course_url}/{entries[rowindex][0]}.html")
 
 
 def select_entries(entries: tg.Sequence[r.ReportEntry]):
     selected = {entry[0]: True for entry in entries}
-    filter_entries(entries, selected, None)
+    filter_entries(entries, selected, None, None)
     return list(filter(lambda entry: selected[entry[0]], entries))
 
 
 #marks entries as accepted if they are, returns rejections as the count might not be enough to know whether they were rejected in current run
-def grade_entries(entries: tg.Sequence[r.ReportEntry]):
+def grade_entries(entries: tg.Sequence[r.ReportEntry], course_url: str):
     submission = b.slurp_yaml(r.SUBMISSION_FILE)
     selected = {entry[0]: (submission.get(entry[0]) or "").startswith(r.ACCEPT_MARK) for entry in entries}
     rejected = {entry[0]: (submission.get(entry[0]) or "").startswith(r.REJECT_MARK) for entry in entries}
-    filter_entries(entries, selected, rejected)
+    filter_entries(entries, selected, rejected, course_url)
     if not(any(selected.values())) and not(any(rejected.values())):
         return None
     for i in range(len(entries)):
         entry = list(entries[i])
         if selected[entry[0]]:
             entry[4] = True
         if rejected[entry[0]]:
```

### Comparing `sedrila-0.6.0/py/sdrl/macros.py` & `sedrila-0.7.0/py/sdrl/macros.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     ppost = ppost if ppost else ""
     if mode == MM.EARLY:
         pass  # use ppre, ppost verbatim
     elif mode == MM.INNER:
         pass  # ditto
     elif mode == MM.BLOCKSTART:
         if not ppre and not ppost:  # Layout 1
-            macrocall.warning("blockmacro blocks must be separated")
+            macrocall.warning("blockmacro blocks must be separated by empty lines _somewhere_")
         elif ppre == '<p>' and not ppost:  # Layout 2
             ppost = ppre  # shift <p> from front to back
             ppre = ""
         elif not ppre and ppost  == '</p>':  # Layout 3
             ppost = ""  # remove
         elif ppre == '<p>' and ppost == '</p>':  # Layout 4
             ppre = ""  # remove
```

### Comparing `sedrila-0.6.0/py/sdrl/markdown.py` & `sedrila-0.7.0/py/sdrl/markdown.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/part.py` & `sedrila-0.7.0/py/sdrl/part.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/participant.py` & `sedrila-0.7.0/py/sdrl/participant.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/replacements.py` & `sedrila-0.7.0/py/sdrl/replacements.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sdrl/repo.py` & `sedrila-0.7.0/py/sdrl/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,19 @@
     accumulate_timevalues_and_attempts(checked_tuples, course)
 
 
 def submission_checked_commit_hashes(course: sdrl.course.Course,
                                      commits: tg.Sequence[git.Commit]) -> tg.Sequence[tg.Sequence[str]]:
     """List of hashes of properly instructor-signed commits of finished submission checks.
     This will be grouped by consecutively done commits of instructors and student, starting with the grading request."""
-    allowed_signers = [b.as_fingerprint(instructor['keyfingerprint'])
-                       for instructor in course.instructors]
+    try:
+        allowed_signers = [b.as_fingerprint(instructor['keyfingerprint'])
+                           for instructor in course.instructors]
+    except KeyError:
+        b.critical("missing 'keyfingerprint' in configuration")
     group = []
     result = [group]
     student_commit = None
     for commit in commits:
         b.debug(f"commit.subject, fpr: {commit.subject}, {commit.key_fingerprint}")
         right_subject = re.match(SUBMISSION_CHECKED_COMMIT_MSG, commit.subject) is not None
         right_signer = commit.key_fingerprint and b.as_fingerprint(commit.key_fingerprint) in allowed_signers
```

### Comparing `sedrila-0.6.0/py/sdrl/subcmd/author.py` & `sedrila-0.7.0/py/sdrl/subcmd/author.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import sdrl.markdown as md
 import sdrl.part
 
 meaning = """Creates and renders an instance of a SeDriLa course.
 Checks consistency of the course description beforehands.
 """
 
-OUTPUT_INSTRUCTORS_DEFAULT_SUBDIR = "cino2r2s2tu"  # alphabetically sorted count-anagram of "instructors"
+OUTPUT_INSTRUCTORS_DEFAULT_SUBDIR = "instructor"
 
 
 def add_arguments(subparser: argparse.ArgumentParser):
     subparser.add_argument('--config', metavar="configfile", default=b.CONFIG_FILENAME,
                            help="SeDriLa configuration description YAML file")
     subparser.add_argument('--include_stage', metavar="stage", default='',
                            help="include parts with this and higher 'stage:' entries in the generated output "
@@ -199,21 +199,21 @@
 
 
 def prepare_directories(course: sdrl.course.Course):
     if course.cache_mode == sdrl.course.CacheMode.READ:
         b.info(f"cached mode: leaving directories as they are: '{course.targetdir_s}', '{course.targetdir_i}'")
     else:
         b.info(f"preparing directories '{course.targetdir_s}', '{course.targetdir_i}'")
-        backup_targetdir(course.targetdir_i, markerfile=f"_{b.CONFIG_FILENAME}")  # do _i first if it is a subdir of _s
-        backup_targetdir(course.targetdir_s, markerfile=f"_{b.CONFIG_FILENAME}")
+        backup_targetdir(course.targetdir_i, markerfile=b.CONFIG_FILENAME)  # do _i first if it is a subdir of _s
+        backup_targetdir(course.targetdir_s, markerfile=b.CONFIG_FILENAME)
         os.mkdir(course.targetdir_s)
         os.mkdir(course.targetdir_i)
         # mark dirs as SeDriLa instances:
-        shutil.copyfile(course.configfile, f"{course.targetdir_s}/_{b.CONFIG_FILENAME}")  
-        shutil.copyfile(course.configfile, f"{course.targetdir_i}/_{b.CONFIG_FILENAME}")
+        shutil.copyfile(course.configfile, f"{course.targetdir_s}/{b.CONFIG_FILENAME}")  
+        shutil.copyfile(course.configfile, f"{course.targetdir_i}/{b.CONFIG_FILENAME}")
     if course.cache_mode == sdrl.course.CacheMode.WRITE:
         with open(cache_filename(course), 'wb') as f:
             pickle.dump(course, f)
         print(f"wrote cache file '{cache_filename(course)}'")
 
 
 def backup_targetdir(targetdir: str, markerfile: str):
@@ -283,14 +283,16 @@
     # ----- register hard-coded block macros:
     macros.register_macro('SECTION', 2, MM.BLOCKSTART, expand_section)
     macros.register_macro('ENDSECTION', 0, MM.BLOCKEND, expand_section)
     macros.register_macro('INNERSECTION', 2, MM.BLOCKSTART, expand_section)
     macros.register_macro('ENDINNERSECTION', 0, MM.BLOCKEND, expand_section)
     macros.register_macro('HINT', 1, MM.BLOCKSTART, expand_hint)
     macros.register_macro('ENDHINT', 0, MM.BLOCKEND, expand_hint)
+    macros.register_macro('FOLDOUT', 1, MM.BLOCKSTART, expand_foldout)
+    macros.register_macro('ENDFOLDOUT', 0, MM.BLOCKEND, expand_foldout)
     # ----- register generic block macros:
     generic_defs = {key: val for key, val in course.blockmacro_topmatter.items() if key.isupper()}
     for key, value in generic_defs.items():
         if "{arg2}" in value:
             args = 2
         elif "{arg1}" in value:
             args = 1
@@ -350,14 +352,22 @@
         content = topmatter(macrocall, 'hint').format(arg1=macrocall.arg1)
         return f"<details class='blockmacro blockmacro-hint'><summary>\n{content}\n</summary>\n"
     elif macrocall.macroname == 'ENDHINT':
         return "</details>"
     assert False, macrocall  # impossible
 
 
+def expand_foldout(macrocall: macros.Macrocall) -> str:
+    if macrocall.macroname == 'FOLDOUT':
+        return f"<details class='blockmacro blockmacro-foldout'><summary>\n{macrocall.arg1}\n</summary>\n"
+    elif macrocall.macroname == 'ENDFOLDOUT':
+        return "</details>"
+    assert False, macrocall  # impossible
+
+
 def expand_block(macrocall: macros.Macrocall) -> str:
     is_end = macrocall.macroname.startswith('END')
     macroname = (macrocall.macroname if not is_end else macrocall.macroname[3:])
     if is_end:
         return f"</div>"
     else:
         content = topmatter(macrocall, macroname).format(arg1=macrocall.arg1, arg2=macrocall.arg2)
@@ -497,15 +507,15 @@
     volume_report_per_stage = course.volume_report_per_stage()
     print("date", end="")
     for stage, numtasks, timevalue in volume_report_per_stage.rows:
         print(f",{stage}", end="")
     print("")  # newline
     print(dt.date.today().strftime("%Y-%m-%d"), end="")
     for stage, numtasks, timevalue in volume_report_per_stage.rows:
-        print(f",{timevalue}", end="")
+        print(",%.2f" % timevalue, end="")
     print("")  # newline
 
     # ----- print all reports as rich tables:
     for report in (volume_report_per_stage,
                    course.volume_report_per_difficulty(),
                    course.volume_report_per_chapter()):
         table = b.Table()
```

### Comparing `sedrila-0.6.0/py/sdrl/subcmd/instructor.py` & `sedrila-0.7.0/py/sdrl/subcmd/instructor.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,25 +49,26 @@
         return
     student = sdrl.participant.Student()
     metadatafile = f"{student.course_url}/{b.METADATA_FILE}"
     course = sdrl.course.Course(metadatafile, read_contentfiles=False, include_stage="")
     r.compute_student_work_so_far(course)
     entries, workhours_total, timevalue_total = r.student_work_so_far(course)
     opentasks = rewrite_submission_file(course, r.SUBMISSION_FILE)
-    entries = list(filter(lambda entry: entry[0] in opentasks and course.task(entry[0]).remaining, entries))
+    entries = list(filter(lambda entry: entry[0] in opentasks and course.task(entry[0]).remaining_attempts > 0, entries))
     if not(pargs.check):
         b.info("Don't run check, just prepare commit")
     elif not(entries):
         b.info("No tasks to check found. Assuming check already done. Preparing commit.")
     elif pargs.interactive:
-        rejections = i.grade_entries(entries)
+        rejections = i.grade_entries(entries, student.course_url)
         if rejections is None:
             b.info("Nothing selected, nothing to do")
             return
         b.spit_yaml(r.SUBMISSION_FILE, r.submission_file_entries(course, entries, rejections))
+        subshell_exit_info(reminder=True)
     else:
         call_instructor_cmd(course, instructor_cmd(), pargs, iteration=0)
     if pargs.put:
         validate_submission_file(course, r.SUBMISSION_FILE)
         commit_and_push(r.SUBMISSION_FILE)
     os.chdir("..")
 
@@ -113,22 +114,30 @@
             entries[taskname] = r.NONTASK_MARK
         elif task.accepted:
             entries[taskname] = r.ACCEPT_MARK
         elif task.rejections > 0:
             entries[taskname] += f" (previously rejected {task.rejections}x)"
 
 
+def subshell_exit_info(reminder: bool = False):
+    if reminder and not(os.environ.get(b.SEDRILA_COMMAND_ENV)):
+        return #explicit call, no subshell. no need to provide that info
+    if reminder:
+        b.info("You are still inside a subshell command!")
+    b.info("Exit that command (e.g. the shell) to trigger automatic commit+push")
+    b.info(f"of the modified {r.SUBMISSION_FILE}.")
+
+
 def call_instructor_cmd(course: sdrl.course.Course, cmd: str, pargs: argparse.Namespace = None, iteration: int = 0):
     """Calls user-set command as indicated by environment variables"""
     if iteration == 0:
         b.info(f"Will now call the command given in the {USER_CMD_VAR} environment variable or else")
         b.info(f"the command given in the SHELL environment variable or else '{USER_CMD_DEFAULT}'.")
         b.info(f"The resulting command in your case will be:\n  '{cmd}'")
-        b.info("Exit that command (e.g. the shell) to trigger automatic commit+push")
-        b.info(f"of the modified {r.SUBMISSION_FILE}.")
+        subshell_exit_info()
         b.info(f"Please change status of tasks in {r.SUBMISSION_FILE} to either {r.ACCEPT_MARK}\nor {r.REJECT_MARK} accordingly.")
         b.info("You can also just run `sedrila` to get an interactive list.")
         b.info("Feel free to add remarks at the end of the accept/reject lines.")
     else:
         b.info(f"Calling '{cmd}' again. (You can Ctrl-C right after it.)")
     if pargs:
         os.environ[b.SEDRILA_COMMAND_ENV] = f"instructor {pargs.repo_url} --interactive --no-get --no-put"
```

### Comparing `sedrila-0.6.0/py/sdrl/subcmd/student.py` & `sedrila-0.7.0/py/sdrl/subcmd/student.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/py/sedrila.py` & `sedrila-0.7.0/py/sedrila.py`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/pyproject.toml` & `sedrila-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # https://packaging.python.org/en/latest/
 # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "sedrila"
-version = "0.6.0"  # keep in sync with base.py
+version = "0.7.0"  # keep in sync with base.py
 description = "Tool infrastructure for building and running \"self-driven lab\" courses"
 license = "MIT"
 authors = ["Lutz Prechelt <prechelt@inf.fu-berlin.de>"]
 readme = "README.md"
 homepage = "https://github.com/fubinf/sedrila"
 repository = "https://github.com/fubinf/sedrila"
 keywords = ["static site generator"]
```

### Comparing `sedrila-0.6.0/templates/base.html` & `sedrila-0.7.0/templates/base.html`

 * *Files identical despite different names*

### Comparing `sedrila-0.6.0/setup.py` & `sedrila-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
  'rich>=13.7,<14.0']
 
 entry_points = \
 {'console_scripts': ['sedrila = sedrila:main']}
 
 setup_kwargs = {
     'name': 'sedrila',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Tool infrastructure for building and running "self-driven lab" courses',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/sedrila/badge/?version=latest)](https://sedrila.readthedocs.io/en/latest/?badge=latest)\n\n# `sedrila`: Tool infrastructure for building and running "self-driven lab" courses\n\nA "self-driven lab" (SeDriLa) course is one where students select freely \na subset from a large set of tasks.\nThe tasks are described with sufficient detail that no guidance from an instructor\nis needed most of the time.\n\nsedrila is a command-line tool supporting course authors for authoring a course\nand then course instructors and students for executing it.\n\nFind the [documentation at readthedocs](https://sedrila.readthedocs.io).\n\n\n## Ideas for future versions\n\n- Process `SEDRILA_INSTRUCTOR_COURSE_URLS` as described in the instructor documentation.\n- `sedrila instructor` should keep a JSON file `student_course_urls.json` that maps student usernames\n  to the course URL first seen for that student, because if a student ever changed\n  the URL in the `student.yaml`, prior signed commits of instructors might become \n  invalid semantically if the new course has a different set of tasks.  \n  The map is added to when a `student.yaml` is first seen\n  and checked against at each later time.  \n  Note that a student taking part a second time, with a fresh repo,\n  might require manual editing of that JSON file to remove that entry.\n- Better yet, there could be an option `sedrial instructor --allow-repo2` that \n  performs that editing automatically\n  and also checks that the new repo contains no instructor-signed commits.\n- Command `sedrila instructor --clean-up-repos-home`\n  to clean up instructor work directory trees-of-trees\n  by deleting all level-1 subtrees in which the `student.yaml`\n  has a `course_url` that is not mentioned in the \n  `SEDRILA_INSTRUCTOR_COURSE_URLS`environment variable.\n  This option should ask a safety question before starting to work.\n\n\n## Development process: TODO-handling during development\n\nWe use this convention for the development of `sedrila`.\nIt may also be helpful for course authors if the team is small enough.\n\nIf something is incomplete, add a TODO marker with a priorization digit:\n- `TODO 1`: to be completed soon (within a few days)\n- `TODO 2`: to be completed once the prio 1 things are done (within days or a few weeks)\n- `TODO 3`: to be completed at some later time (usually several weeks or more into the future,\n  because it is big) or never (because it is not-so-important: "nice-to-have features")\n\nAdd a short description of what needs to be done. Examples:\n- `TODO 1: find proper formulation`\n- `TODO 2: restructure to use ACME lib`\n- `TODO 3: add automatic grammar correction`\n\nIf you intend to do it yourself, add your name in parens:  \n`TODO 1: find proper formulation (Lutz)`\n\nThen use the IDE global search to work through these layer-by-layer.\nDemote items to a lower priority when they become stale or remove them.\nKick out prio 3 items when they become unlikely.\n\n\n## A currently needed refactoring: Target directory structure\n\nThe current layout of the source tree is wrong.\nCurrently, the `templates` and `baseresources` directories will end up \nas top-level directories when the package is installed,\nwhich means they will clash with any top-level modules of that name\nanywhere in our dependencies.\n\nWe need to perform the following refactorings to arrive at a proper structure:\n\n- `py` --> `sedrila`: This will be the top level directory that gets installed.\n- `sedrila/sdrl/*` --> `sedrila/*`: We remove the now-intermediate namespace.\n  This implies joining the current `sdrl/tests` into `sedrila/tests`.\n- `templates` --> `sedrila/templates`: The HTML templates simply become part of the\n  tree to be installed.\n- `baseresources` --> `sedrila/baseresources`: Ditto.\n\nThese changes require a lot of changes of import statements.\nFor instance, the current module `base` will become `sedrila.base`\nand `sdrl.course` will become `sedrila.course`.\nThe logic for computing `sedrila_libdir` in `courses.py` must be adapted.\nThe files lists in `pyproject.toml` must be corrected.\n',
     'author': 'Lutz Prechelt',
     'author_email': 'prechelt@inf.fu-berlin.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fubinf/sedrila',
```

### Comparing `sedrila-0.6.0/PKG-INFO` & `sedrila-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sedrila
-Version: 0.6.0
+Version: 0.7.0
 Summary: Tool infrastructure for building and running "self-driven lab" courses
 Home-page: https://github.com/fubinf/sedrila
 License: MIT
 Keywords: static site generator
 Author: Lutz Prechelt
 Author-email: prechelt@inf.fu-berlin.de
 Requires-Python: >=3.11,<4.0
```

