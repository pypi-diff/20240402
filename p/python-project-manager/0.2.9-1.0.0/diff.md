# Comparing `tmp/python-project-manager-0.2.9.tar.gz` & `tmp/python-project-manager-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-project-manager-0.2.9.tar", last modified: Sat Mar 30 01:08:03 2024, max compression
+gzip compressed data, was "python-project-manager-1.0.0.tar", last modified: Tue Apr  2 04:44:21 2024, max compression
```

## Comparing `python-project-manager-0.2.9.tar` & `python-project-manager-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 01:08:03.025885 python-project-manager-0.2.9/
--rw-rw-rw-   0        0        0    35821 2024-03-20 03:20:34.000000 python-project-manager-0.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0      226 2024-03-30 01:08:03.022883 python-project-manager-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-19 02:00:26.000000 python-project-manager-0.2.9/README.md
--rw-rw-rw-   0        0        0     1061 2024-03-30 01:07:56.000000 python-project-manager-0.2.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-30 01:08:02.984877 python-project-manager-0.2.9/python_project_manager/
--rw-rw-rw-   0        0        0       97 2024-03-28 01:20:11.000000 python-project-manager-0.2.9/python_project_manager/__init__.py
--rw-rw-rw-   0        0        0    11316 2024-03-30 01:01:50.000000 python-project-manager-0.2.9/python_project_manager/app.py
-drwxrwxrwx   0        0        0        0 2024-03-30 01:08:03.018883 python-project-manager-0.2.9/python_project_manager/builtin_engines/
--rw-rw-rw-   0        0        0        0 2024-03-28 01:35:55.000000 python-project-manager-0.2.9/python_project_manager/builtin_engines/__init__.py
--rw-rw-rw-   0        0        0     4971 2024-03-30 01:07:51.000000 python-project-manager-0.2.9/python_project_manager/builtin_engines/builtin_setuptools.py
--rw-rw-rw-   0        0        0     3352 2024-03-29 02:56:46.000000 python-project-manager-0.2.9/python_project_manager/config.py
-drwxrwxrwx   0        0        0        0 2024-03-30 01:08:03.020884 python-project-manager-0.2.9/python_project_manager.egg-info/
--rw-rw-rw-   0        0        0      226 2024-03-30 01:08:02.000000 python-project-manager-0.2.9/python_project_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2024-03-30 01:08:02.000000 python-project-manager-0.2.9/python_project_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 01:08:02.000000 python-project-manager-0.2.9/python_project_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      691 2024-03-30 01:08:02.000000 python-project-manager-0.2.9/python_project_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-03-30 01:08:02.000000 python-project-manager-0.2.9/python_project_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-03-30 01:08:02.000000 python-project-manager-0.2.9/python_project_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      550 2024-03-30 00:11:22.000000 python-project-manager-0.2.9/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2024-03-30 00:10:25.000000 python-project-manager-0.2.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 01:08:03.025885 python-project-manager-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 04:44:21.919062 python-project-manager-1.0.0/
+-rw-rw-rw-   0        0        0    35821 2024-03-20 03:20:34.000000 python-project-manager-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      226 2024-04-02 04:44:21.917062 python-project-manager-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-19 02:00:26.000000 python-project-manager-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1061 2024-04-02 04:44:16.000000 python-project-manager-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-02 04:44:21.876275 python-project-manager-1.0.0/python_project_manager/
+-rw-rw-rw-   0        0        0       97 2024-03-28 01:20:11.000000 python-project-manager-1.0.0/python_project_manager/__init__.py
+-rw-rw-rw-   0        0        0    11788 2024-04-02 03:53:43.000000 python-project-manager-1.0.0/python_project_manager/app.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:44:21.903056 python-project-manager-1.0.0/python_project_manager/builtin_engines/
+-rw-rw-rw-   0        0        0        0 2024-03-28 01:35:55.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/__init__.py
+-rw-rw-rw-   0        0        0     1442 2024-04-02 04:39:44.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/builtin_pyinstaller.py
+-rw-rw-rw-   0        0        0     4606 2024-04-02 04:17:00.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/builtin_setuptools.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:44:21.913062 python-project-manager-1.0.0/python_project_manager/builtin_engines/toml/
+-rw-rw-rw-   0        0        0      960 2024-03-31 20:20:09.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/toml/__init__.py
+-rw-rw-rw-   0        0        0    38938 2024-03-31 20:20:17.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/toml/decoder.py
+-rw-rw-rw-   0        0        0     9936 2024-03-31 20:20:20.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/toml/encoder.py
+-rw-rw-rw-   0        0        0      362 2024-03-31 20:20:38.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/toml/ordered.py
+-rw-rw-rw-   0        0        0      701 2024-03-31 20:11:59.000000 python-project-manager-1.0.0/python_project_manager/builtin_engines/toml/tz.py
+-rw-rw-rw-   0        0        0     3352 2024-03-29 02:56:46.000000 python-project-manager-1.0.0/python_project_manager/config.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:44:21.915062 python-project-manager-1.0.0/python_project_manager.egg-info/
+-rw-rw-rw-   0        0        0      226 2024-04-02 04:44:21.000000 python-project-manager-1.0.0/python_project_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      895 2024-04-02 04:44:21.000000 python-project-manager-1.0.0/python_project_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:44:21.000000 python-project-manager-1.0.0/python_project_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      691 2024-04-02 04:44:21.000000 python-project-manager-1.0.0/python_project_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-02 04:44:21.000000 python-project-manager-1.0.0/python_project_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-02 04:44:21.000000 python-project-manager-1.0.0/python_project_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      536 2024-03-31 20:00:35.000000 python-project-manager-1.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2024-03-31 20:12:35.000000 python-project-manager-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:44:21.919062 python-project-manager-1.0.0/setup.cfg
```

### Comparing `python-project-manager-0.2.9/LICENSE.txt` & `python-project-manager-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-project-manager-0.2.9/pyproject.toml` & `python-project-manager-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "python-project-manager"
 description = "A Python package."
 authors = []
 readme = "README.md"
 keywords = []
