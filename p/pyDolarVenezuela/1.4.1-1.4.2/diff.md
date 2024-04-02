# Comparing `tmp/pyDolarVenezuela-1.4.1.tar.gz` & `tmp/pyDolarVenezuela-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDolarVenezuela-1.4.1.tar", last modified: Thu Nov 23 16:45:52 2023, max compression
+gzip compressed data, was "pyDolarVenezuela-1.4.2.tar", last modified: Tue Apr  2 20:34:22 2024, max compression
```

## Comparing `pyDolarVenezuela-1.4.1.tar` & `pyDolarVenezuela-1.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.702899 pyDolarVenezuela-1.4.1/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pyDolarVenezuela-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     6232 2023-11-23 16:45:52.702899 pyDolarVenezuela-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3863 2023-11-22 14:41:37.000000 pyDolarVenezuela-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.636453 pyDolarVenezuela-1.4.1/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2158 2023-11-23 16:40:50.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.653900 pyDolarVenezuela-1.4.1/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.653900 pyDolarVenezuela-1.4.1/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/assets/icons/__init__.py
--rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      802 2023-11-22 00:44:52.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.690302 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     1271 2023-11-22 00:44:46.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     1934 2023-11-22 04:12:58.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2441 2023-11-23 16:39:39.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     1767 2023-11-22 04:13:37.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/dpedidos.py
--rw-rw-rw-   0        0        0     2849 2023-11-22 04:14:02.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     4031 2023-11-22 04:14:18.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/ivenezuela.py
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.702899 pyDolarVenezuela-1.4.1/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2023-10-15 01:58:15.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      615 2023-11-22 14:41:13.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2023-10-17 04:13:32.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-23 16:45:52.702899 pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     6232 2023-11-23 16:45:52.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      765 2023-11-23 16:45:52.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-23 16:45:52.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-11-23 16:45:52.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-11-23 16:45:52.000000 pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-11-23 16:40:42.000000 pyDolarVenezuela-1.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-23 16:45:52.702899 pyDolarVenezuela-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1472 2023-11-23 16:40:36.000000 pyDolarVenezuela-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:22.011117 pyDolarVenezuela-1.4.2/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pyDolarVenezuela-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     6232 2024-04-02 20:34:21.991657 pyDolarVenezuela-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3863 2024-04-02 19:50:04.000000 pyDolarVenezuela-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.874999 pyDolarVenezuela-1.4.2/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2453 2024-04-02 19:51:59.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.926782 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.926782 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/icons/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      802 2023-11-22 00:44:52.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.975021 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     1420 2024-04-02 19:36:45.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/dpedidos.py
+-rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/ivenezuela.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.991657 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.991657 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     6232 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-04-02 19:51:54.000000 pyDolarVenezuela-1.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 20:34:22.011117 pyDolarVenezuela-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1472 2024-04-02 19:51:50.000000 pyDolarVenezuela-1.4.2/setup.py
```

### Comparing `pyDolarVenezuela-1.4.1/LICENSE` & `pyDolarVenezuela-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/PKG-INFO` & `pyDolarVenezuela-1.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.1
+Version: 1.4.2
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pyDolarVenezuela-1.4.1/README.md` & `pyDolarVenezuela-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/__init__.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,56 @@
+import json
+from typing import Literal
+from colorama import Fore
+
 from . import network
 from .pages import Monitor as Page
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-import json
-from colorama import Fore
-
-version = '1.4.1'
+version = '1.4.2'
 
-def check_dependence_version():
-    response = network.get("https://pypi.org/pypi/pydolarvenezuela/json")
-    latest_version = json.loads(response)["info"]["version"]
+class CheckVersion:
+    check = True
 
-    if version != latest_version:
-        print(f"{Fore.GREEN}New version: {latest_version}.{Fore.RESET} {Fore.RED}Current version {version}.{Fore.RESET} write the following command: pip install --upgrade pyDolarVenezuela\n")
+    @classmethod
+    def _check_dependence_version(self):
+            response = network.get("https://pypi.org/pypi/pydolarvenezuela/json")
+            latest_version = json.loads(response)["info"]["version"]
 
-check_dependence_version()
+            if version != latest_version:
+                print(f"{Fore.GREEN}New version: {latest_version}.{Fore.RESET} {Fore.RED}Current version {version}.{Fore.RESET} write the following command: pip install --upgrade pyDolarVenezuela\n")
 
 class Monitor:
-    def __init__(self, provider: Page, currency: str = 'USD') -> None:
+    def __init__(self, provider: Page, currency: Literal['USD', 'EUR'] = 'USD') -> None:
         """
         La clase `Monitor` proporciona funcionalidades para consultar los precios de diversos monitores en Venezuela.
 
         Parámetros:
         - `provider`: La página de la que se accederán los datos.
         - `currency`: La moneda en la que se expresarán los precios. Puede ser `USD` o `EUR`. Por defecto es `USD`.
         """
+
+        if CheckVersion.check:
+            CheckVersion._check_dependence_version()
         if not isinstance(provider, Page):
             raise TypeError("The parameter must be an object of type Monitor.")
         
         self.provider = provider
         self.currency = currency.lower()
     
