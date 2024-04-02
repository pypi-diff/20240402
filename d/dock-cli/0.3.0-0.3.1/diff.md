# Comparing `tmp/dock-cli-0.3.0.tar.gz` & `tmp/dock-cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock-cli-0.3.0.tar", last modified: Sat Mar 30 15:42:41 2024, max compression
+gzip compressed data, was "dock-cli-0.3.1.tar", last modified: Tue Apr  2 07:58:38 2024, max compression
```

## Comparing `dock-cli-0.3.0.tar` & `dock-cli-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-03-30 15:42:41.402057 dock-cli-0.3.0/
--rw-r--r--   0 posen      (501) staff       (20)     1062 2024-03-05 06:48:54.000000 dock-cli-0.3.0/LICENSE
--rw-r--r--   0 posen      (501) staff       (20)     1957 2024-03-30 15:42:41.401807 dock-cli-0.3.0/PKG-INFO
--rw-r--r--   0 posen      (501) staff       (20)     1693 2024-03-25 15:48:25.000000 dock-cli-0.3.0/README.md
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-03-30 15:42:41.397791 dock-cli-0.3.0/dock_cli/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.0/dock_cli/__init__.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-03-30 15:42:41.399465 dock-cli-0.3.0/dock_cli/cli/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.0/dock_cli/cli/__init__.py
--rw-r--r--   0 posen      (501) staff       (20)     3870 2024-03-30 10:14:50.000000 dock-cli-0.3.0/dock_cli/cli/chart.py
--rw-r--r--   0 posen      (501) staff       (20)     5407 2024-03-30 15:30:50.000000 dock-cli-0.3.0/dock_cli/cli/image.py
--rw-r--r--   0 posen      (501) staff       (20)     2455 2024-03-29 15:34:22.000000 dock-cli-0.3.0/dock_cli/main.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-03-30 15:42:41.401151 dock-cli-0.3.0/dock_cli/utils/
--rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.0/dock_cli/utils/__init__.py
--rw-r--r--   0 posen      (501) staff       (20)      773 2024-03-25 08:12:51.000000 dock-cli-0.3.0/dock_cli/utils/callback.py
--rw-r--r--   0 posen      (501) staff       (20)      629 2024-03-21 16:14:08.000000 dock-cli-0.3.0/dock_cli/utils/commands.py
--rw-r--r--   0 posen      (501) staff       (20)     4529 2024-03-30 06:00:03.000000 dock-cli-0.3.0/dock_cli/utils/helpers.py
--rw-r--r--   0 posen      (501) staff       (20)      530 2024-03-25 08:26:16.000000 dock-cli-0.3.0/dock_cli/utils/schema.py
--rw-r--r--   0 posen      (501) staff       (20)     2089 2024-03-29 18:16:40.000000 dock-cli-0.3.0/dock_cli/utils/utils.py
-drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-03-30 15:42:41.401544 dock-cli-0.3.0/dock_cli.egg-info/
--rw-r--r--   0 posen      (501) staff       (20)     1957 2024-03-30 15:42:41.000000 dock-cli-0.3.0/dock_cli.egg-info/PKG-INFO
--rw-r--r--   0 posen      (501) staff       (20)      483 2024-03-30 15:42:41.000000 dock-cli-0.3.0/dock_cli.egg-info/SOURCES.txt
--rw-r--r--   0 posen      (501) staff       (20)        1 2024-03-30 15:42:41.000000 dock-cli-0.3.0/dock_cli.egg-info/dependency_links.txt
--rw-r--r--   0 posen      (501) staff       (20)       43 2024-03-30 15:42:41.000000 dock-cli-0.3.0/dock_cli.egg-info/entry_points.txt
--rw-r--r--   0 posen      (501) staff       (20)       13 2024-03-30 15:42:41.000000 dock-cli-0.3.0/dock_cli.egg-info/requires.txt
--rw-r--r--   0 posen      (501) staff       (20)        9 2024-03-30 15:42:41.000000 dock-cli-0.3.0/dock_cli.egg-info/top_level.txt
--rw-r--r--   0 posen      (501) staff       (20)       38 2024-03-30 15:42:41.402111 dock-cli-0.3.0/setup.cfg
--rw-r--r--   0 posen      (501) staff       (20)      619 2024-03-30 08:12:01.000000 dock-cli-0.3.0/setup.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.916898 dock-cli-0.3.1/
+-rw-r--r--   0 posen      (501) staff       (20)     1062 2024-03-05 06:48:54.000000 dock-cli-0.3.1/LICENSE
+-rw-r--r--   0 posen      (501) staff       (20)     1957 2024-04-02 07:58:38.916599 dock-cli-0.3.1/PKG-INFO
+-rw-r--r--   0 posen      (501) staff       (20)     1693 2024-03-25 15:48:25.000000 dock-cli-0.3.1/README.md
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.911925 dock-cli-0.3.1/dock_cli/
+-rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/__init__.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.913801 dock-cli-0.3.1/dock_cli/cli/
+-rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/cli/__init__.py
+-rw-r--r--   0 posen      (501) staff       (20)     3934 2024-04-01 06:10:49.000000 dock-cli-0.3.1/dock_cli/cli/chart.py
+-rw-r--r--   0 posen      (501) staff       (20)     5507 2024-04-01 06:10:50.000000 dock-cli-0.3.1/dock_cli/cli/image.py
+-rw-r--r--   0 posen      (501) staff       (20)     2246 2024-04-01 06:39:15.000000 dock-cli-0.3.1/dock_cli/main.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.915929 dock-cli-0.3.1/dock_cli/utils/
+-rw-r--r--   0 posen      (501) staff       (20)        0 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/utils/__init__.py
+-rw-r--r--   0 posen      (501) staff       (20)      797 2024-04-01 14:33:14.000000 dock-cli-0.3.1/dock_cli/utils/callback.py
+-rw-r--r--   0 posen      (501) staff       (20)      629 2024-03-21 16:14:08.000000 dock-cli-0.3.1/dock_cli/utils/commands.py
+-rw-r--r--   0 posen      (501) staff       (20)     4767 2024-04-02 03:20:25.000000 dock-cli-0.3.1/dock_cli/utils/helpers.py
+-rw-r--r--   0 posen      (501) staff       (20)      530 2024-04-02 03:22:43.000000 dock-cli-0.3.1/dock_cli/utils/schema.py
+-rw-r--r--   0 posen      (501) staff       (20)     2021 2024-04-01 06:22:14.000000 dock-cli-0.3.1/dock_cli/utils/utils.py
+drwxr-xr-x   0 posen      (501) staff       (20)        0 2024-04-02 07:58:38.916279 dock-cli-0.3.1/dock_cli.egg-info/
+-rw-r--r--   0 posen      (501) staff       (20)     1957 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/PKG-INFO
+-rw-r--r--   0 posen      (501) staff       (20)      483 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 posen      (501) staff       (20)        1 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 posen      (501) staff       (20)       43 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/entry_points.txt
+-rw-r--r--   0 posen      (501) staff       (20)       13 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/requires.txt
+-rw-r--r--   0 posen      (501) staff       (20)        9 2024-04-02 07:58:38.000000 dock-cli-0.3.1/dock_cli.egg-info/top_level.txt
+-rw-r--r--   0 posen      (501) staff       (20)       38 2024-04-02 07:58:38.916949 dock-cli-0.3.1/setup.cfg
+-rw-r--r--   0 posen      (501) staff       (20)      619 2024-04-01 06:46:51.000000 dock-cli-0.3.1/setup.py
```

### Comparing `dock-cli-0.3.0/LICENSE` & `dock-cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.0/PKG-INFO` & `dock-cli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock-cli-0.3.0/README.md` & `dock-cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.0/dock_cli/cli/chart.py` & `dock-cli-0.3.1/dock_cli/cli/chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,32 +63,32 @@
 def config_cli(ctx):
     """Manage charts' configuration
 
     This is a command line interface for manage charts' configuration
     """
     if ctx.invoked_subcommand is None:
         for section in ctx.obj.helper.get_charts():
