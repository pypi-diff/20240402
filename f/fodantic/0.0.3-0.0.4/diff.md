# Comparing `tmp/fodantic-0.0.3.tar.gz` & `tmp/fodantic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fodantic-0.0.3.tar", last modified: Sun Mar 31 05:33:18 2024, max compression
+gzip compressed data, was "fodantic-0.0.4.tar", last modified: Tue Apr  2 01:24:29 2024, max compression
```

## Comparing `fodantic-0.0.3.tar` & `fodantic-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:33:18.844077 fodantic-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-31 05:33:10.000000 fodantic-0.0.3/MIT-LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-03-31 05:33:18.844077 fodantic-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-31 05:33:10.000000 fodantic-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-31 05:33:10.000000 fodantic-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 05:33:18.844077 fodantic-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:33:18.840077 fodantic-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:33:18.840077 fodantic-0.0.3/src/fodantic/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-31 05:33:10.000000 fodantic-0.0.3/src/fodantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-03-31 05:33:10.000000 fodantic-0.0.3/src/fodantic/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-03-31 05:33:10.000000 fodantic-0.0.3/src/fodantic/form_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-31 05:33:10.000000 fodantic-0.0.3/src/fodantic/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:33:18.844077 fodantic-0.0.3/src/fodantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-03-31 05:33:18.000000 fodantic-0.0.3/src/fodantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-31 05:33:18.000000 fodantic-0.0.3/src/fodantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 05:33:18.000000 fodantic-0.0.3/src/fodantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-31 05:33:18.000000 fodantic-0.0.3/src/fodantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 05:33:18.000000 fodantic-0.0.3/src/fodantic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.524685 fodantic-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 01:24:21.000000 fodantic-0.0.4/MIT-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-02 01:24:29.524685 fodantic-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-02 01:24:21.000000 fodantic-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-02 01:24:21.000000 fodantic-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:24:29.524685 fodantic-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.520684 fodantic-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.520684 fodantic-0.0.4/src/fodantic/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/form_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-02 01:24:21.000000 fodantic-0.0.4/src/fodantic/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:24:29.524685 fodantic-0.0.4/src/fodantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 01:24:29.000000 fodantic-0.0.4/src/fodantic.egg-info/top_level.txt
```

### Comparing `fodantic-0.0.3/MIT-LICENSE` & `fodantic-0.0.4/MIT-LICENSE`

 * *Files identical despite different names*

### Comparing `fodantic-0.0.3/PKG-INFO` & `fodantic-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fodantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydantic-based HTTP forms
 Author-email: Juan-Pablo Scaletti <juanpablo@jpscaletti.com>
 License: Copyright (c) Juan-Pablo Scaletti
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -63,22 +63,27 @@
 @formable
 class UserModel(BaseModel):
     name: str
     friends: list[int]
     active: bool = True
 
 request_data = Multidict(('name', 'John Doe'), ('friends', '2'), ('friends', '3')}
-form = UserModel.as_form(request_data, obj=None)
+
+# The magic
+form = UserModel.as_form(request_data, object=None)
 
 print(form)
 #> UserModel.as_form(name='John Doe', friends=[2, 3], active=False)
 print(form.fields["name"].value)
 #> John Doe
 print(form.fields["name"].error)
-#>
+#> None
+print(form.save())  # Can also update the `object` passed as an argument
+#> {'name': 'John Doe', 'friends': [2, 3], 'active': False}
+
 ```
 
 
 ## Installation
 
   pip install fodantic
```

### Comparing `fodantic-0.0.3/README.md` & `fodantic-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -18,22 +18,27 @@
 @formable
 class UserModel(BaseModel):
     name: str
     friends: list[int]
     active: bool = True
 
 request_data = Multidict(('name', 'John Doe'), ('friends', '2'), ('friends', '3')}
-form = UserModel.as_form(request_data, obj=None)
+
+# The magic
+form = UserModel.as_form(request_data, object=None)
 
 print(form)
 #> UserModel.as_form(name='John Doe', friends=[2, 3], active=False)
 print(form.fields["name"].value)
 #> John Doe
 print(form.fields["name"].error)
-#>
+#> None
+print(form.save())  # Can also update the `object` passed as an argument
+#> {'name': 'John Doe', 'friends': [2, 3], 'active': False}
+
 ```
 
 
 ## Installation
 
   pip install fodantic
```

### Comparing `fodantic-0.0.3/pyproject.toml` & `fodantic-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 
 
 [project]
 name = "fodantic"