-version = "0.2.9"
+version = "1.0.0"
 dynamic = [ "dependencies",]
 
 [project.scripts]
 ppm = "python_project_manager.app:cli"
 ppm-builtin-setuptools-build = "python_project_manager.builtin_engines.builtin_setuptools:_build"
 ppm-builtin-setuptools-install = "python_project_manager.builtin_engines.builtin_setuptools:_install"
 ppm-builtin-setuptools-uninstall = "python_project_manager.builtin_engines.builtin_setuptools:_uninstall"
```

### Comparing `python-project-manager-0.2.9/python_project_manager/app.py` & `python-project-manager-1.0.0/python_project_manager/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import importlib
 import os
 import re
+from types import ModuleType
 from typing import Any, Callable
 import click
 from python_project_manager import Config
 
 VENV = f'venv\\Scripts\\activate'
 
 def sanitize_string_for_file(string: str) -> str:
@@ -37,18 +38,16 @@
     sanitized_string = string.strip()
     sanitized_string = re.sub(r' ', '_', sanitized_string)
     return sanitized_string
 
 def pass_command_to_engine(_command: str, _method: Callable[..., bool], **_kwargs) -> bool:
     try:
     # built-in engines
-        if Config.get('engine', '').startswith('ppm-builtin-setuptools'):
-            engine = importlib.import_module('python_project_manager.builtin_engines.builtin_setuptools')
-        else:
-            engine = importlib.import_module(sanitize_string_for_file(Config.get('engine', _kwargs.get('__engine', ''))))
+        
+        engine = get_engine(_kwargs.get('_engine', Config.get('engine')))
         method: Callable[..., bool] = getattr(engine, _command, None)
         if method:
             keep_processing = method(_method, **_kwargs)
             # If keep_processing is None or True, continue processing
             if keep_processing is None or keep_processing:
                 return _method(**_kwargs)
         else:
@@ -56,73 +55,78 @@
 
     except Exception as e:
         if Config.get('engine') == '':
             return _method(**_kwargs)
         else:
             raise e
 
