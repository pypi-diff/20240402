# Comparing `tmp/hltv_async_api-0.2.5.tar.gz` & `tmp/hltv_async_api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.2.5.tar", last modified: Tue Apr  2 15:09:24 2024, max compression
+gzip compressed data, was "hltv_async_api-0.2.6.tar", last modified: Tue Apr  2 17:26:40 2024, max compression
```

## Comparing `hltv_async_api-0.2.5.tar` & `hltv_async_api-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:09:24.531181 hltv_async_api-0.2.5/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     2449 2024-04-02 15:09:24.521569 hltv_async_api-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1826 2024-04-02 15:07:09.000000 hltv_async_api-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 15:09:24.241148 hltv_async_api-0.2.5/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:09:19.000000 hltv_async_api-0.2.5/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    24390 2024-04-02 15:05:31.000000 hltv_async_api-0.2.5/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:09:24.517824 hltv_async_api-0.2.5/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     2449 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 15:09:23.000000 hltv_async_api-0.2.5/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-02 15:09:19.000000 hltv_async_api-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 15:09:24.533713 hltv_async_api-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-02 15:09:19.000000 hltv_async_api-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:26:40.955364 hltv_async_api-0.2.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     2449 2024-04-02 17:26:40.953362 hltv_async_api-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1826 2024-04-02 15:07:09.000000 hltv_async_api-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 17:26:40.834812 hltv_async_api-0.2.6/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-02 16:33:09.000000 hltv_async_api-0.2.6/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    26016 2024-04-02 17:25:02.000000 hltv_async_api-0.2.6/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 17:26:40.951363 hltv_async_api-0.2.6/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     2449 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-02 16:33:09.000000 hltv_async_api-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 17:26:40.955364 hltv_async_api-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-02 16:33:09.000000 hltv_async_api-0.2.6/setup.py
```

### Comparing `hltv_async_api-0.2.5/LICENSE` & `hltv_async_api-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.5/PKG-INFO` & `hltv_async_api-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.5
+Version: 0.2.6
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.2.5/README.md` & `hltv_async_api-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.5/hltv_async_api/aiohltv.py` & `hltv_async_api-0.2.6/hltv_async_api/aiohltv.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,16 +82,16 @@
                 new_proxy = file.readline().strip()
                 if new_proxy:
                     proxy = new_proxy
 
         else:
             proxy = self.PROXY_LIST[0]
 
-        if self.PROXY_PROTOCOL not in proxy and proxy != '':
-            proxy = self.PROXY_PROTOCOL + '://' + proxy
+        if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
+       	    proxy = self.PROXY_PROTOCOL + '://' + proxy
 
         return proxy
 
     async def switch_proxy(self, proxy):
         if self.PROXY_PATH:
             if self.PROXY_PROTOCOL:
                 proxy = proxy.replace(self.PROXY_PROTOCOL + '://', '')
@@ -209,26 +209,68 @@
             teams = [line.getText() for line in live_matches.find_all("div", {'class', "matchTeamName text-ellipsis"})]
             matches = [(team1, team2) for team1, team2 in tuple(zip(teams, teams[1:]))[::2]]
             liveMatchContainer = live_matches.find_all("div", {'class', "liveMatch-container"})
             maps = [str(line.get('data-maps')).split(',') for line in liveMatchContainer]
             stars = [line.get('stars') for line in liveMatchContainer]
             return [{'teams': teams, 'maps': maps, 'stars': stars} for teams, maps, stars in zip(matches, maps, stars)]
 
-    async def get_upcoming_matches(self):
+    async def get_upcoming_matches(self, days: int = 7, star_rating: int = 1):
         """returns a list of all upcoming matches on HLTV"""
         r = await self.fetch("https://www.hltv.org/matches")
-        if not r:
-            return
+        if not r:return
+
+        matches = []
         try:
-            teams = [line.getText() for line in r.find("div",
-                                                       {'class', "upcomingMatchesContainer"}).find_all(
-                class_=lambda v: v is not None and (v == "team text-ellipsis" or v == "matchTeamName text-ellipsis"))]
+
+            days = 7
+            for i, date_div in enumerate(r.find_all('div', {'class': 'upcomingMatchesSection'}), start=1):
+                if i > days:
+                    break
+                date_ = date_div.find('span', {'class': 'matchDayHeadline'}).text.split()[-1]
+                matches_today = []
+
+                for match in date_div.find_all('div', {'class': 'upcomingMatch'}):
+                    time_ = match.find('div', {'class': 'matchTime'}).text
+                    rating = int(match['stars'])
+                    if rating >= star_rating:
+                        maps = match.find('div', {'class': 'matchMeta'}).text[-1:]
+                        try:
+                            teams = match.find_all('div', {'class': 'matchTeamName text-ellipsis'})
+
+                            team1 = teams[0].text
+                            team2 = teams[1].text
+                        except (IndexError, AttributeError):
+                            team1 = 'TBD'
+                            team2 = 'TBD'
+
+                        try:
+                            event = match.find('div', {'class', 'matchEventName gtSmartphone-only'}).text
+                        except AttributeError:
+
+                            try:
+                                event = match.find('span', {'class': 'line-clamp-3'}).text
+                            except AttributeError:
+                                event = ''
+
+                        matches_today.append({
+                            'team1': team1,
+                            'team2': team2,
+                            'time': time_,
+                            'maps': maps,
+                            'rating': rating,
+                            'event': event
+                    })
+
+                matches.append({
+                    'date': date_,
+                    'matches': matches_today
+                })
         except AttributeError:
             return None
-        return [(team1, team2) for team1, team2 in tuple(zip(teams, teams[1:]))[::2]]
+        return matches
 
     async def get_important_upcoming_matches(self, star_rating=1):
         """returns a list of all upcoming matches on HLTV with the star rating argument (should be between 0 and 5)"""
         r = await self.fetch("https://www.hltv.org/matches")
         if not r:
             return
 
@@ -593,12 +635,12 @@
     # TODO WRITE
     async def get_last_news(self):
         return []
 
 
 async def test():
     hltv = Hltv()
-    print(await hltv.get_event_info(7148, 'pgl-cs2-major-copenhagen-2024'))
+    print(await hltv.get_upcoming_matches())
 
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.2.5/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.2.6/hltv_async_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.2.5
+Version: 0.2.6
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.2.5/pyproject.toml` & `hltv_async_api-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.2.5/setup.py` & `hltv_async_api-0.2.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.2.5',
+    version='0.2.6',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

