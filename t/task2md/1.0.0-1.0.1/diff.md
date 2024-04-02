# Comparing `tmp/task2md-1.0.0.tar.gz` & `tmp/task2md-1.0.1.tar.gz`

## Comparing `task2md-1.0.0.tar` & `task2md-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 task2md-1.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.0.0/.markdownlint.yaml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.0.0/.python-version
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.0.0/.releaserc
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.0.0/.vale.ini
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.0.0/.yamllint
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.0.0/Taskfile.project.yml
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 task2md-1.0.0/Taskfile.yml
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.0.0/lychee.toml
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.0.0/requirements-dev.lock
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.0.0/requirements.lock
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/cli.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/index.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/task2md.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/task/file.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/task/header.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/task/task.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/task/variable.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.0.0/docs/util/dir.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/__init__.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/task/__init__.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/task/file.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/task/header.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/task/task.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/task/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/util/__init__.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.0.0/src/task2md/util/dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/test_dir.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/test_file.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/test_task2md.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/files/empty.yml
--rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/files/lint.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/task/__init__.py
--rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/task/test_file.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/task/test_header.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/task/test_task.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/task/test_variable.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.0.0/tests/util/test_dir.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.0.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.0.0/LICENSE
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.0.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 task2md-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 task2md-1.0.1/.markdownlint.yaml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 task2md-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 task2md-1.0.1/.python-version
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 task2md-1.0.1/.releaserc
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 task2md-1.0.1/.vale.ini
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 task2md-1.0.1/.yamllint
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 task2md-1.0.1/Taskfile.project.yml
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 task2md-1.0.1/Taskfile.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 task2md-1.0.1/lychee.toml
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 task2md-1.0.1/mkdocs.yml
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 task2md-1.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 task2md-1.0.1/requirements.lock
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/cli.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/index.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task2md.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/file.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/header.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/task.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/task/variable.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 task2md-1.0.1/docs/util/dir.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/__init__.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/__init__.py
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/file.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/header.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/task.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/task/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/util/__init__.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 task2md-1.0.1/src/task2md/util/dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/test_dir.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/test_file.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/test_task2md.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/files/empty.yml
+-rw-r--r--   0        0        0    23471 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/files/lint.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/__init__.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_file.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_header.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_task.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/task/test_variable.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 task2md-1.0.1/tests/util/test_dir.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 task2md-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 task2md-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 task2md-1.0.1/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 task2md-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 task2md-1.0.1/PKG-INFO
```

### Comparing `task2md-1.0.0/.gitlab-ci.yml` & `task2md-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/.pre-commit-config.yaml` & `task2md-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/Taskfile.project.yml` & `task2md-1.0.1/Taskfile.project.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/Taskfile.yml` & `task2md-1.0.1/Taskfile.yml`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,16 @@
        FILE | F Taskfile project path (optional, by default Taskfile.project.yml)
     vars:
       FILE: '{{default .F .FILE}}'
       D_FILE: '{{default "Taskfile.project.yml" .FILE}}'
     cmds:
       - |
         if [ -d "{{.DIR_TASKFILES}}" ]; then
-          ls -1 {{.DIR_TASKFILES}}/*.yml |
-          while IFS= read -r template; do
+          for template in {{.DIR_TASKFILES}}/*.yml
+          do
             template_name=$(basename "$template")
             printf "\033[0;33m[ %s: ]\033[0m " "${template_name%.yml}" && task --list -t "$template" || true
             echo ""
           done
         fi
       - |
         if [ ! -z "{{.D_FILE}}" ]; then
```

### Comparing `task2md-1.0.0/requirements-dev.lock` & `task2md-1.0.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/src/task2md/task2md.py` & `task2md-1.0.1/src/task2md/task2md.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import click
 
 from task2md.task.file import File
 from task2md.util.dir import Dir
 
 
 @click.group()