-version = "0.0.3"
+version = "0.0.4"
 description = "Pydantic-based HTTP forms"
 authors = [
   {name = "Juan-Pablo Scaletti", email = "juanpablo@jpscaletti.com"},
 ]
 license = { "file" = "MIT-LICENSE" }
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `fodantic-0.0.3/src/fodantic/form.py` & `fodantic-0.0.4/src/fodantic/form.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,50 +5,50 @@
 
 import typing as t
 
 from pydantic import BaseModel, ValidationError
 from pydantic_core import ErrorDetails
 
 from .form_field import FormField
-from .wrapper import DataWrapper
+from .wrappers import DataWrapper, ObjectWrapper
 
 
 __all__ = ["formable", "Form"]
 
 
 class Form:
     fields: "dict[str, FormField]"
     prefix: str = ""
     is_valid: bool = False
     is_empty: bool = True
     errors: list[ErrorDetails]
 
-    obj: t.Any = None
+    wobject: t.Any = None
     model: BaseModel | None = None
 
     def __init__(
         self,
         reqdata: t.Any = None,
         *,
         model_cls: t.Type[BaseModel],
-        obj: t.Any = None,
+        object: t.Any = None,
         prefix: str = "",
         orm_cls: t.Any = None,
     ):
         """
         A form handler that integrates pydantic models for data validation and can
         interact with ORM models.
 
         ## Arguments:
 
         - reqdata:
             Optional request data used for form submission.
         - model_cls:
             The pydantic model class for data validation.
-        - obj:
+        - object:
             Optional ORM model instance to fill the form and be updated when saving.
         - prefix:
             An optional prefix to prepend to field names (separated with a dot).
             Defaults to an empty string.
         - orm_cls:
             The ORM model class for database interaction. If `None`, the `Form.save()`
             returns a dict when the form is valid.
@@ -124,99 +124,117 @@
         self.prefix = f"{prefix}." if prefix else ""
         self.errors = []
         self.fields = {
             name: FormField(name=name, info=info, form=self)
             for name, info in self.model_cls.model_fields.items()
         }
 
-        if reqdata is None and obj is None:
+        self.is_empty = reqdata is None and object is None
+        if self.is_empty:
             return
 
-        self.is_empty = False
-        reqdata = DataWrapper(reqdata) if reqdata is not None else None
-        if obj is not None:
-            self.obj = obj = DataWrapper(obj)
+        wreqdata = DataWrapper(reqdata)
+        wobject = ObjectWrapper(object)
+
+        if object is not None:
+            self.wobject = wobject
 
         data: dict[str, t.Any] = {}
 
         for field in self.fields.values():
             model_name = field.model_name
             value: t.Any = None
-            if reqdata:
-                value = field.extract_value(reqdata)
-            if value is None and obj:
-                value = obj.get(model_name)
-            if value is None:
-                value = (
-                    field.default_factory() if field.default_factory else field.default
-                )
-            data[model_name] = value
+
+            value = field.extract_value(wreqdata)
+            if object and (value is None):
+                value = wobject.get(model_name)
+
+            if value is not None:
+                data[model_name] = value
 
         for model_name, value in data.items():
-            self.fields[model_name].value = value
+            self.fields[model_name].set_value(value)
+
+        if reqdata is not None:
+            self.validate(data)
 
+    def validate(self, data: dict[str, t.Any] | None = None):
+        if data is None:
+            data = {
+                model_name: field.value
+                for model_name, field in self.fields.items()
+                if field.value is not None
+            }
+
+        # print(data)
         try:
             self.model = self.model_cls(**data)
             self.is_valid = True
         except ValidationError as exc:
             self.is_valid = False
             for error in exc.errors():
                 loc = error.get("loc") or []
                 if not loc:
                     self.errors.append(error)
                 for name in loc:
                     field = self.fields.get(str(name))
                     if field:
                         field.error = error
 
-    def __repr__(self) -> str:
-        model_name = self.model_cls.__name__
-        model_form = f"{model_name}.as_form"
-
-        if self.is_empty:
-            return f"{model_form}(<empty>)"
-
-        if self.is_valid:
-            return repr(self.model).replace(model_name, model_form)
-        else:
-            return f"{model_form}(<invalid>)"
-
     @property
     def is_invalid(self):
         return not self.is_valid
 
+    @property
+    def object(self):
+        if self.wobject is None:
+            return None
+        return self.wobject.source
+
     def save(self) -> t.Any:
         if not self.model or not self.is_valid:
             raise ValueError("Form is not valid")
 
         data = self.model.model_dump()
 
-        if self.obj is not None:
-            return self.obj.update(data)
+        if self.wobject is not None:
+            return self.wobject.update(data)
 
         if self.orm_cls:
             return self.orm_cls(**data)
 
         return data
 
+    def __repr__(self) -> str:
+        model_name = self.model_cls.__name__
+        model_form = f"{model_name}.as_form"
+
+        if self.is_empty:
+            return f"{model_form}(<empty>)"
+
+        if self.is_valid:
+            return repr(self.model).replace(model_name, model_form)
+        else:
+            return f"{model_form}(<invalid>)"
+
     # Private
 
     def _get_model_value(self, name: str) -> t.Any:
         if not self.model:
             return None
         return getattr(self.model, name, None)
 
 
 class FormableBaseModel(BaseModel):
     @classmethod
     def as_form(
         cls,
         reqdata: t.Any = None,
         *,
-        obj: t.Any = None,
+        object: t.Any = None,
         prefix: str = "",
     ) -> "Form": ...
 
 
 BM = t.Type[BaseModel]
 FBM = t.Type[FormableBaseModel]
 
@@ -247,17 +265,17 @@
     def decorator(model_cls: BM) -> FBM:
         """The actual decorator logic that adds the `as_form` method."""
 
         def as_form(
             cls,
             reqdata: t.Any = None,
             *,
-            obj: t.Any = None,
+            object: t.Any = None,
             prefix: str = "",
         ) -> Form:
-            return Form(reqdata, obj=obj, prefix=prefix, model_cls=cls, orm_cls=orm)
+            return Form(reqdata, object=object, prefix=prefix, model_cls=cls, orm_cls=orm)
 
         setattr(model_cls, "as_form", classmethod(as_form))  # noqa
         model_cls = t.cast(FBM, model_cls)
         return model_cls
 
     return decorator if model_cls is None else decorator(model_cls)
```

