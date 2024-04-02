# Comparing `tmp/cerc-persistence-1.0.0.1.tar.gz` & `tmp/cerc-persistence-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerc-persistence-1.0.0.1.tar", last modified: Tue Mar 26 05:49:06 2024, max compression
+gzip compressed data, was "cerc-persistence-1.0.0.2.tar", last modified: Tue Apr  2 07:33:29 2024, max compression
```

## Comparing `cerc-persistence-1.0.0.1.tar` & `cerc-persistence-1.0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1052 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/PKG-INFO
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2493 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/README.md
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/cerc_persistence/
--rw-r--r--   0 jenkins    (103) jenkins    (111)       29 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1941 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/configuration.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     9212 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/db_control.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     2951 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/db_setup.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/cerc_persistence/models/
--rw-r--r--   0 jenkins    (103) jenkins    (111)      203 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/models/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1041 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/models/application.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1276 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/models/city.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3099 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/models/city_object.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1218 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/models/simulation_results.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1130 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/models/user.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/cerc_persistence/repositories/
--rw-r--r--   0 jenkins    (103) jenkins    (111)       29 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repositories/__init__.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     3780 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repositories/application.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     4661 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repositories/city.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7792 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repositories/city_object.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     7276 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repositories/simulation_results.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)     5412 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repositories/user.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)      696 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/repository.py
--rw-r--r--   0 jenkins    (103) jenkins    (111)       64 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/cerc_persistence/version.py
-drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/cerc_persistence.egg-info/
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1052 2024-03-26 05:49:06.000000 cerc-persistence-1.0.0.1/cerc_persistence.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (103) jenkins    (111)      915 2024-03-26 05:49:06.000000 cerc-persistence-1.0.0.1/cerc_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)        1 2024-03-26 05:49:06.000000 cerc-persistence-1.0.0.1/cerc_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)       86 2024-03-26 05:49:06.000000 cerc-persistence-1.0.0.1/cerc_persistence.egg-info/requires.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)       17 2024-03-26 05:49:06.000000 cerc-persistence-1.0.0.1/cerc_persistence.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)      177 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/pyproject.toml
--rw-r--r--   0 jenkins    (103) jenkins    (111)       74 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/requirements.txt
--rw-r--r--   0 jenkins    (103) jenkins    (111)       38 2024-03-26 05:49:06.810294 cerc-persistence-1.0.0.1/setup.cfg
--rw-r--r--   0 jenkins    (103) jenkins    (111)     1717 2024-03-26 05:48:06.000000 cerc-persistence-1.0.0.1/setup.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-02 07:33:29.678137 cerc-persistence-1.0.0.2/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1052 2024-04-02 07:33:29.678137 cerc-persistence-1.0.0.2/PKG-INFO
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2493 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/README.md
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-02 07:33:29.674137 cerc-persistence-1.0.0.2/cerc_persistence/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       29 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1770 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/configuration.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     9221 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/db_control.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     2580 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/db_setup.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-02 07:33:29.678137 cerc-persistence-1.0.0.2/cerc_persistence/models/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      203 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/models/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1026 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/models/application.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1265 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/models/city.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3083 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/models/city_object.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1209 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/models/simulation_results.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1116 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/models/user.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-02 07:33:29.678137 cerc-persistence-1.0.0.2/cerc_persistence/repositories/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       29 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repositories/__init__.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     3731 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repositories/application.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     4612 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repositories/city.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7742 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repositories/city_object.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     7226 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repositories/simulation_results.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     5368 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repositories/user.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      696 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/repository.py
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       64 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/cerc_persistence/version.py
+drwxr-xr-x   0 jenkins    (103) jenkins    (111)        0 2024-04-02 07:33:29.678137 cerc-persistence-1.0.0.2/cerc_persistence.egg-info/
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1052 2024-04-02 07:33:29.000000 cerc-persistence-1.0.0.2/cerc_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      915 2024-04-02 07:33:29.000000 cerc-persistence-1.0.0.2/cerc_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)        1 2024-04-02 07:33:29.000000 cerc-persistence-1.0.0.2/cerc_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       86 2024-04-02 07:33:29.000000 cerc-persistence-1.0.0.2/cerc_persistence.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       17 2024-04-02 07:33:29.000000 cerc-persistence-1.0.0.2/cerc_persistence.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)      177 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/pyproject.toml
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       74 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/requirements.txt
+-rw-r--r--   0 jenkins    (103) jenkins    (111)       38 2024-04-02 07:33:29.678137 cerc-persistence-1.0.0.2/setup.cfg
+-rw-r--r--   0 jenkins    (103) jenkins    (111)     1717 2024-04-02 07:32:29.000000 cerc-persistence-1.0.0.2/setup.py
```

### Comparing `cerc-persistence-1.0.0.1/PKG-INFO` & `cerc-persistence-1.0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-persistence
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: CERC Persistence consist of a set of classes to store and retrieve Cerc Hub cities and results
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pathlib
 Requires-Dist: python-dotenv
 Requires-Dist: SQLAlchemy
