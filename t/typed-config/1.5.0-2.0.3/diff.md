# Comparing `tmp/typed-config-1.5.0.tar.gz` & `tmp/typed-config-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-config-1.5.0.tar", last modified: Tue Apr  2 10:50:01 2024, max compression
+gzip compressed data, was "typed-config-2.0.3.tar", last modified: Tue Apr  2 15:23:31 2024, max compression
```

## Comparing `typed-config-1.5.0.tar` & `typed-config-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.658566 typed-config-1.5.0/
--rw-rw-rw-   0        0        0     1089 2019-03-11 17:34:14.000000 typed-config-1.5.0/LICENSE
--rw-rw-rw-   0        0        0    28620 2024-04-02 10:50:01.655460 typed-config-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    27620 2024-04-02 10:48:08.000000 typed-config-1.5.0/README.md
--rw-rw-rw-   0        0        0       33 2022-11-28 09:33:43.000000 typed-config-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 10:50:01.658566 typed-config-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1461 2022-11-14 18:44:22.000000 typed-config-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.593168 typed-config-1.5.0/test/
--rw-rw-rw-   0        0        0     3032 2024-03-28 16:14:10.000000 typed-config-1.5.0/test/test_casts.py
--rw-rw-rw-   0        0        0     2994 2024-04-02 10:42:42.000000 typed-config-1.5.0/test/test_config_source.py
--rw-rw-rw-   0        0        0    16510 2022-12-01 14:30:40.000000 typed-config-1.5.0/test/test_configuration.py
--rw-rw-rw-   0        0        0      395 2021-11-03 10:30:42.000000 typed-config-1.5.0/test/test_version.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.621997 typed-config-1.5.0/typed_config.egg-info/
--rw-rw-rw-   0        0        0    28620 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-02 10:50:01.000000 typed-config-1.5.0/typed_config.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 10:50:01.652938 typed-config-1.5.0/typedconfig/
--rw-rw-rw-   0        0        0       52 2019-03-11 17:20:46.000000 typed-config-1.5.0/typedconfig/__init__.py
--rw-rw-rw-   0        0        0       66 2024-04-02 10:48:32.000000 typed-config-1.5.0/typedconfig/__version__.py
--rw-rw-rw-   0        0        0     4971 2024-03-28 16:08:15.000000 typed-config-1.5.0/typedconfig/casts.py
--rw-rw-rw-   0        0        0    15717 2022-11-28 09:33:43.000000 typed-config-1.5.0/typedconfig/config.py
--rw-rw-rw-   0        0        0     2951 2022-11-28 09:33:43.000000 typed-config-1.5.0/typedconfig/provider.py
--rw-rw-rw-   0        0        0        0 2021-11-03 10:59:05.000000 typed-config-1.5.0/typedconfig/py.typed
--rw-rw-rw-   0        0        0     3860 2024-04-02 10:39:55.000000 typed-config-1.5.0/typedconfig/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:23:31.584142 typed-config-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 15:23:22.000000 typed-config-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28207 2024-04-02 15:23:31.580142 typed-config-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27280 2024-04-02 15:23:22.000000 typed-config-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 15:23:22.000000 typed-config-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:23:31.584142 typed-config-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-02 15:23:22.000000 typed-config-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:23:31.580142 typed-config-2.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-02 15:23:22.000000 typed-config-2.0.3/test/test_casts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-02 15:23:22.000000 typed-config-2.0.3/test/test_config_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-02 15:23:22.000000 typed-config-2.0.3/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-02 15:23:22.000000 typed-config-2.0.3/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:23:31.580142 typed-config-2.0.3/typed_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28207 2024-04-02 15:23:31.000000 typed-config-2.0.3/typed_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 15:23:31.000000 typed-config-2.0.3/typed_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:23:31.000000 typed-config-2.0.3/typed_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 15:23:31.000000 typed-config-2.0.3/typed_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:23:31.580142 typed-config-2.0.3/typedconfig/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/casts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15161 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-02 15:23:22.000000 typed-config-2.0.3/typedconfig/source.py
```

### Comparing `typed-config-1.5.0/LICENSE` & `typed-config-2.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Ben Windsor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 Ben Windsor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `typed-config-1.5.0/PKG-INFO` & `typed-config-2.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,646 +1,651 @@
-Metadata-Version: 2.1
-Name: typed-config
-Version: 1.5.0
-Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
-Home-page: https://github.com/bwindsor/typed-config
-Author: Ben Windsor
-Author-email: 
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.org/bwindsor/typed-config.svg?branch=master)](https://travis-ci.org/bwindsor/typed-config)
-[![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
-
-# typed-config
-Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
-
-`pip install typed-config`
-
-Requires python 3.6 or above. (Also, needs `typing_extensions` for Python <= 3.7, so not completely dependency free if using old Python).
-
-## Basic usage
-```python
-# my_app/config.py
-from typedconfig import Config, key, section
-from typedconfig.source import EnvironmentConfigSource
-
-@section('database')
-class AppConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-    timeout = key(cast=float)
-
-config = AppConfig()
-config.add_source(EnvironmentConfigSource())
-config.read()
-```
-
-```python
-# my_app/main.py
-from my_app.config import config
-print(config.host)
-```
-In PyCharm, and hopefully other IDEs, it will recognise the datatypes of your configuration and allow you to autocomplete. No more remembering strings to get the right thing out!
-
-## Upgrading from 0.x.x
-There is one breaking change when moving from `0.x.x` to `1.x.x`. The `key` function now expects all arguments to be keyword arguments. So simply replace any calls like so:
-```python
-key('section', 'key', True, str, 'default')  # 0.x.x
-key(section_name='section', key_name='key', required=True, cast=str, default='default')  # 1.x.x
-```
-The reason for this change is to tie down the return type of `key` properly. Previously, when `required=False` or when `cast=None` the return type would not include the possibility of `None` or `string`. The type checker should now be able to infer the return type based on the values of `required`, `cast` and `default`.
-
-## How it works
-Configuration is always supplied in a two level structure, so your source configuration can have multiple sections, and each section contains multiple key/value configuration pairs. For example:
-```ini
-[database]
-host = 127.0.0.1
-port = 2000
-
-[algorithm]
-max_value = 10
-min_value = 20
-```
-
-You then create your configuration hierarchy in code (this can be flat or many levels deep) and supply the matching between strings in your config sources and properties of your configuration classes.
-
-You provide one or more `ConfigSource`s, from which the config for your application can be read. For example, you might supply an `EnvironmentConfigSource`,  and two `IniFileConfigSource`s. This would make your application first look for a configuration value in environment variables, if not found there it would then look at the first INI file (perhaps a user-specific file), before falling back to the second INI file (perhaps a default configuration shared between all users). If a parameter is still not found and is a required parameter, an error would be thrown.
-
-There is emphasis on type information being available for everything so that an IDE will autocomplete when trying to use your config across your application.
-
-### Multiple data sources
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-    username = key(cast=str)
-    password = key(cast=str)
-
-config = DatabaseConfig()
-config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-config.add_source(IniFileConfigSource("config.cfg"))
-
-# OR provide sources directly to the constructor
-config = DatabaseConfig(sources=[
-    EnvironmentConfigSource(prefix="EXAMPLE"),
-    IniFileConfigSource("config.cfg")
-])
-```
-
-Since you don't want to hard code your secret credentials, you might supply them through the environment.
-So for the above configuration, the environment might look like this:
-```bash
-export EXAMPLE_DATABASE_USERNAME=my_username
-export EXAMPLE_DATABASE_PASSWORD=my_very_secret_password
-export EXAMPLE_DATABASE_PORT=2001
-```
-
-Those values which couldn't be found in the environment would then be read from the INI file, which might look like this:
-```ini
-[database]
-HOST = db1.mydomain.com
-PORT = 2000
-```
-
-Note after this, `config.port` will be equal to `2001` as the value in the environment took priority over the value in the INI file.
-
-### Caching
-When config values are first used, they are read. This is lazy evaluation by default so that not everything is read if not necessary.
-
-After first use, they are cached in memory so that there should be no further I/O if the config value is used again.
-
-For fail fast behaviour, and also to stop unexpected latency when a config value is read partway through your application (e.g. your config could be coming across a network), the option is available to read all config values at the start. Just call
-
-`config.read()`
-
-This will throw an exception if any required config value cannot be found, and will also keep all read config values in memory for next time they are used. If you do not use `read` you will only get the exception when you first try to use the offending config key.
-
-### Hierarchical configuration
-Use `group_key` to represent a "sub-config" of a configuration. Set up "sub-configs" exactly as demonstrated above, and then create a parent config to compose them in one place.
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-
-@section('algorithm')
-class AlgorithmConfig(Config):
-    max_value = key(cast=float)
-    min_value = key(cast=float)
-
-class ParentConfig(Config):
-    database = group_key(DatabaseConfig)
-    algorithm = group_key(AlgorithmConfig)
-    description = key(cast=str, section_name="general")
-
-config = ParentConfig()
-config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-config.add_source(IniFileConfigSource("config.cfg"))
-config.read()
-```
-
-The first time the `config.database` or `config.algorithm` is accessed (which in the case above is when `read()` is called), then an instance will be instantiated. Notice that it is the class definition, not an instance of the class, which is passed to the `group_key` function.
-
-### Custom section/key names, optional parameters, default values
-Let's take a look at this:
-```python
-from typedconfig import Config, key, section
-
-@section('database')
-class AppConfig(Config):
-    host1 = key()
-    host2 = key(section_name='database', key_name='HOST2',
-                required=True, cast=str, default=None)
-```
-Both `host1` and `host2` are legitimate configuration key definitions.
-
-* `section_name` - this name of the section in the configuration source from which this parameter should be read. This can be provided on a key-by-key basis, but if it is left out then the section name supplied by the `@section` decorator is used. If all keys supply a `section_name`, the class decorator is not needed. If both `section_name` and a decorator are provided, the `section_name` argument takes priority.
-* `key_name` - the name of this key in the configuration source from which this parameter is read. If not supplied, some magic uses the object property name as the key name.
-* `required` - default True. If False, and the configuration value can't be found, no error will be thrown and the default value will be used, if provided. If a default not provided, `None` will be used.
-* `cast` - probably the most important option for typing. **If you want autocomplete typing support you must specify this**. It's just a function which takes a string as an input and returns a parsed value. See the casting section for more. If not supplied, the value remains as a string.
-* `default` - only applicable if `required` is false. When `required` is false this value is used if a value cannot be found.
-
-### Types
-```python
-from typedconfig import Config, key, section
-from typing import List
-
-def split_str(s: str) -> List[str]:
-    return [x.strip() for x in s.split(",")]
-
-@section('database')
-class AppConfig(Config):
-    host = key()
-    port = key(cast=int)
-    users = key(cast=split_str)
-    zero_based_index = key(cast=lambda x: int(x)-1)
-config = AppConfig(sources=[...])
-```
-In this example we have three ways of casting:
-1. Not casting at all. This defaults to returning a `str`, but your IDE won't know that so if you want type hints use `cast=str`
-2. Casting to an built in type which can take a string input and parse it, for example `int`
-3. Defining a custom function. Your function should take one string input and return one output of any type. To get type hint, just make sure your function has type annotations.
-4. Using a lambda expression. The type inference may or may not work depending on your expression, so if it doesn't just write it as a function with type annotations.
-
-### Validation
-You can validate what has been supplied by providing a custom `cast` function to a `key`, which validates the configuration value in addition to parsing it.
-
-### Extending configuration using shared ConfigProvider
-
-Multiple application modules may use different configuration schemes while sharing the same configuration source. Analogously, various `Config` classes may provide different view of the same configuration data, sharing the same `ConfigProvider`.
-
-```python
-# app/config.py
-from typedconfig.provider import ConfigProvider
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-provider = ConfigProvider()
-provider.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-provider.add_source(IniFileConfigSource("config.cfg"))
-
-__all__ = ["provider"]
-```
-```python
-# app/database/config.py
-from typedconfig import Config, key, section
-from app.config import provider
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-
-database_config = DatabaseConfig(provider=provider)
-```
-```python
-# app/algorithm/config.py
-from typedconfig import Config, key, section
-from app.config import provider
-
-@section('algorithm')
-class AlgorithmConfig(Config):
-    max_value = key(cast=float)
-    min_value = key(cast=float)
-
-algorithm_config = AlgorithmConfig(provider=provider)
-```
-
-Shared configuration provider can be used by plugins, which may need to declare additional configuration sections within the same configuration files as the main application.  Let's assume we have `[database]` section used by main application and `[app_extension]` that provides 3rd party plugin configuration:
-
-```ini
-[database]
-host = 127.0.0.1
-port = 2000
-
-[app_extension]
-api_key = secret
-```
-
-e.g. `app/config.py` may look like that:
-
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    """Database configuration"""
-    host = key(cast=str)
-    port = key(cast=int)
-
-class ApplicationConfig(Config):
-    """Main configuration object"""
-    database = group_key(DatabaseConfig)
-
-app_config = ApplicationConfig(sources=[
-    EnvironmentConfigSource(),
-    IniFileConfigSource("config.cfg")
-])
-```
-
-and plugin can read additional sections by using the same configuration provider as main application config.
-
-e.g. `plugin/config.py`:
-```python
-from typedconfig import Config, key, section, group_key
-
-from app.config import ApplicationConfig, app_config
-
-@section('app_extension')
-class ExtensionConfig(Config):
-    """Extension configuration"""
-    api_key = key(cast=str)
-
-# ExtendedAppConfig extends ApplicationConfig 
-# so original sections are also included
-class ExtendedAppConfig(ApplicationConfig):
-    """Extended main configuration object"""
-    app_extension = group_key(ExtensionConfig)
-    
-# ExtendedAppConfig uses the same provider as the main app_config
-extended_config = ExtendedAppConfig(provider=app_config.provider)
-```
-```python
-from plugin.config import extended_config
-
-# Plugin can access both main and extra sections
-print(extended_config.app_extension.api_key)
-print(extended_config.database.host)
-```
-
-### Configuration variables which depend on other configuration variables
-Sometimes you may wish to set the value of some configuration variables based on others. You may also wish to validate some variables, for example allowed values may be different depending on the value of another config variable. For this you can add a `post_read_hook`.
-
-The default implementation of `post_read_hook` returns an empty `dict`. You can override this by implementing your own `post_read_hook` method. It should receive only `self` as an input, and return a `dict`. This `dict` should be a simple mapping from config keys to values. For hierarchical configurations, you can nest the dictionaries. If you provide a `post_read_hook` in both a parent and a child class which both make changes to the same keys (don't do this) then the values returned by the child method will overwrite those by the parent.
-
-This hook is called whenever you call the `read` method. If you use lazy loading and skip calling the `read` method, you cannot use this hook.
-```python
-# my_app/config.py
-from typedconfig import Config, key, group_key, section
-from typedconfig.source import EnvironmentConfigSource
-
-@section('child')
-class ChildConfig(Config):
-    http_port_plus_one = key(cast=int, required=False)
-
-@section('app')
-class AppConfig(Config):
-    use_https = key(cast=bool)
-    http_port = key(key_name='port', cast=int, required=False)
-    child = group_key(ChildConfig)
-    
-    def post_read_hook(self) -> dict:
-        config_updates = dict()
-        # If the port has not been provided, set it based on the value of use_https
-        if self.http_port is None:
-            config_updates.update(http_port=443 if self.use_https else 80)
-        else:
-            # Modify child config
-            config_updates.update(child=dict(http_port_plus_one=self.http_port + 1))
-            
-        # Validate that the port number has a sensible value
-        # It is recommended to do validation inside the cast method for individual keys, however for dependent keys it can be useful here
-        if self.http_port is not None:
-            if self.use_https:
-                assert self.http_port in [443, 444, 445]
-            else:
-                assert self.http_port in [80, 81, 82]
-
-        return config_updates
-            
-config = AppConfig()
-config.add_source(EnvironmentConfigSource())
-config.read()
-```
-
-## Configuration Sources
-Configuration sources are how your main `Config` class knows where to get its data from. These are totally extensible so that you can read in your configuration from wherever you like - from a database, from S3, anywhere that you can write code for.
-
-You supply your configuration source to your config after you've instantiated it, but **before** you try to read any data from it:
-```python
-config = AppConfig()
-config.add_source(my_first_source)
-config.add_source(my_second_source)
-config.read()
-```
-Or you can supply the sources directly in the constructor like this:
-```python
-config = AppConfig(sources=[my_first_source, my_second_source])
-config.read()
-```
-
-
-### Modifying or refreshing configuration after it has been loaded
-In general it is bad practice to modify configuration at runtime because the configuration for your program should be fixed for the duration of it.  However, there are cases where it may be necessary.
-
-To completely replace the set of config sources, you can use
-```python
-config = AppConfig(sources=[my_first_source, my_second_source])
-config.set_sources([my_first_new_source, my_second_new_source])
-```
-
-To replace a specific config source, for example because a config file has changed and you need to re-read it from disk, you can use `replace_source`:
-```python
-from typedconfig.source import IniFileConfigSource
-original_source = IniFileConfigSource("config.cfg")
-config = AppConfig(sources=[source])
-# Now say you change the contents to config.cfg and need to read it again
-new_source = IniFileConfigSource("config.cfg")  # re-reads file during construction
-config.replace_source(original_source, new_source)
-```
-
-**Important**: if you add or modify the config sources the config has been read, or need to refresh the config for some reason, you'll need to clear any cached values in order to force the config to be fetched from the `ConfigSource`s again. You can do this by
-```python
-config.clear_cache()
-config.read()          # Read all configuration values again
-```
-
-
-
-### Supplied Config Sources
-#### `EnvironmentConfigSource`
-This just reads configuration from environment variables.
-```python
-from typedconfig.source import EnvironmentConfigSource
-source = EnvironmentConfigSource(prefix="XYZ")
-# OR just
-source = EnvironmentConfigSource()
-```
-It just takes one optional input argument, a prefix. This can be useful to avoid name clashes in environment variables.
-
-* If prefix is provided, environment variables are expected to look like `{PREFIX}_{SECTION}_{KEY}`, for example `export XYZ_DATABASE_PORT=2000`. 
-* If no prefix is provided, environment variables should look like `{SECTION}_{KEY}`, for example `export DATABASE_PORT=2000`.
-
-#### `IniFileConfigSource`
-This reads from an INI file using Python's built in [configparser](https://docs.python.org/3/library/configparser.html). Read the docs for `configparser` for more about the structure of the file.
-```python
-from typedconfig.source import IniFileConfigSource
-source = IniFileConfigSource("config.cfg", encoding='utf-8', must_exist=True)
-```
-
-* The first argument is the filename (absolute or relative to the current working directory).
-* `encoding` is the text encoding of the file. `configparser`'s default is used if not supplied.
-* `must_exist` - default `True`. If the file can't be found, an error will be thrown by default. Setting `must_exist` to be `False` allows the file not to be present, in which case this source will just report that it can't find any configuration values and your `Config` class will move onto looking in the next `ConfigSource`.
-
-#### `IniStringConfigSource`
-This reads from a string instead of a file
-```python
-from typedconfig.source import IniStringConfigSource
-source = IniStringConfigSource("""
-[section_name]
-key_name=key_value
-""")
-```
-
-#### `DictConfigSource`
-The most basic source, entirely in memory, and also useful when writing tests. It is case insensitive.
-```python
-from typedconfig.source import DictConfigSource
-source = DictConfigSource({
-    'database': dict(HOST='db1', PORT='2000'),
-    'algorithm': dict(MAX_VALUE='20', MIN_VALUE='10')
-})
-```
-
-It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
-
-This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
-
-#### `CmdConfigSource`
-This reads configuration from command line arguments
-```python
-from typedconfig.source import CmdConfigSource
-source = CmdConfigSource(prefix="XYZ")
-# OR just
-source = CmdConfigSource()
-```
-
-It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
-
-* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
-* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
-
-The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
-
-### Writing your own `ConfigSource`s
-An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
-
-Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
-```python
-import json
-from typing import Optional
-from typedconfig.source import ConfigSource
-
-class JsonConfigSource(ConfigSource):
-    def __init__(self, filename: str):
-        # Read data - will raise an exception if problem with file
-        with open(filename, 'r') as f:
-            self.data = json.load(f)
-        # Quick checks on data format
-        assert type(self.data) is dict
-        for k, v in self.data.items():
-            assert type(k) is str
-            assert type(v) is dict
-            for v_k, v_v in v.items():
-                assert type(v_k) is str
-                assert type(v_v) is str
-        # Convert all keys to lowercase
-        self.data = {
-            k.lower(): {
-                v_k.lower(): v_v
-                for v_k, v_v in v.items()
-            }
-            for k, v in self.data.items()
-        }    
-
-    def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
-        # Extract info from data which we read in during __init__
-        section = self.data.get(section_name.lower(), None)
-        if section is None:
-            return None
-        return section.get(key_name.lower(), None)
-```
-
-### Additional config sources
-In order to keep `typed-config` dependency free, `ConfigSources` requiring additional dependencies are in separate packages, which also have `typed-config` as a dependency.
-
-These are listed here:
-
-| pip install name | import name | Description |
-| --- | --- | --- |
-| [typed-config-aws-sources](https://pypi.org/project/typed-config-aws-sources) | `typedconfig_awssource` | Config sources using `boto3` to get config e.g. from S3 or DynamoDB
-
-
-## Cast function library
-The `typedconfig.casts` module contains helper functions that implement common casting operations. These would generally be passed to the `cast` parameter of the `key()` function
-
-### Casting to an `Enum` type with `enum_cast`
-the `enum_cast` function converts a string input from a source to a member of an `Enum` type. 
-
-For example:
-```python
-from enum import Enum
-from typedconfig.casts import enum_cast
-from typedconfig import Config, key
-...
-class ColorEnum(Enum):
-    RED = 1
-    GREEN = 2
-    BLUE = 3
-...
-
-class MyConfig(Config):
-    color = key(cast=enum_cast(ColorEnum))
-```
-
-In this example, if the `ConfigSource` reads the string `"RED"`, the value of `color` will be set to `ColorEnum.RED`
-
-Note that the `enum_cast` function is designed to read the *name* of an enum member, not its value (`1`, `2` or `3` in the example above)
-
-### Casting to a `tuple` with `tuple_cast`
-If the source contains a list of items, `tuple_cast` will parse them as a python tuple, optionally applying a 
-base_cast function to each element. 
-The default behavior is to call strip() on each element and ignore trailing delimiters.
-
-For example, given the input
-```ini
-nums = 1, 2, 3, 4,
-```
-
-Then you could use
-
-```python
-nums = key(cast=tuple_cast())
-```
-to read the string input and cast it to `("1", "2", "3", "4")`
-
-```python
-key(cast=tuple_cast(base_cast=int))
-```
-Would cast the input to `(1, 2, 3, 4)`
-
-```python
-key(cast=tuple_cast(ignore_trailing_delimiter=False))
-```
-Would cast the input to `("1", "2", "3", "4", "")`
-
-```python
-key(cast=tuple_cast(strip=False))
-```
-Would cast the input to `("1", " 2", " 3", " 4")`
-
-Finally, if a delimiter other that "," is used - say the input string is `"1:2:3:4"` - that can be handled like
-```python
-key(cast=tuple_cast(delimiter=":"))
-```
-
-### Casting to a `bool` with `boolean_cast`
-
-If the source is a boolean value, it can be converted to Python's `True` or `False` using this cast.
-
-```python
-key(cast=boolean_cast)
-```
-
-`boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
-
-Value | Strings
---- | ---
-`True` | `"true"`, `"yes"`, `"on"`, `"1"`
-`False` | `"false"`, `"no"`, `"off"`, `"0"`
-
-### Casting to an `Optional[bool]` with `optional_boolean_cast`
-
-If the source is a boolean value which can also be `None`, it can be converted to Python's `True` or `False` or `None` using this cast.
-
-```python
-key(cast=optional_boolean_cast)
-```
-
-`optional_boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
-
-Value | Strings
---- | ---
-`True` | `"true"`, `"yes"`, `"on"`, `"1"`
-`False` | `"false"`, `"no"`, `"off"`, `"0"`
-`None` | `"none"`, `"unknown"`
-
-
-## Contributing
-Ideas for new features and pull requests are welcome. PRs must come with tests included. This was developed using Python 3.7 but Travis tests run with all versions 3.6-3.9 too.
-
-### Development setup
-1. Clone the git repository
-2. Create a virtual environment `virtualenv venv`
-3. Activate the environment `venv/scripts/activate`
-4. Install development dependencies `pip install -r requirements.txt`
-
-### Code style
-Code style is `black` and this is checked by the CI. To autoformat your code as `black` before committing, just run `black typedconfig test`
-
-### Running tests
-`pytest`
-
-To run with coverage:
-
-`pytest --cov`
-
-### Making a release
-1. Bump version number in `typedconfig/__version__.py`
-1. Add changes to [CHANGELOG.md](CHANGELOG.md)
-1. Commit your changes and tag with `git tag -a v0.1.0 -m "Summary of changes"`
-1. Travis will deploy the release to PyPi for you.
-
-#### Staging release
-If you want to check how a release will look on PyPi before tagging and making it live, you can do the following:
-1. `pip install twine` if you don't already have it
-1. Bump version number in `typedconfig/__version__.py`
-1. Clear the dist directory `rm -r dist`
-1. `python setup.py sdist bdist_wheel`
-1. `twine check dist/*`
-1. Upload to the test PyPI `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
-1. Check all looks ok at [https://test.pypi.org/project/typed-config](https://test.pypi.org/project/typed-config)
-1. If all looks good you can git tag and push for deploy to live PyPi
-
-Here is [a good tutorial](https://realpython.com/pypi-publish-python-package) on publishing packages to PyPI.
+Metadata-Version: 2.1
+Name: typed-config
+Version: 2.0.3
+Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
+Home-page: https://github.com/bwindsor/typed-config
+Author: Ben Windsor
+Author-email: 
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Build Status](https://github.com/bwindsor/typed-config/actions/workflows/unit_test.yml/badge.svg)
+![Deploy Status](https://github.com/bwindsor/typed-config/actions/workflows/deploy_pypi.yml/badge.svg)
+[![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
+
+# typed-config
+Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
+
+`pip install typed-config`
+
+Requires python 3.6 or above. (Also, needs `typing_extensions` for Python <= 3.7, so not completely dependency free if using old Python).
+
+## Basic usage
+```python
+# my_app/config.py
+from typedconfig import Config, key, section
+from typedconfig.source import EnvironmentConfigSource
+
+@section('database')
+class AppConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+    timeout = key(cast=float)
+
+config = AppConfig()
+config.add_source(EnvironmentConfigSource())
+config.read()
+```
+
+```python
+# my_app/main.py
+from my_app.config import config
+print(config.host)
+```
+In PyCharm, and hopefully other IDEs, it will recognise the datatypes of your configuration and allow you to autocomplete. No more remembering strings to get the right thing out!
+
+## Upgrading
+
+### From 0.x.x
+There is one breaking change when moving from `0.x.x` to `1.x.x`. The `key` function now expects all arguments to be keyword arguments. So simply replace any calls like so:
+```python
+key('section', 'key', True, str, 'default')  # 0.x.x
+key(section_name='section', key_name='key', required=True, cast=str, default='default')  # 1.x.x
+```
+The reason for this change is to tie down the return type of `key` properly. Previously, when `required=False` or when `cast=None` the return type would not include the possibility of `None` or `string`. The type checker should now be able to infer the return type based on the values of `required`, `cast` and `default`.
+
+###  From 1.x.x
+When upgrading from `1.x.x` to `2.x.x`, Python 3.7 no longer supported as it is end of life. As long as you are using Python >= 3.8, everything should just work.
+
+## How it works
+Configuration is always supplied in a two level structure, so your source configuration can have multiple sections, and each section contains multiple key/value configuration pairs. For example:
+```ini
+[database]
+host = 127.0.0.1
+port = 2000
+
+[algorithm]
+max_value = 10
+min_value = 20
+```
+
+You then create your configuration hierarchy in code (this can be flat or many levels deep) and supply the matching between strings in your config sources and properties of your configuration classes.
+
+You provide one or more `ConfigSource`s, from which the config for your application can be read. For example, you might supply an `EnvironmentConfigSource`,  and two `IniFileConfigSource`s. This would make your application first look for a configuration value in environment variables, if not found there it would then look at the first INI file (perhaps a user-specific file), before falling back to the second INI file (perhaps a default configuration shared between all users). If a parameter is still not found and is a required parameter, an error would be thrown.
+
+There is emphasis on type information being available for everything so that an IDE will autocomplete when trying to use your config across your application.
+
+### Multiple data sources
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+    username = key(cast=str)
+    password = key(cast=str)
+
+config = DatabaseConfig()
+config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+config.add_source(IniFileConfigSource("config.cfg"))
+
+# OR provide sources directly to the constructor
+config = DatabaseConfig(sources=[
+    EnvironmentConfigSource(prefix="EXAMPLE"),
+    IniFileConfigSource("config.cfg")
+])
+```
+
+Since you don't want to hard code your secret credentials, you might supply them through the environment.
+So for the above configuration, the environment might look like this:
+```bash
+export EXAMPLE_DATABASE_USERNAME=my_username
+export EXAMPLE_DATABASE_PASSWORD=my_very_secret_password
+export EXAMPLE_DATABASE_PORT=2001
+```
+
+Those values which couldn't be found in the environment would then be read from the INI file, which might look like this:
+```ini
+[database]
+HOST = db1.mydomain.com
+PORT = 2000
+```
+
+Note after this, `config.port` will be equal to `2001` as the value in the environment took priority over the value in the INI file.
+
+### Caching
+When config values are first used, they are read. This is lazy evaluation by default so that not everything is read if not necessary.
+
+After first use, they are cached in memory so that there should be no further I/O if the config value is used again.
+
+For fail fast behaviour, and also to stop unexpected latency when a config value is read partway through your application (e.g. your config could be coming across a network), the option is available to read all config values at the start. Just call
+
+`config.read()`
+
+This will throw an exception if any required config value cannot be found, and will also keep all read config values in memory for next time they are used. If you do not use `read` you will only get the exception when you first try to use the offending config key.
+
+### Hierarchical configuration
+Use `group_key` to represent a "sub-config" of a configuration. Set up "sub-configs" exactly as demonstrated above, and then create a parent config to compose them in one place.
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+
+@section('algorithm')
+class AlgorithmConfig(Config):
+    max_value = key(cast=float)
+    min_value = key(cast=float)
+
+class ParentConfig(Config):
+    database = group_key(DatabaseConfig)
+    algorithm = group_key(AlgorithmConfig)
+    description = key(cast=str, section_name="general")
+
+config = ParentConfig()
+config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+config.add_source(IniFileConfigSource("config.cfg"))
+config.read()
+```
+
+The first time the `config.database` or `config.algorithm` is accessed (which in the case above is when `read()` is called), then an instance will be instantiated. Notice that it is the class definition, not an instance of the class, which is passed to the `group_key` function.
+
+### Custom section/key names, optional parameters, default values
+Let's take a look at this:
+```python
+from typedconfig import Config, key, section
+
+@section('database')
+class AppConfig(Config):
+    host1 = key()
+    host2 = key(section_name='database', key_name='HOST2',
+                required=True, cast=str, default=None)
+```
+Both `host1` and `host2` are legitimate configuration key definitions.
+
+* `section_name` - this name of the section in the configuration source from which this parameter should be read. This can be provided on a key-by-key basis, but if it is left out then the section name supplied by the `@section` decorator is used. If all keys supply a `section_name`, the class decorator is not needed. If both `section_name` and a decorator are provided, the `section_name` argument takes priority.
+* `key_name` - the name of this key in the configuration source from which this parameter is read. If not supplied, some magic uses the object property name as the key name.
+* `required` - default True. If False, and the configuration value can't be found, no error will be thrown and the default value will be used, if provided. If a default not provided, `None` will be used.
+* `cast` - probably the most important option for typing. **If you want autocomplete typing support you must specify this**. It's just a function which takes a string as an input and returns a parsed value. See the casting section for more. If not supplied, the value remains as a string.
+* `default` - only applicable if `required` is false. When `required` is false this value is used if a value cannot be found.
+
+### Types
+```python
+from typedconfig import Config, key, section
+from typing import List
+
+def split_str(s: str) -> List[str]:
+    return [x.strip() for x in s.split(",")]
+
+@section('database')
+class AppConfig(Config):
+    host = key()
+    port = key(cast=int)
+    users = key(cast=split_str)
+    zero_based_index = key(cast=lambda x: int(x)-1)
+config = AppConfig(sources=[...])
+```
+In this example we have three ways of casting:
+1. Not casting at all. This defaults to returning a `str`, but your IDE won't know that so if you want type hints use `cast=str`
+2. Casting to an built in type which can take a string input and parse it, for example `int`
+3. Defining a custom function. Your function should take one string input and return one output of any type. To get type hint, just make sure your function has type annotations.
+4. Using a lambda expression. The type inference may or may not work depending on your expression, so if it doesn't just write it as a function with type annotations.
+
+### Validation
+You can validate what has been supplied by providing a custom `cast` function to a `key`, which validates the configuration value in addition to parsing it.
+
+### Extending configuration using shared ConfigProvider
+
+Multiple application modules may use different configuration schemes while sharing the same configuration source. Analogously, various `Config` classes may provide different view of the same configuration data, sharing the same `ConfigProvider`.
+
+```python
+# app/config.py
+from typedconfig.provider import ConfigProvider
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+provider = ConfigProvider()
+provider.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+provider.add_source(IniFileConfigSource("config.cfg"))
+
+__all__ = ["provider"]
+```
+```python
+# app/database/config.py
+from typedconfig import Config, key, section
+from app.config import provider
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+
+database_config = DatabaseConfig(provider=provider)
+```
+```python
+# app/algorithm/config.py
+from typedconfig import Config, key, section
+from app.config import provider
+
+@section('algorithm')
+class AlgorithmConfig(Config):
+    max_value = key(cast=float)
+    min_value = key(cast=float)
+
+algorithm_config = AlgorithmConfig(provider=provider)
+```
+
+Shared configuration provider can be used by plugins, which may need to declare additional configuration sections within the same configuration files as the main application.  Let's assume we have `[database]` section used by main application and `[app_extension]` that provides 3rd party plugin configuration:
+
+```ini
+[database]
+host = 127.0.0.1
+port = 2000
+
+[app_extension]
+api_key = secret
+```
+
+e.g. `app/config.py` may look like that:
+
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    """Database configuration"""
+    host = key(cast=str)
+    port = key(cast=int)
+
+class ApplicationConfig(Config):
+    """Main configuration object"""
+    database = group_key(DatabaseConfig)
+
+app_config = ApplicationConfig(sources=[
+    EnvironmentConfigSource(),
+    IniFileConfigSource("config.cfg")
+])
+```
+
+and plugin can read additional sections by using the same configuration provider as main application config.
+
+e.g. `plugin/config.py`:
+```python
+from typedconfig import Config, key, section, group_key
+
+from app.config import ApplicationConfig, app_config
+
+@section('app_extension')
+class ExtensionConfig(Config):
+    """Extension configuration"""
+    api_key = key(cast=str)
+
+# ExtendedAppConfig extends ApplicationConfig 
+# so original sections are also included
+class ExtendedAppConfig(ApplicationConfig):
+    """Extended main configuration object"""
+    app_extension = group_key(ExtensionConfig)
+    
+# ExtendedAppConfig uses the same provider as the main app_config
+extended_config = ExtendedAppConfig(provider=app_config.provider)
+```
+```python
+from plugin.config import extended_config
+
+# Plugin can access both main and extra sections
+print(extended_config.app_extension.api_key)
+print(extended_config.database.host)
+```
+
+### Configuration variables which depend on other configuration variables
+Sometimes you may wish to set the value of some configuration variables based on others. You may also wish to validate some variables, for example allowed values may be different depending on the value of another config variable. For this you can add a `post_read_hook`.
+
+The default implementation of `post_read_hook` returns an empty `dict`. You can override this by implementing your own `post_read_hook` method. It should receive only `self` as an input, and return a `dict`. This `dict` should be a simple mapping from config keys to values. For hierarchical configurations, you can nest the dictionaries. If you provide a `post_read_hook` in both a parent and a child class which both make changes to the same keys (don't do this) then the values returned by the child method will overwrite those by the parent.
+
+This hook is called whenever you call the `read` method. If you use lazy loading and skip calling the `read` method, you cannot use this hook.
+```python
+# my_app/config.py
+from typedconfig import Config, key, group_key, section
+from typedconfig.source import EnvironmentConfigSource
+
+@section('child')
+class ChildConfig(Config):
+    http_port_plus_one = key(cast=int, required=False)
+
+@section('app')
+class AppConfig(Config):
+    use_https = key(cast=bool)
+    http_port = key(key_name='port', cast=int, required=False)
+    child = group_key(ChildConfig)
+    
+    def post_read_hook(self) -> dict:
+        config_updates = dict()
+        # If the port has not been provided, set it based on the value of use_https
+        if self.http_port is None:
+            config_updates.update(http_port=443 if self.use_https else 80)
+        else:
+            # Modify child config
+            config_updates.update(child=dict(http_port_plus_one=self.http_port + 1))
+            
+        # Validate that the port number has a sensible value
+        # It is recommended to do validation inside the cast method for individual keys, however for dependent keys it can be useful here
+        if self.http_port is not None:
+            if self.use_https:
+                assert self.http_port in [443, 444, 445]
+            else:
+                assert self.http_port in [80, 81, 82]
+
+        return config_updates
+            
+config = AppConfig()
+config.add_source(EnvironmentConfigSource())
+config.read()
+```
+
+## Configuration Sources
+Configuration sources are how your main `Config` class knows where to get its data from. These are totally extensible so that you can read in your configuration from wherever you like - from a database, from S3, anywhere that you can write code for.
+
+You supply your configuration source to your config after you've instantiated it, but **before** you try to read any data from it:
+```python
+config = AppConfig()
+config.add_source(my_first_source)
+config.add_source(my_second_source)
+config.read()
+```
+Or you can supply the sources directly in the constructor like this:
+```python
+config = AppConfig(sources=[my_first_source, my_second_source])
+config.read()
+```
+
+
+### Modifying or refreshing configuration after it has been loaded
+In general it is bad practice to modify configuration at runtime because the configuration for your program should be fixed for the duration of it.  However, there are cases where it may be necessary.
+
+To completely replace the set of config sources, you can use
+```python
+config = AppConfig(sources=[my_first_source, my_second_source])
+config.set_sources([my_first_new_source, my_second_new_source])
+```
+
+To replace a specific config source, for example because a config file has changed and you need to re-read it from disk, you can use `replace_source`:
+```python
+from typedconfig.source import IniFileConfigSource
+original_source = IniFileConfigSource("config.cfg")
+config = AppConfig(sources=[source])
+# Now say you change the contents to config.cfg and need to read it again
+new_source = IniFileConfigSource("config.cfg")  # re-reads file during construction
+config.replace_source(original_source, new_source)
+```
+
+**Important**: if you add or modify the config sources the config has been read, or need to refresh the config for some reason, you'll need to clear any cached values in order to force the config to be fetched from the `ConfigSource`s again. You can do this by
+```python
+config.clear_cache()
+config.read()          # Read all configuration values again
+```
+
+
+
+### Supplied Config Sources
+#### `EnvironmentConfigSource`
+This just reads configuration from environment variables.
+```python
+from typedconfig.source import EnvironmentConfigSource
+source = EnvironmentConfigSource(prefix="XYZ")
+# OR just
+source = EnvironmentConfigSource()
+```
+It just takes one optional input argument, a prefix. This can be useful to avoid name clashes in environment variables.
+
+* If prefix is provided, environment variables are expected to look like `{PREFIX}_{SECTION}_{KEY}`, for example `export XYZ_DATABASE_PORT=2000`. 
+* If no prefix is provided, environment variables should look like `{SECTION}_{KEY}`, for example `export DATABASE_PORT=2000`.
+
+#### `IniFileConfigSource`
+This reads from an INI file using Python's built in [configparser](https://docs.python.org/3/library/configparser.html). Read the docs for `configparser` for more about the structure of the file.
+```python
+from typedconfig.source import IniFileConfigSource
+source = IniFileConfigSource("config.cfg", encoding='utf-8', must_exist=True)
+```
+
+* The first argument is the filename (absolute or relative to the current working directory).
+* `encoding` is the text encoding of the file. `configparser`'s default is used if not supplied.
+* `must_exist` - default `True`. If the file can't be found, an error will be thrown by default. Setting `must_exist` to be `False` allows the file not to be present, in which case this source will just report that it can't find any configuration values and your `Config` class will move onto looking in the next `ConfigSource`.
+
+#### `IniStringConfigSource`
+This reads from a string instead of a file
+```python
+from typedconfig.source import IniStringConfigSource
+source = IniStringConfigSource("""
+[section_name]
+key_name=key_value
+""")
+```
+
+#### `DictConfigSource`
+The most basic source, entirely in memory, and also useful when writing tests. It is case insensitive.
+```python
+from typedconfig.source import DictConfigSource
+source = DictConfigSource({
+    'database': dict(HOST='db1', PORT='2000'),
+    'algorithm': dict(MAX_VALUE='20', MIN_VALUE='10')
+})
+```
+
+It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
+
+This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
+
+#### `CmdConfigSource`
+This reads configuration from command line arguments
+```python
+from typedconfig.source import CmdConfigSource
+source = CmdConfigSource(prefix="XYZ")
+# OR just
+source = CmdConfigSource()
+```
+
+It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
+
+* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
+* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
+
+The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
+
+### Writing your own `ConfigSource`s
+An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
+
+Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
+```python
+import json
+from typing import Optional
+from typedconfig.source import ConfigSource
+
+class JsonConfigSource(ConfigSource):
+    def __init__(self, filename: str):
+        # Read data - will raise an exception if problem with file
+        with open(filename, 'r') as f:
+            self.data = json.load(f)
+        # Quick checks on data format
+        assert type(self.data) is dict
+        for k, v in self.data.items():
+            assert type(k) is str
+            assert type(v) is dict
+            for v_k, v_v in v.items():
+                assert type(v_k) is str
+                assert type(v_v) is str
+        # Convert all keys to lowercase
+        self.data = {
+            k.lower(): {
+                v_k.lower(): v_v
+                for v_k, v_v in v.items()
+            }
+            for k, v in self.data.items()
+        }    
+
+    def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
+        # Extract info from data which we read in during __init__
+        section = self.data.get(section_name.lower(), None)
+        if section is None:
+            return None
+        return section.get(key_name.lower(), None)
+```
+
+### Additional config sources
+In order to keep `typed-config` dependency free, `ConfigSources` requiring additional dependencies are in separate packages, which also have `typed-config` as a dependency.
+
+These are listed here:
+
+| pip install name | import name | Description |
+| --- | --- | --- |
+| [typed-config-aws-sources](https://pypi.org/project/typed-config-aws-sources) | `typedconfig_awssource` | Config sources using `boto3` to get config e.g. from S3 or DynamoDB
+
+
+## Cast function library
+The `typedconfig.casts` module contains helper functions that implement common casting operations. These would generally be passed to the `cast` parameter of the `key()` function
+
+### Casting to an `Enum` type with `enum_cast`
+the `enum_cast` function converts a string input from a source to a member of an `Enum` type. 
+
+For example:
+```python
+from enum import Enum
+from typedconfig.casts import enum_cast
+from typedconfig import Config, key
+...
+class ColorEnum(Enum):
+    RED = 1
+    GREEN = 2
+    BLUE = 3
+...
+
+class MyConfig(Config):
+    color = key(cast=enum_cast(ColorEnum))
+```
+
+In this example, if the `ConfigSource` reads the string `"RED"`, the value of `color` will be set to `ColorEnum.RED`
+
+Note that the `enum_cast` function is designed to read the *name* of an enum member, not its value (`1`, `2` or `3` in the example above)
+
+### Casting to a `tuple` with `tuple_cast`
+If the source contains a list of items, `tuple_cast` will parse them as a python tuple, optionally applying a 
+base_cast function to each element. 
+The default behavior is to call strip() on each element and ignore trailing delimiters.
+
+For example, given the input
+```ini
+nums = 1, 2, 3, 4,
+```
+
+Then you could use
+
+```python
+nums = key(cast=tuple_cast())
+```
+to read the string input and cast it to `("1", "2", "3", "4")`
+
+```python
+key(cast=tuple_cast(base_cast=int))
+```
+Would cast the input to `(1, 2, 3, 4)`
+
+```python
+key(cast=tuple_cast(ignore_trailing_delimiter=False))
+```
+Would cast the input to `("1", "2", "3", "4", "")`
+
+```python
+key(cast=tuple_cast(strip=False))
+```
+Would cast the input to `("1", " 2", " 3", " 4")`
+
+Finally, if a delimiter other that "," is used - say the input string is `"1:2:3:4"` - that can be handled like
+```python
+key(cast=tuple_cast(delimiter=":"))
+```
+
+### Casting to a `bool` with `boolean_cast`
+
+If the source is a boolean value, it can be converted to Python's `True` or `False` using this cast.
+
+```python
+key(cast=boolean_cast)
+```
+
+`boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
+
+Value | Strings
+--- | ---
+`True` | `"true"`, `"yes"`, `"on"`, `"1"`
+`False` | `"false"`, `"no"`, `"off"`, `"0"`
+
+### Casting to an `Optional[bool]` with `optional_boolean_cast`
+
+If the source is a boolean value which can also be `None`, it can be converted to Python's `True` or `False` or `None` using this cast.
+
+```python
+key(cast=optional_boolean_cast)
+```
+
+`optional_boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
+
+Value | Strings
+--- | ---
+`True` | `"true"`, `"yes"`, `"on"`, `"1"`
+`False` | `"false"`, `"no"`, `"off"`, `"0"`
+`None` | `"none"`, `"unknown"`
+
+
+## Contributing
+Ideas for new features and pull requests are welcome. PRs must come with tests included. This is developed using Python 3.9 but Github actions will run tests with all versions 3.8-3.12 too.
+
+### Development setup
+1. Clone the git repository
+2. Create a virtual environment `virtualenv venv`
+3. Activate the environment `venv/scripts/activate`
+4. Install development dependencies `pip install -r requirements.txt`
+
+### Code style
+Code style is `black` and this is checked by the CI. To autoformat your code as `black` before committing, just run `black typedconfig test`
+
+### Running tests
+`pytest`
+
+To run with coverage:
+
+`pytest --cov`
+
+### Making a release
+1. Bump version number in `typedconfig/__version__.py`
+1. Add changes to [CHANGELOG.md](CHANGELOG.md)
+1. Commit your changes and tag with `git tag -a v0.1.0 -m "Summary of changes"`
+1. Github actions will deploy the release to PyPi for you.
+
+#### Staging release
+If you want to check how a release will look on PyPi before tagging and making it live, you can do the following:
+1. `pip install twine` if you don't already have it
+1. Bump version number in `typedconfig/__version__.py`
+1. Clear the dist directory `rm -r dist`
+1. `python setup.py sdist bdist_wheel`
+1. `twine check dist/*`
+1. Upload to the test PyPI `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
+1. Check all looks ok at [https://test.pypi.org/project/typed-config](https://test.pypi.org/project/typed-config)
+1. If all looks good you can git tag and push for deploy to live PyPi
+
+Here is [a good tutorial](https://realpython.com/pypi-publish-python-package) on publishing packages to PyPI.
```

### Comparing `typed-config-1.5.0/README.md` & `typed-config-2.0.3/typed_config.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,622 +1,651 @@
-[![Build Status](https://travis-ci.org/bwindsor/typed-config.svg?branch=master)](https://travis-ci.org/bwindsor/typed-config)
-[![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
-
-# typed-config
-Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
-
-`pip install typed-config`
-
-Requires python 3.6 or above. (Also, needs `typing_extensions` for Python <= 3.7, so not completely dependency free if using old Python).
-
-## Basic usage
-```python
-# my_app/config.py
-from typedconfig import Config, key, section
-from typedconfig.source import EnvironmentConfigSource
-
-@section('database')
-class AppConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-    timeout = key(cast=float)
-
-config = AppConfig()
-config.add_source(EnvironmentConfigSource())
-config.read()
-```
-
-```python
-# my_app/main.py
-from my_app.config import config
-print(config.host)
-```
-In PyCharm, and hopefully other IDEs, it will recognise the datatypes of your configuration and allow you to autocomplete. No more remembering strings to get the right thing out!
-
-## Upgrading from 0.x.x
-There is one breaking change when moving from `0.x.x` to `1.x.x`. The `key` function now expects all arguments to be keyword arguments. So simply replace any calls like so:
-```python
-key('section', 'key', True, str, 'default')  # 0.x.x
-key(section_name='section', key_name='key', required=True, cast=str, default='default')  # 1.x.x
-```
-The reason for this change is to tie down the return type of `key` properly. Previously, when `required=False` or when `cast=None` the return type would not include the possibility of `None` or `string`. The type checker should now be able to infer the return type based on the values of `required`, `cast` and `default`.
-
-## How it works
-Configuration is always supplied in a two level structure, so your source configuration can have multiple sections, and each section contains multiple key/value configuration pairs. For example:
-```ini
-[database]
-host = 127.0.0.1
-port = 2000
-
-[algorithm]
-max_value = 10
-min_value = 20
-```
-
-You then create your configuration hierarchy in code (this can be flat or many levels deep) and supply the matching between strings in your config sources and properties of your configuration classes.
-
-You provide one or more `ConfigSource`s, from which the config for your application can be read. For example, you might supply an `EnvironmentConfigSource`,  and two `IniFileConfigSource`s. This would make your application first look for a configuration value in environment variables, if not found there it would then look at the first INI file (perhaps a user-specific file), before falling back to the second INI file (perhaps a default configuration shared between all users). If a parameter is still not found and is a required parameter, an error would be thrown.
-
-There is emphasis on type information being available for everything so that an IDE will autocomplete when trying to use your config across your application.
-
-### Multiple data sources
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-    username = key(cast=str)
-    password = key(cast=str)
-
-config = DatabaseConfig()
-config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-config.add_source(IniFileConfigSource("config.cfg"))
-
-# OR provide sources directly to the constructor
-config = DatabaseConfig(sources=[
-    EnvironmentConfigSource(prefix="EXAMPLE"),
-    IniFileConfigSource("config.cfg")
-])
-```
-
-Since you don't want to hard code your secret credentials, you might supply them through the environment.
-So for the above configuration, the environment might look like this:
-```bash
-export EXAMPLE_DATABASE_USERNAME=my_username
-export EXAMPLE_DATABASE_PASSWORD=my_very_secret_password
-export EXAMPLE_DATABASE_PORT=2001
-```
-
-Those values which couldn't be found in the environment would then be read from the INI file, which might look like this:
-```ini
-[database]
-HOST = db1.mydomain.com
-PORT = 2000
-```
-
-Note after this, `config.port` will be equal to `2001` as the value in the environment took priority over the value in the INI file.
-
-### Caching
-When config values are first used, they are read. This is lazy evaluation by default so that not everything is read if not necessary.
-
-After first use, they are cached in memory so that there should be no further I/O if the config value is used again.
-
-For fail fast behaviour, and also to stop unexpected latency when a config value is read partway through your application (e.g. your config could be coming across a network), the option is available to read all config values at the start. Just call
-
-`config.read()`
-
-This will throw an exception if any required config value cannot be found, and will also keep all read config values in memory for next time they are used. If you do not use `read` you will only get the exception when you first try to use the offending config key.
-
-### Hierarchical configuration
-Use `group_key` to represent a "sub-config" of a configuration. Set up "sub-configs" exactly as demonstrated above, and then create a parent config to compose them in one place.
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-
-@section('algorithm')
-class AlgorithmConfig(Config):
-    max_value = key(cast=float)
-    min_value = key(cast=float)
-
-class ParentConfig(Config):
-    database = group_key(DatabaseConfig)
-    algorithm = group_key(AlgorithmConfig)
-    description = key(cast=str, section_name="general")
-
-config = ParentConfig()
-config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-config.add_source(IniFileConfigSource("config.cfg"))
-config.read()
-```
-
-The first time the `config.database` or `config.algorithm` is accessed (which in the case above is when `read()` is called), then an instance will be instantiated. Notice that it is the class definition, not an instance of the class, which is passed to the `group_key` function.
-
-### Custom section/key names, optional parameters, default values
-Let's take a look at this:
-```python
-from typedconfig import Config, key, section
-
-@section('database')
-class AppConfig(Config):
-    host1 = key()
-    host2 = key(section_name='database', key_name='HOST2',
-                required=True, cast=str, default=None)
-```
-Both `host1` and `host2` are legitimate configuration key definitions.
-
-* `section_name` - this name of the section in the configuration source from which this parameter should be read. This can be provided on a key-by-key basis, but if it is left out then the section name supplied by the `@section` decorator is used. If all keys supply a `section_name`, the class decorator is not needed. If both `section_name` and a decorator are provided, the `section_name` argument takes priority.
-* `key_name` - the name of this key in the configuration source from which this parameter is read. If not supplied, some magic uses the object property name as the key name.
-* `required` - default True. If False, and the configuration value can't be found, no error will be thrown and the default value will be used, if provided. If a default not provided, `None` will be used.
-* `cast` - probably the most important option for typing. **If you want autocomplete typing support you must specify this**. It's just a function which takes a string as an input and returns a parsed value. See the casting section for more. If not supplied, the value remains as a string.
-* `default` - only applicable if `required` is false. When `required` is false this value is used if a value cannot be found.
-
-### Types
-```python
-from typedconfig import Config, key, section
-from typing import List
-
-def split_str(s: str) -> List[str]:
-    return [x.strip() for x in s.split(",")]
-
-@section('database')
-class AppConfig(Config):
-    host = key()
-    port = key(cast=int)
-    users = key(cast=split_str)
-    zero_based_index = key(cast=lambda x: int(x)-1)
-config = AppConfig(sources=[...])
-```
-In this example we have three ways of casting:
-1. Not casting at all. This defaults to returning a `str`, but your IDE won't know that so if you want type hints use `cast=str`
-2. Casting to an built in type which can take a string input and parse it, for example `int`
-3. Defining a custom function. Your function should take one string input and return one output of any type. To get type hint, just make sure your function has type annotations.
-4. Using a lambda expression. The type inference may or may not work depending on your expression, so if it doesn't just write it as a function with type annotations.
-
-### Validation
-You can validate what has been supplied by providing a custom `cast` function to a `key`, which validates the configuration value in addition to parsing it.
-
-### Extending configuration using shared ConfigProvider
-
-Multiple application modules may use different configuration schemes while sharing the same configuration source. Analogously, various `Config` classes may provide different view of the same configuration data, sharing the same `ConfigProvider`.
-
-```python
-# app/config.py
-from typedconfig.provider import ConfigProvider
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-provider = ConfigProvider()
-provider.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-provider.add_source(IniFileConfigSource("config.cfg"))
-
-__all__ = ["provider"]
-```
-```python
-# app/database/config.py
-from typedconfig import Config, key, section
-from app.config import provider
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-
-database_config = DatabaseConfig(provider=provider)
-```
-```python
-# app/algorithm/config.py
-from typedconfig import Config, key, section
-from app.config import provider
-
-@section('algorithm')
-class AlgorithmConfig(Config):
-    max_value = key(cast=float)
-    min_value = key(cast=float)
-
-algorithm_config = AlgorithmConfig(provider=provider)
-```
-
-Shared configuration provider can be used by plugins, which may need to declare additional configuration sections within the same configuration files as the main application.  Let's assume we have `[database]` section used by main application and `[app_extension]` that provides 3rd party plugin configuration:
-
-```ini
-[database]
-host = 127.0.0.1
-port = 2000
-
-[app_extension]
-api_key = secret
-```
-
-e.g. `app/config.py` may look like that:
-
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    """Database configuration"""
-    host = key(cast=str)
-    port = key(cast=int)
-
-class ApplicationConfig(Config):
-    """Main configuration object"""
-    database = group_key(DatabaseConfig)
-
-app_config = ApplicationConfig(sources=[
-    EnvironmentConfigSource(),
-    IniFileConfigSource("config.cfg")
-])
-```
-
-and plugin can read additional sections by using the same configuration provider as main application config.
-
-e.g. `plugin/config.py`:
-```python
-from typedconfig import Config, key, section, group_key
-
-from app.config import ApplicationConfig, app_config
-
-@section('app_extension')
-class ExtensionConfig(Config):
-    """Extension configuration"""
-    api_key = key(cast=str)
-
-# ExtendedAppConfig extends ApplicationConfig 
-# so original sections are also included
-class ExtendedAppConfig(ApplicationConfig):
-    """Extended main configuration object"""
-    app_extension = group_key(ExtensionConfig)
-    
-# ExtendedAppConfig uses the same provider as the main app_config
-extended_config = ExtendedAppConfig(provider=app_config.provider)
-```
-```python
-from plugin.config import extended_config
-
-# Plugin can access both main and extra sections
-print(extended_config.app_extension.api_key)
-print(extended_config.database.host)
-```
-
-### Configuration variables which depend on other configuration variables
-Sometimes you may wish to set the value of some configuration variables based on others. You may also wish to validate some variables, for example allowed values may be different depending on the value of another config variable. For this you can add a `post_read_hook`.
-
-The default implementation of `post_read_hook` returns an empty `dict`. You can override this by implementing your own `post_read_hook` method. It should receive only `self` as an input, and return a `dict`. This `dict` should be a simple mapping from config keys to values. For hierarchical configurations, you can nest the dictionaries. If you provide a `post_read_hook` in both a parent and a child class which both make changes to the same keys (don't do this) then the values returned by the child method will overwrite those by the parent.
-
-This hook is called whenever you call the `read` method. If you use lazy loading and skip calling the `read` method, you cannot use this hook.
-```python
-# my_app/config.py
-from typedconfig import Config, key, group_key, section
-from typedconfig.source import EnvironmentConfigSource
-
-@section('child')
-class ChildConfig(Config):
-    http_port_plus_one = key(cast=int, required=False)
-
-@section('app')
-class AppConfig(Config):
-    use_https = key(cast=bool)
-    http_port = key(key_name='port', cast=int, required=False)
-    child = group_key(ChildConfig)
-    
-    def post_read_hook(self) -> dict:
-        config_updates = dict()
-        # If the port has not been provided, set it based on the value of use_https
-        if self.http_port is None:
-            config_updates.update(http_port=443 if self.use_https else 80)
-        else:
-            # Modify child config
-            config_updates.update(child=dict(http_port_plus_one=self.http_port + 1))
-            
-        # Validate that the port number has a sensible value
-        # It is recommended to do validation inside the cast method for individual keys, however for dependent keys it can be useful here
-        if self.http_port is not None:
-            if self.use_https:
-                assert self.http_port in [443, 444, 445]
-            else:
-                assert self.http_port in [80, 81, 82]
-
-        return config_updates
-            
-config = AppConfig()
-config.add_source(EnvironmentConfigSource())
-config.read()
-```
-
-## Configuration Sources
-Configuration sources are how your main `Config` class knows where to get its data from. These are totally extensible so that you can read in your configuration from wherever you like - from a database, from S3, anywhere that you can write code for.
-
-You supply your configuration source to your config after you've instantiated it, but **before** you try to read any data from it:
-```python
-config = AppConfig()
-config.add_source(my_first_source)
-config.add_source(my_second_source)
-config.read()
-```
-Or you can supply the sources directly in the constructor like this:
-```python
-config = AppConfig(sources=[my_first_source, my_second_source])
-config.read()
-```
-
-
-### Modifying or refreshing configuration after it has been loaded
-In general it is bad practice to modify configuration at runtime because the configuration for your program should be fixed for the duration of it.  However, there are cases where it may be necessary.
-
-To completely replace the set of config sources, you can use
-```python
-config = AppConfig(sources=[my_first_source, my_second_source])
-config.set_sources([my_first_new_source, my_second_new_source])
-```
-
-To replace a specific config source, for example because a config file has changed and you need to re-read it from disk, you can use `replace_source`:
-```python
-from typedconfig.source import IniFileConfigSource
-original_source = IniFileConfigSource("config.cfg")
-config = AppConfig(sources=[source])
-# Now say you change the contents to config.cfg and need to read it again
-new_source = IniFileConfigSource("config.cfg")  # re-reads file during construction
-config.replace_source(original_source, new_source)
-```
-
-**Important**: if you add or modify the config sources the config has been read, or need to refresh the config for some reason, you'll need to clear any cached values in order to force the config to be fetched from the `ConfigSource`s again. You can do this by
-```python
-config.clear_cache()
-config.read()          # Read all configuration values again
-```
-
-
-
-### Supplied Config Sources
-#### `EnvironmentConfigSource`
-This just reads configuration from environment variables.
-```python
-from typedconfig.source import EnvironmentConfigSource
-source = EnvironmentConfigSource(prefix="XYZ")
-# OR just
-source = EnvironmentConfigSource()
-```
-It just takes one optional input argument, a prefix. This can be useful to avoid name clashes in environment variables.
-
-* If prefix is provided, environment variables are expected to look like `{PREFIX}_{SECTION}_{KEY}`, for example `export XYZ_DATABASE_PORT=2000`. 
-* If no prefix is provided, environment variables should look like `{SECTION}_{KEY}`, for example `export DATABASE_PORT=2000`.
-
-#### `IniFileConfigSource`
-This reads from an INI file using Python's built in [configparser](https://docs.python.org/3/library/configparser.html). Read the docs for `configparser` for more about the structure of the file.
-```python
-from typedconfig.source import IniFileConfigSource
-source = IniFileConfigSource("config.cfg", encoding='utf-8', must_exist=True)
-```
-
-* The first argument is the filename (absolute or relative to the current working directory).
-* `encoding` is the text encoding of the file. `configparser`'s default is used if not supplied.
-* `must_exist` - default `True`. If the file can't be found, an error will be thrown by default. Setting `must_exist` to be `False` allows the file not to be present, in which case this source will just report that it can't find any configuration values and your `Config` class will move onto looking in the next `ConfigSource`.
-
-#### `IniStringConfigSource`
-This reads from a string instead of a file
-```python
-from typedconfig.source import IniStringConfigSource
-source = IniStringConfigSource("""
-[section_name]
-key_name=key_value
-""")
-```
-
-#### `DictConfigSource`
-The most basic source, entirely in memory, and also useful when writing tests. It is case insensitive.
-```python
-from typedconfig.source import DictConfigSource
-source = DictConfigSource({
-    'database': dict(HOST='db1', PORT='2000'),
-    'algorithm': dict(MAX_VALUE='20', MIN_VALUE='10')
-})
-```
-
-It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
-
-This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
-
-#### `CmdConfigSource`
-This reads configuration from command line arguments
-```python
-from typedconfig.source import CmdConfigSource
-source = CmdConfigSource(prefix="XYZ")
-# OR just
-source = CmdConfigSource()
-```
-
-It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
-
-* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
-* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
-
-The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
-
-### Writing your own `ConfigSource`s
-An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
-
-Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
-```python
-import json
-from typing import Optional
-from typedconfig.source import ConfigSource
-
-class JsonConfigSource(ConfigSource):
-    def __init__(self, filename: str):
-        # Read data - will raise an exception if problem with file
-        with open(filename, 'r') as f:
-            self.data = json.load(f)
-        # Quick checks on data format
-        assert type(self.data) is dict
-        for k, v in self.data.items():
-            assert type(k) is str
-            assert type(v) is dict
-            for v_k, v_v in v.items():
-                assert type(v_k) is str
-                assert type(v_v) is str
-        # Convert all keys to lowercase
-        self.data = {
-            k.lower(): {
-                v_k.lower(): v_v
-                for v_k, v_v in v.items()
-            }
-            for k, v in self.data.items()
-        }    
-
-    def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
-        # Extract info from data which we read in during __init__
-        section = self.data.get(section_name.lower(), None)
-        if section is None:
-            return None
-        return section.get(key_name.lower(), None)
-```
-
-### Additional config sources
-In order to keep `typed-config` dependency free, `ConfigSources` requiring additional dependencies are in separate packages, which also have `typed-config` as a dependency.
-
-These are listed here:
-
-| pip install name | import name | Description |
-| --- | --- | --- |
-| [typed-config-aws-sources](https://pypi.org/project/typed-config-aws-sources) | `typedconfig_awssource` | Config sources using `boto3` to get config e.g. from S3 or DynamoDB
-
-
-## Cast function library
-The `typedconfig.casts` module contains helper functions that implement common casting operations. These would generally be passed to the `cast` parameter of the `key()` function
-
-### Casting to an `Enum` type with `enum_cast`
-the `enum_cast` function converts a string input from a source to a member of an `Enum` type. 
-
-For example:
-```python
-from enum import Enum
-from typedconfig.casts import enum_cast
-from typedconfig import Config, key
-...
-class ColorEnum(Enum):
-    RED = 1
-    GREEN = 2
-    BLUE = 3
-...
-
-class MyConfig(Config):
-    color = key(cast=enum_cast(ColorEnum))
-```
-
-In this example, if the `ConfigSource` reads the string `"RED"`, the value of `color` will be set to `ColorEnum.RED`
-
-Note that the `enum_cast` function is designed to read the *name* of an enum member, not its value (`1`, `2` or `3` in the example above)
-
-### Casting to a `tuple` with `tuple_cast`
-If the source contains a list of items, `tuple_cast` will parse them as a python tuple, optionally applying a 
-base_cast function to each element. 
-The default behavior is to call strip() on each element and ignore trailing delimiters.
-
-For example, given the input
-```ini
-nums = 1, 2, 3, 4,
-```
-
-Then you could use
-
-```python
-nums = key(cast=tuple_cast())
-```
-to read the string input and cast it to `("1", "2", "3", "4")`
-
-```python
-key(cast=tuple_cast(base_cast=int))
-```
-Would cast the input to `(1, 2, 3, 4)`
-
-```python
-key(cast=tuple_cast(ignore_trailing_delimiter=False))
-```
-Would cast the input to `("1", "2", "3", "4", "")`
-
-```python
-key(cast=tuple_cast(strip=False))
-```
-Would cast the input to `("1", " 2", " 3", " 4")`
-
-Finally, if a delimiter other that "," is used - say the input string is `"1:2:3:4"` - that can be handled like
-```python
-key(cast=tuple_cast(delimiter=":"))
-```
-
-### Casting to a `bool` with `boolean_cast`
-
-If the source is a boolean value, it can be converted to Python's `True` or `False` using this cast.
-
-```python
-key(cast=boolean_cast)
-```
-
-`boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
-
-Value | Strings
---- | ---
-`True` | `"true"`, `"yes"`, `"on"`, `"1"`
-`False` | `"false"`, `"no"`, `"off"`, `"0"`
-
-### Casting to an `Optional[bool]` with `optional_boolean_cast`
-
-If the source is a boolean value which can also be `None`, it can be converted to Python's `True` or `False` or `None` using this cast.
-
-```python
-key(cast=optional_boolean_cast)
-```
-
-`optional_boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
-
-Value | Strings
---- | ---
-`True` | `"true"`, `"yes"`, `"on"`, `"1"`
-`False` | `"false"`, `"no"`, `"off"`, `"0"`
-`None` | `"none"`, `"unknown"`
-
-
-## Contributing
-Ideas for new features and pull requests are welcome. PRs must come with tests included. This was developed using Python 3.7 but Travis tests run with all versions 3.6-3.9 too.
-
-### Development setup
-1. Clone the git repository
-2. Create a virtual environment `virtualenv venv`
-3. Activate the environment `venv/scripts/activate`
-4. Install development dependencies `pip install -r requirements.txt`
-
-### Code style
-Code style is `black` and this is checked by the CI. To autoformat your code as `black` before committing, just run `black typedconfig test`
-
-### Running tests
-`pytest`
-
-To run with coverage:
-
-`pytest --cov`
-
-### Making a release
-1. Bump version number in `typedconfig/__version__.py`
-1. Add changes to [CHANGELOG.md](CHANGELOG.md)
-1. Commit your changes and tag with `git tag -a v0.1.0 -m "Summary of changes"`
-1. Travis will deploy the release to PyPi for you.
-
-#### Staging release
-If you want to check how a release will look on PyPi before tagging and making it live, you can do the following:
-1. `pip install twine` if you don't already have it
-1. Bump version number in `typedconfig/__version__.py`
-1. Clear the dist directory `rm -r dist`
-1. `python setup.py sdist bdist_wheel`
-1. `twine check dist/*`
-1. Upload to the test PyPI `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
-1. Check all looks ok at [https://test.pypi.org/project/typed-config](https://test.pypi.org/project/typed-config)
-1. If all looks good you can git tag and push for deploy to live PyPi
-
-Here is [a good tutorial](https://realpython.com/pypi-publish-python-package) on publishing packages to PyPI.
+Metadata-Version: 2.1
+Name: typed-config
+Version: 2.0.3
+Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
+Home-page: https://github.com/bwindsor/typed-config
+Author: Ben Windsor
+Author-email: 
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Build Status](https://github.com/bwindsor/typed-config/actions/workflows/unit_test.yml/badge.svg)
+![Deploy Status](https://github.com/bwindsor/typed-config/actions/workflows/deploy_pypi.yml/badge.svg)
+[![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
+
+# typed-config
+Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
+
+`pip install typed-config`
+
+Requires python 3.6 or above. (Also, needs `typing_extensions` for Python <= 3.7, so not completely dependency free if using old Python).
+
+## Basic usage
+```python
+# my_app/config.py
+from typedconfig import Config, key, section
+from typedconfig.source import EnvironmentConfigSource
+
+@section('database')
+class AppConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+    timeout = key(cast=float)
+
+config = AppConfig()
+config.add_source(EnvironmentConfigSource())
+config.read()
+```
+
+```python
+# my_app/main.py
+from my_app.config import config
+print(config.host)
+```
+In PyCharm, and hopefully other IDEs, it will recognise the datatypes of your configuration and allow you to autocomplete. No more remembering strings to get the right thing out!
+
+## Upgrading
+
+### From 0.x.x
+There is one breaking change when moving from `0.x.x` to `1.x.x`. The `key` function now expects all arguments to be keyword arguments. So simply replace any calls like so:
+```python
+key('section', 'key', True, str, 'default')  # 0.x.x
+key(section_name='section', key_name='key', required=True, cast=str, default='default')  # 1.x.x
+```
+The reason for this change is to tie down the return type of `key` properly. Previously, when `required=False` or when `cast=None` the return type would not include the possibility of `None` or `string`. The type checker should now be able to infer the return type based on the values of `required`, `cast` and `default`.
+
+###  From 1.x.x
+When upgrading from `1.x.x` to `2.x.x`, Python 3.7 no longer supported as it is end of life. As long as you are using Python >= 3.8, everything should just work.
+
+## How it works
+Configuration is always supplied in a two level structure, so your source configuration can have multiple sections, and each section contains multiple key/value configuration pairs. For example:
+```ini
+[database]
+host = 127.0.0.1
+port = 2000
+
+[algorithm]
+max_value = 10
+min_value = 20
+```
+
+You then create your configuration hierarchy in code (this can be flat or many levels deep) and supply the matching between strings in your config sources and properties of your configuration classes.
+
+You provide one or more `ConfigSource`s, from which the config for your application can be read. For example, you might supply an `EnvironmentConfigSource`,  and two `IniFileConfigSource`s. This would make your application first look for a configuration value in environment variables, if not found there it would then look at the first INI file (perhaps a user-specific file), before falling back to the second INI file (perhaps a default configuration shared between all users). If a parameter is still not found and is a required parameter, an error would be thrown.
+
+There is emphasis on type information being available for everything so that an IDE will autocomplete when trying to use your config across your application.
+
+### Multiple data sources
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+    username = key(cast=str)
+    password = key(cast=str)
+
+config = DatabaseConfig()
+config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+config.add_source(IniFileConfigSource("config.cfg"))
+
+# OR provide sources directly to the constructor
+config = DatabaseConfig(sources=[
+    EnvironmentConfigSource(prefix="EXAMPLE"),
+    IniFileConfigSource("config.cfg")
+])
+```
+
+Since you don't want to hard code your secret credentials, you might supply them through the environment.
+So for the above configuration, the environment might look like this:
+```bash
+export EXAMPLE_DATABASE_USERNAME=my_username
+export EXAMPLE_DATABASE_PASSWORD=my_very_secret_password
+export EXAMPLE_DATABASE_PORT=2001
+```
+
+Those values which couldn't be found in the environment would then be read from the INI file, which might look like this:
+```ini
+[database]
+HOST = db1.mydomain.com
+PORT = 2000
+```
+
+Note after this, `config.port` will be equal to `2001` as the value in the environment took priority over the value in the INI file.
+
+### Caching
+When config values are first used, they are read. This is lazy evaluation by default so that not everything is read if not necessary.
+
+After first use, they are cached in memory so that there should be no further I/O if the config value is used again.
+
+For fail fast behaviour, and also to stop unexpected latency when a config value is read partway through your application (e.g. your config could be coming across a network), the option is available to read all config values at the start. Just call
+
+`config.read()`
+
+This will throw an exception if any required config value cannot be found, and will also keep all read config values in memory for next time they are used. If you do not use `read` you will only get the exception when you first try to use the offending config key.
+
+### Hierarchical configuration
+Use `group_key` to represent a "sub-config" of a configuration. Set up "sub-configs" exactly as demonstrated above, and then create a parent config to compose them in one place.
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+
+@section('algorithm')
+class AlgorithmConfig(Config):
+    max_value = key(cast=float)
+    min_value = key(cast=float)
+
+class ParentConfig(Config):
+    database = group_key(DatabaseConfig)
+    algorithm = group_key(AlgorithmConfig)
+    description = key(cast=str, section_name="general")
+
+config = ParentConfig()
+config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+config.add_source(IniFileConfigSource("config.cfg"))
+config.read()
+```
+
+The first time the `config.database` or `config.algorithm` is accessed (which in the case above is when `read()` is called), then an instance will be instantiated. Notice that it is the class definition, not an instance of the class, which is passed to the `group_key` function.
+
+### Custom section/key names, optional parameters, default values
+Let's take a look at this:
+```python
+from typedconfig import Config, key, section
+
+@section('database')
+class AppConfig(Config):
+    host1 = key()
+    host2 = key(section_name='database', key_name='HOST2',
+                required=True, cast=str, default=None)
+```
+Both `host1` and `host2` are legitimate configuration key definitions.
+
+* `section_name` - this name of the section in the configuration source from which this parameter should be read. This can be provided on a key-by-key basis, but if it is left out then the section name supplied by the `@section` decorator is used. If all keys supply a `section_name`, the class decorator is not needed. If both `section_name` and a decorator are provided, the `section_name` argument takes priority.
+* `key_name` - the name of this key in the configuration source from which this parameter is read. If not supplied, some magic uses the object property name as the key name.
+* `required` - default True. If False, and the configuration value can't be found, no error will be thrown and the default value will be used, if provided. If a default not provided, `None` will be used.
+* `cast` - probably the most important option for typing. **If you want autocomplete typing support you must specify this**. It's just a function which takes a string as an input and returns a parsed value. See the casting section for more. If not supplied, the value remains as a string.
+* `default` - only applicable if `required` is false. When `required` is false this value is used if a value cannot be found.
+
+### Types
+```python
+from typedconfig import Config, key, section
+from typing import List
+
+def split_str(s: str) -> List[str]:
+    return [x.strip() for x in s.split(",")]
+
+@section('database')
+class AppConfig(Config):
+    host = key()
+    port = key(cast=int)
+    users = key(cast=split_str)
+    zero_based_index = key(cast=lambda x: int(x)-1)
+config = AppConfig(sources=[...])
+```
+In this example we have three ways of casting:
+1. Not casting at all. This defaults to returning a `str`, but your IDE won't know that so if you want type hints use `cast=str`
+2. Casting to an built in type which can take a string input and parse it, for example `int`
+3. Defining a custom function. Your function should take one string input and return one output of any type. To get type hint, just make sure your function has type annotations.
+4. Using a lambda expression. The type inference may or may not work depending on your expression, so if it doesn't just write it as a function with type annotations.
+
+### Validation
+You can validate what has been supplied by providing a custom `cast` function to a `key`, which validates the configuration value in addition to parsing it.
+
+### Extending configuration using shared ConfigProvider
+
+Multiple application modules may use different configuration schemes while sharing the same configuration source. Analogously, various `Config` classes may provide different view of the same configuration data, sharing the same `ConfigProvider`.
+
+```python
+# app/config.py
+from typedconfig.provider import ConfigProvider
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+provider = ConfigProvider()
+provider.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+provider.add_source(IniFileConfigSource("config.cfg"))
+
+__all__ = ["provider"]
+```
+```python
+# app/database/config.py
+from typedconfig import Config, key, section
+from app.config import provider
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+
+database_config = DatabaseConfig(provider=provider)
+```
+```python
+# app/algorithm/config.py
+from typedconfig import Config, key, section
+from app.config import provider
+
+@section('algorithm')
+class AlgorithmConfig(Config):
+    max_value = key(cast=float)
+    min_value = key(cast=float)
+
+algorithm_config = AlgorithmConfig(provider=provider)
+```
+
+Shared configuration provider can be used by plugins, which may need to declare additional configuration sections within the same configuration files as the main application.  Let's assume we have `[database]` section used by main application and `[app_extension]` that provides 3rd party plugin configuration:
+
+```ini
+[database]
+host = 127.0.0.1
+port = 2000
+
+[app_extension]
+api_key = secret
+```
+
+e.g. `app/config.py` may look like that:
+
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    """Database configuration"""
+    host = key(cast=str)
+    port = key(cast=int)
+
+class ApplicationConfig(Config):
+    """Main configuration object"""
+    database = group_key(DatabaseConfig)
+
+app_config = ApplicationConfig(sources=[
+    EnvironmentConfigSource(),
+    IniFileConfigSource("config.cfg")
+])
+```
+
+and plugin can read additional sections by using the same configuration provider as main application config.
+
+e.g. `plugin/config.py`:
+```python
+from typedconfig import Config, key, section, group_key
+
+from app.config import ApplicationConfig, app_config
+
+@section('app_extension')
+class ExtensionConfig(Config):
+    """Extension configuration"""
+    api_key = key(cast=str)
+
+# ExtendedAppConfig extends ApplicationConfig 
+# so original sections are also included
+class ExtendedAppConfig(ApplicationConfig):
+    """Extended main configuration object"""
+    app_extension = group_key(ExtensionConfig)
+    
+# ExtendedAppConfig uses the same provider as the main app_config
+extended_config = ExtendedAppConfig(provider=app_config.provider)
+```
+```python
+from plugin.config import extended_config
+
+# Plugin can access both main and extra sections
+print(extended_config.app_extension.api_key)
+print(extended_config.database.host)
+```
+
+### Configuration variables which depend on other configuration variables
+Sometimes you may wish to set the value of some configuration variables based on others. You may also wish to validate some variables, for example allowed values may be different depending on the value of another config variable. For this you can add a `post_read_hook`.
+
+The default implementation of `post_read_hook` returns an empty `dict`. You can override this by implementing your own `post_read_hook` method. It should receive only `self` as an input, and return a `dict`. This `dict` should be a simple mapping from config keys to values. For hierarchical configurations, you can nest the dictionaries. If you provide a `post_read_hook` in both a parent and a child class which both make changes to the same keys (don't do this) then the values returned by the child method will overwrite those by the parent.
+
+This hook is called whenever you call the `read` method. If you use lazy loading and skip calling the `read` method, you cannot use this hook.
+```python
+# my_app/config.py
+from typedconfig import Config, key, group_key, section
+from typedconfig.source import EnvironmentConfigSource
+
+@section('child')
+class ChildConfig(Config):
+    http_port_plus_one = key(cast=int, required=False)
+
+@section('app')
+class AppConfig(Config):
+    use_https = key(cast=bool)
+    http_port = key(key_name='port', cast=int, required=False)
+    child = group_key(ChildConfig)
+    
+    def post_read_hook(self) -> dict:
+        config_updates = dict()
+        # If the port has not been provided, set it based on the value of use_https
+        if self.http_port is None:
+            config_updates.update(http_port=443 if self.use_https else 80)
+        else:
+            # Modify child config
+            config_updates.update(child=dict(http_port_plus_one=self.http_port + 1))
+            
+        # Validate that the port number has a sensible value
+        # It is recommended to do validation inside the cast method for individual keys, however for dependent keys it can be useful here
+        if self.http_port is not None:
+            if self.use_https:
+                assert self.http_port in [443, 444, 445]
+            else:
+                assert self.http_port in [80, 81, 82]
+
+        return config_updates
+            
+config = AppConfig()
+config.add_source(EnvironmentConfigSource())
+config.read()
+```
+
+## Configuration Sources
+Configuration sources are how your main `Config` class knows where to get its data from. These are totally extensible so that you can read in your configuration from wherever you like - from a database, from S3, anywhere that you can write code for.
+
+You supply your configuration source to your config after you've instantiated it, but **before** you try to read any data from it:
+```python
+config = AppConfig()
+config.add_source(my_first_source)
+config.add_source(my_second_source)
+config.read()
+```
+Or you can supply the sources directly in the constructor like this:
+```python
+config = AppConfig(sources=[my_first_source, my_second_source])
+config.read()
+```
+
+
+### Modifying or refreshing configuration after it has been loaded
+In general it is bad practice to modify configuration at runtime because the configuration for your program should be fixed for the duration of it.  However, there are cases where it may be necessary.
+
+To completely replace the set of config sources, you can use
+```python
+config = AppConfig(sources=[my_first_source, my_second_source])
+config.set_sources([my_first_new_source, my_second_new_source])
+```
+
+To replace a specific config source, for example because a config file has changed and you need to re-read it from disk, you can use `replace_source`:
+```python
+from typedconfig.source import IniFileConfigSource
+original_source = IniFileConfigSource("config.cfg")
+config = AppConfig(sources=[source])
+# Now say you change the contents to config.cfg and need to read it again
+new_source = IniFileConfigSource("config.cfg")  # re-reads file during construction
+config.replace_source(original_source, new_source)
+```
+
+**Important**: if you add or modify the config sources the config has been read, or need to refresh the config for some reason, you'll need to clear any cached values in order to force the config to be fetched from the `ConfigSource`s again. You can do this by
+```python
+config.clear_cache()
+config.read()          # Read all configuration values again
+```
+
+
+
+### Supplied Config Sources
+#### `EnvironmentConfigSource`
+This just reads configuration from environment variables.
+```python
+from typedconfig.source import EnvironmentConfigSource
+source = EnvironmentConfigSource(prefix="XYZ")
+# OR just
+source = EnvironmentConfigSource()
+```
+It just takes one optional input argument, a prefix. This can be useful to avoid name clashes in environment variables.
+
+* If prefix is provided, environment variables are expected to look like `{PREFIX}_{SECTION}_{KEY}`, for example `export XYZ_DATABASE_PORT=2000`. 
+* If no prefix is provided, environment variables should look like `{SECTION}_{KEY}`, for example `export DATABASE_PORT=2000`.
+
+#### `IniFileConfigSource`
+This reads from an INI file using Python's built in [configparser](https://docs.python.org/3/library/configparser.html). Read the docs for `configparser` for more about the structure of the file.
+```python
+from typedconfig.source import IniFileConfigSource
+source = IniFileConfigSource("config.cfg", encoding='utf-8', must_exist=True)
+```
+
+* The first argument is the filename (absolute or relative to the current working directory).
+* `encoding` is the text encoding of the file. `configparser`'s default is used if not supplied.
+* `must_exist` - default `True`. If the file can't be found, an error will be thrown by default. Setting `must_exist` to be `False` allows the file not to be present, in which case this source will just report that it can't find any configuration values and your `Config` class will move onto looking in the next `ConfigSource`.
+
+#### `IniStringConfigSource`
+This reads from a string instead of a file
+```python
+from typedconfig.source import IniStringConfigSource
+source = IniStringConfigSource("""
+[section_name]
+key_name=key_value
+""")
+```
+
+#### `DictConfigSource`
+The most basic source, entirely in memory, and also useful when writing tests. It is case insensitive.
+```python
+from typedconfig.source import DictConfigSource
+source = DictConfigSource({
+    'database': dict(HOST='db1', PORT='2000'),
+    'algorithm': dict(MAX_VALUE='20', MIN_VALUE='10')
+})
+```
+
+It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
+
+This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
+
+#### `CmdConfigSource`
+This reads configuration from command line arguments
+```python
+from typedconfig.source import CmdConfigSource
+source = CmdConfigSource(prefix="XYZ")
+# OR just
+source = CmdConfigSource()
+```
+
+It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
+
+* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
+* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
+
+The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
+
+### Writing your own `ConfigSource`s
+An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
+
+Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
+```python
+import json
+from typing import Optional
+from typedconfig.source import ConfigSource
+
+class JsonConfigSource(ConfigSource):
+    def __init__(self, filename: str):
+        # Read data - will raise an exception if problem with file
+        with open(filename, 'r') as f:
+            self.data = json.load(f)
+        # Quick checks on data format
+        assert type(self.data) is dict
+        for k, v in self.data.items():
+            assert type(k) is str
+            assert type(v) is dict
+            for v_k, v_v in v.items():
+                assert type(v_k) is str
+                assert type(v_v) is str
+        # Convert all keys to lowercase
+        self.data = {
+            k.lower(): {
+                v_k.lower(): v_v
+                for v_k, v_v in v.items()
+            }
+            for k, v in self.data.items()
+        }    
+
+    def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
+        # Extract info from data which we read in during __init__
+        section = self.data.get(section_name.lower(), None)
+        if section is None:
+            return None
+        return section.get(key_name.lower(), None)
+```
+
+### Additional config sources
+In order to keep `typed-config` dependency free, `ConfigSources` requiring additional dependencies are in separate packages, which also have `typed-config` as a dependency.
+
+These are listed here:
+
+| pip install name | import name | Description |
+| --- | --- | --- |
+| [typed-config-aws-sources](https://pypi.org/project/typed-config-aws-sources) | `typedconfig_awssource` | Config sources using `boto3` to get config e.g. from S3 or DynamoDB
+
+
+## Cast function library
+The `typedconfig.casts` module contains helper functions that implement common casting operations. These would generally be passed to the `cast` parameter of the `key()` function
+
+### Casting to an `Enum` type with `enum_cast`
+the `enum_cast` function converts a string input from a source to a member of an `Enum` type. 
+
+For example:
+```python
+from enum import Enum
+from typedconfig.casts import enum_cast
+from typedconfig import Config, key
+...
+class ColorEnum(Enum):
+    RED = 1
+    GREEN = 2
+    BLUE = 3
+...
+
+class MyConfig(Config):
+    color = key(cast=enum_cast(ColorEnum))
+```
+
+In this example, if the `ConfigSource` reads the string `"RED"`, the value of `color` will be set to `ColorEnum.RED`
+
+Note that the `enum_cast` function is designed to read the *name* of an enum member, not its value (`1`, `2` or `3` in the example above)
+
+### Casting to a `tuple` with `tuple_cast`
+If the source contains a list of items, `tuple_cast` will parse them as a python tuple, optionally applying a 
+base_cast function to each element. 
+The default behavior is to call strip() on each element and ignore trailing delimiters.
+
+For example, given the input
+```ini
+nums = 1, 2, 3, 4,
+```
+
+Then you could use
+
+```python
+nums = key(cast=tuple_cast())
+```
+to read the string input and cast it to `("1", "2", "3", "4")`
+
+```python
+key(cast=tuple_cast(base_cast=int))
+```
+Would cast the input to `(1, 2, 3, 4)`
+
+```python
+key(cast=tuple_cast(ignore_trailing_delimiter=False))
+```
+Would cast the input to `("1", "2", "3", "4", "")`
+
+```python
+key(cast=tuple_cast(strip=False))
+```
+Would cast the input to `("1", " 2", " 3", " 4")`
+
+Finally, if a delimiter other that "," is used - say the input string is `"1:2:3:4"` - that can be handled like
+```python
+key(cast=tuple_cast(delimiter=":"))
+```
+
+### Casting to a `bool` with `boolean_cast`
+
+If the source is a boolean value, it can be converted to Python's `True` or `False` using this cast.
+
+```python
+key(cast=boolean_cast)
+```
+
+`boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
+
+Value | Strings
+--- | ---
+`True` | `"true"`, `"yes"`, `"on"`, `"1"`
+`False` | `"false"`, `"no"`, `"off"`, `"0"`
+
+### Casting to an `Optional[bool]` with `optional_boolean_cast`
+
+If the source is a boolean value which can also be `None`, it can be converted to Python's `True` or `False` or `None` using this cast.
+
+```python
+key(cast=optional_boolean_cast)
+```
+
+`optional_boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
+
+Value | Strings
+--- | ---
+`True` | `"true"`, `"yes"`, `"on"`, `"1"`
+`False` | `"false"`, `"no"`, `"off"`, `"0"`
+`None` | `"none"`, `"unknown"`
+
+
+## Contributing
+Ideas for new features and pull requests are welcome. PRs must come with tests included. This is developed using Python 3.9 but Github actions will run tests with all versions 3.8-3.12 too.
+
+### Development setup
+1. Clone the git repository
+2. Create a virtual environment `virtualenv venv`
+3. Activate the environment `venv/scripts/activate`
+4. Install development dependencies `pip install -r requirements.txt`
+
+### Code style
+Code style is `black` and this is checked by the CI. To autoformat your code as `black` before committing, just run `black typedconfig test`
+
+### Running tests
+`pytest`
+
+To run with coverage:
+
+`pytest --cov`
+
+### Making a release
+1. Bump version number in `typedconfig/__version__.py`
+1. Add changes to [CHANGELOG.md](CHANGELOG.md)
+1. Commit your changes and tag with `git tag -a v0.1.0 -m "Summary of changes"`
+1. Github actions will deploy the release to PyPi for you.
+
+#### Staging release
+If you want to check how a release will look on PyPi before tagging and making it live, you can do the following:
+1. `pip install twine` if you don't already have it
+1. Bump version number in `typedconfig/__version__.py`
+1. Clear the dist directory `rm -r dist`
+1. `python setup.py sdist bdist_wheel`
+1. `twine check dist/*`
+1. Upload to the test PyPI `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
+1. Check all looks ok at [https://test.pypi.org/project/typed-config](https://test.pypi.org/project/typed-config)
+1. If all looks good you can git tag and push for deploy to live PyPi
+
+Here is [a good tutorial](https://realpython.com/pypi-publish-python-package) on publishing packages to PyPI.
```

### Comparing `typed-config-1.5.0/setup.py` & `typed-config-2.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from pathlib import Path
-from setuptools import setup
-from typedconfig.__version__ import __version__
-
-# The text of the README file
-readme_text = Path(__file__).with_name("README.md").read_text()
-
-setup(
-    name='typed-config',
-    version=__version__,
-    description='Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.',
-    long_description=readme_text,
-    long_description_content_type='text/markdown',
-    url='https://github.com/bwindsor/typed-config',
-    author='Ben Windsor',
-    author_email='',
-    python_requires='>=3.6.0',
-    license='MIT',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Topic :: Software Development',
-        'Typing :: Typed',
-    ],
-    packages=['typedconfig'],
-    package_data={'typedconfig': ['py.typed']},
-    install_requires=['typing-extensions >= 3.10.0; python_version < "3.8.0"'],
-    entry_points={}
-)
+from pathlib import Path
+from setuptools import setup
+from typedconfig.__version__ import __version__
+
+# The text of the README file
+readme_text = Path(__file__).with_name("README.md").read_text()
+
+setup(
+    name='typed-config',
+    version=__version__,
+    description='Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.',
+    long_description=readme_text,
+    long_description_content_type='text/markdown',
+    url='https://github.com/bwindsor/typed-config',
+    author='Ben Windsor',
+    author_email='',
+    python_requires='>=3.6.0',
+    license='MIT',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Development Status :: 4 - Beta',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Topic :: Software Development',
+        'Typing :: Typed',
+    ],
+    packages=['typedconfig'],
+    package_data={'typedconfig': ['py.typed']},
+    entry_points={}
+)
```

### Comparing `typed-config-1.5.0/test/test_config_source.py` & `typed-config-2.0.3/test/test_config_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import pytest
-import tempfile
-import os
-import sys
-from unittest.mock import patch
-from typedconfig.source import (
-    ConfigSource,
-    IniFileConfigSource,
-    IniStringConfigSource,
-    DictConfigSource,
-    EnvironmentConfigSource,
-    CmdConfigSource,
-)
-
-
-def do_assertions(source: ConfigSource, expected_repr: str):
-    v = source.get_config_value("s", "A")
-    assert "1" == v
-
-    v = source.get_config_value("s", "a")
-    assert "1" == v
-
-    v = source.get_config_value("s", "B")
-    assert "2" == v
-
-    v = source.get_config_value("s", "b")
-    assert "2" == v
-
-    v = source.get_config_value("t", "A")
-    assert v is None
-
-    v = source.get_config_value("s", "C")
-    assert v is None
-
-    assert repr(source) == expected_repr
-
-
-def test_dict_config_source():
-    source = DictConfigSource({"s": dict(A="1", b="2")})
-    do_assertions(source, "<DictConfigSource>")
-
-
-@pytest.mark.parametrize(
-    "encoding",
-    [
-        "utf8",
-        "windows-1252",
-    ],
-)
-def test_ini_file_config_source(encoding):
-    with tempfile.TemporaryDirectory() as td:
-        file_name = os.path.join(td, "config.cfg")
-        with open(file_name, "w", encoding=encoding) as f:
-            f.write(
-                """
-[s]
-a = 1
-B = 2
-"""
-            )
-
-        source = IniFileConfigSource(file_name, encoding=encoding)
-        do_assertions(source, f"<IniFileConfigSource(filename='{file_name}')>")
-
-
-def test_ini_file_config_source_no_file_existence_optional():
-    source = IniFileConfigSource("config-this-file-definitely-does-not-exist.cfg", must_exist=False)
-    v = source.get_config_value("s", "a")
-    assert v is None
-
-
-def test_ini_file_config_source_no_file_must_exist():
-    with pytest.raises(FileNotFoundError):
-        IniFileConfigSource("config-this-file-definitely-does-not-exist.cfg", must_exist=True)
-
-
-def test_ini_string_config_source():
-    source = IniStringConfigSource(
-        """
-[s]
-a = 1
-B = 2
-    """
-    )
-    do_assertions(source, "<IniStringConfigSource>")
-
-
-@patch.dict(os.environ, {"PREFIX_S_A": "1", "PREFIX_S_B": "2"})
-def test_environment_config_source_with_prefix():
-    source = EnvironmentConfigSource("PREFIX")
-    do_assertions(source, "<EnvironmentConfigSource(prefix='PREFIX')>")
-
-
-@patch.dict(os.environ, {"S_A": "1", "S_B": "2"})
-def test_environment_config_source():
-    source = EnvironmentConfigSource()
-    do_assertions(source, "<EnvironmentConfigSource(prefix='')>")
-
-
-@patch('sys.argv', ["name.py", "--S_A", "1", "another_thing", "--S_B", "2", "--extra", "hello", "--no_value"])
-def test_cmd_config_source():
-    source = CmdConfigSource()
-    do_assertions(source, "<CmdConfigSource(prefix='')>")
-
-
-@patch('sys.argv', ["name.py", "--prefix_S_A", "1", "--PREFiX_S_B", "2"])
-def test_cmd_config_source_with_prefix():
-    source = CmdConfigSource(prefix="PREFIX")
-    do_assertions(source, "<CmdConfigSource(prefix='PREFIX')>")
+import pytest
+import tempfile
+import os
+import sys
+from unittest.mock import patch
+from typedconfig.source import (
+    ConfigSource,
+    IniFileConfigSource,
+    IniStringConfigSource,
+    DictConfigSource,
+    EnvironmentConfigSource,
+    CmdConfigSource,
+)
+
+
+def do_assertions(source: ConfigSource, expected_repr: str):
+    v = source.get_config_value("s", "A")
+    assert "1" == v
+
+    v = source.get_config_value("s", "a")
+    assert "1" == v
+
+    v = source.get_config_value("s", "B")
+    assert "2" == v
+
+    v = source.get_config_value("s", "b")
+    assert "2" == v
+
+    v = source.get_config_value("t", "A")
+    assert v is None
+
+    v = source.get_config_value("s", "C")
+    assert v is None
+
+    assert repr(source) == expected_repr
+
+
+def test_dict_config_source():
+    source = DictConfigSource({"s": dict(A="1", b="2")})
+    do_assertions(source, "<DictConfigSource>")
+
+
+@pytest.mark.parametrize(
+    "encoding",
+    [
+        "utf8",
+        "windows-1252",
+    ],
+)
+def test_ini_file_config_source(encoding):
+    with tempfile.TemporaryDirectory() as td:
+        file_name = os.path.join(td, "config.cfg")
+        with open(file_name, "w", encoding=encoding) as f:
+            f.write(
+                """
+[s]
+a = 1
+B = 2
+"""
+            )
+
+        source = IniFileConfigSource(file_name, encoding=encoding)
+        do_assertions(source, f"<IniFileConfigSource(filename='{file_name}')>")
+
+
+def test_ini_file_config_source_no_file_existence_optional():
+    source = IniFileConfigSource("config-this-file-definitely-does-not-exist.cfg", must_exist=False)
+    v = source.get_config_value("s", "a")
+    assert v is None
+
+
+def test_ini_file_config_source_no_file_must_exist():
+    with pytest.raises(FileNotFoundError):
+        IniFileConfigSource("config-this-file-definitely-does-not-exist.cfg", must_exist=True)
+
+
+def test_ini_string_config_source():
+    source = IniStringConfigSource(
+        """
+[s]
+a = 1
+B = 2
+    """
+    )
+    do_assertions(source, "<IniStringConfigSource>")
+
+
+@patch.dict(os.environ, {"PREFIX_S_A": "1", "PREFIX_S_B": "2"})
+def test_environment_config_source_with_prefix():
+    source = EnvironmentConfigSource("PREFIX")
+    do_assertions(source, "<EnvironmentConfigSource(prefix='PREFIX')>")
+
+
+@patch.dict(os.environ, {"S_A": "1", "S_B": "2"})
+def test_environment_config_source():
+    source = EnvironmentConfigSource()
+    do_assertions(source, "<EnvironmentConfigSource(prefix='')>")
+
+
+@patch("sys.argv", ["name.py", "--S_A", "1", "another_thing", "--S_B", "2", "--extra", "hello", "--no_value"])
+def test_cmd_config_source():
+    source = CmdConfigSource()
+    do_assertions(source, "<CmdConfigSource(prefix='')>")
+
+
+@patch("sys.argv", ["name.py", "--prefix_S_A", "1", "--PREFiX_S_B", "2"])
+def test_cmd_config_source_with_prefix():
+    source = CmdConfigSource(prefix="PREFIX")
+    do_assertions(source, "<CmdConfigSource(prefix='PREFIX')>")
```

### Comparing `typed-config-1.5.0/test/test_configuration.py` & `typed-config-2.0.3/test/test_configuration.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,572 +1,572 @@
-import inspect
-import pytest
-from unittest.mock import MagicMock
-from typedconfig.config import Config, key, section, group_key, ConfigProvider
-from typedconfig.source import DictConfigSource, ConfigSource
-
-
-class GrandchildConfig(Config):
-    prop1 = key(section_name="grandchild", key_name="PROP1")
-
-
-class ChildConfig(Config):
-    prop1 = key(section_name="child", key_name="PROP1")
-    grandchild_config = group_key(GrandchildConfig)
-
-
-class ParentConfig(Config):
-    prop1 = key(section_name="parent", key_name="PROP1")
-    child_config = group_key(ChildConfig)
-
-
-def test_subclass_config():
-    class SampleConfig(Config):
-        prop1 = key(section_name="s", key_name="prop1", cast=float)
-        prop2 = key(section_name="s", key_name="prop2", cast=int)
-        prop3 = key(section_name="s", key_name="prop3", cast=str)
-        prop4 = key(section_name="s", key_name="prop4")
-
-    config_source = DictConfigSource({"s": {"PROP1": "3.5", "PROP2": "2", "PROP3": "hello", "PROP4": "abc"}})
-    config = SampleConfig()
-    config.add_source(config_source)
-
-    assert 3.5 == config.prop1
-    assert 2 == config.prop2
-    assert "hello" == config.prop3
-    assert "abc" == config.prop4
-
-
-def test_register_properties():
-    class SampleConfig(Config):
-        registerd_key1 = key(section_name="s", key_name="key1")
-        registerd_key2 = key(section_name="s", key_name="key2")
-
-        not_registered_key = 3
-
-        def not_registered_method(self):
-            pass
-
-    config = SampleConfig()
-    props = config.get_registered_properties()
-    assert sorted(["registerd_key1", "registerd_key2"]) == sorted(props)
-
-
-def test_register_composed_config():
-    class ChildConfig1(Config):
-        pass
-
-    class ChildConfig2(Config):
-        pass
-
-    class SampleConfig(Config):
-        composed_config1 = group_key(ChildConfig1)
-        composed_config2 = group_key(ChildConfig2)
-
-    config = SampleConfig()
-    sub_configs = config.get_registered_composed_config()
-    assert len(sub_configs) == 2
-    assert isinstance(sub_configs[0], ChildConfig1)
-    assert isinstance(sub_configs[1], ChildConfig2)
-
-    # Check we're not creating a new instance of the sub configs each time we call
-    sub_configs_2 = config.get_registered_composed_config()
-    assert sub_configs[0] is sub_configs_2[0]
-    assert sub_configs[1] is sub_configs_2[1]
-
-
-def test_reuse_child_config():
-    class SampleChildConfig(Config):
-        pass
-
-    class SampleConfig(Config):
-        composed_1 = group_key(SampleChildConfig)
-        composed_2 = group_key(SampleChildConfig)
-
-    config = SampleConfig()
-    config.read()
-
-    sub_configs = config.get_registered_composed_config()
-    assert len(sub_configs) == 2
-    assert isinstance(sub_configs[0], SampleChildConfig)
-    assert isinstance(sub_configs[1], SampleChildConfig)
-    assert sub_configs[0] is not sub_configs[1]
-
-
-@pytest.mark.parametrize(
-    "config_dict, expect_error",
-    [({}, True), ({"PROP1": "x"}, False), ({"PROP1": "x", "PROP2": "y"}, False)],
-    ids=["ConfigMissing", "PropertiesMatch", "ExtraConfig"],
-)
-def test_read(config_dict, expect_error):
-    class SampleConfig(Config):
-        prop1 = key(section_name="s", key_name="prop1")
-
-    config = SampleConfig()
-    config.add_source(DictConfigSource({"s": config_dict}))
-
-    if expect_error:
-        with pytest.raises(KeyError):
-            config.read()
-    else:
-        config.read()
-
-    if "PROP1" in config_dict:
-        assert config_dict["PROP1"] == config.prop1
-
-
-@pytest.mark.parametrize(
-    "prop_val, args, expected_value_or_error",
-    [
-        ("3", dict(), "3"),
-        (None, dict(), KeyError),
-        ("3", dict(required=True), "3"),
-        (None, dict(required=True), KeyError),
-        ("3", dict(required=False), "3"),
-        (None, dict(required=False), None),
-        ("3", dict(cast=None), "3"),
-        ("3", dict(cast=int), 3),
-        ("a", dict(cast=int), ValueError),
-        ("3", dict(default=None), "3"),
-        ("3", dict(default="5"), "3"),
-        (None, dict(default="5"), KeyError),
-        (None, dict(required=False, default=3), 3),
-        ("3", dict(required=False, default=3), "3"),
-        (None, dict(required=False, default=3, cast=int), 3),
-        ("3", dict(required=False, default=3, cast=int), 3),
-    ],
-)
-def test_key_getter(prop_val, args, expected_value_or_error):
-    class SampleConfig(Config):
-        prop = key(section_name="s", key_name="prop1", **args)
-
-    config = SampleConfig()
-    if prop_val is None:
-        source_dict = {}
-    else:
-        source_dict = {"s": {"PROP1": prop_val}}
-    config.add_source(DictConfigSource(source_dict))
-
-    if inspect.isclass(expected_value_or_error) and issubclass(expected_value_or_error, BaseException):
-        with pytest.raises(expected_value_or_error):
-            _ = config.prop
-    else:
-        v = config.prop
-        assert v == expected_value_or_error
-
-
-def test_get_key():
-    class SampleConfig(Config):
-        prop = key(section_name="s", key_name="prop1")
-
-    config = SampleConfig()
-    config.add_source(DictConfigSource({"s": {"PROP1": "propval"}}))
-    v = config.get_key("s", "prop1")
-    assert v == "propval"
-
-
-def test_caching():
-    class SampleConfig(Config):
-        prop1 = key(section_name="SampleConfig", key_name="PROP1")
-
-    mock_source: ConfigSource = MagicMock(spec=ConfigSource)
-    mock_source.get_config_value = MagicMock()
-    s = SampleConfig()
-    s.add_source(mock_source)
-
-    mock_source.get_config_value.assert_not_called()
-    a = s.prop1
-    mock_source.get_config_value.assert_called_once_with("SampleConfig", "PROP1")
-    b = s.prop1
-    mock_source.get_config_value.assert_called_once()
-    s.clear_cache()
-    c = s.prop1
-    assert 2 == mock_source.get_config_value.call_count
-
-
-def test_compose_configs():
-    config = ParentConfig()
-    config.add_source(
-        DictConfigSource(
-            {
-                "child": {"PROP1": "1"},
-                "parent": {"PROP1": "2"},
-            }
-        )
-    )
-
-    # Check that we are actually trying to read the grandchild which has a missing key
-    with pytest.raises(KeyError):
-        config.read()
-    config.add_source(DictConfigSource({"grandchild": {"PROP1": "3"}}))
-    config.read()
-    assert "2" == config.prop1
-    assert isinstance(config.child_config, ChildConfig)
-    assert "1" == config.child_config.prop1
-    assert isinstance(config.child_config.grandchild_config, GrandchildConfig)
-    assert "3" == config.child_config.grandchild_config.prop1
-
-
-def test_add_source():
-    c = Config()
-    with pytest.raises(TypeError):
-        bad_type: ConfigSource = 3
-        c.add_source(bad_type)
-
-    assert len(c.config_sources) == 0
-    new_source = DictConfigSource({})
-    c.add_source(new_source)
-    assert len(c.config_sources) == 1
-    assert c.config_sources[-1] is new_source
-
-
-def test_init_with_sources():
-    c = Config(sources=[DictConfigSource({}), DictConfigSource({})])
-    assert 2 == len(c.config_sources)
-
-
-def test_section_decorator():
-    @section("my_section")
-    class SampleConfig(Config):
-        prop1 = key(key_name="prop1")
-
-    c = SampleConfig()
-    c.add_source(DictConfigSource({"my_section": dict(PROP1="abc")}))
-    assert "abc" == c.prop1
-
-
-def test_key_name_inference():
-    class SampleConfig(Config):
-        prop1 = key(section_name="s")
-        prop2 = key(section_name="s")
-
-    c = SampleConfig()
-
-    c.add_source(
-        DictConfigSource(
-            {
-                "s": dict(
-                    PROP1="abc",
-                    PROP2="def",
-                )
-            }
-        )
-    )
-    assert "abc" == c.prop1
-    assert "def" == c.prop2
-
-
-def test_key_name_inference_multi_level():
-    class SampleConfigBase(Config):
-        prop1 = key(section_name="s")
-
-    class SampleConfig(SampleConfigBase):
-        prop2 = key(section_name="s")
-
-    c = SampleConfig()
-
-    c.add_source(
-        DictConfigSource(
-            {
-                "s": dict(
-                    PROP1="abc",
-                    PROP2="def",
-                )
-            }
-        )
-    )
-    assert "abc" == c.prop1
-    assert "def" == c.prop2
-
-
-def test_least_verbose_config():
-    @section("X")
-    class SampleConfig(Config):
-        prop1 = key()
-        prop2 = key(cast=int)
-
-    c = SampleConfig()
-    c.add_source(DictConfigSource({"X": dict(PROP1="abc", PROP2="44")}))
-
-    assert "abc" == c.prop1
-    assert 44 == c.prop2
-
-
-def test_section_decorator_precedence():
-    @section("decorator")
-    class SampleConfig(Config):
-        decorator_section = key(cast=str)
-        key_specific_section = key(section_name="key_specific", cast=str)
-
-    c = SampleConfig(
-        sources=[
-            DictConfigSource({"decorator": dict(decorator_section="a"), "key_specific": dict(key_specific_section="b")})
-        ]
-    )
-    c.read()
-
-
-def test_no_section_provided():
-    class SampleConfig(Config):
-        k = key(cast=str)
-
-    c = SampleConfig()
-    with pytest.raises(ValueError):
-        c.read()
-
-
-def test_multiple_group_keys_with_section_decorators():
-    @section("a")
-    class Child1(Config):
-        k1 = key(cast=str)
-
-    @section("b")
-    class Child2(Config):
-        k2 = key(cast=str)
-
-    class ParentConfig(Config):
-        c1 = group_key(Child1)
-        c2 = group_key(Child2)
-
-    c1 = Child1()
-    c2 = Child2()
-
-    assert c1._section_name == "a"
-    assert c2._section_name == "b"
-
-    p = ParentConfig()
-    p.add_source(DictConfigSource({"a": {"k1": "v1"}, "b": {"k2": "v2"}}))
-    assert p.c1._section_name == "a"
-    assert p.c2._section_name == "b"
-
-    assert "v1" == p.c1.k1
-    assert "v2" == p.c2.k2
-
-
-def test_cast_with_default():
-    @section("s")
-    class SampleConfig(Config):
-        nullable_key = key(cast=str, required=False, default=None)
-        bool_key = key(cast=bool, required=False, default=False)
-
-    s = SampleConfig()
-    s.add_source(DictConfigSource({}))
-    assert s.nullable_key is None
-    assert s.bool_key is False
-
-
-def test_provider_property_read():
-    provider = ConfigProvider()
-    config = ParentConfig(provider=provider)
-    p = config.provider
-    # Check same object is returned
-    assert p is provider
-
-
-def test_provider_property_is_readonly():
-    config = ParentConfig()
-    with pytest.raises(Exception):
-        config.provider = ConfigProvider()
-
-
-def test_construct_config_without_provider():
-    sources = [DictConfigSource({})]
-    config = ParentConfig(sources=sources)
-    assert isinstance(config.provider, ConfigProvider)
-    assert config.provider.config_sources == sources
-
-
-def test_construct_config_bad_provider_type():
-    with pytest.raises(TypeError):
-        config = ParentConfig(provider=3)
-
-
-def test_construct_config_with_provider():
-    sources = [DictConfigSource({})]
-    provider = ConfigProvider(sources)
-    config = ParentConfig(sources=sources, provider=provider)
-    assert config.provider is provider
-    assert config.config_sources == sources
-
-
-def test_replace_source():
-    sources = [DictConfigSource({}), DictConfigSource({})]
-    config = Config(sources=sources)
-
-    assert config.config_sources == sources
-    assert config.config_sources[0] is sources[0]
-    assert config.config_sources[1] is sources[1]
-
-    replacement_source = DictConfigSource({})
-    config.replace_source(sources[0], replacement_source)
-
-    assert config.config_sources == [replacement_source, sources[1]]
-    assert config.config_sources[0] is replacement_source
-    assert config.config_sources[1] is sources[1]
-
-
-def test_replace_source_not_found():
-    source_a = DictConfigSource({})
-    source_b = DictConfigSource({})
-    config = Config()
-    config.add_source(source_a)
-    with pytest.raises(ValueError):
-        config.replace_source(source_b, source_a)
-
-
-def test_replace_source_bad_type():
-    source = DictConfigSource({})
-    config = Config(sources=[source])
-    with pytest.raises(TypeError):
-        bad_type: ConfigSource = 3
-        config.replace_source(source, bad_type)
-
-
-def test_set_sources():
-    old_sources = [DictConfigSource({})]
-    new_sources = [DictConfigSource({}), DictConfigSource({})]
-    config = Config(sources=old_sources)
-    config.set_sources(new_sources)
-    assert len(config.config_sources) == 2
-    assert config.config_sources[0] is new_sources[0]
-    assert config.config_sources[1] is new_sources[1]
-
-
-def test_property_is_read_only():
-    config = GrandchildConfig()
-    with pytest.raises(AttributeError):
-        config.prop1 = "a"
-
-
-def test_post_read_hook():
-    @section("s")
-    class SampleConfig(Config):
-        prop1 = key(cast=str)
-        prop2 = key(cast=str, required=False)
-
-        def post_read_hook(self) -> dict:
-            return dict(prop2="x" + self.prop1)
-
-    config_source = DictConfigSource(
-        {
-            "s": {
-                "prop1": "a",
-            }
-        }
-    )
-    config = SampleConfig(sources=[config_source])
-    config.read()
-
-    assert config.prop1 == "a"
-    assert config.prop2 == "xa"
-
-
-def test_post_read_hook_different_key_name():
-    @section("s")
-    class SampleConfig(Config):
-        prop1 = key(section_name="s", key_name="key1", cast=str)
-        prop2 = key(section_name="s", key_name="key2", cast=str, required=False)
-
-        def post_read_hook(self) -> dict:
-            return dict(prop2="x" + self.prop1)
-
-    config_source = DictConfigSource(
-        {
-            "s": {
-                "key1": "a",
-            }
-        }
-    )
-    config = SampleConfig(sources=[config_source])
-    config.read()
-
-    assert config.prop1 == "a"
-    assert config.prop2 == "xa"
-
-
-def test_post_read_hook_modify_child():
-    class SampleChildConfig(Config):
-        prop3 = key(section_name="s", key_name="key3", cast=str)
-
-    class SampleConfig(Config):
-        prop3 = group_key(SampleChildConfig)
-
-        def post_read_hook(self) -> dict:
-            return dict(prop3=dict(prop3="new_value"))
-
-    config_source = DictConfigSource(
-        {
-            "s": {
-                "key3": "b",
-            }
-        }
-    )
-    config = SampleConfig(sources=[config_source])
-    config.read()
-
-    assert config.prop3.prop3 == "new_value"
-
-
-def test_post_read_hook_child_takes_priority():
-    class SampleChildConfig(Config):
-        prop3 = key(section_name="s", key_name="key3", cast=str)
-
-        def post_read_hook(self) -> dict:
-            return dict(prop3="child_new_value")
-
-    class SampleConfig(Config):
-        prop3 = group_key(SampleChildConfig)
-
-        def post_read_hook(self) -> dict:
-            return dict(prop3=dict(prop3="new_value"))
-
-    config_source = DictConfigSource(
-        {
-            "s": {
-                "key3": "b",
-            }
-        }
-    )
-    config = SampleConfig(sources=[config_source])
-    config.read()
-
-    assert config.prop3.prop3 == "child_new_value"
-
-
-@pytest.mark.parametrize(
-    "post_read_hook_return_value",
-    [
-        dict(wrong_prop="c"),
-        dict(prop1=dict(a=4)),
-        dict(prop2="d"),
-    ],
-    ids=["KeyNotExist", "DictNotValue", "ValueNotDict"],
-)
-def test_post_read_hook_invalid_attributes(post_read_hook_return_value: dict):
-    class SampleChildConfig(Config):
-        pass
-
-    @section("s")
-    class SampleConfig(Config):
-        prop1 = key(cast=str)
-        prop2 = group_key(SampleChildConfig)
-
-        def post_read_hook(self) -> dict:
-            return post_read_hook_return_value
-
-    config_source = DictConfigSource({"s": {"prop1": "a"}})
-    config = SampleConfig(sources=[config_source])
-    with pytest.raises(KeyError):
-        config.read()
-
-
-def test_config_repr():
-    class SampleChildConfig(Config):
-        a = key(section_name="test", cast=str, required=False, default="A")
-
-    @section("test")
-    class SampleConfig(Config):
-        b = key(cast=str, required=False, default="B")
-        child = group_key(SampleChildConfig)
-
-    config = SampleConfig()
-    assert repr(config) == "SampleConfig(b='B', child=SampleChildConfig(a='A'))"
+import inspect
+import pytest
+from unittest.mock import MagicMock
+from typedconfig.config import Config, key, section, group_key, ConfigProvider
+from typedconfig.source import DictConfigSource, ConfigSource
+
+
+class GrandchildConfig(Config):
+    prop1 = key(section_name="grandchild", key_name="PROP1")
+
+
+class ChildConfig(Config):
+    prop1 = key(section_name="child", key_name="PROP1")
+    grandchild_config = group_key(GrandchildConfig)
+
+
+class ParentConfig(Config):
+    prop1 = key(section_name="parent", key_name="PROP1")
+    child_config = group_key(ChildConfig)
+
+
+def test_subclass_config():
+    class SampleConfig(Config):
+        prop1 = key(section_name="s", key_name="prop1", cast=float)
+        prop2 = key(section_name="s", key_name="prop2", cast=int)
+        prop3 = key(section_name="s", key_name="prop3", cast=str)
+        prop4 = key(section_name="s", key_name="prop4")
+
+    config_source = DictConfigSource({"s": {"PROP1": "3.5", "PROP2": "2", "PROP3": "hello", "PROP4": "abc"}})
+    config = SampleConfig()
+    config.add_source(config_source)
+
+    assert 3.5 == config.prop1
+    assert 2 == config.prop2
+    assert "hello" == config.prop3
+    assert "abc" == config.prop4
+
+
+def test_register_properties():
+    class SampleConfig(Config):
+        registerd_key1 = key(section_name="s", key_name="key1")
+        registerd_key2 = key(section_name="s", key_name="key2")
+
+        not_registered_key = 3
+
+        def not_registered_method(self):
+            pass
+
+    config = SampleConfig()
+    props = config.get_registered_properties()
+    assert sorted(["registerd_key1", "registerd_key2"]) == sorted(props)
+
+
+def test_register_composed_config():
+    class ChildConfig1(Config):
+        pass
+
+    class ChildConfig2(Config):
+        pass
+
+    class SampleConfig(Config):
+        composed_config1 = group_key(ChildConfig1)
+        composed_config2 = group_key(ChildConfig2)
+
+    config = SampleConfig()
+    sub_configs = config.get_registered_composed_config()
+    assert len(sub_configs) == 2
+    assert isinstance(sub_configs[0], ChildConfig1)
+    assert isinstance(sub_configs[1], ChildConfig2)
+
+    # Check we're not creating a new instance of the sub configs each time we call
+    sub_configs_2 = config.get_registered_composed_config()
+    assert sub_configs[0] is sub_configs_2[0]
+    assert sub_configs[1] is sub_configs_2[1]
+
+
+def test_reuse_child_config():
+    class SampleChildConfig(Config):
+        pass
+
+    class SampleConfig(Config):
+        composed_1 = group_key(SampleChildConfig)
+        composed_2 = group_key(SampleChildConfig)
+
+    config = SampleConfig()
+    config.read()
+
+    sub_configs = config.get_registered_composed_config()
+    assert len(sub_configs) == 2
+    assert isinstance(sub_configs[0], SampleChildConfig)
+    assert isinstance(sub_configs[1], SampleChildConfig)
+    assert sub_configs[0] is not sub_configs[1]
+
+
+@pytest.mark.parametrize(
+    "config_dict, expect_error",
+    [({}, True), ({"PROP1": "x"}, False), ({"PROP1": "x", "PROP2": "y"}, False)],
+    ids=["ConfigMissing", "PropertiesMatch", "ExtraConfig"],
+)
+def test_read(config_dict, expect_error):
+    class SampleConfig(Config):
+        prop1 = key(section_name="s", key_name="prop1")
+
+    config = SampleConfig()
+    config.add_source(DictConfigSource({"s": config_dict}))
+
+    if expect_error:
+        with pytest.raises(KeyError):
+            config.read()
+    else:
+        config.read()
+
+    if "PROP1" in config_dict:
+        assert config_dict["PROP1"] == config.prop1
+
+
+@pytest.mark.parametrize(
+    "prop_val, args, expected_value_or_error",
+    [
+        ("3", dict(), "3"),
+        (None, dict(), KeyError),
+        ("3", dict(required=True), "3"),
+        (None, dict(required=True), KeyError),
+        ("3", dict(required=False), "3"),
+        (None, dict(required=False), None),
+        ("3", dict(cast=None), "3"),
+        ("3", dict(cast=int), 3),
+        ("a", dict(cast=int), ValueError),
+        ("3", dict(default=None), "3"),
+        ("3", dict(default="5"), "3"),
+        (None, dict(default="5"), KeyError),
+        (None, dict(required=False, default=3), 3),
+        ("3", dict(required=False, default=3), "3"),
+        (None, dict(required=False, default=3, cast=int), 3),
+        ("3", dict(required=False, default=3, cast=int), 3),
+    ],
+)
+def test_key_getter(prop_val, args, expected_value_or_error):
+    class SampleConfig(Config):
+        prop = key(section_name="s", key_name="prop1", **args)
+
+    config = SampleConfig()
+    if prop_val is None:
+        source_dict = {}
+    else:
+        source_dict = {"s": {"PROP1": prop_val}}
+    config.add_source(DictConfigSource(source_dict))
+
+    if inspect.isclass(expected_value_or_error) and issubclass(expected_value_or_error, BaseException):
+        with pytest.raises(expected_value_or_error):
+            _ = config.prop
+    else:
+        v = config.prop
+        assert v == expected_value_or_error
+
+
+def test_get_key():
+    class SampleConfig(Config):
+        prop = key(section_name="s", key_name="prop1")
+
+    config = SampleConfig()
+    config.add_source(DictConfigSource({"s": {"PROP1": "propval"}}))
+    v = config.get_key("s", "prop1")
+    assert v == "propval"
+
+
+def test_caching():
+    class SampleConfig(Config):
+        prop1 = key(section_name="SampleConfig", key_name="PROP1")
+
+    mock_source: ConfigSource = MagicMock(spec=ConfigSource)
+    mock_source.get_config_value = MagicMock()
+    s = SampleConfig()
+    s.add_source(mock_source)
+
+    mock_source.get_config_value.assert_not_called()
+    a = s.prop1
+    mock_source.get_config_value.assert_called_once_with("SampleConfig", "PROP1")
+    b = s.prop1
+    mock_source.get_config_value.assert_called_once()
+    s.clear_cache()
+    c = s.prop1
+    assert 2 == mock_source.get_config_value.call_count
+
+
+def test_compose_configs():
+    config = ParentConfig()
+    config.add_source(
+        DictConfigSource(
+            {
+                "child": {"PROP1": "1"},
+                "parent": {"PROP1": "2"},
+            }
+        )
+    )
+
+    # Check that we are actually trying to read the grandchild which has a missing key
+    with pytest.raises(KeyError):
+        config.read()
+    config.add_source(DictConfigSource({"grandchild": {"PROP1": "3"}}))
+    config.read()
+    assert "2" == config.prop1
+    assert isinstance(config.child_config, ChildConfig)
+    assert "1" == config.child_config.prop1
+    assert isinstance(config.child_config.grandchild_config, GrandchildConfig)
+    assert "3" == config.child_config.grandchild_config.prop1
+
+
+def test_add_source():
+    c = Config()
+    with pytest.raises(TypeError):
+        bad_type: ConfigSource = 3
+        c.add_source(bad_type)
+
+    assert len(c.config_sources) == 0
+    new_source = DictConfigSource({})
+    c.add_source(new_source)
+    assert len(c.config_sources) == 1
+    assert c.config_sources[-1] is new_source
+
+
+def test_init_with_sources():
+    c = Config(sources=[DictConfigSource({}), DictConfigSource({})])
+    assert 2 == len(c.config_sources)
+
+
+def test_section_decorator():
+    @section("my_section")
+    class SampleConfig(Config):
+        prop1 = key(key_name="prop1")
+
+    c = SampleConfig()
+    c.add_source(DictConfigSource({"my_section": dict(PROP1="abc")}))
+    assert "abc" == c.prop1
+
+
+def test_key_name_inference():
+    class SampleConfig(Config):
+        prop1 = key(section_name="s")
+        prop2 = key(section_name="s")
+
+    c = SampleConfig()
+
+    c.add_source(
+        DictConfigSource(
+            {
+                "s": dict(
+                    PROP1="abc",
+                    PROP2="def",
+                )
+            }
+        )
+    )
+    assert "abc" == c.prop1
+    assert "def" == c.prop2
+
+
+def test_key_name_inference_multi_level():
+    class SampleConfigBase(Config):
+        prop1 = key(section_name="s")
+
+    class SampleConfig(SampleConfigBase):
+        prop2 = key(section_name="s")
+
+    c = SampleConfig()
+
+    c.add_source(
+        DictConfigSource(
+            {
+                "s": dict(
+                    PROP1="abc",
+                    PROP2="def",
+                )
+            }
+        )
+    )
+    assert "abc" == c.prop1
+    assert "def" == c.prop2
+
+
+def test_least_verbose_config():
+    @section("X")
+    class SampleConfig(Config):
+        prop1 = key()
+        prop2 = key(cast=int)
+
+    c = SampleConfig()
+    c.add_source(DictConfigSource({"X": dict(PROP1="abc", PROP2="44")}))
+
+    assert "abc" == c.prop1
+    assert 44 == c.prop2
+
+
+def test_section_decorator_precedence():
+    @section("decorator")
+    class SampleConfig(Config):
+        decorator_section = key(cast=str)
+        key_specific_section = key(section_name="key_specific", cast=str)
+
+    c = SampleConfig(
+        sources=[
+            DictConfigSource({"decorator": dict(decorator_section="a"), "key_specific": dict(key_specific_section="b")})
+        ]
+    )
+    c.read()
+
+
+def test_no_section_provided():
+    class SampleConfig(Config):
+        k = key(cast=str)
+
+    c = SampleConfig()
+    with pytest.raises(ValueError):
+        c.read()
+
+
+def test_multiple_group_keys_with_section_decorators():
+    @section("a")
+    class Child1(Config):
+        k1 = key(cast=str)
+
+    @section("b")
+    class Child2(Config):
+        k2 = key(cast=str)
+
+    class ParentConfig(Config):
+        c1 = group_key(Child1)
+        c2 = group_key(Child2)
+
+    c1 = Child1()
+    c2 = Child2()
+
+    assert c1._section_name == "a"
+    assert c2._section_name == "b"
+
+    p = ParentConfig()
+    p.add_source(DictConfigSource({"a": {"k1": "v1"}, "b": {"k2": "v2"}}))
+    assert p.c1._section_name == "a"
+    assert p.c2._section_name == "b"
+
+    assert "v1" == p.c1.k1
+    assert "v2" == p.c2.k2
+
+
+def test_cast_with_default():
+    @section("s")
+    class SampleConfig(Config):
+        nullable_key = key(cast=str, required=False, default=None)
+        bool_key = key(cast=bool, required=False, default=False)
+
+    s = SampleConfig()
+    s.add_source(DictConfigSource({}))
+    assert s.nullable_key is None
+    assert s.bool_key is False
+
+
+def test_provider_property_read():
+    provider = ConfigProvider()
+    config = ParentConfig(provider=provider)
+    p = config.provider
+    # Check same object is returned
+    assert p is provider
+
+
+def test_provider_property_is_readonly():
+    config = ParentConfig()
+    with pytest.raises(Exception):
+        config.provider = ConfigProvider()
+
+
+def test_construct_config_without_provider():
+    sources = [DictConfigSource({})]
+    config = ParentConfig(sources=sources)
+    assert isinstance(config.provider, ConfigProvider)
+    assert config.provider.config_sources == sources
+
+
+def test_construct_config_bad_provider_type():
+    with pytest.raises(TypeError):
+        config = ParentConfig(provider=3)
+
+
+def test_construct_config_with_provider():
+    sources = [DictConfigSource({})]
+    provider = ConfigProvider(sources)
+    config = ParentConfig(sources=sources, provider=provider)
+    assert config.provider is provider
+    assert config.config_sources == sources
+
+
+def test_replace_source():
+    sources = [DictConfigSource({}), DictConfigSource({})]
+    config = Config(sources=sources)
+
+    assert config.config_sources == sources
+    assert config.config_sources[0] is sources[0]
+    assert config.config_sources[1] is sources[1]
+
+    replacement_source = DictConfigSource({})
+    config.replace_source(sources[0], replacement_source)
+
+    assert config.config_sources == [replacement_source, sources[1]]
+    assert config.config_sources[0] is replacement_source
+    assert config.config_sources[1] is sources[1]
+
+
+def test_replace_source_not_found():
+    source_a = DictConfigSource({})
+    source_b = DictConfigSource({})
+    config = Config()
+    config.add_source(source_a)
+    with pytest.raises(ValueError):
+        config.replace_source(source_b, source_a)
+
+
+def test_replace_source_bad_type():
+    source = DictConfigSource({})
+    config = Config(sources=[source])
+    with pytest.raises(TypeError):
+        bad_type: ConfigSource = 3
+        config.replace_source(source, bad_type)
+
+
+def test_set_sources():
+    old_sources = [DictConfigSource({})]
+    new_sources = [DictConfigSource({}), DictConfigSource({})]
+    config = Config(sources=old_sources)
+    config.set_sources(new_sources)
+    assert len(config.config_sources) == 2
+    assert config.config_sources[0] is new_sources[0]
+    assert config.config_sources[1] is new_sources[1]
+
+
+def test_property_is_read_only():
+    config = GrandchildConfig()
+    with pytest.raises(AttributeError):
+        config.prop1 = "a"
+
+
+def test_post_read_hook():
+    @section("s")
+    class SampleConfig(Config):
+        prop1 = key(cast=str)
+        prop2 = key(cast=str, required=False)
+
+        def post_read_hook(self) -> dict:
+            return dict(prop2="x" + self.prop1)
+
+    config_source = DictConfigSource(
+        {
+            "s": {
+                "prop1": "a",
+            }
+        }
+    )
+    config = SampleConfig(sources=[config_source])
+    config.read()
+
+    assert config.prop1 == "a"
+    assert config.prop2 == "xa"
+
+
+def test_post_read_hook_different_key_name():
+    @section("s")
+    class SampleConfig(Config):
+        prop1 = key(section_name="s", key_name="key1", cast=str)
+        prop2 = key(section_name="s", key_name="key2", cast=str, required=False)
+
+        def post_read_hook(self) -> dict:
+            return dict(prop2="x" + self.prop1)
+
+    config_source = DictConfigSource(
+        {
+            "s": {
+                "key1": "a",
+            }
+        }
+    )
+    config = SampleConfig(sources=[config_source])
+    config.read()
+
+    assert config.prop1 == "a"
+    assert config.prop2 == "xa"
+
+
+def test_post_read_hook_modify_child():
+    class SampleChildConfig(Config):
+        prop3 = key(section_name="s", key_name="key3", cast=str)
+
+    class SampleConfig(Config):
+        prop3 = group_key(SampleChildConfig)
+
+        def post_read_hook(self) -> dict:
+            return dict(prop3=dict(prop3="new_value"))
+
+    config_source = DictConfigSource(
+        {
+            "s": {
+                "key3": "b",
+            }
+        }
+    )
+    config = SampleConfig(sources=[config_source])
+    config.read()
+
+    assert config.prop3.prop3 == "new_value"
+
+
+def test_post_read_hook_child_takes_priority():
+    class SampleChildConfig(Config):
+        prop3 = key(section_name="s", key_name="key3", cast=str)
+
+        def post_read_hook(self) -> dict:
+            return dict(prop3="child_new_value")
+
+    class SampleConfig(Config):
+        prop3 = group_key(SampleChildConfig)
+
+        def post_read_hook(self) -> dict:
+            return dict(prop3=dict(prop3="new_value"))
+
+    config_source = DictConfigSource(
+        {
+            "s": {
+                "key3": "b",
+            }
+        }
+    )
+    config = SampleConfig(sources=[config_source])
+    config.read()
+
+    assert config.prop3.prop3 == "child_new_value"
+
+
+@pytest.mark.parametrize(
+    "post_read_hook_return_value",
+    [
+        dict(wrong_prop="c"),
+        dict(prop1=dict(a=4)),
+        dict(prop2="d"),
+    ],
+    ids=["KeyNotExist", "DictNotValue", "ValueNotDict"],
+)
+def test_post_read_hook_invalid_attributes(post_read_hook_return_value: dict):
+    class SampleChildConfig(Config):
+        pass
+
+    @section("s")
+    class SampleConfig(Config):
+        prop1 = key(cast=str)
+        prop2 = group_key(SampleChildConfig)
+
+        def post_read_hook(self) -> dict:
+            return post_read_hook_return_value
+
+    config_source = DictConfigSource({"s": {"prop1": "a"}})
+    config = SampleConfig(sources=[config_source])
+    with pytest.raises(KeyError):
+        config.read()
+
+
+def test_config_repr():
+    class SampleChildConfig(Config):
+        a = key(section_name="test", cast=str, required=False, default="A")
+
+    @section("test")
+    class SampleConfig(Config):
+        b = key(cast=str, required=False, default="B")
+        child = group_key(SampleChildConfig)
+
+    config = SampleConfig()
+    assert repr(config) == "SampleConfig(b='B', child=SampleChildConfig(a='A'))"
```

### Comparing `typed-config-1.5.0/typed_config.egg-info/PKG-INFO` & `typed-config-2.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,646 +1,628 @@
-Metadata-Version: 2.1
-Name: typed-config
-Version: 1.5.0
-Summary: Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
-Home-page: https://github.com/bwindsor/typed-config
-Author: Ben Windsor
-Author-email: 
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.org/bwindsor/typed-config.svg?branch=master)](https://travis-ci.org/bwindsor/typed-config)
-[![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
-
-# typed-config
-Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
-
-`pip install typed-config`
-
-Requires python 3.6 or above. (Also, needs `typing_extensions` for Python <= 3.7, so not completely dependency free if using old Python).
-
-## Basic usage
-```python
-# my_app/config.py
-from typedconfig import Config, key, section
-from typedconfig.source import EnvironmentConfigSource
-
-@section('database')
-class AppConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-    timeout = key(cast=float)
-
-config = AppConfig()
-config.add_source(EnvironmentConfigSource())
-config.read()
-```
-
-```python
-# my_app/main.py
-from my_app.config import config
-print(config.host)
-```
-In PyCharm, and hopefully other IDEs, it will recognise the datatypes of your configuration and allow you to autocomplete. No more remembering strings to get the right thing out!
-
-## Upgrading from 0.x.x
-There is one breaking change when moving from `0.x.x` to `1.x.x`. The `key` function now expects all arguments to be keyword arguments. So simply replace any calls like so:
-```python
-key('section', 'key', True, str, 'default')  # 0.x.x
-key(section_name='section', key_name='key', required=True, cast=str, default='default')  # 1.x.x
-```
-The reason for this change is to tie down the return type of `key` properly. Previously, when `required=False` or when `cast=None` the return type would not include the possibility of `None` or `string`. The type checker should now be able to infer the return type based on the values of `required`, `cast` and `default`.
-
-## How it works
-Configuration is always supplied in a two level structure, so your source configuration can have multiple sections, and each section contains multiple key/value configuration pairs. For example:
-```ini
-[database]
-host = 127.0.0.1
-port = 2000
-
-[algorithm]
-max_value = 10
-min_value = 20
-```
-
-You then create your configuration hierarchy in code (this can be flat or many levels deep) and supply the matching between strings in your config sources and properties of your configuration classes.
-
-You provide one or more `ConfigSource`s, from which the config for your application can be read. For example, you might supply an `EnvironmentConfigSource`,  and two `IniFileConfigSource`s. This would make your application first look for a configuration value in environment variables, if not found there it would then look at the first INI file (perhaps a user-specific file), before falling back to the second INI file (perhaps a default configuration shared between all users). If a parameter is still not found and is a required parameter, an error would be thrown.
-
-There is emphasis on type information being available for everything so that an IDE will autocomplete when trying to use your config across your application.
-
-### Multiple data sources
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-    username = key(cast=str)
-    password = key(cast=str)
-
-config = DatabaseConfig()
-config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-config.add_source(IniFileConfigSource("config.cfg"))
-
-# OR provide sources directly to the constructor
-config = DatabaseConfig(sources=[
-    EnvironmentConfigSource(prefix="EXAMPLE"),
-    IniFileConfigSource("config.cfg")
-])
-```
-
-Since you don't want to hard code your secret credentials, you might supply them through the environment.
-So for the above configuration, the environment might look like this:
-```bash
-export EXAMPLE_DATABASE_USERNAME=my_username
-export EXAMPLE_DATABASE_PASSWORD=my_very_secret_password
-export EXAMPLE_DATABASE_PORT=2001
-```
-
-Those values which couldn't be found in the environment would then be read from the INI file, which might look like this:
-```ini
-[database]
-HOST = db1.mydomain.com
-PORT = 2000
-```
-
-Note after this, `config.port` will be equal to `2001` as the value in the environment took priority over the value in the INI file.
-
-### Caching
-When config values are first used, they are read. This is lazy evaluation by default so that not everything is read if not necessary.
-
-After first use, they are cached in memory so that there should be no further I/O if the config value is used again.
-
-For fail fast behaviour, and also to stop unexpected latency when a config value is read partway through your application (e.g. your config could be coming across a network), the option is available to read all config values at the start. Just call
-
-`config.read()`
-
-This will throw an exception if any required config value cannot be found, and will also keep all read config values in memory for next time they are used. If you do not use `read` you will only get the exception when you first try to use the offending config key.
-
-### Hierarchical configuration
-Use `group_key` to represent a "sub-config" of a configuration. Set up "sub-configs" exactly as demonstrated above, and then create a parent config to compose them in one place.
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-
-@section('algorithm')
-class AlgorithmConfig(Config):
-    max_value = key(cast=float)
-    min_value = key(cast=float)
-
-class ParentConfig(Config):
-    database = group_key(DatabaseConfig)
-    algorithm = group_key(AlgorithmConfig)
-    description = key(cast=str, section_name="general")
-
-config = ParentConfig()
-config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-config.add_source(IniFileConfigSource("config.cfg"))
-config.read()
-```
-
-The first time the `config.database` or `config.algorithm` is accessed (which in the case above is when `read()` is called), then an instance will be instantiated. Notice that it is the class definition, not an instance of the class, which is passed to the `group_key` function.
-
-### Custom section/key names, optional parameters, default values
-Let's take a look at this:
-```python
-from typedconfig import Config, key, section
-
-@section('database')
-class AppConfig(Config):
-    host1 = key()
-    host2 = key(section_name='database', key_name='HOST2',
-                required=True, cast=str, default=None)
-```
-Both `host1` and `host2` are legitimate configuration key definitions.
-
-* `section_name` - this name of the section in the configuration source from which this parameter should be read. This can be provided on a key-by-key basis, but if it is left out then the section name supplied by the `@section` decorator is used. If all keys supply a `section_name`, the class decorator is not needed. If both `section_name` and a decorator are provided, the `section_name` argument takes priority.
-* `key_name` - the name of this key in the configuration source from which this parameter is read. If not supplied, some magic uses the object property name as the key name.
-* `required` - default True. If False, and the configuration value can't be found, no error will be thrown and the default value will be used, if provided. If a default not provided, `None` will be used.
-* `cast` - probably the most important option for typing. **If you want autocomplete typing support you must specify this**. It's just a function which takes a string as an input and returns a parsed value. See the casting section for more. If not supplied, the value remains as a string.
-* `default` - only applicable if `required` is false. When `required` is false this value is used if a value cannot be found.
-
-### Types
-```python
-from typedconfig import Config, key, section
-from typing import List
-
-def split_str(s: str) -> List[str]:
-    return [x.strip() for x in s.split(",")]
-
-@section('database')
-class AppConfig(Config):
-    host = key()
-    port = key(cast=int)
-    users = key(cast=split_str)
-    zero_based_index = key(cast=lambda x: int(x)-1)
-config = AppConfig(sources=[...])
-```
-In this example we have three ways of casting:
-1. Not casting at all. This defaults to returning a `str`, but your IDE won't know that so if you want type hints use `cast=str`
-2. Casting to an built in type which can take a string input and parse it, for example `int`
-3. Defining a custom function. Your function should take one string input and return one output of any type. To get type hint, just make sure your function has type annotations.
-4. Using a lambda expression. The type inference may or may not work depending on your expression, so if it doesn't just write it as a function with type annotations.
-
-### Validation
-You can validate what has been supplied by providing a custom `cast` function to a `key`, which validates the configuration value in addition to parsing it.
-
-### Extending configuration using shared ConfigProvider
-
-Multiple application modules may use different configuration schemes while sharing the same configuration source. Analogously, various `Config` classes may provide different view of the same configuration data, sharing the same `ConfigProvider`.
-
-```python
-# app/config.py
-from typedconfig.provider import ConfigProvider
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-provider = ConfigProvider()
-provider.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
-provider.add_source(IniFileConfigSource("config.cfg"))
-
-__all__ = ["provider"]
-```
-```python
-# app/database/config.py
-from typedconfig import Config, key, section
-from app.config import provider
-
-@section('database')
-class DatabaseConfig(Config):
-    host = key(cast=str)
-    port = key(cast=int)
-
-database_config = DatabaseConfig(provider=provider)
-```
-```python
-# app/algorithm/config.py
-from typedconfig import Config, key, section
-from app.config import provider
-
-@section('algorithm')
-class AlgorithmConfig(Config):
-    max_value = key(cast=float)
-    min_value = key(cast=float)
-
-algorithm_config = AlgorithmConfig(provider=provider)
-```
-
-Shared configuration provider can be used by plugins, which may need to declare additional configuration sections within the same configuration files as the main application.  Let's assume we have `[database]` section used by main application and `[app_extension]` that provides 3rd party plugin configuration:
-
-```ini
-[database]
-host = 127.0.0.1
-port = 2000
-
-[app_extension]
-api_key = secret
-```
-
-e.g. `app/config.py` may look like that:
-
-```python
-from typedconfig import Config, key, section, group_key
-from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
-
-@section('database')
-class DatabaseConfig(Config):
-    """Database configuration"""
-    host = key(cast=str)
-    port = key(cast=int)
-
-class ApplicationConfig(Config):
-    """Main configuration object"""
-    database = group_key(DatabaseConfig)
-
-app_config = ApplicationConfig(sources=[
-    EnvironmentConfigSource(),
-    IniFileConfigSource("config.cfg")
-])
-```
-
-and plugin can read additional sections by using the same configuration provider as main application config.
-
-e.g. `plugin/config.py`:
-```python
-from typedconfig import Config, key, section, group_key
-
-from app.config import ApplicationConfig, app_config
-
-@section('app_extension')
-class ExtensionConfig(Config):
-    """Extension configuration"""
-    api_key = key(cast=str)
-
-# ExtendedAppConfig extends ApplicationConfig 
-# so original sections are also included
-class ExtendedAppConfig(ApplicationConfig):
-    """Extended main configuration object"""
-    app_extension = group_key(ExtensionConfig)
-    
-# ExtendedAppConfig uses the same provider as the main app_config
-extended_config = ExtendedAppConfig(provider=app_config.provider)
-```
-```python
-from plugin.config import extended_config
-
-# Plugin can access both main and extra sections
-print(extended_config.app_extension.api_key)
-print(extended_config.database.host)
-```
-
-### Configuration variables which depend on other configuration variables
-Sometimes you may wish to set the value of some configuration variables based on others. You may also wish to validate some variables, for example allowed values may be different depending on the value of another config variable. For this you can add a `post_read_hook`.
-
-The default implementation of `post_read_hook` returns an empty `dict`. You can override this by implementing your own `post_read_hook` method. It should receive only `self` as an input, and return a `dict`. This `dict` should be a simple mapping from config keys to values. For hierarchical configurations, you can nest the dictionaries. If you provide a `post_read_hook` in both a parent and a child class which both make changes to the same keys (don't do this) then the values returned by the child method will overwrite those by the parent.
-
-This hook is called whenever you call the `read` method. If you use lazy loading and skip calling the `read` method, you cannot use this hook.
-```python
-# my_app/config.py
-from typedconfig import Config, key, group_key, section
-from typedconfig.source import EnvironmentConfigSource
-
-@section('child')
-class ChildConfig(Config):
-    http_port_plus_one = key(cast=int, required=False)
-
-@section('app')
-class AppConfig(Config):
-    use_https = key(cast=bool)
-    http_port = key(key_name='port', cast=int, required=False)
-    child = group_key(ChildConfig)
-    
-    def post_read_hook(self) -> dict:
-        config_updates = dict()
-        # If the port has not been provided, set it based on the value of use_https
-        if self.http_port is None:
-            config_updates.update(http_port=443 if self.use_https else 80)
-        else:
-            # Modify child config
-            config_updates.update(child=dict(http_port_plus_one=self.http_port + 1))
-            
-        # Validate that the port number has a sensible value
-        # It is recommended to do validation inside the cast method for individual keys, however for dependent keys it can be useful here
-        if self.http_port is not None:
-            if self.use_https:
-                assert self.http_port in [443, 444, 445]
-            else:
-                assert self.http_port in [80, 81, 82]
-
-        return config_updates
-            
-config = AppConfig()
-config.add_source(EnvironmentConfigSource())
-config.read()
-```
-
-## Configuration Sources
-Configuration sources are how your main `Config` class knows where to get its data from. These are totally extensible so that you can read in your configuration from wherever you like - from a database, from S3, anywhere that you can write code for.
-
-You supply your configuration source to your config after you've instantiated it, but **before** you try to read any data from it:
-```python
-config = AppConfig()
-config.add_source(my_first_source)
-config.add_source(my_second_source)
-config.read()
-```
-Or you can supply the sources directly in the constructor like this:
-```python
-config = AppConfig(sources=[my_first_source, my_second_source])
-config.read()
-```
-
-
-### Modifying or refreshing configuration after it has been loaded
-In general it is bad practice to modify configuration at runtime because the configuration for your program should be fixed for the duration of it.  However, there are cases where it may be necessary.
-
-To completely replace the set of config sources, you can use
-```python
-config = AppConfig(sources=[my_first_source, my_second_source])
-config.set_sources([my_first_new_source, my_second_new_source])
-```
-
-To replace a specific config source, for example because a config file has changed and you need to re-read it from disk, you can use `replace_source`:
-```python
-from typedconfig.source import IniFileConfigSource
-original_source = IniFileConfigSource("config.cfg")
-config = AppConfig(sources=[source])
-# Now say you change the contents to config.cfg and need to read it again
-new_source = IniFileConfigSource("config.cfg")  # re-reads file during construction
-config.replace_source(original_source, new_source)
-```
-
-**Important**: if you add or modify the config sources the config has been read, or need to refresh the config for some reason, you'll need to clear any cached values in order to force the config to be fetched from the `ConfigSource`s again. You can do this by
-```python
-config.clear_cache()
-config.read()          # Read all configuration values again
-```
-
-
-
-### Supplied Config Sources
-#### `EnvironmentConfigSource`
-This just reads configuration from environment variables.
-```python
-from typedconfig.source import EnvironmentConfigSource
-source = EnvironmentConfigSource(prefix="XYZ")
-# OR just
-source = EnvironmentConfigSource()
-```
-It just takes one optional input argument, a prefix. This can be useful to avoid name clashes in environment variables.
-
-* If prefix is provided, environment variables are expected to look like `{PREFIX}_{SECTION}_{KEY}`, for example `export XYZ_DATABASE_PORT=2000`. 
-* If no prefix is provided, environment variables should look like `{SECTION}_{KEY}`, for example `export DATABASE_PORT=2000`.
-
-#### `IniFileConfigSource`
-This reads from an INI file using Python's built in [configparser](https://docs.python.org/3/library/configparser.html). Read the docs for `configparser` for more about the structure of the file.
-```python
-from typedconfig.source import IniFileConfigSource
-source = IniFileConfigSource("config.cfg", encoding='utf-8', must_exist=True)
-```
-
-* The first argument is the filename (absolute or relative to the current working directory).
-* `encoding` is the text encoding of the file. `configparser`'s default is used if not supplied.
-* `must_exist` - default `True`. If the file can't be found, an error will be thrown by default. Setting `must_exist` to be `False` allows the file not to be present, in which case this source will just report that it can't find any configuration values and your `Config` class will move onto looking in the next `ConfigSource`.
-
-#### `IniStringConfigSource`
-This reads from a string instead of a file
-```python
-from typedconfig.source import IniStringConfigSource
-source = IniStringConfigSource("""
-[section_name]
-key_name=key_value
-""")
-```
-
-#### `DictConfigSource`
-The most basic source, entirely in memory, and also useful when writing tests. It is case insensitive.
-```python
-from typedconfig.source import DictConfigSource
-source = DictConfigSource({
-    'database': dict(HOST='db1', PORT='2000'),
-    'algorithm': dict(MAX_VALUE='20', MIN_VALUE='10')
-})
-```
-
-It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
-
-This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
-
-#### `CmdConfigSource`
-This reads configuration from command line arguments
-```python
-from typedconfig.source import CmdConfigSource
-source = CmdConfigSource(prefix="XYZ")
-# OR just
-source = CmdConfigSource()
-```
-
-It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
-
-* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
-* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
-
-The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
-
-### Writing your own `ConfigSource`s
-An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
-
-Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
-```python
-import json
-from typing import Optional
-from typedconfig.source import ConfigSource
-
-class JsonConfigSource(ConfigSource):
-    def __init__(self, filename: str):
-        # Read data - will raise an exception if problem with file
-        with open(filename, 'r') as f:
-            self.data = json.load(f)
-        # Quick checks on data format
-        assert type(self.data) is dict
-        for k, v in self.data.items():
-            assert type(k) is str
-            assert type(v) is dict
-            for v_k, v_v in v.items():
-                assert type(v_k) is str
-                assert type(v_v) is str
-        # Convert all keys to lowercase
-        self.data = {
-            k.lower(): {
-                v_k.lower(): v_v
-                for v_k, v_v in v.items()
-            }
-            for k, v in self.data.items()
-        }    
-
-    def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
-        # Extract info from data which we read in during __init__
-        section = self.data.get(section_name.lower(), None)
-        if section is None:
-            return None
-        return section.get(key_name.lower(), None)
-```
-
-### Additional config sources
-In order to keep `typed-config` dependency free, `ConfigSources` requiring additional dependencies are in separate packages, which also have `typed-config` as a dependency.
-
-These are listed here:
-
-| pip install name | import name | Description |
-| --- | --- | --- |
-| [typed-config-aws-sources](https://pypi.org/project/typed-config-aws-sources) | `typedconfig_awssource` | Config sources using `boto3` to get config e.g. from S3 or DynamoDB
-
-
-## Cast function library
-The `typedconfig.casts` module contains helper functions that implement common casting operations. These would generally be passed to the `cast` parameter of the `key()` function
-
-### Casting to an `Enum` type with `enum_cast`
-the `enum_cast` function converts a string input from a source to a member of an `Enum` type. 
-
-For example:
-```python
-from enum import Enum
-from typedconfig.casts import enum_cast
-from typedconfig import Config, key
-...
-class ColorEnum(Enum):
-    RED = 1
-    GREEN = 2
-    BLUE = 3
-...
-
-class MyConfig(Config):
-    color = key(cast=enum_cast(ColorEnum))
-```
-
-In this example, if the `ConfigSource` reads the string `"RED"`, the value of `color` will be set to `ColorEnum.RED`
-
-Note that the `enum_cast` function is designed to read the *name* of an enum member, not its value (`1`, `2` or `3` in the example above)
-
-### Casting to a `tuple` with `tuple_cast`
-If the source contains a list of items, `tuple_cast` will parse them as a python tuple, optionally applying a 
-base_cast function to each element. 
-The default behavior is to call strip() on each element and ignore trailing delimiters.
-
-For example, given the input
-```ini
-nums = 1, 2, 3, 4,
-```
-
-Then you could use
-
-```python
-nums = key(cast=tuple_cast())
-```
-to read the string input and cast it to `("1", "2", "3", "4")`
-
-```python
-key(cast=tuple_cast(base_cast=int))
-```
-Would cast the input to `(1, 2, 3, 4)`
-
-```python
-key(cast=tuple_cast(ignore_trailing_delimiter=False))
-```
-Would cast the input to `("1", "2", "3", "4", "")`
-
-```python
-key(cast=tuple_cast(strip=False))
-```
-Would cast the input to `("1", " 2", " 3", " 4")`
-
-Finally, if a delimiter other that "," is used - say the input string is `"1:2:3:4"` - that can be handled like
-```python
-key(cast=tuple_cast(delimiter=":"))
-```
-
-### Casting to a `bool` with `boolean_cast`
-
-If the source is a boolean value, it can be converted to Python's `True` or `False` using this cast.
-
-```python
-key(cast=boolean_cast)
-```
-
-`boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
-
-Value | Strings
---- | ---
-`True` | `"true"`, `"yes"`, `"on"`, `"1"`
-`False` | `"false"`, `"no"`, `"off"`, `"0"`
-
-### Casting to an `Optional[bool]` with `optional_boolean_cast`
-
-If the source is a boolean value which can also be `None`, it can be converted to Python's `True` or `False` or `None` using this cast.
-
-```python
-key(cast=optional_boolean_cast)
-```
-
-`optional_boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
-
-Value | Strings
---- | ---
-`True` | `"true"`, `"yes"`, `"on"`, `"1"`
-`False` | `"false"`, `"no"`, `"off"`, `"0"`
-`None` | `"none"`, `"unknown"`
-
-
-## Contributing
-Ideas for new features and pull requests are welcome. PRs must come with tests included. This was developed using Python 3.7 but Travis tests run with all versions 3.6-3.9 too.
-
-### Development setup
-1. Clone the git repository
-2. Create a virtual environment `virtualenv venv`
-3. Activate the environment `venv/scripts/activate`
-4. Install development dependencies `pip install -r requirements.txt`
-
-### Code style
-Code style is `black` and this is checked by the CI. To autoformat your code as `black` before committing, just run `black typedconfig test`
-
-### Running tests
-`pytest`
-
-To run with coverage:
-
-`pytest --cov`
-
-### Making a release
-1. Bump version number in `typedconfig/__version__.py`
-1. Add changes to [CHANGELOG.md](CHANGELOG.md)
-1. Commit your changes and tag with `git tag -a v0.1.0 -m "Summary of changes"`
-1. Travis will deploy the release to PyPi for you.
-
-#### Staging release
-If you want to check how a release will look on PyPi before tagging and making it live, you can do the following:
-1. `pip install twine` if you don't already have it
-1. Bump version number in `typedconfig/__version__.py`
-1. Clear the dist directory `rm -r dist`
-1. `python setup.py sdist bdist_wheel`
-1. `twine check dist/*`
-1. Upload to the test PyPI `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
-1. Check all looks ok at [https://test.pypi.org/project/typed-config](https://test.pypi.org/project/typed-config)
-1. If all looks good you can git tag and push for deploy to live PyPi
-
-Here is [a good tutorial](https://realpython.com/pypi-publish-python-package) on publishing packages to PyPI.
+![Build Status](https://github.com/bwindsor/typed-config/actions/workflows/unit_test.yml/badge.svg)
+![Deploy Status](https://github.com/bwindsor/typed-config/actions/workflows/deploy_pypi.yml/badge.svg)
+[![codecov](https://codecov.io/gh/bwindsor/typed-config/branch/master/graph/badge.svg)](https://codecov.io/gh/bwindsor/typed-config)
+
+# typed-config
+Typed, extensible, dependency free configuration reader for Python projects for multiple config sources and working well in IDEs for great autocomplete performance.
+
+`pip install typed-config`
+
+Requires python 3.6 or above. (Also, needs `typing_extensions` for Python <= 3.7, so not completely dependency free if using old Python).
+
+## Basic usage
+```python
+# my_app/config.py
+from typedconfig import Config, key, section
+from typedconfig.source import EnvironmentConfigSource
+
+@section('database')
+class AppConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+    timeout = key(cast=float)
+
+config = AppConfig()
+config.add_source(EnvironmentConfigSource())
+config.read()
+```
+
+```python
+# my_app/main.py
+from my_app.config import config
+print(config.host)
+```
+In PyCharm, and hopefully other IDEs, it will recognise the datatypes of your configuration and allow you to autocomplete. No more remembering strings to get the right thing out!
+
+## Upgrading
+
+### From 0.x.x
+There is one breaking change when moving from `0.x.x` to `1.x.x`. The `key` function now expects all arguments to be keyword arguments. So simply replace any calls like so:
+```python
+key('section', 'key', True, str, 'default')  # 0.x.x
+key(section_name='section', key_name='key', required=True, cast=str, default='default')  # 1.x.x
+```
+The reason for this change is to tie down the return type of `key` properly. Previously, when `required=False` or when `cast=None` the return type would not include the possibility of `None` or `string`. The type checker should now be able to infer the return type based on the values of `required`, `cast` and `default`.
+
+###  From 1.x.x
+When upgrading from `1.x.x` to `2.x.x`, Python 3.7 no longer supported as it is end of life. As long as you are using Python >= 3.8, everything should just work.
+
+## How it works
+Configuration is always supplied in a two level structure, so your source configuration can have multiple sections, and each section contains multiple key/value configuration pairs. For example:
+```ini
+[database]
+host = 127.0.0.1
+port = 2000
+
+[algorithm]
+max_value = 10
+min_value = 20
+```
+
+You then create your configuration hierarchy in code (this can be flat or many levels deep) and supply the matching between strings in your config sources and properties of your configuration classes.
+
+You provide one or more `ConfigSource`s, from which the config for your application can be read. For example, you might supply an `EnvironmentConfigSource`,  and two `IniFileConfigSource`s. This would make your application first look for a configuration value in environment variables, if not found there it would then look at the first INI file (perhaps a user-specific file), before falling back to the second INI file (perhaps a default configuration shared between all users). If a parameter is still not found and is a required parameter, an error would be thrown.
+
+There is emphasis on type information being available for everything so that an IDE will autocomplete when trying to use your config across your application.
+
+### Multiple data sources
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+    username = key(cast=str)
+    password = key(cast=str)
+
+config = DatabaseConfig()
+config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+config.add_source(IniFileConfigSource("config.cfg"))
+
+# OR provide sources directly to the constructor
+config = DatabaseConfig(sources=[
+    EnvironmentConfigSource(prefix="EXAMPLE"),
+    IniFileConfigSource("config.cfg")
+])
+```
+
+Since you don't want to hard code your secret credentials, you might supply them through the environment.
+So for the above configuration, the environment might look like this:
+```bash
+export EXAMPLE_DATABASE_USERNAME=my_username
+export EXAMPLE_DATABASE_PASSWORD=my_very_secret_password
+export EXAMPLE_DATABASE_PORT=2001
+```
+
+Those values which couldn't be found in the environment would then be read from the INI file, which might look like this:
+```ini
+[database]
+HOST = db1.mydomain.com
+PORT = 2000
+```
+
+Note after this, `config.port` will be equal to `2001` as the value in the environment took priority over the value in the INI file.
+
+### Caching
+When config values are first used, they are read. This is lazy evaluation by default so that not everything is read if not necessary.
+
+After first use, they are cached in memory so that there should be no further I/O if the config value is used again.
+
+For fail fast behaviour, and also to stop unexpected latency when a config value is read partway through your application (e.g. your config could be coming across a network), the option is available to read all config values at the start. Just call
+
+`config.read()`
+
+This will throw an exception if any required config value cannot be found, and will also keep all read config values in memory for next time they are used. If you do not use `read` you will only get the exception when you first try to use the offending config key.
+
+### Hierarchical configuration
+Use `group_key` to represent a "sub-config" of a configuration. Set up "sub-configs" exactly as demonstrated above, and then create a parent config to compose them in one place.
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+
+@section('algorithm')
+class AlgorithmConfig(Config):
+    max_value = key(cast=float)
+    min_value = key(cast=float)
+
+class ParentConfig(Config):
+    database = group_key(DatabaseConfig)
+    algorithm = group_key(AlgorithmConfig)
+    description = key(cast=str, section_name="general")
+
+config = ParentConfig()
+config.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+config.add_source(IniFileConfigSource("config.cfg"))
+config.read()
+```
+
+The first time the `config.database` or `config.algorithm` is accessed (which in the case above is when `read()` is called), then an instance will be instantiated. Notice that it is the class definition, not an instance of the class, which is passed to the `group_key` function.
+
+### Custom section/key names, optional parameters, default values
+Let's take a look at this:
+```python
+from typedconfig import Config, key, section
+
+@section('database')
+class AppConfig(Config):
+    host1 = key()
+    host2 = key(section_name='database', key_name='HOST2',
+                required=True, cast=str, default=None)
+```
+Both `host1` and `host2` are legitimate configuration key definitions.
+
+* `section_name` - this name of the section in the configuration source from which this parameter should be read. This can be provided on a key-by-key basis, but if it is left out then the section name supplied by the `@section` decorator is used. If all keys supply a `section_name`, the class decorator is not needed. If both `section_name` and a decorator are provided, the `section_name` argument takes priority.
+* `key_name` - the name of this key in the configuration source from which this parameter is read. If not supplied, some magic uses the object property name as the key name.
+* `required` - default True. If False, and the configuration value can't be found, no error will be thrown and the default value will be used, if provided. If a default not provided, `None` will be used.
+* `cast` - probably the most important option for typing. **If you want autocomplete typing support you must specify this**. It's just a function which takes a string as an input and returns a parsed value. See the casting section for more. If not supplied, the value remains as a string.
+* `default` - only applicable if `required` is false. When `required` is false this value is used if a value cannot be found.
+
+### Types
+```python
+from typedconfig import Config, key, section
+from typing import List
+
+def split_str(s: str) -> List[str]:
+    return [x.strip() for x in s.split(",")]
+
+@section('database')
+class AppConfig(Config):
+    host = key()
+    port = key(cast=int)
+    users = key(cast=split_str)
+    zero_based_index = key(cast=lambda x: int(x)-1)
+config = AppConfig(sources=[...])
+```
+In this example we have three ways of casting:
+1. Not casting at all. This defaults to returning a `str`, but your IDE won't know that so if you want type hints use `cast=str`
+2. Casting to an built in type which can take a string input and parse it, for example `int`
+3. Defining a custom function. Your function should take one string input and return one output of any type. To get type hint, just make sure your function has type annotations.
+4. Using a lambda expression. The type inference may or may not work depending on your expression, so if it doesn't just write it as a function with type annotations.
+
+### Validation
+You can validate what has been supplied by providing a custom `cast` function to a `key`, which validates the configuration value in addition to parsing it.
+
+### Extending configuration using shared ConfigProvider
+
+Multiple application modules may use different configuration schemes while sharing the same configuration source. Analogously, various `Config` classes may provide different view of the same configuration data, sharing the same `ConfigProvider`.
+
+```python
+# app/config.py
+from typedconfig.provider import ConfigProvider
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+provider = ConfigProvider()
+provider.add_source(EnvironmentConfigSource(prefix="EXAMPLE"))
+provider.add_source(IniFileConfigSource("config.cfg"))
+
+__all__ = ["provider"]
+```
+```python
+# app/database/config.py
+from typedconfig import Config, key, section
+from app.config import provider
+
+@section('database')
+class DatabaseConfig(Config):
+    host = key(cast=str)
+    port = key(cast=int)
+
+database_config = DatabaseConfig(provider=provider)
+```
+```python
+# app/algorithm/config.py
+from typedconfig import Config, key, section
+from app.config import provider
+
+@section('algorithm')
+class AlgorithmConfig(Config):
+    max_value = key(cast=float)
+    min_value = key(cast=float)
+
+algorithm_config = AlgorithmConfig(provider=provider)
+```
+
+Shared configuration provider can be used by plugins, which may need to declare additional configuration sections within the same configuration files as the main application.  Let's assume we have `[database]` section used by main application and `[app_extension]` that provides 3rd party plugin configuration:
+
+```ini
+[database]
+host = 127.0.0.1
+port = 2000
+
+[app_extension]
+api_key = secret
+```
+
+e.g. `app/config.py` may look like that:
+
+```python
+from typedconfig import Config, key, section, group_key
+from typedconfig.source import EnvironmentConfigSource, IniFileConfigSource
+
+@section('database')
+class DatabaseConfig(Config):
+    """Database configuration"""
+    host = key(cast=str)
+    port = key(cast=int)
+
+class ApplicationConfig(Config):
+    """Main configuration object"""
+    database = group_key(DatabaseConfig)
+
+app_config = ApplicationConfig(sources=[
+    EnvironmentConfigSource(),
+    IniFileConfigSource("config.cfg")
+])
+```
+
+and plugin can read additional sections by using the same configuration provider as main application config.
+
+e.g. `plugin/config.py`:
+```python
+from typedconfig import Config, key, section, group_key
+
+from app.config import ApplicationConfig, app_config
+
+@section('app_extension')
+class ExtensionConfig(Config):
+    """Extension configuration"""
+    api_key = key(cast=str)
+
+# ExtendedAppConfig extends ApplicationConfig 
+# so original sections are also included
+class ExtendedAppConfig(ApplicationConfig):
+    """Extended main configuration object"""
+    app_extension = group_key(ExtensionConfig)
+    
+# ExtendedAppConfig uses the same provider as the main app_config
+extended_config = ExtendedAppConfig(provider=app_config.provider)
+```
+```python
+from plugin.config import extended_config
+
+# Plugin can access both main and extra sections
+print(extended_config.app_extension.api_key)
+print(extended_config.database.host)
+```
+
+### Configuration variables which depend on other configuration variables
+Sometimes you may wish to set the value of some configuration variables based on others. You may also wish to validate some variables, for example allowed values may be different depending on the value of another config variable. For this you can add a `post_read_hook`.
+
+The default implementation of `post_read_hook` returns an empty `dict`. You can override this by implementing your own `post_read_hook` method. It should receive only `self` as an input, and return a `dict`. This `dict` should be a simple mapping from config keys to values. For hierarchical configurations, you can nest the dictionaries. If you provide a `post_read_hook` in both a parent and a child class which both make changes to the same keys (don't do this) then the values returned by the child method will overwrite those by the parent.
+
+This hook is called whenever you call the `read` method. If you use lazy loading and skip calling the `read` method, you cannot use this hook.
+```python
+# my_app/config.py
+from typedconfig import Config, key, group_key, section
+from typedconfig.source import EnvironmentConfigSource
+
+@section('child')
+class ChildConfig(Config):
+    http_port_plus_one = key(cast=int, required=False)
+
+@section('app')
+class AppConfig(Config):
+    use_https = key(cast=bool)
+    http_port = key(key_name='port', cast=int, required=False)
+    child = group_key(ChildConfig)
+    
+    def post_read_hook(self) -> dict:
+        config_updates = dict()
+        # If the port has not been provided, set it based on the value of use_https
+        if self.http_port is None:
+            config_updates.update(http_port=443 if self.use_https else 80)
+        else:
+            # Modify child config
+            config_updates.update(child=dict(http_port_plus_one=self.http_port + 1))
+            
+        # Validate that the port number has a sensible value
+        # It is recommended to do validation inside the cast method for individual keys, however for dependent keys it can be useful here
+        if self.http_port is not None:
+            if self.use_https:
+                assert self.http_port in [443, 444, 445]
+            else:
+                assert self.http_port in [80, 81, 82]
+
+        return config_updates
+            
+config = AppConfig()
+config.add_source(EnvironmentConfigSource())
+config.read()
+```
+
+## Configuration Sources
+Configuration sources are how your main `Config` class knows where to get its data from. These are totally extensible so that you can read in your configuration from wherever you like - from a database, from S3, anywhere that you can write code for.
+
+You supply your configuration source to your config after you've instantiated it, but **before** you try to read any data from it:
+```python
+config = AppConfig()
+config.add_source(my_first_source)
+config.add_source(my_second_source)
+config.read()
+```
+Or you can supply the sources directly in the constructor like this:
+```python
+config = AppConfig(sources=[my_first_source, my_second_source])
+config.read()
+```
+
+
+### Modifying or refreshing configuration after it has been loaded
+In general it is bad practice to modify configuration at runtime because the configuration for your program should be fixed for the duration of it.  However, there are cases where it may be necessary.
+
+To completely replace the set of config sources, you can use
+```python
+config = AppConfig(sources=[my_first_source, my_second_source])
+config.set_sources([my_first_new_source, my_second_new_source])
+```
+
+To replace a specific config source, for example because a config file has changed and you need to re-read it from disk, you can use `replace_source`:
+```python
+from typedconfig.source import IniFileConfigSource
+original_source = IniFileConfigSource("config.cfg")
+config = AppConfig(sources=[source])
+# Now say you change the contents to config.cfg and need to read it again
+new_source = IniFileConfigSource("config.cfg")  # re-reads file during construction
+config.replace_source(original_source, new_source)
+```
+
+**Important**: if you add or modify the config sources the config has been read, or need to refresh the config for some reason, you'll need to clear any cached values in order to force the config to be fetched from the `ConfigSource`s again. You can do this by
+```python
+config.clear_cache()
+config.read()          # Read all configuration values again
+```
+
+
+
+### Supplied Config Sources
+#### `EnvironmentConfigSource`
+This just reads configuration from environment variables.
+```python
+from typedconfig.source import EnvironmentConfigSource
+source = EnvironmentConfigSource(prefix="XYZ")
+# OR just
+source = EnvironmentConfigSource()
+```
+It just takes one optional input argument, a prefix. This can be useful to avoid name clashes in environment variables.
+
+* If prefix is provided, environment variables are expected to look like `{PREFIX}_{SECTION}_{KEY}`, for example `export XYZ_DATABASE_PORT=2000`. 
+* If no prefix is provided, environment variables should look like `{SECTION}_{KEY}`, for example `export DATABASE_PORT=2000`.
+
+#### `IniFileConfigSource`
+This reads from an INI file using Python's built in [configparser](https://docs.python.org/3/library/configparser.html). Read the docs for `configparser` for more about the structure of the file.
+```python
+from typedconfig.source import IniFileConfigSource
+source = IniFileConfigSource("config.cfg", encoding='utf-8', must_exist=True)
+```
+
+* The first argument is the filename (absolute or relative to the current working directory).
+* `encoding` is the text encoding of the file. `configparser`'s default is used if not supplied.
+* `must_exist` - default `True`. If the file can't be found, an error will be thrown by default. Setting `must_exist` to be `False` allows the file not to be present, in which case this source will just report that it can't find any configuration values and your `Config` class will move onto looking in the next `ConfigSource`.
+
+#### `IniStringConfigSource`
+This reads from a string instead of a file
+```python
+from typedconfig.source import IniStringConfigSource
+source = IniStringConfigSource("""
+[section_name]
+key_name=key_value
+""")
+```
+
+#### `DictConfigSource`
+The most basic source, entirely in memory, and also useful when writing tests. It is case insensitive.
+```python
+from typedconfig.source import DictConfigSource
+source = DictConfigSource({
+    'database': dict(HOST='db1', PORT='2000'),
+    'algorithm': dict(MAX_VALUE='20', MIN_VALUE='10')
+})
+```
+
+It expects data type `Dict[str, Dict[str, str]]`, i.e. such that `string_value = d['section_name']['key_name']`. Everything should be provided as string data so that it can be parsed in the same way as if data was coming from a file or elsewhere.
+
+This is an alternative way of supplying default values instead of using the `default` option when defining your `key`s. Just provide a `DictConfigSource` as the lowest priority source, containing your defaults.
+
+#### `CmdConfigSource`
+This reads configuration from command line arguments
+```python
+from typedconfig.source import CmdConfigSource
+source = CmdConfigSource(prefix="XYZ")
+# OR just
+source = CmdConfigSource()
+```
+
+It will use Python's `argparse` library to extract the relevant command line arguments. It takes an optional input argument, the `prefix`. This can be useful if you also accept other command line arguments and wish to avoid clashes with your own arguments.
+
+* Arguments will be expected in the format `--{PREFIX}_{SECTION}_{KEY} {VALUE}`, for example `--xyz_database_port 2000`
+* If no `prefix` is provided, arguments will be expected in the format `--{SECTION}_{KEY} {VALUE}`, for example `--database_port 2000`
+
+The names are case insensitive so, for example, `--DATABASE_PORT` and `--database_port` would be treated the same.
+
+### Writing your own `ConfigSource`s
+An abstract base class `ConfigSource` is supplied. You should extend it and implement the method `get_config_value` as demonstrated below, which takes a section name and key name, and returns either a `str` config value, or `None` if the value could not be found. It should not error if the value cannot be found, `Config` will throw an error later if it still can't find the value in any of its other available sources. To make it easier for the user try to make your source case insensitive.
+
+Here's an outline of how you might implement a source to read your config from a JSON file, for example. Use the `__init__` method to provide any information your source needs to fetch the data, such as filename, api details, etc. You can do sanity checks in the `__init__` method and throw an error if something is wrong.
+```python
+import json
+from typing import Optional
+from typedconfig.source import ConfigSource
+
+class JsonConfigSource(ConfigSource):
+    def __init__(self, filename: str):
+        # Read data - will raise an exception if problem with file
+        with open(filename, 'r') as f:
+            self.data = json.load(f)
+        # Quick checks on data format
+        assert type(self.data) is dict
+        for k, v in self.data.items():
+            assert type(k) is str
+            assert type(v) is dict
+            for v_k, v_v in v.items():
+                assert type(v_k) is str
+                assert type(v_v) is str
+        # Convert all keys to lowercase
+        self.data = {
+            k.lower(): {
+                v_k.lower(): v_v
+                for v_k, v_v in v.items()
+            }
+            for k, v in self.data.items()
+        }    
+
+    def get_config_value(self, section_name: str, key_name: str) -> Optional[str]:
+        # Extract info from data which we read in during __init__
+        section = self.data.get(section_name.lower(), None)
+        if section is None:
+            return None
+        return section.get(key_name.lower(), None)
+```
+
+### Additional config sources
+In order to keep `typed-config` dependency free, `ConfigSources` requiring additional dependencies are in separate packages, which also have `typed-config` as a dependency.
+
+These are listed here:
+
+| pip install name | import name | Description |
+| --- | --- | --- |
+| [typed-config-aws-sources](https://pypi.org/project/typed-config-aws-sources) | `typedconfig_awssource` | Config sources using `boto3` to get config e.g. from S3 or DynamoDB
+
+
+## Cast function library
+The `typedconfig.casts` module contains helper functions that implement common casting operations. These would generally be passed to the `cast` parameter of the `key()` function
+
+### Casting to an `Enum` type with `enum_cast`
+the `enum_cast` function converts a string input from a source to a member of an `Enum` type. 
+
+For example:
+```python
+from enum import Enum
+from typedconfig.casts import enum_cast
+from typedconfig import Config, key
+...
+class ColorEnum(Enum):
+    RED = 1
+    GREEN = 2
+    BLUE = 3
+...
+
+class MyConfig(Config):
+    color = key(cast=enum_cast(ColorEnum))
+```
+
+In this example, if the `ConfigSource` reads the string `"RED"`, the value of `color` will be set to `ColorEnum.RED`
+
+Note that the `enum_cast` function is designed to read the *name* of an enum member, not its value (`1`, `2` or `3` in the example above)
+
+### Casting to a `tuple` with `tuple_cast`
+If the source contains a list of items, `tuple_cast` will parse them as a python tuple, optionally applying a 
+base_cast function to each element. 
+The default behavior is to call strip() on each element and ignore trailing delimiters.
+
+For example, given the input
+```ini
+nums = 1, 2, 3, 4,
+```
+
+Then you could use
+
+```python
+nums = key(cast=tuple_cast())
+```
+to read the string input and cast it to `("1", "2", "3", "4")`
+
+```python
+key(cast=tuple_cast(base_cast=int))
+```
+Would cast the input to `(1, 2, 3, 4)`
+
+```python
+key(cast=tuple_cast(ignore_trailing_delimiter=False))
+```
+Would cast the input to `("1", "2", "3", "4", "")`
+
+```python
+key(cast=tuple_cast(strip=False))
+```
+Would cast the input to `("1", " 2", " 3", " 4")`
+
+Finally, if a delimiter other that "," is used - say the input string is `"1:2:3:4"` - that can be handled like
+```python
+key(cast=tuple_cast(delimiter=":"))
+```
+
+### Casting to a `bool` with `boolean_cast`
+
+If the source is a boolean value, it can be converted to Python's `True` or `False` using this cast.
+
+```python
+key(cast=boolean_cast)
+```
+
+`boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
+
+Value | Strings
+--- | ---
+`True` | `"true"`, `"yes"`, `"on"`, `"1"`
+`False` | `"false"`, `"no"`, `"off"`, `"0"`
+
+### Casting to an `Optional[bool]` with `optional_boolean_cast`
+
+If the source is a boolean value which can also be `None`, it can be converted to Python's `True` or `False` or `None` using this cast.
+
+```python
+key(cast=optional_boolean_cast)
+```
+
+`optional_boolean_cast` supports the following values and is case-insensitive. Any other values will result in a `KeyError` while parsing.
+
+Value | Strings
+--- | ---
+`True` | `"true"`, `"yes"`, `"on"`, `"1"`
+`False` | `"false"`, `"no"`, `"off"`, `"0"`
+`None` | `"none"`, `"unknown"`
+
+
+## Contributing
+Ideas for new features and pull requests are welcome. PRs must come with tests included. This is developed using Python 3.9 but Github actions will run tests with all versions 3.8-3.12 too.
+
+### Development setup
+1. Clone the git repository
+2. Create a virtual environment `virtualenv venv`
+3. Activate the environment `venv/scripts/activate`
+4. Install development dependencies `pip install -r requirements.txt`
+
+### Code style
+Code style is `black` and this is checked by the CI. To autoformat your code as `black` before committing, just run `black typedconfig test`
+
+### Running tests
+`pytest`
+
+To run with coverage:
+
+`pytest --cov`
+
+### Making a release
+1. Bump version number in `typedconfig/__version__.py`
+1. Add changes to [CHANGELOG.md](CHANGELOG.md)
+1. Commit your changes and tag with `git tag -a v0.1.0 -m "Summary of changes"`
+1. Github actions will deploy the release to PyPi for you.
+
+#### Staging release
+If you want to check how a release will look on PyPi before tagging and making it live, you can do the following:
+1. `pip install twine` if you don't already have it
+1. Bump version number in `typedconfig/__version__.py`
+1. Clear the dist directory `rm -r dist`
+1. `python setup.py sdist bdist_wheel`
+1. `twine check dist/*`
+1. Upload to the test PyPI `twine upload --repository-url https://test.pypi.org/legacy/ dist/*`
+1. Check all looks ok at [https://test.pypi.org/project/typed-config](https://test.pypi.org/project/typed-config)
+1. If all looks good you can git tag and push for deploy to live PyPi
+
+Here is [a good tutorial](https://realpython.com/pypi-publish-python-package) on publishing packages to PyPI.
```

### Comparing `typed-config-1.5.0/typedconfig/casts.py` & `typed-config-2.0.3/typedconfig/casts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,159 +1,157 @@
-import configparser
-from enum import Enum
-from typing import Callable, Optional, Type, TypeVar, Tuple, Union, overload
-
-T = TypeVar("T")
-TEnum = TypeVar("TEnum", bound="Enum")
-
-
-def enum_cast(enum_type: Type[TEnum]) -> Callable[[str], TEnum]:
-    """
-    A cast function that translates a string input into a member of named Enum
-    Throws a KeyError of the string is not in the given Enum
-
-    Parameters
-    ----------
-    enum_type
-       The EnumType that the string input should be cast to
-
-    Returns
-    -------
-    Cast method that can be used with the key() function
-    """
-
-    def getter(name: str) -> TEnum:
-        try:
-            return enum_type[name]
-        except KeyError:
-            raise KeyError(f"{name} is not a member of {enum_type}")
-
-    return getter
-
-
-@overload
-def tuple_cast(
-    base_cast: None = None,
-    delimiter: str = ...,
-    ignore_trailing_delimiter: bool = ...,
-    strip: bool = ...,
-) -> Callable[[str], Tuple[str, ...]]:
-    ...
-
-
-@overload
-def tuple_cast(
-    base_cast: Callable[[str], T],
-    delimiter: str = ...,
-    ignore_trailing_delimiter: bool = ...,
-    strip: bool = ...,
-) -> Callable[[str], Tuple[T, ...]]:
-    ...
-
-
-def tuple_cast(
-    base_cast: Optional[Callable[[str], T]] = None,
-    delimiter: str = ",",
-    ignore_trailing_delimiter: bool = True,
-    strip: bool = True,
-) -> Callable[[str], Union[Tuple[T, ...], Tuple[str, ...]]]:
-    """
-    A cast function that creates a list based on the given base_cast function.
-    If no base_cast method is provided, returns a list of str.
-
-    Parameters
-    ----------
-    base_cast:
-        function to be applied to each member of the parsed list before returning. If base_cast is None, the
-        cast function will return a list of strings
-    delimiter:
-        delimiter to use to separate elements when parsing the input. Default is a comma.
-    ignore_trailing_delimiter:
-        How to interpret a trailing delimiter, as in "one,two,three,".
-        If True (the default) the funal comma will be dropped
-        If False, the list would end with a single empty string
-    strip:
-        Whether to call strip() on each element of the parsed strings.
-        If True (the default) an input like "a, b, c" will be cast as ["a", "b", "c"]
-        If False an input like "a, b, c" will be cast as ["a", "b ", "c "], with no
-        extraneous whitespace removed
-
-    Returns
-    -------
-    Cast method that can be used with the key() function
-    """
-
-    def getter(s: str) -> Union[Tuple[T, ...], Tuple[str, ...]]:
-        # If the string is empty string, allways return empty list
-        # The empty list needs an explicit type to make mypy happy
-        if len(s) == 0:
-            if base_cast is None:
-                str_tuple: Tuple[str, ...] = tuple()
-                return str_tuple
-            else:
-                t_tuple: Tuple[T, ...] = tuple()
-                return t_tuple
-
-        str_list = s.split(delimiter)
-
-        # remove whitespace if the strip arg is True
-        if strip:
-            str_list = [s.strip() for s in str_list]
-
-        # remove the final element if it is empty and we should ignore trailing delimiters
-        if ignore_trailing_delimiter and len(str_list[-1]) == 0:
-            str_list.pop()
-
-        # no base_cast means just a list of str
-        if base_cast is None:
-            return tuple(str_list)
-
-        return tuple(base_cast(s) for s in str_list)
-
-    return getter
-
-
-def boolean_cast(s: str) -> bool:
-    """
-    Casts a string to a boolean using the values supplied by configparser.ConfigParser.BOOLEAN_STATES.
-    This function is designed to be passed directly to the key() function.
-
-    The following are interpreted as True: "0", "true", "on", "yes"
-    The following are interpreted as False: "1", "false", "off", "no"
-
-    This method is case insensitive.
-    Other inputs will result in an error.
-
-    Parameters
-    ----------
-    s - string to cast to boolean
-
-    Returns
-    -------
-    Boolean.
-    """
-    return configparser.ConfigParser.BOOLEAN_STATES[s.lower()]
-
-
-def optional_boolean_cast(s: str) -> Optional[bool]:
-    """
-    Casts a string to an optional boolean using the values supplied by configparser.ConfigParser.BOOLEAN_STATES.
-    This function is designed to be passed directly to the key() function.
-
-    The following are interpreted as True: "0", "true", "on", "yes"
-    The following are interpreted as False: "1", "false", "off", "no"
-    The following are interpreted as None: "none", "unknown"
-
-    This method is case insensitive.
-    Other inputs will result in an error.
-
-    Parameters
-    ----------
-    s - string to cast to optional boolean
-
-    Returns
-    -------
-    Boolean or None
-    """
-    if s.lower() in ["none", "unknown"]:
-        return None
-    return boolean_cast(s)
+import configparser
+from enum import Enum
+from typing import Callable, Optional, Type, TypeVar, Tuple, Union, overload
+
+T = TypeVar("T")
+TEnum = TypeVar("TEnum", bound="Enum")
+
+
+def enum_cast(enum_type: Type[TEnum]) -> Callable[[str], TEnum]:
+    """
+    A cast function that translates a string input into a member of named Enum
+    Throws a KeyError of the string is not in the given Enum
+
+    Parameters
+    ----------
+    enum_type
+       The EnumType that the string input should be cast to
+
+    Returns
+    -------
+    Cast method that can be used with the key() function
+    """
+
+    def getter(name: str) -> TEnum:
+        try:
+            return enum_type[name]
+        except KeyError:
+            raise KeyError(f"{name} is not a member of {enum_type}")
+
+    return getter
+
+
+@overload
+def tuple_cast(
+    base_cast: None = None,
+    delimiter: str = ...,
+    ignore_trailing_delimiter: bool = ...,
+    strip: bool = ...,
+) -> Callable[[str], Tuple[str, ...]]: ...
+
+
+@overload
+def tuple_cast(
+    base_cast: Callable[[str], T],
+    delimiter: str = ...,
+    ignore_trailing_delimiter: bool = ...,
+    strip: bool = ...,
+) -> Callable[[str], Tuple[T, ...]]: ...
+
+
+def tuple_cast(
+    base_cast: Optional[Callable[[str], T]] = None,
+    delimiter: str = ",",
+    ignore_trailing_delimiter: bool = True,
+    strip: bool = True,
+) -> Callable[[str], Union[Tuple[T, ...], Tuple[str, ...]]]:
+    """
+    A cast function that creates a list based on the given base_cast function.
+    If no base_cast method is provided, returns a list of str.
+
+    Parameters
+    ----------
+    base_cast:
+        function to be applied to each member of the parsed list before returning. If base_cast is None, the
+        cast function will return a list of strings
+    delimiter:
+        delimiter to use to separate elements when parsing the input. Default is a comma.
+    ignore_trailing_delimiter:
+        How to interpret a trailing delimiter, as in "one,two,three,".
+        If True (the default) the funal comma will be dropped
+        If False, the list would end with a single empty string
+    strip:
+        Whether to call strip() on each element of the parsed strings.
+        If True (the default) an input like "a, b, c" will be cast as ["a", "b", "c"]
+        If False an input like "a, b, c" will be cast as ["a", "b ", "c "], with no
+        extraneous whitespace removed
+
+    Returns
+    -------
+    Cast method that can be used with the key() function
+    """
+
+    def getter(s: str) -> Union[Tuple[T, ...], Tuple[str, ...]]:
+        # If the string is empty string, allways return empty list
+        # The empty list needs an explicit type to make mypy happy
+        if len(s) == 0:
+            if base_cast is None:
+                str_tuple: Tuple[str, ...] = tuple()
+                return str_tuple
+            else:
+                t_tuple: Tuple[T, ...] = tuple()
+                return t_tuple
+
+        str_list = s.split(delimiter)
+
+        # remove whitespace if the strip arg is True
+        if strip:
+            str_list = [s.strip() for s in str_list]
+
+        # remove the final element if it is empty and we should ignore trailing delimiters
+        if ignore_trailing_delimiter and len(str_list[-1]) == 0:
+            str_list.pop()
+
+        # no base_cast means just a list of str
+        if base_cast is None:
+            return tuple(str_list)
+
+        return tuple(base_cast(s) for s in str_list)
+
+    return getter
+
+
+def boolean_cast(s: str) -> bool:
+    """
+    Casts a string to a boolean using the values supplied by configparser.ConfigParser.BOOLEAN_STATES.
+    This function is designed to be passed directly to the key() function.
+
+    The following are interpreted as True: "0", "true", "on", "yes"
+    The following are interpreted as False: "1", "false", "off", "no"
+
+    This method is case insensitive.
+    Other inputs will result in an error.
+
+    Parameters
+    ----------
+    s - string to cast to boolean
+
+    Returns
+    -------
+    Boolean.
+    """
+    return configparser.ConfigParser.BOOLEAN_STATES[s.lower()]
+
+
+def optional_boolean_cast(s: str) -> Optional[bool]:
+    """
+    Casts a string to an optional boolean using the values supplied by configparser.ConfigParser.BOOLEAN_STATES.
+    This function is designed to be passed directly to the key() function.
+
+    The following are interpreted as True: "0", "true", "on", "yes"
+    The following are interpreted as False: "1", "false", "off", "no"
+    The following are interpreted as None: "none", "unknown"
+
+    This method is case insensitive.
+    Other inputs will result in an error.
+
+    Parameters
+    ----------
+    s - string to cast to optional boolean
+
+    Returns
+    -------
+    Boolean or None
+    """
+    if s.lower() in ["none", "unknown"]:
+        return None
+    return boolean_cast(s)
```

### Comparing `typed-config-1.5.0/typedconfig/config.py` & `typed-config-2.0.3/typedconfig/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,433 +1,424 @@
-import sys
-import typing
-from itertools import chain
-from typing import TypeVar, List, Optional, Callable, Type, Union, Tuple, Any, overload, Dict
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    # Python <= 3.7
-    from typing_extensions import Literal
-from typedconfig.provider import ConfigProvider
-from typedconfig.source import ConfigSource
-import logging
-import inspect
-
-logger = logging.getLogger(__name__)
-
-TConfig = TypeVar("TConfig", bound="Config")
-T = TypeVar("T")
-U = TypeVar("U")
-V = TypeVar("V")
-
-"""
-required | cast | default | return_type
-True  | None/missing    | -       | str
-True  | NotNone | -       | T
-
-False | NotNone | None/missing | Optional[T]
-False | NotNone | NotNone | T
-False | None    | -       | Union[str, Optional[T]]
-"""
-
-
-@overload
-def key(
-    *,
-    section_name: Optional[str] = ...,
-    key_name: Optional[str] = ...,
-    required: Literal[False],
-    cast: Callable[[str], T],
-    default: T,
-) -> T:
-    ...
-
-
-@overload
-def key(
-    *,
-    section_name: Optional[str] = ...,
-    key_name: Optional[str] = ...,
-    required: Literal[False],
-    cast: Callable[[str], T],
-    default: None = ...,
-) -> Optional[T]:
-    ...
-
-
-@overload
-def key(
-    *,
-    section_name: Optional[str] = ...,
-    key_name: Optional[str] = ...,
-    required: Literal[False],
-    cast: None = ...,
-    default: Optional[T] = ...,
-) -> Union[str, Optional[T]]:
-    ...
-
-
-@overload
-def key(
-    *,
-    section_name: Optional[str] = ...,
-    key_name: Optional[str] = ...,
-    required: Literal[True] = ...,
-    cast: Callable[[str], T],
-    default: Optional[T] = ...,
-) -> T:
-    ...
-
-
-@overload
-def key(
-    *,
-    section_name: Optional[str] = ...,
-    key_name: Optional[str] = ...,
-    required: Literal[True] = ...,
-    cast: None = ...,
-    default: Optional[T] = ...,
-) -> str:
-    ...
-
-
-def key(
-    *,
-    section_name: Optional[str] = None,
-    key_name: Optional[str] = None,
-    required: bool = True,
-    cast: Optional[Callable[[str], T]] = None,
-    default: Optional[T] = None,
-) -> Union[Optional[T], str]:
-    """
-    Provides a getter for a configuration key
-    Parameters
-    ----------
-    section_name: section name where the key resides. If not specified,
-        the @section decorator should be used on the Config class to specify it
-    key_name: key name within the specified section. If not specified,
-        the python key name will be capitalised and used
-    required: optional, default True. Whether the key is required or optional
-    cast: optional, default None (no cast). Function taking a string argument and returning the parsed value
-    default: optional, default None. If required is set to False, the value to use if the config value is not found
-    """
-
-    # In general, this should not store any state since the class property is shared across instances. However, the
-    # property name will be the same across all instances, so when this is looked up the first time it is ok to store
-    # it.
-    _mutable_state = {"key_name": key_name.upper() if key_name is not None else None}
-
-    def getter_method(self: Config) -> Union[Optional[T], str]:
-        """
-        Returns
-        -------
-        value: the parsed config value
-        """
-
-        resolved_section_name = self._resolve_section_name(section_name)
-
-        resolved_key_name = _mutable_state["key_name"]
-        if resolved_key_name is None:
-            resolved_key_name = self._resolve_key_name(getter)
-            _mutable_state["key_name"] = resolved_key_name
-
-        # If value is cached, just use the cached value
-        cached_value: Union[T, str] = self._provider.get_from_cache(resolved_section_name, resolved_key_name)
-        if cached_value is not None:
-            return cached_value
-
-        string_value = self._provider.get_key(resolved_section_name, resolved_key_name)
-        cast_value: Union[Optional[T], str] = None
-
-        # If we still haven't found a config value and this parameter is required,
-        # raise an exception, otherwise use the default
-        if string_value is None:
-            if required:
-                raise KeyError("Config parameter {0}.{1} not found".format(resolved_section_name, resolved_key_name))
-            else:
-                if default is not None:
-                    cast_value = default
-        else:
-            # If a casting function has been specified then cast to the required data type
-            if cast is not None:
-                cast_value = cast(string_value)
-            else:
-                cast_value = string_value
-
-        # Cache this for next time if still not none
-        if cast_value is not None:
-            self._provider.add_to_cache(resolved_section_name, resolved_key_name, cast_value)
-
-        return cast_value
-
-    getter = property(getter_method)
-    setattr(getter.fget, Config._config_key_registration_string, True)
-    setattr(getter.fget, Config._config_key_key_name_string, key_name.upper() if key_name is not None else None)
-    setattr(getter.fget, Config._config_key_section_name_string, section_name)
-    return typing.cast(Union[Optional[T], str], getter)
-
-
-def group_key(cls: Type[TConfig], *, group_section_name: Optional[str] = None, hierarchical: bool = False) -> TConfig:
-    """
-    Creates a key containing a composed config (or child config) of the configuration. The first time the
-    child config is required, it is created and stored in an attribute. This attribute is then used from that
-    point onwards.
-    Parameters
-    ----------
-    f - getter function returning a new instance of the child config (usually just the constructor).
-
-    Returns
-    -------
-    Decorated composed config getter function
-    """
-
-    def wrapped_f_getter(self: Config) -> TConfig:
-        attr_name = "_" + self._get_property_name_from_object(wrapped_f)
-        if not hasattr(self, attr_name):
-            setattr(self, attr_name, cls(provider=self._provider))
-        return typing.cast(TConfig, getattr(self, attr_name))
-
-    wrapped_f = property(wrapped_f_getter)
-    setattr(wrapped_f.fget, Config._composed_config_registration_string, True)
-
-    return typing.cast(TConfig, wrapped_f)
-
-
-def section(section_name: str) -> Callable[[Type[TConfig]], Type[TConfig]]:
-    def _section(cls: Type[TConfig]) -> Type[TConfig]:
-        class SectionConfig(cls):  # type: ignore
-            def __init__(self, *args, **kwargs):  # type: ignore
-                super().__init__(*args, section_name=section_name, **kwargs)
-
-        SectionConfig.__name__ = cls.__name__
-        SectionConfig.__qualname__ = cls.__qualname__
-
-        return SectionConfig
-
-    return _section
-
-
-class Config:
-    """
-    Base class for all configuration objects
-    """
-
-    _composed_config_registration_string = "__composed_config__"
-    _config_key_registration_string = "__config_key__"
-    _config_key_key_name_string = "__config_key_key_name__"
-    _config_key_section_name_string = "__config_key_section_name__"
-
-    def __init__(
-        self,
-        section_name: Optional[str] = None,
-        sources: Optional[List[ConfigSource]] = None,
-        provider: Optional[ConfigProvider] = None,
-    ):
-        if provider is None:
-            provider = ConfigProvider(sources=sources)
-        elif not isinstance(provider, ConfigProvider):
-            raise TypeError("provider must be a ConfigProvider object")
-        self._section_name = section_name
-        self._provider: ConfigProvider = provider
-
-    def __repr__(self) -> str:
-        key_names = self.get_registered_properties()
-        group_key_info = inspect.getmembers(
-            self.__class__,
-            predicate=lambda x: self.is_member_registered(x, Config._composed_config_registration_string),
-        )
-
-        joined_repr = ", ".join(
-            chain(
-                (f"{k}={getattr(self, k)!r}" for k in key_names),
-                (f"{k}={getattr(self, k)!r}" for k, _ in group_key_info),
-            )
-        )
-
-        return f"{self.__class__.__name__}({joined_repr})"
-
-    @property
-    def config_sources(self) -> List[ConfigSource]:
-        return self._provider.config_sources
-
-    @property
-    def provider(self) -> ConfigProvider:
-        return self._provider
-
-    def get_registered_properties(self) -> List[str]:
-        """
-        Gets a list of all properties which have been defined using the key function
-        Returns
-        -------
-        A list of strings giving the names of the registered properties/methods
-        """
-        all_properties = self._get_registered_properties_with_values()
-        return [f[0] for f in all_properties]
-
-    def _get_registered_properties_with_values(self) -> List[Tuple[str, Any]]:
-        return inspect.getmembers(
-            self.__class__, predicate=lambda x: self.is_member_registered(x, Config._config_key_registration_string)
-        )
-
-    def _resolve_section_name(self, key_section_name: Optional[str]) -> str:
-        if key_section_name is not None:
-            return key_section_name
-
-        if self._section_name is None:
-            raise ValueError("Section name was not specified by the key function or the section class decorator.")
-        return self._section_name
-
-    def _resolve_key_name(self, property_object: property) -> str:
-        key_key_name: str = getattr(property_object.fget, self._config_key_key_name_string)
-        if key_key_name is not None:
-            return key_key_name
-
-        return self._get_property_name_from_object(property_object)
-
-    def _get_property_name_from_object(self, property_object: property) -> str:
-        members = inspect.getmembers(self.__class__, lambda x: x is property_object)
-        assert len(members) == 1
-        return members[0][0].upper()
-
-    @staticmethod
-    def is_member_registered(member: Any, reg_string: str) -> bool:
-        if isinstance(member, property):
-            return typing.cast(bool, getattr(member.fget, reg_string, False))
-        else:
-            return False
-
-    def get_registered_composed_config(self) -> List["Config"]:
-        """
-        Gets a list of all composed configs or "sub configs",
-        that is configs which are registered with the group_key function.
-        This returns the sub-config instances themselves (not just references to the getter methods)
-        Returns
-        -------
-        A list of Config subclasses which have been registered
-        """
-
-        all_properties = inspect.getmembers(
-            self.__class__,
-            predicate=lambda x: self.is_member_registered(x, Config._composed_config_registration_string),
-        )
-        return [getattr(self, f[0]) if isinstance(f[1], property) else f[1](self) for f in all_properties]
-
-    def read(self) -> None:
-        """
-        Loops through all config properties generated with the key function and reads their values in.
-        It is useful to call this after adding the config sources for fail-fast behaviour, since an error will occur at
-        this point if any required config value is missing. It also means all config values are loaded into cache at
-        this point so future accesses will be reliable and fast.
-        Returns
-        -------
-        None
-        """
-        child_configs = self.get_registered_composed_config()
-        registered_properties = self.get_registered_properties()
-        for f in registered_properties:
-            getattr(self, f)
-
-        self._post_read(self.post_read_hook())
-
-        for c in child_configs:
-            c.read()
-
-    def post_read_hook(self) -> Dict[str, Any]:
-        """
-        This method can be overridden to modify config values after read() is called.
-        Returns
-        -------
-        A dict of key-value pairs containing new configuration values for key() items in this Config class
-        """
-        return dict()
-
-    def _post_read(self, updated_values: Dict[str, Any]) -> None:
-        registered_properties = set(self.get_registered_properties())
-
-        for k, v in updated_values.items():
-            if isinstance(v, dict):
-                group_property_object: property = getattr(self.__class__, k)
-                if not self.is_member_registered(group_property_object, self._composed_config_registration_string):
-                    raise KeyError(f"{k} is not a valid typed config group_key() of {self.__class__.__name__}")
-                child_config = getattr(self, k)
-                child_config._post_read(v)
-            else:
-                if k not in registered_properties:
-                    raise KeyError(f"{k} is not a valid attribute of {self.__class__.__name__}")
-
-                key_property_object: property = getattr(self.__class__, k)
-
-                section_name = self._resolve_section_name(
-                    getattr(key_property_object.fget, self._config_key_section_name_string)
-                )
-                key_name = self._resolve_key_name(key_property_object)
-                self._provider.add_to_cache(section_name, key_name, v)
-
-    def clear_cache(self) -> None:
-        """
-        Config values are cached the first time they are requested. This means that if, for example, config values are
-        coming from a database or API, the call does not need to be made again. This function clears the cache.
-        Returns
-        -------
-        None
-        """
-        self._provider.clear_cache()
-
-    def add_source(self, source: ConfigSource) -> None:
-        """
-        Adds a configuration source
-        Parameters
-        ----------
-        source: a subclass of ConfigSource which can provide string values for configuration parameters
-
-        Returns
-        -------
-        None
-        """
-        self._provider.add_source(source)
-
-    def replace_source(self, old_source: ConfigSource, new_source: ConfigSource) -> None:
-        """
-        Replaces a ConfigSource with a new one. This is useful for example if you modify a config file, so want
-        to swap a ConfigSource which reads from a file on initialisation for a new one.
-        This does not clear the cache. To access new values you also need to call clear_cache.
-
-        Parameters
-        ----------
-        old_source: The old config source to be replaced
-        new_source: The config source to replace it with
-
-        Returns
-        -------
-        None
-        """
-        self._provider.replace_source(old_source, new_source)
-
-    def set_sources(self, sources: List[ConfigSource]) -> None:
-        """
-        Completely replaces the set of ConfigSources with a new set.
-
-        This does not clear the cache. To access new values you also need to call clear_cache
-        Parameters
-        ----------
-        sources: List of ConfigSource subclasses to supply the configuration
-
-        Returns
-        -------
-        None
-        """
-        self._provider.set_sources(sources)
-
-    def get_key(self, section_name: str, key_name: str) -> Optional[str]:
-        """
-        Gets a string configuration key from available sources
-        Parameters
-        ----------
-        section_name: section name where the key resides
-        key_name: key name within the specified section
-
-        Returns
-        -------
-        value: the loaded config value as a string
-        """
-        return self._provider.get_key(section_name, key_name)
+import sys
+import typing
+from itertools import chain
+from typing import TypeVar, List, Optional, Callable, Type, Union, Tuple, Any, overload, Dict
+
+from typing import Literal
+from typedconfig.provider import ConfigProvider
+from typedconfig.source import ConfigSource
+import logging
+import inspect
+
+logger = logging.getLogger(__name__)
+
+TConfig = TypeVar("TConfig", bound="Config")
+T = TypeVar("T")
+U = TypeVar("U")
+V = TypeVar("V")
+
+"""
+required | cast | default | return_type
+True  | None/missing    | -       | str
+True  | NotNone | -       | T
+
+False | NotNone | None/missing | Optional[T]
+False | NotNone | NotNone | T
+False | None    | -       | Union[str, Optional[T]]
+"""
+
+
+@overload
+def key(
+    *,
+    section_name: Optional[str] = ...,
+    key_name: Optional[str] = ...,
+    required: Literal[False],
+    cast: Callable[[str], T],
+    default: T,
+) -> T: ...
+
+
+@overload
+def key(
+    *,
+    section_name: Optional[str] = ...,
+    key_name: Optional[str] = ...,
+    required: Literal[False],
+    cast: Callable[[str], T],
+    default: None = ...,
+) -> Optional[T]: ...
+
+
+@overload
+def key(
+    *,
+    section_name: Optional[str] = ...,
+    key_name: Optional[str] = ...,
+    required: Literal[False],
+    cast: None = ...,
+    default: Optional[T] = ...,
+) -> Union[str, Optional[T]]: ...
+
+
+@overload
+def key(
+    *,
+    section_name: Optional[str] = ...,
+    key_name: Optional[str] = ...,
+    required: Literal[True] = ...,
+    cast: Callable[[str], T],
+    default: Optional[T] = ...,
+) -> T: ...
+
+
+@overload
+def key(
+    *,
+    section_name: Optional[str] = ...,
+    key_name: Optional[str] = ...,
+    required: Literal[True] = ...,
+    cast: None = ...,
+    default: Optional[T] = ...,
+) -> str: ...
+
+
+def key(
+    *,
+    section_name: Optional[str] = None,
+    key_name: Optional[str] = None,
+    required: bool = True,
+    cast: Optional[Callable[[str], T]] = None,
+    default: Optional[T] = None,
+) -> Union[Optional[T], str]:
+    """
+    Provides a getter for a configuration key
+    Parameters
+    ----------
+    section_name: section name where the key resides. If not specified,
+        the @section decorator should be used on the Config class to specify it
+    key_name: key name within the specified section. If not specified,
+        the python key name will be capitalised and used
+    required: optional, default True. Whether the key is required or optional
+    cast: optional, default None (no cast). Function taking a string argument and returning the parsed value
+    default: optional, default None. If required is set to False, the value to use if the config value is not found
+    """
+
+    # In general, this should not store any state since the class property is shared across instances. However, the
+    # property name will be the same across all instances, so when this is looked up the first time it is ok to store
+    # it.
+    _mutable_state = {"key_name": key_name.upper() if key_name is not None else None}
+
+    def getter_method(self: Config) -> Union[Optional[T], str]:
+        """
+        Returns
+        -------
+        value: the parsed config value
+        """
+
+        resolved_section_name = self._resolve_section_name(section_name)
+
+        resolved_key_name = _mutable_state["key_name"]
+        if resolved_key_name is None:
+            resolved_key_name = self._resolve_key_name(getter)
+            _mutable_state["key_name"] = resolved_key_name
+
+        # If value is cached, just use the cached value
+        cached_value: Union[T, str] = self._provider.get_from_cache(resolved_section_name, resolved_key_name)
+        if cached_value is not None:
+            return cached_value
+
+        string_value = self._provider.get_key(resolved_section_name, resolved_key_name)
+        cast_value: Union[Optional[T], str] = None
+
+        # If we still haven't found a config value and this parameter is required,
+        # raise an exception, otherwise use the default
+        if string_value is None:
+            if required:
+                raise KeyError("Config parameter {0}.{1} not found".format(resolved_section_name, resolved_key_name))
+            else:
+                if default is not None:
+                    cast_value = default
+        else:
+            # If a casting function has been specified then cast to the required data type
+            if cast is not None:
+                cast_value = cast(string_value)
+            else:
+                cast_value = string_value
+
+        # Cache this for next time if still not none
+        if cast_value is not None:
+            self._provider.add_to_cache(resolved_section_name, resolved_key_name, cast_value)
+
+        return cast_value
+
+    getter = property(getter_method)
+    setattr(getter.fget, Config._config_key_registration_string, True)
+    setattr(getter.fget, Config._config_key_key_name_string, key_name.upper() if key_name is not None else None)
+    setattr(getter.fget, Config._config_key_section_name_string, section_name)
+    return typing.cast(Union[Optional[T], str], getter)
+
+
+def group_key(cls: Type[TConfig], *, group_section_name: Optional[str] = None, hierarchical: bool = False) -> TConfig:
+    """
+    Creates a key containing a composed config (or child config) of the configuration. The first time the
+    child config is required, it is created and stored in an attribute. This attribute is then used from that
+    point onwards.
+    Parameters
+    ----------
+    f - getter function returning a new instance of the child config (usually just the constructor).
+
+    Returns
+    -------
+    Decorated composed config getter function
+    """
+
+    def wrapped_f_getter(self: Config) -> TConfig:
+        attr_name = "_" + self._get_property_name_from_object(wrapped_f)
+        if not hasattr(self, attr_name):
+            setattr(self, attr_name, cls(provider=self._provider))
+        return typing.cast(TConfig, getattr(self, attr_name))
+
+    wrapped_f = property(wrapped_f_getter)
+    setattr(wrapped_f.fget, Config._composed_config_registration_string, True)
+
+    return typing.cast(TConfig, wrapped_f)
+
+
+def section(section_name: str) -> Callable[[Type[TConfig]], Type[TConfig]]:
+    def _section(cls: Type[TConfig]) -> Type[TConfig]:
+        class SectionConfig(cls):  # type: ignore
+            def __init__(self, *args, **kwargs):  # type: ignore
+                super().__init__(*args, section_name=section_name, **kwargs)
+
+        SectionConfig.__name__ = cls.__name__
+        SectionConfig.__qualname__ = cls.__qualname__
+
+        return SectionConfig
+
+    return _section
+
+
+class Config:
+    """
+    Base class for all configuration objects
+    """
+
+    _composed_config_registration_string = "__composed_config__"
+    _config_key_registration_string = "__config_key__"
+    _config_key_key_name_string = "__config_key_key_name__"
+    _config_key_section_name_string = "__config_key_section_name__"
+
+    def __init__(
+        self,
+        section_name: Optional[str] = None,
+        sources: Optional[List[ConfigSource]] = None,
+        provider: Optional[ConfigProvider] = None,
+    ):
+        if provider is None:
+            provider = ConfigProvider(sources=sources)
+        elif not isinstance(provider, ConfigProvider):
+            raise TypeError("provider must be a ConfigProvider object")
+        self._section_name = section_name
+        self._provider: ConfigProvider = provider
+
+    def __repr__(self) -> str:
+        key_names = self.get_registered_properties()
+        group_key_info = inspect.getmembers(
+            self.__class__,
+            predicate=lambda x: self.is_member_registered(x, Config._composed_config_registration_string),
+        )
+
+        joined_repr = ", ".join(
+            chain(
+                (f"{k}={getattr(self, k)!r}" for k in key_names),
+                (f"{k}={getattr(self, k)!r}" for k, _ in group_key_info),
+            )
+        )
+
+        return f"{self.__class__.__name__}({joined_repr})"
+
+    @property
+    def config_sources(self) -> List[ConfigSource]:
+        return self._provider.config_sources
+
+    @property
+    def provider(self) -> ConfigProvider:
+        return self._provider
+
+    def get_registered_properties(self) -> List[str]:
+        """
+        Gets a list of all properties which have been defined using the key function
+        Returns
+        -------
+        A list of strings giving the names of the registered properties/methods
+        """
+        all_properties = self._get_registered_properties_with_values()
+        return [f[0] for f in all_properties]
+
+    def _get_registered_properties_with_values(self) -> List[Tuple[str, Any]]:
+        return inspect.getmembers(
+            self.__class__, predicate=lambda x: self.is_member_registered(x, Config._config_key_registration_string)
+        )
+
+    def _resolve_section_name(self, key_section_name: Optional[str]) -> str:
+        if key_section_name is not None:
+            return key_section_name
+
+        if self._section_name is None:
+            raise ValueError("Section name was not specified by the key function or the section class decorator.")
+        return self._section_name
+
+    def _resolve_key_name(self, property_object: property) -> str:
+        key_key_name: str = getattr(property_object.fget, self._config_key_key_name_string)
+        if key_key_name is not None:
+            return key_key_name
+
+        return self._get_property_name_from_object(property_object)
+
+    def _get_property_name_from_object(self, property_object: property) -> str:
+        members = inspect.getmembers(self.__class__, lambda x: x is property_object)
+        assert len(members) == 1
+        return members[0][0].upper()
+
+    @staticmethod
+    def is_member_registered(member: Any, reg_string: str) -> bool:
+        if isinstance(member, property):
+            return typing.cast(bool, getattr(member.fget, reg_string, False))
+        else:
+            return False
+
+    def get_registered_composed_config(self) -> List["Config"]:
+        """
+        Gets a list of all composed configs or "sub configs",
+        that is configs which are registered with the group_key function.
+        This returns the sub-config instances themselves (not just references to the getter methods)
+        Returns
+        -------
+        A list of Config subclasses which have been registered
+        """
+
+        all_properties = inspect.getmembers(
+            self.__class__,
+            predicate=lambda x: self.is_member_registered(x, Config._composed_config_registration_string),
+        )
+        return [getattr(self, f[0]) if isinstance(f[1], property) else f[1](self) for f in all_properties]
+
+    def read(self) -> None:
+        """
+        Loops through all config properties generated with the key function and reads their values in.
+        It is useful to call this after adding the config sources for fail-fast behaviour, since an error will occur at
+        this point if any required config value is missing. It also means all config values are loaded into cache at
+        this point so future accesses will be reliable and fast.
+        Returns
+        -------
+        None
+        """
+        child_configs = self.get_registered_composed_config()
+        registered_properties = self.get_registered_properties()
+        for f in registered_properties:
+            getattr(self, f)
+
+        self._post_read(self.post_read_hook())
+
+        for c in child_configs:
+            c.read()
+
+    def post_read_hook(self) -> Dict[str, Any]:
+        """
+        This method can be overridden to modify config values after read() is called.
+        Returns
+        -------
+        A dict of key-value pairs containing new configuration values for key() items in this Config class
+        """
+        return dict()
+
+    def _post_read(self, updated_values: Dict[str, Any]) -> None:
+        registered_properties = set(self.get_registered_properties())
+
+        for k, v in updated_values.items():
+            if isinstance(v, dict):
+                group_property_object: property = getattr(self.__class__, k)
+                if not self.is_member_registered(group_property_object, self._composed_config_registration_string):
+                    raise KeyError(f"{k} is not a valid typed config group_key() of {self.__class__.__name__}")
+                child_config = getattr(self, k)
+                child_config._post_read(v)
+            else:
+                if k not in registered_properties:
+                    raise KeyError(f"{k} is not a valid attribute of {self.__class__.__name__}")
+
+                key_property_object: property = getattr(self.__class__, k)
+
+                section_name = self._resolve_section_name(
+                    getattr(key_property_object.fget, self._config_key_section_name_string)
+                )
+                key_name = self._resolve_key_name(key_property_object)
+                self._provider.add_to_cache(section_name, key_name, v)
+
+    def clear_cache(self) -> None:
+        """
+        Config values are cached the first time they are requested. This means that if, for example, config values are
+        coming from a database or API, the call does not need to be made again. This function clears the cache.
+        Returns
+        -------
+        None
+        """
+        self._provider.clear_cache()
+
+    def add_source(self, source: ConfigSource) -> None:
+        """
+        Adds a configuration source
+        Parameters
+        ----------
+        source: a subclass of ConfigSource which can provide string values for configuration parameters
+
+        Returns
+        -------
+        None
+        """
+        self._provider.add_source(source)
+
+    def replace_source(self, old_source: ConfigSource, new_source: ConfigSource) -> None:
+        """
+        Replaces a ConfigSource with a new one. This is useful for example if you modify a config file, so want
+        to swap a ConfigSource which reads from a file on initialisation for a new one.
+        This does not clear the cache. To access new values you also need to call clear_cache.
+
+        Parameters
+        ----------
+        old_source: The old config source to be replaced
+        new_source: The config source to replace it with
+
+        Returns
+        -------
+        None
+        """
+        self._provider.replace_source(old_source, new_source)
+
+    def set_sources(self, sources: List[ConfigSource]) -> None:
+        """
+        Completely replaces the set of ConfigSources with a new set.
+
+        This does not clear the cache. To access new values you also need to call clear_cache
+        Parameters
+        ----------
+        sources: List of ConfigSource subclasses to supply the configuration
+
+        Returns
+        -------
+        None
+        """
+        self._provider.set_sources(sources)
+
+    def get_key(self, section_name: str, key_name: str) -> Optional[str]:
+        """
+        Gets a string configuration key from available sources
+        Parameters
+        ----------
+        section_name: section name where the key resides
+        key_name: key name within the specified section
+
+        Returns
+        -------
+        value: the loaded config value as a string
+        """
+        return self._provider.get_key(section_name, key_name)
```

### Comparing `typed-config-1.5.0/typedconfig/provider.py` & `typed-config-2.0.3/typedconfig/provider.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import logging
-from typing import List, Optional, Dict, Any
-from typedconfig.source import ConfigSource
-
-logger = logging.getLogger(__name__)
-
-
-class ConfigProvider:
-    """
-    Configuration provider keeping the cache and sources that can be shared
-    across the configuration objects
-    """
-
-    def __init__(self, sources: Optional[List[ConfigSource]] = None):
-        self._cache: Dict[str, Dict[str, Any]] = {}
-        self._config_sources: List[ConfigSource] = []
-        if sources is not None:
-            for source in sources:
-                self.add_source(source)
-
-    def add_to_cache(self, section_name: str, key_name: str, value: Any) -> None:
-        if section_name not in self._cache:
-            self._cache[section_name] = {}
-        self._cache[section_name][key_name] = value
-
-    def get_from_cache(self, section_name: str, key_name: str) -> Any:
-        if section_name not in self._cache:
-            return None
-        return self._cache[section_name].get(key_name, None)
-
-    def clear_cache(self) -> None:
-        self._cache.clear()
-
-    @property
-    def config_sources(self) -> List[ConfigSource]:
-        return self._config_sources
-
-    def get_key(self, section_name: str, key_name: str) -> Optional[str]:
-        value = None
-
-        # Go through the config sources until we find one which supplies the requested value
-        for source in self._config_sources:
-            logger.debug(f"Looking for config value {section_name}/{key_name} in {source}")
-            value = source.get_config_value(section_name, key_name)
-            if value is not None:
-                logger.debug(f"Found config value {section_name}/{key_name} in {source}")
-                break
-
-        return value
-
-    def add_source(self, source: ConfigSource) -> None:
-        if not isinstance(source, ConfigSource):
-            raise TypeError("Sources must be subclasses of ConfigSource")
-        logger.debug(f"Adding config source of type {source.__class__.__name__} to {self.__class__.__name__}")
-        self._config_sources.append(source)
-
-    def set_sources(self, sources: List[ConfigSource]) -> None:
-        self._config_sources.clear()
-        for source in sources:
-            self.add_source(source)
-
-    def replace_source(self, old_source: ConfigSource, new_source: ConfigSource) -> None:
-        if not isinstance(new_source, ConfigSource):
-            raise TypeError("Sources must be subclasses of ConfigSource")
-        logger.debug(
-            f"Replacing config source of type {old_source.__class__.__name__} with {new_source.__class__.__name__}"
-        )
-        for i, source in enumerate(self.config_sources):
-            if source is old_source:
-                self.config_sources[i] = new_source
-                return
-
-        raise ValueError("ConfigProvider did not find the supplied old source to replace: %s", old_source)
+import logging
+from typing import List, Optional, Dict, Any
+from typedconfig.source import ConfigSource
+
+logger = logging.getLogger(__name__)
+
+
+class ConfigProvider:
+    """
+    Configuration provider keeping the cache and sources that can be shared
+    across the configuration objects
+    """
+
+    def __init__(self, sources: Optional[List[ConfigSource]] = None):
+        self._cache: Dict[str, Dict[str, Any]] = {}
+        self._config_sources: List[ConfigSource] = []
+        if sources is not None:
+            for source in sources:
+                self.add_source(source)
+
+    def add_to_cache(self, section_name: str, key_name: str, value: Any) -> None:
+        if section_name not in self._cache:
+            self._cache[section_name] = {}
+        self._cache[section_name][key_name] = value
+
+    def get_from_cache(self, section_name: str, key_name: str) -> Any:
+        if section_name not in self._cache:
+            return None
+        return self._cache[section_name].get(key_name, None)
+
+    def clear_cache(self) -> None:
+        self._cache.clear()
+
+    @property
+    def config_sources(self) -> List[ConfigSource]:
+        return self._config_sources
+
+    def get_key(self, section_name: str, key_name: str) -> Optional[str]:
+        value = None
+
+        # Go through the config sources until we find one which supplies the requested value
+        for source in self._config_sources:
+            logger.debug(f"Looking for config value {section_name}/{key_name} in {source}")
+            value = source.get_config_value(section_name, key_name)
+            if value is not None:
+                logger.debug(f"Found config value {section_name}/{key_name} in {source}")
+                break
+
+        return value
+
+    def add_source(self, source: ConfigSource) -> None:
+        if not isinstance(source, ConfigSource):
+            raise TypeError("Sources must be subclasses of ConfigSource")
+        logger.debug(f"Adding config source of type {source.__class__.__name__} to {self.__class__.__name__}")
+        self._config_sources.append(source)
+
+    def set_sources(self, sources: List[ConfigSource]) -> None:
+        self._config_sources.clear()
+        for source in sources:
+            self.add_source(source)
+
+    def replace_source(self, old_source: ConfigSource, new_source: ConfigSource) -> None:
+        if not isinstance(new_source, ConfigSource):
+            raise TypeError("Sources must be subclasses of ConfigSource")
+        logger.debug(
+            f"Replacing config source of type {old_source.__class__.__name__} with {new_source.__class__.__name__}"
+        )
+        for i, source in enumerate(self.config_sources):
+            if source is old_source:
+                self.config_sources[i] = new_source
+                return
+
+        raise ValueError("ConfigProvider did not find the supplied old source to replace: %s", old_source)
```