-    def get_value_monitors(self, monitor_code: str = None, name_property: str = None, prettify: bool = False):
+    def get_value_monitors(self, monitor_code: str = None, name_property: Literal['title', 'price', 'last_update'] = None, prettify: bool = False):
         """
         El método `get_value_monitors` permite acceder a los datos extraídos de los monitores.
 
         Parámetros:
         - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
         - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
         - `prettify`: Si es True, muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
         """ 
-        return select_monitor(self.provider, self.currency, monitor_code, name_property, prettify)
-
-__all__ = ['pages', 'currency_converter', 'getdate', 'Monitor']
+        return select_monitor(
+            self.provider,
+            currency=self.currency,
+            monitor_code=monitor_code,
+            name_property=name_property,
+            prettify=prettify
+        )
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/assets/icons/__init__.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/pages.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/__init__.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,24 +18,28 @@
     'eur': {
         B.name: BCV,
         C.name: CriptoDolar,
         E.name: ExchangeMonitor
     }
 }
 
-def select_monitor(provider: Monitor,
-                   currency: str,
-                   monitor_code: str,
-                   name_property: str,
-                   prettify: bool):
-    
+def select_monitor(provider: Monitor, **kwargs):
+    currency = kwargs.get('currency')
+    monitor_code = kwargs.get('monitor_code')
+    name_property = kwargs.get('name_property')
+    prettify = kwargs.get('prettify', False)
+
     if currency not in ['usd', 'eur']:
-        raise ValueError(f"The type must be 'usd' or 'eur' not {currency}")
+        raise ValueError(f"The currency type must be 'usd' or 'eur', not {currency}")
 
     try:
         monitor_class = monitor_classes.get(currency).get(provider.name)
         if monitor_class is not None:
-            return monitor_class(provider.provider, currency).get_values(monitor_code, name_property, prettify)
+            return monitor_class(provider.provider, currency).get_values(
+                monitor_code=monitor_code,
+                name_property=name_property, 
+                prettify=prettify
+            )
         else:
-            raise ValueError(f"Provider not supported")
+            raise ValueError("Provider not supported")
     except Exception as e:
         raise e
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/bcv.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/bcv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pyDolarVenezuela.utils import currencies
-
 import requests
 from bs4 import BeautifulSoup
 
+from ..utils import currencies
+
 requests.packages.urllib3.disable_warnings()
 
 def _get_rate_by_id(tag_id: str, soup: BeautifulSoup):
     return float(soup.find(id=tag_id).find("strong").text.strip().replace(',', '.'))
 
 def _get_time(soup: BeautifulSoup):
-    date = soup.find("span", "date-display-single")
-    return date.text.strip().replace('  ', ' ')
+    date = soup.find("span", "date-display-single").get('content')
+    return date.split('T')[0].replace('-', '/')
 
 class BCV:
     def __init__(self, url: str, currency: str) -> None:
         response      = requests.get(url, verify=False)
         response.raise_for_status()
 
         self.soup     = BeautifulSoup(response.content, 'html.parser')
@@ -29,21 +29,27 @@
         for code, values in currencies.items():
             self.rates[code] = {
                 "title": values['name'],
                 "price": round(_get_rate_by_id(values['id'], section_tipo_de_cambio_oficial), 2),
                 "price_old": _get_rate_by_id(values['id'], section_tipo_de_cambio_oficial)
             }
 
-    def get_values(self, currency_code: str, name_property: str, prettify: bool):
+    def get_values(self, **kwargs):
+        currency_code = kwargs.get('monitor_code')
+        name_property = kwargs.get('name_property')
+        prettify = kwargs.get('prettify', False)
+        
         self._load()
 
         if not currency_code:
             return self.rates
         
         try:
             monitor_data = self.rates[currency_code.lower()]
             if name_property:
+                if name_property == 'last_update':
+                    return self.rates['last_update']
                 value = monitor_data[name_property]
                 return f'Bs. {value}' if prettify and name_property == 'price' else value
             return monitor_data
         except KeyError:
             raise KeyError("Does not match any of the properties that were provided in the dictionary. Most information: https://github.com/fcoagz/pyDolarVenezuela")
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/criptodolar.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/criptodolar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from pyDolarVenezuela import network
-from pyDolarVenezuela.tools import time
-
 import json
+from .. import network
+from ..tools import time
 
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
 
@@ -35,15 +34,19 @@
                     'price_old': monitor['priceOld'],
                     'type': 'bank' if monitor['type'] == 'bancove' else 'monitor',
                     'last_update': time.get_time_standard(monitor['updatedAt']),
                 }
 
                 self.data[_convert_specific_format(data['title'])] = data
     
-    def get_values(self, monitor_code: str, name_property: str, prettify: bool):
+    def get_values(self, **kwargs):
+        monitor_code = kwargs.get('monitor_code')
+        name_property = kwargs.get('name_property')
+        prettify = kwargs.get('prettify', False)
+        
         self._load()
 
         if not monitor_code:
             return self.data
         
         try:
             monitor_data = self.data[monitor_code.lower()]
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/dpedidos.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/dpedidos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from pyDolarVenezuela import network
-from pyDolarVenezuela.tools import time
-from pyDolarVenezuela.utils import monitors
-
 import json
 