```

### Comparing `cerc-persistence-1.0.0.1/README.md` & `cerc-persistence-1.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/configuration.py` & `cerc-persistence-1.0.0.2/cerc_persistence/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,14 @@
 
 class Configuration:
   """
   Configuration class to hold common persistence configuration
   """
 
   def __init__(self, db_name: str, dotenv_path: str, app_env='TEST'):
-    """
-    :param db_name: database name
-    :param app_env: application environment, test or production
-    :param dotenv_path: the absolute path to dotenv file
-    """
     try:
       # load environmental variables
       if not Path(dotenv_path).exists():
         error_message = f'dotenv file doesn\'t exists at {dotenv_path}'
         logging.error(error_message)
         raise FileNotFoundError(error_message)
       load_dotenv(dotenv_path=dotenv_path)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/db_control.py` & `cerc-persistence-1.0.0.2/cerc_persistence/db_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,35 +144,35 @@
     :param user_id: User who create the city
     return identity_id
     """
     return self._city.insert(city, pickle_path, scenario,  application_id, user_id)
 
   def update_city(self, city_id, city):
     """
-   Update an existing city in the database
-   :param city_id: the id of the city to update
-   :param city: the updated city object
+    Update an existing city in the database
+    :param city_id: the id of the city to update
+    :param city: the updated city object
     """
     return self._city.update(city_id, city)
 
   def persist_application(self, name: str, description: str, application_uuid: str):
     """
     Creates information for an application in the database
-   :param name: name of application
-   :param description: the description of the application
-   :param application_uuid: the uuid of the application to be created
+    :param name: name of application
+    :param description: the description of the application
+    :param application_uuid: the uuid of the application to be created
     """
     return self._application.insert(name, description, application_uuid)
 
   def update_application(self, name: str, description: str, application_uuid: str):
     """
     Update the application information stored in the database
-   :param name: name of application
-   :param description: the description of the application
-   :param application_uuid: the uuid of the application to be created
+    :param name: name of application
+    :param description: the description of the application
+    :param application_uuid: the uuid of the application to be created
     """
     return self._application.update(application_uuid, name, description)
 
   def add_simulation_results(self, name, values, city_id=None, city_object_id=None):
     """
     Add simulation results to the city or to the city_object to the database
     :param name: simulation and simulation engine name
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/db_setup.py` & `cerc-persistence-1.0.0.2/cerc_persistence/db_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,22 +19,14 @@
 
 class DBSetup:
   """
   Creates a Persistence database structure
   """
 
   def __init__(self, db_name, app_env, dotenv_path, admin_password, application_uuid):