-            utils.print_chart_config(section)
+            utils.print_chart_config(ctx.obj.config, section)
 
 @config_cli.command(name='init',
                     help='Initialize chart default settings in the configuration')
 @click.pass_obj
 @click.option('--registry', required=False, type=str, default='oci://registry-1.docker.io/namespace', show_default=True,
               help='Default oci registry for all charts.')
 def config_init(obj, registry):
-    utils.set_config_option(configparser.DEFAULTSECT, Chart.REGISTRY, registry)
+    utils.set_config_option(obj.config, configparser.DEFAULTSECT, Chart.REGISTRY, registry)
     for section in obj.helper.get_charts():
-        utils.print_chart_config(section)
+        utils.print_chart_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
 
 @config_cli.command(name='add',
                     help='Add or update an chart section in the configuration')
 @click.pass_obj
 @click.argument('section', required=True, type=click.Path(exists=True, file_okay=False),
                 callback=cb.transform_to_section)
 def config_set(obj, section):
     if obj.config.has_section(section) is False:
         obj.config.add_section(section)
-    utils.set_config_option(section, Chart.TYPE, SectionType.CHART)
+    utils.set_config_option(obj.config, section, Chart.TYPE, SectionType.CHART)
     obj.helper.validate_section(section)
-    utils.print_chart_config(section)
+    utils.print_chart_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
```

### Comparing `dock-cli-0.3.0/dock_cli/cli/image.py` & `dock-cli-0.3.1/dock_cli/cli/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,25 +81,25 @@
 def config_cli(ctx):
     """Manage images' configuration
 
     This is a command line interface for manage images' configuration
     """
     if ctx.invoked_subcommand is None:
         for section in ctx.obj.helper.get_images():