### Comparing `fodantic-0.0.3/src/fodantic/form_field.py` & `fodantic-0.0.4/src/fodantic/form_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,18 +29,20 @@
         - model_name:
             The name used in the pydantic Model (different than the one in the
             HTML form if a prefix is used).
         - name:
             The name, maybe with a prefix, used in the HTML form.
         - value:
             The current (potentially invalid) field value.
-        - is_multiple:
-            Whether the field expects a list of values instead of just one.
         - is_required:
             Whether the field is required or optional.
+        - is_multiple:
+            Whether the field expects a list of values instead of just one.
+        - is_bool:
+            Whether the field is of type boolean.
 
         - annotation:
             The type annotation of the field.
         - alias:
             The alias name of the field.
         - alias_name:
             The alias, maybe with a prefix, that can be also used in the HTML form.
@@ -55,19 +57,20 @@
         - examples:
             List of examples of the field.
         - title:
             The title of the field.
 
         """
         self._form = form
-
         self.model_name = name
         self.is_required = info.is_required()
-        self.annotation_origin = t.get_origin(info.annotation)
-        self.is_multiple = self.annotation_origin in (list, tuple)
+
+        annotation_origin = t.get_origin(info.annotation)
+        self.is_multiple = annotation_origin in (list, tuple)
+        self.is_bool = info.annotation == bool or annotation_origin == bool
 
         self.annotation = info.annotation
         self.alias = info.alias
         self.alias_priority = info.alias_priority or 2
         self.default = info.default
         self.default_factory = info.default_factory
         self.description = info.description
@@ -89,14 +92,26 @@
 
     @property
     def alias_name(self) -> str:
         if self.alias:
             return f"{self._form.prefix}{self.alias}"
         return ""
 
+    def set_value(self, value: t.Any):
+        if self.is_bool:
+            if value is None:
+                self.value = False
+            elif value == "":
+                self.value = True
+            else:
+                self.value = bool(value)
+        if value is None:
+            return
+        self.value = value
+
     def extract_value(self, reqdata: t.Any) -> str | bool | None | list[str]:
         return (
             self._extract_many(reqdata)
             if self.is_multiple
             else self._extract_one(reqdata)
         )
 
@@ -106,31 +121,36 @@
             default = None
         if default is None:
             default = [] if self.is_multiple else ""
         return default
 
     # Private
 
-    def _extract_one(self, reqdata: t.Any) -> str | bool | None:
+    def _extract_one(self, reqdata: t.Any) -> t.Any:
+        if self.is_bool and (self.name not in reqdata):
+            return False
+
         value = reqdata.get(self.name)
         alias_value = reqdata.get(self.alias_name)
         if self.alias_priority > 1:
             value, alias_value = alias_value, value
 
         extracted = alias_value if value is None else value
 
-        if self.annotation == bool or self.annotation_origin == bool:
+        if self.is_bool:
             if extracted is None:
                 return False
             if extracted == "":
                 return True
             return bool(extracted)
 
         return extracted
 
-    def _extract_many(self, reqdata: t.Any) -> list[str]:
+    def _extract_many(self, reqdata: t.Any) -> list[str] | None:
+        if self.name not in reqdata:
+            return None
         value = reqdata.getall(self.name)
         alias_value = reqdata.getall(self.alias_name)
         if self.alias_priority > 1:
             value, alias_value = alias_value, value
 
         return alias_value if value == [] else value
```

### Comparing `fodantic-0.0.3/src/fodantic/wrapper.py` & `fodantic-0.0.4/src/fodantic/wrappers.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,49 +13,75 @@
 
         ## Arguments:
 
         - source: The underlying data source. Can be a Multidict implementation
             or a regular dict.
 
         """