-    """
-    Creates database tables a default admin user and a default admin app with the given password and uuid
-    :param db_name: database name
-    :param app_env: application environment type [TEST|PROD]
-    :param dotenv_path: .env file path
-    :param admin_password: administrator password for the application uuid
-    :application_uuid: application uuid
-    """
     repository = Repository(db_name=db_name, app_env=app_env, dotenv_path=dotenv_path)
 
     # Create the tables using the models
     Application.__table__.create(bind=repository.engine, checkfirst=True)
     User.__table__.create(bind=repository.engine, checkfirst=True)
     City.__table__.create(bind=repository.engine, checkfirst=True)
     CityObject.__table__.create(bind=repository.engine, checkfirst=True)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/models/application.py` & `cerc-persistence-1.0.0.2/cerc_persistence/models/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from sqlalchemy.dialects.postgresql import UUID
 
 from cerc_persistence.configuration import Models
 
 
 class Application(Models):
   """
-  A model representation of an application
+  Application(Models) class
   """
   __tablename__ = 'application'
   id = Column(Integer, Sequence('application_id_seq'), primary_key=True)
   name = Column(String, nullable=False)
   description = Column(String, nullable=False)
   application_uuid = Column(UUID(as_uuid=True), nullable=False)
   created = Column(DateTime, default=datetime.datetime.utcnow)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/models/city.py` & `cerc-persistence-1.0.0.2/cerc_persistence/models/city.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from sqlalchemy import Column, Integer, String, Sequence, ForeignKey
 from sqlalchemy import DateTime
 
 from cerc_persistence.configuration import Models
 
 
 class City(Models):
-  """A model representation of a city
+  """
+  City(Models) class
   """
   __tablename__ = 'city'
   id = Column(Integer, Sequence('city_id_seq'), primary_key=True)
   pickle_path = Column(String, nullable=False)
   name = Column(String, nullable=False)
   scenario = Column(String, nullable=False)
   application_id = Column(Integer, ForeignKey('application.id', ondelete='CASCADE'), nullable=False)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/models/city_object.py` & `cerc-persistence-1.0.0.2/cerc_persistence/models/city_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from hub.city_model_structure.building import Building
 from cerc_persistence.configuration import Models
 
 
 class CityObject(Models):
   """
-  A model representation of an application
+  CityObject(Models) class
   """
   __tablename__ = 'city_object'
   id = Column(Integer, Sequence('city_object_id_seq'), primary_key=True)
   city_id = Column(Integer, ForeignKey('city.id', ondelete='CASCADE'), nullable=False)
   name = Column(String, nullable=False)
   aliases = Column(String, nullable=True)
   type = Column(String, nullable=False)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/models/simulation_results.py` & `cerc-persistence-1.0.0.2/cerc_persistence/models/simulation_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sqlalchemy import DateTime
 from sqlalchemy.dialects.postgresql import JSONB
 from cerc_persistence.configuration import Models
 
 
 class SimulationResults(Models):
   """
-  A model representation of an application
+  SimulationResults(Models) class
   """
   __tablename__ = 'simulation_results'
   id = Column(Integer, Sequence('simulation_results_id_seq'), primary_key=True)
   city_id = Column(Integer, ForeignKey('city.id', ondelete='CASCADE'), nullable=True)
   city_object_id = Column(Integer, ForeignKey('city_object.id', ondelete='CASCADE'), nullable=True)
   name = Column(String, nullable=False)
   values = Column(JSONB, nullable=False)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/models/user.py` & `cerc-persistence-1.0.0.2/cerc_persistence/models/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   """
   Admin = 'Admin'
   Hub_Reader = 'Hub_Reader'
 
 
 class User(Models):
   """
-  A model representation of a city
+  User(Models) class
   """
   __tablename__ = 'user'
   id = Column(Integer, Sequence('user_id_seq'), primary_key=True)
   name = Column(String, nullable=False)
   password = Column(String, nullable=False)
   role = Column(Enum(UserRoles), nullable=False, default=UserRoles.Hub_Reader)
   application_id = Column(Integer, nullable=False)
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/repositories/application.py` & `cerc-persistence-1.0.0.2/cerc_persistence/repositories/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,22 @@
 
 from cerc_persistence.repository import Repository
 from cerc_persistence.models import Application as Model
 
 
 class Application(Repository):
   """
-  Application repository
+  Application(Repository) class
   """
   _instance = None
 
   def __init__(self, db_name: str, dotenv_path: str, app_env: str):
     super().__init__(db_name, dotenv_path, app_env)
 
   def __new__(cls, db_name, dotenv_path, app_env):
-    """
-    Implemented for a singleton pattern
-    """
     if cls._instance is None:
       cls._instance = super(Application, cls).__new__(cls)
     return cls._instance
 
   def insert(self, name: str, description: str, application_uuid: str):
     """
     Inserts a new application
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/repositories/city.py` & `cerc-persistence-1.0.0.2/cerc_persistence/repositories/city.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,22 @@
 from cerc_persistence.repository import Repository
 from cerc_persistence.models import City as Model
 from cerc_persistence.models import CityObject
 
 
 class City(Repository):
   """