-            utils.print_image_config(section)
+            utils.print_image_config(ctx.obj.config, section)
 
 @config_cli.command(name='init',
                     help='Initialize image default settings in the configuration')
 @click.pass_obj
 @click.option('--registry', required=False, type=str, default='namespace',
               help='Default registry for all images.')
 def config_init(obj, registry):
-    utils.set_config_option(configparser.DEFAULTSECT, Image.REGISTRY, registry)
+    utils.set_config_option(obj.config, configparser.DEFAULTSECT, Image.REGISTRY, registry)
     for section in obj.helper.get_images():
-        utils.print_image_config(section)
+        utils.print_image_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
 
 @config_cli.command(name='add',
                     help='Add or update an image section in the configuration')
 @click.pass_obj
 @click.argument('section', required=True, type=click.Path(exists=True, file_okay=False),
                 callback=cb.transform_to_section)
@@ -111,14 +111,14 @@
               type=click.Path(exists=True, file_okay=False),
               callback=cb.multiline_sections,
               help='List of sections or paths that this section depends on.')
 def config_add(obj, section, file, name, depends_on):
     # pylint: disable=too-many-arguments
     if obj.config.has_section(section) is False:
         obj.config.add_section(section)
-    utils.set_config_option(section, Image.FILE, file)
-    utils.set_config_option(section, Image.NAME, name)
-    utils.set_config_option(section, Image.DEPENDS_ON, depends_on)
-    utils.set_config_option(section, Image.TYPE, SectionType.IMAGE)
+    utils.set_config_option(obj.config, section, Image.FILE, file)
+    utils.set_config_option(obj.config, section, Image.NAME, name)
+    utils.set_config_option(obj.config, section, Image.DEPENDS_ON, depends_on)
+    utils.set_config_option(obj.config, section, Image.TYPE, SectionType.IMAGE)
     obj.helper.validate_section(section)
-    utils.print_image_config(section)
+    utils.print_image_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
```

### Comparing `dock-cli-0.3.0/dock_cli/main.py` & `dock-cli-0.3.1/dock_cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,18 +37,15 @@
 @click.version_option(package_name='dock-cli')
 def cli(ctx, config_file, log_level, docker, helm, git):
     # pylint: disable=too-many-arguments
     logging.basicConfig(level=getattr(logging, log_level.upper()),
                         format='[%(levelname)s] %(message)s')
 
     ctx.ensure_object(types.SimpleNamespace)
-    ctx.obj.command = hlp.Command()
-    ctx.obj.command.docker = ctx.obj.command.docker if docker is None else docker
-    ctx.obj.command.helm = ctx.obj.command.helm if helm is None else helm
-    ctx.obj.command.git = ctx.obj.command.git if git is None else git
+    ctx.obj.command = hlp.Command(docker, helm, git)
 
     logging.getLogger(__name__).debug('Reading configuration from %s', config_file)
     ctx.obj.config = configparser.ConfigParser()
     ctx.obj.config.read(config_file)
     ctx.obj.config_dir = pathlib.Path(config_file).parent.as_posix()
     ctx.obj.config_file = config_file