+def get_engine(engine_name: str) -> ModuleType | None:
+    if engine_name == None or engine_name == '':
+        return None
+    match engine_name:
+        case 'ppm-builtin-setuptools': # Built-in engine
+            return importlib.import_module('.builtin_engines.builtin_setuptools', package='python_project_manager')
+        case 'ppm-builtin-pyinstaller': # Built-in engine
+            return importlib.import_module('.builtin_engines.builtin_pyinstaller', package='python_project_manager')
+        case _: # External engine
+            return importlib.import_module(sanitize_string_for_file(engine_name))
+        
 @click.group()
 def cli():
     pass
 
 @cli.command()
 @click.argument('project_name', type=str, required=True)
-@click.option('--engine', '-e', type=str, default='ppm-builtin-setuptools', help='Choose the engine \'module\' to use')
+@click.option('--engine', '-e', type=str, default='',
+    help='Choose the engine \'module\' to use. Built in engines are \'ppm-builtin-setuptools\' and \'ppm-builtin-pyinstaller\'.')
 @click.option('--force', '-f', is_flag=True, help='Force initialization of the project')
 # @click.option('--python', '-p', type=str, default='', help='Python version to use')
 def init(project_name: str, engine: str, force: bool) -> None:
     '''
     <project_name> - Name of the project to be setup
     '''
-    # Verify project can be initialized with the given parameters
-    if pass_command_to_engine('verify', _verify,
-        force=force, project_name=project_name, __engine=engine):
-
-        # Even though the looks like it belongs in the '_init' method,
-        # it is placed here so external engines can not stop nessary files from being created
-
-        # Set the project name and engine
-        Config.set('project_name', project_name)
-        Config.set('engine', engine)
-        Config.save()
-
-        # Create the requirements.txt and requirements-dev.txt files
-        with open(os.path.join(os.getcwd(), 'requirements.txt'), 'w') as file:
-            pass
-        with open(os.path.join(os.getcwd(), 'requirements-dev.txt'), 'w') as file:
-            pass
-
-        # Create the venv
-        os.system('python -m venv venv')
-    
-        # Initialize the project
-        pass_command_to_engine('init', _init,
-            project_name=project_name, engine=engine)
-
-def _verify(**kwargs) -> bool:
-    force: bool = kwargs.get('force', None)
-    engine: str = kwargs.get('engine', None)
-
     # Check if the project has already been initialized
     if not force and Config.load():
         print('Project already initialized')
         return False
     
-    # Check if the engine if not empty and not a built-in engine
-    if engine != '' and not engine.startswith('ppm-builtin'):
-        try:
-            importlib.import_module(sanitize_string_for_file(Config.get('engine')))
-        except Exception as e:
-            print(f"Engine '{engine}': Error: {e}")
-            return False
+    # Check if the engine is available
+    try:
+        get_engine(engine)
+    except ImportError:
+        print(f"Engine '{engine}' not found")
+        return False
 
-    return True
+    # Even though the looks like it belongs in the '_init' method,
+    # it is placed here so external engines can not stop nessary files from being created
+
+    # Set the project name and engine
+    Config.set('project_name', project_name)
+    Config.set('engine', engine)
+    Config.set('src_dir', 'src')
+    Config.set('version', '0.0.0')
+    Config.save()
+
+    # Create the requirements.txt and requirements-dev.txt files
+    with open(os.path.join(os.getcwd(), 'requirements.txt'), 'w') as file:
+        pass
+    with open(os.path.join(os.getcwd(), 'requirements-dev.txt'), 'w') as file:
+        pass
+
+    # Create the venv
+    os.system('python -m venv venv')
+
+    # Initialize the project
+    pass_command_to_engine('init', _init,
+        project_name=project_name, engine=engine)
 
 def _init(**kwargs) -> bool:
     src_dir = os.path.join(os.getcwd(), Config.get('src_dir'))