-@click.version_option("1.0.0", prog_name="task2md")
+@click.version_option("1.0.1", prog_name="task2md")
 def cli() -> None:
     """A CLI tool to generate markdown documentation files from Task files."""
     pass
 
 
 @cli.command()
 @click.option(
```

### Comparing `task2md-1.0.0/src/task2md/task/file.py` & `task2md-1.0.1/src/task2md/task/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         output = """
 | Tasks | Description |
 | ----- | ----------- |
 """
         for task in self.tasks:
             file_name = self.get_filename()
             output += (
-                f"| [`{file_name}:{task.name}`](#:simple-task:-{file_name}:{task.name})"
+                f"| [`{file_name}:{task.name}`](#{file_name}{task.name})"
                 f" | {task.desc} |\n"
             )
 
         return output
 
     def global_variables_to_md(self) -> str:
         """Return the global variables to a markdown table
```

### Comparing `task2md-1.0.0/src/task2md/task/header.py` & `task2md-1.0.1/src/task2md/task/header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/src/task2md/task/task.py` & `task2md-1.0.1/src/task2md/task/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,17 @@
                     else:
                         break
             if found_req:
                 del partial_summary_lines[i : (i + j + 2)]
                 break
 
         # Comments
-        self.summary_comments = "\n".join(partial_summary_lines).strip("\n")
+        self.summary_comments = (
+            "\n".join(partial_summary_lines).strip().replace("\n", "  \n")
+        )
 
         self.parsed = True
 
     def to_md(self, file_name: str) -> str:
         """Return the details of the task
 
         Args:
@@ -115,16 +117,15 @@
 | Arguments | Description |
 | --------- | ----------- |
 """
         if len(self.summary_args) == 0:
             output += "| - | - |\n"
         else:
             for arg in self.summary_args:
-                label = arg.label.replace("|", "\\|")
-                output += f"| `{label}` | {arg.value} |\n"
+                output += f"| `{arg.label}` | {arg.value} |\n"
         output += "\n"
 
         # Comments
         output += f"{self.summary_comments}\n\n"
 
         # Requirements
         output += '!!! info "Requirements:"\n\n'
```

### Comparing `task2md-1.0.0/src/task2md/task/variable.py` & `task2md-1.0.1/src/task2md/task/variable.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/src/task2md/util/dir.py` & `task2md-1.0.1/src/task2md/util/dir.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/tests/test_dir.py` & `task2md-1.0.1/tests/test_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         assert "Task documentation generated: empty.md" in result.stdout
         assert "Task documentation generated: lint.md" in result.stdout
         output = self.get_output_content("lint.md")
         assert "tags:" in output
         assert "  - lint" in output
         assert " * :material-check-circle: Status: stable" in output
         assert " * :material-license: License: MIT" in output
-        assert "| [`lint:all`](#:simple-task:-lint:all) " in output
+        assert "| [`lint:all`](#lintall) " in output
         assert "| `IMAGE_HADOLINT` |" in output
         assert "| Default image for lint:docker task |" in output
         assert "| `hadolint/hadolint` |" in output
         assert "## :simple-task: lint:all" in output
         assert "[LINT] Linter" in output
         assert "Usage: task" in output
         assert "| Arguments | Description |" in output
```

### Comparing `task2md-1.0.0/tests/test_file.py` & `task2md-1.0.1/tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         assert result.exit_code == 0
         assert "Task documentation generated: lint.md" in result.stdout
         output = self.get_output_content("lint.md")
         assert "tags:" in output
         assert "  - lint" in output
         assert " * :material-check-circle: Status: stable" in output
         assert " * :material-license: License: MIT" in output
-        assert "| [`lint:all`](#:simple-task:-lint:all) " in output
+        assert "| [`lint:all`](#lintall) " in output
         assert "| `IMAGE_HADOLINT` |" in output
         assert "| Default image for lint:docker task |" in output
         assert "| `hadolint/hadolint` |" in output
         assert "## :simple-task: lint:all" in output
         assert "[LINT] Linter" in output
         assert "Usage: task" in output
         assert "| Arguments | Description |" in output
```

### Comparing `task2md-1.0.0/tests/test_task2md.py` & `task2md-1.0.1/tests/test_task2md.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/tests/files/lint.yml` & `task2md-1.0.1/tests/files/lint.yml`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/tests/task/test_file.py` & `task2md-1.0.1/tests/task/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,18 +237,18 @@
         f = File(content=TASKS)
         f.path = "my_dir/lint.yml"
         f.parse()
         output = f.tasks_list_to_md()
 
         assert TASKS_LIST_HEADER in output
         assert (
-            '| [`lint:all`](#:simple-task:-lint:all) | Linter for files, markdown, yaml extensions. Arguments: [FIX|F=y|Y] [MEX|M="#node_modules"] (*) |'
+            '| [`lint:all`](#lintall) | Linter for files, markdown, yaml extensions. Arguments: [FIX|F=y|Y] [MEX|M="#node_modules"] (*) |'
             in output
         )
-        assert "| [`lint:file`](#:simple-task:-lint:file) | Linter for files" in output
+        assert "| [`lint:file`](#lintfile) | Linter for files" in output
 
     def test_file_global_variables_to_md(self) -> None:
         f = File(content=VARS4)
         f.parse()
         assert len(f.global_variables) == 4
         output = f.global_variables_to_md()
```

### Comparing `task2md-1.0.0/tests/task/test_header.py` & `task2md-1.0.1/tests/task/test_header.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/tests/task/test_task.py` & `task2md-1.0.1/tests/task/test_task.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/tests/task/test_variable.py` & `task2md-1.0.1/tests/task/test_variable.py`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/LICENSE` & `task2md-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/README.md` & `task2md-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `task2md-1.0.0/pyproject.toml` & `task2md-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "task2md"
-version = "1.0.0"
+version = "1.0.1"
 description = "A program to generate markdown documentation files from Task files"
 authors = [
     { name = "FX Soubirou", email = "soubirou@yahoo.fr" }
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
```

### Comparing `task2md-1.0.0/PKG-INFO` & `task2md-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: task2md
-Version: 1.0.0
+Version: 1.0.1
 Summary: A program to generate markdown documentation files from Task files
 Project-URL: Homepage, https://gitlab.com/op_so/task/task2md
 Project-URL: Documentation, https://op_so.gitlab.io/task/task2md/
 Author-email: FX Soubirou <soubirou@yahoo.fr>
 License: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