```

### Comparing `dock-cli-0.3.0/dock_cli/utils/commands.py` & `dock-cli-0.3.1/dock_cli/utils/commands.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.0/dock_cli/utils/helpers.py` & `dock-cli-0.3.1/dock_cli/utils/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,24 @@
 from dock_cli.utils import commands as cmd
 from dock_cli.utils.schema import ChartConfigOptions as Chart, ImageConfigOptions as Image, SectionType
 from dock_cli.utils.utils import topological_sort
 
 
 @dataclasses.dataclass()
 class Command():
-    docker: str = 'docker'
-    helm: str = 'helm'
-    git: str = 'git'
+    __slots__ = ['docker', 'helm', 'git']
+
+    docker: str
+    helm: str
+    git: str
+
+    def __post_init__(self):
+        self.docker = 'docker' if self.docker is None else self.docker
+        self.helm = 'helm' if self.helm is None else self.helm
+        self.git = 'git' if self.git is None else self.git
 
 
 class OrderedGroup(click.Group):
     def list_commands(self, _ctx):
         return self.commands
```

### Comparing `dock-cli-0.3.0/dock_cli/utils/schema.py` & `dock-cli-0.3.1/dock_cli/utils/schema.py`

 * *Files identical despite different names*

### Comparing `dock-cli-0.3.0/dock_cli/utils/utils.py` & `dock-cli-0.3.1/dock_cli/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,41 +4,37 @@
 from dock_cli.utils.schema import ImageConfigOptions as Image, ChartConfigOptions as Chart
 
 def update_config(config, config_file):
     logging.getLogger(__name__).debug('Updating configuration to %s', config_file)
     with open(config_file, 'w', encoding='utf-8') as fp:
         config.write(fp)
 
-@click.pass_obj
-def to_section(obj, value):
-    section = pathlib.Path(value).resolve().relative_to(obj.config_dir).as_posix()
+def to_section(config_dir, value):
+    section = pathlib.Path(value).resolve().relative_to(config_dir).as_posix()
     logging.getLogger(__name__).debug('Transform value `%s` to section `%s`', value, section)
     return section
 
-@click.pass_obj
-def set_config_option(obj, section, option, value=None):
+def set_config_option(config, section, option, value=None):
     logging.getLogger(__name__).debug('Removing section [%s] option `%s`', section, option)
-    obj.config.remove_option(section, option)
+    config.remove_option(section, option)
     if value:
         logging.getLogger(__name__).debug('Setting section [%s] option `%s` to `%s`', section, option, value)
-        obj.config.set(section, option, value)
+        config.set(section, option, value)
         click.echo(f'Set [{section}] {option} = {value}')
 
-@click.pass_obj
-def print_image_config(obj, section):
+def print_image_config(config, section):
     click.echo(f"{click.style(section, fg='bright_cyan')}:")
     for option in Image:
-        value = ' '.join(obj.config.get(section, option, fallback='').strip().splitlines())
+        value = ' '.join(config.get(section, option, fallback='').strip().splitlines())
         click.echo(f"- {click.style(option, fg='green')}: {click.style(value, fg='yellow')}")
 
-@click.pass_obj
-def print_chart_config(obj, section):
+def print_chart_config(config, section):
     click.echo(f"{click.style(section, fg='bright_cyan')}:")
     for option in Chart:
-        value = ' '.join(obj.config.get(section, option, fallback='').strip().splitlines())
+        value = ' '.join(config.get(section, option, fallback='').strip().splitlines())
         click.echo(f"- {click.style(option, fg='green')}: {click.style(value, fg='yellow')}")
 
 def topological_sort(dependencies):
     visited = set()
     result = []
 
     def dfs(node):
```

### Comparing `dock-cli-0.3.0/dock_cli.egg-info/PKG-INFO` & `dock-cli-0.3.1/dock_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock-cli-0.3.0/setup.py` & `dock-cli-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='dock-cli',
-    version='0.3.0',
+    version='0.3.1',
     author='Posen',
     author_email='posen2101024@gmail.com',
     description='CLI for manage container applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
```