+    Config.set('scripts.start', f'py -m %src_dir%.app')
+    Config.save()
     os.makedirs(src_dir, exist_ok=True)
     return True
 
 @cli.command()
 @click.argument('script_name', type=str, required=True)
 def run(script_name) -> None:
     '''
@@ -137,15 +141,15 @@
 def _run(**kwargs) -> bool:
     cli_command: str = kwargs.get('cli_command', None)
     script_name: str = kwargs.get('script_name', None)
 
     if not cli_command:
         print(f"Script '{script_name}' not found")
         return
-    
+
     ## Smart change directory
     cwd = os.getcwd() # Get the current working directory
 
     # Check if the command has a change directory command
     has_change_directory_command = re.search(r'(^|\s)cd\s\w*', cli_command)
     if not has_change_directory_command:
         # Searches for the 'python' command along with the script path
@@ -158,43 +162,47 @@
                 targ_dir = re.search(r'^\w*(.|\|/)(?!py)', python_path[0])
                 if targ_dir:
                     # Join the target dir with the current working directory
                     cwd = os.path.join(cwd, targ_dir[0][:-1])
                     # Remove targ_dir from python_path
                     cli_command = cli_command.replace(python_path[0],python_path[0].replace(targ_dir[0], ""))
                     if targ_dir[0][:-1] == Config.get('test_dir'):
-                        cli_command = f'set PYTHONPATH=C:\{Config.get('src_dir')};%PYTHONPATH% && {cli_command}'
+                        cli_command = f'set PYTHONPATH=C:\\{Config.get('src_dir')};%PYTHONPATH% && {cli_command}'
                         
     os.chdir(cwd) # Change the current working directory
     os.system(f'{VENV} && {cli_command}') # Run the command
 
 @cli.command()
-@click.argument('action', type=click.Choice(['inc', 'dec', 'show', 'set']), required=True, default='show')
+@click.argument('action', type=click.Choice(['inc', 'dec', 'show', 'set', 'sync']), required=True, default='show')
 @click.option('--major', '-M', type=int, default=0, help='Change the major version')
 @click.option('--minor', '-m', type=int, default=0, help='Change the minor version')
 @click.option('--patch', '-p', type=int, default=0, help='Change the patch version')
 @click.option('--timestamp', '-t', is_flag=True, help='Include timestamp in the version')
 def version(action, major, minor, patch, timestamp) -> None:
     '''
     <action> - Action to perform on the version
-    '''       
+    '''
     if action == 'show':
         print(Config.get('version'))
         return
 
     pass_command_to_engine('version', _version,
         action=action, major=major, minor=minor, patch=patch, timestamp=timestamp)
 
 def _version(**kwargs) -> bool:
     action: str = kwargs.get('action', None)
+    if action == 'sync':
+        print('No built-in sync action, external engine sync action may have been called')
+        return True
+    
     major: str = kwargs.get('major', None)
     minor: str = kwargs.get('minor', None)
     patch: str = kwargs.get('patch', None)
     timestamp: str = kwargs.get('timestamp', None)
-    
+
     # Split the version by '.' and '+'
     version_list = re.split(r'\.', Config.get('version'))
     ver_major = int(version_list[0])
     ver_minor = int(version_list[1])
     ver_patch = int(version_list[2])
     ver_timestamp = version_list[3] if len(version_list) > 3 else ''
 
@@ -234,61 +242,63 @@
 
     print(f'Version: {Config.get('version')} -> {version}')
     Config.set('version', version)
     Config.save()
     return True
 
 # Pip commands
-@cli.command(context_settings=dict(
-    ignore_unknown_options=True
-))
+@cli.command(context_settings=dict(ignore_unknown_options=True))
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.option('--help', '-h', is_flag=True) # Allows '--help' to be passed as an argument
 def list(args, help) -> None:
     '''
     Uses pip's 'list' command
     '''
     if help:
         os.system(f'{VENV} && pip list --help')
     else:
         os.system(f'{VENV} && pip list {' '.join(args)}')
 
-@cli.command(context_settings=dict(
-    ignore_unknown_options=True
-))
+@cli.command(context_settings=dict(ignore_unknown_options=True))
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
 @click.option('--dev', '-d', is_flag=True) # Add the package to the dev requirements
 @click.option('--help', '-h', is_flag=True) # Allows '--help' to be passed as an argument
 def install(args, help, dev) -> None:
     '''
     Uses pip's 'install' command
     '''
+    # Create the command
+    cmd = f'{VENV} && pip install {" ".join(args)}'.strip()
+
+    # If 'pip install pip' is passed, install pip
+    if cmd == f'{VENV} && pip install pip':
+        os.system(f'{VENV} && python -m ensurepip')
+        return
+
+    # Use the help command if the '--help' flag is passed
     if help:
         os.system(f'{VENV} && pip install --help')
         return
-    
-    cmd = f'{VENV} && pip install {" ".join(args)}'
 
