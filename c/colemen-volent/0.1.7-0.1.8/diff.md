# Comparing `tmp/colemen_volent-0.1.7.tar.gz` & `tmp/colemen_volent-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_volent-0.1.7.tar", last modified: Sun Mar 31 16:11:43 2024, max compression
+gzip compressed data, was "colemen_volent-0.1.8.tar", last modified: Tue Apr  2 20:13:20 2024, max compression
```

## Comparing `colemen_volent-0.1.7.tar` & `colemen_volent-0.1.8.tar`

### file list

```diff
@@ -1,79 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.847989 colemen_volent-0.1.7/
--rw-rw-rw-   0        0        0      469 2024-03-31 16:11:43.846989 colemen_volent-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.770988 colemen_volent-0.1.7/colemen_volent.egg-info/
--rw-rw-rw-   0        0        0      469 2024-03-31 16:11:43.000000 colemen_volent-0.1.7/colemen_volent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1814 2024-03-31 16:11:43.000000 colemen_volent-0.1.7/colemen_volent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:11:43.000000 colemen_volent-0.1.7/colemen_volent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-31 16:11:43.000000 colemen_volent-0.1.7/colemen_volent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-31 16:11:43.000000 colemen_volent-0.1.7/colemen_volent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 16:11:43.847989 colemen_volent-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-03-31 16:11:42.000000 colemen_volent-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.772987 colemen_volent-0.1.7/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.1.7/tests/schema_dict_test.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.790988 colemen_volent-0.1.7/volent/
--rw-rw-rw-   0        0        0    10003 2023-05-07 20:40:28.000000 colemen_volent-0.1.7/volent/Column.py
--rw-rw-rw-   0        0        0    10788 2023-05-08 18:14:13.000000 colemen_volent-0.1.7/volent/Database.py
--rw-rw-rw-   0        0        0    14712 2023-05-07 21:21:17.000000 colemen_volent-0.1.7/volent/Field.py
--rw-rw-rw-   0        0        0     2914 2023-04-28 15:52:22.000000 colemen_volent-0.1.7/volent/FullTextIndex.py
--rw-rw-rw-   0        0        0    34852 2023-05-08 13:47:52.000000 colemen_volent-0.1.7/volent/Model.py
--rw-rw-rw-   0        0        0     9621 2023-05-07 21:32:40.000000 colemen_volent-0.1.7/volent/NestedField.py
--rw-rw-rw-   0        0        0     5037 2023-04-28 17:06:40.000000 colemen_volent-0.1.7/volent/Relationship.py
--rw-rw-rw-   0        0        0    21549 2023-04-28 20:34:26.000000 colemen_volent-0.1.7/volent/ReverseEngineer.py
--rw-rw-rw-   0        0        0    28274 2023-05-07 21:21:49.000000 colemen_volent-0.1.7/volent/Schema.py
--rw-rw-rw-   0        0        0     1195 2023-05-08 16:29:35.000000 colemen_volent-0.1.7/volent/Trigger.py
--rw-rw-rw-   0        0        0     2657 2023-04-28 15:48:09.000000 colemen_volent-0.1.7/volent/UniqueConstraint.py
--rw-rw-rw-   0        0        0    18361 2023-05-08 18:34:56.000000 colemen_volent-0.1.7/volent/Volent.py
--rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.1.7/volent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.801990 colemen_volent-0.1.7/volent/data_types/
--rw-rw-rw-   0        0        0     2345 2023-04-26 13:07:40.000000 colemen_volent-0.1.7/volent/data_types/BigInt.py
--rw-rw-rw-   0        0        0     1815 2023-04-27 19:22:16.000000 colemen_volent-0.1.7/volent/data_types/Bool.py
--rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.1.7/volent/data_types/Decimal.py
--rw-rw-rw-   0        0        0     1793 2023-04-26 13:07:50.000000 colemen_volent-0.1.7/volent/data_types/EncodedPrimary.py
--rw-rw-rw-   0        0        0     1954 2023-04-26 16:26:49.000000 colemen_volent-0.1.7/volent/data_types/Integer.py
--rw-rw-rw-   0        0        0     2787 2023-04-27 19:21:56.000000 colemen_volent-0.1.7/volent/data_types/String.py
--rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.1.7/volent/data_types/TinyInt.py
--rw-rw-rw-   0        0        0     4481 2023-05-08 15:10:58.000000 colemen_volent-0.1.7/volent/data_types/TypeBase.py
--rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.1.7/volent/data_types/__init__.py
--rw-rw-rw-   0        0        0     3362 2023-04-27 21:05:39.000000 colemen_volent-0.1.7/volent/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.809988 colemen_volent-0.1.7/volent/mixins/
--rw-rw-rw-   0        0        0    26960 2023-05-08 18:23:24.000000 colemen_volent-0.1.7/volent/mixins/DatabaseConnection.py
--rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.1.7/volent/mixins/EntityName.py
--rw-rw-rw-   0        0        0    27271 2023-05-08 18:06:08.000000 colemen_volent-0.1.7/volent/mixins/MySQLGeneratorMixin.py
--rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.1.7/volent/mixins/OrderedClass.py
--rw-rw-rw-   0        0        0     1835 2023-04-28 20:31:20.000000 colemen_volent-0.1.7/volent/mixins/ReverseEngineerMixin.py
--rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.1.7/volent/mixins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.819018 colemen_volent-0.1.7/volent/query/
--rw-rw-rw-   0        0        0     4801 2023-04-28 12:53:20.000000 colemen_volent-0.1.7/volent/query/Delete.py
--rw-rw-rw-   0        0        0    10091 2023-05-15 16:31:04.000000 colemen_volent-0.1.7/volent/query/Insert.py
--rw-rw-rw-   0        0        0    21408 2023-05-08 17:43:32.000000 colemen_volent-0.1.7/volent/query/Query.py
--rw-rw-rw-   0        0        0    10162 2023-05-07 21:56:41.000000 colemen_volent-0.1.7/volent/query/Select.py
--rw-rw-rw-   0        0        0     5321 2023-04-28 14:43:43.000000 colemen_volent-0.1.7/volent/query/Update.py
--rw-rw-rw-   0        0        0    13639 2023-05-07 22:01:32.000000 colemen_volent-0.1.7/volent/query/WhereMixin.py
--rw-rw-rw-   0        0        0      183 2023-04-26 16:50:07.000000 colemen_volent-0.1.7/volent/query/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.822989 colemen_volent-0.1.7/volent/settings/
--rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.1.7/volent/settings/__init__.py
--rw-rw-rw-   0        0        0     6183 2023-04-24 14:05:40.000000 colemen_volent-0.1.7/volent/settings/control.py
--rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.1.7/volent/settings/globe.py
--rw-rw-rw-   0        0        0     2484 2023-05-07 20:55:51.000000 colemen_volent-0.1.7/volent/settings/types.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.825988 colemen_volent-0.1.7/volent/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.1.7/volent/tests/__init__.py
--rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.1.7/volent/tests/schema_dict_test.py
--rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.1.7/volent/tests/validators_test.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:11:43.845989 colemen_volent-0.1.7/volent/validate/
--rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.1.7/volent/validate/CreditCardNumber.py
--rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.1.7/volent/validate/Email.py
--rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.1.7/volent/validate/Equal.py
--rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.1.7/volent/validate/FutureUnixDate.py
--rw-rw-rw-   0        0        0     3993 2023-04-25 15:53:35.000000 colemen_volent-0.1.7/volent/validate/IpAddress.py
--rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.1.7/volent/validate/Length.py
--rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.1.7/volent/validate/NoneOf.py
--rw-rw-rw-   0        0        0     2771 2023-04-25 15:57:11.000000 colemen_volent-0.1.7/volent/validate/OneOf.py
--rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.1.7/volent/validate/PastUnixDate.py
--rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.1.7/volent/validate/PhoneNumber.py
--rw-rw-rw-   0        0        0     5995 2023-04-25 15:51:54.000000 colemen_volent-0.1.7/volent/validate/Range.py
--rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.1.7/volent/validate/Regex.py
--rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.1.7/volent/validate/SocialSecurityNumber.py
--rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.1.7/volent/validate/StrongPassword.py
--rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.1.7/volent/validate/Validator.py
--rw-rw-rw-   0        0        0      770 2023-04-24 16:48:21.000000 colemen_volent-0.1.7/volent/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.977916 colemen_volent-0.1.8/
+-rw-rw-rw-   0        0        0      469 2024-04-02 20:13:20.976915 colemen_volent-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.793914 colemen_volent-0.1.8/colemen_volent.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-04-02 20:13:20.000000 colemen_volent-0.1.8/colemen_volent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1928 2024-04-02 20:13:20.000000 colemen_volent-0.1.8/colemen_volent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:13:20.000000 colemen_volent-0.1.8/colemen_volent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-02 20:13:20.000000 colemen_volent-0.1.8/colemen_volent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-02 20:13:20.000000 colemen_volent-0.1.8/colemen_volent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 20:13:20.977916 colemen_volent-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-04-02 20:13:19.000000 colemen_volent-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.803915 colemen_volent-0.1.8/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.1.8/tests/schema_dict_test.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.850916 colemen_volent-0.1.8/volent/
+-rw-rw-rw-   0        0        0    10030 2024-04-01 19:24:32.000000 colemen_volent-0.1.8/volent/Column.py
+-rw-rw-rw-   0        0        0    10951 2024-04-01 19:23:52.000000 colemen_volent-0.1.8/volent/Database.py
+-rw-rw-rw-   0        0        0    14712 2023-05-07 21:21:17.000000 colemen_volent-0.1.8/volent/Field.py
+-rw-rw-rw-   0        0        0     2914 2023-04-28 15:52:22.000000 colemen_volent-0.1.8/volent/FullTextIndex.py
+-rw-rw-rw-   0        0        0    36555 2024-04-02 17:23:36.000000 colemen_volent-0.1.8/volent/Model.py
+-rw-rw-rw-   0        0        0     9621 2023-05-07 21:32:40.000000 colemen_volent-0.1.8/volent/NestedField.py
+-rw-rw-rw-   0        0        0     5037 2023-04-28 17:06:40.000000 colemen_volent-0.1.8/volent/Relationship.py
+-rw-rw-rw-   0        0        0    21549 2023-04-28 20:34:26.000000 colemen_volent-0.1.8/volent/ReverseEngineer.py
+-rw-rw-rw-   0        0        0    32371 2024-04-02 20:13:15.000000 colemen_volent-0.1.8/volent/Schema.py
+-rw-rw-rw-   0        0        0     1195 2023-05-08 16:29:35.000000 colemen_volent-0.1.8/volent/Trigger.py
+-rw-rw-rw-   0        0        0     2657 2023-04-28 15:48:09.000000 colemen_volent-0.1.8/volent/UniqueConstraint.py
+-rw-rw-rw-   0        0        0    18452 2024-04-01 19:25:16.000000 colemen_volent-0.1.8/volent/Volent.py
+-rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.1.8/volent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.871915 colemen_volent-0.1.8/volent/data_types/
+-rw-rw-rw-   0        0        0     2345 2023-04-26 13:07:40.000000 colemen_volent-0.1.8/volent/data_types/BigInt.py
+-rw-rw-rw-   0        0        0     1815 2023-04-27 19:22:16.000000 colemen_volent-0.1.8/volent/data_types/Bool.py
+-rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.1.8/volent/data_types/Decimal.py
+-rw-rw-rw-   0        0        0     1793 2023-04-26 13:07:50.000000 colemen_volent-0.1.8/volent/data_types/EncodedPrimary.py
+-rw-rw-rw-   0        0        0     1954 2023-04-26 16:26:49.000000 colemen_volent-0.1.8/volent/data_types/Integer.py
+-rw-rw-rw-   0        0        0     2787 2023-04-27 19:21:56.000000 colemen_volent-0.1.8/volent/data_types/String.py
+-rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.1.8/volent/data_types/TinyInt.py
+-rw-rw-rw-   0        0        0     4481 2023-05-08 15:10:58.000000 colemen_volent-0.1.8/volent/data_types/TypeBase.py
+-rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.1.8/volent/data_types/__init__.py
+-rw-rw-rw-   0        0        0     3362 2023-04-27 21:05:39.000000 colemen_volent-0.1.8/volent/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.880921 colemen_volent-0.1.8/volent/mixins/
+-rw-rw-rw-   0        0        0    30021 2024-04-01 19:22:25.000000 colemen_volent-0.1.8/volent/mixins/DatabaseConnection.py
+-rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.1.8/volent/mixins/EntityName.py
+-rw-rw-rw-   0        0        0    27271 2023-05-08 18:06:08.000000 colemen_volent-0.1.8/volent/mixins/MySQLGeneratorMixin.py
+-rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.1.8/volent/mixins/OrderedClass.py
+-rw-rw-rw-   0        0        0     1835 2023-04-28 20:31:20.000000 colemen_volent-0.1.8/volent/mixins/ReverseEngineerMixin.py
+-rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.1.8/volent/mixins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.930914 colemen_volent-0.1.8/volent/query/
+-rw-rw-rw-   0        0        0     4801 2023-04-28 12:53:20.000000 colemen_volent-0.1.8/volent/query/Delete.py
+-rw-rw-rw-   0        0        0    10711 2024-04-01 19:24:45.000000 colemen_volent-0.1.8/volent/query/Insert.py
+-rw-rw-rw-   0        0        0    25261 2024-04-02 15:02:15.000000 colemen_volent-0.1.8/volent/query/Query.py
+-rw-rw-rw-   0        0        0     2000 2024-04-02 14:28:32.000000 colemen_volent-0.1.8/volent/query/QueryParam.py
+-rw-rw-rw-   0        0        0    11675 2024-04-02 15:17:38.000000 colemen_volent-0.1.8/volent/query/Select.py
+-rw-rw-rw-   0        0        0    10555 2024-04-02 15:58:45.000000 colemen_volent-0.1.8/volent/query/Update.py
+-rw-rw-rw-   0        0        0     7566 2024-04-02 15:41:13.000000 colemen_volent-0.1.8/volent/query/WhereClause.py
+-rw-rw-rw-   0        0        0    14613 2024-04-01 22:27:51.000000 colemen_volent-0.1.8/volent/query/WhereMixin.py
+-rw-rw-rw-   0        0        0      183 2023-04-26 16:50:07.000000 colemen_volent-0.1.8/volent/query/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.942915 colemen_volent-0.1.8/volent/settings/
+-rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.1.8/volent/settings/__init__.py
+-rw-rw-rw-   0        0        0     6346 2024-04-02 15:41:23.000000 colemen_volent-0.1.8/volent/settings/control.py
+-rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.1.8/volent/settings/globe.py
+-rw-rw-rw-   0        0        0     3499 2024-04-02 15:25:01.000000 colemen_volent-0.1.8/volent/settings/types.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.954916 colemen_volent-0.1.8/volent/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.1.8/volent/tests/__init__.py
+-rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.1.8/volent/tests/schema_dict_test.py
+-rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.1.8/volent/tests/validators_test.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:13:20.975916 colemen_volent-0.1.8/volent/validate/
+-rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.1.8/volent/validate/CreditCardNumber.py
+-rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.1.8/volent/validate/Email.py
+-rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.1.8/volent/validate/Equal.py
+-rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.1.8/volent/validate/FutureUnixDate.py
+-rw-rw-rw-   0        0        0     2104 2024-04-02 18:26:45.000000 colemen_volent-0.1.8/volent/validate/GreaterThan.py
+-rw-rw-rw-   0        0        0     3993 2023-04-25 15:53:35.000000 colemen_volent-0.1.8/volent/validate/IpAddress.py
+-rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.1.8/volent/validate/Length.py
+-rw-rw-rw-   0        0        0     2083 2024-04-02 18:26:55.000000 colemen_volent-0.1.8/volent/validate/LessThan.py
+-rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.1.8/volent/validate/NoneOf.py
+-rw-rw-rw-   0        0        0     2771 2023-04-25 15:57:11.000000 colemen_volent-0.1.8/volent/validate/OneOf.py
+-rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.1.8/volent/validate/PastUnixDate.py
+-rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.1.8/volent/validate/PhoneNumber.py
+-rw-rw-rw-   0        0        0     5995 2023-04-25 15:51:54.000000 colemen_volent-0.1.8/volent/validate/Range.py
+-rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.1.8/volent/validate/Regex.py
+-rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.1.8/volent/validate/SocialSecurityNumber.py
+-rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.1.8/volent/validate/StrongPassword.py
+-rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.1.8/volent/validate/Validator.py
+-rw-rw-rw-   0        0        0      870 2024-04-02 18:14:05.000000 colemen_volent-0.1.8/volent/validate/__init__.py
```

### Comparing `colemen_volent-0.1.7/colemen_volent.egg-info/SOURCES.txt` & `colemen_volent-0.1.8/colemen_volent.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,31 +34,35 @@
 volent/mixins/MySQLGeneratorMixin.py
 volent/mixins/OrderedClass.py
 volent/mixins/ReverseEngineerMixin.py
 volent/mixins/__init__.py
 volent/query/Delete.py
 volent/query/Insert.py
 volent/query/Query.py