-        self.source = source
-        self.get = self._get_get_method()
-        self.getall = self._get_getall_method()
+        self.source: t.Any = {} if source is None else source
+        self.get = self._find_get_method()
+        self.getall = self._find_getall_method()
 
-    def update(self, data: dict[str, t.Any]) -> t.Any:
-        if hasattr(self.source, "update"):
-            self.source.update(data)
-        else:
-            for key, value in data.items():
-                setattr(self.source, key, value)
-
-        return self.source
+    def __contains__(self, __name: str) -> bool:
+        return __name in self.source
 
-    def _get_get_method(self) -> t.Callable[[str], t.Any]:
-        if self.source and hasattr(self.source, "get"):
+    def _find_get_method(self) -> t.Callable[[str], t.Any]:
+        if hasattr(self.source, "get"):
             return self.source.get
 
         def get_fallback(name: str) -> t.Any:
-            if not self.source:
-                return None
-            return getattr(self.source, name)
+            return getattr(self.source, name, None)
 
         return get_fallback
 
-    def _get_getall_method(self) -> t.Callable[[str], list[t.Any]]:
-        if self.source:
-            # WebOb, Bottle, and Proper uses `getall`
-            if hasattr(self.source, "getall"):
-                return self.source.getall
-            # Django, Flask (Werkzeug), cgi.FieldStorage, etc. uses `getlist`
-            if hasattr(self.source, "getlist"):
-                return self.source.getlist
+    def _find_getall_method(self) -> t.Callable[[str], list[t.Any]]:
+        # WebOb, Bottle, and Proper uses `getall`
+        if hasattr(self.source, "getall"):
+            return self.source.getall
+        # Django, Flask (Werkzeug), cgi.FieldStorage, etc. uses `getlist`
+        if hasattr(self.source, "getlist"):
+            return self.source.getlist
 
         def getall_fallback(name: str) -> list[t.Any]:
-            if not self.source:
-                return []
             values = self.get(name)
             if values is None:
                 return []
+            if isinstance(values, list):
+                return values
             return [values]
 
         return getall_fallback
+
+
+class ObjectWrapper:
+    def __init__(self, source: t.Any):
+        """
+        A utility class for wrapping request data and providing a consistent interface
+        for updating, accessing single values, or lists of values.
+
+        ## Arguments:
+
+        - source: The underlying data source. Can be a Multidict implementation
+            or a regular dict.
+
+        """
+        self.source: t.Any = {} if source is None else source
+        self.is_dict = isinstance(source, dict)
+        self.get = self._find_get_method()
+
+    def _find_get_method(self) -> t.Callable[[str], t.Any]:
+        if self.is_dict:
+            return self.source.get
+
+        def get_fallback(name: str) -> t.Any:
+            return getattr(self.source, name, None)
+
+        return get_fallback
+
+    def update(self, data: dict[str, t.Any]) -> t.Any:
+        if self.is_dict:
+            self.source.update(data)
+        else:
+            for key, value in data.items():
+                setattr(self.source, key, value)
+
+        return self.source
```

### Comparing `fodantic-0.0.3/src/fodantic.egg-info/PKG-INFO` & `fodantic-0.0.4/src/fodantic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fodantic
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pydantic-based HTTP forms
 Author-email: Juan-Pablo Scaletti <juanpablo@jpscaletti.com>
 License: Copyright (c) Juan-Pablo Scaletti
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -63,22 +63,27 @@
 @formable
 class UserModel(BaseModel):
     name: str
     friends: list[int]
     active: bool = True
 
 request_data = Multidict(('name', 'John Doe'), ('friends', '2'), ('friends', '3')}
-form = UserModel.as_form(request_data, obj=None)
+
+# The magic
+form = UserModel.as_form(request_data, object=None)
 
 print(form)
 #> UserModel.as_form(name='John Doe', friends=[2, 3], active=False)
 print(form.fields["name"].value)
 #> John Doe
 print(form.fields["name"].error)
-#>
+#> None
+print(form.save())  # Can also update the `object` passed as an argument
+#> {'name': 'John Doe', 'friends': [2, 3], 'active': False}
+
 ```
 
 
 ## Installation
 
   pip install fodantic
```