-  City repository
+  City(Repository) class
   """
   _instance = None
 
   def __init__(self, db_name: str, dotenv_path: str, app_env: str):
     super().__init__(db_name, dotenv_path, app_env)
 
   def __new__(cls, db_name, dotenv_path, app_env):
-    """
-    Implemented for a singleton pattern
-    """
     if cls._instance is None:
       cls._instance = super(City, cls).__new__(cls)
     return cls._instance
 
   def insert(self, city: CityHub, pickle_path, scenario, application_id, user_id: int):
     """
     Inserts a city
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/repositories/city_object.py` & `cerc-persistence-1.0.0.2/cerc_persistence/repositories/city_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 
 from cerc_persistence.models import CityObject as Model
 from cerc_persistence.repository import Repository
 
 
 class CityObject(Repository):
   """
-  City object repository
+  CityObject(Repository) class
   """
   _instance = None
 
   def __init__(self, db_name: str, dotenv_path: str, app_env: str):
     super().__init__(db_name, dotenv_path, app_env)
 
   def __new__(cls, db_name, dotenv_path, app_env):
-    """
-    Implemented for a singleton pattern
-    """
     if cls._instance is None:
       cls._instance = super(CityObject, cls).__new__(cls)
     return cls._instance
 
   def insert(self, city_id: int, building: Building):
     """
     Inserts a new city object
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/repositories/simulation_results.py` & `cerc-persistence-1.0.0.2/cerc_persistence/repositories/simulation_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,22 @@
 from cerc_persistence.models import City
 from cerc_persistence.models import CityObject
 from cerc_persistence.models import SimulationResults as Model
 
 
 class SimulationResults(Repository):
   """
-  Simulation results repository
+  SimulationResults(Repository) class
   """
   _instance = None
 
   def __init__(self, db_name: str, dotenv_path: str, app_env: str):
     super().__init__(db_name, dotenv_path, app_env)
 
   def __new__(cls, db_name, dotenv_path, app_env):
-    """
-    Implemented for a singleton pattern
-    """
     if cls._instance is None:
       cls._instance = super(SimulationResults, cls).__new__(cls)
     return cls._instance
 
   def insert(self, name: str, values: str, city_id=None, city_object_id=None):
     """
     Inserts simulations results linked either with a city as a whole or with a city object
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/repositories/user.py` & `cerc-persistence-1.0.0.2/cerc_persistence/repositories/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,22 @@
 from hub.helpers.auth import Auth
 from cerc_persistence.repository import Repository
 from cerc_persistence.models import User as Model, Application as ApplicationModel, UserRoles
 
 
 class User(Repository):
   """
-  User class
+  User(Repository) class
   """
   _instance = None
 
   def __init__(self, db_name: str, dotenv_path: str, app_env: str):
     super().__init__(db_name, dotenv_path, app_env)
 
   def __new__(cls, db_name, dotenv_path, app_env):
-    """
-    Implemented for a singleton pattern
-    """
     if cls._instance is None:
       cls._instance = super(User, cls).__new__(cls)
     return cls._instance
 
   def insert(self, name: str, password: str, role: UserRoles, application_id: int):
     """
     Inserts a new user
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence/repository.py` & `cerc-persistence-1.0.0.2/cerc_persistence/repository.py`

 * *Files identical despite different names*

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence.egg-info/PKG-INFO` & `cerc-persistence-1.0.0.2/cerc_persistence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-persistence
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: CERC Persistence consist of a set of classes to store and retrieve Cerc Hub cities and results
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pathlib
 Requires-Dist: python-dotenv
 Requires-Dist: SQLAlchemy
```

### Comparing `cerc-persistence-1.0.0.1/cerc_persistence.egg-info/SOURCES.txt` & `cerc-persistence-1.0.0.2/cerc_persistence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-persistence-1.0.0.1/setup.py` & `cerc-persistence-1.0.0.2/setup.py`

 * *Files identical despite different names*