-    if cmd.strip() == f'{VENV} && pip install':
+    # If no arguments are passed, install the requirements
+    if cmd == f'{VENV} && pip install':
         os.system(f'{VENV} && pip install -r requirements.txt -r requirements-dev.txt')
 
-    try:
-        output = os.popen(cmd)
-
-        # Read and print each line of the output
-        for line in output:
-            print(line.strip())
-            if 'Successfully installed' in line:
-                update_requirements(line.strip(), dev)
+    # Otherwise, install the packages
+    output = os.popen(cmd)
 
-        # Close the output stream
-        output.close()
+    # Read and print each line of the output
+    for line in output:
+        print(line.strip())
+        if 'Successfully installed' in line:
+            # Update the requirements file
+            update_requirements(line.strip(), dev)
 
-    except Exception as e:
-        print(f"An error occurred: {e}")
+    # Close the output stream
+    output.close()
     
 def update_requirements(packages_to_update: str, is_dev=False) -> None:
     requirement_file = 'requirements-dev.txt' if is_dev else 'requirements.txt'
     packages_to_update = packages_to_update.replace('Successfully installed ', '').split(' ')
     packages_to_update = [re.split(r'-(?=[^-]*$)', package) for package in packages_to_update]
     packages_to_update = [(package[0], package[1]) for package in packages_to_update]
```

### Comparing `python-project-manager-0.2.9/python_project_manager/builtin_engines/builtin_setuptools.py` & `python-project-manager-1.0.0/python_project_manager/builtin_engines/builtin_setuptools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import os
-import toml
+import re
+from .toml import load as toml_load, dump as toml_dump
 from python_project_manager import Config, sanitize_string_for_file, sanitize_string_for_module
 
 SetuptoolsEngineConfig = {
     'username': '',
     'password': '',
     'wheel': ''
 }
 
-def verify(_method, **_kwargs) -> bool:
-    force: bool = _kwargs.get('force', False)
-    if force: # If the force flag is set, the engine will be verified regardless of the packages installed
-        return True
-    
-    missing_packages = []
-    for package in ['toml', 'build', 'twine', 'setuptools']:
-        try:
-            __import__(package)
-        except ImportError:
-            missing_packages.append(package)
-
-    if missing_packages:
-        print('The following packages are required to use the Setuptools engine:')
-        for package in missing_packages:
-            print(f' - {package}')
-        return False
-    
-    return True
-
-def init(_method, **_kwargs) -> bool:
+def init(_method, **kwargs) -> bool:
+    os.system('ppm install build==1.2.1 twine==5.0.0 setuptools==69.2.0 --dev')
     edit_config()
     create_template_app()
     set_default_scripts()
     create_files()
     return False
 
-def version(_method, **_kwargs) -> bool:
-    _method(**_kwargs)
+def version(_method, **kwargs) -> bool:
+    action: str = kwargs.get('action', None)
+    if action == 'sync':
+        try:
+            output = os.popen(f'pip index versions {Config.get("project_name")}')
+            for line in output:
+                print(line.strip())
+                version_number = re.search(r'\((\d|\.)*\)', line)
+                if version_number:
+                    pypi_version = version_number.group(0)[1:-1]
+            output.close()
+            
+            print(f'Version: {Config.get('version')} -> {pypi_version}')
+            Config.set('version', pypi_version)
+            Config.save()
+        except Exception as e:
+            print(f'Error: {e}')
+    else:
+        _method(**kwargs)
+
     toml_file = load_toml()
     toml_file['project']['version'] = Config.get('version')
     save_toml(toml_file)
     return False
 
 def edit_config() -> None:
     Config.set('src_dir', sanitize_string_for_file(Config.get('project_name')))
@@ -58,18 +58,16 @@
         f.write('    print(os.getcwd())\n')
         f.write('    print("Hello World.")\n\n')
         f.write('if __name__ == "__main__":\n')
         f.write('    app()')
 
 def set_default_scripts() -> None:
     default_scripts = {
-        'start': f'py -m %src_dir%.app',
+        'start': f'python -m %src_dir%.app',
         'build': f'ppm-builtin-setuptools-build',
-        'install': f'ppm-builtin-setuptools-install',
-        'uninstall': f'ppm-builtin-setuptools-uninstall',
         'publish-major': f'ppm-builtin-setuptools-publish-major',
         'publish-minor': f'ppm-builtin-setuptools-publish-minor',
         'publish-patch': f'ppm-builtin-setuptools-publish-patch'
     }
     Config.set('scripts', default_scripts)
     Config.save()
 
