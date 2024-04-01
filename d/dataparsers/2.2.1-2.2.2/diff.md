# Comparing `tmp/dataparsers-2.2.1.tar.gz` & `tmp/dataparsers-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataparsers-2.2.1.tar", max compression
+gzip compressed data, was "dataparsers-2.2.2.tar", max compression
```

## Comparing `dataparsers-2.2.1.tar` & `dataparsers-2.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      647 2024-03-21 13:57:45.730929 dataparsers-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     5431 2024-03-21 13:51:49.370881 dataparsers-2.2.1/README.md
--rw-r--r--   0        0        0    30191 2024-03-21 13:55:01.307034 dataparsers-2.2.1/src/dataparsers/__init__.md
--rw-r--r--   0        0        0       28 2024-02-26 03:54:48.282640 dataparsers-2.2.1/src/dataparsers/__init__.py
--rw-r--r--   0        0        0   114510 2024-03-21 13:55:01.308049 dataparsers-2.2.1/src/dataparsers/__init__.pyi
--rw-r--r--   0        0        0    13172 2024-03-21 11:46:09.650416 dataparsers-2.2.1/src/dataparsers/dataparsers.py
--rw-r--r--   0        0        0     5961 1970-01-01 00:00:00.000000 dataparsers-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      647 2024-04-01 22:05:13.741598 dataparsers-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5433 2024-04-01 22:04:54.771026 dataparsers-2.2.2/README.md
+-rw-r--r--   0        0        0    30280 2024-03-28 14:00:35.753753 dataparsers-2.2.2/src/dataparsers/__init__.md
+-rw-r--r--   0        0        0       28 2024-02-26 03:54:48.282640 dataparsers-2.2.2/src/dataparsers/__init__.py
+-rw-r--r--   0        0        0   114599 2024-04-01 22:04:54.688070 dataparsers-2.2.2/src/dataparsers/__init__.pyi
+-rw-r--r--   0        0        0    13172 2024-03-21 11:46:09.650416 dataparsers-2.2.2/src/dataparsers/dataparsers.py
+-rw-r--r--   0        0        0     5963 1970-01-01 00:00:00.000000 dataparsers-2.2.2/PKG-INFO
```

### Comparing `dataparsers-2.2.1/pyproject.toml` & `dataparsers-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataparsers"
-version = "2.2.1"
+version = "2.2.2"
 description = "A wrapper around argparse to get command line argument parsers from dataclasses"
 authors = ["Diogo Rossi <rossi.diogo@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Diogo-Rossi/dataparsers.git"
 documentation = "https://dataparsers.readthedocs.io/en/latest/index.html#"
```

### Comparing `dataparsers-2.2.1/README.md` & `dataparsers-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,18 +121,18 @@
 - More control over the interface display
 - More control over the argument flag `--` creation
 - More similarity with `argparse` module
 - More simplicity
 
 The simplicity is mentioned because it is just a simple module
 [`dataparsers.py`](https://github.com/Diogo-Rossi/dataparsers/blob/main/src/dataparsers/dataparsers.py)
-that doesn't have any additional dependency (it is pure Python) which can be
+that doesn't have any additional dependencies (it is pure Python) which can be
 downloaded directly and placed in your CLI scripts folder to import from.
 
-In deed, the module consists of a 315 lines
+In deed, the module consists of a 320 lines
 [IPython code cell region](https://docs.spyder-ide.org/current/panes/editor.html#code-cells)
 (i.e., starts and ends with a `#%%` line comment block), that can also be placed
 on top of your "single file" CLI script to directly distribute. The used names
 are just the few
 [provided functions](https://dataparsers.readthedocs.io/en/latest/2_available_functions.html),
 the _stdlib_ imports, `Class` (a `TypeVar`) and `SubParser` (a frozen `dataclass`).
```

### Comparing `dataparsers-2.2.1/src/dataparsers/__init__.md` & `dataparsers-2.2.2/src/dataparsers/__init__.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,29 @@
     Args(foo='newtest', bar=32)
 
 To create a argument parser and not immediately parse the arguments (i.e., save it for later), use the `make_parser()`
 function::
 
     >>> parser = make_parser(Args)
 
-Both functions `parse()` and `make_parser()` accepts a `parser=...` keyword argument to modify an existing parser::
+It is also possible to parse only a few of the command-line arguments, passing the remaining arguments on to another
+script or program, using the `parse_known()` function for this. It works much like `parse()` except that it does not
+produce an error when extra arguments are present. Instead, it returns a two item tuple containing the populated class
+and the list of remaining argument strings::
+
+    >>> @dataclass
+    ... class Args:
+    ...     foo: bool
+    ...     bar: str
+    ...
+    >>> parse_known(Args, ['--foo', '--badger', 'BAR', 'spam'])
+    (Args(foo=True, bar='BAR'), ['--badger', 'spam'])
+
+All functions `parse()`,  `make_parser()` and `parse_known()` accepts a `parser=...` keyword argument to modify an
+existing parser::
 
     >>> from argparse import ArgumentParser
     >>> prev_parser = ArgumentParser(description="Existing parser")
     >>> parse(Args, ["-h"], parser=prev_parser)
     usage: [-h] [--bar BAR] foo
 
     Existing parser
@@ -66,28 +80,14 @@
     positional arguments:
       foo
 
     options:
       -h, --help  show this help message and exit
       --bar BAR
 
-It is also possible to parse only a few of the command-line arguments, passing the remaining arguments on to another
-script or program, using the `parse_known()` function for this. It works much like `parse()` except that it does not
-produce an error when extra arguments are present. Instead, it returns a two item tuple containing the populated class
-and the list of remaining argument strings::
-
-    >>> @dataclass
-    ... class Args:
-    ...     foo: bool
-    ...     bar: str
-    ...
-    >>> parse_known(Args, ['--foo', '--badger', 'BAR', 'spam'])
-    (Args(foo=True, bar='BAR'), ['--badger', 'spam'])
-
-
 ## Argument specification
 
 To specify detailed information about each argument, call the `arg()` function on the `dataclass` fields::
 
     # prog.py
     from dataclasses import dataclass
     from dataparsers import parse, arg
@@ -112,19 +112,19 @@
       --bar BAR   bar help
 
 In general, the `arg()` function accepts all parameters that are used in the original `add_argument()` method (with few
 exceptions) and some additional parameters. The `default` keyword argument used above makes the argument optional (i.e.,
 passed with flags like `--bar`) except in some specific situations.
 
 One parameter of `add_argument()` that are not possible to pass to `arg()` is the `dest` keyword argument. That's
-because the name of the class attribute is determined by the `dataclass` field name. So, it is unnecessary to pass the
-`dest` parameter, since it doesn't makes sense in this situation.
+because the name of the class attribute is determined by the `dataclass` field name. So, it is not allowed to pass the
+`dest` parameter.
 
-The parameter `type` is another `add_argument()` parameter that are inferred from the `dataclass` field when not
-present.
+The parameter `type` is one of the `add_argument()` parameters that is inferred from the `dataclass` field properties
+when not present.
 
 ### Aliases
 
 The first parameter of the the original `add_argument()` method is `name_or_flags`, which is a series of flags, or a
 simple argument name. This parameter can be passed to `arg()` function to define aliases for optional arguments::
 
     @dataclass
@@ -197,17 +197,17 @@
     options:
       -h, --help  show this help message and exit
       -b BAR      bar help
 
 #### Booleans
 
 Booleans attributes are always considered as flag arguments, using the `"store_true"` or `"store_false"` values for the
-`action` parameter of the original `add_argument()` method. If the boolean `dataclass` field is created with no default
-value, the flag is still automatically created and the default value for the parameter will be `False` (it's defaults
-can be modified by the keyword argument `default_bool` of the `dataparser()` decorator - see "Default for booleans")::
+`action` parameter of the original `add_argument()` method. If the boolean field is created with no default value, the
+flag is still automatically created and the default value of the parameter is set to `False` (this default value can be
+modified by the keyword argument `default_bool` of the `dataparser()` decorator - see "Default for booleans")::
 
     >>> @dataclass
     ... class Args:
     ...     bar: bool
     ...
     >>> make_parser(Args).print_help()
     usage: [-h] [--bar]
@@ -430,33 +430,34 @@
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
     AttributeError: 'Args' object has no attribute 'my_first_group'
 
 ### Parser-level defaults
 
 Most of the time, the attributes of the object returned by `parse()` will be fully determined by inspecting the
-command-line arguments. However, there is a original `set_defaults()` method that allows some additional attributes to
-be determined without any inspection of the command line to be added. This functionality can be reproduced with the
-`default()` function::
+command-line arguments. However, there is the original `argparse`'s `set_defaults()` method that allows some additional
+attributes to be determined without any inspection of the command line to be added. This functionality can be reproduced
+with the `default()` function::
 
     >>> from dataparsers import parse, default
     >>> @dataclass
     ... class Args:
     ...     foo: int
     ...     bar: int = default(42)
     ...     baz: str = default("badger")
     ...
     >>> parse(Args, ["736"])
     Args(foo=736, bar=42, baz='badger')
 
-Parser-level defaults are the original recommended useful way to work with multiple parsers. See the `subparser()`
-method for examples.
+Parser-level defaults are the original
+[recommended useful way to work with multiple sub-parsers](https://github.com/python/cpython/blob/main/Doc/library/argparse.rst#L1901-L1904).
+See the `subparser()` method in section "Subparsers" for examples.
 
 One obvious difference of using this `default()` function in place of the original `set_defaults()` method is that this
-function must be used for each separated argument.
+function must be used for each argument separated.
 
 ## Parser specifications
 
 To specify detailed options to the created `ArgumentParser` object, use the `dataparser()` decorator::
 
     >>> from dataparsers import dataparser, make_parser
     >>> @dataparser(prog='MyProgram', description='A foo that bars')
@@ -594,14 +595,46 @@
     ...     baz: str = arg(make_flag=True, choices="XYZ", help="baz help", subparser=b)
     ...
     >>> parse(Args, ["a", "12"])
     Args(foo=False, bar=12, baz=None)
     >>> parse(Args, ["--foo", "b", "--baz", "Z"])
     Args(foo=True, bar=None, baz='Z')
 
+As in the original module, when a help message is requested from a subparser, only the help for that particular parser
+will be printed. The help message will not include parent parser or sibling parser messages. A help message for each
+subparser command, however, can be given by supplying the `help=...` argument to `subparser()` as above::
+
+    >>> parse(Args, ["--help"])
+    usage: PROG [-h] [--foo] {a,b} ...
+    
+    positional arguments:
+      {a,b}
+        a         a help
+        b         b help
+    
+    options:
+      -h, --help  show this help message and exit
+      --foo       foo help
+
+    >>> parse(Args, ["a", "--help"])
+    usage: PROG a [-h] bar
+
+    positional arguments:
+      bar         bar help
+
+    options:
+      -h, --help  show this help message and exit
+
+    >>> parse(Args, ["b", "--help"])
+    usage: PROG b [-h] [--baz {X,Y,Z}]
+
+    options:
+      -h, --help     show this help message and exit
+      --baz {X,Y,Z}  baz help
+
 The `ClassVar` defined with the function `subparser()` remains as a read-only class variable at run time (which is an
 instance of type `SubParser`: a frozen `dataclass` with some fields)::
 
     >>> args = parse(Args) 
     >>> args.a
     SubParser(defaults=None, kwargs=mappingproxy({'help': 'a help'}))
     >>> args.a.defaults="test"
@@ -624,46 +657,14 @@
     ...     ...
     ...     a: ClassVar = subparser(help="a help")
     ...     bar: int = arg(help="bar help", subparser=a)
     ...     ...
     ...     b: ClassVar = subparser(help="b help")
     ...     baz: str = arg(make_flag=True, choices="XYZ", help="baz help", subparser=b)
 
-As in the original module, when a help message is requested from a subparser, only the help for that particular parser
-will be printed. The help message will not include parent parser or sibling parser messages. A help message for each
-subparser command, however, can be given by supplying the `help=...` argument to `subparser()` as above::
-
-    >>> parse(Args, ["--help"])
-    usage: PROG [-h] [--foo] {a,b} ...
-
-    positional arguments:
-      {a,b}       sub-command help
-        a         a help
-        b         b help
-
-    options:
-      -h, --help  show this help message and exit
-      --foo       foo help
-
-    >>> parse(Args, ["a", "--help"])
-    usage: PROG a [-h] bar
-
-    positional arguments:
-      bar         bar help
-
-    options:
-      -h, --help  show this help message and exit
-
-    >>> parse(Args, ["b", "--help"])
-    usage: PROG b [-h] [--baz {X,Y,Z}]
-
-    options:
-      -h, --help     show this help message and exit
-      --baz {X,Y,Z}  baz help
-
 Some possible keyword arguments highlighted in the original `add_subparsers()` method are `title=...` and
 `description=...`. When either is present, the subparser's commands will appear in their own group in the help output::
 
     >>> @dataclass
     ... class Args:
     ...     subparsers_group: str = subparsers(
     ...         title="subcommands",
```

### Comparing `dataparsers-2.2.1/src/dataparsers/__init__.pyi` & `dataparsers-2.2.2/src/dataparsers/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,29 @@
     Args(foo='newtest', bar=32)
 
 To create a argument parser and not immediately parse the arguments (i.e., save it for later), use the `make_parser()`
 function::
 
     >>> parser = make_parser(Args)
 
-Both functions `parse()` and `make_parser()` accepts a `parser=...` keyword argument to modify an existing parser::
+It is also possible to parse only a few of the command-line arguments, passing the remaining arguments on to another
+script or program, using the `parse_known()` function for this. It works much like `parse()` except that it does not
+produce an error when extra arguments are present. Instead, it returns a two item tuple containing the populated class
+and the list of remaining argument strings::
+
+    >>> @dataclass
+    ... class Args:
+    ...     foo: bool
+    ...     bar: str
+    ...
+    >>> parse_known(Args, ['--foo', '--badger', 'BAR', 'spam'])
+    (Args(foo=True, bar='BAR'), ['--badger', 'spam'])
+
+All functions `parse()`,  `make_parser()` and `parse_known()` accepts a `parser=...` keyword argument to modify an
+existing parser::
 
     >>> from argparse import ArgumentParser
     >>> prev_parser = ArgumentParser(description="Existing parser")
     >>> parse(Args, ["-h"], parser=prev_parser)
     usage: [-h] [--bar BAR] foo
 
     Existing parser
@@ -66,28 +80,14 @@
     positional arguments:
       foo
 
     options:
       -h, --help  show this help message and exit
       --bar BAR
 
-It is also possible to parse only a few of the command-line arguments, passing the remaining arguments on to another
-script or program, using the `parse_known()` function for this. It works much like `parse()` except that it does not
-produce an error when extra arguments are present. Instead, it returns a two item tuple containing the populated class
-and the list of remaining argument strings::
-
-    >>> @dataclass
-    ... class Args:
-    ...     foo: bool
-    ...     bar: str
-    ...
-    >>> parse_known(Args, ['--foo', '--badger', 'BAR', 'spam'])
-    (Args(foo=True, bar='BAR'), ['--badger', 'spam'])
-
-
 ## Argument specification
 
 To specify detailed information about each argument, call the `arg()` function on the `dataclass` fields::
 
     # prog.py
     from dataclasses import dataclass
     from dataparsers import parse, arg
@@ -112,19 +112,19 @@
       --bar BAR   bar help
 
 In general, the `arg()` function accepts all parameters that are used in the original `add_argument()` method (with few
 exceptions) and some additional parameters. The `default` keyword argument used above makes the argument optional (i.e.,
 passed with flags like `--bar`) except in some specific situations.
 
 One parameter of `add_argument()` that are not possible to pass to `arg()` is the `dest` keyword argument. That's
-because the name of the class attribute is determined by the `dataclass` field name. So, it is unnecessary to pass the
-`dest` parameter, since it doesn't makes sense in this situation.
+because the name of the class attribute is determined by the `dataclass` field name. So, it is not allowed to pass the
+`dest` parameter.
 
-The parameter `type` is another `add_argument()` parameter that are inferred from the `dataclass` field when not
-present.
+The parameter `type` is one of the `add_argument()` parameters that is inferred from the `dataclass` field properties
+when not present.
 
 ### Aliases
 
 The first parameter of the the original `add_argument()` method is `name_or_flags`, which is a series of flags, or a
 simple argument name. This parameter can be passed to `arg()` function to define aliases for optional arguments::
 
     @dataclass
@@ -197,17 +197,17 @@
     options:
       -h, --help  show this help message and exit
       -b BAR      bar help
 
 #### Booleans
 
 Booleans attributes are always considered as flag arguments, using the `"store_true"` or `"store_false"` values for the
-`action` parameter of the original `add_argument()` method. If the boolean `dataclass` field is created with no default
-value, the flag is still automatically created and the default value for the parameter will be `False` (it's defaults
-can be modified by the keyword argument `default_bool` of the `dataparser()` decorator - see "Default for booleans")::
+`action` parameter of the original `add_argument()` method. If the boolean field is created with no default value, the
+flag is still automatically created and the default value of the parameter is set to `False` (this default value can be
+modified by the keyword argument `default_bool` of the `dataparser()` decorator - see "Default for booleans")::
 
     >>> @dataclass
     ... class Args:
     ...     bar: bool
     ...
     >>> make_parser(Args).print_help()
     usage: [-h] [--bar]
@@ -430,33 +430,34 @@
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
     AttributeError: 'Args' object has no attribute 'my_first_group'
 
 ### Parser-level defaults
 
 Most of the time, the attributes of the object returned by `parse()` will be fully determined by inspecting the
-command-line arguments. However, there is a original `set_defaults()` method that allows some additional attributes to
-be determined without any inspection of the command line to be added. This functionality can be reproduced with the
-`default()` function::
+command-line arguments. However, there is the original `argparse`'s `set_defaults()` method that allows some additional
+attributes to be determined without any inspection of the command line to be added. This functionality can be reproduced
+with the `default()` function::
 
     >>> from dataparsers import parse, default
     >>> @dataclass
     ... class Args:
     ...     foo: int
     ...     bar: int = default(42)
     ...     baz: str = default("badger")
     ...
     >>> parse(Args, ["736"])
     Args(foo=736, bar=42, baz='badger')
 
-Parser-level defaults are the original recommended useful way to work with multiple parsers. See the `subparser()`
-method for examples.
+Parser-level defaults are the original
+[recommended useful way to work with multiple sub-parsers](https://github.com/python/cpython/blob/main/Doc/library/argparse.rst#L1901-L1904).
+See the `subparser()` method in section "Subparsers" for examples.
 
 One obvious difference of using this `default()` function in place of the original `set_defaults()` method is that this
-function must be used for each separated argument.
+function must be used for each argument separated.
 
 ## Parser specifications
 
 To specify detailed options to the created `ArgumentParser` object, use the `dataparser()` decorator::
 
     >>> from dataparsers import dataparser, make_parser
     >>> @dataparser(prog='MyProgram', description='A foo that bars')
@@ -594,14 +595,46 @@
     ...     baz: str = arg(make_flag=True, choices="XYZ", help="baz help", subparser=b)
     ...
     >>> parse(Args, ["a", "12"])
     Args(foo=False, bar=12, baz=None)
     >>> parse(Args, ["--foo", "b", "--baz", "Z"])
     Args(foo=True, bar=None, baz='Z')
 
+As in the original module, when a help message is requested from a subparser, only the help for that particular parser
+will be printed. The help message will not include parent parser or sibling parser messages. A help message for each
+subparser command, however, can be given by supplying the `help=...` argument to `subparser()` as above::
+
+    >>> parse(Args, ["--help"])
+    usage: PROG [-h] [--foo] {a,b} ...
+    
+    positional arguments:
+      {a,b}
+        a         a help
+        b         b help
+    
+    options:
+      -h, --help  show this help message and exit
+      --foo       foo help
+
+    >>> parse(Args, ["a", "--help"])
+    usage: PROG a [-h] bar
+
+    positional arguments:
+      bar         bar help
+
+    options:
+      -h, --help  show this help message and exit
+
+    >>> parse(Args, ["b", "--help"])
+    usage: PROG b [-h] [--baz {X,Y,Z}]
+
+    options:
+      -h, --help     show this help message and exit
+      --baz {X,Y,Z}  baz help
+
 The `ClassVar` defined with the function `subparser()` remains as a read-only class variable at run time (which is an
 instance of type `SubParser`: a frozen `dataclass` with some fields)::
 
     >>> args = parse(Args) 
     >>> args.a
     SubParser(defaults=None, kwargs=mappingproxy({'help': 'a help'}))
     >>> args.a.defaults="test"
@@ -624,46 +657,14 @@
     ...     ...
     ...     a: ClassVar = subparser(help="a help")
     ...     bar: int = arg(help="bar help", subparser=a)
     ...     ...
     ...     b: ClassVar = subparser(help="b help")
     ...     baz: str = arg(make_flag=True, choices="XYZ", help="baz help", subparser=b)
 
-As in the original module, when a help message is requested from a subparser, only the help for that particular parser
-will be printed. The help message will not include parent parser or sibling parser messages. A help message for each
-subparser command, however, can be given by supplying the `help=...` argument to `subparser()` as above::
-
-    >>> parse(Args, ["--help"])
-    usage: PROG [-h] [--foo] {a,b} ...
-
-    positional arguments:
-      {a,b}       sub-command help
-        a         a help
-        b         b help
-
-    options:
-      -h, --help  show this help message and exit
-      --foo       foo help
-
-    >>> parse(Args, ["a", "--help"])
-    usage: PROG a [-h] bar
-
-    positional arguments:
-      bar         bar help
-
-    options:
-      -h, --help  show this help message and exit
-
-    >>> parse(Args, ["b", "--help"])
-    usage: PROG b [-h] [--baz {X,Y,Z}]
-
-    options:
-      -h, --help     show this help message and exit
-      --baz {X,Y,Z}  baz help
-
 Some possible keyword arguments highlighted in the original `add_subparsers()` method are `title=...` and
 `description=...`. When either is present, the subparser's commands will appear in their own group in the help output::
 
     >>> @dataclass
     ... class Args:
     ...     subparsers_group: str = subparsers(
     ...         title="subcommands",
```

### Comparing `dataparsers-2.2.1/src/dataparsers/dataparsers.py` & `dataparsers-2.2.2/src/dataparsers/dataparsers.py`

 * *Files identical despite different names*

### Comparing `dataparsers-2.2.1/PKG-INFO` & `dataparsers-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataparsers
-Version: 2.2.1
+Version: 2.2.2
 Summary: A wrapper around argparse to get command line argument parsers from dataclasses
 Home-page: https://github.com/Diogo-Rossi/dataparsers.git
 Author: Diogo Rossi
 Author-email: rossi.diogo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -137,18 +137,18 @@
 - More control over the interface display
 - More control over the argument flag `--` creation
 - More similarity with `argparse` module
 - More simplicity
 
 The simplicity is mentioned because it is just a simple module
 [`dataparsers.py`](https://github.com/Diogo-Rossi/dataparsers/blob/main/src/dataparsers/dataparsers.py)
-that doesn't have any additional dependency (it is pure Python) which can be
+that doesn't have any additional dependencies (it is pure Python) which can be
 downloaded directly and placed in your CLI scripts folder to import from.
 
-In deed, the module consists of a 315 lines
+In deed, the module consists of a 320 lines
 [IPython code cell region](https://docs.spyder-ide.org/current/panes/editor.html#code-cells)
 (i.e., starts and ends with a `#%%` line comment block), that can also be placed
 on top of your "single file" CLI script to directly distribute. The used names
 are just the few
 [provided functions](https://dataparsers.readthedocs.io/en/latest/2_available_functions.html),
 the _stdlib_ imports, `Class` (a `TypeVar`) and `SubParser` (a frozen `dataclass`).
```

