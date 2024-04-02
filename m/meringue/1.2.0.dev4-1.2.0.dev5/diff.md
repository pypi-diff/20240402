# Comparing `tmp/meringue-1.2.0.dev4.tar.gz` & `tmp/meringue-1.2.0.dev5.tar.gz`

## Comparing `meringue-1.2.0.dev4.tar` & `meringue-1.2.0.dev5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/apps.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/routers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/docs/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/docs/patchers.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/api/docs/views.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/conf/__init__.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/apps.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/fields.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/protected/views.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/actions.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/apps.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/constants.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/drf_fields.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/exceptions.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/generators.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/images.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/properties.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/shortcuts.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/storage.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/templatetags/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/meringue/thumbnail/templatetags/m_thumbnails.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/LICENSE
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/README.md
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 meringue-1.2.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/apps.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/routers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/conf/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/protected/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/protected/apps.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/protected/fields.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/protected/views.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/actions.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/apps.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/constants.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/drf_fields.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/exceptions.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/generators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/images.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/properties.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/shortcuts.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/storage.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/templatetags/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/meringue/thumbnail/templatetags/m_thumbnails.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/LICENSE
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/README.md
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     7906 2020-02-02 00:00:00.000000 meringue-1.2.0.dev5/PKG-INFO
```

### Comparing `meringue-1.2.0.dev4/meringue/api/handlers.py` & `meringue-1.2.0.dev5/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/api/routers.py` & `meringue-1.2.0.dev5/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/api/utils.py` & `meringue-1.2.0.dev5/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/api/docs/patchers.py` & `meringue-1.2.0.dev5/meringue/api/docs/patchers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/api/docs/views.py` & `meringue-1.2.0.dev5/meringue/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/conf/__init__.py` & `meringue-1.2.0.dev5/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/conf/default_settings.py` & `meringue-1.2.0.dev5/meringue/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/models.py` & `meringue-1.2.0.dev5/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/query.py` & `meringue-1.2.0.dev5/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/translation.py` & `meringue-1.2.0.dev5/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/upload_handlers.py` & `meringue-1.2.0.dev5/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.2.0.dev5/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.2.0.dev5/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/templatetags/meringue_base.py` & `meringue-1.2.0.dev5/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/utils/crypt.py` & `meringue-1.2.0.dev5/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/utils/datetime.py` & `meringue-1.2.0.dev5/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/core/utils/frontend.py` & `meringue-1.2.0.dev5/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/protected/fields.py` & `meringue-1.2.0.dev5/meringue/protected/fields.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class ProtectedFileMixin:
     @property
     def url(self):
         self._require_file()
         result_url = reverse(
-            "meringue-protected-file",
+            self.field.m_protected_view_name,
             kwargs={
                 "contenttype_id": ContentType.objects.get_for_model(self.instance.__class__).id,
                 "field": self.field.name,
                 "pk": self.instance.pk,
             },
         )
         return result_url
@@ -27,23 +27,49 @@
 
 
 class ProtectedFieldFile(ProtectedFileMixin, FieldFile):
     pass
 
 
 class ProtectedFileField(FileField):
+    """
+    A field that adds the mechanism of a protected file.
+    """
+
     attr_class = ProtectedFieldFile
 
-    def __init__(self, verbose_name=None, name=None, upload_to="protected", storage=None, **kwargs):
+    def __init__(
+        self,
+        verbose_name=None,
+        name=None,
+        upload_to="protected",
+        storage=None,
+        protected_view_name="meringue-protected-file",
+        **kwargs,
+    ):
+        self.m_protected_view_name = protected_view_name
         super().__init__(verbose_name, name, upload_to, storage, **kwargs)
 
 
 class ProtectedImageFieldFile(ProtectedFileMixin, ImageFieldFile):
     pass
 
 
 class ProtectedImageField(ImageField):
+    """
+    A field that adds the mechanism of a protected image.
+    """
+
     attr_class = ProtectedImageFieldFile
 
-    def __init__(self, verbose_name=None, name=None, width_field=None, height_field=None, **kwargs):
+    def __init__(
+        self,
+        verbose_name=None,
+        name=None,
+        width_field=None,
+        height_field=None,
+        protected_view_name="meringue-protected-file",
+        **kwargs,
+    ):
         kwargs.setdefault("upload_to", "protected")
+        self.m_protected_view_name = protected_view_name
         super().__init__(verbose_name, name, width_field, height_field, **kwargs)
```

### Comparing `meringue-1.2.0.dev4/meringue/protected/views.py` & `meringue-1.2.0.dev5/meringue/protected/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/actions.py` & `meringue-1.2.0.dev5/meringue/thumbnail/actions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/constants.py` & `meringue-1.2.0.dev5/meringue/thumbnail/constants.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/drf_fields.py` & `meringue-1.2.0.dev5/meringue/thumbnail/drf_fields.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/exceptions.py` & `meringue-1.2.0.dev5/meringue/thumbnail/exceptions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/generators.py` & `meringue-1.2.0.dev5/meringue/thumbnail/generators.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/images.py` & `meringue-1.2.0.dev5/meringue/thumbnail/images.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/properties.py` & `meringue-1.2.0.dev5/meringue/thumbnail/properties.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/shortcuts.py` & `meringue-1.2.0.dev5/meringue/thumbnail/shortcuts.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/storage.py` & `meringue-1.2.0.dev5/meringue/thumbnail/storage.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/meringue/thumbnail/templatetags/m_thumbnails.py` & `meringue-1.2.0.dev5/meringue/thumbnail/templatetags/m_thumbnails.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/LICENSE` & `meringue-1.2.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/README.md` & `meringue-1.2.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/pyproject.toml` & `meringue-1.2.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev4/PKG-INFO` & `meringue-1.2.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: meringue
-Version: 1.2.0.dev4
+Version: 1.2.0.dev5
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Documentation, https://dd.github.io/Meringue
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@tovarisch.engineer>
 License-Expression: LGPL-3.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: meringue Version: 1.2.0.dev4 Summary: A set of
+Metadata-Version: 2.3 Name: meringue Version: 1.2.0.dev5 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Documentation, https://dd.github.io/Meringue Project-URL: Repository, https://
 github.com/dd/Meringue Project-URL: Changelog, https://github.com/dd/Meringue/
 blob/master/CHANGELOG.md Project-URL: Bug Tracker, https://github.com/dd/
 Meringue/issues Author-email: Dmitry Dobrynin
 tovarisch.engineer> License-Expression: LGPL-3.0 License-File: AUTHORS License-
 File: LICENSE Keywords: django,utils Classifier: Development Status :: 5 -
```