+volent/query/QueryParam.py
 volent/query/Select.py
 volent/query/Update.py
+volent/query/WhereClause.py
 volent/query/WhereMixin.py
 volent/query/__init__.py
 volent/settings/__init__.py
 volent/settings/control.py
 volent/settings/globe.py
 volent/settings/types.py
 volent/tests/__init__.py
 volent/tests/schema_dict_test.py
 volent/tests/validators_test.py
 volent/validate/CreditCardNumber.py
 volent/validate/Email.py
 volent/validate/Equal.py
 volent/validate/FutureUnixDate.py
+volent/validate/GreaterThan.py
 volent/validate/IpAddress.py
 volent/validate/Length.py
+volent/validate/LessThan.py
 volent/validate/NoneOf.py
 volent/validate/OneOf.py
 volent/validate/PastUnixDate.py
 volent/validate/PhoneNumber.py
 volent/validate/Range.py
 volent/validate/Regex.py
 volent/validate/SocialSecurityNumber.py
```

### Comparing `colemen_volent-0.1.7/setup.py` & `colemen_volent-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from glob import glob
 from setuptools import setup, find_packages
 import colemen_utilities.build_utils.general as _gen
 
 
-VERSION='0.1.7'
+VERSION='0.1.8'
 DESCRIPTION = 'volent'
 LONG_DESCRIPTION = 'None'
 
 
 _root_path = f"{os.getcwd()}/volent"
 PY_MODULES = _gen.list_py_modules(
     _root_path,
```

### Comparing `colemen_volent-0.1.7/tests/schema_dict_test.py` & `colemen_volent-0.1.8/tests/schema_dict_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/Column.py` & `colemen_volent-0.1.8/volent/Column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
 
 
 from dataclasses import dataclass
+from time import time
 from typing import Iterable
 
 import colemen_utils as _c
 
 import volent.settings.types as _t
 import volent.settings as _settings
 from volent.mixins import MySQLGeneratorMixin
@@ -126,14 +127,16 @@
         self.comment = comment
         self.is_foreign_key = is_foreign_key
         self.is_primary = is_primary
         self.auto_increment = auto_increment
         self.dump_only = dump_only
         self._column_value = _t.undefined
 
+
+
     @property
     def summary(self):
         '''
             Get this Column's summary
 
             `default`:None
```

### Comparing `colemen_volent-0.1.7/volent/Database.py` & `colemen_volent-0.1.8/volent/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,15 +324,20 @@
             * @xxx [12-16-2022 08:44:37]: documentation for last_id
         '''
         sql = 'SELECT LAST_INSERT_ID();'
         if _settings.globe.flavor in ['sqlite']:
             sql = "SELECT last_insert_rowid()"
         result = self.run_select(sql)
         if isinstance(result,(list)):
-            result = result[0]['LAST_INSERT_ID()']
+            try:
+                result = result[0]['LAST_INSERT_ID()']
+            except TypeError:
+                result = result[0][0]
+            except IndexError:
+                result = result[0][0]
         return result
```

### Comparing `colemen_volent-0.1.7/volent/Field.py` & `colemen_volent-0.1.8/volent/Field.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/FullTextIndex.py` & `colemen_volent-0.1.8/volent/FullTextIndex.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/Model.py` & `colemen_volent-0.1.8/volent/Model.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,25 +129,59 @@
                     continue
                 if v != _t.no_default:
                     col.value = v
         self._parent_models = []
         self._child_models = []
         self.__gen_auto_columns()
 
+    def __repr__(self) -> str:
+        return f"<Model: {self._model_name} | Columns:{len(self.columns)}>"
+
+    def _cpid(self,data,locals):
+
+        d = {}
+        for x in data.args:
+            # if x in ["self","_is_root"]:
+            #     continue
+            d[x] = locals[x]
+            # print(f"x : {x}")
+        d = self.filter_dict_by_columns(d)
+        # for k,v in d.items():
+        #     col = self.get_column(k)
+        #     if col is not None:
+        #         print(f"value for column:{col.name} found: {v}")
+
+        return d
+
     def _get_attrs_from_parent(self):
         '''Used internally to apply the root model attributes to this instance.
 
         Essentially this just copies the database reference to all child instances of a model.
         '''
         if self._is_root is False:
             # print(f"self.name:{self.name}")
             mdl = _settings.globe.Volent.get_model(self.model_name)
             self._database = mdl.database
 
     def __setattr__(self, name, value):
+        # This is useful for setting the value of a column without accessing the column itself
+        # Not critically necessary but it is convenient.
+        try:
+            # @Mstep [] Attempt to retrieve a column with a matching name.
+            nv = super().__getattribute__(name)
+            # @Mstep [IF] if the attribute exists and its a column instance.
+            if isinstance(nv,(_column)):
+                # @Mstep [] set the column value to the value provided.
+                nv.value = value
+                # @Mstep [RETURN] 
+                return
+        except AttributeError:
+            pass
+
+
         super().__setattr__(name, value)
 
         if not name in self._order:
             self._order.append(name)
             if isinstance(value,_column):
                 cols = [] if self._columns is None else self._columns
                 col_lookup = {} if self._column_lookup is None else self._column_lookup
@@ -354,14 +388,15 @@
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 04-11-2023 14:48:54
             `@memberOf`: Model
             `@property`: data
         '''
+        self.__gen_auto_columns()
         value = {}
         for col in self.columns:
             value[col.name] = col.value
         return value
 
 
     @property
@@ -389,14 +424,15 @@
             for key in keys:
                 if hasattr(self,key):
                     val = getattr(self,key)
                     break
             # if hasattr(self,"__table_name__"):
                 # value = getattr(self,"__table_name__")
             self._gen_meta_columns = val
+            value = val
         return value
 
     def __gen_auto_columns(self):
         '''
             If the __meta_columns__ key is True, this will create the
             timestamp,deleted and modified_timestamp columns on this model automatically.
 
@@ -410,24 +446,29 @@
             `version`: 1.0
             `method_name`: __gen_auto_columns
             * @xxx [04-28-2023 11:08:31]: documentation for __gen_auto_columns
         '''
         if self.gen_meta_columns is False:
             return
 
+
         from volent.data_types import Integer
         cut = round(datetime.now(tz=timezone.utc).timestamp())
 
         ct = _column(Integer(), nullable=True, on_insert=cut, comment='The unix timestamp of when this was created.')
         dt = _column(Integer(), nullable=True, default=None, comment='The unix timestamp of when this was deleted, null otherwise.')
         mt = _column(Integer(), nullable=True, default=None, on_update=cut,on_insert=cut, comment='The unix timestamp of when this was last modified, null otherwise.')
         setattr(self,"timestamp",ct)
         setattr(self,"modified_timestamp",mt)
         setattr(self,"deleted",dt)
 
+        # self._columns.append(ct)
+        # self._columns.append(mt)
+        # self._columns.append(dt)
+
     def __gen_col_sums(self):
         primes = []
         col_lookup = {}
 
         for col in self.columns:
             col_lookup[col.name] = col
             if col.is_primary is True:
@@ -473,14 +514,22 @@
 
         for col in self.columns:
             if col.name == name:
                 return col
 
         return None
 
+    def filter_dict_by_columns(self,data:dict):
+        out = {}
+        for col in self.columns:
+            if col.name in data:
+                out[col.name] = data[col.name]
+        return out
+
+
     @property
     def columns(self)->Iterable[_t.column_type]:
         '''
             Get this Model's columns
 
             `default`:None
 
@@ -489,15 +538,15 @@
             ----------
             `@author`: Colemen Atwood
             `@created`: 04-11-2023 14:07:35
             `@memberOf`: Model
             `@property`: columns
         '''
         value = self._columns
-
+        self.__gen_auto_columns()
         if value is None:
             # print(f"GENERATING COLUMN LIST {'-'*80}")
             dif = self._unique_prop_keys
             # df_props = dir(Model(_is_root=False))
             # # # @Mstep [] gather the props of this instance.
             # props = dir(self)
             # # # @Mstep [] find the props that exist on this instance and not on the base.
@@ -825,18 +874,21 @@
             `version`: 1.0
             `method_name`: insert
             * @xxx [04-28-2023 09:49:25]: documentation for insert
         '''
         # self.database.run('show variables like "max_connections";')
         # print(self.database.fetchall())
         if isinstance(data,(dict)) is False:
+            if data is None:
+                data = self.data
             from volent.Schema import Schema as _schema
             if isinstance(data,_schema):
                 data.model = self
                 data = data.dump(self)
+            
 
         ins = _insert(self,data)
         # ins.database = self.database
         # result = ins.execute()
         return ins
 
     def select(self,*columns)->_select:
@@ -862,15 +914,15 @@
             `version`: 1.0
             `method_name`: select
             * @xxx [04-28-2023 09:51:05]: documentation for select
         '''
         s = _select(self,columns=columns)
         return s
 
-    def update(self,**columns)->_update:
+    def update(self,*columns)->_t.update_query_type:
         '''
             Create an update query on this model.
 
             ----------
 
             Keyword Arguments
             -------------------------
@@ -886,15 +938,15 @@
             `author`: Colemen Atwood
             `created`: 04-28-2023 09:49:36
             `memberOf`: Model
             `version`: 1.0
             `method_name`: update
             * @xxx [04-28-2023 09:51:05]: documentation for update
         '''
-        # print(f"columns: {columns}")
+        print(f"columns: {columns}")
         s = _update(self,columns=columns)
         return s
 
     def delete(self)->_delete:
         '''
             Create a delete query on this model.
```

### Comparing `colemen_volent-0.1.7/volent/NestedField.py` & `colemen_volent-0.1.8/volent/NestedField.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/Relationship.py` & `colemen_volent-0.1.8/volent/Relationship.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/ReverseEngineer.py` & `colemen_volent-0.1.8/volent/ReverseEngineer.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/Schema.py` & `colemen_volent-0.1.8/volent/Schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,35 +24,43 @@
 
 @dataclass
 class Schema(metaclass=OrderedClass):
 
     main = None
     # database:_t.database_type = None
     model:_t.model_type = None
+    _table_name:str = None
     _name:str = None
     _fields:Iterable[_t.field_type] = None
     _nested_fields:Iterable[_t.nested_field_type] = None
     _schema_description:str = None
     _schema_crud_type:str = None
 
     __unique_prop_keys = None
 
+    has_nested_schemas:bool = False
+
     # _field_aliases = None
 
 
 
     def __init__(
         self,
         model:_t.model_type=None
         ) -> None:
         from volent.Model import Model as _model
         if isinstance(model,_model):
             self.model = model
         else:
-            if model is not None:
+            if isinstance(self.table_name,(str)):
+                mdl = _settings.globe.Volent.get_model(self.table_name)
+                if mdl is not None:
+                    self.model = mdl
+
+            elif model is not None:
                 md = model()
 
     #     self.from_dict(kwargs)
 
 
     @property
     def summary(self):
@@ -77,14 +85,40 @@
         value = {
             "name":self.name.snake_,
             "fields": [x.summary for x in self.fields],
         }
         return value
 
     @property
+    def table_name(self):
+        '''
+            Get this Schema's table_name
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-02-2024 12:30:25
+            `@memberOf`: Schema
+            `@property`: table_name
+        '''
+        value = self._table_name
+        if value is None:
+            value = None
+            keys = ["__table_name__","__tablename__"]
+            for key in keys:
+                if hasattr(self,key):
+                    value = getattr(self,key)
+                    break
+            self._table_name = value
+        return value
+
+    @property
     def schema_name(self)->str:
         '''
             Get this Schema's name
 
             `default`:None
 
 
@@ -197,14 +231,15 @@
             ----------
             `@author`: Colemen Atwood
             `@created`: 04-11-2023 14:07:35
             `@memberOf`: Model
             `@property`: fields
         '''
         value = self._fields
+        nested_fields = []
 
         if value is None:
             dif = self._unique_prop_keys
             # df_props = dir(Model(_is_root=False))
             # # # @Mstep [] gather the props of this instance.
             # props = dir(self)
             # # # @Mstep [] find the props that exist on this instance and not on the base.
@@ -380,14 +415,15 @@
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:44:07
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: get_field
             * @xxx [04-21-2023 07:44:52]: documentation for get_field
         '''
+        # print(f"Schema.get_field.name : {name}")
         name = c.string.to_snake_case(name)
         for field in self.fields:
             if field.name == name:
                 return field
         return None
 
     def from_dict(self,data:dict):
@@ -409,25 +445,37 @@
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: from_dict
             * @xxx [04-21-2023 07:48:45]: documentation for from_dict
         '''
 
         if isinstance(data,(dict)) is False:
-            raise TypeError(f"Data expects a dictionary, {type(data)} received.")
+            if c.types.is_list_of_dicts(data):
+                self.from_list_of_dicts(data)
+                return
+            else:
+                raise TypeError(f"from_dict expects a dictionary, {type(data)} received.")
 
         for col in self.model.columns:
-            if col not in data:
+            if col.name not in data:
                 continue
             field = self.get_field(col.name)
             if field is None:
                 continue
 
-            col.column_value = data[col]
+            # col.column_value = data[col.name]
+            col.value = data[col.name]
+        return self
 
+    def from_list_of_dicts(self,data:Iterable[dict])->_t.schema_type:
+        if c.types.is_list_of_dicts(data) is False:
+            raise TypeError(f"from_list_of_dicts expects a list of dictionaries, {type(data)} received.")
+        nm = self.__dicts_to_models(data)
+        if nm is None:
+            model = model if nm is None else nm
 
     def open_api_definition(self):
         '''
             Generate the open API definition for this schema.
 
             ----------
 
@@ -569,17 +617,49 @@
         if isinstance(model,(_model)) is True:
             out_data = self.__deserialize_model(mdl)
             if many:
                 out_data = c.arr.force_list(out_data)
             return out_data
     load = deserialized
 
+    def __dicts_to_models(self,data:Iterable[dict])->Union[Iterable[_t.model_type],None]:
+        '''
+            This will attempt to convert a list of dictionaries into a list of model instances.
+
+            Arguments
+            -------------------------
+            `data` {list}
+                A list of dictionaries to convert
+
+            Return {list}
+            ----------------------
+            A list of models if successful, None otherwise
 
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-02-2024 13:28:23
+            `memberOf`: Schema
+            `version`: 1.0
+            `method_name`: __dicts_to_models
+            * @xxx [04-02-2024 13:29:51]: documentation for __dicts_to_models
+        '''
+        from volent.Model import Model as _model
+        nm = []
+        if c.types.is_list_of_dicts(data):
+            if isinstance(self.model,_model) is True:
+                for mdl in data:
+                    nc = self.model.__class__
+                    n = nc(**mdl)
+                    nm.append(n)
+        if len(nm) == 0:
+            return None
+        return nm
 
-    def dump(self,model:_t.model_type=None,many=False,ignore_unprovided=False)->dict:
+    def dump(self,model:_t.model_type=None,many=False,ignore_unprovided=False)->Union[dict,Iterable[dict]]:
         '''Dump the contents of the model(s) using the fields to filter.'''
 
         if isinstance(model,(dict)):
             # print(f"dictionary provided for dumping.")
             data = self._correlate_to_dict(model,ignore_unprovided)
             self.__validate_dict(model)
             out_data = {}
@@ -605,19 +685,33 @@
 
 
         # print(f"model: {model}")
         if isinstance(model,(list)):
             # print(f"a list was provided for dumping.")
             result = []
             from volent.Model import Model as _model
+            nm = self.__dicts_to_models(model)
+            model = model if nm is None else nm
+            # nm = []
+            # if c.types.is_list_of_dicts(model):
+            #     if isinstance(self.model,_model) is True:
+            #         for mdl in model:
+            #             nc = self.model.__class__
+            #             n = nc(**mdl)
+            #             nm.append(n)
+            #         model = nm
+
             for mdl in model:
+
                 if isinstance(mdl,_model) is False:
                     c.con.log(f"The mdl is not an instance of model:{mdl}","magenta")
 
+
                 # mdl = model
+
                 self.model = mdl
                 self._correlate_to_columns()
                 self.__validate()
                 data = {}
                 for f in self.fields:
                     if hasattr(f.data_type_instance,"serializer"):
                         v = f.data_type_instance.serializer(f.value,f.name)
@@ -655,47 +749,74 @@
                     data[f.name] = v
                     continue
                 data[f.name] = f.value
         if many:
             data = c.arr.force_list(data)
         return data
 
-    def new(self)->_t.schema_type:
+    def new(self,data:dict=None)->_t.schema_type:
         '''
             Validate this schema's data and submit it to the model's table in the databse.
-            ----------
+
+
+            Arguments
+            ----------------------
+            `data` {dict,None}
+                A dictionary to populate the columns with.
+
+                This is the same as calling "schema.from_dict(data).new()
 
             Return {schema}
             ----------------------
             This schema instance.
 
+            Example
+            ---
+            ```
+                songData = {
+                    "title":f"{c.rand.abstract_name()}{c.rand.number()}",
+                    "artist":c.rand.abstract_name(),
+                    "lyrics":"bobs_borbers on my norblers.",
+                }
+
+                SongsNewSchema().new(songData)
+            ```
+
+
+
+
             Meta
             ----------
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:50:29
             `memberOf`: Schema
             `version`: 1.0
             `method_name`: new
             * @xxx [04-21-2023 07:51:43]: documentation for new
         '''
+        if data is not None:
+            if isinstance(data,(dict)) is False:
+                raise TypeError(f"Schema.new() expects the data argument to be a dictionary, {type(data).__name__} provided.")
+            else:
+                self.from_dict(data)
         # @Mstep [] correlate the fields to their columns in the model.
         self._correlate_to_columns()
         # @Mstep [] validate the schema fields.
         self.__validate()
 
         # data = {}
         # # @Mstep [LOOP] iterate this schema's fields
         # for f in self.fields:
         #     # @Mstep [IF] if the field is NOT dump_only
         #     if f.dump_only is False:
         #         # @Mstep [] add the field to the data dictionary.
         #         data[f.name] = f.value
 
         # @Mstep [] execute the insert on the model.
-        self.model.insert(self)
+        self.model.insert(self).execute()
         # @Mstep [RETURN] return this schema instance.
         return self
 
     def update(self)->_t.schema_type:
         self._correlate_to_columns()
         self.__validate()
         data = {}
@@ -807,15 +928,15 @@
 
 
         return out_data
 
     def _correlate_to_columns(self):
         '''
             Iterate all fields to find their corresponding columns in the current model.
-            ----------
+
 
             Meta
             ----------
             `author`: Colemen Atwood
             `created`: 04-21-2023 07:40:42
             `memberOf`: Schema
             `version`: 1.0
```

### Comparing `colemen_volent-0.1.7/volent/Trigger.py` & `colemen_volent-0.1.8/volent/Trigger.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/UniqueConstraint.py` & `colemen_volent-0.1.8/volent/UniqueConstraint.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/Volent.py` & `colemen_volent-0.1.8/volent/Volent.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,16 +547,18 @@
                     if force is True:
                         db.run(mdl.drop_statement)
                     db.run(mdl.create_statement,foreign_key_checks=False)
         if _settings.globe.flavor == "sqlite":
             for db in self.databases:
 
                 for mdl in db.models:
-                    print(f"creating table: {mdl.model_name}")
+                    # print(f"creating table: {mdl.model_name}")
                     if force is True:
                         db.run(mdl.drop_statement)
+                    # print(mdl.create_statement)
                     db.run(mdl.create_statement,foreign_key_checks=False)
+                    # print(f"\n\n")
 
 if __name__ == '__main__':
     m = Volent()
     m.master()
```

### Comparing `colemen_volent-0.1.7/volent/data_types/BigInt.py` & `colemen_volent-0.1.8/volent/data_types/BigInt.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/Bool.py` & `colemen_volent-0.1.8/volent/data_types/Bool.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/Decimal.py` & `colemen_volent-0.1.8/volent/data_types/Decimal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/EncodedPrimary.py` & `colemen_volent-0.1.8/volent/data_types/EncodedPrimary.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/Integer.py` & `colemen_volent-0.1.8/volent/data_types/Integer.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/String.py` & `colemen_volent-0.1.8/volent/data_types/String.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/TinyInt.py` & `colemen_volent-0.1.8/volent/data_types/TinyInt.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/data_types/TypeBase.py` & `colemen_volent-0.1.8/volent/data_types/TypeBase.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/exceptions.py` & `colemen_volent-0.1.8/volent/exceptions.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/mixins/DatabaseConnection.py` & `colemen_volent-0.1.8/volent/mixins/DatabaseConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         '''
 
         # if foreign_key_checks is False:
             # self.execute_single_statement("SET FOREIGN_KEY_CHECKS = 0;")
             # sql = f"SET FOREIGN_KEY_CHECKS = 0;\n{sql}\nSET FOREIGN_KEY_CHECKS = 0;"
         statements = sql
         success = False
-        print(f"executing: {sql}")
+        # print(f"executing: {sql}")
         # if the sql is a string, split it into a list of statements
         if isinstance(sql, (str)):
             statements = _to_statement_list(sql)
         # print(f"statements:{statements}")
         if len(statements) > 1:
             # print(f"Multiple statements [{len(statements)}] found in sql.")
             success = True
@@ -365,14 +365,88 @@
         # _log(f"args:{args}","cyan")
 
         if self.run(sql,args):
             return self.fetchall()
         return default
 
 
+    def run_select_internal(self,sql:str,select:_t.query_type,args=False,default=None,limit=None,offset=None):
+        '''
+            Execute a select query on the database.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `sql` {str}
+                The Select query to execute.
+
+            `args` {list,dict}
+                The arguments to use in parameterized placeholders
+
+            Keyword Arguments
+            -------------------------
+            [`default`=None] {any}
+                The default value to return in the event of an error.
+
+            [`limit`=None] {int}
+                The maximum number of results to return
+
+            [`offset`=None] {int}
+                The index offset to apply to the query.
+
+            Return {any}
+            ----------------------
+            The results of the query if successful, the default value otherwise.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 12-09-2022 11:12:16
+            `memberOf`: MySQLDatabase
+            `version`: 1.0
+            `method_name`: run_select
+            * @xxx [12-09-2022 11:15:35]: documentation for run_select
+        '''
+        # default = _obj.get_kwarg(['default'],None,None,**kwargs)
+        # limit = _obj.get_kwarg(['limit'],None,(int),**kwargs)
+        # offset = _obj.get_kwarg(['offset'],None,(int),**kwargs)
+
+        sql = _paginate_select_query(sql,limit,offset)
+        if isinstance(args,(dict)):
+            sql = _format_query_params(sql,args)
+        # print(f"sql:{sql}")
+        if self.is_connected is False:
+            c.con.log("Not Connected to a database dork.","warning")
+        # if self.connect() is False:
+            return default
+
+        # _log(f"sql:{sql}","cyan")
+        # _log(f"args:{args}","cyan")
+
+
+        self.cursor.row_factory = sqlite3.Row
+        if self.run(sql,args):
+            rows = self.cursor.fetchall()
+            # print(rows)
+            dicts = self._to_dict(rows)
+            return dicts
+            # contents = self.cursor.fetchall()
+            # print(f"selects: ")
+            # print(select._selects)
+            # print(contents)
+            # if len(select._selects) == 0:
+            #     out = []
+            #     for x in contents:
+                    
+                
+            return self.fetchall()
+        return default
+
+
 
     def close(self):
         '''
             Close the connection to the mySQL database.
 
             ----------
 
@@ -577,14 +651,26 @@
             `author`: Colemen Atwood
             `created`: 06-02-2022 13:58:55
             `memberOf`: DatabaseManager
             `version`: 1.0
             `method_name`: fetchall
             * @xxx [06-02-2022 13:59:37]: documentation for fetchall
         '''
+        # def dict_factory(cursor, row):
+        #     d = {}
+        #     for idx, col in enumerate(cursor.description):
+        #         d[col[0]] = row[idx]
+        #     return d
+        # return dict_factory(self.cursor,self.cursor.fetchall())
+        # colname = [ d[0] for d in query.description ]
+        # result_list = [ dict(zip(colname, r)) for r in query.fetchall() ]
+        
+        result = self.cursor.fetchall()
+        # print(f"fetchall::result : {result}")
+        return result
         return self._to_dict(self.cursor.fetchall())
 
     def fetchone(self):
         """ DOCBLOCK {
                 "class_name":"Database",
                 "method_name":"fetchone",
                 "author":"Colemen Atwood",
@@ -596,26 +682,27 @@
                     "description":"The result of the fetchone command"
                 }
             }"""
         r = self.cursor.fetchone()
         return r
 
     def _to_dict(self, result):
-        # print(f"_to_dict: resultType: {type(result)}")
-        if isinstance(result, list):
+        # print(f"_to_dict:resultType: {type(result)}")
+        # print(f"_to_dict:result : {result}")
+        if isinstance(result, (list)):
             new_data = []
             for row in result:
                 tmp = {}
                 # @Mstep [IF] if the row is a tuple
                 # this means its probably the response of the sqlite last insert id.
                 if isinstance(row,(tuple)):
                     if len(row) == 1:
                         row = row[0]
                     return row
-                # print(f"row:{row}")
+                # print(f"row:{row.keys()}")
                 for col in row.keys():
                     tmp[col] = row[col]
                 new_data.append(tmp)
             return new_data
         # if isinstance(result, sqlite3.Row):
         #     new_data = {}
         #     for col in result.keys():
```

### Comparing `colemen_volent-0.1.7/volent/mixins/EntityName.py` & `colemen_volent-0.1.8/volent/mixins/EntityName.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/mixins/MySQLGeneratorMixin.py` & `colemen_volent-0.1.8/volent/mixins/MySQLGeneratorMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/mixins/OrderedClass.py` & `colemen_volent-0.1.8/volent/mixins/OrderedClass.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/mixins/ReverseEngineerMixin.py` & `colemen_volent-0.1.8/volent/mixins/ReverseEngineerMixin.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/query/Delete.py` & `colemen_volent-0.1.8/volent/query/Delete.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/query/Insert.py` & `colemen_volent-0.1.8/volent/query/Insert.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,22 +152,27 @@
             `@memberOf`: Insert
             `@property`: _multi_query
         '''
 
         place_holders,data = self.placeholder_string
 
         template = f"""INSERT INTO {self.model.quoted_name} ({self.column_list_string}) VALUES {place_holders}"""
-
+        # print(f"==================================================================")
+        # print(data)
+        # print(f"==================================================================\n\n")
+        
         return (template,data)
 
     def _inserts_from_data(self):
+        # print(f"insert._inserts_from_data")
         data = self.data
         # @Mstep [IF] if the data is a list.
         if isinstance(data,(list)):
             self._is_multi = True
+            self._multi_inserts = []
 
 
             # @Mstep [LOOP] iterate the list of datas
             for d in data:
                 # @Mstep [IF] if the element is not a dictionary
                 if isinstance(d,(dict)) is False:
                     # @Mstep [] skip that shit.
@@ -180,41 +185,51 @@
                 if len(d.keys()) == 0:
                     # @Mstep [] skip this element.
                     continue
 
 
                 # @Mstep [loop] Iterate the items in the dict.
                 for k,v in d.items():
-                    self.__add_unique_coluumn(k)
+
                     # @Mstep [IF] if the value is not undefined.
                     if v != _t.undefined:
+                        self.__add_unique_coluumn(k)
                         # @Mstep [] add the key and value to the d_insert dict.
                         d_insert[k] = v
                 # @Mstep [LOOP] iterate the model columns.
                 for col in self.model.columns:
                     # @Mstep [IF] if thhe column has an on_insert value.
                     if col.on_insert != _t.undefined:
+                        # print(f"On insert column found : {col.name}")
                         # @Mstep [IF] if the column is not already being set.
                         if col.name not in d_insert:
                             # @Mstep [] set the key and value on d_insert.
                             d_insert[col.name] = col.on_insert
                             self.__add_unique_coluumn(col.name)
                 # @Mstep [] append the d_insert dictionary to self._multi_inserts.
                 self._multi_inserts.append(d_insert)
 
             # @Mstep [RETURN] return the _multi_inserts list.
             return self._multi_inserts
 
+
+
+
+
         data = self.filter_dict_by_columns(data)
+        # print(f"data: {data}")
         for k,v in data.items():
             if v != _t.undefined:
                 self.add_insert(k,v)
 
         for col in self.model.columns:
+            # print(f"col.on_insert: {col.on_insert}")
             if col.on_insert != _t.undefined:
+            # if isinstance(col.on_insert,(_t.undefined)) is False:
+                # print(f"On insert column found : {col.name}")
                 if col.name not in self._inserts:
                     self.add_insert(col.name,col.on_insert)
         return self._inserts
 
     def add_insert(self,column_name,value):
         self._inserts[column_name] = value
 
@@ -274,9 +289,9 @@
             result = self.model.select().is_(self.model.primary_column.name,result).execute()
         if result is True and return_result is False:
             result = self.database.last_id()
 
 
         # print(f"sql: {sql}")
         # print(f"args: {args}")
-        print(f"insert execute duration: {time() - start}")
+        # print(f"insert execute duration: {time() - start} : {result}")
         return result
```

### Comparing `colemen_volent-0.1.7/volent/query/Query.py` & `colemen_volent-0.1.8/volent/query/Query.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,26 +15,29 @@
     * @xxx [04-28-2023 07:04:34]: documentation for query
 '''
 
 
 
 from dataclasses import dataclass
 import re
+from select import select
 from typing import Iterable, Union
 from datetime import datetime
 from datetime import timezone
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
 import volent.settings as _settings
 # import volent.settings as _settings
 # from volent.Field import Field as _field
 from volent.mixins import OrderedClass
+from volent.query.WhereClause import WhereClause as _w
+from volent.query.QueryParam import QueryParam as _param
 
 
 @dataclass
 class Query(metaclass=OrderedClass):
     main = None
     # database:_t.database_type = None
     model:_t.model_type = None
@@ -47,14 +50,31 @@
 
     _selects:Iterable[str] = None
     _wheres:Iterable[str] = None
     _count:bool = False
     _average:bool = False
     _sum:bool = False
 
+    _where_clauses:Iterable[_t.where_clause_type] = None
+    _params:Iterable[_t.query_param_type] = None
+
+
+
+    _items_per_page:int=_settings.control.query.pagination.items_per_page
+    '''How many items should be shown per page when the query is paginated.
+
+    This directly corresponds to the "LIMIT" value.'''
+
+
+    _page_number:int=_settings.control.query.pagination.default_page_number
+    '''Which page of items should be returned.
+
+    This is used in conjunction with the items_per_page to calculate the "OFFSET" value.
+    '''
+
     def __init__(
         self,
         model:_t.model_type,
         data:dict=None,
         select_columns=None,
         update_columns=None
         ):
@@ -83,15 +103,17 @@
             `version`: 1.0
             `method_name`: query
             * @xxx [04-28-2023 07:07:59]: documentation for query
         '''
         self.model = model
         self.data = data
         self.database = model.database
+        self._params = []
         self._wheres = []
+        self._where_clauses = []
         self._selects = []
         self._updates = {}
 
         self.__parse_col_data(select_columns,update_columns)
         # else:
         #     for col in update_columns:
         #         if isinstance(col,(list,tuple)):
@@ -131,23 +153,26 @@
             `author`: Colemen Atwood
             `created`: 04-28-2023 07:08:04
             `memberOf`: Query
             `version`: 1.0
             `method_name`: __parse_col_data
             * @xxx [04-28-2023 07:10:20]: documentation for __parse_col_data
         '''
+        if isinstance(select_columns,(str)):
+            select_columns = c.arr.force_list(select_columns)
         if isinstance(select_columns,(list)):
             for col in select_columns:
                 if isinstance(col,(list,tuple)):
                     if len(col) >= 2:
                         name,alias = col
                         self.add_select(name,alias)
                     if len(col) == 1:
                         col = col[0]
                 if isinstance(col,(str)):
+                    # print(f"adding column by name: {col}")
                     self.add_select(col)
 
         if isinstance(update_columns,(dict)):
             mt_col = self.model.get_column("modified_timestamp")
             if mt_col is not None:
                 self.add_update("modified_timestamp",round(datetime.now(tz=timezone.utc).timestamp()))
 
@@ -165,14 +190,29 @@
                 # @Mstep [IF] if the column has an "on_update" value set.
                 if col.on_update != _t.undefined:
                     # @Mstep [IF] if the column is not already being updated.
                     if col.name not in self._updates:
                         # @Mstep [] add a new update clause to this query.
                         self.add_update(col.name,col.on_update)
 
+    @property
+    def items_per_page(self):
+        value = self._items_per_page
+        if value is None:
+            value = 100
+            self._items_per_page = value
+        return value
+
+    @items_per_page.setter
+    def items_per_page(self,value):
+        self._items_per_page = value
+
+
+
+
     def filter_dict_by_columns(self,data:dict)->dict:
         '''
             Iterate a dictionary to remove key's that do not have a corresponding column in this query's model
             ----------
 
             Arguments
             -------------------------
@@ -197,14 +237,23 @@
             col = self.model.get_column(k)
             if col is not None:
                 if v is None and col.nullable is False:
                     continue
                 output[k] = v
         return output
 
+    def filter_undefined_values(self,data:dict)->dict:
+        '''Iterate a dictionary to remove any undefined values'''
+        out = {}
+        for k,v in data.items():
+            if v == _t.undefined:
+                continue
+            out[k] = v
+        return out
+
     def sort_dict_by_columns(self,data:dict)->dict:
         '''
             Sort the keys of dictionary to match the order of columns in this query's model.
 
             This is primarily useful for parameterized insert statements, where the order of the columns
             is critical to inserting the correct data.
 
@@ -234,14 +283,75 @@
         output = {}
         for col in self.model.columns:
             if col.name in data:
                 output[col.name] = data[col.name]
         return output
 
 
+
+    @property
+    def where_count(self):
+        '''
+            Get this Query's where_count
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-01-2024 16:56:43
+            `@memberOf`: Query
+            `@property`: where_count
+        '''
+        return len(self._where_clauses)
+
+    # def add_where_obj(self,WhereClause:_t.where_clause_type):
+    #     self._where_clauses.append(WhereClause)
+
+
+    def add_param(self,key,value)->_t.query_param_type:
+        p = _param(self,key,value)
+        self._params.append(p)
+        return p
+
+    @property
+    def serialized_params(self)->dict:
+        '''
+            Get a dictionary of all params associated to this query.
+
+            The parameter names are serialized according to the flavor.
+
+            Return {dict}
+            ----------------------
+            The serialized param dictionary
+
+            Example
+            ----------------------
+            ```
+            {
+                "@track_number":34,
+                "@title":"AlienBiscuits"
+            }
+            ```
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-02-2024 09:44:08
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: serialized_params
+            * @xxx [04-02-2024 09:46:24]: documentation for serialized_params
+        '''
+        value = {}
+        for p in self._params:
+            value[p.name] = p.value
+        return value
+
     def add_where(self,column_name,value,comparison):
         '''
             Add a where clause to this query.
 
             ----------
 
             Arguments
@@ -262,63 +372,67 @@
             `author`: Colemen Atwood
             `created`: 04-28-2023 07:14:41
             `memberOf`: Query
             `version`: 1.0
             `method_name`: add_where
             * @xxx [04-28-2023 07:19:24]: documentation for add_where
         '''
-        if value is None:
-            value = "NULL"
-        # self.wheres.append(f"{column_name} {comparison} {value}")
-
-
-
-        if c.string.to_snake_case(comparison) in ["!","!=","isnt","isnot","is_not","<>"]:
-            comparison = "is not"
+        # if value is None:
+        #     value = "NULL"
+        # # self.wheres.append(f"{column_name} {comparison} {value}")
 
-        data = {
-            "column_name":column_name,
-            "comparison":comparison,
-            "value":value,
-            "max_value":None,
-        }
-
-        if c.string.to_snake_case(comparison) in ["match","full_text_search"]:
-            data['comparison'] = "match"
-            data['column_name'] = c.arr.force_list(column_name)
-
-        if c.string.to_snake_case(comparison) in ["between"]:
-            if isinstance(value,(list,tuple)):
-                data['value'] = value[0]
-                data['max_value'] = value[1]
-            else:
-                data['value'] = 0
-                data['max_value'] = value
-
-        if c.string.to_snake_case(comparison) in ["in"]:
-            value = c.arr.force_list(value)
-            if isinstance(value,(list,tuple)):
-                items = []
-                for idx,x in enumerate(value):
-                    if isinstance(x,(str)):
-                        # key = f"{column_name}_{idx}"
-                        # items[key] = f"'{x}'"
-                        items.append(x)
-
-
-                    if isinstance(x,(int,float)):
-                        # key = f"{column_name}_{idx}"
-                        items.append(f"{x}")
-                        # items[key] = f"{x}"
 
-                # str_list = ', '.join(items)
 
-                data['value'] = items
+        # if c.string.to_snake_case(comparison) in ["!","!=","isnt","isnot","is_not","<>"]:
+        #     comparison = "is not"
+
+        # data = {
+        #     "column_name":column_name,
+        #     "comparison":comparison,
+        #     "value":value,
+        #     "max_value":None,
+        # }
+
+        # if c.string.to_snake_case(comparison) in ["match","full_text_search"]:
+        #     data['comparison'] = "match"
+        #     data['column_name'] = c.arr.force_list(column_name)
+
+        # if c.string.to_snake_case(comparison) in ["between"]:
+        #     if isinstance(value,(list,tuple)):
+        #         data['value'] = value[0]
+        #         data['max_value'] = value[1]
+        #     else:
+        #         data['value'] = 0
+        #         data['max_value'] = value
+
+        # if c.string.to_snake_case(comparison) in ["in"]:
+        #     value = c.arr.force_list(value)
+        #     if isinstance(value,(list,tuple)):
+        #         items = []
+        #         for idx,x in enumerate(value):
+        #             if isinstance(x,(str)):
+        #                 # key = f"{column_name}_{idx}"
+        #                 # items[key] = f"'{x}'"
+        #                 items.append(x)
+
+
+        #             if isinstance(x,(int,float)):
+        #                 # key = f"{column_name}_{idx}"
+        #                 items.append(f"{x}")
+        #                 # items[key] = f"{x}"
+
+        #         # str_list = ', '.join(items)
+
+        #         data['value'] = items
+
+        # # self._wheres.append(data)
+        w = _w(self,column_name,value,comparison)
+        self._where_clauses.append(w)
+        return w
 
-        self._wheres.append(data)
 
 
     @property
     def where_string(self)->str:
         '''
             Generate this query's where string.
 
@@ -328,67 +442,24 @@
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 12-09-2022 15:45:29
             `@memberOf`: UpdateQuery
             `@property`: where_string
         '''
-        value = self._wheres
+        value = self._where_clauses
         # self._params = {}
-        if len(self._wheres) > 0:
+        if len(self._where_clauses) > 0:
             wheres = []
-            for where in self._wheres:
-                wcol = where['column_name']
-                wcomp = where['comparison']
-                wval = str(where['value'])
-                join_wcol = None
-
-                if self.has_joins is True:
-                    print(f"QUERY HAS WHERE STRING")
-                    col:_t.column_type = self.model.get_column(wcol)
-                    join_wcol = f"{self.model.quoted_name}.{col.quoted_name}"
-
-                if c.string.to_snake_case(wcomp) in ["match"]:
-                    col_name_list = ','.join(wcol)
-                    single_where = f"MATCH({col_name_list}) AGAINST('{wval}' IN NATURAL LANGUAGE MODE)"
-                    # single_where = f"{wcol} {wcomp.upper()} :{min_key} AND :{max_key}"
-                    # self._params[min_key] = where['value']
-                    # self._params[max_key] = where['max_value']
-
-                if c.string.to_snake_case(wcomp) in ["between"]:
-                    min_key =f"{wcol}_minimum"
-                    max_key =f"{wcol}_maximum"
-
-                    single_where = f"{wcol} {where['comparison'].upper()} :{min_key} AND :{max_key}"
-                    self._params[min_key] = where['value']
-                    self._params[max_key] = where['max_value']
-
-
-                elif c.string.to_snake_case(wcomp) in ["in","not_in"]:
-                    in_list = []
-                    for idx,val in enumerate(where['value']):
-                        key = f"{where['column_name']}_{idx}"
-                        self._params[key] = val
-                        in_list.append(f":{key}")
-                    in_list_string = ', '.join(in_list)
-                    single_where = f"{where['column_name']} {where['comparison'].upper()} ({in_list_string})"
-
-
-                # @Mstep [IF] if comparison matches [is,is not]
-                elif c.string.to_snake_case(wcomp) in ["is","is_not"]:
-                    # @Mstep [] generate the where string without applying a parameterized value.
-                    # This can cause issues with "IS NULL" type clauses, because those cannot be parameterized
-                    # single_where = f"{where['column_name']} {where['comparison'].upper()} {str(where['value'])}"
-                    single_where = f"{wcol} {wcomp} {wval}"
-                    # if wval.upper() == "NULL":
-                        # single_where = f"{wcol} {wcomp} {wval}"
-                    # params[where['column_name']] = where['value']
-                else:
-                    single_where = f"{join_wcol} {where['comparison']} :{where['column_name']}"
-                    self._params[wcol] = where['value']
+            for where in self._where_clauses:
+                if where.is_or_child is True:
+                    c.con.log(f"    Query.where_string : skipping or child: {where}","cyan")
+                    continue
+
+                single_where = where.where_string()
 
                 wheres.append(single_where)
             wheres = ' AND '.join(wheres)
             value = f" WHERE {wheres}"
         else:
             value = ""
         return value
@@ -455,15 +526,51 @@
             `memberOf`: QueryBase
             `version`: 1.0
             `method_name`: __paginate_select_query
             * @xxx [12-14-2022 11:46:12]: documentation for __paginate_select_query
         '''
         return _paginate_select_query(sql,self.limit,self.offset)
 
+    def copy_wheres(self,query:_t.query_type)->_t.query_type:
+        '''
+            Used to copy where clauses from one query to another
+
+            Arguments
+            -------------------------
+            `query` {Query}
+                The source query to copy where instances from.
+
+            Return {Query}
+            ----------------------
+            returns this query instance.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-02-2024 09:39:58
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: copy_wheres
+            * @xxx [04-02-2024 09:40:45]: documentation for copy_wheres
+        '''
+        wheres = query._where_clauses
+        for w in wheres:
+            column_name = w.column_name
+            value = w.value
+            max_value = w.max_value
+            comparison = w.comparison
+
+            if max_value is not None:
+                value = [value,max_value]
+            self.add_where(column_name=column_name,value=value,comparison=comparison)
+
+        return self
+
     def add_where_from_wheres(self,wheres:Iterable[dict]):
+        '''This is used to copy all where instances from one query to another.'''
         for w in wheres:
             column_name = w["column_name"]
             value = w["value"]
             max_value = w["max_value"]
             comparison = w["comparison"]
 
             if max_value is not None:
@@ -481,15 +588,60 @@
         if max_value is not None:
             value = [value,max_value]
 
         self.add_where(column_name,value,comparison)
 
         return self
 
+    def gather_wheres(self,where:_t.where_clause_type)->Iterable[_t.where_clause_type]:
+        print(f"Query.gather_wheres ===================================")
+        total_wheres = len(self._where_clauses)
+        occ = where.or_child_count
+        child_ids = range((total_wheres-1)-occ,total_wheres-1)
+        for cid in child_ids:
+            sw = self._where_clauses[cid]
+            sw.or_parent_id = where.or_parent_id
+            sw.is_or_child = True
+            print(sw)
+        print(f"Query.gather_wheres ===================================")
+
+    def get_wheres_by_or_id(self,or_id:str)->Iterable[_t.where_clause_type]:
+        out = []
+        for w in self._where_clauses:
+            if w.or_parent_id == or_id and w.is_or_child is True:
+                out.append(w)
+        return out
 
+    def set_on_update_values(self,data:dict)->dict:
+        '''
+        Assign key/value to an array when there is a column with an on_update value and the
+        key does not yet exist in the dict.
+        '''
+        out = data
+        for col in self.model.columns:
+            on_update = col.on_update
+            if on_update == _t.undefined:
+                continue
+
+            # @Mstep [] Filter out onUpdates that match a where clause column
+            skip = False
+            for w in self._where_clauses:
+                if w.column_name == col.name:
+                    skip = True
+                    break
+            if skip is True:
+                continue
+
+
+            if col.name not in out:
+                val = on_update
+                if callable(val):
+                    val = val()
+                out[col.name] = val
+        return out
 
 
 
 
 def format_null(value):
     '''
         convert a None value to a "null" string.
```

### Comparing `colemen_volent-0.1.7/volent/query/Select.py` & `colemen_volent-0.1.8/volent/query/Select.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
 
 
 from dataclasses import dataclass
+import re
 from typing import Iterable,OrderedDict, Union
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
@@ -22,18 +23,24 @@
 
 @dataclass
 class Select(Query,WhereMixin):
     def __init__(self,model:_t.model_type,columns=None,limit:int=100,offset:int=0) -> None:
         self._params = {}
         self._selects = []
         self._joins = []
-        self._limit = limit
-        self._offset = offset
+        # self._limit = limit
+        # self._offset = offset
 
         self.query_crud_type = "read"
+        if columns is None:
+            columns = model.columns
+        if isinstance(columns,(tuple)):
+            if len(columns) == 1:
+                columns = columns[0]
+        # print(f"Select.__init__.columns : {columns}")
         super().__init__(model,select_columns=columns)
 
     @property
     def has_joins(self):
         '''
             Get this Select's has_joins
 
@@ -47,59 +54,14 @@
             `@memberOf`: Select
             `@property`: has_joins
         '''
         if len(self._joins) > 0:
             return True
         return False
 
-    def paginate(self,limit,offset):
-        self.limit = limit
-        self.offset = offset
-        return self
-
-    @property
-    def limit(self):
-        return self._limit
-    @limit.setter
-    def limit(self,value:int):
-        '''
-            Set the Select's limit property
-
-            `default`:None
-
-
-            Meta
-            ----------
-            `@author`: Colemen Atwood
-            `@created`: 04-21-2023 10:14:11
-            `@memberOf`: Select
-            `@property`: limit
-        '''
-        self._limit = value
-
-    @property
-    def offset(self):
-        return self._offset
-    @offset.setter
-    def offset(self,value:int):
-        '''
-            Set the Select's offset property
-
-            `default`:None
-
-
-            Meta
-            ----------
-            `@author`: Colemen Atwood
-            `@created`: 04-21-2023 10:14:11
-            `@memberOf`: Select
-            `@property`: offset
-        '''
-        self._offset = value
-
     @property
     def select_string(self)->str:
         '''
             Get the compiled select string for this query.
 
             `default`:None
 
@@ -137,19 +99,19 @@
     @property
     def query(self):
 
         # print(f"self.select_string: {self.select_string}")
 
         value = f"""SELECT {self.select_string} FROM {self.model.quoted_name}{self.left_join_string}{self.where_string}"""
 
-        value = self._paginate_select_query(value)
-        value = self._format_query_params(value,self._params)
+        # value = self._paginate_select_query(value)
+        # value = self._format_query_params(value,self._params)
         # print(f"value: {value}")
         # print(f"self._params: {self._params}")
-        return value,self._params
+        return value,self.serialized_params
 
     def execute(self,return_models=True)->Union[bool,dict,int,_t.model_type]:
         '''
             Execute the select query on the table.
 
             ----------
 
@@ -182,21 +144,28 @@
         if sql is False:
             return False
 
         # print(f"sql:{sql}")
         # print(f"args:{args}")
         try:
             # @Mstep [] execute the insert query.
-            result = self.database.run_select(sql,args)
+
+            # result = self.database.run_select(sql,args)
+            result = self.database.run_select_internal(sql,self,args)
+
+            # print(f"result : {type(result)} : {result}")
             if return_models and result is not None:
                 models = []
+                # if isinstance(result[0],(tuple)) is False:
+                #     result = [result]
                 for r in result:
+                    # print(f"r : {r}")
                     mdl = self.model.__class__(**r)
                     mdl.__doc__ = self.model.__doc__
-                    mdl._name = self.model.name
+                    mdl._model_name = self.model._model_name
                     mdl._database_name = self.model._database_name
                     mdl._database = self.model._database
                     models.append(mdl)
                 return models
         except OperationalError as e:
             c.con.log(e,"red")
         except InterfaceError as e:
@@ -335,12 +304,72 @@
                 continue
             template = f""" {join['join_type']} JOIN {self.model.quoted_name}
     ON {self.model.quoted_name}.{join['column_name']} = {join['table_name']}.{join['column_name']}"""
             return template
         return ""
 
 
+    def paginate(self,page_number:int=1,per_page:int=None):
+        '''
+            update the pagination settings for this query.
+
+            Arguments
+            -------------------------
+            `page_number` {int} = 1
+                Which page of items to return
+
+                If set to 0, None or False the query will NOT be paginated.
+
+            `per_page` {int} = None
+                How many items per page should be shown.
+
+            Return {Select}
+            ----------------------
+            returns this select instance.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-02-2024 10:14:25
+            `memberOf`: Select
+            `version`: 1.0
+            `method_name`: paginate
+            * @xxx [04-02-2024 10:16:07]: documentation for paginate
+        '''
+        self._page_number = page_number
+        if per_page is not None:
+            self._items_per_page = per_page
+        return self
+
+    def _paginate_query(self,sql:str)->str:
+        page_number = self._page_number
+        per_page = self._items_per_page
+        offset = None if (page_number * per_page) < 1 else page_number * per_page
+        limit = per_page
+
+        if limit in [0,None,False]:
+            return sql
+
+        # @Mstep [] remove any trailing spaces and semicolons
+        sql = c.string.strip(sql,[";"," "],"right")
+        # @Mstep [] remove any already existing pagination strings.
+        sql = re.sub(r'limit\s*[0-9]*\s*(,|offset)\s*(:?[0-9\s]*)?',"",sql,re.MULTILINE | re.IGNORECASE)
+
+        limit_string = f"LIMIT {limit}"
+        offset_string = ""
+        if offset is not None:
+            offset_string = f"OFFSET {offset}"
+
+        paginate = f"{limit_string} {offset_string}"
+        sql = f"{sql} {paginate}"
+        return sql
+
+
+    def __repr__(self) -> str:
+        return f"<Select : {self.model.model_name}>"
+
+
 def format_null(value):
     if value is None:
         return "NULL"
     return value
```

### Comparing `colemen_volent-0.1.7/volent/query/WhereMixin.py` & `colemen_volent-0.1.8/volent/query/WhereMixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Iterable, Union
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
+from volent.query.WhereClause import WhereClause as _w
 # import volent.settings as _settings
 # from volent.Field import Field as _field
 # from volent.Relationship import Relationship as _relationship
 # from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 # from volent.query.Query import Query
 
 
@@ -54,15 +55,15 @@
         '''
         if value is None and ignore_nulls is True:
             return self
         if value == _t.no_default:
             return self
         value = format_null(value)
 
-        self.add_where(column_name=column_name,value=value,comparison="=")
+        self.add_where(column_name=column_name,value=value,comparison="is")
         return self
     is_ = equals
 
     def is_not(self,column_name:str,value)->_t.query_type:
         '''
             Add an "IS NOT" where clause to the query.
 
@@ -86,15 +87,15 @@
             `created`: 04-25-2023 11:16:43
             `memberOf`: WhereMixin
             `version`: 1.0
             `method_name`: equals
             * @xxx [04-25-2023 11:18:26]: documentation for equals
         '''
         value = format_null(value)
-        self.add_where(column_name=column_name,value=value,comparison="!=")
+        self.add_where(column_name=column_name,value=value,comparison="is_not")
         return self
     not_ = is_not
 
     def null(self,column_name:str)->_t.query_type:
         '''
             Add a "IS NULL" where clause to the query.
 
@@ -144,15 +145,15 @@
             `version`: 1.0
             `method_name`: equals
             * @xxx [04-25-2023 11:18:26]: documentation for equals
         '''
         self.add_where(column_name=column_name,value="NULL",comparison="IS NOT")
         return self
 
-    def in_(self,column_name:str,options:Iterable[str])->_t.query_type:
+    def in_(self,column_name:str,options:Iterable[Union[str,int,float]])->_t.query_type:
         '''
             Add an "IN" where clause to the query.
 
             ----------
 
             Arguments
             -------------------------
@@ -278,15 +279,15 @@
             `version`: 1.0
             `method_name`: greater_than
             * @xxx [04-25-2023 11:18:26]: documentation for greater_than
         '''
         if inclusive is True:
             self.greater_than_equal(column_name,value)
         else:
-            self.add_where(column_name,value,">")
+            self.add_where(column_name,value,"greater_than")
         return self
 
     def greater_than_equal(self,column_name:str,value:Union[int,float])->_t.query_type:
         '''
             Add a ">=" where clause to the query.
 
             ----------
@@ -308,15 +309,15 @@
             `author`: Colemen Atwood
             `created`: 04-25-2023 11:16:43
             `memberOf`: WhereMixin
             `version`: 1.0
             `method_name`: greater_than_equal
             * @xxx [04-25-2023 11:18:26]: documentation for greater_than_equal
         '''
-        self.add_where(column_name,value,">=")
+        self.add_where(column_name,value,"greater_than_equal")
         return self
 
     def less_than(self,column_name:str,value:Union[int,float],inclusive:bool=False)->_t.query_type:
         '''
             Add a "<" where clause to the query.
 
             ----------
@@ -345,15 +346,15 @@
             `version`: 1.0
             `method_name`: less_than
             * @xxx [04-25-2023 11:18:26]: documentation for less_than
         '''
         if inclusive is True:
             self.less_than_equal(column_name,value)
         else:
-            self.add_where(column_name,value,">")
+            self.add_where(column_name,value,"less_than")
         return self
 
     def less_than_equal(self,column_name:str,value:Union[int,float])->_t.query_type:
         '''
             Add a "<=" where clause to the query.
 
             ----------
@@ -375,15 +376,15 @@
             `author`: Colemen Atwood
             `created`: 04-25-2023 11:16:43
             `memberOf`: WhereMixin
             `version`: 1.0
             `method_name`: less_than
             * @xxx [04-25-2023 11:18:26]: documentation for less_than
         '''
-        self.add_where(column_name,value,">=")
+        self.add_where(column_name,value,"less_than_equal")
         return self
 
     def timestamps(self,column_name:str,start_timestamp:int=None,end_timestamp:int=None):
         '''
             Add a where clause used for filtering rows by dates.
 
             If both timestamps are provided only rows that are between will be returned.
@@ -428,14 +429,41 @@
         # @Mstep [] force the value to be a list of strings and remove any null values.
         value = c.arr.strip_list_nulls(c.arr.force_list(value))
         # @Mstep [] convert all values to strings.
         value = [str(x) for x in value]
         self.add_where(columns,value)
         return self
 
+    def like(self,column:Union[str,list,_t.column_type],value:str):
+        if isinstance(column,(list)) is False:
+            column = c.arr.force_list(column)
+        from volent.Column import Column as _column
+        columns = []
+        for col in column:
+            if isinstance(col,(str)):
+                co = self.model.get_column(col)
+                if co is not None:
+                    columns.append(co.name)
+            if isinstance(col,(_column)):
+                columns.append(col.name)
+        for col in columns:
+            self.add_where(col,value,"like")
+        return self
+
+
+
+    def or_(self,*or_children:_t.where_clause_type):
+        # print(or_children)
+        w = self.add_where(_t.undefined,[],"or")
+        w.or_child_count = len(or_children)
+        w.Query.gather_wheres(w)
+
+    
+
+
 
 def format_null(value):
     if value is None:
         return "NULL"
     return value
```

### Comparing `colemen_volent-0.1.7/volent/settings/control.py` & `colemen_volent-0.1.8/volent/settings/control.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 
 
 sql_quote_char:str = "`"
 '''The character to use for quoting strings in the sql output'''
 varchar_default_length:int = 50
 '''The default character length for varchar columns'''
 
+class query:
+    '''Settings which are applied to all queries'''
+
+    class pagination:
+        items_per_page:int = 100
+        default_page_number:int = 1
 
 # mysql_maximum_column_name_length:int = 64
 class mysql:
     '''MySQL specific settings'''
     create_table_indent:int = 4
     '''How many spaces to indent the contents of a create table statement'''
     safe_scripts:bool = True
```

### Comparing `colemen_volent-0.1.7/volent/settings/types.py` & `colemen_volent-0.1.8/volent/settings/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,22 +7,28 @@
 
 _main_type = None
 model_type = None
 database_type = None
 column_type = None
 type_base_type = None
 query_type = None
+where_clause_type = None
+query_param_type = None
 
 relationship_type = None
 schema_type = None
 field_type = None
 nested_field_type = None
 unique_constraint_type = None
 full_text_index_type = None
 
+insert_query_type = None
+select_query_type = None
+update_query_type = None
+delete_query_type = None
 
 
 if TYPE_CHECKING:
 
     from volent.Volent import Volent as _m
     _main_type = _TypeVar('_main_type', bound=_m)
 
@@ -32,20 +38,43 @@
     from volent.Model import Model as _HFem
     model_type = _TypeVar('model_type', bound=_HFem)
 
     from volent.Database import Database as _e8Ig
     database_type = _TypeVar('database_type', bound=_e8Ig)
 
 
+
+    from volent.query.Insert import Insert as _wyFSbRdHe6gB
+    insert_query_type = _TypeVar('insert_query_type', bound=_wyFSbRdHe6gB)
+
+    from volent.query.Select import Select as _YTxzOsQXPA2r
+    select_query_type = _TypeVar('select_query_type', bound=_YTxzOsQXPA2r)
+
+
+    from volent.query.Update import Update as _L1hIZD4YCbjF
+    update_query_type = _TypeVar('update_query_type', bound=_L1hIZD4YCbjF)
+
+    from volent.query.Delete import Delete as _FoUnRQwSOBhN
+    delete_query_type = _TypeVar('delete_query_type', bound=_FoUnRQwSOBhN)
+
+
+
     from volent.data_types.TypeBase import TypeBase as _NZwn
     type_base_type = _TypeVar('type_base_type', bound=_NZwn)
 
     from volent.Relationship import Relationship as _gt25
     relationship_type = _TypeVar('relationship_type', bound=_gt25)
 
+    from volent.query.WhereClause import WhereClause as _wqWn4l7D3AOh
+    where_clause_type = _TypeVar('where_clause_type', bound=_wqWn4l7D3AOh)
+
+
+    from volent.query.QueryParam import QueryParam as _MXvEFm2oA9Vp
+    query_param_type = _TypeVar('query_param_type', bound=_MXvEFm2oA9Vp)
+
 
     from volent.Schema import Schema as _gmhq
     schema_type = _TypeVar('schema_type', bound=_gmhq)
 
     from volent.Field import Field as _zoTC
     field_type = _TypeVar('field_type', bound=_zoTC)
```

### Comparing `colemen_volent-0.1.7/volent/tests/schema_dict_test.py` & `colemen_volent-0.1.8/volent/tests/schema_dict_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/tests/validators_test.py` & `colemen_volent-0.1.8/volent/tests/validators_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/CreditCardNumber.py` & `colemen_volent-0.1.8/volent/validate/CreditCardNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/Email.py` & `colemen_volent-0.1.8/volent/validate/Email.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/Equal.py` & `colemen_volent-0.1.8/volent/validate/Equal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/FutureUnixDate.py` & `colemen_volent-0.1.8/volent/validate/FutureUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/IpAddress.py` & `colemen_volent-0.1.8/volent/validate/IpAddress.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/Length.py` & `colemen_volent-0.1.8/volent/validate/Length.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/NoneOf.py` & `colemen_volent-0.1.8/volent/validate/NoneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/OneOf.py` & `colemen_volent-0.1.8/volent/validate/OneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/PastUnixDate.py` & `colemen_volent-0.1.8/volent/validate/PastUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/PhoneNumber.py` & `colemen_volent-0.1.8/volent/validate/PhoneNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/Range.py` & `colemen_volent-0.1.8/volent/validate/Range.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/Regex.py` & `colemen_volent-0.1.8/volent/validate/Regex.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/SocialSecurityNumber.py` & `colemen_volent-0.1.8/volent/validate/SocialSecurityNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/StrongPassword.py` & `colemen_volent-0.1.8/volent/validate/StrongPassword.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/Validator.py` & `colemen_volent-0.1.8/volent/validate/Validator.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.1.7/volent/validate/__init__.py` & `colemen_volent-0.1.8/volent/validate/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 from volent.validate.Validator import Validator
 from volent.validate.Length import Length
 from volent.validate.OneOf import OneOf,ContainsOnly
 from volent.validate.Email import Email
 from volent.validate.Equal import Equal
+from volent.validate.GreaterThan import GreaterThan
+from volent.validate.LessThan import LessThan
 from volent.validate.NoneOf import NoneOf
 from volent.validate.Range import Range
 from volent.validate.Regex import Regex
 from volent.validate.IpAddress import IpAddress
 from volent.validate.CreditCardNumber import CreditCardNumber
 from volent.validate.PhoneNumber import PhoneNumber
 from volent.validate.SocialSecurityNumber import SocialSecurityNumber
```