+from .. import network
+from ..tools import time
+from ..utils import monitors
+
 class Dpedidos:
     def __init__(self, url: str, currency: str) -> None:
         response           = network.get(url + 'minmaxhistorial')
         json_response      = json.loads(response)
 
         self.json_response = json_response['result'][0]
         self.currency      = currency
     
-    def get_values(self, monitor_code: str, name_property: str, prettify: bool):
+    def get_values(self, **kwargs):
+        monitor_code = kwargs.get('monitor_code')
+        name_property = kwargs.get('name_property')
+        prettify = kwargs.get('prettify', False)
+        
         result = {}
 
         for key, title in monitors.items():
             if key in self.json_response and self.json_response[key] not in ['0', None]:
                 data = {
                     'title': title,
                     'price': round(float(self.json_response[key]), 2)
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/exchangemonitor.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from bs4 import BeautifulSoup
+
 from .. import network
 from ..tools import time
 
-from bs4 import BeautifulSoup
-
 def _convert_specific_format(text: str, character: str = '_') -> str:
     acentos = {'á': 'a', 'é': 'e', 'í': 'i', 'ó': 'o', 'ú': 'u'}
     for acento, sin_acento in acentos.items():
         text = text.lower().replace(acento, sin_acento).replace(' ', character)
     return text
 
 def _get_values_monitors(soup: BeautifulSoup):
@@ -28,14 +28,15 @@
 
             name  = result.find("h6", "nombre").text
             price = str(result.find('p', "precio").text).replace(',', '.')
 
             if price.count('.') == 2:
                 price = price.replace('.', '', 1)
 
+            price = float(price)
             last_update = time.get_formatted_time(' '.join(str(result.find('p', "fecha").text).split(' ')[1:]).capitalize())
             symbol = str(result.find('p', "cambio-por").text)[0] if not str(result.find('p', "cambio-por").text)[0] == ' ' else ''
             color  = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
             percent = str(result.find('p', "cambio-por").text)[1:].strip()
             change = str(result.find('p', "cambio-num").text)
 
             data = {
@@ -46,15 +47,19 @@
                 'change': change,
                 'color': color,
                 'symbol': symbol
             }
 
             self.data[_convert_specific_format(name)] = data
     
-    def get_values(self, monitor_code: str, name_property: str, prettify: bool):
+    def get_values(self, **kwargs):
+        monitor_code = kwargs.get('monitor_code')
+        name_property = kwargs.get('name_property')
+        prettify = kwargs.get('prettify', False)
+        
         self._load()
 
         if not monitor_code:
             return self.data
         
         try:
             monitor_data = self.data[monitor_code.lower()]
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/provider/ivenezuela.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/ivenezuela.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyDolarVenezuela import network
+from .. import network
 from bs4 import BeautifulSoup
 
 endpoint = 'venezuela/dolar/precio-dolar-venezuela-{0}-{1}-{2}-{3}-oficial-bcv-paralelo-monitor-dolartoday/'
 
 def _get_price_and_symbol_in_simple(strong_tag: BeautifulSoup):
     price = str(strong_tag.find_next('strong').text).split('Bs.')[-1][:-1].strip()
     symbol = str(strong_tag.find_next('strong').text).split('Bs.')[-1][-1]
@@ -81,15 +81,19 @@
                 date_words.pop(2)
 
                 href = self.url + endpoint.format(*date_words)
 
                 self.data = _get_values_monitors(href)
                 self.data['date'] = ' '.join(date_words)
     
-    def get_values(self, monitor_code: str, name_property: str, prettify: bool):
+    def get_values(self, **kwargs):
+        monitor_code = kwargs.get('monitor_code')
+        name_property = kwargs.get('name_property')
+        prettify = kwargs.get('prettify', False)
+        
         self._load()
 
         if not monitor_code:
             return self.data
         
         try:
             monitor_data = self.data[monitor_code.lower()]
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/tools/calculator.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/calculator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-def currency_converter(type: str, value, monitor: dict):
+from typing import Literal
+
+def currency_converter(type: Literal['VES', 'USD', 'EUR'], value, monitor: dict):
     """
     Convierte una cantidad de dinero de una moneda a otra utilizando los datos de un monitor específico.
     """
     price_monitor = monitor['price']
 
     try:
         if isinstance(value, int) or isinstance(value, float):
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/tools/time.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela/utils.py` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/PKG-INFO` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.1
+Version: 1.4.2
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pyDolarVenezuela-1.4.1/pyDolarVenezuela.egg-info/SOURCES.txt` & `pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.1/pyproject.toml` & `pyDolarVenezuela-1.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.4.1"
+version = "1.4.2"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pyDolarVenezuela-1.4.1/setup.py` & `pyDolarVenezuela-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.4.1'
+VERSION = '1.4.2'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