@@ -78,15 +76,15 @@
         'build-system': {
             'requires': ['setuptools', 'wheel'],
             'build-backend': 'setuptools.build_meta'
         },
 
         'project': {
             'name': sanitize_string_for_module(Config.get('project_name')),
-            'version': Config.get('version', '0.0.0'),
+            'version': Config.get('version'),
             'description': 'A Python package.',
             'authors': [],
             'readme': 'README.md',
             'keywords': [],
             'dynamic': ['dependencies']
         },
         
@@ -97,38 +95,33 @@
                         'file': ['requirements.txt']
                     }
                 }
             }
         }
     }
     with open('pyproject.toml', 'w') as f:
-        toml.dump(toml_config, f)
+        toml_dump(toml_config, f)
     with open('LICENSE.txt', 'w') as f:
         pass
     with open('README.md', 'w') as f:
         pass
     
 def load_toml() -> dict:
     with open('pyproject.toml', 'r') as f:
-        return toml.load(f)
+        return toml_load(f)
     
 def save_toml(toml_config) -> None:
     with open('pyproject.toml', 'w') as f:
-        toml.dump(toml_config, f)
+        toml_dump(toml_config, f)
 
 # Setuptools Engine built-in cli commands
 # Allows for shorthand commands to be used in the cli
-_publish_command = 'del /S /Q %dist_dir%\\* && python -m build && twine upload -u %twine.username% -p %twine.password% -r pypi %dist_dir%/*'
+_publish_command = f'del /S /Q %dist_dir%\\* && python -m build && twine upload -u %twine.username% -p %twine.password% -r pypi %dist_dir%/*'
+VENV = f'venv\\Scripts\\activate'
 def _build():
     os.system(Config.parse(f'ppm version inc -t && python -m build', Config._value_config))
-def _install():
-    os.system(Config.parse(f'pip install %dist_dir%/%twine.wheel%-%version%-py3-none-any.whl --force-reinstall', Config._value_config))
-def _uninstall():
-    os.system(Config.parse(f'pip uninstall %dist_dir%/%twine.wheel%-%version%-py3-none-any.whl', Config._value_config))
-def _publish():
-    os.system(Config.parse(f'del /S /Q %dist_dir%\\* && python -m build && twine upload -u %twine.username% -p %twine.password% -r pypi %dist_dir%/*', Config._value_config))
 def _publish_patch():
-    os.system(Config.parse(f'ppm version inc -p 1 && {_publish_command}', Config._value_config))
+    os.system(Config.parse(f'ppm version sync && ppm version inc -p 1 && {_publish_command}', Config._value_config))
 def _publish_minor():
-    os.system(Config.parse(f'ppm version inc -m 1 && {_publish_command}', Config._value_config))
+    os.system(Config.parse(f'ppm version sync && ppm version inc -m 1 && {_publish_command}', Config._value_config))
 def _publish_major():
-    os.system(Config.parse(f'ppm version inc -M 1 && {_publish_command}', Config._value_config))
+    os.system(Config.parse(f'ppm version sync && ppm version inc -M 1 && {_publish_command}', Config._value_config))
```

### Comparing `python-project-manager-0.2.9/python_project_manager/config.py` & `python-project-manager-1.0.0/python_project_manager/config.py`

 * *Files identical despite different names*

### Comparing `python-project-manager-0.2.9/python_project_manager.egg-info/entry_points.txt` & `python-project-manager-1.0.0/python_project_manager.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-project-manager-0.2.9/requirements-dev.txt` & `python-project-manager-1.0.0/requirements-dev.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,11 +19,10 @@
 pywin32-ctypes~=0.2.2
 readme-renderer~=43.0
 requests-toolbelt~=1.0.0
 requests~=2.31.0
 rfc3986~=2.0.0
 rich~=13.7.1
 setuptools~=69.2.0
-toml~=0.10.2
 twine~=5.0.0
 urllib3~=2.2.1
 zipp~=3.18.1
```

